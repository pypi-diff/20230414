# Comparing `tmp/dsw-database-3.22.0.tar.gz` & `tmp/dsw-database-3.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-database-3.22.0.tar", last modified: Tue Apr  4 15:01:45 2023, max compression
+gzip compressed data, was "dsw-database-3.22.1.tar", last modified: Fri Apr 14 12:55:32 2023, max compression
```

## Comparing `dsw-database-3.22.0.tar` & `dsw-database-3.22.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:45.147642 dsw-database-3.22.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-04 15:01:40.000000 dsw-database-3.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-04 15:01:45.147642 dsw-database-3.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-04 15:01:40.000000 dsw-database-3.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:45.143642 dsw-database-3.22.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:45.147642 dsw-database-3.22.0/dsw/database/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-04 15:01:40.000000 dsw-database-3.22.0/dsw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 15:01:44.000000 dsw-database-3.22.0/dsw/database/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-04-04 15:01:40.000000 dsw-database-3.22.0/dsw/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-04-04 15:01:40.000000 dsw-database-3.22.0/dsw/database/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:45.147642 dsw-database-3.22.0/dsw_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 15:01:45.000000 dsw-database-3.22.0/dsw_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-04 15:01:40.000000 dsw-database-3.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:45.147642 dsw-database-3.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:40.000000 dsw-database-3.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.658208 dsw-database-3.22.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:28.000000 dsw-database-3.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 12:55:32.654209 dsw-database-3.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 12:55:28.000000 dsw-database-3.22.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw/database/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 12:55:28.000000 dsw-database-3.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:32.658208 dsw-database-3.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:28.000000 dsw-database-3.22.1/setup.py
```

### Comparing `dsw-database-3.22.0/LICENSE` & `dsw-database-3.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.0/PKG-INFO` & `dsw-database-3.22.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.22.0/README.md` & `dsw-database-3.22.1/README.md`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.0/dsw/database/database.py` & `dsw-database-3.22.1/dsw/database/database.py`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.0/dsw/database/model.py` & `dsw-database-3.22.1/dsw/database/model.py`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.0/dsw_database.egg-info/PKG-INFO` & `dsw-database-3.22.1/dsw_database.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.22.0/pyproject.toml` & `dsw-database-3.22.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-database'
-version = "3.22.0"
+version = "3.22.1"
 description = 'Library for managing DSW database'
 readme = 'README.md'
 keywords = ['dsw', 'database']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -24,15 +24,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.7, <4'
 dependencies = [
     'psycopg[binary]',
     'tenacity',
     # DSW
-    "dsw-config==3.22.0",
+    "dsw-config==3.22.1",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

