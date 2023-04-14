# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.871.tar", last modified: Wed Apr 12 00:29:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.873.tar", last modified: Fri Apr 14 00:44:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.871.tar` & `tencentcloud-sdk-python-mariadb-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)    69766 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)   213570 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14808 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-12 00:29:26.000000 tencentcloud-sdk-python-mariadb-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:29:27.000000 tencentcloud-sdk-python-mariadb-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    69766 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14808 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213570 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:44:10.000000 tencentcloud-sdk-python-mariadb-3.0.873/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.871
+Version: 3.0.873
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.873/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.871'
+__version__ = '3.0.873'
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.873/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.871
+Version: 3.0.873
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.871/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.873/setup.py`

 * *Files identical despite different names*

