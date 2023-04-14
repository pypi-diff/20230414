# Comparing `tmp/database-factory-1.0.4.tar.gz` & `tmp/database-factory-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/database-factory-1.0.4.tar", last modified: Wed Jun 15 09:05:28 2022, max compression
+gzip compressed data, was "dist/database-factory-1.0.5.tar", last modified: Fri Apr 14 13:58:01 2023, max compression
```

## Comparing `database-factory-1.0.4.tar` & `database-factory-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.750703 database-factory-1.0.4/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2021-03-16 10:53:13.000000 database-factory-1.0.4/LICENSE
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      233 2021-03-16 12:44:42.000000 database-factory-1.0.4/MANIFEST.in
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7676 2022-06-15 09:05:28.750703 database-factory-1.0.4/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4978 2021-04-05 09:13:47.000000 database-factory-1.0.4/README.md
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.746703 database-factory-1.0.4/database_factory/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory/.version
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.746703 database-factory-1.0.4/database_factory/cloud/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.750703 database-factory-1.0.4/database_factory/cloud/aws/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/aws/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3204 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/aws/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3888 2021-08-10 05:53:56.000000 database-factory-1.0.4/database_factory/cloud/aws/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.750703 database-factory-1.0.4/database_factory/cloud/gcp/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/gcp/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5800 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/gcp/auth.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/gcp/resource_manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3876 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/cloud/gcp/secrete_manager.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.750703 database-factory-1.0.4/database_factory/common/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/common/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4217 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/common/common.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    16949 2022-06-15 06:33:26.000000 database-factory-1.0.4/database_factory/manager.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.4/database_factory/operations.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:05:28.746703 database-factory-1.0.4/database_factory.egg-info/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     7676 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      753 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      256 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       17 2022-06-15 09:05:28.000000 database-factory-1.0.4/database_factory.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2022-06-15 09:05:28.750703 database-factory-1.0.4/setup.cfg
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     6186 2022-06-15 08:46:59.000000 database-factory-1.0.4/setup.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/.circleci/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1066 2023-04-14 13:57:53.000000 database-factory-1.0.5/.circleci/config.yml
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)    53248 2023-04-14 13:57:53.000000 database-factory-1.0.5/.coverage
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      137 2021-03-16 10:53:13.000000 database-factory-1.0.5/.coveragerc
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       66 2023-04-14 13:57:53.000000 database-factory-1.0.5/.gitignore
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2021-03-16 10:53:13.000000 database-factory-1.0.5/LICENSE
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      233 2021-03-16 12:44:42.000000 database-factory-1.0.5/MANIFEST.in
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     7677 2023-04-14 13:58:01.730333 database-factory-1.0.5/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     4979 2023-04-14 13:57:53.000000 database-factory-1.0.5/README.md
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     8582 2023-04-14 13:57:53.000000 database-factory-1.0.5/coverage.xml
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory/.version
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/__init__.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/cloud/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/__init__.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory/cloud/aws/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/aws/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3204 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/aws/auth.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3888 2021-08-10 05:53:56.000000 database-factory-1.0.5/database_factory/cloud/aws/secrete_manager.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/database_factory/cloud/gcp/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5800 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/auth.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/resource_manager.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3876 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/cloud/gcp/secrete_manager.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/database_factory/common/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/common/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     4217 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/common/common.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)    17304 2023-04-14 13:57:53.000000 database-factory-1.0.5/database_factory/manager.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5435 2021-03-16 10:53:13.000000 database-factory-1.0.5/database_factory/operations.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.726333 database-factory-1.0.5/database_factory.egg-info/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     7677 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      878 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1132 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       17 2023-04-14 13:58:01.000000 database-factory-1.0.5/database_factory.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-04-14 13:58:01.730333 database-factory-1.0.5/setup.cfg
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     7121 2023-04-14 13:57:53.000000 database-factory-1.0.5/setup.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-04-14 13:58:01.730333 database-factory-1.0.5/test/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2022-06-15 09:04:02.000000 database-factory-1.0.5/test/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     2719 2022-06-15 09:04:02.000000 database-factory-1.0.5/test/database_factory_test.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       18 2023-04-14 13:57:53.000000 database-factory-1.0.5/version.py
```

### Comparing `database-factory-1.0.4/LICENSE` & `database-factory-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/PKG-INFO` & `database-factory-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.4
+Version: 1.0.5
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
 Description: # database-factory
@@ -171,15 +171,15 @@
         
         
         ### Development Setup
         
         #### Using virtualenv
         
         ```bash
-        python3 -m venv env
+        python3 -m venv venv
         source env/bin/activate
         pip install .
         ```
         
         ### Contributing
         
         1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
```

### Comparing `database-factory-1.0.4/README.md` & `database-factory-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
 
 ### Development Setup
 
 #### Using virtualenv
 
 ```bash
-python3 -m venv env
+python3 -m venv venv
 source env/bin/activate
 pip install .
 ```
 
 ### Contributing
 
 1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
```

### Comparing `database-factory-1.0.4/database_factory/cloud/aws/auth.py` & `database-factory-1.0.5/database_factory/cloud/aws/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/cloud/aws/secrete_manager.py` & `database-factory-1.0.5/database_factory/cloud/aws/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/cloud/gcp/auth.py` & `database-factory-1.0.5/database_factory/cloud/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/cloud/gcp/resource_manager.py` & `database-factory-1.0.5/database_factory/cloud/gcp/resource_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/cloud/gcp/secrete_manager.py` & `database-factory-1.0.5/database_factory/cloud/gcp/secrete_manager.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/common/common.py` & `database-factory-1.0.5/database_factory/common/common.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory/manager.py` & `database-factory-1.0.5/database_factory/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 File holds the module of Migration database manager and decide to connect with
 multiple databases using the configuration parameters.
 URI of database handled automatically for multiple databases using SQLAlchemy
 """
 
 import os
+import sys
 import logging
 import traceback
 from urllib.parse import quote_plus as urlquote
 from pandas import DataFrame
 from sqlalchemy import create_engine
 from sqlalchemy.orm import scoped_session
 from sqlalchemy.orm import sessionmaker
@@ -49,15 +50,15 @@
                                 as Pandas DataFrame.
         object
     """
 
     def __init__(self,
                  engine_type: str,
                  database: str,
-                 sqlite_db_path: str = os.environ["HOME"],
+                 sqlite_db_path: str = None,
                  username: str = None,
                  password: str = None,
                  schema: str = "public",
                  host: str = None,
                  port: str = None,
                  snowflake_role: str = None,
                  snowflake_warehouse: str = None,
@@ -132,14 +133,23 @@
                                     service.
                                     Default: is 'us-east-1'
             detail_logs:            (Optional) => Detailed logs for debugging.
                                     Default: Fasle.
         """
         self.engine_type = engine_type
         self.database = database
+
+        if not sqlite_db_path:
+            # Check current OS, it is Windows or Linux
+            is_windows = sys.platform.lower().startswith('win')
+            if is_windows:
+                sqlite_db_path = f"{os.environ['HOMEDRIVE']}{os.environ['HOMEPATH']}"
+            else:
+                sqlite_db_path = os.environ['HOME']
+
         self.sqlite_db_path = sqlite_db_path
         self.username = username
         self.password = password
         self.schema = schema
         self.host = host
         self.port = port
         self.snowflake_role = snowflake_role
@@ -237,15 +247,15 @@
         logger.info(
             f'SQLAlchemy Dialects will be created for database type: {self.engine_type}')
 
         if self.engine_type in ["sqlite"]:
             uri = 'sqlite:///' + os.path.join(self.sqlite_db_path,
                                               f"{self.database}.db")
         elif self.engine_type in ["postgres"]:
-            uri = f"postgres+pg8000://{self.username}:{self.password}@{self.host}:{self.port}/{self.database}"
+            uri = f"postgresql+pg8000://{self.username}:{self.password}@{self.host}:{self.port}/{self.database}"
             param = dict(client_encoding="utf8")
             is_not_dialect_desc = True
         elif self.engine_type in ["mysql", "mariadb"]:
             uri = f"mysql+pymysql://{self.username}:{self.password}@{self.host}:{self.port}/{self.database}?charset=utf8mb4"
         elif self.engine_type in ["snowflake"]:
             from snowflake.sqlalchemy import URL
             uri = URL(
@@ -278,15 +288,16 @@
         Use the class variables and update to hold the sessions.
         """
 
         try:
             logger.info(f'Creating SQLAlchemy Dialects session scope.')
             uri, param, is_not_dialect_desc = self.create_uri()
             if param:
-                self.engine = create_engine(uri, echo=self.detail_logs, **param)
+                self.engine = create_engine(
+                    uri, echo=self.detail_logs, **param)
             else:
                 self.engine = create_engine(uri, echo=self.detail_logs)
 
             if is_not_dialect_desc:
                 # https: // github.com/sqlalchemy/sqlalchemy/issues/5645
                 self.engine.dialect.description_encoding = None
```

### Comparing `database-factory-1.0.4/database_factory/operations.py` & `database-factory-1.0.5/database_factory/operations.py`

 * *Files identical despite different names*

### Comparing `database-factory-1.0.4/database_factory.egg-info/PKG-INFO` & `database-factory-1.0.5/database_factory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-factory
-Version: 1.0.4
+Version: 1.0.5
 Summary: Database Factory;
 Home-page: https://github.com/shrivastava-v-ankit/database-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/database-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/database-factory/issues
 Description: # database-factory
@@ -171,15 +171,15 @@
         
         
         ### Development Setup
         
         #### Using virtualenv
         
         ```bash
-        python3 -m venv env
+        python3 -m venv venv
         source env/bin/activate
         pip install .
         ```
         
         ### Contributing
         
         1. Fork repo- https://github.com/shrivastava-v-ankit/database-factory.git
```

### Comparing `database-factory-1.0.4/setup.py` & `database-factory-1.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,52 +32,109 @@
 __NAME__ = "database-factory"
 
 ROOT = os.path.dirname(os.path.abspath(__file__))
 VERSION_FILE = os.path.join(ROOT, __NAME__.replace("-", "_"), ".version")
 VERSION_RE = re.compile(r'''__version__ = ['"]([0-9.]+)['"]''')
 
 base = [
-    "sqlalchemy",                     # Database Abstraction Library
-    "pandas",                         # Powerful data structures for data analysis,
-                                      # time series, and statistics
-    "numpy"                           # NumPy is the fundamental package for array
-                                      # computing with Python.
+    # Database Abstraction Library
+    "sqlalchemy==1.4.47",
+    # Powerful data structures for data analysis, time series, and statistics
+    "pandas==1.5.3"
+
 ]
 
 aws = [
-    "boto3"                           # The AWS SDK for Python
+    # The AWS SDK for Python
+    "boto3==1.26.113"
 ]
 
 gcp = [
-    "google-cloud-bigquery",          # Google BigQuery API client library
-    "google-api-python-client",       # Google API Client Library for Python
-    "google-cloud-bigquery-storage",  # Google BigQuery Storage API client library
-    "google-cloud-secret-manager",    # Google Secret Manager API API client library
-    "google-cloud-resource-manager",  # Google Cloud Resource Manager API client lib
-    "pybigquery",                     # SQLAlchemy dialect for BigQuery
-    "pyarrow"                         # Python library for Apache Arrow
+    # This library simplifies using Google’s various server-to-server authentication mechanisms to access Google APIs.
+    "google-auth==2.17.3",
+    # This library provides an httplib2 transport for google-auth.
+    "google-auth-httplib2==0.1.0",
+    # Google BigQuery API client library
+    "google-cloud-bigquery==3.9.0",
+    # Google API Client Library for Python
+    "google-api-python-client==2.85.0",
+    # Google Secret Manager API API client library
+    "google-cloud-secret-manager==2.16.1",
+    # Google Cloud Resource Manager API client lib
+    "google-cloud-resource-manager==1.9.1",
+    # SQLAlchemy dialect for BigQuery
+    "pybigquery==0.10.2"
 ]
 
 snowflake = [
-    "snowflake-connector-python",     # Snowflake Connector Library
-    "snowflake-sqlalchemy",           # Snowflake SQLAlchemy Dialect
-    "requests"                        # Python HTTP for Humans.
+    # Snowflake Connector Library
+    "snowflake-connector-python==2.7.9",
+    # Snowflake SQLAlchemy Dialect
+    "snowflake-sqlalchemy==1.4.7"
 ]
 
 postgres = [
-    "pg8000"                          # PostgreSQL interface library.
+    # PostgreSQL interface library.
+    "pg8000==1.29.4"
 ]
 
 mysql = [
-    "pymysql"                         # Pure Python MySQL Driver
+    # Pure Python MySQL Driver
+    "pymysql"
+]
+
+dependencies = [
+    "asn1crypto==1.5.1",
+    "botocore==1.29.113",
+    "cachetools==5.3.0",
+    "certifi==2022.12.7",
+    "cffi==1.15.1",
+    "charset-normalizer==2.0.12",
+    "cryptography==36.0.2",
+    "future==0.18.3",
+    "google-api-core==2.11.0",
+    "google-cloud-bigquery-storage==2.19.1",
+    "google-cloud-core==2.3.2",
+    "google-crc32c==1.5.0",
+    "google-resumable-media==2.4.1",
+    "googleapis-common-protos==1.59.0",
+    "greenlet==2.0.2",
+    "grpc-google-iam-v1==0.12.6",
+    "grpcio==1.53.0",
+    "httplib2==0.22.0",
+    "idna==3.4",
+    "jmespath==1.0.1",
+    "numpy==1.24.2",
+    "oscrypto==1.3.0",
+    "packaging==23.1",
+    "proto-plus==1.22.2",
+    "protobuf==4.22.3",
+    "pyarrow==6.0.1",
+    "pyasn1==0.4.8",
+    "pyasn1-modules==0.2.8",
+    "pycparser==2.21",
+    "pycryptodomex==3.17",
+    "pyjwt==2.6.0",
+    "pymysql==1.0.3",
+    "pyopenssl==22.0.0",
+    "pyparsing==3.0.9",
+    "python-dateutil==2.8.2",
+    "pytz==2023.3",
+    "requests==2.28.2",
+    "rsa==4.9",
+    "s3transfer==0.6.0",
+    "scramp==1.4.4",
+    "six==1.16.0",
+    "uritemplate==4.1.1",
+    "urllib3==1.26.15"
 ]
 
 setups = []
 
-ir = (base + aws + gcp + snowflake + postgres + mysql)
+ir = (base + aws + gcp + snowflake + postgres + mysql + dependencies)
 requires = ir
 
 
 def delete(path):
     if os.path.exists(path=path):
         try:
             if os.path.isfile(path=path):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

