# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.872.tar", last modified: Thu Apr 13 01:08:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.873.tar", last modified: Fri Apr 14 01:02:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.872.tar` & `tencentcloud-sdk-python-vrs-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)     5710 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15237 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 01:08:59.000000 tencentcloud-sdk-python-vrs-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15482 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 01:02:20.000000 tencentcloud-sdk-python-vrs-3.0.873/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/README.rst` & `tencentcloud-sdk-python-vrs-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/vrs/v20200824/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,27 +420,35 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Words(AbstractModel):
-    """Words
+    """音频检测提示信息：
+    1.检测字是否存在多读、 少读、 错读等
+    2.检测准确度和流畅度
 
     """
 
     def __init__(self):
         r"""
-        :param PronAccuracy: 准确度
+        :param PronAccuracy: 准确度 (<75则认为不合格)
 注意：此字段可能返回 null，表示取不到有效值。
         :type PronAccuracy: float
-        :param PronFluency: 流畅度
+        :param PronFluency: 流畅度 (<0.95则认为不合格)
 注意：此字段可能返回 null，表示取不到有效值。
         :type PronFluency: float
-        :param Tag: tag: 0: match, 1: insert, 2: delete, 3: replace, 4: oov, 5: unknown
+        :param Tag: tag: 
+0: match  匹配
+1: insert   多读
+2: delete  少读
+3: replace 错读
+4: oov  待评估字不在发音评估的词库
+5: unknown 未知错误
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tag: int
         :param Word: 字
 注意：此字段可能返回 null，表示取不到有效值。
         :type Word: str
         """
         self.PronAccuracy = None
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.873/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.873/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.872/setup.py` & `tencentcloud-sdk-python-vrs-3.0.873/setup.py`

 * *Files identical despite different names*

