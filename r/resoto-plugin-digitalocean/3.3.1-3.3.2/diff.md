# Comparing `tmp/resoto-plugin-digitalocean-3.3.1.tar.gz` & `tmp/resoto-plugin-digitalocean-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.3.1.tar", last modified: Fri Mar 31 23:54:16 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.3.2.tar", last modified: Fri Apr 14 16:15:40 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.3.1.tar` & `resoto-plugin-digitalocean-3.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:16.263278 resoto-plugin-digitalocean-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-31 23:54:16.263278 resoto-plugin-digitalocean-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:16.259278 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:16.259278 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-31 23:54:16.000000 resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 23:54:16.267278 resoto-plugin-digitalocean-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:16.259278 resoto-plugin-digitalocean-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:54:16.263278 resoto-plugin-digitalocean-3.3.1/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-31 23:51:13.000000 resoto-plugin-digitalocean-3.3.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:40.287186 resoto-plugin-digitalocean-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-14 16:15:40.287186 resoto-plugin-digitalocean-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:40.279186 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:40.279186 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:15:40.000000 resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:15:40.287186 resoto-plugin-digitalocean-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:40.279186 resoto-plugin-digitalocean-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:40.287186 resoto-plugin-digitalocean-3.3.2/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 16:12:22.000000 resoto-plugin-digitalocean-3.3.2/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.3.1/PKG-INFO` & `resoto-plugin-digitalocean-3.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto DigitalOcean Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto DigitalOcean Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.3.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.3.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/setup.py` & `resoto-plugin-digitalocean-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-digitalocean",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto DigitalOcean Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": ["digitalocean_collector = resoto_plugin_digitalocean:DigitalOceanCollectorPlugin"]
```

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.3.2/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.3.1/test/test_collector.py` & `resoto-plugin-digitalocean-3.3.2/test/test_collector.py`

 * *Files identical despite different names*

