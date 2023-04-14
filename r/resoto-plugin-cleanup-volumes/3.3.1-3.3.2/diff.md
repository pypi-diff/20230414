# Comparing `tmp/resoto-plugin-cleanup-volumes-3.3.1.tar.gz` & `tmp/resoto-plugin-cleanup-volumes-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-volumes-3.3.1.tar", last modified: Fri Mar 31 23:52:55 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-volumes-3.3.2.tar", last modified: Fri Apr 14 16:12:21 2023, max compression
```

## Comparing `resoto-plugin-cleanup-volumes-3.3.1.tar` & `resoto-plugin-cleanup-volumes-3.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-31 23:52:55.000000 resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:55.982403 resoto-plugin-cleanup-volumes-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-31 23:51:15.000000 resoto-plugin-cleanup-volumes-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:21.526658 resoto-plugin-cleanup-volumes-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 16:12:21.526658 resoto-plugin-cleanup-volumes-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:21.522658 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:21.526658 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 16:12:21.000000 resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:12:21.526658 resoto-plugin-cleanup-volumes-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:21.526658 resoto-plugin-cleanup-volumes-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-14 16:10:40.000000 resoto-plugin-cleanup-volumes-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.3.1
+Version: 3.3.2
 Summary: Volume Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/README.md` & `resoto-plugin-cleanup-volumes-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes/__init__.py` & `resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes/config.py` & `resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.3.1
+Version: 3.3.2
 Summary: Volume Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-volumes-3.3.2/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.3.1/setup.py` & `resoto-plugin-cleanup-volumes-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-volumes",
-    version="3.3.1",
+    version="3.3.2",
     description="Volume Cleaner Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["cleanup_volumes = resoto_plugin_cleanup_volumes:CleanupVolumesPlugin"]},
     include_package_data=True,
```

