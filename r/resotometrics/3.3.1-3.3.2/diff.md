# Comparing `tmp/resotometrics-3.3.1.tar.gz` & `tmp/resotometrics-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.3.1.tar", last modified: Fri Mar 31 23:52:54 2023, max compression
+gzip compressed data, was "resotometrics-3.3.2.tar", last modified: Fri Apr 14 16:12:07 2023, max compression
```

## Comparing `resotometrics-3.3.1.tar` & `resotometrics-3.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.256782 resotometrics-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 23:51:12.000000 resotometrics-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-03-31 23:52:54.256782 resotometrics-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-03-31 23:51:12.000000 resotometrics-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 23:51:12.000000 resotometrics-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.256782 resotometrics-3.3.1/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-31 23:51:12.000000 resotometrics-3.3.1/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.256782 resotometrics-3.3.1/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 23:52:54.000000 resotometrics-3.3.1/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:52:54.256782 resotometrics-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-31 23:51:12.000000 resotometrics-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.256782 resotometrics-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-31 23:51:12.000000 resotometrics-3.3.1/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:07.986926 resotometrics-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 16:10:26.000000 resotometrics-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-14 16:12:07.986926 resotometrics-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-14 16:10:26.000000 resotometrics-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:10:26.000000 resotometrics-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:07.986926 resotometrics-3.3.2/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-14 16:10:26.000000 resotometrics-3.3.2/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:07.986926 resotometrics-3.3.2/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 16:12:07.000000 resotometrics-3.3.2/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:12:07.986926 resotometrics-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 16:10:26.000000 resotometrics-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:07.986926 resotometrics-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 16:10:26.000000 resotometrics-3.3.2/test/test_args.py
```

### Comparing `resotometrics-3.3.1/PKG-INFO` & `resotometrics-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.3.1
+Version: 3.3.2
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.3.1/README.md` & `resotometrics-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics/__main__.py` & `resotometrics-3.3.2/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics/config.py` & `resotometrics-3.3.2/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics/default_metrics.yaml` & `resotometrics-3.3.2/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics/metrics.py` & `resotometrics-3.3.2/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics/search.py` & `resotometrics-3.3.2/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.3.2/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.3.1
+Version: 3.3.2
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.3.1/setup.py` & `resotometrics-3.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.1/test/test_args.py` & `resotometrics-3.3.2/test/test_args.py`

 * *Files identical despite different names*

