# Comparing `tmp/sqlfluff-2.0.3.tar.gz` & `tmp/sqlfluff-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-9gznxqhz/sqlfluff-2.0.3.tar", last modified: Wed Apr  5 17:26:58 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-yzhiwodd/sqlfluff-2.0.4.tar", last modified: Fri Apr 14 09:56:03 2023, max compression
```

## Comparing `sqlfluff-2.0.3.tar` & `sqlfluff-2.0.4.tar`

### file list

```diff
@@ -1,259 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)   366970 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    43460 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50049 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34642 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72624 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61143 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28434 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126330 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68381 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    99588 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80229 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   153055 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36571 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69113 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   201286 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)    95369 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    28498 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172212 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31286 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    89479 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23166 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25468 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:26:58.000000 sqlfluff-2.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-05 17:26:43.000000 sqlfluff-2.0.3/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)   376240 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50049 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34648 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28534 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130072 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68391 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99588 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80857 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170049 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200667 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28498 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89741 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/test/test_testing.py
```

### Comparing `sqlfluff-2.0.3/CHANGELOG.md` & `sqlfluff-2.0.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,90 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.0.4] - 2023-04-14
+
+## Highlights
+
+This is primarily a _bugfix_ and _dialect_ release:
+* Several bugfixes related to templating and indentation, in particular some
+  improvements to the indentation of aliases and window functions.
+* Performance improvements to the parser.
+* The `--persist-timing` option is now also available on `sqlfluff fix`.
+* A refresh to getting started and rule documentation.
+* Dialect improvements to PostgreSQL, Athena, SparkSQL, MySQL & Snowflake.
+
+Thanks also to [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+and [@Thashin](https://github.com/Thashin) who made their first contributions
+in this release. In particular, [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+made **twenty one** contributions in their first month! 🎉🎉🎉
+
+## What’s Changed
+
+* SparkSQL: Improvements to lateral view, hints, sort by [#4731](https://github.com/sqlfluff/sqlfluff/pull/4731) [@bmorck](https://github.com/bmorck)
+* Add ExpressionSegment to CREATE TABLE ... DEFAULT / Fix multiple parse issues in Expression_A_Grammar [#4717](https://github.com/sqlfluff/sqlfluff/pull/4717) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add support for the PG VACUUM statement [#4742](https://github.com/sqlfluff/sqlfluff/pull/4742) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Simplify and fix PG array accessor segment & support expressions [#4748](https://github.com/sqlfluff/sqlfluff/pull/4748) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* SparkSQL: Allow for any ordering of create table clauses [#4721](https://github.com/sqlfluff/sqlfluff/pull/4721) [@bmorck](https://github.com/bmorck)
+* Suggested started config file [#4702](https://github.com/sqlfluff/sqlfluff/pull/4702) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Indents on window functions [#4560](https://github.com/sqlfluff/sqlfluff/pull/4560) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* SparkSQL: Fix Group By Clause [#4732](https://github.com/sqlfluff/sqlfluff/pull/4732) [@bmorck](https://github.com/bmorck)
+* Improve support for EXCLUDE table constraints in PG [#4725](https://github.com/sqlfluff/sqlfluff/pull/4725) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add support for dropping multiple indexes in PG [#4737](https://github.com/sqlfluff/sqlfluff/pull/4737) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Recognize "on" value and integers for PG SET statement [#4740](https://github.com/sqlfluff/sqlfluff/pull/4740) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Improve interval expressions on MySQL [#4746](https://github.com/sqlfluff/sqlfluff/pull/4746) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Keep out zero length keywords [#4723](https://github.com/sqlfluff/sqlfluff/pull/4723) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add PG support for CREATE SCHEMA AUTHORIZATION [#4735](https://github.com/sqlfluff/sqlfluff/pull/4735) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add support for dropping multiple views with PostgreSQL [#4736](https://github.com/sqlfluff/sqlfluff/pull/4736) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add CHAR VARYING data type for PG [#4738](https://github.com/sqlfluff/sqlfluff/pull/4738) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* fix(athena): map type matching failed, array type only contains a datatype [#4739](https://github.com/sqlfluff/sqlfluff/pull/4739) [@timcosta](https://github.com/timcosta)
+* Allow DML queries to be selectable in CTEs on PG [#4741](https://github.com/sqlfluff/sqlfluff/pull/4741) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add the CREATE/DROP CAST statements to ANSI and PG [#4744](https://github.com/sqlfluff/sqlfluff/pull/4744) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add support for PG SET ROLE / RESET ROLE [#4734](https://github.com/sqlfluff/sqlfluff/pull/4734) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Support Spark Iceberg DDL [#4690](https://github.com/sqlfluff/sqlfluff/pull/4690) [@bmorck](https://github.com/bmorck)
+* Fix #4680 [#4707](https://github.com/sqlfluff/sqlfluff/pull/4707) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Indent Aliases [#4706](https://github.com/sqlfluff/sqlfluff/pull/4706) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* SparkSQL: Improve window frame bounds [#4722](https://github.com/sqlfluff/sqlfluff/pull/4722) [@bmorck](https://github.com/bmorck)
+* Add support for PG CREATE/ALTER/DROP PUBLICATION stmts [#4716](https://github.com/sqlfluff/sqlfluff/pull/4716) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* SparkSQL: Create external table support [#4692](https://github.com/sqlfluff/sqlfluff/pull/4692) [@bmorck](https://github.com/bmorck)
+* SparkSQL: Fix file literal lexing [#4718](https://github.com/sqlfluff/sqlfluff/pull/4718) [@bmorck](https://github.com/bmorck)
+* Add PG DROP/REASSIGN OWNED statements [#4720](https://github.com/sqlfluff/sqlfluff/pull/4720) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* SparkSQL: Add distinct to comparison operator [#4719](https://github.com/sqlfluff/sqlfluff/pull/4719) [@bmorck](https://github.com/bmorck)
+* Rethink Rule Docs [#4695](https://github.com/sqlfluff/sqlfluff/pull/4695) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Performance: Reduce calls to _prune_options [#4705](https://github.com/sqlfluff/sqlfluff/pull/4705) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Snowflake: Add ReferencedVariableNameSegment to sample function [#4712](https://github.com/sqlfluff/sqlfluff/pull/4712) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Mark AM02 as fix compatible [#4714](https://github.com/sqlfluff/sqlfluff/pull/4714) [@yoichi](https://github.com/yoichi)
+* Fix LT01 spacing check in templated areas [#4698](https://github.com/sqlfluff/sqlfluff/pull/4698) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Don't do newline conversion on write [#4703](https://github.com/sqlfluff/sqlfluff/pull/4703) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* MySQL: CREATE/ALTER VIEW may take UNION [#4713](https://github.com/sqlfluff/sqlfluff/pull/4713) [@yoichi](https://github.com/yoichi)
+* Preserve zero-length template segments [#4708](https://github.com/sqlfluff/sqlfluff/pull/4708) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* CV06: don't flag files that don't have code [#4709](https://github.com/sqlfluff/sqlfluff/pull/4709) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Add a no-output option [#4704](https://github.com/sqlfluff/sqlfluff/pull/4704) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Jinja templater: treat "import" and "from" as templated [#4696](https://github.com/sqlfluff/sqlfluff/pull/4696) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Capitalization rules ignore templated code only if configured to [#4697](https://github.com/sqlfluff/sqlfluff/pull/4697) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Update getting started docs [#4700](https://github.com/sqlfluff/sqlfluff/pull/4700) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Add a default for config_keywords and remove noisy error. [#4701](https://github.com/sqlfluff/sqlfluff/pull/4701) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Snowflake Select System Functions [#4687](https://github.com/sqlfluff/sqlfluff/pull/4687) [@Thashin](https://github.com/Thashin)
+* SparkSQL: Add using and options clause to create view statement [#4691](https://github.com/sqlfluff/sqlfluff/pull/4691) [@bmorck](https://github.com/bmorck)
+* MySQL: Add RETURN Statement [#4693](https://github.com/sqlfluff/sqlfluff/pull/4693) [@yoichi](https://github.com/yoichi)
+* Safety valve for fixes in CV03 [#4685](https://github.com/sqlfluff/sqlfluff/pull/4685) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Allow persist timing on `fix` too. [#4679](https://github.com/sqlfluff/sqlfluff/pull/4679) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* fix{dialect-snowflake}:Alter Table Column Set/Unset Tag [#4682](https://github.com/sqlfluff/sqlfluff/pull/4682) [@Thashin](https://github.com/Thashin)
+* fix{dialect-snowflake}:Execute Task [#4683](https://github.com/sqlfluff/sqlfluff/pull/4683) [@Thashin](https://github.com/Thashin)
+* Make version number an argument not an option in release script. [#4677](https://github.com/sqlfluff/sqlfluff/pull/4677) [@alanmcruickshank](https://github.com/alanmcruickshank)
+
+
+## New Contributors
+* [@Thashin](https://github.com/Thashin) made their first contribution in [#4683](https://github.com/sqlfluff/sqlfluff/pull/4683)
+* [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack) made their first contribution in [#4697](https://github.com/sqlfluff/sqlfluff/pull/4697)
+
 ## [2.0.3] - 2023-04-05
 
 ## Highlights
 
 This is primarily a _bugfix_ and _dialect_ release:
 * Several bugfixes related to templating and indentation.
 * Configurable indentation before `THEN` in `CASE` statements
```

### Comparing `sqlfluff-2.0.3/LICENSE.md` & `sqlfluff-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/PKG-INFO` & `sqlfluff-2.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.3
+Version: 2.0.4
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.3/README.md` & `sqlfluff-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/setup.cfg` & `sqlfluff-2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.0.3
+version = 2.0.4
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
-stable_version = 2.0.3
+stable_version = 2.0.4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/api/simple.py` & `sqlfluff-2.0.4/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/commands.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,24 @@
         "--disable_progress_bar",
         "--disable-progress-bar",
         is_flag=True,
         help="Disables progress bars.",
         cls=DeprecatedOption,
         deprecated=["--disable_progress_bar"],
     )(f)
+    f = click.option(
+        "--persist-timing",
+        default=None,
+        help=(
+            "A filename to persist the timing information for a linting run to "
+            "in csv format for external analysis. NOTE: This feature should be "
+            "treated as beta, and the format of the csv file may change in "
+            "future releases without warning."
+        ),
+    )(f)
     return f
 
 
 def get_config(
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     **kwargs,
@@ -522,39 +532,29 @@
     ),
 )
 @click.option(
     "--disregard-sqlfluffignores",
     is_flag=True,
     help="Perform the operation regardless of .sqlfluffignore configurations",
 )
-@click.option(
-    "--persist-timing",
-    default=None,
-    help=(
-        "A filename to persist the timing information for a linting run to "
-        "in csv format for external analysis. NOTE: This feature should be "
-        "treated as beta, and the format of the csv file may change in "
-        "future releases without warning."
-    ),
-)
 @click.argument("paths", nargs=-1, type=click.Path(allow_dash=True))
 def lint(
     paths: Tuple[str],
     format: str,
     write_output: Optional[str],
     annotation_level: str,
     nofail: bool,
     disregard_sqlfluffignores: bool,
     logger: Optional[logging.Logger] = None,
     bench: bool = False,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
+    persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
-    persist_timing: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Lint SQL files via passing a list of files or using stdin.
 
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
@@ -612,14 +612,16 @@
     if verbose >= 1 and not non_human_output:
         click.echo(formatter.format_linting_stats(result, verbose=verbose))
 
     if format == FormatType.json.value:
         file_output = json.dumps(result.as_records())
     elif format == FormatType.yaml.value:
         file_output = yaml.dump(result.as_records(), sort_keys=False)
+    elif format == FormatType.none.value:
+        file_output = ""
     elif format == FormatType.github_annotation.value:
         if annotation_level == "error":
             annotation_level = "failure"
 
         github_result = []
         for record in result.as_records():
             filepath = record["filepath"]
@@ -755,14 +757,15 @@
     processes,
     fix_even_unparsable,
     force,
     fixed_suffix,
     bench,
     show_lint_violations,
     warn_force: bool = True,
+    persist_timing: Optional[str] = None,
 ):
     """Handle fixing from paths."""
     # Lint the paths (not with the fix argument at this stage), outputting as we go.
     click.echo("==== finding fixable violations ====")
     exit_code = EXIT_SUCCESS
 
     with PathAndUserErrorHandler(formatter):
@@ -858,14 +861,17 @@
         sorted_files = sorted(all_results.keys())
         for file in sorted_files:
             violations = all_results.get(file, [])
             click.echo(formatter.format_filename(file, success=(not violations)))
             for violation in violations:
                 click.echo(formatter.format_violation(violation))
 
+    if persist_timing:
+        result.persist_timing_records(persist_timing)
+
     sys.exit(exit_code)
 
 
 @cli.command(cls=DeprecatedOptionsCommand)
 @common_options
 @core_options
 @lint_options
@@ -907,14 +913,15 @@
     force: bool,
     paths: Tuple[str],
     bench: bool = False,
     fixed_suffix: str = "",
     logger: Optional[logging.Logger] = None,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
+    persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     show_lint_violations: bool = False,
     **kwargs,
 ) -> None:
     """Fix SQL files.
 
@@ -958,14 +965,15 @@
             paths,
             processes,
             fix_even_unparsable,
             force,
             fixed_suffix,
             bench,
             show_lint_violations,
+            persist_timing=persist_timing,
         )
 
 
 @cli.command(name="format", cls=DeprecatedOptionsCommand)
 @common_options
 @core_options
 @lint_options
@@ -979,14 +987,15 @@
 def cli_format(
     paths: Tuple[str],
     bench: bool = False,
     fixed_suffix: str = "",
     logger: Optional[logging.Logger] = None,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
+    persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     **kwargs,
 ) -> None:
     """Autoformat SQL files.
 
     This effectively force applies `sqlfluff fix` with a known subset of fairly
@@ -1055,14 +1064,15 @@
             processes,
             fix_even_unparsable=False,
             force=True,  # Always force in format mode.
             fixed_suffix=fixed_suffix,
             bench=bench,
             show_lint_violations=False,
             warn_force=False,  # don't warn about being in force mode.
+            persist_timing=persist_timing,
         )
 
 
 def quoted_presenter(dumper, data):
     """Re-presenter which always double quotes string values needing escapes."""
     if "\n" in data or "\t" in data or "'" in data:
         return dumper.represent_scalar("tag:yaml.org,2002:str", data, style='"')
@@ -1097,14 +1107,15 @@
     "--format",
     default=FormatType.human.value,
     type=click.Choice(
         [
             FormatType.human.value,
             FormatType.json.value,
             FormatType.yaml.value,
+            FormatType.none.value,
         ],
         case_sensitive=False,
     ),
     help="What format to return the parse result in.",
 )
 @click.option(
     "--write-output",
@@ -1227,14 +1238,16 @@
         if format == FormatType.yaml.value:
             # For yaml dumping always dump double quoted strings if they contain
             # tabs or newlines.
             yaml.add_representer(str, quoted_presenter)
             file_output = yaml.dump(parsed_strings_dict, sort_keys=False)
         elif format == FormatType.json.value:
             file_output = json.dumps(parsed_strings_dict)
+        elif format == FormatType.none.value:
+            file_output = ""
 
         # Dump the output to stdout or to file as appropriate.
         dump_file_payload(write_output, file_output)
     if profiler:
         pr.disable()
         profiler_buffer = StringIO()
         ps = pstats.Stats(pr, stream=profiler_buffer).sort_stats("cumulative")
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.0.4/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/config.py` & `sqlfluff-2.0.4/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.0.4/src/sqlfluff/core/default_config.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,17 @@
 
 [sqlfluff:layout:type:numeric_literal]
 spacing_within = touch:inline
 
 [sqlfluff:layout:type:sign_indicator]
 spacing_after = touch:inline
 
+[sqlfluff:layout:type:tilde]
+spacing_after = touch:inline
+
 [sqlfluff:layout:type:function_name]
 spacing_within = touch:inline
 spacing_after = touch:inline
 
 [sqlfluff:layout:type:array_type]
 spacing_within = touch:inline
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.0.4/src/sqlfluff/core/dialects/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,22 @@
         dialect objects to create some of the bulk-produced rules.
 
         """
         if label not in self._sets:
             self._sets[label] = set()
         return self._sets[label]
 
+    def update_keywords_set_from_multiline_string(
+        self, set_label: str, values: str
+    ) -> None:
+        """Special function to update a keywords set from a multi-line string."""
+        self.sets(set_label).update(
+            [n.strip().upper() for n in values.strip().split("\n")]
+        )
+
     def copy_as(self, name):
         """Copy this dialect and create a new one with a different name.
 
         This is the primary method for inheritance, after which, the
         `replace` method can be used to override particular rules.
         """
         # Are we already expanded?
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.0.4/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/errors.py` & `sqlfluff-2.0.4/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,14 +586,15 @@
         else:
             if stat.S_ISREG(status.st_mode):
                 mode = stat.S_IMODE(status.st_mode)
         dirname, basename = os.path.split(output_path)
         with tempfile.NamedTemporaryFile(
             mode="w",
             encoding=encoding,
+            newline="",  # NOTE: No newline conversion. Write as read.
             prefix=basename,
             dir=dirname,
             suffix=os.path.splitext(output_path)[1],
             delete=False,
         ) as tmp:
             tmp.file.write(write_buff)
             tmp.flush()
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.0.4/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files 9% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         # to return earlier if we can.
         # `segments` may already be nested so we need to break out
         # the raw segments within it.
         available_options = self._prune_options(segments, parse_context=parse_context)
 
         # If we've pruned all the options, return unmatched (with some logging).
         if not available_options:
-            return MatchResult.from_unmatched(segments)
+            return MatchResult.from_unmatched(segments), None
 
         with parse_context.deeper_match() as ctx:
             match, matched_option = self._longest_trimmed_match(
                 segments,
                 available_options,
                 parse_context=ctx,
                 trim_noncode=False,
@@ -190,16 +190,15 @@
 
         # Match on each of the options
         matched_segments: MatchResult = MatchResult.from_empty()
         unmatched_segments: Tuple[BaseSegment, ...] = segments
         n_matches = 0
 
         # Keep track of the number of times each option has been matched.
-        available_options = self._prune_options(segments, parse_context=parse_context)
-        available_option_counter = {str(o): 0 for o in available_options}
+        option_counter = {elem.cache_key(): 0 for elem in self._elements}
 
         while True:
             if self.max_times and n_matches >= self.max_times:
                 # We've matched as many times as we can
                 return MatchResult(
                     matched_segments.matched_segments, unmatched_segments
                 )
@@ -224,25 +223,26 @@
                 pre_seg = ()  # empty tuple
 
             match, matched_option = self._match_once(
                 unmatched_segments, parse_context=parse_context
             )
 
             # Increment counter for matched option.
-            if matched_option and (str(matched_option) in available_option_counter):
-                available_option_counter[str(matched_option)] += 1
-                # Check if we have matched an option too many times.
-                if (
-                    self.max_times_per_element
-                    and available_option_counter[str(matched_option)]
-                    > self.max_times_per_element
-                ):
-                    return MatchResult(
-                        matched_segments.matched_segments, unmatched_segments
-                    )
+            if matched_option:
+                matched_key = matched_option.cache_key()
+                if matched_option.cache_key() in option_counter:
+                    option_counter[matched_key] += 1
+                    # Check if we have matched an option too many times.
+                    if (
+                        self.max_times_per_element
+                        and option_counter[matched_key] > self.max_times_per_element
+                    ):
+                        return MatchResult(
+                            matched_segments.matched_segments, unmatched_segments
+                        )
 
             if match:
                 matched_segments += pre_seg + match.matched_segments
                 unmatched_segments = match.unmatched_segments
                 n_matches += 1
             else:
                 # If we get here, then we've not managed to match. And the next
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,24 +430,23 @@
                     source_str=placeholder_str,
                     block_type="skipped_source",
                 )
 
         # Move on
         return
 
-    # We've got a zero slice. This could be a block, unrendered templates
-    # or unrendered code (either because of loops of consumption).
-    if not is_zero_slice(tfs.source_slice):
-        yield TemplateSegment.from_slice(
-            tfs.source_slice,
-            tfs.templated_slice,
-            tfs.slice_type,
-            templated_file,
-        )
-    return
+    # Always return the slice, even if the source slice was also zero length.  Some
+    # templaters might want to pass through totally zero length slices as a way of
+    # marking locations in the middle of templated output.
+    yield TemplateSegment.from_slice(
+        tfs.source_slice,
+        tfs.templated_slice,
+        tfs.slice_type,
+        templated_file,
+    )
 
 
 def _iter_segments(
     lexed_elements: List[TemplateElement],
     templated_file_slices: List[TemplatedFileSlice],
     templated_file: TemplatedFile,
     add_indents: bool = True,
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,19 +82,21 @@
 class PathStep:
     """An element of the response to BaseSegment.path_to().
 
     Attributes:
         segment (:obj:`BaseSegment`): The segment in the chain.
         idx (int): The index of the target within its `segment`.
         len (int): The number of children `segment` has.
+        code_idxs (:obj:`tuple` of int): The indices which contain code.
     """
 
     segment: "BaseSegment"
     idx: int
     len: int
+    code_idxs: Tuple[int, ...]
 
 
 @dataclass
 class FixPatch:
     """An edit patch for a source file."""
 
     templated_slice: slice
@@ -454,17 +456,18 @@
 
     @cached_property
     def raw_segments_with_ancestors(
         self,
     ) -> List[Tuple["RawSegment", List[PathStep]]]:
         """Returns a list of raw segments in this segment with the ancestors."""
         buffer = []
+        code_idxs = tuple(idx for idx, seg in enumerate(self.segments) if seg.is_code)
         for idx, seg in enumerate(self.segments):
             # If it's a raw, yield it with this segment as the parent
-            new_step = [PathStep(self, idx, len(self.segments))]
+            new_step = [PathStep(self, idx, len(self.segments), code_idxs)]
             if seg.is_type("raw"):
                 buffer.append((seg, new_step))
             # If it's not, recurse - prepending self to the ancestor stack
             else:
                 buffer.extend(
                     [
                         (raw_seg, new_step + stack)
@@ -1146,17 +1149,19 @@
         if not self.get_start_loc() <= other.get_start_loc() <= self.get_end_loc():
             return []
 
         # Do we have any child segments at all?
         if not self.segments:
             return []
 
+        # Check code idxs
+        code_idxs = tuple(idx for idx, seg in enumerate(self.segments) if seg.is_code)
         # Check through each of the child segments
         for idx, seg in enumerate(self.segments):
-            step = PathStep(self, idx, len(self.segments))
+            step = PathStep(self, idx, len(self.segments), code_idxs)
             # Have we found the target?
             if seg is other:
                 return [step]
             # Is there a path to the target?
             res = seg.path_to(other)
             if res:
                 return [step] + res
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.0.4/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.0.4/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,14 +661,17 @@
     targets_templated = False
     # Some fix routines do their own checking for whether their fixes
     # are safe around templated elements. For those - the default
     # safety checks might be inappropriate. In those cases, set
     # template_safe_fixes to True.
     template_safe_fixes = False
 
+    # Config settings supported for this rule.
+    # See config_info.py for supported values.
+    config_keywords: List[str] = []
     # Lint loop / crawl behavior. When appropriate, rules can (and should)
     # override these values to make linting faster.
     crawl_behaviour: BaseCrawler
     # Rules can override this to specify "post". "Post" rules are those that are
     # not expected to trigger any downstream rules, e.g. capitalization fixes.
     # They run on two occasions:
     # - On the first pass of the main phase
@@ -690,15 +693,15 @@
     code: str
     description: str
 
     # Should we document this rule as fixable? Used by the metaclass to add
     # a line to the docstring.
     is_fix_compatible = False
 
-    # Add comma seperated string to Base Rule to ensure that it uses the same
+    # Add comma separated string to Base Rule to ensure that it uses the same
     # Configuration that is defined in the Config.py file
     split_comma_separated_string = staticmethod(split_comma_separated_string)
 
     def __init__(self, code, description, **kwargs):
         self.description = description
         self.code = code
         # kwargs represents the config passed to the rule. Add all kwargs as class
@@ -706,26 +709,23 @@
         for key, value in kwargs.items():
             self.__dict__[key] = value
 
         # We also define a custom logger here, which also includes the code
         # of the rule in the logging.
         self.logger = RuleLoggingAdapter(rules_logger, {"code": code})
         # Validate that declared configuration options exist
-        try:
-            for keyword in self.config_keywords:
-                if keyword not in kwargs.keys():
-                    raise ValueError(
-                        (
-                            "Unrecognized config '{}' for Rule {}. If this "
-                            "is a new option, please add it to "
-                            "`default_config.cfg`"
-                        ).format(keyword, code)
-                    )
-        except AttributeError:
-            self.logger.info(f"No config_keywords defined for {code}")
+        for keyword in self.config_keywords:
+            if keyword not in kwargs.keys():
+                raise ValueError(
+                    (
+                        "Unrecognized config '{}' for Rule {}. If this "
+                        "is a new option, please add it to "
+                        "`default_config.cfg`"
+                    ).format(keyword, code)
+                )
 
     @classmethod
     def get_config_ref(cls):
         """Return the config lookup ref for this rule.
 
         If a `name` is defined, it's the name - otherwise the code.
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.0.4/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.0.4/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,16 @@
 
     @staticmethod
     def extract_block_type(tag_name, block_subtype):
         """Determine block type."""
         # :TRICKY: Syntactically, the Jinja {% include %} directive looks like
         # a block, but its behavior is basically syntactic sugar for
         # {{ open("somefile).read() }}. Thus, treat it as templated code.
-        if tag_name == "include":
+        # It's a similar situation with {% import %} and {% from ... import %}.
+        if tag_name in ["include", "import", "from"]:
             block_type = "templated"
         elif tag_name.startswith("end"):
             block_type = "block_end"
         elif tag_name.startswith("el"):
             # else, elif
             block_type = "block_mid"
         else:
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/core/timing.py` & `sqlfluff-2.0.4/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,20 +258,19 @@
         "YEAR",
     ]
 )
 
 ansi_dialect.sets("date_part_function_name").update(["DATEADD"])
 
 # Set Keywords
-ansi_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in ansi_unreserved_keywords.split("\n")]
+ansi_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", ansi_unreserved_keywords
 )
-
-ansi_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in ansi_reserved_keywords.split("\n")]
+ansi_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", ansi_reserved_keywords
 )
 
 # Bracket pairs (a set of tuples).
 # (name, startref, endref, persists)
 # NOTE: The `persists` value controls whether this type
 # of bracket is persisted during matching to speed up other
 # parts of the matching process. Round brackets are the most
@@ -415,17 +414,15 @@
         Ref("ModuloSegment"),
         Ref("BitwiseAndSegment"),
         Ref("BitwiseOrSegment"),
         Ref("BitwiseXorSegment"),
         Ref("BitwiseLShiftSegment"),
         Ref("BitwiseRShiftSegment"),
     ),
-    SignedSegmentGrammar=AnyNumberOf(
-        Ref("PositiveSegment"), Ref("NegativeSegment"), min_times=1
-    ),
+    SignedSegmentGrammar=OneOf(Ref("PositiveSegment"), Ref("NegativeSegment")),
     StringBinaryOperatorGrammar=OneOf(Ref("ConcatSegment")),
     BooleanBinaryOperatorGrammar=OneOf(
         Ref("AndOperatorGrammar"), Ref("OrOperatorGrammar")
     ),
     ComparisonOperatorGrammar=OneOf(
         Ref("EqualsSegment"),
         Ref("GreaterThanSegment"),
@@ -1065,14 +1062,20 @@
 
 class IndexReferenceSegment(ObjectReferenceSegment):
     """A reference to an index."""
 
     type = "index_reference"
 
 
+class CollationReferenceSegment(ObjectReferenceSegment):
+    """A reference to a collation."""
+
+    type = "collation_reference"
+
+
 class RoleReferenceSegment(ObjectReferenceSegment):
     """A reference to a role, user, or account."""
 
     type = "role_reference"
     match_grammar: Matchable = Ref("SingleIdentifierGrammar")
 
 
@@ -1154,23 +1157,25 @@
     """A reference to an object with an `AS` clause.
 
     The optional AS keyword allows both implicit and explicit aliasing.
     """
 
     type = "alias_expression"
     match_grammar: Matchable = Sequence(
+        Indent,
         Ref.keyword("AS", optional=True),
         OneOf(
             Sequence(
                 Ref("SingleIdentifierGrammar"),
                 # Column alias in VALUES clause
                 Bracketed(Ref("SingleIdentifierListSegment"), optional=True),
             ),
             Ref("SingleQuotedIdentifierSegment"),
         ),
+        Dedent,
     )
 
 
 class ShorthandCastSegment(BaseSegment):
     """A casting operation using '::'."""
 
     type = "cast_expression"
@@ -1187,15 +1192,15 @@
             ),
             min_times=1,
         ),
     )
 
 
 class QualifiedNumericLiteralSegment(BaseSegment):
-    """A numeric literal with one or more + or - signs preceding.
+    """A numeric literal with one + or - sign preceding.
 
     The qualified numeric literal is a compound of a raw
     literal and a plus/minus sign. We do it this way rather
     than at the lexing step because the lexer doesn't deal
     well with ambiguity.
     """
 
@@ -1271,22 +1276,24 @@
 
 
 class OverClauseSegment(BaseSegment):
     """An OVER clause for window functions."""
 
     type = "over_clause"
     match_grammar: Matchable = Sequence(
+        Indent,
         Sequence(OneOf("IGNORE", "RESPECT"), "NULLS", optional=True),
         "OVER",
         OneOf(
             Ref("SingleIdentifierGrammar"),  # Window name
             Bracketed(
                 Ref("WindowSpecificationSegment", optional=True),
             ),
         ),
+        Dedent,
     )
 
 
 class WindowSpecificationSegment(BaseSegment):
     """Window specification within OVER(...)."""
 
     type = "window_specification"
@@ -1900,50 +1907,73 @@
         ),
     )
 
 
 ansi_dialect.add(
     # Expression_A_Grammar
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.html#a_expr
-    Expression_A_Grammar=Sequence(
-        OneOf(
-            Ref("Expression_C_Grammar"),
-            Sequence(
-                OneOf(
-                    Ref("SignedSegmentGrammar"),
-                    # Ref('TildeSegment'),
-                    Ref("NotOperatorGrammar"),
-                    "PRIOR",
-                    # used in CONNECT BY clauses (EXASOL, Snowflake, Postgres...)
-                ),
-                Ref("Expression_C_Grammar"),
-            ),
+    # The upstream grammar is defined recursively, which if implemented naively
+    # will cause SQLFluff to overflow the stack from recursive function calls.
+    # To work around this, the a_expr grammar is reworked a bit into sub-grammars
+    # that effectively provide tail recursion.
+    Expression_A_Unary_Operator_Grammar=OneOf(
+        # This grammar corresponds to the unary operator portion of the initial
+        # recursive block on the Cockroach Labs a_expr grammar.  It includes the
+        # unary operator matching sub-block, but not the recursive call to a_expr.
+        Ref(
+            "SignedSegmentGrammar",
+            exclude=Sequence(Ref("QualifiedNumericLiteralSegment")),
         ),
+        Ref("TildeSegment"),
+        Ref("NotOperatorGrammar"),
+        # used in CONNECT BY clauses (EXASOL, Snowflake, Postgres...)
+        "PRIOR",
+    ),
+    Tail_Recurse_Expression_A_Grammar=Sequence(
+        # This should be used instead of a recursive call to Expression_A_Grammar
+        # whenever the repeating element in Expression_A_Grammar makes a recursive
+        # call to itself at the _end_.  If it's in the middle then you still need
+        # to recurse into Expression_A_Grammar normally.
+        AnyNumberOf(Ref("Expression_A_Unary_Operator_Grammar")),
+        Ref("Expression_C_Grammar"),
+    ),
+    Expression_A_Grammar=Sequence(
+        # Grammar always starts with optional unary operator, plus c_expr.  This
+        # section must always match the tail recurse grammar.
+        Ref("Tail_Recurse_Expression_A_Grammar"),
+        # As originally pictured in the diagram, the grammar then repeats itself
+        # for any number of times with a loop.
         AnyNumberOf(
             OneOf(
+                # This corresponds to the big repeating block in the diagram that
+                # has like dozens and dozens of possibilities.  Some of them are
+                # recursive.  If the item __ends__ with a recursive call to "a_expr",
+                # use Ref("Tail_Recurse_Expression_A_Grammar") instead so that the
+                # stack depth can be minimized.  If the item has a recursive call
+                # in the middle of the expression, you'll need to recurse
+                # Expression_A_Grammar normally.
+                #
+                # We need to add a lot more here...
                 Sequence(
-                    OneOf(
-                        Sequence(
-                            Ref.keyword("NOT", optional=True),
-                            Ref("LikeGrammar"),
-                        ),
-                        Sequence(
-                            Ref("BinaryOperatorGrammar"),
-                            Ref.keyword("NOT", optional=True),
-                        ),
-                        # We need to add a lot more here...
+                    Sequence(
+                        Ref.keyword("NOT", optional=True),
+                        Ref("LikeGrammar"),
                     ),
-                    Ref("Expression_C_Grammar"),
+                    Ref("Expression_A_Grammar"),
                     Sequence(
                         Ref.keyword("ESCAPE"),
-                        Ref("Expression_C_Grammar"),
+                        Ref("Tail_Recurse_Expression_A_Grammar"),
                         optional=True,
                     ),
                 ),
                 Sequence(
+                    Ref("BinaryOperatorGrammar"),
+                    Ref("Tail_Recurse_Expression_A_Grammar"),
+                ),
+                Sequence(
                     Ref.keyword("NOT", optional=True),
                     "IN",
                     Bracketed(
                         OneOf(
                             Delimited(
                                 Ref("Expression_A_Grammar"),
                             ),
@@ -1962,48 +1992,57 @@
                     Ref.keyword("NOT", optional=True),
                     Ref("IsClauseGrammar"),
                 ),
                 Ref("IsNullGrammar"),
                 Ref("NotNullGrammar"),
                 Ref("CollateGrammar"),
                 Sequence(
-                    # e.g. NOT EXISTS, but other expressions could be met as
-                    # well by inverting the condition with the NOT operator
-                    "NOT",
-                    Ref("Expression_C_Grammar"),
-                ),
-                Sequence(
                     Ref.keyword("NOT", optional=True),
                     "BETWEEN",
                     Ref("Expression_B_Grammar"),
                     "AND",
-                    Ref("Expression_A_Grammar"),
+                    Ref("Tail_Recurse_Expression_A_Grammar"),
                 ),
             )
         ),
     ),
     # Expression_B_Grammar: Does not directly feed into Expression_A_Grammar
     # but is used for a BETWEEN statement within Expression_A_Grammar.
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.htm#b_expr
-    Expression_B_Grammar=Sequence(
-        OneOf(
-            Ref("Expression_C_Grammar"),
-            Sequence(
-                Ref("SignedSegmentGrammar"),
-                Ref("Expression_B_Grammar"),
-            ),
+    #
+    # We use a similar trick as seen with Expression_A_Grammar to avoid recursion
+    # by using a tail recursion grammar.  See the comments for a_expr to see how
+    # that works.
+    Expression_B_Unary_Operator_Grammar=OneOf(
+        Ref(
+            "SignedSegmentGrammar",
+            exclude=Sequence(Ref("QualifiedNumericLiteralSegment")),
         ),
+        Ref("TildeSegment"),
+    ),
+    Tail_Recurse_Expression_B_Grammar=Sequence(
+        # Only safe to use if the recursive call is at the END of the repeating
+        # element in the main b_expr portion
+        AnyNumberOf(Ref("Expression_B_Unary_Operator_Grammar")),
+        Ref("Expression_C_Grammar"),
+    ),
+    Expression_B_Grammar=Sequence(
+        # Always start with tail recursion element!
+        Ref("Tail_Recurse_Expression_B_Grammar"),
         AnyNumberOf(
-            Sequence(
-                OneOf(
-                    Ref("ArithmeticBinaryOperatorGrammar"),
-                    Ref("StringBinaryOperatorGrammar"),
-                    Ref("ComparisonOperatorGrammar"),
+            OneOf(
+                Sequence(
+                    OneOf(
+                        Ref("ArithmeticBinaryOperatorGrammar"),
+                        Ref("StringBinaryOperatorGrammar"),
+                        Ref("ComparisonOperatorGrammar"),
+                    ),
+                    Ref("Tail_Recurse_Expression_B_Grammar"),
                 ),
-                Ref("Expression_C_Grammar"),
+                # TODO: Add more things from b_expr here
             ),
         ),
     ),
     # Expression_C_Grammar
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.htm#c_expr
     Expression_C_Grammar=OneOf(
         Sequence("EXISTS", Bracketed(Ref("SelectableGrammar"))),
@@ -3115,19 +3154,18 @@
     )
 
 
 class DropIndexStatementSegment(BaseSegment):
     """A `DROP INDEX` statement."""
 
     type = "drop_index_statement"
-    # DROP INDEX <Index name> [CONCURRENTLY] [IF EXISTS] {RESTRICT | CASCADE}
+    # DROP INDEX <Index name> [IF EXISTS] {RESTRICT | CASCADE}
     match_grammar: Matchable = Sequence(
         "DROP",
         "INDEX",
-        Ref.keyword("CONCURRENTLY", optional=True),
         Ref("IfExistsGrammar", optional=True),
         Ref("IndexReferenceSegment"),
         Ref("DropBehaviorGrammar", optional=True),
     )
 
 
 class AccessStatementSegment(BaseSegment):
@@ -3436,14 +3474,68 @@
             Ref("ExpressionSegment"),
             Ref("ValuesClauseSegment"),
             "DEFAULT",
         ),
     )
 
 
+class CreateCastStatementSegment(BaseSegment):
+    """A `CREATE CAST` statement.
+
+    https://jakewheat.github.io/sql-overview/sql-2016-foundation-grammar.html#_11_63_user_defined_cast_definition
+    """
+
+    type = "create_cast_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "CAST",
+        Bracketed(
+            Ref("DatatypeSegment"),
+            "AS",
+            Ref("DatatypeSegment"),
+        ),
+        "WITH",
+        Ref.keyword("SPECIFIC", optional=True),
+        OneOf(
+            "ROUTINE",
+            "FUNCTION",
+            "PROCEDURE",
+            Sequence(
+                OneOf("INSTANCE", "STATIC", "CONSTRUCTOR", optional=True),
+                "METHOD",
+            ),
+        ),
+        Ref("FunctionNameSegment"),
+        Ref("FunctionParameterListGrammar", optional=True),
+        Sequence("FOR", Ref("ObjectReferenceSegment"), optional=True),
+        Sequence("AS", "ASSIGNMENT", optional=True),
+    )
+
+
+class DropCastStatementSegment(BaseSegment):
+    """A `DROP CAST` statement.
+
+    https://jakewheat.github.io/sql-overview/sql-2016-foundation-grammar.html#_11_64_drop_user_defined_cast_statement
+    """
+
+    type = "drop_cast_statement"
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "CAST",
+        Bracketed(
+            Ref("DatatypeSegment"),
+            "AS",
+            Ref("DatatypeSegment"),
+        ),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
 class FunctionDefinitionGrammar(BaseSegment):
     """This is the body of a `CREATE FUNCTION AS` statement."""
 
     type = "function_definition"
     match_grammar: Matchable = Sequence(
         "AS",
         Ref("QuotedLiteralSegment"),
@@ -3657,14 +3749,16 @@
         Ref("CreateDatabaseStatementSegment"),
         Ref("DropDatabaseStatementSegment"),
         Ref("CreateIndexStatementSegment"),
         Ref("DropIndexStatementSegment"),
         Ref("CreateViewStatementSegment"),
         Ref("DeleteStatementSegment"),
         Ref("UpdateStatementSegment"),
+        Ref("CreateCastStatementSegment"),
+        Ref("DropCastStatementSegment"),
         Ref("CreateFunctionStatementSegment"),
         Ref("DropFunctionStatementSegment"),
         Ref("CreateModelStatementSegment"),
         Ref("DropModelStatementSegment"),
         Ref("DescribeStatementSegment"),
         Ref("UseStatementSegment"),
         Ref("ExplainStatementSegment"),
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
 COMMAND_FUNCTION_CODE
 COMMENT
 COMMIT
 COMMITTED
 COMPLETION
 COMPRESS
 COMPUTE
-CONCURRENTLY
 CONDITION
 CONDITION_NUMBER
 CONNECT
 CONNECTION
 CONNECTION_NAME
 CONSTRAINT
 CONSTRAINT_CATALOG
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena.py`

 * *Files 4% similar despite different names*

```diff
@@ -254,20 +254,39 @@
 
 
 class ArrayTypeSchemaSegment(ansi.ArrayTypeSegment):
     """Prefix for array literals specifying the type."""
 
     type = "array_type_schema"
     match_grammar = Bracketed(
-        Delimited(
-            Sequence(
-                Ref("DatatypeSegment"),
-                Ref("CommentGrammar", optional=True),
-            ),
-            bracket_pairs_set="angle_bracket_pairs",
+        Ref("DatatypeSegment"),
+        bracket_pairs_set="angle_bracket_pairs",
+        bracket_type="angle",
+    )
+
+
+class MapTypeSegment(BaseSegment):
+    """Expression to construct a MAP datatype."""
+
+    type = "map_type"
+    match_grammar = Sequence(
+        "MAP",
+        Ref("MapTypeSchemaSegment", optional=True),
+    )
+
+
+class MapTypeSchemaSegment(BaseSegment):
+    """Expression to construct the schema of a MAP datatype."""
+
+    type = "map_type_schema"
+    match_grammar = Bracketed(
+        Sequence(
+            Ref("PrimitiveTypeSegment"),
+            Ref("CommaSegment"),
+            Ref("DatatypeSegment"),
         ),
         bracket_pairs_set="angle_bracket_pairs",
         bracket_type="angle",
     )
 
 
 class StructTypeSegment(ansi.StructTypeSegment):
@@ -342,30 +361,15 @@
     """
 
     type = "data_type"
     match_grammar = OneOf(
         Ref("PrimitiveTypeSegment"),
         Ref("StructTypeSegment"),
         Ref("ArrayTypeSegment"),
-        Sequence(
-            "MAP",
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        Ref("NakedIdentifierSegment"),
-                        Ref("CommaSegment"),
-                        Ref("DatatypeSegment"),
-                        Ref("CommentGrammar", optional=True),
-                    ),
-                    bracket_pairs_set="angle_bracket_pairs",
-                ),
-                bracket_pairs_set="angle_bracket_pairs",
-                bracket_type="angle",
-            ),
-        ),
+        Ref("MapTypeSegment"),
         Sequence(
             "ROW",
             Bracketed(
                 Delimited(
                     AnyNumberOf(
                         Sequence(
                             Ref("NakedIdentifierSegment"),
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,21 +244,21 @@
     PrimaryKeyGrammar=Nothing(),
     ForeignKeyGrammar=Nothing(),
 )
 
 
 # Set Keywords
 bigquery_dialect.sets("unreserved_keywords").clear()
-bigquery_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in bigquery_unreserved_keywords.split("\n")]
+bigquery_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", bigquery_unreserved_keywords
 )
 
 bigquery_dialect.sets("reserved_keywords").clear()
-bigquery_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in bigquery_reserved_keywords.split("\n")]
+bigquery_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", bigquery_reserved_keywords
 )
 
 # Add additional datetime units
 # https://cloud.google.com/bigquery/docs/reference/standard-sql/timestamp_functions#extract
 bigquery_dialect.sets("datetime_units").update(
     [
         "MICROSECOND",
@@ -1754,20 +1754,22 @@
 
 
 class UnpivotAliasExpressionSegment(BaseSegment):
     """In BigQuery UNPIVOT alias's can be single or double quoted or numeric."""
 
     type = "alias_expression"
     match_grammar = Sequence(
+        Indent,
         Ref.keyword("AS", optional=True),
         OneOf(
             Ref("SingleQuotedLiteralSegment"),
             Ref("DoubleQuotedLiteralSegment"),
             Ref("NumericLiteralSegment"),
         ),
+        Dedent,
     )
 
 
 class FromUnpivotExpressionSegment(BaseSegment):
     """An UNPIVOT expression.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax#unpivot_operator
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,28 +236,30 @@
 
 
 class AliasExpressionSegment(ansi.AliasExpressionSegment):
     """A reference to an object with an `AS` clause."""
 
     type = "alias_expression"
     match_grammar: Matchable = Sequence(
+        Indent,
         Ref.keyword("AS", optional=True),
         OneOf(
             Sequence(
                 Ref("SingleIdentifierGrammar"),
                 # Column alias in VALUES clause
                 Bracketed(Ref("SingleIdentifierListSegment"), optional=True),
             ),
             Ref("SingleQuotedIdentifierSegment"),
             exclude=OneOf(
                 "LATERAL",
                 "WINDOW",
                 "KEYS",
             ),
         ),
+        Dedent,
     )
 
 
 class FromExpressionElementSegment(ansi.FromExpressionElementSegment):
     """A table expression.
 
     Overridden from ANSI to allow FINAL modifier.
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
     materialize_reserved_keywords,
     materialize_unreserved_keywords,
 )
 
 postgres_dialect = load_raw_dialect("postgres")
 
 materialize_dialect = postgres_dialect.copy_as("materialize")
-materialize_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in materialize_unreserved_keywords.split("\n")]
+materialize_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", materialize_unreserved_keywords
 )
 
 materialize_dialect.sets("reserved_keywords").clear()
-materialize_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in materialize_reserved_keywords.split("\n")]
+materialize_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", materialize_reserved_keywords
 )
 
 
 class StatementSegment(ansi.StatementSegment):
     """A generic segment, to any of its child subsegments."""
 
     match_grammar = ansi.StatementSegment.match_grammar
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     RegexLexer,
     RegexParser,
     Sequence,
     StartsWith,
     StringLexer,
     StringParser,
     SymbolSegment,
+    Indent,
+    Dedent,
 )
 from sqlfluff.dialects.dialect_mysql_keywords import (
     mysql_reserved_keywords,
     mysql_unreserved_keywords,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 
@@ -90,33 +92,53 @@
     ],
     before="numeric_literal",
 )
 
 # Set Keywords
 # Do not clear inherited unreserved ansi keywords. Too many are needed to parse well.
 # Just add MySQL unreserved keywords.
-mysql_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in mysql_unreserved_keywords.split("\n")]
+mysql_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", mysql_unreserved_keywords
 )
 
 mysql_dialect.sets("reserved_keywords").clear()
-mysql_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in mysql_reserved_keywords.split("\n")]
+mysql_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", mysql_reserved_keywords
 )
 
-# Remove these reserved keywords to avoid issue in interval.sql
-# TODO - resolve this properly
-mysql_dialect.sets("reserved_keywords").difference_update(
-    ["MINUTE_SECOND", "SECOND_MICROSECOND"]
+# Set the datetime units
+mysql_dialect.sets("datetime_units").clear()
+mysql_dialect.sets("datetime_units").update(
+    [
+        # https://github.com/mysql/mysql-server/blob/1bfe02bdad6604d54913c62614bde57a055c8332/sql/sql_yacc.yy#L12321-L12345
+        # interval:
+        "DAY_HOUR",
+        "DAY_MICROSECOND",
+        "DAY_MINUTE",
+        "DAY_SECOND",
+        "HOUR_MICROSECOND",
+        "HOUR_MINUTE",
+        "HOUR_SECOND",
+        "MINUTE_MICROSECOND",
+        "MINUTE_SECOND",
+        "SECOND_MICROSECOND",
+        "YEAR_MONTH",
+        # interval_time_stamp
+        "DAY",
+        "WEEK",
+        "HOUR",
+        "MINUTE",
+        "MONTH",
+        "QUARTER",
+        "SECOND",
+        "MICROSECOND",
+        "YEAR",
+    ]
 )
 
-# Remove this reserved keyword to avoid issue in create_table_primary_foreign_keys.sql
-# TODO - resolve this properly
-mysql_dialect.sets("reserved_keywords").difference_update(["INDEX"])
-
 
 mysql_dialect.replace(
     QuotedIdentifierSegment=TypedParser(
         "back_quote",
         ansi.IdentifierSegment,
         type="quoted_identifier",
         trim_chars=("`",),
@@ -158,16 +180,14 @@
     DateTimeLiteralGrammar=Sequence(
         # MySQL does not require the keyword to be specified:
         # https://dev.mysql.com/doc/refman/8.0/en/date-and-time-literals.html
         OneOf(
             "DATE",
             "TIME",
             "TIMESTAMP",
-            "DATETIME",
-            "INTERVAL",
             optional=True,
         ),
         OneOf(
             TypedParser(
                 "single_quote",
                 ansi.LiteralSegment,
                 type="date_constructor_literal",
@@ -259,19 +279,21 @@
     """A reference to an object with an `AS` clause.
 
     The optional AS keyword allows both implicit and explicit aliasing.
     """
 
     type = "alias_expression"
     match_grammar = Sequence(
+        Indent,
         Ref.keyword("AS", optional=True),
         OneOf(
             Ref("SingleIdentifierGrammar"),
             Ref("QuotedLiteralSegment"),
         ),
+        Dedent,
     )
 
 
 class ColumnDefinitionSegment(BaseSegment):
     """A column definition, e.g. for CREATE TABLE or ALTER TABLE."""
 
     type = "column_definition"
@@ -819,23 +841,16 @@
 
     https://dev.mysql.com/doc/refman/8.0/en/date-and-time-functions.html#function_adddate
     """
 
     type = "interval_expression"
     match_grammar = Sequence(
         "INTERVAL",
-        OneOf(
-            # The Numeric Version
-            Sequence(
-                Ref("ExpressionSegment"),
-                OneOf(Ref("QuotedLiteralSegment"), Ref("DatetimeUnitSegment")),
-            ),
-            # The String version
-            Ref("QuotedLiteralSegment"),
-        ),
+        Ref("ExpressionSegment"),
+        Ref("DatetimeUnitSegment"),
     )
 
 
 mysql_dialect.add(
     OutputParameterSegment=StringParser(
         "OUT", SymbolSegment, type="parameter_direction"
     ),
@@ -1090,14 +1105,15 @@
             Ref("OptimizeTableStatementSegment"),
             Ref("UpsertClauseListSegment"),
             Ref("InsertRowAliasSegment"),
             Ref("FlushStatementSegment"),
             Ref("LoadDataSegment"),
             Ref("ReplaceSegment"),
             Ref("AlterDatabaseStatementSegment"),
+            Ref("ReturnStatementSegment"),
         ],
         remove=[
             # handle CREATE SCHEMA in CreateDatabaseStatementSegment
             Ref("CreateSchemaStatementSegment"),
         ],
     )
 
@@ -1340,15 +1356,20 @@
         ),
         Ref("DefinerSegment", optional=True),
         Sequence("SQL", "SECURITY", OneOf("DEFINER", "INVOKER"), optional=True),
         "VIEW",
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
         "AS",
-        OptionallyBracketed(Ref("SelectStatementSegment")),
+        OptionallyBracketed(
+            OneOf(
+                Ref("SelectStatementSegment"),
+                Ref("SetExpressionSegment"),
+            )
+        ),
         Ref("WithCheckOptionSegment", optional=True),
     )
 
 
 class CreateViewStatementSegment(BaseSegment):
     """An `CREATE VIEW .. AS ..` statement.
 
@@ -1368,15 +1389,20 @@
         ),
         Ref("DefinerSegment", optional=True),
         Sequence("SQL", "SECURITY", OneOf("DEFINER", "INVOKER"), optional=True),
         "VIEW",
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
         "AS",
-        OptionallyBracketed(Ref("SelectStatementSegment")),
+        OptionallyBracketed(
+            OneOf(
+                Ref("SelectStatementSegment"),
+                Ref("SetExpressionSegment"),
+            )
+        ),
         Ref("WithCheckOptionSegment", optional=True),
     )
 
 
 class ProcedureParameterListGrammar(BaseSegment):
     """The parameters for a procedure ie. `(in/out/inout name datatype)`."""
 
@@ -2153,15 +2179,15 @@
             Sequence(
                 "TO",
                 Ref("QuotedLiteralSegment"),
             ),
             Sequence(
                 "BEFORE",
                 OneOf(
-                    Ref("DateTimeLiteralGrammar"),
+                    Ref("ExpressionSegment"),
                 ),
             ),
         ),
     )
 
 
 class HelpStatementSegment(BaseSegment):
@@ -2642,7 +2668,20 @@
                 "READ",
                 "ONLY",
                 Ref("EqualsSegment", optional=True),
                 OneOf("DEFAULT", Ref("NumericLiteralSegment")),
             ),
         ),
     )
+
+
+class ReturnStatementSegment(BaseSegment):
+    """A RETURN statement.
+
+    As specified in https://dev.mysql.com/doc/refman/8.0/en/return.html
+    """
+
+    type = "return_statement"
+    match_grammar = Sequence(
+        "RETURN",
+        Ref("ExpressionSegment"),
+    )
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             "double_quote",
             r'(?s)".+?"',
             CodeSegment,
             segment_kwargs={"type": "double_quote"},
         ),
         RegexLexer(
             "code",
-            r"[0-9a-zA-Z_]+[0-9a-zA-Z_$]*",
+            r"[a-zA-Z_][0-9a-zA-Z_$]*",
             CodeSegment,
             segment_kwargs={"type": "code"},
         ),
     ]
 )
 
 postgres_dialect.sets("reserved_keywords").update(
@@ -248,21 +248,47 @@
     ),
     # Add a Full equivalent which also allow keywords
     NakedIdentifierFullSegment=TypedParser(
         "code",
         ansi.IdentifierSegment,
         type="naked_identifier_all",
     ),
+    PropertiesNakedIdentifierSegment=TypedParser(  # allows reserved keywords
+        "code",
+        CodeSegment,
+        type="properties_naked_identifier",
+    ),
     SingleIdentifierFullGrammar=OneOf(
         Ref("NakedIdentifierSegment"),
         Ref("QuotedIdentifierSegment"),
         Ref("NakedIdentifierFullSegment"),
     ),
+    DefinitionArgumentValueGrammar=OneOf(
+        # This comes from def_arg:
+        # https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6331
+        # TODO: this list is incomplete
+        Ref("LiteralGrammar"),
+        # This is a gross simplification of the grammar, which seems overly
+        # permissive for the actual use cases here.  Grammar says this matches
+        # reserved keywords.  Plus also unreserved keywords and IDENT:  func_type -->
+        #     Typename --> SimpleTypename --> GenericType --> type_function_name -->
+        #     { unreserved_keyword | type_func_name_keyword | IDENT }
+        # We'll just match any normal code/keyword string here to keep it simple.
+        Ref("PropertiesNakedIdentifierSegment"),
+    ),
     CascadeRestrictGrammar=OneOf("CASCADE", "RESTRICT"),
+    ExtendedTableReferenceGrammar=OneOf(
+        Ref("TableReferenceSegment"),
+        Sequence("ONLY", OptionallyBracketed(Ref("TableReferenceSegment"))),
+        Sequence(Ref("TableReferenceSegment"), Ref("StarSegment")),
+    ),
     RightArrowSegment=StringParser("=>", SymbolSegment, type="right_arrow"),
+    OnKeywordAsIdentifierSegment=StringParser(
+        "ON", ansi.IdentifierSegment, type="naked_identifier"
+    ),
 )
 
 postgres_dialect.replace(
     LikeGrammar=OneOf("LIKE", "ILIKE", Sequence("SIMILAR", "TO")),
     StringBinaryOperatorGrammar=OneOf(Ref("ConcatSegment"), "COLLATE"),
     ComparisonOperatorGrammar=OneOf(
         Ref("EqualsSegment"),
@@ -478,14 +504,26 @@
         Ref("ForClauseSegment"),
     ),
     Accessor_Grammar=AnyNumberOf(
         Ref("ArrayAccessorSegment"),
         # Add in semi structured expressions
         Ref("SemiStructuredAccessorSegment"),
     ),
+    # PostgreSQL supports the non-standard "RETURNING" keyword, and therefore the
+    # INSERT/UPDATE/DELETE statements can also be used in subqueries.
+    NonWithSelectableGrammar=OneOf(
+        Ref("SetExpressionSegment"),
+        OptionallyBracketed(Ref("SelectStatementSegment")),
+        Ref("NonSetSelectableGrammar"),
+        # moved from NonWithNonSelectableGrammar:
+        Ref("UpdateStatementSegment"),
+        Ref("InsertStatementSegment"),
+        Ref("DeleteStatementSegment"),
+    ),
+    NonWithNonSelectableGrammar=OneOf(),
 )
 
 
 # Inherit from the ANSI ObjectReferenceSegment this way so we can inherit
 # other segment types from it.
 class ObjectReferenceSegment(ansi.ObjectReferenceSegment):
     """A reference to an object."""
@@ -544,52 +582,38 @@
 class ArrayAccessorSegment(ansi.ArrayAccessorSegment):
     """Overwrites Array Accessor in ANSI to allow n many consecutive brackets.
 
     Postgres can also have array access like python [:2] or [2:] so
     numbers on either side of the slice segment are optional.
     """
 
-    match_grammar = Sequence(
-        AnyNumberOf(
-            Bracketed(
-                Sequence(
-                    OneOf(
-                        OneOf(
-                            Ref("QualifiedNumericLiteralSegment"),
-                            Ref("NumericLiteralSegment"),
-                        ),
-                        Sequence(
-                            OneOf(
-                                Ref("QualifiedNumericLiteralSegment"),
-                                Ref("NumericLiteralSegment"),
-                                optional=True,
-                            ),
-                            Ref("SliceSegment"),
-                            OneOf(
-                                Ref("QualifiedNumericLiteralSegment"),
-                                Ref("NumericLiteralSegment"),
-                            ),
-                        ),
-                        Sequence(
-                            OneOf(
-                                Ref("QualifiedNumericLiteralSegment"),
-                                Ref("NumericLiteralSegment"),
-                            ),
-                            Ref("SliceSegment"),
-                            OneOf(
-                                Ref("QualifiedNumericLiteralSegment"),
-                                Ref("NumericLiteralSegment"),
-                                optional=True,
-                            ),
-                        ),
-                    ),
+    match_grammar = Bracketed(
+        OneOf(
+            # These three are for a single element access: [n]
+            Ref("QualifiedNumericLiteralSegment"),
+            Ref("NumericLiteralSegment"),
+            Ref("ExpressionSegment"),
+            # This is for slice access: [n:m], [:m], [n:], and [:]
+            Sequence(
+                OneOf(
+                    Ref("QualifiedNumericLiteralSegment"),
+                    Ref("NumericLiteralSegment"),
+                    Ref("ExpressionSegment"),
+                    optional=True,
                 ),
-                bracket_type="square",
-            )
-        )
+                Ref("SliceSegment"),
+                OneOf(
+                    Ref("QualifiedNumericLiteralSegment"),
+                    Ref("NumericLiteralSegment"),
+                    Ref("ExpressionSegment"),
+                    optional=True,
+                ),
+            ),
+        ),
+        bracket_type="square",
     )
 
 
 class DateTimeTypeIdentifier(BaseSegment):
     """Date Time Type."""
 
     type = "datetime_type_identifier"
@@ -667,14 +691,18 @@
                     # monetary type
                     "MONEY",
                     # character types
                     OneOf(
                         Sequence(
                             OneOf(
                                 "CHAR",
+                                # CHAR VARYING is not documented, but it's
+                                # in the real grammar:
+                                # https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L14262
+                                Sequence("CHAR", "VARYING"),
                                 "CHARACTER",
                                 Sequence("CHARACTER", "VARYING"),
                                 "VARCHAR",
                             ),
                             Ref("BracketedArguments", optional=True),
                         ),
                         "TEXT",
@@ -732,14 +760,152 @@
 class ArrayTypeSegment(ansi.ArrayTypeSegment):
     """Prefix for array literals specifying the type."""
 
     type = "array_type"
     match_grammar = Ref.keyword("ARRAY")
 
 
+class IndexAccessMethodSegment(BaseSegment):
+    """Index access method (e.g. `USING gist`)."""
+
+    type = "index_access_method"
+    match_grammar = Ref("SingleIdentifierGrammar")
+
+
+class OperatorClassReferenceSegment(ObjectReferenceSegment):
+    """A reference to an operator class."""
+
+    type = "operator_class_reference"
+
+
+class DefinitionParameterSegment(BaseSegment):
+    """A single definition parameter.
+
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6320
+    """
+
+    type = "definition_parameter"
+    match_grammar: Matchable = Sequence(
+        Ref("PropertiesNakedIdentifierSegment"),
+        Sequence(
+            Ref("EqualsSegment"),
+            # could also contain ParameterNameSegment:
+            Ref("DefinitionArgumentValueGrammar"),
+            optional=True,
+        ),
+    )
+
+
+class DefinitionParametersSegment(BaseSegment):
+    """List of definition parameters.
+
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6313
+    """
+
+    type = "definition_parameters"
+    match_grammar: Matchable = Bracketed(
+        Delimited(
+            Ref("DefinitionParameterSegment"),
+        )
+    )
+
+
+class CreateCastStatementSegment(ansi.CreateCastStatementSegment):
+    """A `CREATE CAST` statement.
+
+    https://www.postgresql.org/docs/15/sql-createcast.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L8951
+    """
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "CAST",
+        Bracketed(
+            Ref("DatatypeSegment"),
+            "AS",
+            Ref("DatatypeSegment"),
+        ),
+        OneOf(
+            Sequence(
+                "WITH",
+                "FUNCTION",
+                Ref("FunctionNameSegment"),
+                Ref("FunctionParameterListGrammar", optional=True),
+            ),
+            Sequence("WITHOUT", "FUNCTION"),
+            Sequence("WITH", "INOUT"),
+        ),
+        OneOf(
+            Sequence("AS", "ASSIGNMENT", optional=True),
+            Sequence("AS", "IMPLICIT", optional=True),
+            optional=True,
+        ),
+    )
+
+
+class DropCastStatementSegment(ansi.DropCastStatementSegment):
+    """A `DROP CAST` statement.
+
+    https://www.postgresql.org/docs/15/sql-dropcast.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L8995
+    """
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "CAST",
+        Sequence("IF", "EXISTS", optional=True),
+        Bracketed(
+            Ref("DatatypeSegment"),
+            "AS",
+            Ref("DatatypeSegment"),
+        ),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
+class RelationOptionSegment(BaseSegment):
+    """Relation option element from reloptions.
+
+    It is very similar to DefinitionParameterSegment except that it allows qualified
+    names (e.g. namespace.attr = 5).
+
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L3016-L3035
+    """
+
+    type = "relation_option"
+    match_grammar: Matchable = Sequence(
+        Ref("PropertiesNakedIdentifierSegment"),
+        Sequence(
+            Ref("DotSegment"),
+            Ref("PropertiesNakedIdentifierSegment"),
+            optional=True,
+        ),
+        Sequence(
+            Ref("EqualsSegment"),
+            # could also contain ParameterNameSegment:
+            Ref("DefinitionArgumentValueGrammar"),
+            optional=True,
+        ),
+    )
+
+
+class RelationOptionsSegment(BaseSegment):
+    """List of relation options.
+
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L3003-L3014
+    """
+
+    type = "relation_options"
+    match_grammar: Matchable = Bracketed(
+        Delimited(
+            Ref("RelationOptionSegment"),
+        )
+    )
+
+
 class CreateFunctionStatementSegment(ansi.CreateFunctionStatementSegment):
     """A `CREATE FUNCTION` statement.
 
     This version in the ANSI dialect should be a "common subset" of the
     structure of the code for those dialects.
     postgres: https://www.postgresql.org/docs/13/sql-createfunction.html
     """
@@ -1471,38 +1637,41 @@
                 optional=True,
             ),
             Sequence("RENAME", "TO", Ref("RoleReferenceSegment"), optional=True),
             Sequence(
                 Sequence(
                     "IN",
                     "DATABASE",
-                    Ref("ObjectReferenceSegment"),
+                    Ref("DatabaseReferenceSegment"),
                     optional=True,
                 ),
                 OneOf(
                     Sequence(
                         "SET",
-                        Ref("ObjectReferenceSegment"),
+                        Ref("ParameterNameSegment"),
                         OneOf(
                             Sequence(
                                 OneOf("TO", Ref("EqualsSegment")),
                                 OneOf(
-                                    Ref("QuotedLiteralSegment"),
                                     "DEFAULT",
-                                    "ON",
-                                    "OFF",
+                                    Delimited(
+                                        Ref("LiteralGrammar"),
+                                        Ref("NakedIdentifierSegment"),
+                                        # https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L1810-L1815
+                                        Ref("OnKeywordAsIdentifierSegment"),
+                                    ),
                                 ),
                             ),
                             Sequence(
                                 "FROM",
                                 "CURRENT",
                             ),
                         ),
                     ),
-                    Sequence("RESET", OneOf(Ref("QuotedLiteralSegment"), "ALL")),
+                    Sequence("RESET", OneOf(Ref("ParameterNameSegment"), "ALL")),
                 ),
                 optional=True,
             ),
         ),
     )
 
 
@@ -1569,14 +1738,37 @@
         Sequence(
             "FORMAT",
             OneOf("TEXT", "XML", "JSON", "YAML"),
         ),
     )
 
 
+class CreateSchemaStatementSegment(ansi.CreateSchemaStatementSegment):
+    """A `CREATE SCHEMA` statement.
+
+    https://www.postgresql.org/docs/15/sql-createschema.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L1493
+    """
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "SCHEMA",
+        Ref("IfNotExistsGrammar", optional=True),
+        OneOf(
+            Sequence(
+                # schema name defaults to role if not provided
+                Ref("SchemaReferenceSegment", optional=True),
+                "AUTHORIZATION",
+                Ref("RoleReferenceSegment"),
+            ),
+            Ref("SchemaReferenceSegment"),
+        ),
+    )
+
+
 class CreateTableStatementSegment(ansi.CreateTableStatementSegment):
     """A `CREATE TABLE` statement.
 
     As specified in https://www.postgresql.org/docs/13/sql-createtable.html
     """
 
     match_grammar = Sequence(
@@ -1966,19 +2158,15 @@
                     Bracketed(Delimited(Ref("ParameterNameSegment"))),
                 ),
                 Sequence(
                     "SET", "STORAGE", OneOf("PLAIN", "EXTERNAL", "EXTENDED", "MAIN")
                 ),
             ),
         ),
-        Sequence(
-            "ADD",
-            Ref("TableConstraintSegment"),
-            Sequence("NOT", "VALID", optional=True),
-        ),
+        Sequence("ADD", Ref("TableConstraintSegment")),
         Sequence("ADD", Ref("TableConstraintUsingIndexSegment")),
         Sequence(
             "ALTER",
             "CONSTRAINT",
             Ref("ParameterNameSegment"),
             OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE"), optional=True),
             OneOf(
@@ -2068,37 +2256,17 @@
 
 
 class VersionIdentifierSegment(BaseSegment):
     """A reference to an version."""
 
     type = "version_identifier"
     # match grammar (don't allow whitespace)
-    match_grammar: Matchable = Sequence(
-        OneOf(
-            Ref("QuotedLiteralSegment"),
-            Ref("NumericLiteralSegment"),
-            Ref("NakedIdentifierSegment"),
-        ),
-        AnyNumberOf(
-            OneOf(
-                # Literals might follow literals if these literals
-                # begin with a "." e.g. 1.2.3.4
-                Ref("NumericLiteralSegment"),
-                Sequence(
-                    Ref("DotSegment"),
-                    OneOf(
-                        Ref("NumericLiteralSegment"),
-                        Ref("NakedIdentifierSegment"),
-                    ),
-                    allow_gaps=False,
-                ),
-            ),
-            allow_gaps=False,
-        ),
-        allow_gaps=False,
+    match_grammar: Matchable = OneOf(
+        Ref("QuotedLiteralSegment"),
+        Ref("NakedIdentifierSegment"),
     )
 
 
 class CreateExtensionStatementSegment(BaseSegment):
     """A `CREATE EXTENSION` statement.
 
     https://www.postgresql.org/docs/9.1/sql-createextension.html
@@ -2125,15 +2293,141 @@
 
     type = "drop_extension_statement"
     match_grammar: Matchable = Sequence(
         "DROP",
         "EXTENSION",
         Ref("IfExistsGrammar", optional=True),
         Ref("ExtensionReferenceSegment"),
-        Ref("CascadeRestrictGrammar", optional=True),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
+class PublicationReferenceSegment(ObjectReferenceSegment):
+    """A reference to a publication."""
+
+    type = "publication_reference"
+    match_grammar: Matchable = Ref("SingleIdentifierGrammar")
+
+
+class PublicationTableSegment(BaseSegment):
+    """Specification for a single table object in a publication."""
+
+    type = "publication_table"
+    match_grammar: Matchable = Sequence(
+        Ref("ExtendedTableReferenceGrammar"),
+        Ref("BracketedColumnReferenceListGrammar", optional=True),
+        Sequence("WHERE", Bracketed(Ref("ExpressionSegment")), optional=True),
+    )
+
+
+class PublicationObjectsSegment(BaseSegment):
+    """Specification for one or more objects in a publication.
+
+    Unlike the underlying PG grammar which has one object per PublicationObjSpec and
+    so requires one to track the previous object type if it's a "continuation object
+    type", this grammar groups together the continuation objects, e.g.
+    "TABLE a, b, TABLE c, d" results in two segments: one containing references
+    "a, b", and the other contianing "c, d".
+
+    https://www.postgresql.org/docs/15/sql-createpublication.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L10435-L10530
+    """
+
+    type = "publication_objects"
+    match_grammar: Matchable = OneOf(
+        Sequence(
+            "TABLE",
+            Delimited(
+                Ref("PublicationTableSegment"),
+                terminator=Sequence(Ref("CommaSegment"), OneOf("TABLE", "TABLES")),
+            ),
+        ),
+        Sequence(
+            "TABLES",
+            "IN",
+            "SCHEMA",
+            Delimited(
+                OneOf(Ref("SchemaReferenceSegment"), "CURRENT_SCHEMA"),
+                terminator=Sequence(Ref("CommaSegment"), OneOf("TABLE", "TABLES")),
+            ),
+        ),
+    )
+
+
+class CreatePublicationStatementSegment(BaseSegment):
+    """A `CREATE PUBLICATION` statement.
+
+    https://www.postgresql.org/docs/15/sql-createpublication.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L10390-L10530
+    """
+
+    type = "create_publication_statement"
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "PUBLICATION",
+        Ref("PublicationReferenceSegment"),
+        OneOf(
+            Sequence("FOR", "ALL", "TABLES"),
+            Sequence("FOR", Delimited(Ref("PublicationObjectsSegment"))),
+            optional=True,
+        ),
+        Sequence(
+            "WITH",
+            Ref("DefinitionParametersSegment"),
+            optional=True,
+        ),
+    )
+
+
+class AlterPublicationStatementSegment(BaseSegment):
+    """A `ALTER PUBLICATION` statement.
+
+    https://www.postgresql.org/docs/15/sql-alterpublication.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L10549
+    """
+
+    type = "alter_publication_statement"
+    match_grammar: Matchable = Sequence(
+        "ALTER",
+        "PUBLICATION",
+        Ref("PublicationReferenceSegment"),
+        OneOf(
+            Sequence("SET", Ref("DefinitionParametersSegment")),
+            Sequence("ADD", Delimited(Ref("PublicationObjectsSegment"))),
+            Sequence("SET", Delimited(Ref("PublicationObjectsSegment"))),
+            Sequence("DROP", Delimited(Ref("PublicationObjectsSegment"))),
+            Sequence("RENAME", "TO", Ref("PublicationReferenceSegment")),
+            Sequence(
+                "OWNER",
+                "TO",
+                OneOf(
+                    "CURRENT_ROLE",
+                    "CURRENT_USER",
+                    "SESSION_USER",
+                    # must come last; CURRENT_USER isn't reserved:
+                    Ref("RoleReferenceSegment"),
+                ),
+            ),
+        ),
+    )
+
+
+class DropPublicationStatementSegment(BaseSegment):
+    """A `DROP PUBLICATION` statement.
+
+    https://www.postgresql.org/docs/15/sql-droppublication.html
+    """
+
+    type = "drop_publication_statement"
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "PUBLICATION",
+        Ref("IfExistsGrammar", optional=True),
+        Delimited(Ref("PublicationReferenceSegment")),
+        Ref("DropBehaviorGrammar", optional=True),
     )
 
 
 class CreateMaterializedViewStatementSegment(BaseSegment):
     """A `CREATE MATERIALIZED VIEW` statement.
 
     As specified in https://www.postgresql.org/docs/14/sql-creatematerializedview.html
@@ -2469,14 +2763,30 @@
                 "RESET",
                 Bracketed(Delimited(Ref("ParameterNameSegment"))),
             ),
         ),
     )
 
 
+class DropViewStatementSegment(ansi.DropViewStatementSegment):
+    """A `DROP VIEW` statement.
+
+    https://www.postgresql.org/docs/15/sql-dropview.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6698-L6719
+    """
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "VIEW",
+        Ref("IfExistsGrammar", optional=True),
+        Delimited(Ref("TableReferenceSegment")),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
 class CreateDatabaseStatementSegment(ansi.CreateDatabaseStatementSegment):
     """A `CREATE DATABASE` statement.
 
     As specified in https://www.postgresql.org/docs/14/sql-createdatabase.html
     """
 
     match_grammar = Sequence(
@@ -2616,14 +2926,69 @@
             Ref.keyword("WITH", optional=True),
             Bracketed("FORCE"),
             optional=True,
         ),
     )
 
 
+class VacuumStatementSegment(BaseSegment):
+    """A `VACUUM` statement.
+
+    https://www.postgresql.org/docs/15/sql-vacuum.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L11658
+    """
+
+    type = "vacuum_statement"
+    match_grammar = Sequence(
+        "VACUUM",
+        OneOf(
+            Sequence(
+                Ref.keyword("FULL", optional=True),
+                Ref.keyword("FREEZE", optional=True),
+                Ref.keyword("VERBOSE", optional=True),
+                OneOf("ANALYZE", "ANALYSE", optional=True),
+            ),
+            Bracketed(
+                Delimited(
+                    Sequence(
+                        OneOf(
+                            "FULL",
+                            "FREEZE",
+                            "VERBOSE",
+                            "ANALYZE",
+                            "ANALYSE",
+                            "DISABLE_PAGE_SKIPPING",
+                            "SKIP_LOCKED",
+                            "INDEX_CLEANUP",
+                            "PROCESS_TOAST",
+                            "TRUNCATE",
+                            "PARALLEL",
+                        ),
+                        OneOf(
+                            Ref("LiteralGrammar"),
+                            Ref("NakedIdentifierSegment"),
+                            # https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L1810-L1815
+                            Ref("OnKeywordAsIdentifierSegment"),
+                            optional=True,
+                        ),
+                    ),
+                ),
+            ),
+            optional=True,
+        ),
+        Delimited(
+            Sequence(
+                Ref("TableReferenceSegment"),
+                Ref("BracketedColumnReferenceListGrammar", optional=True),
+            ),
+            optional=True,
+        ),
+    )
+
+
 class LikeOptionSegment(BaseSegment):
     """Like Option Segment.
 
     As specified in https://www.postgresql.org/docs/13/sql-createtable.html
     """
 
     type = "like_option_segment"
@@ -2668,14 +3033,15 @@
             Sequence(  # DEFAULT <value>
                 "DEFAULT",
                 OneOf(
                     Ref("ShorthandCastSegment"),
                     Ref("LiteralGrammar"),
                     Ref("FunctionSegment"),
                     Ref("BareFunctionSegment"),
+                    Ref("ExpressionSegment"),
                 ),
             ),
             Sequence("GENERATED", "ALWAYS", "AS", Ref("ExpressionSegment"), "STORED"),
             Sequence(
                 "GENERATED",
                 OneOf("ALWAYS", Sequence("BY", "DEFAULT")),
                 "AS",
@@ -2763,43 +3129,37 @@
                 Ref("PrimaryKeyGrammar"),
                 # Columns making up PRIMARY KEY constraint
                 Ref("BracketedColumnReferenceListGrammar"),
                 Ref("IndexParametersSegment", optional=True),
             ),
             Sequence(
                 "EXCLUDE",
-                Sequence("USING", Ref("FunctionSegment"), optional=True),
-                Bracketed(
-                    Delimited(
-                        Sequence(
-                            Ref("ExcludeElementSegment"),
-                            "WITH",
-                            Ref("ComparisonOperatorGrammar"),
-                        )
-                    )
-                ),
+                Sequence("USING", Ref("IndexAccessMethodSegment"), optional=True),
+                Bracketed(Delimited(Ref("ExclusionConstraintElementSegment"))),
                 Ref("IndexParametersSegment", optional=True),
-                Sequence("WHERE", Ref("ExpressionSegment")),
+                Sequence("WHERE", Bracketed(Ref("ExpressionSegment")), optional=True),
             ),
             Sequence(  # FOREIGN KEY ( column_name [, ... ] )
                 # REFERENCES reftable [ ( refcolumn [, ... ] ) ]
                 "FOREIGN",
                 "KEY",
                 # Local columns making up FOREIGN KEY constraint
                 Ref("BracketedColumnReferenceListGrammar"),
                 Ref(
                     "ReferenceDefinitionGrammar"
                 ),  # REFERENCES reftable [ ( refcolumn) ]
             ),
-            OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE"), optional=True),
+        ),
+        AnyNumberOf(
+            OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE")),
             OneOf(
-                Sequence("INITIALLY", "DEFERRED"),
-                Sequence("INITIALLY", "IMMEDIATE"),
-                optional=True,
+                Sequence("INITIALLY", "DEFERRED"), Sequence("INITIALLY", "IMMEDIATE")
             ),
+            Sequence("NOT", "VALID"),
+            Sequence("NO", "INHERIT"),
         ),
     )
 
 
 class TableConstraintUsingIndexSegment(BaseSegment):
     """table_constraint_using_index.
 
@@ -2832,27 +3192,15 @@
     As specified in https://www.postgresql.org/docs/13/sql-altertable.html.
     """
 
     type = "index_parameters"
 
     match_grammar = Sequence(
         Sequence("INCLUDE", Ref("BracketedColumnReferenceListGrammar"), optional=True),
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
+        Sequence("WITH", Ref("DefinitionParametersSegment"), optional=True),
         Sequence(
             "USING",
             "INDEX",
             "TABLESPACE",
             Ref("TablespaceReferenceSegment"),
             optional=True,
         ),
@@ -2872,28 +3220,72 @@
         Sequence("SET", "NULL"),
         Sequence("SET", "DEFAULT"),
         "RESTRICT",
         Sequence("NO", "ACTION"),
     )
 
 
-class ExcludeElementSegment(BaseSegment):
-    """Exclude element segment.
+class IndexElementOptionsSegment(BaseSegment):
+    """Index element options segment.
 
-    As found in https://www.postgresql.org/docs/13/sql-altertable.html.
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L8057
     """
 
+    type = "index_element_options"
     match_grammar = Sequence(
-        OneOf(Ref("ColumnReferenceSegment"), Bracketed(Ref("ExpressionSegment"))),
-        Ref("ParameterNameSegment", optional=True),
+        Sequence("COLLATE", Ref("CollationReferenceSegment"), optional=True),
+        Sequence(
+            Ref(
+                "OperatorClassReferenceSegment",
+                exclude=Sequence("NULLS", OneOf("FIRST", "LAST")),
+            ),
+            Ref("RelationOptionsSegment", optional=True),  # args for opclass
+            optional=True,
+        ),
         OneOf("ASC", "DESC", optional=True),
         Sequence("NULLS", OneOf("FIRST", "LAST"), optional=True),
     )
 
 
+class IndexElementSegment(BaseSegment):
+    """Index element segment.
+
+    As found in https://www.postgresql.org/docs/15/sql-altertable.html.
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L8089
+    """
+
+    type = "index_element"
+    match_grammar = Sequence(
+        OneOf(
+            Ref("ColumnReferenceSegment"),
+            # TODO: This is still not perfect.  This corresponds to
+            # func_expr_windowless in the grammar and we don't currently
+            # implement everything it provides.
+            Ref("FunctionSegment"),
+            Bracketed(Ref("ExpressionSegment")),
+        ),
+        Ref("IndexElementOptionsSegment", optional=True),
+    )
+
+
+class ExclusionConstraintElementSegment(BaseSegment):
+    """Exclusion constraint element segment.
+
+    As found in https://www.postgresql.org/docs/15/sql-altertable.html.
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L4277
+    """
+
+    type = "exclusion_constraint_element"
+    match_grammar = Sequence(
+        Ref("IndexElementSegment"),
+        "WITH",
+        Ref("ComparisonOperatorGrammar"),
+    )
+
+
 class AlterDefaultPrivilegesStatementSegment(BaseSegment):
     """`ALTER DEFAULT PRIVILEGES` statement.
 
     ```
     ALTER DEFAULT PRIVILEGES
     [ FOR { ROLE | USER } target_role [, ...] ]
     [ IN SCHEMA schema_name [, ...] ]
@@ -3032,14 +3424,73 @@
             Ref("AlterDefaultPrivilegesToFromRolesSegment"),
             terminator=OneOf("RESTRICT", "CASCADE"),
         ),
         Ref("DropBehaviorGrammar", optional=True),
     )
 
 
+class DropOwnedStatementSegment(BaseSegment):
+    """A `DROP OWNED` statement.
+
+    https://www.postgresql.org/docs/15/sql-drop-owned.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6667
+    """
+
+    type = "drop_owned_statement"
+
+    match_grammar = Sequence(
+        "DROP",
+        "OWNED",
+        "BY",
+        Delimited(
+            OneOf(
+                "CURRENT_ROLE",
+                "CURRENT_USER",
+                "SESSION_USER",
+                # must come last; CURRENT_USER isn't reserved:
+                Ref("RoleReferenceSegment"),
+            ),
+        ),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
+class ReassignOwnedStatementSegment(BaseSegment):
+    """A `REASSIGN OWNED` statement.
+
+    https://www.postgresql.org/docs/15/sql-reassign-owned.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6678
+    """
+
+    type = "reassign_owned_statement"
+
+    match_grammar = Sequence(
+        "REASSIGN",
+        "OWNED",
+        "BY",
+        Delimited(
+            OneOf(
+                "CURRENT_ROLE",
+                "CURRENT_USER",
+                "SESSION_USER",
+                # must come last; CURRENT_USER isn't reserved:
+                Ref("RoleReferenceSegment"),
+            ),
+        ),
+        "TO",
+        OneOf(
+            "CURRENT_ROLE",
+            "CURRENT_USER",
+            "SESSION_USER",
+            # must come last; CURRENT_USER isn't reserved:
+            Ref("RoleReferenceSegment"),
+        ),
+    )
+
+
 class CommentOnStatementSegment(BaseSegment):
     """`COMMENT ON` statement.
 
     https://www.postgresql.org/docs/13/sql-comment.html
     """
 
     type = "comment_clause"
@@ -3379,14 +3830,32 @@
                 Ref.keyword("CONCURRENTLY", optional=True),
                 Ref("DatabaseReferenceSegment"),
             ),
         ),
     )
 
 
+class DropIndexStatementSegment(ansi.DropIndexStatementSegment):
+    """A `DROP INDEX` statement.
+
+    https://www.postgresql.org/docs/15/sql-dropindex.html
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6698-L6719
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L6808-L6829
+    """
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "INDEX",
+        Ref.keyword("CONCURRENTLY", optional=True),
+        Ref("IfExistsGrammar", optional=True),
+        Delimited(Ref("IndexReferenceSegment")),
+        Ref("DropBehaviorGrammar", optional=True),
+    )
+
+
 class FrameClauseSegment(ansi.FrameClauseSegment):
     """A frame clause for window functions.
 
     As specified in https://www.postgresql.org/docs/13/sql-expressions.html
     """
 
     _frame_extent = ansi.FrameClauseSegment._frame_extent
@@ -3551,14 +4020,16 @@
 class StatementSegment(ansi.StatementSegment):
     """A generic segment, to any of its child subsegments."""
 
     match_grammar = ansi.StatementSegment.match_grammar
     parse_grammar = ansi.StatementSegment.parse_grammar.copy(
         insert=[
             Ref("AlterDefaultPrivilegesStatementSegment"),
+            Ref("DropOwnedStatementSegment"),
+            Ref("ReassignOwnedStatementSegment"),
             Ref("CommentOnStatementSegment"),
             Ref("AnalyzeStatementSegment"),
             Ref("CreateTableAsStatementSegment"),
             Ref("AlterTriggerStatementSegment"),
             Ref("SetStatementSegment"),
             Ref("CreatePolicyStatementSegment"),
             Ref("DropPolicyStatementSegment"),
@@ -3567,14 +4038,15 @@
             Ref("DropDomainStatementSegment"),
             Ref("CreateMaterializedViewStatementSegment"),
             Ref("AlterMaterializedViewStatementSegment"),
             Ref("DropMaterializedViewStatementSegment"),
             Ref("RefreshMaterializedViewStatementSegment"),
             Ref("AlterDatabaseStatementSegment"),
             Ref("DropDatabaseStatementSegment"),
+            Ref("VacuumStatementSegment"),
             Ref("AlterFunctionStatementSegment"),
             Ref("CreateViewStatementSegment"),
             Ref("AlterViewStatementSegment"),
             Ref("ListenStatementSegment"),
             Ref("NotifyStatementSegment"),
             Ref("UnlistenStatementSegment"),
             Ref("LoadStatementSegment"),
@@ -3586,14 +4058,17 @@
             Ref("CopyStatementSegment"),
             Ref("DoStatementSegment"),
             Ref("AlterIndexStatementSegment"),
             Ref("ReindexStatementSegment"),
             Ref("AlterRoleStatementSegment"),
             Ref("CreateExtensionStatementSegment"),
             Ref("DropExtensionStatementSegment"),
+            Ref("CreatePublicationStatementSegment"),
+            Ref("AlterPublicationStatementSegment"),
+            Ref("DropPublicationStatementSegment"),
             Ref("CreateTypeStatementSegment"),
             Ref("AlterTypeStatementSegment"),
             Ref("AlterSchemaStatementSegment"),
             Ref("LockTableStatementSegment"),
             Ref("CreateCollationStatementSegment"),
             Ref("CallStoredProcedureSegment"),
         ],
@@ -3748,16 +4223,18 @@
 
     N.B. We keep as a separate segment since the `alias_expression`
     type is required for rules to interpret the alias.
     """
 
     type = "alias_expression"
     match_grammar = Sequence(
+        Indent,
         "AS",
         Ref("SingleIdentifierGrammar"),
+        Dedent,
     )
 
 
 class OperationClassReferenceSegment(ObjectReferenceSegment):
     """A reference to an operation class."""
 
     type = "operation_class_reference"
@@ -3893,34 +4370,42 @@
     )
 
 
 class SetStatementSegment(BaseSegment):
     """Set Statement.
 
     As specified in https://www.postgresql.org/docs/14/sql-set.html
+    Also: https://www.postgresql.org/docs/15/sql-set-role.html (still a VariableSetStmt)
+    https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L1584
     """
 
     type = "set_statement"
 
     match_grammar = Sequence(
         "SET",
         OneOf("SESSION", "LOCAL", optional=True),
         OneOf(
             Sequence(
                 Ref("ParameterNameSegment"),
                 OneOf("TO", Ref("EqualsSegment")),
                 OneOf(
-                    Delimited(Ref("LiteralGrammar"), Ref("NakedIdentifierSegment")),
                     "DEFAULT",
+                    Delimited(
+                        Ref("LiteralGrammar"),
+                        Ref("NakedIdentifierSegment"),
+                        # https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L1810-L1815
+                        Ref("OnKeywordAsIdentifierSegment"),
+                    ),
                 ),
             ),
             Sequence(
                 "TIME", "ZONE", OneOf(Ref("QuotedLiteralSegment"), "LOCAL", "DEFAULT")
             ),
             Sequence("SCHEMA", Ref("QuotedLiteralSegment")),
+            Sequence("ROLE", OneOf("NONE", Ref("RoleReferenceSegment"))),
         ),
     )
 
 
 class CreatePolicyStatementSegment(BaseSegment):
     """A `CREATE POLICY` statement.
 
@@ -4126,20 +4611,21 @@
     )
 
 
 class ResetStatementSegment(BaseSegment):
     """A `RESET` statement.
 
     As Specified in https://www.postgresql.org/docs/14/sql-reset.html
+    Also, RESET ROLE from: https://www.postgresql.org/docs/15/sql-set-role.html
     """
 
     type = "reset_statement"
     match_grammar = Sequence(
         "RESET",
-        OneOf("ALL", Ref("ParameterNameSegment")),
+        OneOf("ALL", "ROLE", Ref("ParameterNameSegment")),
     )
 
 
 class DiscardStatementSegment(BaseSegment):
     """A `DISCARD` statement.
 
     As Specified in https://www.postgresql.org/docs/14/sql-discard.html
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,24 +922,26 @@
     ("CURRENT_USER", "non-reserved"),
     ("CREATEDB", "non-reserved"),
     ("CREATEROLE", "non-reserved"),
     ("DATE", "non-reserved"),
     ("DEPTH", "non-reserved"),
     ("DESCRIBE", "non-reserved"),
     ("DETERMINISTIC", "non-reserved"),
+    ("DISABLE_PAGE_SKIPPING", "non-reserved"),
     ("EXECUTION", "not-keyword"),
     ("EXTENDED", "non-reserved"),
     ("FILE", "non-reserved"),
     ("FORCE_NOT_NULL", "non-reserved"),
     ("FORCE_NULL", "non-reserved"),
     ("FORCE_QUOTE", "non-reserved"),
     ("FORMAT", "non-reserved"),
     ("HASH", "non-reserved"),
     ("ICU", "non-reserved"),
     ("IGNORE", "non-reserved"),
+    ("INDEX_CLEANUP", "non-reserved"),
     ("IS_TEMPLATE", "non-reserved"),
     ("JSON", "non-reserved"),
     ("LC_COLLATE", "non-reserved"),
     ("LC_CTYPE", "non-reserved"),
     ("LIBC", "non-reserved"),
     ("LIST", "non-reserved"),
     ("LOGIN", "non-reserved"),
@@ -950,14 +952,15 @@
     ("NOCREATEDB", "non-reserved"),
     ("NOCREATEROLE", "non-reserved"),
     ("NOINHERIT", "non-reserved"),
     ("NOLOGIN", "non-reserved"),
     ("NOREPLICATION", "non-reserved"),
     ("NOSUPERUSER", "non-reserved"),
     ("PLAIN", "non-reserved"),
+    ("PROCESS_TOAST", "non-reserved"),
     ("PROVIDER", "non-reserved"),
     ("PUBLIC", "non-reserved"),
     ("REMAINDER", "non-reserved"),
     ("REPLICATION", "non-reserved"),
     ("RESPECT", "non-reserved"),
     ("RESTRICTED", "non-reserved"),
     ("SAFE", "non-reserved"),
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 postgres_dialect = load_raw_dialect("postgres")
 ansi_dialect = load_raw_dialect("ansi")
 redshift_dialect = postgres_dialect.copy_as("redshift")
 
 # Set Keywords
 redshift_dialect.sets("unreserved_keywords").clear()
-redshift_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in redshift_unreserved_keywords.split("\n")]
+redshift_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", redshift_unreserved_keywords
 )
 
 redshift_dialect.sets("reserved_keywords").clear()
-redshift_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in redshift_reserved_keywords.split("\n")]
+redshift_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", redshift_reserved_keywords
 )
 
 redshift_dialect.sets("bare_functions").clear()
 redshift_dialect.sets("bare_functions").update(
     [
         "current_date",
         "sysdate",
@@ -1491,34 +1491,34 @@
     )
 
 
 class CreateSchemaStatementSegment(BaseSegment):
     """A `CREATE SCHEMA` statement.
 
     https://docs.aws.amazon.com/redshift/latest/dg/r_CREATE_SCHEMA.html
-    TODO: support optional SCHEMA_ELEMENT
+    TODO: support optional SCHEMA_ELEMENT (should mostly be provided by ansi)
     """
 
     type = "create_schema_statement"
     match_grammar = Sequence(
         "CREATE",
         "SCHEMA",
         OneOf(
             Sequence(
                 Ref("IfNotExistsGrammar", optional=True),
                 Ref("SchemaReferenceSegment"),
                 Sequence(
                     "AUTHORIZATION",
-                    Ref("ObjectReferenceSegment"),
+                    Ref("RoleReferenceSegment"),
                     optional=True,
                 ),
             ),
             Sequence(
                 "AUTHORIZATION",
-                Ref("ObjectReferenceSegment"),
+                Ref("RoleReferenceSegment"),
             ),
         ),
         Ref("QuotaGrammar", optional=True),
     )
 
 
 class ProcedureParameterListSegment(BaseSegment):
@@ -1948,21 +1948,20 @@
                 optional=True,
             ),
             optional=True,
         ),
     )
 
 
-class VacuumStatementSegment(BaseSegment):
+class VacuumStatementSegment(postgres.VacuumStatementSegment):
     """A `VACUUM` statement.
 
     https://docs.aws.amazon.com/redshift/latest/dg/r_VACUUM_command.html
     """
 
-    type = "vacuum_statement"
     match_grammar = Sequence(
         "VACUUM",
         OneOf(
             "FULL",
             "REINDEX",
             "RECLUSTER",
             Sequence(
@@ -2010,15 +2009,14 @@
             Ref("DropDatashareStatementSegment"),
             Ref("ShowDatasharesStatementSegment"),
             Ref("AltereDatashareStatementSegment"),
             Ref("DeclareStatementSegment"),
             Ref("FetchStatementSegment"),
             Ref("CloseStatementSegment"),
             Ref("AnalyzeCompressionStatementSegment"),
-            Ref("VacuumStatementSegment"),
             Ref("AlterProcedureStatementSegment"),
             Ref("CallStatementSegment"),
             Ref("CreateRlsPolicyStatementSegment"),
             Ref("ManageRlsPolicyStatementSegment"),
             Ref("DropRlsPolicyStatementSegment"),
             Ref("CreateExternalFunctionStatementSegment"),
         ],
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -645,21 +645,21 @@
         "FETCH",
         "OFFSET",
     ),
 )
 
 # Add all Snowflake keywords
 snowflake_dialect.sets("unreserved_keywords").clear()
-snowflake_dialect.sets("unreserved_keywords").update(
-    [n.strip().upper() for n in snowflake_unreserved_keywords.split("\n")]
+snowflake_dialect.update_keywords_set_from_multiline_string(
+    "unreserved_keywords", snowflake_unreserved_keywords
 )
 
 snowflake_dialect.sets("reserved_keywords").clear()
-snowflake_dialect.sets("reserved_keywords").update(
-    [n.strip().upper() for n in snowflake_reserved_keywords.split("\n")]
+snowflake_dialect.update_keywords_set_from_multiline_string(
+    "reserved_keywords", snowflake_reserved_keywords
 )
 
 # Add datetime units and their aliases from
 # https://docs.snowflake.com/en/sql-reference/functions-date-time.html#label-supported-date-time-parts
 snowflake_dialect.sets("datetime_units").clear()
 snowflake_dialect.sets("datetime_units").update(
     [
@@ -1007,14 +1007,15 @@
             Ref("ListStatementSegment"),
             Ref("GetStatementSegment"),
             Ref("PutStatementSegment"),
             Ref("RemoveStatementSegment"),
             Ref("CreateDatabaseFromShareStatementSegment"),
             Ref("AlterRoleStatementSegment"),
             Ref("AlterStorageIntegrationSegment"),
+            Ref("ExecuteTaskClauseSegment"),
         ],
         remove=[
             Ref("CreateIndexStatementSegment"),
             Ref("DropIndexStatementSegment"),
         ],
     )
 
@@ -1315,15 +1316,18 @@
 
 class SamplingExpressionSegment(ansi.SamplingExpressionSegment):
     """A sampling expression."""
 
     match_grammar = Sequence(
         OneOf("SAMPLE", "TABLESAMPLE"),
         OneOf("BERNOULLI", "ROW", "SYSTEM", "BLOCK", optional=True),
-        Bracketed(Ref("NumericLiteralSegment"), Ref.keyword("ROWS", optional=True)),
+        Bracketed(
+            OneOf(Ref("NumericLiteralSegment"), Ref("ReferencedVariableNameSegment")),
+            Ref.keyword("ROWS", optional=True),
+        ),
         Sequence(
             OneOf("REPEATABLE", "SEED"),
             Bracketed(Ref("NumericLiteralSegment")),
             optional=True,
         ),
     )
 
@@ -1435,14 +1439,31 @@
 
     parse_grammar = ansi.SelectStatementSegment.parse_grammar.copy(
         insert=[Ref("QualifyClauseSegment", optional=True)],
         before=Ref("OrderByClauseSegment", optional=True),
     )
 
 
+class SelectClauseElementSegment(ansi.SelectClauseElementSegment):
+    """Inherit from ansi but also allow for Snowflake System Functions.
+
+    https://docs.snowflake.com/en/sql-reference/functions-system
+    """
+
+    match_grammar = ansi.SelectClauseElementSegment.match_grammar.copy(
+        insert=[
+            Sequence(
+                Ref("SystemFunctionName"),
+                Bracketed(Ref("QuotedLiteralSegment")),
+            )
+        ],
+        before=Ref("WildcardExpressionSegment"),
+    )
+
+
 class WildcardExpressionSegment(ansi.WildcardExpressionSegment):
     """An extension of the star expression for Snowflake."""
 
     match_grammar = ansi.WildcardExpressionSegment.match_grammar.copy(
         insert=[
             # Optional Exclude or Rename clause
             Ref("ExcludeClauseSegment", optional=True),
@@ -1726,15 +1747,30 @@
                         Sequence(
                             "COLUMN",
                             Ref("ColumnReferenceSegment"),
                             "UNSET",
                             "MASKING",
                             "POLICY",
                         ),
-                        # @TODO: Set/Unset TAG support
+                        Sequence(
+                            "COLUMN",
+                            Ref("ColumnReferenceSegment"),
+                            "SET",
+                            "TAG",
+                            Ref("TagReferenceSegment"),
+                            Ref("EqualsSegment"),
+                            Ref("QuotedLiteralSegment"),
+                        ),
+                        Sequence(
+                            "COLUMN",
+                            Ref("ColumnReferenceSegment"),
+                            "UNSET",
+                            "TAG",
+                            Ref("TagReferenceSegment"),
+                        ),
                     ),
                 ),
             ),
         ),
         # Drop column
         Sequence(
             "DROP",
@@ -3388,18 +3424,58 @@
         Ref("IfNotExistsGrammar", optional=True),
         Ref("ObjectReferenceSegment"),
         # Next set are Notification Integration statements
         # https://docs.snowflake.com/en/sql-reference/sql/create-notification-integration.html
         AnySetOf(
             Sequence("TYPE", Ref("EqualsSegment"), "QUEUE"),
             Sequence("ENABLED", Ref("EqualsSegment"), Ref("BooleanLiteralGrammar")),
+            Sequence(
+                "NOTIFICATION_PROVIDER",
+                Ref("EqualsSegment"),
+                OneOf("AWS_SNS", "AZURE_EVENT_GRID", "GCP_PUBSUB"),
+            ),
+            # AWS specific params:
+            Sequence(
+                "AWS_SNS_TOPIC_ARN",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+            ),
+            Sequence(
+                "AWS_SNS_ROLE_ARN",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+            ),
+            # Azure specific params:
+            Sequence(
+                "AZURE_TENANT_ID", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")
+            ),
             OneOf(
-                Ref("S3NotificationIntegrationParameters"),
-                Ref("GCSNotificationIntegrationParameters"),
-                Ref("AzureNotificationIntegrationParameters"),
+                Sequence(
+                    "AZURE_STORAGE_QUEUE_PRIMARY_URI",
+                    Ref("EqualsSegment"),
+                    Ref("QuotedLiteralSegment"),
+                ),
+                Sequence(
+                    "AZURE_EVENT_GRID_TOPIC_ENDPOINT",
+                    Ref("EqualsSegment"),
+                    Ref("QuotedLiteralSegment"),
+                ),
+            ),
+            # GCP specific params:
+            OneOf(
+                Sequence(
+                    "GCP_PUBSUB_SUBSCRIPTION_NAME",
+                    Ref("EqualsSegment"),
+                    Ref("QuotedLiteralSegment"),
+                ),
+                Sequence(
+                    "GCP_PUBSUB_TOPIC_NAME",
+                    Ref("EqualsSegment"),
+                    Ref("QuotedLiteralSegment"),
+                ),
             ),
             Sequence(
                 "DIRECTION",
                 Ref("EqualsSegment"),
                 "OUTBOUND",
                 optional=True,
             ),
@@ -3430,18 +3506,31 @@
             ),
         ),
         # Next set are Storage Integration statements
         # https://docs.snowflake.com/en/sql-reference/sql/create-storage-integration.html
         AnySetOf(
             Sequence("TYPE", Ref("EqualsSegment"), "EXTERNAL_STAGE"),
             Sequence("ENABLED", Ref("EqualsSegment"), Ref("BooleanLiteralGrammar")),
-            OneOf(
-                Ref("S3StorageIntegrationParameters"),
-                Ref("GCSStorageIntegrationParameters"),
-                Ref("AzureStorageIntegrationParameters"),
+            Sequence(
+                "STORAGE_PROVIDER", Ref("EqualsSegment"), OneOf("S3", "AZURE", "GCS")
+            ),
+            # Azure specific params:
+            Sequence(
+                "AZURE_TENANT_ID", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")
+            ),
+            # AWS specific params:
+            Sequence(
+                "STORAGE_AWS_ROLE_ARN",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+            ),
+            Sequence(
+                "STORAGE_AWS_OBJECT_ACL",
+                Ref("EqualsSegment"),
+                StringParser("'bucket-owner-full-control'", ansi.LiteralSegment),
             ),
             Sequence(
                 "STORAGE_ALLOWED_LOCATIONS",
                 Ref("EqualsSegment"),
                 OneOf(
                     Bracketed(
                         Delimited(
@@ -4693,140 +4782,14 @@
         Ref("StagePath"),
         Ref("S3Path"),
         Ref("GCSPath"),
         Ref("AzureBlobStoragePath"),
     )
 
 
-class S3StorageIntegrationParameters(BaseSegment):
-    """Parameters for an S3 Storage Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-storage-integration.html
-    """
-
-    name = "s3_storage_integration_parameters"
-    type = "storage_integration_parameters"
-
-    match_grammar = AnySetOf(
-        Sequence("STORAGE_PROVIDER", Ref("EqualsSegment"), "S3"),
-        Sequence(
-            "STORAGE_AWS_ROLE_ARN", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")
-        ),
-        Sequence(
-            "STORAGE_AWS_OBJECT_ACL",
-            Ref("EqualsSegment"),
-            StringParser("'bucket-owner-full-control'", ansi.LiteralSegment),
-        ),
-    )
-
-
-class GCSStorageIntegrationParameters(BaseSegment):
-    """Parameters for a GCS Storage Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-storage-integration.html
-    """
-
-    name = "gcs_storage_integration_parameters"
-    type = "storage_integration_parameters"
-
-    match_grammar = Sequence("STORAGE_PROVIDER", Ref("EqualsSegment"), "GCS")
-
-
-class AzureStorageIntegrationParameters(BaseSegment):
-    """Parameters for an Azure Storage Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-storage-integration.html
-    """
-
-    name = "azure_storage_integration_parameters"
-    type = "storage_integration_parameters"
-
-    match_grammar = AnySetOf(
-        Sequence("STORAGE_PROVIDER", Ref("EqualsSegment"), "AZURE"),
-        Sequence("AZURE_TENANT_ID", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")),
-    )
-
-
-class S3NotificationIntegrationParameters(BaseSegment):
-    """Parameters for an S3 Notification Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-notification-integration.html
-    """
-
-    name = "s3_notification_integration_parameters"
-    type = "notification_integration_parameters"
-
-    match_grammar = AnySetOf(
-        Sequence("NOTIFICATION_PROVIDER", Ref("EqualsSegment"), "AWS_SNS"),
-        Sequence(
-            "AWS_SNS_TOPIC_ARN",
-            Ref("EqualsSegment"),
-            Ref("QuotedLiteralSegment"),
-        ),
-        Sequence(
-            "AWS_SNS_ROLE_ARN",
-            Ref("EqualsSegment"),
-            Ref("QuotedLiteralSegment"),
-        ),
-    )
-
-
-class GCSNotificationIntegrationParameters(BaseSegment):
-    """Parameters for a GCS Notification Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-notification-integration.html
-    """
-
-    name = "gcs_notification_integration_parameters"
-    type = "notification_integration_parameters"
-
-    match_grammar = AnySetOf(
-        Sequence("NOTIFICATION_PROVIDER", Ref("EqualsSegment"), "GCP_PUBSUB"),
-        OneOf(
-            Sequence(
-                "GCP_PUBSUB_SUBSCRIPTION_NAME",
-                Ref("EqualsSegment"),
-                Ref("QuotedLiteralSegment"),
-            ),
-            Sequence(
-                "GCP_PUBSUB_TOPIC_NAME",
-                Ref("EqualsSegment"),
-                Ref("QuotedLiteralSegment"),
-            ),
-        ),
-    )
-
-
-class AzureNotificationIntegrationParameters(BaseSegment):
-    """Parameters for an Azure Notification Integration in Snowflake.
-
-    https://docs.snowflake.com/en/sql-reference/sql/create-notification-integration.html
-    """
-
-    name = "azure_notification_integration_parameters"
-    type = "storage_notification_parameters"
-
-    match_grammar = AnySetOf(
-        Sequence("NOTIFICATION_PROVIDER", Ref("EqualsSegment"), "AZURE_EVENT_GRID"),
-        Sequence("AZURE_TENANT_ID", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")),
-        OneOf(
-            Sequence(
-                "AZURE_STORAGE_QUEUE_PRIMARY_URI",
-                Ref("EqualsSegment"),
-                Ref("QuotedLiteralSegment"),
-            ),
-            Sequence(
-                "AZURE_EVENT_GRID_TOPIC_ENDPOINT",
-                Ref("EqualsSegment"),
-                Ref("QuotedLiteralSegment"),
-            ),
-        ),
-    )
-
-
 class InternalStageParameters(BaseSegment):
     """Parameters for an internal stage in Snowflake.
 
     https://docs.snowflake.com/en/sql-reference/sql/create-stage.html
     https://docs.snowflake.com/en/sql-reference/sql/alter-stage.html
     """
 
@@ -5769,14 +5732,32 @@
 
     match_grammar = Sequence(
         "UNSET",
         Delimited(Ref("ParameterNameSegment")),
     )
 
 
+class ExecuteTaskClauseSegment(BaseSegment):
+    """Snowflake's EXECUTE TASK clause.
+
+    ```
+        EXECUTE TASK <name>
+    ```
+
+    https://docs.snowflake.com/en/sql-reference/sql/execute-task
+    """
+
+    type = "execute_task_clause"
+    match_grammar = Sequence(
+        "EXECUTE",
+        "TASK",
+        Ref("ParameterNameSegment"),
+    )
+
+
 ############################
 # MERGE
 ############################
 class MergeUpdateClauseSegment(ansi.MergeUpdateClauseSegment):
     """`UPDATE` clause within the `MERGE` statement."""
 
     match_grammar = Sequence(
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     SymbolSegment,
     Anything,
     StartsWith,
     RegexParser,
     Matchable,
     MultiStringParser,
     StringLexer,
+    AnySetOf,
 )
 from sqlfluff.core.parser.segments.raw import CodeSegment, KeywordSegment
 from sqlfluff.dialects.dialect_sparksql_keywords import (
     RESERVED_KEYWORDS,
     UNRESERVED_KEYWORDS,
 )
 
@@ -151,16 +152,17 @@
     before="code",
 )
 sparksql_dialect.insert_lexer_matchers(
     [
         RegexLexer(
             "file_literal",
             (
-                r"[a-zA-z0-9]*:?([a-zA-Z0-9\-_\.]*(\/|\\))+"
-                r"([a-zA-Z0-9\-_\.]*(:|\?|=|&))*[a-zA-Z0-9\-_\.]*\.?[a-z]*"
+                r"[a-zA-Z0-9]*:?([a-zA-Z0-9\-_\.]*(\/|\\)){2,}"
+                r"((([a-zA-Z0-9\-_\.]*(:|\?|=|&)[a-zA-Z0-9\-_\.]*)+)"
+                r"|([a-zA-Z0-9\-_\.]*\.[a-z]+))"
             ),
             CodeSegment,
             segment_kwargs={"type": "file_literal"},
         ),
     ],
     before="newline",
 )
@@ -226,14 +228,16 @@
         Ref("EqualsSegment_b"),
         Ref("GreaterThanSegment"),
         Ref("LessThanSegment"),
         Ref("GreaterThanOrEqualToSegment"),
         Ref("LessThanOrEqualToSegment"),
         Ref("NotEqualToSegment"),
         Ref("LikeOperatorSegment"),
+        Sequence("IS", "DISTINCT", "FROM"),
+        Sequence("IS", "NOT", "DISTINCT", "FROM"),
     ),
     FromClauseTerminatorGrammar=OneOf(
         "WHERE",
         "LIMIT",
         Sequence("GROUP", "BY"),
         Sequence("ORDER", "BY"),
         Sequence("CLUSTER", "BY"),
@@ -507,20 +511,14 @@
         Sequence(
             "INPUTFORMAT",
             Ref("QuotedLiteralSegment"),
             "OUTPUTFORMAT",
             Ref("QuotedLiteralSegment"),
         ),
     ),
-    DataSourceFormatGrammar=OneOf(
-        Ref("FileFormatGrammar"),
-        # NB: JDBC is part of DataSourceV2 but not included
-        # there since there are no significant syntax changes
-        "JDBC",
-    ),
     TimestampAsOfGrammar=Sequence(
         "TIMESTAMP",
         "AS",
         "OF",
         OneOf(
             Ref("QuotedLiteralSegment"),
             Ref("BareFunctionSegment"),
@@ -548,18 +546,52 @@
                     Ref("ColumnDefinitionSegment"),
                     Sequence(
                         Ref("ColumnReferenceSegment"),
                         Ref("EqualsSegment", optional=True),
                         Ref("LiteralGrammar", optional=True),
                         Ref("CommentGrammar", optional=True),
                     ),
+                    Ref("IcebergTransformationSegment", optional=True),
                 ),
             ),
         ),
     ),
+    PartitionFieldGrammar=Sequence(
+        "PARTITION",
+        "FIELD",
+        Delimited(
+            OneOf(
+                Ref("ColumnDefinitionSegment"),
+                Sequence(
+                    Ref("ColumnReferenceSegment"),
+                    Ref("EqualsSegment", optional=True),
+                    Ref("LiteralGrammar", optional=True),
+                    Ref("CommentGrammar", optional=True),
+                ),
+                Ref("IcebergTransformationSegment", optional=True),
+            ),
+        ),
+        Sequence(
+            Ref.keyword("WITH", optional=True),
+            Delimited(
+                OneOf(
+                    Ref("ColumnDefinitionSegment"),
+                    Sequence(
+                        Ref("ColumnReferenceSegment"),
+                        Ref("EqualsSegment", optional=True),
+                        Ref("LiteralGrammar", optional=True),
+                        Ref("CommentGrammar", optional=True),
+                    ),
+                    Ref("IcebergTransformationSegment", optional=True),
+                ),
+            ),
+            optional=True,
+        ),
+        Sequence("AS", Ref("NakedIdentifierSegment"), optional=True),
+    ),
     # NB: Redefined from `NakedIdentifierSegment` which uses an anti-template to
     # not match keywords; however, SparkSQL allows keywords to be used in table
     # and runtime properties.
     PropertiesNakedIdentifierSegment=RegexParser(
         r"[A-Z0-9]*[A-Z][A-Z0-9]*",
         ansi.IdentifierSegment,
         type="properties_naked_identifier",
@@ -657,14 +689,73 @@
         CodeSegment,
         type="widget_name_identifier",
     ),
     WidgetDefaultGrammar=Sequence(
         "DEFAULT",
         Ref("QuotedLiteralSegment"),
     ),
+    TableDefinitionSegment=Sequence(
+        OneOf(Ref("OrReplaceGrammar"), Ref("OrRefreshGrammar"), optional=True),
+        Ref("TemporaryGrammar", optional=True),
+        Ref.keyword("EXTERNAL", optional=True),
+        Ref.keyword("STREAMING", optional=True),
+        Ref.keyword("LIVE", optional=True),
+        "TABLE",
+        Ref("IfNotExistsGrammar", optional=True),
+        OneOf(
+            Ref("FileReferenceSegment"),
+            Ref("TableReferenceSegment"),
+        ),
+        OneOf(
+            # Columns and comment syntax:
+            Bracketed(
+                Delimited(
+                    Sequence(
+                        OneOf(
+                            Ref("ColumnDefinitionSegment"),
+                            Ref("GeneratedColumnDefinitionSegment"),
+                        ),
+                        Ref("CommentGrammar", optional=True),
+                    ),
+                ),
+            ),
+            # Like Syntax
+            Sequence(
+                "LIKE",
+                OneOf(
+                    Ref("FileReferenceSegment"),
+                    Ref("TableReferenceSegment"),
+                ),
+            ),
+            optional=True,
+        ),
+        Ref("UsingClauseSegment", optional=True),
+        AnySetOf(
+            Ref("RowFormatClauseSegment"),
+            Ref("StoredAsGrammar"),
+            Ref("CommentGrammar"),
+            Ref("OptionsGrammar"),
+            Ref("PartitionSpecGrammar"),
+            Ref("BucketSpecGrammar"),
+            optional=True,
+        ),
+        Indent,
+        AnyNumberOf(
+            Ref("LocationGrammar", optional=True),
+            Ref("CommentGrammar", optional=True),
+            Ref("TablePropertiesGrammar", optional=True),
+        ),
+        Dedent,
+        # Create AS syntax:
+        Sequence(
+            Ref.keyword("AS", optional=True),
+            OptionallyBracketed(Ref("SelectableGrammar")),
+            optional=True,
+        ),
+    ),
 )
 
 # Adding Hint related grammar before comment `block_comment` and
 # `single_quote` so they are applied before comment lexer so
 # hints are treated as such instead of comments when parsing.
 # https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-hints.html
 sparksql_dialect.insert_lexer_matchers(
@@ -793,15 +884,15 @@
     match_grammar = OneOf(
         Ref("PrimitiveTypeSegment"),
         Ref("ArrayTypeSegment"),
         Sequence(
             "MAP",
             Bracketed(
                 Sequence(
-                    Ref("PrimitiveTypeSegment"),
+                    Ref("DatatypeSegment"),
                     Ref("CommaSegment"),
                     Ref("DatatypeSegment"),
                 ),
                 bracket_pairs_set="angle_bracket_pairs",
                 bracket_type="angle",
             ),
         ),
@@ -852,23 +943,31 @@
             # ALTER TABLE - RENAME `partition_spec`
             Sequence(
                 Ref("PartitionSpecGrammar"),
                 "RENAME",
                 "TO",
                 Ref("PartitionSpecGrammar"),
             ),
+            # ALTER TABLE - RENAME TO 'column_identifier'
+            Sequence(
+                "RENAME",
+                "COLUMN",
+                Ref("ColumnReferenceSegment"),
+                "TO",
+                Ref("ColumnReferenceSegment"),
+            ),
             # ALTER TABLE - ADD COLUMNS
             Sequence(
                 "ADD",
-                "COLUMNS",
+                OneOf("COLUMNS", "COLUMN"),
                 Indent,
                 OptionallyBracketed(
                     Delimited(
                         Sequence(
-                            Ref("ColumnDefinitionSegment"),
+                            Ref("ColumnFieldDefinitionSegment"),
                             OneOf(
                                 "FIRST",
                                 Sequence(
                                     "AFTER",
                                     Ref("ColumnReferenceSegment"),
                                 ),
                                 optional=True,
@@ -942,23 +1041,34 @@
                     ),
                 ),
             ),
             # ALTER TABLE - ADD PARTITION
             Sequence(
                 "ADD",
                 Ref("IfNotExistsGrammar", optional=True),
-                AnyNumberOf(Ref("PartitionSpecGrammar"), min_times=1),
+                AnyNumberOf(
+                    Ref("PartitionSpecGrammar"),
+                    Ref("PartitionFieldGrammar"),
+                    min_times=1,
+                ),
             ),
             # ALTER TABLE - DROP PARTITION
             Sequence(
                 "DROP",
                 Ref("IfExistsGrammar", optional=True),
-                Ref("PartitionSpecGrammar"),
+                OneOf(
+                    Ref("PartitionSpecGrammar"),
+                    Ref("PartitionFieldGrammar"),
+                ),
                 Sequence("PURGE", optional=True),
             ),
+            Sequence(
+                "Replace",
+                Ref("PartitionFieldGrammar"),
+            ),
             # ALTER TABLE - REPAIR PARTITION
             Sequence("RECOVER", "PARTITIONS"),
             # ALTER TABLE - SET PROPERTIES
             Sequence("SET", Ref("TablePropertiesGrammar")),
             # ALTER TABLE - UNSET PROPERTIES
             Ref("UnsetTablePropertiesGrammar"),
             # ALTER TABLE - SET SERDE
@@ -978,15 +1088,15 @@
                 ),
             ),
             # ALTER TABLE - SET FILE FORMAT
             Sequence(
                 Ref("PartitionSpecGrammar", optional=True),
                 "SET",
                 "FILEFORMAT",
-                Ref("DataSourceFormatGrammar"),
+                Ref("DataSourceFormatSegment"),
             ),
             # ALTER TABLE - CHANGE FILE LOCATION
             Sequence(
                 Ref("PartitionSpecGrammar"),
                 "SET",
                 Ref("LocationGrammar"),
             ),
@@ -999,19 +1109,93 @@
                     "ColumnReferenceSegment",
                     exclude=Ref.keyword("CHECK"),
                 ),
                 Ref.keyword("CHECK", optional=True),
                 Bracketed(Ref("ExpressionSegment"), optional=True),
                 Dedent,
             ),
+            # ALTER TABLE - ICEBERG WRITE ORDER / DISTRIBUTION
+            # https://iceberg.apache.org/docs/latest/spark-ddl/#alter-table--write-ordered-by
+            Sequence(
+                "WRITE",
+                AnyNumberOf(
+                    Sequence("DISTRIBUTED", "BY", "PARTITION", optional=True),
+                    Sequence(
+                        Ref.keyword("LOCALLY", optional=True),
+                        "ORDERED",
+                        "BY",
+                        Indent,
+                        Delimited(
+                            Sequence(
+                                Ref("ColumnReferenceSegment"),
+                                OneOf("ASC", "DESC", optional=True),
+                                # NB: This isn't really ANSI, and isn't supported
+                                # in Mysql,but is supported in enough other dialects
+                                # for it to make sense here for now.
+                                Sequence(
+                                    "NULLS", OneOf("FIRST", "LAST"), optional=True
+                                ),
+                            ),
+                            optional=True,
+                        ),
+                        Dedent,
+                        optional=True,
+                    ),
+                    min_times=1,
+                    max_times_per_element=1,
+                ),
+            ),
+            # ALTER TABLE - ICEBERG SET IDENTIFIER FIELDS
+            Sequence(
+                "SET",
+                "IDENTIFIER",
+                "FIELDS",
+                Indent,
+                Delimited(
+                    Sequence(
+                        Ref("ColumnReferenceSegment"),
+                    ),
+                ),
+                Dedent,
+            ),
+            # ALTER TABLE - ICEBERG DROP IDENTIFIER FIELDS
+            Sequence(
+                "DROP",
+                "IDENTIFIER",
+                "FIELDS",
+                Indent,
+                Delimited(
+                    Sequence(
+                        Ref("ColumnReferenceSegment"),
+                    ),
+                ),
+                Dedent,
+            ),
         ),
         Dedent,
     )
 
 
+class ColumnFieldDefinitionSegment(ansi.ColumnDefinitionSegment):
+    """A column field definition, e.g. for CREATE TABLE or ALTER TABLE.
+
+    This supports the iceberg syntax and allows for iceberg syntax such
+    as ADD COLUMN a.b.
+    """
+
+    match_grammar: Matchable = Sequence(
+        Ref("ColumnReferenceSegment"),  # Column name
+        Ref("DatatypeSegment"),  # Column type
+        Bracketed(Anything(), optional=True),  # For types like VARCHAR(100)
+        AnyNumberOf(
+            Ref("ColumnConstraintSegment", optional=True),
+        ),
+    )
+
+
 class AlterViewStatementSegment(BaseSegment):
     """A `ALTER VIEW` statement to change the view schema or properties.
 
     https://spark.apache.org/docs/latest/sql-ref-syntax-ddl-alter-view.html
     """
 
     type = "alter_view_statement"
@@ -1078,69 +1262,15 @@
     """A `CREATE TABLE` statement using a Data Source or Like.
 
     http://spark.apache.org/docs/latest/sql-ref-syntax-ddl-create-table-datasource.html
     https://spark.apache.org/docs/latest/sql-ref-syntax-ddl-create-table-like.html
     https://docs.delta.io/latest/delta-batch.html#create-a-table
     """
 
-    match_grammar = Sequence(
-        "CREATE",
-        OneOf(Ref("OrReplaceGrammar"), Ref("OrRefreshGrammar"), optional=True),
-        Ref("TemporaryGrammar", optional=True),
-        Ref.keyword("STREAMING", optional=True),
-        Ref.keyword("LIVE", optional=True),
-        "TABLE",
-        Ref("IfNotExistsGrammar", optional=True),
-        OneOf(
-            Ref("FileReferenceSegment"),
-            Ref("TableReferenceSegment"),
-        ),
-        OneOf(
-            # Columns and comment syntax:
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        OneOf(
-                            Ref("ColumnDefinitionSegment"),
-                            Ref("GeneratedColumnDefinitionSegment"),
-                        ),
-                        Ref("CommentGrammar", optional=True),
-                    ),
-                ),
-            ),
-            # Like Syntax
-            Sequence(
-                "LIKE",
-                OneOf(
-                    Ref("FileReferenceSegment"),
-                    Ref("TableReferenceSegment"),
-                ),
-            ),
-            optional=True,
-        ),
-        Sequence("USING", Ref("DataSourceFormatGrammar"), optional=True),
-        Ref("RowFormatClauseSegment", optional=True),
-        Ref("StoredAsGrammar", optional=True),
-        Ref("OptionsGrammar", optional=True),
-        Ref("PartitionSpecGrammar", optional=True),
-        Ref("BucketSpecGrammar", optional=True),
-        Indent,
-        AnyNumberOf(
-            Ref("LocationGrammar", optional=True),
-            Ref("CommentGrammar", optional=True),
-            Ref("TablePropertiesGrammar", optional=True),
-        ),
-        Dedent,
-        # Create AS syntax:
-        Sequence(
-            Ref.keyword("AS", optional=True),
-            OptionallyBracketed(Ref("SelectableGrammar")),
-            optional=True,
-        ),
-    )
+    match_grammar = Sequence("CREATE", Ref("TableDefinitionSegment"))
 
 
 class CreateHiveFormatTableStatementSegment(hive.CreateTableStatementSegment):
     """A `CREATE TABLE` statement using Hive format.
 
     https://spark.apache.org/docs/latest/sql-ref-syntax-ddl-create-table-hiveformat.html
     """
@@ -1171,18 +1301,19 @@
                         Ref("ColumnReferenceSegment"),
                         Ref("CommentGrammar", optional=True),
                     ),
                 ),
             ),
             optional=True,
         ),
+        Sequence("USING", Ref("DataSourceFormatSegment"), optional=True),
+        Ref("OptionsGrammar", optional=True),
         Ref("CommentGrammar", optional=True),
         Ref("TablePropertiesGrammar", optional=True),
-        "AS",
-        OptionallyBracketed(Ref("SelectableGrammar")),
+        Sequence("AS", OptionallyBracketed(Ref("SelectableGrammar")), optional=True),
         Ref("WithNoSchemaBindingClauseSegment", optional=True),
     )
 
 
 class CreateWidgetStatementSegment(BaseSegment):
     """A `CREATE WIDGET` STATEMENT.
 
@@ -1204,14 +1335,24 @@
             Sequence(
                 "TEXT", Ref("WidgetNameIdentifierSegment"), Ref("WidgetDefaultGrammar")
             ),
         ),
     )
 
 
+class ReplaceTableStatementSegment(BaseSegment):
+    """A `REPLACE TABLE` statement using the iceberg table format.
+
+    https://iceberg.apache.org/docs/latest/spark-ddl/#replace-table--as-select
+    """
+
+    type = "replace_table_statement"
+    match_grammar = Sequence("REPLACE", Ref("TableDefinitionSegment"))
+
+
 class RemoveWidgetStatementSegment(BaseSegment):
     """A `REMOVE WIDGET` STATEMENT.
 
     https://docs.databricks.com/notebooks/widgets.html#databricks-widget-api
     """
 
     type = "remove_widget_statement"
@@ -1350,15 +1491,15 @@
     match_grammar = Sequence(
         "INSERT",
         "OVERWRITE",
         Ref.keyword("LOCAL", optional=True),
         "DIRECTORY",
         Ref("QuotedLiteralSegment", optional=True),
         "USING",
-        Ref("DataSourceFormatGrammar"),
+        Ref("DataSourceFormatSegment"),
         Ref("OptionsGrammar", optional=True),
         OneOf(
             AnyNumberOf(
                 Ref("ValuesClauseSegment"),
                 min_times=1,
             ),
             Ref("SelectableGrammar"),
@@ -1469,14 +1610,15 @@
     """
 
     type = "distribute_by_clause"
 
     match_grammar = StartsWith(
         Sequence("DISTRIBUTE", "BY"),
         terminator=OneOf(
+            "SORT",
             "LIMIT",
             "HAVING",
             # For window functions
             "WINDOW",
             Ref("FrameClauseUnitGrammar"),
             "SEPARATOR",
         ),
@@ -1496,14 +1638,15 @@
                     Ref("ExpressionSegment"),
                 ),
             ),
             terminator=OneOf(
                 "WINDOW",
                 "LIMIT",
                 Ref("FrameClauseUnitGrammar"),
+                "SORT",
             ),
         ),
         Dedent,
     )
 
 
 class HintFunctionSegment(BaseSegment):
@@ -1517,14 +1660,16 @@
     match_grammar = Sequence(
         Ref("FunctionNameSegment"),
         Bracketed(
             Delimited(
                 AnyNumberOf(
                     Ref("SingleIdentifierGrammar"),
                     Ref("NumericLiteralSegment"),
+                    Ref("TableReferenceSegment"),
+                    Ref("ColumnReferenceSegment"),
                     min_times=1,
                 ),
             ),
             # May be Bare Function unique to Hints, i.e. REBALANCE
             optional=True,
         ),
     )
@@ -1675,34 +1820,60 @@
         enforce_whitespace_preceding_terminator=True,
     )
 
     parse_grammar = Sequence(
         "GROUP",
         "BY",
         Indent,
-        Delimited(
-            OneOf(
+        OneOf(
+            Delimited(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
                 Ref("NumericLiteralSegment"),
                 # Can `GROUP BY coalesce(col, 1)`
                 Ref("ExpressionSegment"),
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingSetsClauseSegment"),
             ),
-            terminator=Ref("GroupByClauseTerminatorGrammar"),
+            Sequence(
+                Delimited(
+                    Ref("ColumnReferenceSegment"),
+                    # Can `GROUP BY 1`
+                    Ref("NumericLiteralSegment"),
+                    # Can `GROUP BY coalesce(col, 1)`
+                    Ref("ExpressionSegment"),
+                ),
+                OneOf(
+                    Ref("WithCubeRollupClauseSegment"), Ref("GroupingSetsClauseSegment")
+                ),
+            ),
         ),
-        # TODO: New Rule
-        #  Warn if CubeRollupClauseSegment and
-        #  WithCubeRollupClauseSegment used in same query
-        Ref("WithCubeRollupClauseSegment", optional=True),
         Dedent,
     )
 
 
+class OrderByClauseSegment(ansi.OrderByClauseSegment):
+    """A `ORDER BY` clause like in `SELECT`."""
+
+    match_grammar = ansi.OrderByClauseSegment.match_grammar.copy()
+    match_grammar.terminator = OneOf(  # type: ignore
+        "CLUSTER",
+        "DISTRIBUTE",
+        "SORT",
+        "LIMIT",
+        "HAVING",
+        "QUALIFY",
+        # For window functions
+        "WINDOW",
+        Ref("FrameClauseUnitGrammar"),
+        "SEPARATOR",
+    )
+    parse_grammar = ansi.OrderByClauseSegment.parse_grammar
+
+
 class WithCubeRollupClauseSegment(BaseSegment):
     """A `[WITH CUBE | WITH ROLLUP]` clause after the `GROUP BY` clause.
 
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-groupby.html
     """
 
     type = "with_cube_rollup_clause"
@@ -1866,25 +2037,17 @@
 
     match_grammar = Sequence(
         Indent,
         "LATERAL",
         "VIEW",
         Ref.keyword("OUTER", optional=True),
         Ref("FunctionSegment"),
-        # NB: AliasExpressionSegment is not used here for table
-        # or column alias because `AS` is optional within it
-        # (and in most scenarios). Here it's explicitly defined
-        # for when it is required and not allowed.
+        # This allows for a table name to precede the alias expression.
         Ref("SingleIdentifierGrammar", optional=True),
-        Sequence(
-            "AS",
-            Delimited(
-                Ref("SingleIdentifierGrammar"),
-            ),
-        ),
+        Ref("AliasExpressionSegment", optional=True),
         Dedent,
     )
 
 
 class PivotClauseSegment(BaseSegment):
     """A `PIVOT` clause as using in FROM clause.
 
@@ -2499,14 +2662,15 @@
             Ref("RestoreTableStatementSegment"),
             # Databricks - Delta Live Tables
             Ref("ConstraintStatementSegment"),
             Ref("ApplyChangesIntoStatementSegment"),
             # Databricks - widgets
             Ref("CreateWidgetStatementSegment"),
             Ref("RemoveWidgetStatementSegment"),
+            Ref("ReplaceTableStatementSegment"),
         ],
         remove=[
             Ref("TransactionStatementSegment"),
             Ref("CreateSchemaStatementSegment"),
             Ref("SetSchemaStatementSegment"),
             Ref("CreateModelStatementSegment"),
             Ref("DropModelStatementSegment"),
@@ -3150,7 +3314,90 @@
             "LIMIT",
             "OVERLAPS",
         ),
         enforce_whitespace_preceding_terminator=True,
     )
 
     parse_grammar: Matchable = Ref("SelectClauseSegmentGrammar")
+
+
+class UsingClauseSegment(BaseSegment):
+    """`USING` clause segment."""
+
+    type = "using_clause"
+    match_grammar = Sequence("USING", Ref("DataSourceFormatSegment"))
+
+
+class DataSourceFormatSegment(BaseSegment):
+    """Data source format segment."""
+
+    type = "data_source_format"
+    match_grammar = OneOf(
+        Ref("FileFormatGrammar"),
+        # NB: JDBC is part of DataSourceV2 but not included
+        # there since there are no significant syntax changes
+        "JDBC",
+        Ref(
+            "ObjectReferenceSegment"
+        ),  # This allows for formats such as org.apache.spark.sql.jdbc
+    )
+
+
+class IcebergTransformationSegment(BaseSegment):
+    """A Transformation expressions used in PARTITIONED BY.
+
+    This segment is to be used in creating hidden partitions
+    in the iceberg table format.
+    https://iceberg.apache.org/docs/latest/spark-ddl/#partitioned-by
+    """
+
+    type = "iceberg_transformation"
+    match_grammar = OneOf(
+        Sequence(
+            OneOf(
+                "YEARS",
+                "MONTHS",
+                "DAYS",
+                "DATE",
+                "HOURS",
+                "DATE_HOUR",
+            ),
+            Bracketed(Ref("ColumnReferenceSegment")),
+        ),
+        Sequence(
+            OneOf("BUCKET", "TRUNCATE"),
+            Bracketed(
+                Sequence(
+                    Ref("NumericLiteralSegment"),
+                    Ref("CommaSegment"),
+                    Ref("ColumnReferenceSegment"),
+                )
+            ),
+        ),
+    )
+
+
+class FrameClauseSegment(ansi.FrameClauseSegment):
+    """A frame clause for window functions.
+
+    This overrides the ansi dialect frame clause segment as the sparksql
+    frame clause allows for a more expressive frame syntax.
+    https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-window.html
+    """
+
+    type = "frame_clause"
+    _frame_extent = OneOf(
+        Sequence("CURRENT", "ROW"),
+        Sequence(
+            OneOf(
+                Ref("NumericLiteralSegment"),
+                "UNBOUNDED",
+                Ref("IntervalExpressionSegment"),
+            ),
+            OneOf("PRECEDING", "FOLLOWING"),
+        ),
+    )
+
+    match_grammar: Matchable = Sequence(
+        Ref("FrameClauseUnitGrammar"),
+        OneOf(_frame_extent, Sequence("BETWEEN", _frame_extent, "AND", _frame_extent)),
+    )
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     "CONSTRAINT",
     "CREATE",
     "CROSS",
     "CURRENT_DATE",
     "CURRENT_TIME",
     "CURRENT_TIMESTAMP",
     "CURRENT_USER",
-    "DISTINCT",
     "ELSE",
     "END",
     "ESCAPE",
     "EXCEPT",
     "FALSE",
     "FETCH",
     "FILTER",
@@ -104,48 +103,56 @@
     "COMPACTIONS",
     "COMPUTE",
     "CONCATENATE",
     "COST",
     "CUBE",
     "CURRENT",
     "DATA",
+    "DATE",
+    "DATE_HOUR",
     "DATABASE",
     "DATABASES",
     "DAY",
+    "DAYS",
     "DBPROPERTIES",
     "DEFINED",
     "DELETE",
     "DELIMITED",
     "DESC",
     "DESCRIBE",
     "DFS",
     "DIRECTORIES",
     "DIRECTORY",
+    "DISTINCT",
     "DISTRIBUTE",
+    "DISTRIBUTED",
     "DIV",
     "DROP",
     "ESCAPED",
     "EXCHANGE",
     "EXISTS",
     "EXPLAIN",
     "EXPORT",
     "EXTENDED",
     "EXTERNAL",
     "EXTRACT",
+    "FIELD",
     "FIELDS",
     "FILEFORMAT",
     "FIRST",
     "FOLLOWING",
     "FORMAT",
     "FORMATTED",
     "FUNCTION",
     "FUNCTIONS",
     "GLOBAL",
     "GROUPING",
     "HOUR",
+    "HOURS",
+    "IDENTIFIER",
     "IF",
     "IGNORE",
     "ILIKE",
     "IMPORT",
     "INDEX",
     "INDEXES",
     "INPATH",
@@ -158,32 +165,35 @@
     "LAZY",
     "LIKE",
     "LIMIT",
     "LINES",
     "LIST",
     "LOAD",
     "LOCAL",
+    "LOCALLY",
     "LOCATION",
     "LOCK",
     "LOCKS",
     "LOGICAL",
     "MACRO",
     "MAP",
     "MATCHED",
     "MERGE",
     "MINUTE",
     "MONTH",
+    "MONTHS",
     "MSCK",
     "NAMESPACE",
     "NAMESPACES",
     "NO",
     "NULLS",
     "OF",
     "OPTION",
     "OPTIONS",
+    "ORDERED",
     "OUT",
     "OUTPUTFORMAT",
     "OVER",
     "OVERLAY",
     "OVERWRITE",
     "PARTITION",
     "PARTITIONED",
@@ -263,16 +273,18 @@
     "UNLOCK",
     "UNSET",
     "UPDATE",
     "USE",
     "VALUES",
     "VIEW",
     "VIEWS",
+    "WRITE",
     "WINDOW",
     "YEAR",
+    "YEARS",
     "ZONE",
     # Spark Core Data Sources
     # https://spark.apache.org/docs/latest/sql-data-sources.html
     "AVRO",
     "CSV",
     "JSON",
     "PARQUET",
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -4341,15 +4341,15 @@
     type = "create_schema_statement"
     match_grammar = Sequence(
         "CREATE",
         "SCHEMA",
         Ref("SchemaReferenceSegment"),
         Sequence(
             "AUTHORIZATION",
-            Ref("SingleIdentifierGrammar"),
+            Ref("RoleReferenceSegment"),
             optional=True,
         ),
         Ref(
             "DelimiterGrammar",
             optional=True,
         ),
     )
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.0.4/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,46 +57,58 @@
         it contains an AS keyword. This is the _eval function for both AL01 and AL02.
         """
         # Config type hints
         self.aliasing: str
 
         assert context.segment.is_type("alias_expression")
         if context.parent_stack[-1].is_type(*self._target_parent_types):
-            if any(e.raw_upper == "AS" for e in context.segment.segments):
+            # Search for an AS keyword.
+            for as_keyword in context.segment.segments:
+                if as_keyword.raw_upper == "AS":
+                    break
+            else:
+                as_keyword = None
+
+            if as_keyword:
                 if self.aliasing == "implicit":
-                    if context.segment.segments[0].raw_upper == "AS":
-                        self.logger.debug("Removing AS keyword and respacing.")
-                        as_keyword = context.segment.segments[0]
-                        return LintResult(
-                            anchor=as_keyword,
-                            # Generate the fixes to remove and respace accordingly.
-                            fixes=ReflowSequence.from_around_target(
-                                as_keyword,
-                                context.parent_stack[0],
-                                config=context.config,
-                            )
-                            .without(as_keyword)
-                            .respace()
-                            .get_fixes(),
+                    self.logger.debug("Removing AS keyword and respacing.")
+                    return LintResult(
+                        anchor=as_keyword,
+                        # Generate the fixes to remove and respace accordingly.
+                        fixes=ReflowSequence.from_around_target(
+                            as_keyword,
+                            context.parent_stack[0],
+                            config=context.config,
                         )
+                        .without(as_keyword)
+                        .respace()
+                        .get_fixes(),
+                    )
 
             elif self.aliasing != "implicit":
                 self.logger.debug("Inserting AS keyword and respacing.")
+                for identifier in context.segment.raw_segments:
+                    if identifier.is_code:
+                        break
+                else:  # pragma: no cover
+                    raise NotImplementedError(
+                        "Failed to find identifier. Raise this as a bug on GitHub."
+                    )
                 return LintResult(
                     anchor=context.segment,
                     # Work out the insertion and reflow fixes.
                     fixes=ReflowSequence.from_around_target(
-                        context.segment.raw_segments[0],
+                        identifier,
                         context.parent_stack[0],
                         config=context.config,
                         # Only reflow before, otherwise we catch too much.
                         sides="before",
                     )
                     .insert(
                         KeywordSegment("AS"),
-                        target=context.segment.raw_segments[0],
+                        target=identifier,
                         pos="before",
                     )
                     .respace()
                     .get_fixes(),
                 )
         return None
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     """
 
     name = "ambiguous.union"
     aliases = ("L033",)
     groups: Tuple[str, ...] = ("all", "core", "ambiguous")
     crawl_behaviour = SegmentSeekerCrawler({"set_operator"})
+    is_fix_compatible = True
 
     def _eval(self, context: RuleContext) -> LintResult:
         """Look for UNION keyword not immediately followed by DISTINCT or ALL.
 
         Note that UNION DISTINCT is valid, rule only applies to bare UNION.
         The function does this by looking for a segment of type set_operator
         which has a UNION but no DISTINCT or ALL.
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,48 +82,53 @@
         # Used by CP03 (that inherits from this rule)
         # If it's a qualified function_name (i.e with more than one part to
         # function_name). Then it is likely an existing user defined function (UDF)
         # which are case sensitive so ignore for this.
         if parent.get_type() == "function_name" and len(parent.segments) != 1:
             return [LintResult(memory=context.memory)]
 
-        return [self._handle_segment(context.segment, context.memory)]
+        return [self._handle_segment(context.segment, context)]
 
-    def _handle_segment(self, segment, memory) -> LintResult:
+    def _handle_segment(self, segment, context: RuleContext) -> LintResult:
         # NOTE: this mutates the memory field.
+        memory = context.memory
         self.logger.info("_handle_segment: %s, %s", segment, segment.get_type())
         # Config type hints
         self.ignore_words_regex: str
 
         # Get the capitalisation policy configuration.
         try:
             cap_policy = self.cap_policy
             cap_policy_opts = self.cap_policy_opts
             ignore_words_list = self.ignore_words_list
+            ignore_templated_areas = self.ignore_templated_areas
         except AttributeError:
             # First-time only, read the settings from configuration. This is
             # very slow.
             (
                 cap_policy,
                 cap_policy_opts,
                 ignore_words_list,
-            ) = self._init_capitalisation_policy()
+                ignore_templated_areas,
+            ) = self._init_capitalisation_policy(context)
 
         # Skip if in ignore list
         if ignore_words_list and segment.raw.lower() in ignore_words_list:
             return LintResult(memory=memory)
 
         # Skip if matches ignore regex
         if self.ignore_words_regex and regex.search(
             self.ignore_words_regex, segment.raw
         ):
             return LintResult(memory=memory)
 
-        # Skip if templated.
-        if segment.is_templated:
+        # Skip if templated.  If the user wants to ignore templated areas, we don't
+        # even want to look at them to avoid affecting flagging non-template areas
+        # that are inconsistent with the template areas.
+        if segment.is_templated and ignore_templated_areas:
             return LintResult(memory=memory)
 
         # Skip if empty.
         if not segment.raw:
             return LintResult(memory=memory)
 
         refuted_cases = memory.get("refuted_cases", set())
@@ -246,15 +251,15 @@
         """Given a segment found to have a fix, returns a LintFix for it.
 
         May be overridden by subclasses, which is useful when the parse tree
         structure varies from this simple base case.
         """
         return LintFix.replace(segment, [segment.edit(fixed_raw)])
 
-    def _init_capitalisation_policy(self):
+    def _init_capitalisation_policy(self, context: RuleContext):
         """Called first time rule is evaluated to fetch & cache the policy."""
         cap_policy_name = next(
             k for k in self.config_keywords if k.endswith("capitalisation_policy")
         )
         self.cap_policy = getattr(self, cap_policy_name)
         self.cap_policy_opts = [
             opt
@@ -265,15 +270,17 @@
         ignore_words_config = str(getattr(self, "ignore_words"))
         if ignore_words_config and ignore_words_config != "None":
             self.ignore_words_list = self.split_comma_separated_string(
                 ignore_words_config.lower()
             )
         else:
             self.ignore_words_list = []
+        self.ignore_templated_areas = context.config.get("ignore_templated_areas")
         self.logger.debug(
             f"Selected '{cap_policy_name}': '{self.cap_policy}' from options "
             f"{self.cap_policy_opts}"
         )
         cap_policy = self.cap_policy
         cap_policy_opts = self.cap_policy_opts
         ignore_words_list = self.ignore_words_list
-        return cap_policy, cap_policy_opts, ignore_words_list
+        ignore_templated_areas = self.ignore_templated_areas
+        return cap_policy, cap_policy_opts, ignore_words_list, ignore_templated_areas
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,22 +79,22 @@
             for seg in context.segment.segments:
                 # We don't want to edit symbols, quoted things or identifiers
                 # if they appear.
                 if seg.is_type(
                     "symbol", "identifier", "quoted_literal"
                 ) or not seg.is_type("raw"):
                     continue
-                res = self._handle_segment(seg, context.memory)
+                res = self._handle_segment(seg, context)
                 if res:
                     results.append(res)
 
         # NOTE: Given the dialect structure we can assume the targets have a parent.
         parent: BaseSegment = context.parent_stack[-1]
         # Don't process it if it's likely to have been processed by the parent.
         if context.segment.is_type("data_type_identifier") and not parent.is_type(
             "primitive_type", "datetime_type_identifier", "data_type"
         ):
             results.append(
-                self._handle_segment(context.segment, context.memory)
+                self._handle_segment(context.segment, context)
             )  # pragma: no cover
 
         return results
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV05.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,24 @@
 
         # Allow assignments in EXEC clauses, or any other explicit assignments
         if context.parent_stack and context.parent_stack[-1].is_type(
             "set_clause_list", "execute_script_statement", "assignment_operator"
         ):
             return None
 
+        # If the operator is in an EXCLUDE constraint (PostgreSQL feature), the SQL
+        # could look like: EXCLUDE (field WITH =).  In that case, we can exit early
+        # to avoid an assertion failure due to no segment following the operator.
+        # Note that if the EXCLUDE is based on an expression, we will still be
+        # checking that expression because it will be under a different child segment.
+        if context.parent_stack and context.parent_stack[-1].is_type(
+            "exclusion_constraint_element"
+        ):
+            return None
+
         # We only care about equality operators.
         if context.segment.raw not in ("=", "!=", "<>"):
             return None
 
         # We only care if it's followed by a NULL literal.
         siblings = Segments(*context.parent_stack[-1].segments)
         after_op_list = siblings.select(start_seg=context.segment)
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV06.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,14 +318,16 @@
                 semi_colon_exist_flag = True
             elif segment.is_code:
                 is_one_line = self._is_one_line_statement(parent_segment, segment)
                 break
             elif not segment.is_meta:
                 before_segment.append(segment)
             trigger_segment = segment
+        else:
+            return None  # File does not contain any statements
         self.logger.debug("Trigger on: %s", trigger_segment)
         self.logger.debug("Anchoring on: %s", anchor_segment)
 
         semicolon_newline = self.multiline_newline if not is_one_line else False
 
         if not semi_colon_exist_flag:
             # Create the final semi-colon if it does not yet exist.
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     """Jinja tags should have a single whitespace on either side.
 
     **Anti-pattern**
 
     Jinja tags with either no whitespace or very long whitespace
     are hard to read.
 
-    .. code-block:: sql
+    .. code-block:: jinja
        :force:
 
         SELECT {{    a     }} from {{ref('foo')}}
 
     **Best practice**
 
     A single whitespace surrounding Jinja tags, alternatively
     longer gaps containing newlines are acceptable.
 
-    .. code-block:: sql
+    .. code-block:: jinja
        :force:
 
         SELECT {{ a }} from {{ ref('foo') }};
         SELECT {{ a }} from {{
             ref('foo')
         }};
     """
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.0.4/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,24 @@
     idx: int
     len: int
     type: str
 
     @staticmethod
     def _stack_pos_interpreter(path_step: PathStep) -> str:
         """Interpret a path step for stack_positions."""
-        if path_step.idx == 0 and path_step.idx == path_step.len - 1:
+        # If no code, then no.
+        if not path_step.code_idxs:
+            return ""
+        # If there's only one code element, this must be it.
+        elif len(path_step.code_idxs) == 1:
             return "solo"
-        elif path_step.idx == 0:
+        # Check for whether first or last code element
+        elif path_step.idx == min(path_step.code_idxs):
             return "start"
-        elif path_step.idx == path_step.len - 1:
+        elif path_step.idx == max(path_step.code_idxs):
             return "end"
         else:
             return ""  # NOTE: Empty string evaluates as falsy.
 
     @classmethod
     def from_path_step(
         cls: Type["StackPosition"], path_step: PathStep
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Dataclasses for reflow work."""
 
 from itertools import chain
 import logging
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
 
+from sqlfluff.core.parser import PositionMarker
 from sqlfluff.core.parser.segments import (
     BaseSegment,
     RawSegment,
     NewlineSegment,
     WhitespaceSegment,
     TemplateSegment,
     Indent,
@@ -73,14 +74,22 @@
         return self._class_types(self.segments)
 
     @property
     def raw(self) -> str:
         """Get the current raw representation."""
         return "".join(seg.raw for seg in self.segments)
 
+    @property
+    def pos_marker(self) -> Optional[PositionMarker]:
+        """Get the first position marker of the element."""
+        for seg in self.segments:
+            if seg.pos_marker:
+                return seg.pos_marker
+        return None
+
     def num_newlines(self) -> int:
         """Return the number of newlines in this element.
 
         These newlines are either newline segments or contained
         within consumed sections of whitespace. This counts
         both.
         """
@@ -624,15 +633,15 @@
         however it exists as a convenience for rules which wish to use it.
         """
         existing_results = lint_results[:]
         pre_constraint, post_constraint, strip_newlines = determine_constraints(
             prev_block, next_block, strip_newlines
         )
 
-        reflow_logger.debug("Respacing: %s", self)
+        reflow_logger.debug("* Respacing: %r @ %s", self.raw, self.pos_marker)
 
         # The buffer is used to create the new reflow point to return
         segment_buffer, last_whitespace, new_results = process_spacing(
             list(self.segments), strip_newlines
         )
 
         # Check for final trailing whitespace (which otherwise looks like an indent).
@@ -658,15 +667,21 @@
             # If we find that the last whitespace has a newline
             # before it, and the position markers imply there was
             # a removal between them, then remove the whitespace.
             # This ensures a consistent indent.
             if last_whitespace:
                 ws_idx = self.segments.index(last_whitespace)
                 if ws_idx > 0:
-                    prev_seg = self.segments[ws_idx - 1]
+                    # NOTE: Iterate by index so that we don't slice the full range.
+                    for prev_seg_idx in range(ws_idx - 1, -1, -1):
+                        prev_seg = self.segments[prev_seg_idx]
+                        # Skip past any indents
+                        if not prev_seg.is_type("indent"):
+                            break
+
                     if (
                         prev_seg.is_type("newline")
                         # Not just unequal. Must be actively _before_.
                         # NOTE: Based on working locations
                         and prev_seg.get_end_loc() < last_whitespace.get_start_loc()
                     ):
                         reflow_logger.debug(
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 if not isinstance(end_elem, ReflowBlock):
                     continue
                 elif key not in end_elem.depth_info.stack_positions:
                     # If we get here, it means the last block was the end.
                     # NOTE: This feels a little hacky, but it's because of a limitation
                     # in detecting the "end" and "solo" markers effectively in larger
                     # sections.
-                    final_idx = end_idx - 2
+                    final_idx = end_idx - 2  # pragma: no cover
                 elif end_elem.depth_info.stack_positions[key].type in ("end", "solo"):
                     final_idx = end_idx
 
                 if final_idx is not None:
                     # Found the end. Add it to the stack.
                     # We reference the appropriate element from the parent stack.
                     target_depth = elem.depth_info.stack_hashes.index(key)
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/reindent.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,18 @@
             _case_type = None
             if first_segment.is_type("placeholder"):
                 _case_type = cast(TemplateSegment, first_segment).block_type
 
             if _case_type in ("block_start", "block_mid"):
                 # Is following _line_ AND element also a block?
                 # i.e. nothing else between.
-                if first_point_idx + 3 == lines[idx + 1].indent_points[0].idx + 1:
+                if (
+                    idx + 1 < len(lines)
+                    and first_point_idx + 3 == lines[idx + 1].indent_points[0].idx + 1
+                ):
                     seg = elements[first_point_idx + 3].segments[0]
                     if seg.is_type("placeholder"):
                         if cast(TemplateSegment, seg).block_type == "block_start":
                             _inter_steps = list(
                                 range(
                                     line.initial_indent_balance,
                                     lines[idx + 1].initial_indent_balance,
@@ -1855,15 +1858,18 @@
     # Only keep indices which are after the critical point.
     target_breaks = [e_idx for e_idx in target_breaks if e_idx >= purge_before]
     reflow_logger.debug("    Remaining breaks: %s.", target_breaks)
 
     for e_idx in target_breaks:
         e = cast(ReflowPoint, elements[e_idx])
         indent_stats = _indent_stats_cache[e_idx]
-        if indent_stats.trough < 0:
+        # NOTE: We check against the _impulse_ here rather than the
+        # _trough_ because if we're about to step back up again then
+        # it should still be indented.
+        if indent_stats.impulse < 0:
             new_indent = outer_indent
             # NOTE: If we're about to insert a dedent before a
             # comma or semicolon ... don't. They are a bit special
             # in being allowed to trail.
             if elements[e_idx + 1].class_types.intersection(
                 ("statement_terminator", "comma")
             ):
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/respace.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,22 +109,16 @@
     """Given the existing spacing, extract information and do basic pruning."""
     removal_buffer: List[RawSegment] = []
     result_buffer: List[LintResult] = []
     last_whitespace: List[RawSegment] = []
 
     # Loop through the existing segments looking for spacing.
     for seg in segment_buffer:
-        # If it has a position marker, but it's not literal, then
-        # it's a templated element and so we shouldn't consider it
-        # here.
-        if seg.pos_marker and not seg.pos_marker.is_literal():
-            continue
-
         # If it's whitespace, store it.
-        elif seg.is_type("whitespace"):
+        if seg.is_type("whitespace"):
             last_whitespace.append(seg)
 
         # If it's a newline, react accordingly.
         # NOTE: This should only trigger on literal newlines.
         elif seg.is_type("newline", "end_of_file"):
             # Are we stripping newlines?
             if strip_newlines and seg.is_type("newline"):
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,17 +511,14 @@
                 # Reset the values
                 reflow_logger.debug(
                     "    Filter %r applied. Resetting %s", filter, point
                 )
                 new_point = point
             # Otherwise apply the new fixes
             else:
-                reflow_logger.debug(
-                    "    Filter %r allows fixes for point: %s", filter, new_lint_results
-                )
                 lint_results = new_lint_results
 
             if pre and (not new_elements or new_elements[-1] != pre):
                 new_elements.append(pre)
             new_elements.append(new_point)
             if post:
                 new_elements.append(post)
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.0.4/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.0.4/src/sqlfluff.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.3
+Version: 2.0.4
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.0.4/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 src/sqlfluff/dialects/dialect_sparksql_keywords.py
 src/sqlfluff/dialects/dialect_sqlite.py
 src/sqlfluff/dialects/dialect_sqlite_keywords.py
 src/sqlfluff/dialects/dialect_teradata.py
 src/sqlfluff/dialects/dialect_tsql.py
 src/sqlfluff/dialects/dialect_tsql_keywords.py
 src/sqlfluff/rules/__init__.py
-src/sqlfluff/rules/sphinx.py
 src/sqlfluff/rules/aliasing/AL01.py
 src/sqlfluff/rules/aliasing/AL02.py
 src/sqlfluff/rules/aliasing/AL03.py
 src/sqlfluff/rules/aliasing/AL04.py
 src/sqlfluff/rules/aliasing/AL05.py
 src/sqlfluff/rules/aliasing/AL06.py
 src/sqlfluff/rules/aliasing/AL07.py
```

### Comparing `sqlfluff-2.0.3/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.0.4/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.3/test/test_testing.py` & `sqlfluff-2.0.4/test/test_testing.py`

 * *Files identical despite different names*

