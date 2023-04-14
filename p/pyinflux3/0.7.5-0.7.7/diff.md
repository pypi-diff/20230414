# Comparing `tmp/pyinflux3-0.7.5.tar.gz` & `tmp/pyinflux3-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.5.tar", last modified: Thu Apr 13 14:47:44 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.7.tar", last modified: Fri Apr 14 08:21:30 2023, max compression
```

## Comparing `pyinflux3-0.7.5.tar` & `pyinflux3-0.7.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.691131 pyinflux3-0.7.5/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 14:47:44.690784 pyinflux3-0.7.5/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.5/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.686756 pyinflux3-0.7.5/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.5/influxdb_client_3/__init__.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.690122 pyinflux3-0.7.5/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      219 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)      101 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)     1794 2023-04-13 14:47:39.000000 pyinflux3-0.7.5/setup-client.py
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 14:47:44.691234 pyinflux3-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 08:21:30.000000 pyinflux3-0.7.7/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/setup.cfg
```

### Comparing `pyinflux3-0.7.5/PKG-INFO` & `pyinflux3-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.5
+Version: 0.7.7
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.5/README.md` & `pyinflux3-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.5/influxdb_client_3/__init__.py` & `pyinflux3-0.7.7/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.5/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.7/pyinflux3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.5
+Version: 0.7.7
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.5/setup-client.py` & `pyinflux3-0.7.7/setup-client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 import os
 import re
 
 binary_name = "influx3"
 binary_destination = os.path.join("bin", binary_name)
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("./README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def get_version_from_github_ref():
     github_ref = os.environ.get("GITHUB_REF")
     if not github_ref:
         return None
```

