# Comparing `tmp/apache-airflow-providers-fastetl-0.0.3.tar.gz` & `tmp/apache-airflow-providers-fastetl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-fastetl-0.0.3.tar", last modified: Thu Apr 13 22:44:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-fastetl-0.0.4.tar", last modified: Fri Apr 14 03:07:47 2023, max compression
```

## Comparing `apache-airflow-providers-fastetl-0.0.3.tar` & `apache-airflow-providers-fastetl-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.796745 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 22:44:06.000000 apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.796745 apache-airflow-providers-fastetl-0.0.3/fastetl/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.796745 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/copy_db_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/fast_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/patchwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/samba_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/encode_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/get_table_cols_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/load_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/load_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/string_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/table_comments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/bacen_STA_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/ckan_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/db_to_db_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/dou_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/gsheet_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/osrm_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/datapackage_to_datadictionary_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/db_to_csv_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/gsheet_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/fastetl/operators/osrm_distance_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:44:06.800745 apache-airflow-providers-fastetl-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/tests/test_db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/tests/test_odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-13 22:43:51.000000 apache-airflow-providers-fastetl-0.0.3/tests/test_osrm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.572355 apache-airflow-providers-fastetl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 03:07:47.568355 apache-airflow-providers-fastetl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.560355 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 03:07:47.000000 apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.560355 apache-airflow-providers-fastetl-0.0.4/fastetl/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.564355 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/copy_db_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/fast_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/patchwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/samba_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.564355 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/encode_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/get_table_cols_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/load_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/load_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/string_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/table_comments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.568355 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/bacen_STA_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/ckan_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/db_to_db_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/dou_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/gsheet_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/osrm_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.568355 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/datapackage_to_datadictionary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/db_to_csv_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/gsheet_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/fastetl/operators/osrm_distance_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:07:47.572355 apache-airflow-providers-fastetl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:07:47.568355 apache-airflow-providers-fastetl-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/tests/test_db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/tests/test_odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 03:07:27.000000 apache-airflow-providers-fastetl-0.0.4/tests/test_osrm.py
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/LICENSE` & `apache-airflow-providers-fastetl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.3
+Version: 0.0.4
 Summary: FastETL custom package Apache Airflow provider.
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/README.md` & `apache-airflow-providers-fastetl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.3
+Version: 0.0.4
 Summary: FastETL custom package Apache Airflow provider.
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/apache_airflow_providers_fastetl.egg-info/SOURCES.txt` & `apache-airflow-providers-fastetl-0.0.4/apache_airflow_providers_fastetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/copy_db_extensions.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/copy_db_extensions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/fast_etl.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/fast_etl.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/patchwork.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/patchwork.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/samba_services.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/samba_services.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/date.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/db_connection.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/db_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/encode_html.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/encode_html.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/get_table_cols_name.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/get_table_cols_name.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/load_env_var.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/load_env_var.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/load_info.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/load_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/odf_tables.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/odf_tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module for handling tables in Open Document Format (ODF) text documents
 and generating textual data dictionaries.
 """
 from typing import List
 import logging
 
-from frictionless import Package
+from frictionless import Package, Resource
 
 import odf
 import odf.table, odf.text
 from odf.opendocument import OpenDocumentText
 
 DATA_DICT_COLUMN_NAMES = {
     "en": ["field name", "type", "description"],
@@ -354,88 +354,135 @@
         document.
 
         Args:
             name (str): a name for the table
         """
         self.tables[name] = DocDataTable(document=self, name=name, **kw_args)
 
+    def append_heading(self, text: str, level: int = 1):
+        """Appends a heading section containing the text provided,
+
+        Args:
+            text (str): contents of the heading,
+            level (int): level of the heading. Defaults to 1.
+        """
+        heading = odf.text.H(stylename="Heading", text=text, outlinelevel=level)
+        self.odf_document.text.addElement(heading)
+
+    def append_paragraph(self, text: str):
+        """Appends a paragraph of text containing the text provided,
+
+        TODO: Add support for converting markdown text.
+
+        Args:
+            text (str): contents of the paragraph
+        """
+        for line in text.split("\n\n"):
+            paragraph = odf.text.P(stylename="Standard", text=line)
+            self.odf_document.text.addElement(paragraph)
+
 
 def create_data_dictionary(
-    data_package: str,
+    data_package: Package,
     output: str,
     lang: str = "en",
 ):
     """Creates a data dictionary text document from a Frictionless Data
     package and table schema.
 
     Args:
-        data_package (str): path to the Frictionless data package
-            descriptor.
+        data_package (Package): a Frictionless data package.
         output (str): path to the resulting odf file.
         lang (str): language code to use for the table column headers.
             Defaults to "en".
     """
-    package = Package(data_package)
-
     document = DocumentWithTables()
-    for resource in package.resources:
+
+    if data_package.title:
+        document.append_heading(data_package.title)
+    if data_package.description:
+        document.append_paragraph(data_package.description)
+
+    for resource in data_package.resources:
         document.append_table(
             resource.name,
             column_names=DATA_DICT_COLUMN_NAMES[lang],
             title=resource.title,
             description=resource.description,
         )
         rows = []
         for field in resource.schema.fields:
             rows.append([field.name, field.type, field.description])
         document.tables[resource.name].add_rows(rows)
 
     document.save(output)
 
 
+def fill_template_table(
+    resource: Resource,
+    document: OpenDocumentText,
+) -> OpenDocumentText:
+    """Fills a table in a template document with data from the given
+    resource schema.
+
+    Args:
+        resource (Resource): a Frictionless Data Resource.
+        document (DocumentWithTables): a DocumentWithTables object.
+
+    Returns:
+        DocumentWithTables: the document with the table filled out.
+    """
+    if resource.name not in document.tables.keys():
+        raise ValueError(f"Table with id '{resource.name}' not found in document.")
+    table = document.tables[resource.name]
+    rows = []
+    for field in resource.schema.fields:
+        rows.append([field.name, field.type, field.description])
+    table.add_rows(rows)
+    return document
+
+
 def create_data_dictionary_from_template(
-    data_package: str,
+    data_package: Package,
     doc_template: str,
-    resource_name: str,
+    resource_names: List[str] = None,
     # after_heading: str = None, # TODO
     output: str = None,
 ):
     """Creates a data dictionary text document from a Frictionless Data
     package and table schema, using a provided document template..
 
     Args:
         data_package (str): path to the Frictionless data package
             descriptor.
         doc_template (str): path to the odf file to be used as a
             template. If omitted, will create a new document from
             scratch.
-        resource_name (str): resource name in the data package
-            to use to describe the table.
+        resource_name (List[str]): list of resource names in the data
+            package which will update the table.
 
-            This must also match the exact id of the table in the
-            OpenDocumentText text file to be altered. The table must
-            contain only a header and one row.
+            Default to None.
+
+            If None, will update all tables whose name match the
+            resource names in the data package.
         after_heading (str, optional): Text of the heading under which
             the new table will be created.
             If None, will use the resource title from the data package
             to search the document for headings with a corresponding
             title.
 
             If None, won't add the resource's title and description.
             Defaults to None.
         output (str): path to the resulting odf file. Defaults to None.
             Caution: if None, will overwrite the original template
             document!
     """
-    package = Package(data_package)
-
     document = DocumentWithTables.load_from_template(doc_template, load_all_tables=True)
-    if resource_name not in document.tables.keys():
-        raise ValueError(f"Table with id '{resource_name}' not found in document.")
-    table = document.tables[resource_name]
-    resource = package.get_resource(resource_name)
-    rows = []
-    for field in resource.schema.fields:
-        rows.append([field.name, field.type, field.description])
-    table.add_rows(rows)
+
+    if resource_names is None:
+        resource_names = data_package.resource_names
+    for resource_name in resource_names:
+        if resource_name in document.tables.keys():
+            resource = data_package.get_resource(resource_name)
+            document = fill_template_table(resource, document)
 
     document.save(output)
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/string_formatting.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/string_formatting.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/custom_functions/utils/table_comments.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/custom_functions/utils/table_comments.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/bacen_STA_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/bacen_STA_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/ckan_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/ckan_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/db_to_db_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/db_to_db_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/dou_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/dou_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/gsheet_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/gsheet_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/hooks/osrm_hook.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/hooks/osrm_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/operators/db_to_csv_operator.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/operators/db_to_csv_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/operators/db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/operators/db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/operators/gsheet_operator.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/operators/gsheet_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/fastetl/operators/osrm_distance_operator.py` & `apache-airflow-providers-fastetl-0.0.4/fastetl/operators/osrm_distance_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/setup.py` & `apache-airflow-providers-fastetl-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 """Perform the package apache-airflow-providers-fastetl setup."""
 setup(
     name="apache-airflow-providers-fastetl",
     version=__version__,
     description="FastETL custom package Apache Airflow provider.",
     long_description=long_description,
@@ -24,15 +24,15 @@
         "apache-airflow-providers-microsoft-mssql",
         "apache-airflow-providers-mysql",
         "apache-airflow-providers-postgres",
         "apache-airflow-providers-common-sql",
         "alembic>=1.8.1",
         "beautifulsoup4>=4.1.11",
         "ckanapi>=4.6",
-        "frictionless>5.8.3",
+        "frictionless>=5.11.1",
         "markdown>=3.4.1",
         "odfpy>=1.4.1",
         "pandas>=1.5.2,<2",
         "psycopg2>=2.9.5",
         "pygsheets>=2.0.5",
         "pyodbc>=4.0.35",
         "pysmb>=1.2.6",
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/tests/test_dag.py` & `apache-airflow-providers-fastetl-0.0.4/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/tests/test_db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.4/tests/test_db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.3/tests/test_odf_tables.py` & `apache-airflow-providers-fastetl-0.0.4/tests/test_odf_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 @pytest.mark.parametrize(
     "data_package_descriptor",
     [(PACKAGE_DESCRIPTOR)],
 )
 def test_create_new_data_dictionary(data_package_descriptor: str):
     descriptor = yaml.safe_load(data_package_descriptor)
-    create_data_dictionary(descriptor, TEMP_DOCUMENT_NAME)
+    create_data_dictionary(Package(descriptor), TEMP_DOCUMENT_NAME)
 
     # verify contents of document file
     document = odf.opendocument.load(TEMP_DOCUMENT_NAME)
     assert odf.teletype.extractText(document.text) == "".join(
         (
             TABLE_TITLE,
             TABLE_DESCRIPTION,
```

### Comparing `apache-airflow-providers-fastetl-0.0.3/tests/test_osrm.py` & `apache-airflow-providers-fastetl-0.0.4/tests/test_osrm.py`

 * *Files identical despite different names*

