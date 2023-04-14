# Comparing `tmp/nops_metadata-0.4.8.tar.gz` & `tmp/nops_metadata-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nops_metadata-0.4.8.tar", max compression
+gzip compressed data, was "nops_metadata-0.4.9.tar", max compression
```

## Comparing `nops_metadata-0.4.8.tar` & `nops_metadata-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5729 2023-03-17 10:53:13.196169 nops_metadata-0.4.8/nops_metadata/__init__.py
--rw-r--r--   0        0        0    17720 2023-03-17 10:53:13.200169 nops_metadata-0.4.8/nops_metadata/constants.py
--rw-r--r--   0        0        0     4456 2023-03-17 10:53:13.200169 nops_metadata-0.4.8/nops_metadata/schema.py
--rw-r--r--   0        0        0     6144 2023-01-05 14:54:37.229865 nops_metadata-0.4.8/nops_metadata/spark_schema.py
--rw-r--r--   0        0        0        0 2023-01-05 14:54:37.229865 nops_metadata-0.4.8/nops_metadata/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-01-05 14:54:37.229865 nops_metadata-0.4.8/nops_metadata/tests/conftest.py
--rw-r--r--   0        0        0     5085 2023-03-17 10:53:13.200169 nops_metadata-0.4.8/nops_metadata/tests/test_fetcher.py
--rw-r--r--   0        0        0     1577 2023-03-17 10:53:13.200169 nops_metadata-0.4.8/nops_metadata/tests/test_schema.py
--rw-r--r--   0        0        0     2905 2023-01-05 14:54:37.229865 nops_metadata-0.4.8/nops_metadata/utils.py
--rw-r--r--   0        0        0      766 2023-03-17 10:53:13.200169 nops_metadata-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 nops_metadata-0.4.8/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nops_metadata-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     5729 2023-03-17 10:53:13.196169 nops_metadata-0.4.9/nops_metadata/__init__.py
+-rw-r--r--   0        0        0    17817 2023-04-14 12:15:05.575133 nops_metadata-0.4.9/nops_metadata/constants.py
+-rw-r--r--   0        0        0     4456 2023-03-17 10:53:13.200169 nops_metadata-0.4.9/nops_metadata/schema.py
+-rw-r--r--   0        0        0     6144 2023-01-05 14:54:37.229865 nops_metadata-0.4.9/nops_metadata/spark_schema.py
+-rw-r--r--   0        0        0        0 2023-01-05 14:54:37.229865 nops_metadata-0.4.9/nops_metadata/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-01-05 14:54:37.229865 nops_metadata-0.4.9/nops_metadata/tests/conftest.py
+-rw-r--r--   0        0        0     5085 2023-03-17 10:53:13.200169 nops_metadata-0.4.9/nops_metadata/tests/test_fetcher.py
+-rw-r--r--   0        0        0     1577 2023-03-17 10:53:13.200169 nops_metadata-0.4.9/nops_metadata/tests/test_schema.py
+-rw-r--r--   0        0        0     2905 2023-01-05 14:54:37.229865 nops_metadata-0.4.9/nops_metadata/utils.py
+-rw-r--r--   0        0        0      766 2023-04-14 12:14:18.873135 nops_metadata-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 nops_metadata-0.4.9/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nops_metadata-0.4.9/PKG-INFO
```

### Comparing `nops_metadata-0.4.8/nops_metadata/__init__.py` & `nops_metadata-0.4.9/nops_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/nops_metadata/constants.py` & `nops_metadata-0.4.9/nops_metadata/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "ec2_snapshots": {"fetch_method": "describe_snapshots", "response_key": "Snapshots", "kwargs": {"OwnerIds": ["self"]}},
         "ec2_subnets": {"fetch_method": "describe_subnets", "response_key": "Subnets"},
         "ec2_volumes": {"fetch_method": "describe_volumes", "response_key": "Volumes"},
         "ec2_vpcs": {"fetch_method": "describe_vpcs", "response_key": "Vpcs"},
         "ecs_clusters": {"fetch_method": "list_clusters", "response_key": "clusterArns"},
         "efs_file_systems": {"fetch_method": "describe_file_systems", "response_key": "FileSystems"},
         "eks_clusters": {"fetch_method": "list_clusters", "response_key": "clusters"},
+        "eks_describe_cluster": {"fetch_method": "describe_cluster", "response_key": "cluster"},
         "eks_nodegroups_metadata": {"fetch_method": "describe_nodegroup", "response_key": "nodegroup"},
         "elasticache_cache_clusters": {"fetch_method": "describe_cache_clusters", "response_key": "CacheClusters"},
         "elasticache_replication_groups": {"fetch_method": "describe_replication_groups", "response_key": "ReplicationGroups"},
         "elasticache_cache_subnet_groups": {"fetch_method": "describe_cache_subnet_groups", "response_key": "CacheSubnetGroups"},
         "elbv2_load_balancers": {"fetch_method": "describe_load_balancers", "response_key": "LoadBalancers"},
         "elbv2_target_groups": {"fetch_method": "describe_target_groups", "response_key": "TargetGroups"},
         "iam_account_aliases": {"fetch_method": "list_account_aliases", "response_key": "AccountAliases"},
```

### Comparing `nops_metadata-0.4.8/nops_metadata/schema.py` & `nops_metadata-0.4.9/nops_metadata/schema.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/nops_metadata/spark_schema.py` & `nops_metadata-0.4.9/nops_metadata/spark_schema.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/nops_metadata/tests/test_fetcher.py` & `nops_metadata-0.4.9/nops_metadata/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/nops_metadata/tests/test_schema.py` & `nops_metadata-0.4.9/nops_metadata/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/nops_metadata/utils.py` & `nops_metadata-0.4.9/nops_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `nops_metadata-0.4.8/pyproject.toml` & `nops_metadata-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nops-metadata"
-version = "0.4.8"
+version = "0.4.9"
 description = "Metadata producer tooling used in nOps.io"
 authors = ["nOps Engineers <eng@nops.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 boto3 = ">=1.17.102"
 pyrsistent = ">=0.17.3"
```

### Comparing `nops_metadata-0.4.8/setup.py` & `nops_metadata-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3>=1.17.102',
  'pydantic>=1.8.0',
  'pyrsistent>=0.17.3',
  'pyspark[sql]==3.3.1']
 
 setup_kwargs = {
     'name': 'nops-metadata',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Metadata producer tooling used in nOps.io',
     'long_description': 'None',
     'author': 'nOps Engineers',
     'author_email': 'eng@nops.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nops_metadata-0.4.8/PKG-INFO` & `nops_metadata-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nops-metadata
-Version: 0.4.8
+Version: 0.4.9
 Summary: Metadata producer tooling used in nOps.io
 Author: nOps Engineers
 Author-email: eng@nops.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

