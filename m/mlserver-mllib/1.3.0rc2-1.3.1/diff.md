# Comparing `tmp/mlserver-mllib-1.3.0rc2.tar.gz` & `tmp/mlserver-mllib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-mllib-1.3.0rc2.tar", last modified: Thu Apr  6 15:39:33 2023, max compression
+gzip compressed data, was "mlserver-mllib-1.3.1.tar", last modified: Fri Apr 14 18:06:25 2023, max compression
```

## Comparing `mlserver-mllib-1.3.0rc2.tar` & `mlserver-mllib-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:39:33.637978 mlserver-mllib-1.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-06 15:39:33.633978 mlserver-mllib-1.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:39:33.633978 mlserver-mllib-1.3.0rc2/mlserver_mllib/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib/mllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:39:33.633978 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-06 15:39:33.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-06 15:39:33.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:39:33.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 15:39:33.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 15:39:33.000000 mlserver-mllib-1.3.0rc2/mlserver_mllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:39:33.637978 mlserver-mllib-1.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-06 15:38:54.000000 mlserver-mllib-1.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:25.270398 mlserver-mllib-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 18:06:25.270398 mlserver-mllib-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:25.270398 mlserver-mllib-1.3.1/mlserver_mllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/mlserver_mllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/mlserver_mllib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/mlserver_mllib/mllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/mlserver_mllib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/mlserver_mllib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:25.270398 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 18:06:25.000000 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 18:06:25.000000 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:25.000000 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 18:06:25.000000 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:06:25.000000 mlserver-mllib-1.3.1/mlserver_mllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:06:25.270398 mlserver-mllib-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-14 18:05:54.000000 mlserver-mllib-1.3.1/setup.py
```

### Comparing `mlserver-mllib-1.3.0rc2/LICENSE` & `mlserver-mllib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.0rc2/mlserver_mllib/mllib.py` & `mlserver-mllib-1.3.1/mlserver_mllib/mllib.py`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.0rc2/mlserver_mllib/utils.py` & `mlserver-mllib-1.3.1/mlserver_mllib/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.0rc2/setup.py` & `mlserver-mllib-1.3.1/setup.py`

 * *Files identical despite different names*

