# Comparing `tmp/resoto-plugin-posthog-3.3.1.tar.gz` & `tmp/resoto-plugin-posthog-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.3.1.tar", last modified: Fri Mar 31 23:52:52 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.3.2.tar", last modified: Fri Apr 14 16:13:54 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.3.1.tar` & `resoto-plugin-posthog-3.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:52.794623 resoto-plugin-posthog-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-31 23:52:52.794623 resoto-plugin-posthog-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:52.790623 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:52.794623 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 23:52:52.000000 resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:52:52.794623 resoto-plugin-posthog-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:52.794623 resoto-plugin-posthog-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 23:51:11.000000 resoto-plugin-posthog-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:54.026393 resoto-plugin-posthog-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 16:13:54.026393 resoto-plugin-posthog-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:54.026393 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:54.026393 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 16:13:54.000000 resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:13:54.030393 resoto-plugin-posthog-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:54.026393 resoto-plugin-posthog-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 16:12:14.000000 resoto-plugin-posthog-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.3.1/PKG-INFO` & `resoto-plugin-posthog-3.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.3.1/README.md` & `resoto-plugin-posthog-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.1/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.3.2/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.3.1/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.3.2/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.1/setup.py` & `resoto-plugin-posthog-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-posthog",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto Posthog Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["posthog = resoto_plugin_posthog:PosthogCollectorPlugin"]},
     include_package_data=True,
```

