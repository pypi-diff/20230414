# Comparing `tmp/tencentcloud-sdk-python-iai-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-iai-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.872.tar", last modified: Thu Apr 13 00:42:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.873.tar", last modified: Fri Apr 14 00:38:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iai-3.0.872.tar` & `tencentcloud-sdk-python-iai-3.0.873.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/
--rw-r--r--   0 root         (0) root         (0)    49376 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/iai_client.py
--rw-r--r--   0 root         (0) root         (0)    12105 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175621 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/
--rw-r--r--   0 root         (0) root         (0)    46159 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/iai_client.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164095 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:42:56.000000 tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/
+-rw-r--r--   0 root         (0) root         (0)    49376 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)    12105 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175621 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    46159 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164095 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:38:50.000000 tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iai-3.0.872/README.rst` & `tencentcloud-sdk-python-iai-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20200303/models.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20200303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/iai/v20180301/models.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/iai/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iai-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.873/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.872/setup.py` & `tencentcloud-sdk-python-iai-3.0.873/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.872/tencentcloud_sdk_python_iai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.873/tencentcloud_sdk_python_iai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

