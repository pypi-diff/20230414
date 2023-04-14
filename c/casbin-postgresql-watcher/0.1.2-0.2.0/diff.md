# Comparing `tmp/casbin-postgresql-watcher-0.1.2.tar.gz` & `tmp/casbin-postgresql-watcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-postgresql-watcher-0.1.2.tar", last modified: Tue May 17 11:16:44 2022, max compression
+gzip compressed data, was "casbin-postgresql-watcher-0.2.0.tar", last modified: Fri Apr 14 13:46:37 2023, max compression
```

## Comparing `casbin-postgresql-watcher-0.1.2.tar` & `casbin-postgresql-watcher-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 11:16:44.023000 casbin-postgresql-watcher-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-17 11:16:08.000000 casbin-postgresql-watcher-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-05-17 11:16:44.023000 casbin-postgresql-watcher-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-05-17 11:16:08.000000 casbin-postgresql-watcher-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 11:16:44.023000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-05-17 11:16:43.000000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-17 11:16:43.000000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 11:16:43.000000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-17 11:16:43.000000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-17 11:16:43.000000 casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 11:16:44.023000 casbin-postgresql-watcher-0.1.2/postgresql_watcher/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-17 11:16:08.000000 casbin-postgresql-watcher-0.1.2/postgresql_watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3914 2022-05-17 11:16:08.000000 casbin-postgresql-watcher-0.1.2/postgresql_watcher/watcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-17 11:16:44.023000 casbin-postgresql-watcher-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-05-17 11:16:08.000000 casbin-postgresql-watcher-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:46:37.538399 casbin-postgresql-watcher-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 13:46:37.538399 casbin-postgresql-watcher-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:46:37.538399 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 13:46:37.000000 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 13:46:37.000000 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:46:37.000000 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 13:46:37.000000 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 13:46:37.000000 casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:46:37.538399 casbin-postgresql-watcher-0.2.0/postgresql_watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/postgresql_watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/postgresql_watcher/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 13:46:37.542400 casbin-postgresql-watcher-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:46:37.538399 casbin-postgresql-watcher-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 13:45:57.000000 casbin-postgresql-watcher-0.2.0/tests/test_postgresql_watcher.py
```

### Comparing `casbin-postgresql-watcher-0.1.2/LICENSE` & `casbin-postgresql-watcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-postgresql-watcher-0.1.2/PKG-INFO` & `casbin-postgresql-watcher-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-postgresql-watcher
-Version: 0.1.2
+Version: 0.2.0
 Summary: Casbin role watcher to be used for monitoring updates to policies for PyCasbin
 Home-page: https://github.com/pycasbin/postgresql-watcher
 Author: hsluoyz
 Author-email: hsluoyz@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -39,7 +39,24 @@
 from casbin.persist.adapters import FileAdapter
 
 casbin_enforcer = CasbinEnforcer(app, adapter)
 watcher = PostgresqlWatcher(host=HOST, port=PORT, user=USER, password=PASSWORD, dbname=DBNAME)
 watcher.set_update_callback(casbin_enforcer.e.load_policy)
 casbin_enforcer.set_watcher(watcher)
 ```
+
+## Basic Usage Example With SSL Enabled
+
+See [PostgresQL documentation](https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS) for full details of SSL parameters.
+
+### With Flask-authz
+```python
+from flask_authz import CasbinEnforcer
+from postgresql_watcher import PostgresqlWatcher
+from flask import Flask
+from casbin.persist.adapters import FileAdapter
+
+casbin_enforcer = CasbinEnforcer(app, adapter)
+watcher = PostgresqlWatcher(host=HOST, port=PORT, user=USER, password=PASSWORD, dbname=DBNAME, sslmode="verify_full", sslcert=SSLCERT, sslrootcert=SSLROOTCERT, sslkey=SSLKEY)
+watcher.set_update_callback(casbin_enforcer.e.load_policy)
+casbin_enforcer.set_watcher(watcher)
+```
```

### Comparing `casbin-postgresql-watcher-0.1.2/casbin_postgresql_watcher.egg-info/PKG-INFO` & `casbin-postgresql-watcher-0.2.0/casbin_postgresql_watcher.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-postgresql-watcher
-Version: 0.1.2
+Version: 0.2.0
 Summary: Casbin role watcher to be used for monitoring updates to policies for PyCasbin
 Home-page: https://github.com/pycasbin/postgresql-watcher
 Author: hsluoyz
 Author-email: hsluoyz@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -39,7 +39,24 @@
 from casbin.persist.adapters import FileAdapter
 
 casbin_enforcer = CasbinEnforcer(app, adapter)
 watcher = PostgresqlWatcher(host=HOST, port=PORT, user=USER, password=PASSWORD, dbname=DBNAME)
 watcher.set_update_callback(casbin_enforcer.e.load_policy)
 casbin_enforcer.set_watcher(watcher)
 ```
+
+## Basic Usage Example With SSL Enabled
+
+See [PostgresQL documentation](https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS) for full details of SSL parameters.
+
+### With Flask-authz
+```python
+from flask_authz import CasbinEnforcer
+from postgresql_watcher import PostgresqlWatcher
+from flask import Flask
+from casbin.persist.adapters import FileAdapter
+
+casbin_enforcer = CasbinEnforcer(app, adapter)
+watcher = PostgresqlWatcher(host=HOST, port=PORT, user=USER, password=PASSWORD, dbname=DBNAME, sslmode="verify_full", sslcert=SSLCERT, sslrootcert=SSLROOTCERT, sslkey=SSLKEY)
+watcher.set_update_callback(casbin_enforcer.e.load_policy)
+casbin_enforcer.set_watcher(watcher)
+```
```

### Comparing `casbin-postgresql-watcher-0.1.2/postgresql_watcher/watcher.py` & `casbin-postgresql-watcher-0.2.0/postgresql_watcher/watcher.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,23 +13,31 @@
     host: str,
     user: str,
     password: str,
     port: Optional[int] = 5432,
     dbname: Optional[str] = "postgres",
     delay: Optional[int] = 2,
     channel_name: Optional[str] = POSTGRESQL_CHANNEL_NAME,
+    sslmode: Optional[str] = None,
+    sslrootcert: Optional[str] = None,
+    sslcert: Optional[str] = None,
+    sslkey: Optional[str] = None
 ):
     # delay connecting to postgresql (postgresql connection failure)
     time.sleep(delay)
     conn = connect(
         host=host,
         port=port,
         user=user,
         password=password,
-        dbname=dbname
+        dbname=dbname,
+        sslmode=sslmode,
+        sslrootcert=sslrootcert,
+        sslcert=sslcert,
+        sslkey=sslkey
     )
     # Can only receive notifications when not in transaction, set this for easier usage
     conn.set_isolation_level(extensions.ISOLATION_LEVEL_AUTOCOMMIT)
     curs = conn.cursor()
     curs.execute(f"LISTEN {channel_name};")
     print("Waiting for casbin policy update")
     while True and not curs.closed:
@@ -48,23 +56,31 @@
         host: str,
         user: str,
         password: str,
         port: Optional[int] = 5432,
         dbname: Optional[str] = "postgres",
         channel_name: Optional[str] = POSTGRESQL_CHANNEL_NAME,
         start_process: Optional[bool] = True,
+        sslmode: Optional[str] = None,
+        sslrootcert: Optional[str] = None,
+        sslcert: Optional[str] = None,
+        sslkey: Optional[str] = None
     ):
         self.update_callback = None
         self.parent_conn = None
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.dbname = dbname
         self.channel_name = channel_name
+        self.sslmode = sslmode
+        self.sslrootcert = sslrootcert
+        self.sslcert = sslcert
+        self.sslkey = sslkey
         self.subscribed_process = self.create_subscriber_process(start_process)
 
     def create_subscriber_process(
         self,
         start_process: Optional[bool] = True,
         delay: Optional[int] = 2,
     ):
@@ -78,14 +94,18 @@
                 self.host,
                 self.user,
                 self.password,
                 self.port,
                 self.dbname,
                 delay,
                 self.channel_name,
+                self.sslmode,
+                self.sslrootcert,
+                self.sslcert,
+                self.sslkey
             ),
             daemon=True,
         )
         if start_process:
             p.start()
         return p
 
@@ -96,14 +116,18 @@
     def update(self):
         conn = connect(
             host=self.host,
             port=self.port,
             user=self.user,
             password=self.password,
             dbname=self.dbname,
+            sslmode=self.sslmode,
+            sslrootcert=self.sslrootcert,
+            sslcert=self.sslcert,
+            sslkey=self.sslkey
         )
         # Can only receive notifications when not in transaction, set this for easier usage
         conn.set_isolation_level(extensions.ISOLATION_LEVEL_AUTOCOMMIT)
         curs = conn.cursor()
         curs.execute(
             f"NOTIFY {self.channel_name},'casbin policy update at {time.time()}'"
         )
```

### Comparing `casbin-postgresql-watcher-0.1.2/setup.py` & `casbin-postgresql-watcher-0.2.0/setup.py`

 * *Files identical despite different names*

