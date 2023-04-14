# Comparing `tmp/pyinflux3-cli-0.7.4.tar.gz` & `tmp/pyinflux3-cli-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.7.4.tar", last modified: Thu Apr 13 14:43:41 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.7.7.tar", last modified: Fri Apr 14 08:21:29 2023, max compression
```

## Comparing `pyinflux3-cli-0.7.4.tar` & `pyinflux3-cli-0.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:41.217357 pyinflux3-cli-0.7.4/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2445 2023-04-13 14:43:41.217038 pyinflux3-cli-0.7.4/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-cli-0.7.4/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:41.212882 pyinflux3-cli-0.7.4/influxdb_cli/
--rw-r--r--   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:57:11.000000 pyinflux3-cli-0.7.4/influxdb_cli/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-cli-0.7.4/influxdb_cli/influx3.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:41.216521 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2445 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      295 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       54 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       88 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       13 2023-04-13 14:43:41.000000 pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)     1758 2023-04-13 14:31:24.000000 pyinflux3-cli-0.7.4/setup-cli.py
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 14:43:41.217451 pyinflux3-cli-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/setup.cfg
```

### Comparing `pyinflux3-cli-0.7.4/PKG-INFO` & `pyinflux3-cli-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.7.4
+Version: 0.7.7
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-cli-0.7.4/README.md` & `pyinflux3-cli-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.7.4/influxdb_cli/influx3.py` & `pyinflux3-cli-0.7.7/influxdb_cli/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.7.4/pyinflux3_cli.egg-info/PKG-INFO` & `pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.7.4
+Version: 0.7.7
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-cli-0.7.4/setup-cli.py` & `pyinflux3-cli-0.7.7/setup-cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 import re
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("./README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def get_version_from_github_ref():
     github_ref = os.environ.get("GITHUB_REF")
     if not github_ref:
         return None
```

