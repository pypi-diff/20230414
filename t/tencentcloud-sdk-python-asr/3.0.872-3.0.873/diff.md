# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.872.tar", last modified: Thu Apr 13 00:20:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.873.tar", last modified: Fri Apr 14 00:18:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.872.tar` & `tencentcloud-sdk-python-asr-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    23847 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62089 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:20:08.000000 tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    23847 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62143 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:18:53.000000 tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-asr-3.0.872/README.rst` & `tencentcloud-sdk-python-asr-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.872/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.873/tencentcloud/asr/v20190614/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -973,15 +973,21 @@
         :type DictName: str
         :param ModelId: 模型Id
         :type ModelId: str
         :param ModelType: 模型类型，“8k”或者”16k“
         :type ModelType: str
         :param ServiceType: 服务类型
         :type ServiceType: str
-        :param ModelState: 模型状态，-1下线状态，1上线状态, 0训练中, -2 训练失败
+        :param ModelState: 模型状态：
+-2：模型训练失败；
+-1：已下线；
+0：训练中；
+1：已上线；
+3：上线中；
+4：下线中；
         :type ModelState: int
         :param AtUpdated: 最后更新时间
         :type AtUpdated: str
         :param TagInfos: 标签信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type TagInfos: list of str
         """
```

### Comparing `tencentcloud-sdk-python-asr-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.873/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.872/setup.py` & `tencentcloud-sdk-python-asr-3.0.873/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.872/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.873/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

