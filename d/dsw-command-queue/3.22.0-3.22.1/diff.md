# Comparing `tmp/dsw-command-queue-3.22.0.tar.gz` & `tmp/dsw-command-queue-3.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-command-queue-3.22.0.tar", last modified: Tue Apr  4 15:01:48 2023, max compression
+gzip compressed data, was "dsw-command-queue-3.22.1.tar", last modified: Fri Apr 14 12:55:20 2023, max compression
```

## Comparing `dsw-command-queue-3.22.0.tar` & `dsw-command-queue-3.22.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:48.672277 dsw-command-queue-3.22.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-04 15:01:48.672277 dsw-command-queue-3.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:48.668277 dsw-command-queue-3.22.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:48.672277 dsw-command-queue-3.22.0/dsw/command_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/dsw/command_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw/command_queue/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/dsw/command_queue/command_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:48.672277 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 15:01:48.000000 dsw-command-queue-3.22.0/dsw_command_queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:48.676277 dsw-command-queue-3.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:36.000000 dsw-command-queue-3.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/dsw/command_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/dsw/command_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw/command_queue/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/dsw/command_queue/command_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:20.000000 dsw-command-queue-3.22.1/dsw_command_queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:20.394454 dsw-command-queue-3.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:16.000000 dsw-command-queue-3.22.1/setup.py
```

### Comparing `dsw-command-queue-3.22.0/LICENSE` & `dsw-command-queue-3.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.22.0/PKG-INFO` & `dsw-command-queue-3.22.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
```

### Comparing `dsw-command-queue-3.22.0/README.md` & `dsw-command-queue-3.22.1/README.md`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.22.0/dsw/command_queue/command_queue.py` & `dsw-command-queue-3.22.1/dsw/command_queue/command_queue.py`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.22.0/dsw_command_queue.egg-info/PKG-INFO` & `dsw-command-queue-3.22.1/dsw_command_queue.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
```

### Comparing `dsw-command-queue-3.22.0/pyproject.toml` & `dsw-command-queue-3.22.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-command-queue'
-version = "3.22.0"
+version = "3.22.1"
 description = 'Library for working with command queue and persistent commands'
 readme = 'README.md'
 keywords = ['dsw', 'subscriber', 'publisher', 'database', 'queue', 'processing']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -23,15 +23,15 @@
     'Topic :: Database',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
 requires-python = '>=3.7, <4'
 dependencies = [
     # DSW
-    "dsw-database==3.22.0",
+    "dsw-database==3.22.1",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

