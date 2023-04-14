# Comparing `tmp/resoto-plugin-dockerhub-3.3.1.tar.gz` & `tmp/resoto-plugin-dockerhub-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-dockerhub-3.3.1.tar", last modified: Fri Mar 31 23:52:50 2023, max compression
+gzip compressed data, was "resoto-plugin-dockerhub-3.3.2.tar", last modified: Fri Apr 14 16:16:47 2023, max compression
```

## Comparing `resoto-plugin-dockerhub-3.3.1.tar` & `resoto-plugin-dockerhub-3.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:50.986235 resoto-plugin-dockerhub-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-31 23:52:50.986235 resoto-plugin-dockerhub-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:50.982235 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:50.986235 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 23:52:50.000000 resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:52:50.986235 resoto-plugin-dockerhub-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:50.986235 resoto-plugin-dockerhub-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-31 23:51:10.000000 resoto-plugin-dockerhub-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 16:16:47.000000 resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:47.764952 resoto-plugin-dockerhub-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 16:15:06.000000 resoto-plugin-dockerhub-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-dockerhub-3.3.1/PKG-INFO` & `resoto-plugin-dockerhub-3.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Docker Hub Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-dockerhub-3.3.1/README.md` & `resoto-plugin-dockerhub-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/__init__.py` & `resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub/resources.py` & `resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/PKG-INFO` & `resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Docker Hub Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-dockerhub-3.3.1/resoto_plugin_dockerhub.egg-info/SOURCES.txt` & `resoto-plugin-dockerhub-3.3.2/resoto_plugin_dockerhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.3.1/setup.py` & `resoto-plugin-dockerhub-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-dockerhub",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto Docker Hub Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["dockerhub = resoto_plugin_dockerhub:DockerHubCollectorPlugin"]},
     include_package_data=True,
```

