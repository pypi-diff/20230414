# Comparing `tmp/tinybird-cdk-0.16.4.tar.gz` & `tmp/tinybird-cdk-0.16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.16.4.tar", last modified: Thu Apr 13 14:46:55 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.16.5.tar", last modified: Fri Apr 14 14:16:06 2023, max compression
```

## Comparing `tinybird-cdk-0.16.4.tar` & `tinybird-cdk-0.16.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.086019 tinybird-cdk-0.16.4/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 14:46:55.086019 tinybird-cdk-0.16.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:46:55.086019 tinybird-cdk-0.16.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.082019 tinybird-cdk-0.16.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.082019 tinybird-cdk-0.16.4/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.082019 tinybird-cdk-0.16.4/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.086019 tinybird-cdk-0.16.4/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 14:46:44.000000 tinybird-cdk-0.16.4/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:46:55.082019 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 14:46:55.000000 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-13 14:46:55.000000 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:46:55.000000 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 14:46:55.000000 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 14:46:55.000000 tinybird-cdk-0.16.4/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.16.4/README.md` & `tinybird-cdk-0.16.5/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/setup.py` & `tinybird-cdk-0.16.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.16.4',
+    version='0.16.5',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.16.4/tests/test_gcp.py` & `tinybird-cdk-0.16.5/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.16.5/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.16.5/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.16.5/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/config.py` & `tinybird-cdk-0.16.5/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connector.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.16.5/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/errors.py` & `tinybird-cdk-0.16.5/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/export.py` & `tinybird-cdk-0.16.5/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/formats.py` & `tinybird-cdk-0.16.5/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/logger.py` & `tinybird-cdk-0.16.5/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/schema.py` & `tinybird-cdk-0.16.5/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.16.5/tinybird_cdk/tinybird.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from . import config, errors, formats, logger
 from typing import Optional
 
 
 class Client:
     '''Tinybird client. All connectors have an instance of this class.'''
 
-    DS_PATH     = '/v0/datasources'
-    SQL_PATH    = '/v0/sql'
-    EVENTS_PATH = '/v0/events'
+    DS_PATH      = '/v0/datasources'
+    SQL_PATH     = '/v0/sql'
+    EVENTS_PATH  = '/v0/events'
+    LINKERS_PATH = '/v0/linkers'
 
     JOB_POLL_PERIOD_S     = 1.0
     MAX_RETRIES           = 5
     MAX_RATE_LIMIT_WAIT_S = 60*60
     MIN_WAIT_S = 60
 
     # By default, HTTPX uses a timeout of 5s. David said in
@@ -104,14 +105,35 @@
 
     # --- Truncate --------------------------------------------------------------------------------
 
     def truncate(self, data_source):
         logger.info(f'Truncating {data_source}')
         return self._post(f'{self.DS_PATH}/{urllib.parse.quote(data_source)}/truncate')
 
+    # --- Alter -----------------------------------------------------------------------------------
+
+    def alter(self, data_source: str, schema: str):
+        logger.info(f'Altering {data_source} with schema {schema}')
+        params = {'name': data_source, 'schema': schema}
+        return self._post(f'{self.DS_PATH}/{urllib.parse.quote(data_source)}/alter', params=params)
+
+    # --- Linker -----------------------------------------------------------------------------------
+
+    def alter_linker(self, data_source: str, kind: str, schema: str):
+        logger.info(f'Altering linker for {data_source} with schema {schema}')
+        params = {'name': data_source, 'service': kind, 'query': schema}
+        return self._put(f'{self.LINKERS_PATH}/{urllib.parse.quote(data_source)}', params=params)
+
+    # --- Data Source -----------------------------------------------------------------------------------
+
+    def data_source(self, data_source: str):
+        logger.info(f'Getting info for data source {data_source}')
+        response = self._get(f'{self.DS_PATH}/{urllib.parse.quote(data_source)}')
+        return response.json()
+
     # --- Events ----------------------------------------------------------------------------------
 
     def append_event(self, event, data_source):
         params = {'name': data_source}
         return self._post(self.EVENTS_PATH, params=params, content=event)
 
     def append_events(self, events, data_source):
@@ -171,14 +193,19 @@
             return self._post(self.DS_PATH, params=params, files=files)
 
     def _post(self, path, headers=None, **kwargs):
         if headers is None:
             headers = {}
         return self._request('POST', path, headers=headers, **kwargs)
 
+    def _put(self, path, headers=None, **kwargs):
+        if headers is None:
+            headers = {}
+        return self._request('PUT', path, headers=headers, **kwargs)
+
     def _get(self, path, headers=None, **kwargs):
         if headers is None:
             headers = {}
         return self._request('GET', path, headers=headers, **kwargs)
 
     def _request(self, method, url_or_path, headers, **kwargs):
         if url_or_path.startswith('/'):
```

### Comparing `tinybird-cdk-0.16.4/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.16.5/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 tinybird_cdk/__init__.py
 tinybird_cdk/config.py
 tinybird_cdk/connector.py
 tinybird_cdk/errors.py
 tinybird_cdk/export.py
 tinybird_cdk/formats.py
 tinybird_cdk/logger.py
+tinybird_cdk/migration.py
 tinybird_cdk/schema.py
 tinybird_cdk/tinybird.py
 tinybird_cdk/utils.py
 tinybird_cdk.egg-info/PKG-INFO
 tinybird_cdk.egg-info/SOURCES.txt
 tinybird_cdk.egg-info/dependency_links.txt
 tinybird_cdk.egg-info/requires.txt
```

