# Comparing `tmp/apache-airflow-providers-fastetl-0.0.5.tar.gz` & `tmp/apache-airflow-providers-fastetl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-fastetl-0.0.5.tar", last modified: Fri Apr 14 14:27:05 2023, max compression
+gzip compressed data, was "apache-airflow-providers-fastetl-0.0.6.tar", last modified: Fri Apr 14 14:55:02 2023, max compression
```

## Comparing `apache-airflow-providers-fastetl-0.0.5.tar` & `apache-airflow-providers-fastetl-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.060016 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:27:05.000000 apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.060016 apache-airflow-providers-fastetl-0.0.5/fastetl/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.060016 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/copy_db_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/fast_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/patchwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/samba_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.060016 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/encode_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/get_table_cols_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/load_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/load_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/string_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/table_comments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/bacen_STA_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/ckan_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/db_to_db_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/dou_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/gsheet_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/osrm_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/datapackage_to_datadictionary_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/db_to_csv_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/gsheet_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/fastetl/operators/osrm_distance_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:27:05.064016 apache-airflow-providers-fastetl-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/tests/test_db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/tests/test_odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 14:26:49.000000 apache-airflow-providers-fastetl-0.0.5/tests/test_osrm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.146343 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:55:02.000000 apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.146343 apache-airflow-providers-fastetl-0.0.6/fastetl/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.146343 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/copy_db_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/fast_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/patchwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/samba_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/encode_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/get_table_cols_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/load_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/load_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/string_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/table_comments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/bacen_STA_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/ckan_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/db_to_db_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/dou_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/gsheet_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/osrm_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/datapackage_to_datadictionary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/db_to_csv_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/gsheet_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/fastetl/operators/osrm_distance_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:55:02.150344 apache-airflow-providers-fastetl-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/tests/test_db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/tests/test_odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 14:54:39.000000 apache-airflow-providers-fastetl-0.0.6/tests/test_osrm.py
```

### Comparing `apache-airflow-providers-fastetl-0.0.5/LICENSE` & `apache-airflow-providers-fastetl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.5
+Version: 0.0.6
 Summary: FastETL custom package Apache Airflow provider.
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
```

### Comparing `apache-airflow-providers-fastetl-0.0.5/README.md` & `apache-airflow-providers-fastetl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.5
+Version: 0.0.6
 Summary: FastETL custom package Apache Airflow provider.
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.8
```

### Comparing `apache-airflow-providers-fastetl-0.0.5/apache_airflow_providers_fastetl.egg-info/SOURCES.txt` & `apache-airflow-providers-fastetl-0.0.6/apache_airflow_providers_fastetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/copy_db_extensions.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/copy_db_extensions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/fast_etl.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/fast_etl.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/patchwork.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/patchwork.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/samba_services.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/samba_services.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/date.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/db_connection.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/db_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/encode_html.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/encode_html.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/get_table_cols_name.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/get_table_cols_name.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/load_env_var.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/load_env_var.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/load_info.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/load_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/odf_tables.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/string_formatting.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/string_formatting.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/custom_functions/utils/table_comments.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/custom_functions/utils/table_comments.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/bacen_STA_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/bacen_STA_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/ckan_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/ckan_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/db_to_db_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/db_to_db_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/dou_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/dou_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/gsheet_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/gsheet_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/hooks/osrm_hook.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/hooks/osrm_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/operators/datapackage_to_datadictionary_operator.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/operators/datapackage_to_datadictionary_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/operators/db_to_csv_operator.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/operators/db_to_csv_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/operators/db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/operators/db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/operators/gsheet_operator.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/operators/gsheet_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/fastetl/operators/osrm_distance_operator.py` & `apache-airflow-providers-fastetl-0.0.6/fastetl/operators/osrm_distance_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/setup.py` & `apache-airflow-providers-fastetl-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 """Perform the package apache-airflow-providers-fastetl setup."""
 setup(
     name="apache-airflow-providers-fastetl",
     version=__version__,
     description="FastETL custom package Apache Airflow provider.",
     long_description=long_description,
```

### Comparing `apache-airflow-providers-fastetl-0.0.5/tests/test_dag.py` & `apache-airflow-providers-fastetl-0.0.6/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/tests/test_db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.6/tests/test_db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/tests/test_odf_tables.py` & `apache-airflow-providers-fastetl-0.0.6/tests/test_odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.5/tests/test_osrm.py` & `apache-airflow-providers-fastetl-0.0.6/tests/test_osrm.py`

 * *Files identical despite different names*

