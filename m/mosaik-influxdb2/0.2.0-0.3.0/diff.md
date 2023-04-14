# Comparing `tmp/mosaik_influxdb2-0.2.0.tar.gz` & `tmp/mosaik_influxdb2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik_influxdb2-0.2.0.tar", max compression
+gzip compressed data, was "mosaik_influxdb2-0.3.0.tar", max compression
```

## Comparing `mosaik_influxdb2-0.2.0.tar` & `mosaik_influxdb2-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     2208 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/mosaik/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/mosaik/components/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/mosaik/components/influxdb2/__init__.py
--rwxr-xr-x   0        0        0     4942 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/mosaik/components/influxdb2/writer.py
--rw-r--r--   0        0        0      495 2023-02-15 15:50:24.750584 mosaik_influxdb2-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 mosaik_influxdb2-0.2.0/setup.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 mosaik_influxdb2-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-14 11:46:45.345411 mosaik_influxdb2-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0     2208 2023-04-14 11:46:45.345411 mosaik_influxdb2-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 11:46:45.346411 mosaik_influxdb2-0.3.0/mosaik/components/influxdb2/__init__.py
+-rwxr-xr-x   0        0        0     4942 2023-04-14 11:46:45.346411 mosaik_influxdb2-0.3.0/mosaik/components/influxdb2/writer.py
+-rw-r--r--   0        0        0      495 2023-04-14 11:46:45.346411 mosaik_influxdb2-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 mosaik_influxdb2-0.3.0/PKG-INFO
```

### Comparing `mosaik_influxdb2-0.2.0/LICENSE` & `mosaik_influxdb2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaik_influxdb2-0.2.0/README.md` & `mosaik_influxdb2-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mosaik_influxdb2-0.2.0/mosaik/components/influxdb2/writer.py` & `mosaik_influxdb2-0.3.0/mosaik/components/influxdb2/writer.py`

 * *Files identical despite different names*

### Comparing `mosaik_influxdb2-0.2.0/PKG-INFO` & `mosaik_influxdb2-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-influxdb2
-Version: 0.2.0
+Version: 0.3.0
 Summary: An adapter to connect mosaik with InfluxDB 2
 License: MIT
 Author: Eike Schulte
 Author-email: eike.schulte@offis.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

