# Comparing `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.3.1.tar.gz` & `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.3.1.tar", last modified: Fri Mar 31 23:53:22 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.3.2.tar", last modified: Fri Apr 14 16:13:29 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1.tar` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 23:53:22.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:22.182593 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-31 23:51:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:29.620683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-14 16:13:29.620683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:29.612683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:29.620683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 16:13:29.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:13:29.620683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:29.620683 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-14 16:11:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.3.1
+Version: 3.3.2
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/README.md` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers/config.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.3.1
+Version: 3.3.2
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.1/setup.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-aws-loadbalancers",
-    version="3.3.1",
+    version="3.3.2",
     description="AWS Loadbalancers Cleaner Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": [
```

