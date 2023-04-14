# Comparing `tmp/via-hub-logistc-0.0.9.tar.gz` & `tmp/via-hub-logistc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-hub-logistc-0.0.9.tar", max compression
+gzip compressed data, was "via-hub-logistc-1.0.0.tar", max compression
```

## Comparing `via-hub-logistc-0.0.9.tar` & `via-hub-logistc-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0      434 2023-03-04 02:38:25.977047 via-hub-logistc-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1568 2023-03-03 21:35:57.553317 via-hub-logistc-0.0.9/README.md
--rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-0.0.9/via_hub_logistc/__init__.py
--rw-r--r--   0        0        0      671 2023-03-04 01:33:48.330516 via-hub-logistc-0.0.9/via_hub_logistc/core/via_atlassian.py
--rw-r--r--   0        0        0     1788 2023-03-04 01:34:08.362573 via-hub-logistc-0.0.9/via_hub_logistc/core/via_azure.py
--rw-r--r--   0        0        0     1141 2023-03-04 01:10:40.466266 via-hub-logistc-0.0.9/via_hub_logistc/core/via_file.py
--rw-r--r--   0        0        0      409 2023-03-04 01:33:59.718219 via-hub-logistc-0.0.9/via_hub_logistc/core/via_scenario.py
--rw-r--r--   0        0        0      597 2023-03-04 01:09:25.003935 via-hub-logistc-0.0.9/via_hub_logistc/core/via_timer.py
--rw-r--r--   0        0        0     2892 2023-03-04 02:27:35.419563 via-hub-logistc-0.0.9/via_hub_logistc/core/via_zephry.py
--rw-r--r--   0        0        0     1143 2023-03-04 01:20:18.640682 via-hub-logistc-0.0.9/via_hub_logistc/model/zephry.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.9/setup.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-04-14 13:29:22.164363 via-hub-logistc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7347 2023-04-12 22:34:20.470829 via-hub-logistc-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-1.0.0/via_hub_logistc/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-12 22:34:20.479827 via-hub-logistc-1.0.0/via_hub_logistc/core/via_file.py
+-rw-r--r--   0        0        0      276 2023-04-12 22:34:20.482829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_number.py
+-rw-r--r--   0        0        0     9591 2023-04-04 16:49:43.006120 via-hub-logistc-1.0.0/via_hub_logistc/core/via_report.py
+-rw-r--r--   0        0        0      418 2023-04-12 22:34:20.485828 via-hub-logistc-1.0.0/via_hub_logistc/core/via_scenario.py
+-rw-r--r--   0        0        0      549 2023-04-12 22:34:20.487829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_text.py
+-rw-r--r--   0        0        0      599 2023-04-12 22:34:20.490829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_timer.py
+-rw-r--r--   0        0        0     1097 2023-04-12 17:18:04.992073 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_db2.py
+-rw-r--r--   0        0        0     1888 2023-04-12 17:18:43.091789 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_microsoft.py
+-rw-r--r--   0        0        0     1664 2023-04-12 17:19:00.638957 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_mongodb.py
+-rw-r--r--   0        0        0      307 2023-04-04 15:39:11.800307 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_text.py
+-rw-r--r--   0        0        0     1143 2023-03-06 17:06:38.522855 via-hub-logistc-1.0.0/via_hub_logistc/model/zephry.py
+-rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.0/setup.py
+-rw-r--r--   0        0        0     7514 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.0/PKG-INFO
```

### Comparing `via-hub-logistc-0.0.9/via_hub_logistc/core/via_azure.py` & `via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_microsoft.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from azure.storage.blob import BlobServiceClient
 
 from robot.api.deco import keyword
 from robot.api import Error
 
-class Blob():
-    ###connect to blob service###
-    @keyword(name="conect azure blob")
-    def conect_azure_blob(self, host, account_name, account_key):
+class ViaAzure():
+    ###Return the one connction with azure blob server###
+    @keyword(name="Azure Connect Blob Server")
+    def azure_connect_blob_server(self, host:str, account_name:str, account_key:str):
         try:
             str_conn = f'DefaultEndpointsProtocol=https;AccountName={account_name};AccountKey={account_key};EndpointsSuffix={host}'
 
             return  BlobServiceClient.from_connection_string(str_conn)
         except Exception as e:
             raise Error(e)
 
-
-    ###List all directories in a container###
-    @keyword(name="list all directories in container")
-    def list_all_directories_in_container(self, connection, container_name, folder, format=True):
+    ###Return the json with all directories in a container###
+    @keyword(name="Azure List All Directories In Container")
+    def azure_list_all_directories_in_container(self, connection, container_name:str, folder:str, format=True):
         try:
-
             client = connection.get_container_client(container_name)
 
             directories = []
 
             for file in client.walk_blobs(folder, delimiter='/'):
                 if format == False:
                     directories.append(file.name)
                 else:
                     directories.append(file.name[4:-1])
 
             return directories
         except Exception as e:
             raise Error(e)
     
-    ### checks if the folder exists in the container ###
-    @keyword(name="is exist directory in container")
-    def is_exist_directory_in_container(self, connection, container_name, folder, directory):
+    ### Return if the folder exists in the container ###
+    @keyword(name="Azure Is Exist Directory In Container")
+    def azure_is_exist_directory_in_container(self, connection, container_name:str, folder:str, directory:str):
         try:
-
             client = connection.get_container_client(container_name)
 
             for file in client.walk_blobs(folder, delimiter='/'):
                 if directory.casefold() == str(file.name[4:-1]).casefold():
-                    return file.name[4:-1]
+                    return True
 
-            return None
+            return False
         except Exception as e:
             raise Error(e)
```

### Comparing `via-hub-logistc-0.0.9/via_hub_logistc/core/via_file.py` & `via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_db2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-import random
-import yaml
+import ibm_db
 
+from robot.api.deco import keyword
 from robot.api import Error
-from yaml.loader import SafeLoader
 
 
-class FileYaml():
-    ### Load data file yaml  ###
-    def read_yaml_file(self, filename):
-        absolute_path = f'{filename}.yaml'
+class ViaDb2():
+    ### Return conncection with db2 ###
+    @keyword(name="Db2 Connect To Database")
+    def db2_connect_to_database(self, host:str, db_name:str, user_id:str, password:str):
         try:
-            with open(absolute_path) as f:
-                return yaml.load(f, Loader=SafeLoader)
+            connString = f"ATTACH=FALSE;DATABASE={db_name};HOSTNAME={host};PROTOCOL=TCPIP;UID={user_id};PWD={password}"
+            return ibm_db.connect(connString, '', '')
         except Exception as e:
             raise Error(e)
+    
+    ### Return json with result the of query ###
+    @keyword(name="Db2 Execute Query")
+    def db2_execute_query(self, connection, query:str):
+        lsr_result = []
 
-
-class Text():
-    ### Split text informations $text and $length cut  ###
-    def split_text(self, text, length, start=0):
         try:
-            return str(text)[start: int(length)]
-        except Exception as e:
-            raise Error(e)
+            stmt = ibm_db.exec_immediate(connection, query)
+            result = ibm_db.fetch_assoc(stmt)
 
+            while(result):
+                if type(result) != bool:
+                    lsr_result.append(result)
 
-### Cut text informations $separator and $length cut  ###
+                result = ibm_db.fetch_assoc(stmt)
 
-    def cut_text(self, text, separator, maxsplit):
-        try:
-            return str(text).rsplit(separator, -1)[maxsplit]
-        except Exception as e:
-            raise Error(e)
-
-
-class Number():
-    ### choose number in range the numbers  ###
-    def choose_number(self, obj):
-        try:
-            return random.randrange(1, obj)
+            return lsr_result
         except Exception as e:
             raise Error(e)
```

### Comparing `via-hub-logistc-0.0.9/via_hub_logistc/core/via_timer.py` & `via-hub-logistc-1.0.0/via_hub_logistc/core/via_timer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from robot.api import Error
 
-class Timer():
-    ### calculate  date in two date###
+class ViaTimer():
+    ### calculate date in two date###
     def interval(start, end):
         try:
 
             d1 = datetime.strptime(start, '%Y%m%d %H:%M:%S.%f')
             d2 = datetime.strptime(end, '%Y%m%d %H:%M:%S.%f')
 
             return d2 - d1
```

### Comparing `via-hub-logistc-0.0.9/via_hub_logistc/model/zephry.py` & `via-hub-logistc-1.0.0/via_hub_logistc/model/zephry.py`

 * *Files identical despite different names*

