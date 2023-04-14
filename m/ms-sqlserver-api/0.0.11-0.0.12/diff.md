# Comparing `tmp/ms_sqlserver_api-0.0.11.tar.gz` & `tmp/ms_sqlserver_api-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_sqlserver_api-0.0.11.tar", max compression
+gzip compressed data, was "ms_sqlserver_api-0.0.12.tar", max compression
```

## Comparing `ms_sqlserver_api-0.0.11.tar` & `ms_sqlserver_api-0.0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/LICENSE
--rw-r--r--   0        0        0      614 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/README.md
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/__tests__/__init__.py
--rw-r--r--   0        0        0     2363 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/__tests__/test_marathon.py
--rw-r--r--   0        0        0      620 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/api.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/parsers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/parsers/parse_table1.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/queries/__init__.py
--rw-r--r--   0        0        0       64 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/queries/bigquery.py
--rw-r--r--   0        0        0       43 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/queries/sql_server.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/sql_server/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/sql_server/__tests__/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/sql_server/__tests__/test_sql_server.py
--rw-r--r--   0        0        0     1251 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/ms_marathon_api/sql_server/connection.py
--rw-r--r--   0        0        0      764 2023-04-12 09:33:17.828519 ms_sqlserver_api-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 ms_sqlserver_api-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/LICENSE
+-rw-r--r--   0        0        0      614 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/__tests__/__init__.py
+-rw-r--r--   0        0        0     2363 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/__tests__/test_marathon.py
+-rw-r--r--   0        0        0      623 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/parsers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/parsers/parse_table1.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/queries/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/queries/bigquery.py
+-rw-r--r--   0        0        0       43 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/queries/sql_server.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/sql_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/sql_server/__tests__/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/sql_server/__tests__/test_sql_server.py
+-rw-r--r--   0        0        0     1393 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/ms_marathon_api/sql_server/connection.py
+-rw-r--r--   0        0        0      945 2023-04-14 09:24:33.954208 ms_sqlserver_api-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 ms_sqlserver_api-0.0.12/PKG-INFO
```

### Comparing `ms_sqlserver_api-0.0.11/LICENSE` & `ms_sqlserver_api-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_sqlserver_api-0.0.11/README.md` & `ms_sqlserver_api-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/__tests__/test_marathon.py` & `ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/__tests__/test_marathon.py`

 * *Files identical despite different names*

### Comparing `ms_sqlserver_api-0.0.11/ms_marathon_api/marathon/api.py` & `ms_sqlserver_api-0.0.12/ms_marathon_api/marathon/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from gc_google_services_api.bigquery import execute_query
 
-from ms_marathon_api.marathon.parsers.parse_table1 import \
-    build_table1_export_query
+from ms_marathon_api.marathon.parsers.parse_table1 import (
+    build_table1_export_query,
+)
 from ms_marathon_api.marathon.queries.bigquery import INSERT_TABLE1
 from ms_marathon_api.marathon.queries.sql_server import SELECT_ALL_TABLE1
 from ms_marathon_api.sql_server.connection import SQLServer
 
 
 class SQLMarathon(SQLServer):
     def migrate_table1(self):
```

### Comparing `ms_sqlserver_api-0.0.11/ms_marathon_api/sql_server/__tests__/test_sql_server.py` & `ms_sqlserver_api-0.0.12/ms_marathon_api/sql_server/__tests__/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `ms_sqlserver_api-0.0.11/pyproject.toml` & `ms_sqlserver_api-0.0.12/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-sqlserver-api"
-version = "0.0.11"
+version = "0.0.12"
 description = "API to connect with Marathon system and migrate data to Bigquery"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_marathon_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
@@ -20,13 +20,21 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 extend-exclude="# noqa"
 
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 79
+
 [[tool.poetry.source]]
 name = "syscorp-librarian"
 url = "https://europe-west1-python.pkg.dev/ms--tiber-com-lib--pro--8bd7/syscorp-librarian/"
 default = false
 secondary = true
-
```

### Comparing `ms_sqlserver_api-0.0.11/PKG-INFO` & `ms_sqlserver_api-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-sqlserver-api
-Version: 0.0.11
+Version: 0.0.12
 Summary: API to connect with Marathon system and migrate data to Bigquery
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

