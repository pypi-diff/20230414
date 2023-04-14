# Comparing `tmp/resoto-plugin-onprem-3.3.1.tar.gz` & `tmp/resoto-plugin-onprem-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onprem-3.3.1.tar", last modified: Fri Mar 31 23:52:54 2023, max compression
+gzip compressed data, was "resoto-plugin-onprem-3.3.2.tar", last modified: Fri Apr 14 16:15:23 2023, max compression
```

## Comparing `resoto-plugin-onprem-3.3.1.tar` & `resoto-plugin-onprem-3.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-31 23:52:54.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 23:52:53.000000 resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:52:54.004147 resoto-plugin-onprem-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-31 23:51:09.000000 resoto-plugin-onprem-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 16:15:23.000000 resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:23.384924 resoto-plugin-onprem-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-14 16:13:16.000000 resoto-plugin-onprem-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-onprem-3.3.1/PKG-INFO` & `resoto-plugin-onprem-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto On-Premises Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onprem
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/__init__.py` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/config.py` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/resources.py` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem/ssh.py` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/PKG-INFO` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto On-Premises Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onprem
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.3.1/resoto_plugin_onprem.egg-info/SOURCES.txt` & `resoto-plugin-onprem-3.3.2/resoto_plugin_onprem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.3.1/setup.py` & `resoto-plugin-onprem-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-onprem",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto On-Premises Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["onprem = resoto_plugin_onprem:OnpremCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-onprem-3.3.1/test/test_config.py` & `resoto-plugin-onprem-3.3.2/test/test_config.py`

 * *Files identical despite different names*

