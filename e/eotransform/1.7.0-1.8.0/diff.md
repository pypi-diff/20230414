# Comparing `tmp/eotransform-1.7.0.tar.gz` & `tmp/eotransform-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotransform-1.7.0.tar", last modified: Tue Mar  7 11:46:00 2023, max compression
+gzip compressed data, was "eotransform-1.8.0.tar", last modified: Fri Apr 14 12:28:55 2023, max compression
```

## Comparing `eotransform-1.7.0.tar` & `eotransform-1.8.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.069865 eotransform-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-07 11:45:44.000000 eotransform-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-07 11:46:00.069865 eotransform-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-07 11:45:44.000000 eotransform-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-07 11:45:44.000000 eotransform-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-07 11:46:00.069865 eotransform-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-07 11:45:44.000000 eotransform-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.053865 eotransform-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.057865 eotransform-1.7.0/src/eotransform/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-07 11:45:46.000000 eotransform-1.7.0/src/eotransform/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/collection_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.057865 eotransform-1.7.0/src/eotransform/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/protocol/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/protocol/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.061865 eotransform-1.7.0/src/eotransform/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/sinks/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/sinks/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/sinks/sink_to_progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/sinks/with_performance_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/streamed_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.061865 eotransform-1.7.0/src/eotransform/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/apply_to_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/to_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/transformers/with_performance_clock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.065865 eotransform-1.7.0/src/eotransform/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-07 11:45:44.000000 eotransform-1.7.0/src/eotransform/utilities/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.057865 eotransform-1.7.0/src/eotransform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-07 11:46:00.000000 eotransform-1.7.0/src/eotransform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-07 11:46:00.000000 eotransform-1.7.0/src/eotransform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 11:46:00.000000 eotransform-1.7.0/src/eotransform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-07 11:46:00.000000 eotransform-1.7.0/src/eotransform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-07 11:46:00.000000 eotransform-1.7.0/src/eotransform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:46:00.069865 eotransform-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_collection_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_sink_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_sink_report_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_sink_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_sink_with_performance_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_streamed_process_from_source_to_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_applied_to_element_at_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_by_applying_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_compound_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_result_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_to_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_transform_with_performance_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-07 11:45:44.000000 eotransform-1.7.0/tests/test_utilities_profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.271803 eotransform-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-14 12:28:38.000000 eotransform-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 12:28:55.271803 eotransform-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-14 12:28:38.000000 eotransform-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 12:28:38.000000 eotransform-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 12:28:55.275803 eotransform-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 12:28:38.000000 eotransform-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.259803 eotransform-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.263803 eotransform-1.8.0/src/eotransform/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 12:28:39.000000 eotransform-1.8.0/src/eotransform/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/collection_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.263803 eotransform-1.8.0/src/eotransform/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/protocol/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/protocol/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/protocol/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.263803 eotransform-1.8.0/src/eotransform/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/sinks/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/sinks/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/sinks/sink_to_progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/sinks/with_performance_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/streamed_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.267803 eotransform-1.8.0/src/eotransform/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/apply_to_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/send_to_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/to_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/transformers/with_performance_clock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.267803 eotransform-1.8.0/src/eotransform/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-14 12:28:38.000000 eotransform-1.8.0/src/eotransform/utilities/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.263803 eotransform-1.8.0/src/eotransform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 12:28:55.000000 eotransform-1.8.0/src/eotransform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-14 12:28:55.000000 eotransform-1.8.0/src/eotransform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:28:55.000000 eotransform-1.8.0/src/eotransform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 12:28:55.000000 eotransform-1.8.0/src/eotransform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 12:28:55.000000 eotransform-1.8.0/src/eotransform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:28:55.271803 eotransform-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_collection_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_sink_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_sink_report_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_sink_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_sink_with_performance_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_streamed_process_from_source_to_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_applied_to_element_at_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_by_applying_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_compound_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_result_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_send_to_stream_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_to_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_transform_with_performance_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-14 12:28:38.000000 eotransform-1.8.0/tests/test_utilities_profiling.py
```

### Comparing `eotransform-1.7.0/LICENSE` & `eotransform-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/PKG-INFO` & `eotransform-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotransform
-Version: 1.7.0
+Version: 1.8.0
 Summary: Protocol definition for streamed source/transform/sink process
 Home-page: https://github.com/TUW-GEO/eotransform
 Author: TU Wien GEO MRS group
 Author-email: remote.sensing@geo.tuwien.ac.at
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `eotransform-1.7.0/setup.cfg` & `eotransform-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/apply.py` & `eotransform-1.8.0/src/eotransform/apply.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/collection_transformation.py` & `eotransform-1.8.0/src/eotransform/collection_transformation.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/protocol/transformer.py` & `eotransform-1.8.0/src/eotransform/protocol/transformer.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/result.py` & `eotransform-1.8.0/src/eotransform/result.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/sinks/filtered.py` & `eotransform-1.8.0/src/eotransform/sinks/filtered.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/sinks/result.py` & `eotransform-1.8.0/src/eotransform/sinks/result.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/sinks/sink_to_progress_report.py` & `eotransform-1.8.0/src/eotransform/sinks/sink_to_progress_report.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/streamed_process.py` & `eotransform-1.8.0/src/eotransform/streamed_process.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/transformers/apply_to_enumeration.py` & `eotransform-1.8.0/src/eotransform/transformers/apply_to_enumeration.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/transformers/compose.py` & `eotransform-1.8.0/src/eotransform/transformers/compose.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/transformers/map.py` & `eotransform-1.8.0/src/eotransform/transformers/map.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/transformers/repeat.py` & `eotransform-1.8.0/src/eotransform/transformers/repeat.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/transformers/result.py` & `eotransform-1.8.0/src/eotransform/transformers/result.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform/utilities/profiling.py` & `eotransform-1.8.0/src/eotransform/utilities/profiling.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/src/eotransform.egg-info/PKG-INFO` & `eotransform-1.8.0/src/eotransform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotransform
-Version: 1.7.0
+Version: 1.8.0
 Summary: Protocol definition for streamed source/transform/sink process
 Home-page: https://github.com/TUW-GEO/eotransform
 Author: TU Wien GEO MRS group
 Author-email: remote.sensing@geo.tuwien.ac.at
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `eotransform-1.7.0/src/eotransform.egg-info/SOURCES.txt` & `eotransform-1.8.0/src/eotransform.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 src/eotransform.egg-info/PKG-INFO
 src/eotransform.egg-info/SOURCES.txt
 src/eotransform.egg-info/dependency_links.txt
 src/eotransform.egg-info/requires.txt
 src/eotransform.egg-info/top_level.txt
 src/eotransform/protocol/__init__.py
 src/eotransform/protocol/sink.py
+src/eotransform/protocol/stream.py
 src/eotransform/protocol/transformer.py
 src/eotransform/sinks/__init__.py
 src/eotransform/sinks/filtered.py
 src/eotransform/sinks/result.py
 src/eotransform/sinks/sink_to_progress_report.py
 src/eotransform/sinks/with_performance_clock.py
 src/eotransform/transformers/__init__.py
 src/eotransform/transformers/apply_to_enumeration.py
 src/eotransform/transformers/chain.py
 src/eotransform/transformers/compose.py
 src/eotransform/transformers/identity.py
 src/eotransform/transformers/map.py
 src/eotransform/transformers/repeat.py
 src/eotransform/transformers/result.py
+src/eotransform/transformers/send_to_stream.py
 src/eotransform/transformers/to_tuple.py
 src/eotransform/transformers/with_performance_clock.py
 src/eotransform/utilities/__init__.py
 src/eotransform/utilities/profiling.py
 tests/test_collection_transformation.py
 tests/test_sink_filtered.py
 tests/test_sink_report_progress.py
@@ -44,10 +46,11 @@
 tests/test_transform_by_applying_function.py
 tests/test_transform_chain.py
 tests/test_transform_compound_transform.py
 tests/test_transform_identity.py
 tests/test_transform_map.py
 tests/test_transform_repeat.py
 tests/test_transform_result_result.py
+tests/test_transform_send_to_stream_input.py
 tests/test_transform_to_tuple.py
 tests/test_transform_with_performance_clock.py
 tests/test_utilities_profiling.py
```

### Comparing `eotransform-1.7.0/tests/test_collection_transformation.py` & `eotransform-1.8.0/tests/test_collection_transformation.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_sink_report_progress.py` & `eotransform-1.8.0/tests/test_sink_report_progress.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_sink_result.py` & `eotransform-1.8.0/tests/test_sink_result.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_sink_with_performance_clock.py` & `eotransform-1.8.0/tests/test_sink_with_performance_clock.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_streamed_process_from_source_to_sink.py` & `eotransform-1.8.0/tests/test_streamed_process_from_source_to_sink.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_transform_result_result.py` & `eotransform-1.8.0/tests/test_transform_result_result.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_transform_with_performance_clock.py` & `eotransform-1.8.0/tests/test_transform_with_performance_clock.py`

 * *Files identical despite different names*

### Comparing `eotransform-1.7.0/tests/test_utilities_profiling.py` & `eotransform-1.8.0/tests/test_utilities_profiling.py`

 * *Files identical despite different names*

