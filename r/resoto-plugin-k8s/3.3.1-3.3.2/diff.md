# Comparing `tmp/resoto-plugin-k8s-3.3.1.tar.gz` & `tmp/resoto-plugin-k8s-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.3.1.tar", last modified: Fri Mar 31 23:54:22 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.3.2.tar", last modified: Fri Apr 14 16:16:44 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.3.1.tar` & `resoto-plugin-k8s-3.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:22.036877 resoto-plugin-k8s-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-31 23:54:22.036877 resoto-plugin-k8s-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:22.036877 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   104090 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:22.036877 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-31 23:54:22.000000 resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 23:54:22.036877 resoto-plugin-k8s-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-31 23:51:12.000000 resoto-plugin-k8s-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:44.356037 resoto-plugin-k8s-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-14 16:16:44.356037 resoto-plugin-k8s-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:44.356037 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104090 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:16:44.356037 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:16:44.000000 resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 16:16:44.356037 resoto-plugin-k8s-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-14 16:14:07.000000 resoto-plugin-k8s-3.3.2/setup.py
```

### Comparing `resoto-plugin-k8s-3.3.1/PKG-INFO` & `resoto-plugin-k8s-3.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Kubernetes Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.3.1/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.3.2/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.3.1/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.3.2/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Kubernetes Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.3.1/setup.py` & `resoto-plugin-k8s-3.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-k8s",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto Kubernetes Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["k8s_collector = resoto_plugin_k8s:KubernetesCollectorPlugin"]},
     include_package_data=True,
```

