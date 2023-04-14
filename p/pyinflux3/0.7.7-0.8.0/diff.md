# Comparing `tmp/pyinflux3-0.7.7.tar.gz` & `tmp/pyinflux3-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.7.tar", last modified: Fri Apr 14 08:21:30 2023, max compression
+gzip compressed data, was "pyinflux3-0.8.0.tar", last modified: Fri Apr 14 08:42:12 2023, max compression
```

## Comparing `pyinflux3-0.7.7.tar` & `pyinflux3-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/influxdb_client_3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 08:21:30.000000 pyinflux3-0.7.7/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 08:21:29.000000 pyinflux3-0.7.7/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 08:21:24.000000 pyinflux3-0.7.7/setup-client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:21:30.013379 pyinflux3-0.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:12.582271 pyinflux3-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 08:42:12.578271 pyinflux3-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 08:42:05.000000 pyinflux3-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:12.578271 pyinflux3-0.8.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-14 08:42:05.000000 pyinflux3-0.8.0/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:12.578271 pyinflux3-0.8.0/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 08:42:12.000000 pyinflux3-0.8.0/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 08:42:12.000000 pyinflux3-0.8.0/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:42:12.000000 pyinflux3-0.8.0/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 08:42:12.000000 pyinflux3-0.8.0/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 08:42:12.000000 pyinflux3-0.8.0/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 08:42:05.000000 pyinflux3-0.8.0/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:42:12.582271 pyinflux3-0.8.0/setup.cfg
```

### Comparing `pyinflux3-0.7.7/PKG-INFO` & `pyinflux3-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-Metadata-Version: 2.1
-Name: pyinflux3
-Version: 0.7.7
-Summary: Community Python client for InfluxDB IOx
-Home-page: https://github.com/InfluxCommunity/pyinflux3
-Author: InfluxData
-Author-email: contact@influxdata.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: cli
-
 # About
 This is a community repository of Python code for InfluxDB with IOx. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
+# Install
+To install only the client:
+```bash
+python3 -m pip install pyinflux3
+```
+To install the client and CLI:
+```bash
+sudo python3 -m pip install "pyinflux3[cli]"
+```
+***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
+
 # Add a Config
 You can drop a config file called config.json in the directory where you are running the influx3 command:
 
 ```json
 {
 {
     "my-config": {
```

### Comparing `pyinflux3-0.7.7/influxdb_client_3/__init__.py` & `pyinflux3-0.8.0/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.7/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.7
+Version: 0.8.0
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,25 @@
 # About
 This is a community repository of Python code for InfluxDB with IOx. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
+# Install
+To install only the client:
+```bash
+python3 -m pip install pyinflux3
+```
+To install the client and CLI:
+```bash
+sudo python3 -m pip install "pyinflux3[cli]"
+```
+***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
+
 # Add a Config
 You can drop a config file called config.json in the directory where you are running the influx3 command:
 
 ```json
 {
 {
     "my-config": {
```

### Comparing `pyinflux3-0.7.7/setup-client.py` & `pyinflux3-0.8.0/setup-client.py`

 * *Files identical despite different names*

