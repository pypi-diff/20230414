# Comparing `tmp/pyinflux3-cli-0.7.7.tar.gz` & `tmp/pyinflux3-cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.7.7.tar", last modified: Fri Apr 14 08:21:29 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.8.0.tar", last modified: Fri Apr 14 08:42:11 2023, max compression
```

## Comparing `pyinflux3-cli-0.7.7.tar` & `pyinflux3-cli-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/influxdb_cli/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 08:21:29.000000 pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-14 08:21:23.000000 pyinflux3-cli-0.7.7/setup-cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:21:29.476717 pyinflux3-cli-0.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:11.915275 pyinflux3-cli-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-14 08:42:11.915275 pyinflux3-cli-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 08:42:04.000000 pyinflux3-cli-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:11.915275 pyinflux3-cli-0.8.0/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:04.000000 pyinflux3-cli-0.8.0/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-14 08:42:04.000000 pyinflux3-cli-0.8.0/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:42:11.915275 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 08:42:11.000000 pyinflux3-cli-0.8.0/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-14 08:42:04.000000 pyinflux3-cli-0.8.0/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:42:11.915275 pyinflux3-cli-0.8.0/setup.cfg
```

### Comparing `pyinflux3-cli-0.7.7/PKG-INFO` & `pyinflux3-cli-0.8.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-Metadata-Version: 2.1
-Name: pyinflux3-cli
-Version: 0.7.7
-Summary: Community Python client for InfluxDB IOx (CLI)
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

### Comparing `pyinflux3-cli-0.7.7/influxdb_cli/influx3.py` & `pyinflux3-cli-0.8.0/influxdb_cli/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.7.7/pyinflux3_cli.egg-info/PKG-INFO` & `pyinflux3-cli-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.7.7
+Version: 0.8.0
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,25 @@
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

### Comparing `pyinflux3-cli-0.7.7/setup-cli.py` & `pyinflux3-cli-0.8.0/setup-cli.py`

 * *Files identical despite different names*

