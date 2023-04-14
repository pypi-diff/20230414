# Comparing `tmp/resoto-plugin-gcp-3.3.1.tar.gz` & `tmp/resoto-plugin-gcp-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.3.1.tar", last modified: Fri Mar 31 23:55:17 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.3.2.tar", last modified: Fri Apr 14 16:15:02 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.3.1.tar` & `resoto-plugin-gcp-3.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:55:17.438280 resoto-plugin-gcp-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-31 23:55:17.438280 resoto-plugin-gcp-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:55:17.434280 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/gcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/gcp_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/project_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:55:17.434280 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   276212 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    41166 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:55:17.434280 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-31 23:55:17.000000 resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-31 23:55:17.438280 resoto-plugin-gcp-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:55:17.438280 resoto-plugin-gcp-3.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_project_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-31 23:51:15.000000 resoto-plugin-gcp-3.3.1/test/test_sqladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.798521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/project_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   278397 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41166 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.798521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_project_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_sqladmin.py
```

### Comparing `resoto-plugin-gcp-3.3.1/PKG-INFO` & `resoto-plugin-gcp-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/gcp_resources.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/project_collector.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -763,14 +763,66 @@
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "default_disk_size_gb": S("defaultDiskSizeGb"),
         "valid_disk_size": S("validDiskSize"),
     }
     default_disk_size_gb: Optional[str] = field(default=None)
     valid_disk_size: Optional[str] = field(default=None)
 
+    resource_group_map: ClassVar[Dict[str, str]] = {
+        "local-ssd": "LocalSSD",
+        "pd-balanced": "SSD",
+        "pd-ssd": "SSD",
+        "pd-standard": "PDStandard",
+    }
+
+    def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
+        """Adds edges from disk_types type to SKUs and determines ondemand pricing"""
+        if not self.name:
+            return
+
+        log.debug((f"Looking up pricing for {self.rtdname} in {self.region().rtdname}"))
+        resource_group = self.resource_group_map.get(self.name)
+
+        def sku_filter(sku: GcpSku) -> bool:
+            if not self.name:
+                return False
+            if not sku.description or not sku.category or not sku.geo_taxonomy:
+                return False
+            if self.region().name not in sku.geo_taxonomy.regions:
+                return False
+
+            if sku.category.resource_family != "Storage" or sku.category.usage_type != "OnDemand":
+                return False
+            if not sku.category.resource_group == resource_group:
+                return False
+
+            if self.name == "pd-balanced" and not sku.description.startswith("Balanced"):
+                return False
+            if self.name != "pd-balanced" and sku.description.startswith("Balanced"):
+                return False
+            if self.zone().name != "undefined" and sku.description.startswith("Regional"):
+                # Zonal (i.e. not regional?) disk_type but regional SKU
+                return False
+            if (
+                # Zonal disk_type, but regional SKU and ALSO
+                # not of type pd-balanced
+                self.zone().name == "undefined"
+                and not sku.description.startswith("Regional")
+                and self.name != "pd-balanced"
+            ):
+                return False
+            return True
+
+        skus = builder.nodes(GcpSku, filter=sku_filter)
+        if len(skus) == 1 and skus[0].usage_unit_nanos:
+            builder.add_edge(self, reverse=True, node=skus[0])
+            self.ondemand_cost = skus[0].usage_unit_nanos / 1000000000
+        else:
+            log.debug(f"Unable to determine SKU for {self.rtdname}")
+
 
 @define(eq=False, slots=False)
 class GcpCustomerEncryptionKey:
     kind: ClassVar[str] = "gcp_customer_encryption_key"
     mapping: ClassVar[Dict[str, Bender]] = {
         "kms_key_name": S("kmsKeyName"),
         "kms_key_service_account": S("kmsKeyServiceAccount"),
```

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.3.1
+Version: 3.3.2
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.3.1/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/setup.py` & `resoto-plugin-gcp-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-gcp",
-    version="3.3.1",
+    version="3.3.2",
     description="Resoto GCP Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["gcp = resoto_plugin_gcp:GCPCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-gcp-3.3.1/test/conftest.py` & `resoto-plugin-gcp-3.3.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/random_client.py` & `resoto-plugin-gcp-3.3.2/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/test_base.py` & `resoto-plugin-gcp-3.3.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/test_billing.py` & `resoto-plugin-gcp-3.3.2/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/test_compute.py` & `resoto-plugin-gcp-3.3.2/test/test_compute.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,37 @@
     assert len(random_builder.edges_of(GcpNetwork, GcpBackendService)) == 1
 
 
 def test_gcp_disk_type(random_builder: GraphBuilder) -> None:
     roundtrip(GcpDiskType, random_builder)
 
 
+def test_disk_type_ondemand_cost(random_builder: GraphBuilder) -> None:
+    known_prices_per_gig = [
+        ("pd-standard", "us-east1", 0.08),
+    ]
+    with open(os.path.dirname(__file__) + "/files/skus.json") as f:
+        GcpSku.collect(raw=json.load(f)["skus"], builder=random_builder)
+
+    with open(os.path.dirname(__file__) + "/files/disk_type.json") as f:
+        GcpDiskType.collect(raw=json.load(f)["items"]["diskTypes"], builder=random_builder)
+
+    regions = random_builder.resources_of(GcpRegion)
+    disk_types = random_builder.resources_of(GcpDiskType)
+
+    for price in known_prices_per_gig:
+        region = next((obj for obj in regions if obj.id == price[1]), None)
+        disk_type = next((obj for obj in disk_types if obj.name == price[0]), None)
+        assert disk_type
+        disk_type._region = region
+        disk_type.connect_in_graph(random_builder, {"Dummy": "Source"})
+        assert disk_type.ondemand_cost > 0.0
+        assert round(disk_type.ondemand_cost, 5) == price[2]
+
+
 def test_gcp_disk(random_builder: GraphBuilder) -> None:
     disk = roundtrip(GcpDisk, random_builder)
     connect_resource(random_builder, disk, GcpDiskType, selfLink=disk.volume_type)
     assert len(random_builder.edges_of(GcpDiskType, GcpDisk)) == 1
 
 
 def test_gcp_external_vpn_gateway(random_builder: GraphBuilder) -> None:
```

### Comparing `resoto-plugin-gcp-3.3.1/test/test_config.py` & `resoto-plugin-gcp-3.3.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/test_container.py` & `resoto-plugin-gcp-3.3.2/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.1/test/test_project_collector.py` & `resoto-plugin-gcp-3.3.2/test/test_project_collector.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,14 @@
     with open(os.path.dirname(__file__) + "/files/machine_type.json") as f:
         GcpMachineType.collect(raw=json.load(f)["items"]["machineTypes"], builder=random_builder)
     with open(os.path.dirname(__file__) + "/files/skus.json") as f:
         GcpSku.collect(raw=json.load(f)["skus"], builder=random_builder)
 
     collector = collector_with_graph(random_builder.graph)
 
-    assert len(list(collector.graph.nodes("kind", "gcp_machine_type"))) == 28
-    assert len(list(collector.graph.nodes("kind", "gcp_sku"))) == 28
+    num_all_machine_types = len(list(collector.graph.search("kind", "gcp_machine_type")))
+    num_all_skus = len(list(collector.graph.search("kind", "gcp_sku")))
 
     collector.remove_unconnected_nodes()
 
-    assert len(list(collector.graph.nodes("kind", "gcp_machine_type"))) == 7
-    assert len(list(collector.graph.nodes("kind", "gcp_sku"))) == 7
+    assert len(list(collector.graph.search("kind", "gcp_machine_type"))) < num_all_machine_types
+    assert len(list(collector.graph.search("kind", "gcp_sku"))) < num_all_skus
```

### Comparing `resoto-plugin-gcp-3.3.1/test/test_sqladmin.py` & `resoto-plugin-gcp-3.3.2/test/test_sqladmin.py`

 * *Files identical despite different names*

