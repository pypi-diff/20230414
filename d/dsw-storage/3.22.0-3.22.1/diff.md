# Comparing `tmp/dsw-storage-3.22.0.tar.gz` & `tmp/dsw-storage-3.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-storage-3.22.0.tar", last modified: Tue Apr  4 15:01:43 2023, max compression
+gzip compressed data, was "dsw-storage-3.22.1.tar", last modified: Fri Apr 14 12:55:36 2023, max compression
```

## Comparing `dsw-storage-3.22.0.tar` & `dsw-storage-3.22.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:43.709724 dsw-storage-3.22.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-04 15:01:43.709724 dsw-storage-3.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:43.705724 dsw-storage-3.22.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:43.705724 dsw-storage-3.22.0/dsw/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/dsw/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw/storage/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/dsw/storage/s3storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:43.705724 dsw-storage-3.22.0/dsw_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 15:01:43.000000 dsw-storage-3.22.0/dsw_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:43.709724 dsw-storage-3.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:40.000000 dsw-storage-3.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:36.805125 dsw-storage-3.22.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 12:55:36.805125 dsw-storage-3.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:36.801125 dsw-storage-3.22.1/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:36.801125 dsw-storage-3.22.1/dsw/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/dsw/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw/storage/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/dsw/storage/s3storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:36.805125 dsw-storage-3.22.1/dsw_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:36.000000 dsw-storage-3.22.1/dsw_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:36.805125 dsw-storage-3.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:31.000000 dsw-storage-3.22.1/setup.py
```

### Comparing `dsw-storage-3.22.0/LICENSE` & `dsw-storage-3.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.22.0/PKG-INFO` & `dsw-storage-3.22.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
```

### Comparing `dsw-storage-3.22.0/README.md` & `dsw-storage-3.22.1/README.md`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.22.0/dsw/storage/s3storage.py` & `dsw-storage-3.22.1/dsw/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.22.0/dsw_storage.egg-info/PKG-INFO` & `dsw-storage-3.22.1/dsw_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
```

### Comparing `dsw-storage-3.22.0/pyproject.toml` & `dsw-storage-3.22.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-storage'
-version = "3.22.0"
+version = "3.22.1"
 description = 'Library for managing DSW S3 storage'
 readme = 'README.md'
 keywords = ['dsw', 's3', 'bucket', 'storage']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -24,15 +24,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.7, <4'
 dependencies = [
     'minio',
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

