# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.872.tar", last modified: Thu Apr 13 01:07:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.873.tar", last modified: Fri Apr 14 01:00:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.872.tar` & `tencentcloud-sdk-python-trtc-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198775 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58128 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 01:07:45.000000 tencentcloud-sdk-python-trtc-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198930 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58128 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 01:00:34.000000 tencentcloud-sdk-python-trtc-3.0.873/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/README.rst` & `tencentcloud-sdk-python-trtc-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1569,21 +1569,25 @@
 class DescribeTrtcRoomUsageResponse(AbstractModel):
     """DescribeTrtcRoomUsage返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param Data: 房间维度用量数据，csv文件格式。
+        :type Data: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self.Data = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.Data = params.get("Data")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeTrtcUsageRequest(AbstractModel):
     """DescribeTrtcUsage请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.873/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.873/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.872/setup.py` & `tencentcloud-sdk-python-trtc-3.0.873/setup.py`

 * *Files identical despite different names*

