# Comparing `tmp/resoto-plugin-scarf-3.3.1.tar.gz` & `tmp/resoto-plugin-scarf-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-scarf-3.3.1.tar", last modified: Fri Mar 31 23:53:10 2023, max compression
+gzip compressed data, was "resoto-plugin-scarf-3.3.2.tar", last modified: Fri Apr 14 16:11:39 2023, max compression
```

## Comparing `resoto-plugin-scarf-3.3.1.tar` & `resoto-plugin-scarf-3.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:10.177005 resoto-plugin-scarf-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-31 23:53:10.177005 resoto-plugin-scarf-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:10.173005 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:10.177005 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 23:53:10.000000 resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:53:10.177005 resoto-plugin-scarf-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:53:10.177005 resoto-plugin-scarf-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-31 23:51:14.000000 resoto-plugin-scarf-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:39.718371 resoto-plugin-scarf-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 16:11:39.718371 resoto-plugin-scarf-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:39.714371 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:39.718371 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 16:11:39.000000 resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:11:39.718371 resoto-plugin-scarf-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:39.718371 resoto-plugin-scarf-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 16:09:58.000000 resoto-plugin-scarf-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-scarf-3.3.1/PKG-INFO` & `resoto-plugin-scarf-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Scarf Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/scarf
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-scarf-3.3.1/README.md` & `resoto-plugin-scarf-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/__init__.py` & `resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/resources.py` & `resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.3.1/resoto_plugin_scarf/scarf.py` & `resoto-plugin-scarf-3.3.2/resoto_plugin_scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.3.1/resoto_plugin_scarf.egg-info/PKG-INFO` & `resoto-plugin-scarf-3.3.2/resoto_plugin_scarf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto Scarf Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/scarf
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-scarf-3.3.1/setup.py` & `resoto-plugin-scarf-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-scarf",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto Scarf Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["scarf = resoto_plugin_scarf:ScarfCollectorPlugin"]},
     include_package_data=True,
```

