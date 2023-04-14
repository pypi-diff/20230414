# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.872.tar", last modified: Thu Apr 13 00:54:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.873.tar", last modified: Fri Apr 14 00:50:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.872.tar` & `tencentcloud-sdk-python-redis-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86576 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   288285 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86576 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   288654 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:50:03.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:50:01.000000 tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.872/README.rst` & `tencentcloud-sdk-python-redis-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.873/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6600,15 +6600,16 @@
 - 3：CKV 3.2内存版（标准架构）。
 - 4：CKV 3.2内存版（集群架构）。
 - 5：Redis 2.8内存版（单机）。
 - 6：Redis 4.0内存版（标准架构）。
 - 7：Redis 4.0内存版（集群架构）。
 - 8：Redis 5.0内存版（标准架构）。
 - 9：Redis 5.0内存版（集群架构）。
-
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type ProductType: int
         """
         self.TemplateId = None
         self.Name = None
         self.Description = None
         self.ProductType = None
 
@@ -6691,39 +6692,55 @@
 class ProductConf(AbstractModel):
     """产品信息
 
     """
 
     def __init__(self):
         r"""
-        :param Type: 产品类型，2 – Redis2.8内存版(标准架构)，3 – CKV 3.2内存版(标准架构)，4 – CKV 3.2内存版(集群架构)，5 – Redis2.8内存版(单机版)，6 – Redis4.0内存版(标准架构)，7 – Redis4.0内存版(集群架构)，8 – Redis5.0内存版(标准架构)，9 – Redis5.0内存版(集群架构)，10 – Redis4.0混合存储版Tendis
+        :param Type: 产品类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type Type: int
-        :param TypeName: 产品名称，Redis主从版，CKV主从版，CKV集群版，Redis单机版，Redis集群版，混合存储版Tendis
+        :param TypeName: 产品名称。包括：Redis 主从版、CKV 主从版、CKV 集群版、Redis 单机版、Redis 集群版。
         :type TypeName: str
-        :param MinBuyNum: 购买时的最小数量
+        :param MinBuyNum: 购买时的最小数量。
         :type MinBuyNum: int
-        :param MaxBuyNum: 购买时的最大数量
+        :param MaxBuyNum: 购买时的最大数量。
         :type MaxBuyNum: int
-        :param Saleout: 产品是否售罄
+        :param Saleout: 产品是否售罄。
+- true：售罄。
+- false：未售罄。
         :type Saleout: bool
-        :param Engine: 产品引擎，腾讯云CKV或者社区版Redis
+        :param Engine: 产品引擎。包括：腾讯云 CKV与社区版 Redis。
         :type Engine: str
-        :param Version: 兼容版本，Redis-2.8，Redis-3.2，Redis-4.0
+        :param Version: 兼容版本。包括：Redis-2.8、Redis-3.2、Redis-4.0、Redis-5.0、Redis-6.2。
         :type Version: str
-        :param TotalSize: 规格总大小，单位G
+        :param TotalSize: 规格总大小，单位GB。
         :type TotalSize: list of str
-        :param ShardSize: 每个分片大小，单位G
+        :param ShardSize: 每个分片大小，单位GB。
         :type ShardSize: list of str
-        :param ReplicaNum: 副本数量
+        :param ReplicaNum: 副本数量。
         :type ReplicaNum: list of str
-        :param ShardNum: 分片数量
+        :param ShardNum: 分片数量。
         :type ShardNum: list of str
-        :param PayMode: 支持的计费模式，1-包年包月，0-按量计费
+        :param PayMode: 支持的计费模式。
+- 1：包年包月。
+- 0：按量计费。
         :type PayMode: str
-        :param EnableRepicaReadOnly: 是否支持副本只读
+        :param EnableRepicaReadOnly: 是否支持副本只读。
+- true：支持副本只读。
+- false：不支持。
         :type EnableRepicaReadOnly: bool
         """
         self.Type = None
         self.TypeName = None
         self.MinBuyNum = None
         self.MaxBuyNum = None
         self.Saleout = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.873/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.872'
+__version__ = '3.0.873'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.873/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.872/setup.py` & `tencentcloud-sdk-python-redis-3.0.873/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.873/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

