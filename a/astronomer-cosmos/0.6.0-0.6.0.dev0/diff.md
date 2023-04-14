# Comparing `tmp/astronomer_cosmos-0.6.0.tar.gz` & `tmp/astronomer_cosmos-0.6.0.dev0.tar.gz`

## Comparing `astronomer_cosmos-0.6.0.tar` & `astronomer_cosmos-0.6.0.dev0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/LICENSE
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/README.rst
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/README.rst
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.0/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/.gitignore` & `astronomer_cosmos-0.6.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/LICENSE` & `astronomer_cosmos-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/README.rst` & `astronomer_cosmos-0.6.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/pyproject.toml` & `astronomer_cosmos-0.6.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0/PKG-INFO` & `astronomer_cosmos-0.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.0
+Version: 0.6.0.dev0
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

