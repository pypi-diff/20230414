# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.872.tar", last modified: Thu Apr 13 01:02:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.873.tar", last modified: Fri Apr 14 00:54:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.872.tar` & `tencentcloud-sdk-python-teo-3.0.873.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)   468214 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)    87643 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    20875 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   504803 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    20875 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   504803 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:54:54.000000 tencentcloud-sdk-python-teo-3.0.873/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.872/README.rst` & `tencentcloud-sdk-python-teo-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/teo_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,190 +13,190 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.abstract_client import AbstractClient
-from tencentcloud.teo.v20220106 import models
+from tencentcloud.teo.v20220901 import models
 
 
 class TeoClient(AbstractClient):
-    _apiVersion = '2022-01-06'
+    _apiVersion = '2022-09-01'
     _endpoint = 'teo.tencentcloudapi.com'
     _service = 'teo'
 
 
-    def CheckCertificate(self, request):
-        """校验证书
+    def BindZoneToPlan(self, request):
+        """将未绑定套餐的站点绑定到已有套餐
 
-        :param request: Request instance for CheckCertificate.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CheckCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CheckCertificateResponse`
+        :param request: Request instance for BindZoneToPlan.
+        :type request: :class:`tencentcloud.teo.v20220901.models.BindZoneToPlanRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.BindZoneToPlanResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CheckCertificate", params, headers=headers)
+            body = self.call("BindZoneToPlan", params, headers=headers)
             response = json.loads(body)
-            model = models.CheckCertificateResponse()
+            model = models.BindZoneToPlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateApplicationProxy(self, request):
-        """创建应用代理
+    def CheckCertificate(self, request):
+        """校验证书
 
-        :param request: Request instance for CreateApplicationProxy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyResponse`
+        :param request: Request instance for CheckCertificate.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CheckCertificateRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CheckCertificateResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateApplicationProxy", params, headers=headers)
+            body = self.call("CheckCertificate", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateApplicationProxyResponse()
+            model = models.CheckCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateApplicationProxyRule(self, request):
-        """创建应用代理规则
+    def CreateAccelerationDomain(self, request):
+        """创建加速域名
 
-        :param request: Request instance for CreateApplicationProxyRule.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyRuleRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyRuleResponse`
+        :param request: Request instance for CreateAccelerationDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateAccelerationDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateAccelerationDomainResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateApplicationProxyRule", params, headers=headers)
+            body = self.call("CreateAccelerationDomain", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateApplicationProxyRuleResponse()
+            model = models.CreateAccelerationDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateApplicationProxyRules(self, request):
-        """批量创建应用代理规则
+    def CreateAliasDomain(self, request):
+        """创建别称域名。
 
-        :param request: Request instance for CreateApplicationProxyRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateApplicationProxyRulesResponse`
+        :param request: Request instance for CreateAliasDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateAliasDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateAliasDomainResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateApplicationProxyRules", params, headers=headers)
+            body = self.call("CreateAliasDomain", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateApplicationProxyRulesResponse()
+            model = models.CreateAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateCustomErrorPage(self, request):
-        """创建自定义规则的自定义页
+    def CreateApplicationProxy(self, request):
+        """创建应用代理
 
-        :param request: Request instance for CreateCustomErrorPage.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateCustomErrorPageRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateCustomErrorPageResponse`
+        :param request: Request instance for CreateApplicationProxy.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateCustomErrorPage", params, headers=headers)
+            body = self.call("CreateApplicationProxy", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateCustomErrorPageResponse()
+            model = models.CreateApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateDnsRecord(self, request):
-        """创建 DNS 记录
+    def CreateApplicationProxyRule(self, request):
+        """创建应用代理规则
 
-        :param request: Request instance for CreateDnsRecord.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateDnsRecordRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateDnsRecordResponse`
+        :param request: Request instance for CreateApplicationProxyRule.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyRuleRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateDnsRecord", params, headers=headers)
+            body = self.call("CreateApplicationProxyRule", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateDnsRecordResponse()
+            model = models.CreateApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateLoadBalancing(self, request):
-        """创建负载均衡
+    def CreateCredential(self, request):
+        """用于创建COS回源私有凭证
 
-        :param request: Request instance for CreateLoadBalancing.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateLoadBalancingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateLoadBalancingResponse`
+        :param request: Request instance for CreateCredential.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateCredentialRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateCredentialResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateLoadBalancing", params, headers=headers)
+            body = self.call("CreateCredential", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateLoadBalancingResponse()
+            model = models.CreateCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateOriginGroup(self, request):
-        """源站组创建
+        """创建源站组
 
         :param request: Request instance for CreateOriginGroup.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateOriginGroupRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateOriginGroupResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateOriginGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateOriginGroupResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateOriginGroup", params, headers=headers)
             response = json.loads(body)
@@ -210,16 +210,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePlanForZone(self, request):
         """为未购买套餐的站点购买套餐
 
         :param request: Request instance for CreatePlanForZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreatePlanForZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreatePlanForZoneResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreatePlanForZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreatePlanForZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreatePlanForZone", params, headers=headers)
             response = json.loads(body)
@@ -233,16 +233,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePrefetchTask(self, request):
         """创建预热任务
 
         :param request: Request instance for CreatePrefetchTask.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreatePrefetchTaskRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreatePrefetchTaskResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreatePrefetchTaskRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreatePrefetchTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreatePrefetchTask", params, headers=headers)
             response = json.loads(body)
@@ -256,16 +256,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePurgeTask(self, request):
         """创建清除缓存任务
 
         :param request: Request instance for CreatePurgeTask.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreatePurgeTaskRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreatePurgeTaskResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreatePurgeTaskRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreatePurgeTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreatePurgeTask", params, headers=headers)
             response = json.loads(body)
@@ -275,528 +275,503 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateRule(self, request):
-        """规则引擎创建规则。
-
-        :param request: Request instance for CreateRule.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateRuleRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateRuleResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateRule", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateRuleResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateZone(self, request):
-        """用于用户接入新的站点
+    def CreateReplayTask(self, request):
+        """创建刷新/预热重放任务
 
-        :param request: Request instance for CreateZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.CreateZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.CreateZoneResponse`
+        :param request: Request instance for CreateReplayTask.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateReplayTaskRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateReplayTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateZone", params, headers=headers)
+            body = self.call("CreateReplayTask", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateZoneResponse()
+            model = models.CreateReplayTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteApplicationProxy(self, request):
-        """删除应用代理
+    def CreateRule(self, request):
+        """规则引擎创建规则。
 
-        :param request: Request instance for DeleteApplicationProxy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteApplicationProxyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteApplicationProxyResponse`
+        :param request: Request instance for CreateRule.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateRuleRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteApplicationProxy", params, headers=headers)
+            body = self.call("CreateRule", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteApplicationProxyResponse()
+            model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteApplicationProxyRule(self, request):
-        """删除应用代理规则
+    def CreateSpeedTesting(self, request):
+        """对用户指定的域名进行一次站点拨测
 
-        :param request: Request instance for DeleteApplicationProxyRule.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteApplicationProxyRuleRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteApplicationProxyRuleResponse`
+        :param request: Request instance for CreateSpeedTesting.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteApplicationProxyRule", params, headers=headers)
+            body = self.call("CreateSpeedTesting", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteApplicationProxyRuleResponse()
+            model = models.CreateSpeedTestingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteDnsRecords(self, request):
-        """批量删除 DNS 记录
+    def CreateZone(self, request):
+        """用于用户接入新的站点。
 
-        :param request: Request instance for DeleteDnsRecords.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteDnsRecordsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteDnsRecordsResponse`
+        :param request: Request instance for CreateZone.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CreateZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteDnsRecords", params, headers=headers)
+            body = self.call("CreateZone", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteDnsRecordsResponse()
+            model = models.CreateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteLoadBalancing(self, request):
-        """删除负载均衡
+    def DeleteAccelerationDomains(self, request):
+        """批量删除加速域名
 
-        :param request: Request instance for DeleteLoadBalancing.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteLoadBalancingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteLoadBalancingResponse`
+        :param request: Request instance for DeleteAccelerationDomains.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteAccelerationDomainsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteAccelerationDomainsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteLoadBalancing", params, headers=headers)
+            body = self.call("DeleteAccelerationDomains", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteLoadBalancingResponse()
+            model = models.DeleteAccelerationDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteOriginGroup(self, request):
-        """源站组删除
+    def DeleteAliasDomain(self, request):
+        """删除别称域名。
 
-        :param request: Request instance for DeleteOriginGroup.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteOriginGroupRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteOriginGroupResponse`
+        :param request: Request instance for DeleteAliasDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteAliasDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteAliasDomainResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteOriginGroup", params, headers=headers)
+            body = self.call("DeleteAliasDomain", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteOriginGroupResponse()
+            model = models.DeleteAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteRules(self, request):
-        """批量删除规则引擎规则。
+    def DeleteApplicationProxy(self, request):
+        """删除应用代理
 
-        :param request: Request instance for DeleteRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteRulesResponse`
+        :param request: Request instance for DeleteApplicationProxy.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteRules", params, headers=headers)
+            body = self.call("DeleteApplicationProxy", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteRulesResponse()
+            model = models.DeleteApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteZone(self, request):
-        """删除站点
+    def DeleteApplicationProxyRule(self, request):
+        """删除应用代理规则
 
-        :param request: Request instance for DeleteZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DeleteZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DeleteZoneResponse`
+        :param request: Request instance for DeleteApplicationProxyRule.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyRuleRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteZone", params, headers=headers)
+            body = self.call("DeleteApplicationProxyRule", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteZoneResponse()
+            model = models.DeleteApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeApplicationProxy(self, request):
-        """获取应用代理列表
+    def DeleteOriginGroup(self, request):
+        """删除源站组
 
-        :param request: Request instance for DescribeApplicationProxy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeApplicationProxyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeApplicationProxyResponse`
+        :param request: Request instance for DeleteOriginGroup.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteOriginGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteOriginGroupResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeApplicationProxy", params, headers=headers)
+            body = self.call("DeleteOriginGroup", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeApplicationProxyResponse()
+            model = models.DeleteOriginGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeApplicationProxyDetail(self, request):
-        """获取应用代理详细信息
+    def DeleteRules(self, request):
+        """批量删除规则引擎规则。
 
-        :param request: Request instance for DescribeApplicationProxyDetail.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeApplicationProxyDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeApplicationProxyDetailResponse`
+        :param request: Request instance for DeleteRules.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteRulesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteRulesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeApplicationProxyDetail", params, headers=headers)
+            body = self.call("DeleteRules", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeApplicationProxyDetailResponse()
+            model = models.DeleteRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeAvailablePlans(self, request):
-        """查询当前账户可用套餐信息列表
+    def DeleteZone(self, request):
+        """删除站点。
 
-        :param request: Request instance for DescribeAvailablePlans.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeAvailablePlansRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeAvailablePlansResponse`
+        :param request: Request instance for DeleteZone.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DeleteZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DeleteZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAvailablePlans", params, headers=headers)
+            body = self.call("DeleteZone", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAvailablePlansResponse()
+            model = models.DeleteZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeBotLog(self, request):
-        """查询Bot攻击日志
+    def DescribeAccelerationDomains(self, request):
+        """查询加速域名列表，支持搜索、分页、排序、过滤。
 
-        :param request: Request instance for DescribeBotLog.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeBotLogRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeBotLogResponse`
+        :param request: Request instance for DescribeAccelerationDomains.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAccelerationDomainsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAccelerationDomainsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBotLog", params, headers=headers)
+            body = self.call("DescribeAccelerationDomains", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBotLogResponse()
+            model = models.DescribeAccelerationDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeBotManagedRules(self, request):
-        """分页查询Bot托管规则
+    def DescribeAddableEntityList(self, request):
+        """本接口（DescribeAddableEntityList）用于查询剩余可添加的日志推送实体列表。
 
-        :param request: Request instance for DescribeBotManagedRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeBotManagedRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeBotManagedRulesResponse`
+        :param request: Request instance for DescribeAddableEntityList.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAddableEntityListRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAddableEntityListResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBotManagedRules", params, headers=headers)
+            body = self.call("DescribeAddableEntityList", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBotManagedRulesResponse()
+            model = models.DescribeAddableEntityListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeCnameStatus(self, request):
-        """查询域名 CNAME 状态
+    def DescribeAliasDomains(self, request):
+        """查询别称域名信息列表。
 
-        :param request: Request instance for DescribeCnameStatus.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeCnameStatusRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeCnameStatusResponse`
+        :param request: Request instance for DescribeAliasDomains.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAliasDomainsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAliasDomainsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCnameStatus", params, headers=headers)
+            body = self.call("DescribeAliasDomains", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCnameStatusResponse()
+            model = models.DescribeAliasDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDoSPolicy(self, request):
-        """查询DDoS防护配置详情
+    def DescribeApplicationProxies(self, request):
+        """查询应用代理列表。
 
-        :param request: Request instance for DescribeDDoSPolicy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDoSPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDoSPolicyResponse`
+        :param request: Request instance for DescribeApplicationProxies.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeApplicationProxiesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeApplicationProxiesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDoSPolicy", params, headers=headers)
+            body = self.call("DescribeApplicationProxies", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDoSPolicyResponse()
+            model = models.DescribeApplicationProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosAttackData(self, request):
-        """查询DDos攻击时序数据
+    def DescribeAvailablePlans(self, request):
+        """查询当前账户可用套餐信息列表
 
-        :param request: Request instance for DescribeDDosAttackData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackDataResponse`
+        :param request: Request instance for DescribeAvailablePlans.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAvailablePlansRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAvailablePlansResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosAttackData", params, headers=headers)
+            body = self.call("DescribeAvailablePlans", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosAttackDataResponse()
+            model = models.DescribeAvailablePlansResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosAttackEvent(self, request):
-        """查询DDos攻击事件
+    def DescribeClientRuleList(self, request):
+        """本接口（DescribeClientRuleList）用于查询封禁客户端信息列表。
 
-        :param request: Request instance for DescribeDDosAttackEvent.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackEventRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackEventResponse`
+        :param request: Request instance for DescribeClientRuleList.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeClientRuleListRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeClientRuleListResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosAttackEvent", params, headers=headers)
+            body = self.call("DescribeClientRuleList", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosAttackEventResponse()
+            model = models.DescribeClientRuleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosAttackEventDetail(self, request):
-        """查询DDos攻击事件详情
+    def DescribeContentQuota(self, request):
+        """查询内容管理接口配额
 
-        :param request: Request instance for DescribeDDosAttackEventDetail.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackEventDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackEventDetailResponse`
+        :param request: Request instance for DescribeContentQuota.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeContentQuotaRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeContentQuotaResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosAttackEventDetail", params, headers=headers)
+            body = self.call("DescribeContentQuota", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosAttackEventDetailResponse()
+            model = models.DescribeContentQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosAttackSourceEvent(self, request):
-        """查询DDos攻击源信息
+    def DescribeDDoSAttackData(self, request):
+        """本接口（DescribeDDoSAttackData）用于查询DDoS攻击时序数据。
 
-        :param request: Request instance for DescribeDDosAttackSourceEvent.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackSourceEventRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackSourceEventResponse`
+        :param request: Request instance for DescribeDDoSAttackData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosAttackSourceEvent", params, headers=headers)
+            body = self.call("DescribeDDoSAttackData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosAttackSourceEventResponse()
+            model = models.DescribeDDoSAttackDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosAttackTopData(self, request):
-        """查询DDos攻击Top数据
+    def DescribeDDoSAttackEvent(self, request):
+        """本接口（DescribeDDoSAttackEvent）用于查询DDoS攻击事件列表。
 
-        :param request: Request instance for DescribeDDosAttackTopData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackTopDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosAttackTopDataResponse`
+        :param request: Request instance for DescribeDDoSAttackEvent.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackEventRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackEventResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosAttackTopData", params, headers=headers)
+            body = self.call("DescribeDDoSAttackEvent", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosAttackTopDataResponse()
+            model = models.DescribeDDoSAttackEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDDosMajorAttackEvent(self, request):
-        """此接口已经做不兼容变更，所以此版本的接口已经无法调用，故作下线处理
-
-        查询DDos主攻击事件
+    def DescribeDDoSAttackTopData(self, request):
+        """本接口（DescribeDDoSAttackTopData）用于查询DDoS攻击Top数据。
 
-        :param request: Request instance for DescribeDDosMajorAttackEvent.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDDosMajorAttackEventRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDDosMajorAttackEventResponse`
+        :param request: Request instance for DescribeDDoSAttackTopData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackTopDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackTopDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDDosMajorAttackEvent", params, headers=headers)
+            body = self.call("DescribeDDoSAttackTopData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDDosMajorAttackEventResponse()
+            model = models.DescribeDDoSAttackTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDefaultCertificates(self, request):
         """查询默认证书列表
 
         :param request: Request instance for DescribeDefaultCertificates.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDefaultCertificatesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDefaultCertificatesResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDefaultCertificatesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDefaultCertificatesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDefaultCertificates", params, headers=headers)
             response = json.loads(body)
@@ -810,16 +785,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDnsData(self, request):
         """获取DNS请求数统计曲线
 
         :param request: Request instance for DescribeDnsData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDnsDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDnsDataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDnsDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDnsDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDnsData", params, headers=headers)
             response = json.loads(body)
@@ -829,89 +804,20 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDnsRecords(self, request):
-        """查询 DNS 记录列表，支持搜索、分页、排序、过滤。
-
-        :param request: Request instance for DescribeDnsRecords.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDnsRecordsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDnsRecordsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDnsRecords", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDnsRecordsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDnssec(self, request):
-        """用于查询 DNSSEC 相关信息
-
-        :param request: Request instance for DescribeDnssec.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeDnssecRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeDnssecResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDnssec", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDnssecResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeHostsCertificate(self, request):
-        """查询域名证书列表，支持搜索、分页、排序、过滤。
-
-        :param request: Request instance for DescribeHostsCertificate.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeHostsCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeHostsCertificateResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeHostsCertificate", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeHostsCertificateResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeHostsSetting(self, request):
         """用于查询域名配置信息
 
         :param request: Request instance for DescribeHostsSetting.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeHostsSettingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeHostsSettingResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeHostsSettingRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeHostsSettingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeHostsSetting", params, headers=headers)
             response = json.loads(body)
@@ -921,89 +827,89 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeIdentification(self, request):
-        """查询验证结果
+    def DescribeIdentifications(self, request):
+        """查询站点的验证信息。
 
-        :param request: Request instance for DescribeIdentification.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeIdentificationRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeIdentificationResponse`
+        :param request: Request instance for DescribeIdentifications.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeIdentificationsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeIdentificationsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeIdentification", params, headers=headers)
+            body = self.call("DescribeIdentifications", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeIdentificationResponse()
+            model = models.DescribeIdentificationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeLoadBalancing(self, request):
-        """获取负载均衡列表
+    def DescribeLogSets(self, request):
+        """本接口（DescribeLogSets）用于获取日志集列表。
 
-        :param request: Request instance for DescribeLoadBalancing.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeLoadBalancingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeLoadBalancingResponse`
+        :param request: Request instance for DescribeLogSets.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeLogSetsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeLogSetsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeLoadBalancing", params, headers=headers)
+            body = self.call("DescribeLogSets", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeLoadBalancingResponse()
+            model = models.DescribeLogSetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeLoadBalancingDetail(self, request):
-        """获取负载均衡详细信息
+    def DescribeLogTopicTasks(self, request):
+        """本接口（DescribeLogTopicTasks）用于获取日志推送任务列表。
 
-        :param request: Request instance for DescribeLoadBalancingDetail.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeLoadBalancingDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeLoadBalancingDetailResponse`
+        :param request: Request instance for DescribeLogTopicTasks.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeLogTopicTasksRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeLogTopicTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeLoadBalancingDetail", params, headers=headers)
+            body = self.call("DescribeLogTopicTasks", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeLoadBalancingDetailResponse()
+            model = models.DescribeLogTopicTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeOriginGroup(self, request):
-        """获取源站组信息列表
+        """获取源站组列表
 
         :param request: Request instance for DescribeOriginGroup.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeOriginGroupRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeOriginGroupResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOriginGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeOriginGroupResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeOriginGroup", params, headers=headers)
             response = json.loads(body)
@@ -1013,45 +919,43 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeOriginGroupDetail(self, request):
-        """获取源站组详细信息
+    def DescribeOriginProtection(self, request):
+        """查询源站防护信息
 
-        :param request: Request instance for DescribeOriginGroupDetail.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeOriginGroupDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeOriginGroupDetailResponse`
+        :param request: Request instance for DescribeOriginProtection.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOriginProtectionRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeOriginProtectionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeOriginGroupDetail", params, headers=headers)
+            body = self.call("DescribeOriginProtection", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeOriginGroupDetailResponse()
+            model = models.DescribeOriginProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeOverviewL7Data(self, request):
-        """接口已经不兼容升级，故作下线处理
-
-        本接口（DescribeOverviewL7Data）用于查询七层监控类时序流量数据。
+        """本接口（DescribeOverviewL7Data）用于查询七层监控类时序流量数据。
 
         :param request: Request instance for DescribeOverviewL7Data.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeOverviewL7DataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeOverviewL7DataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOverviewL7DataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeOverviewL7DataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeOverviewL7Data", params, headers=headers)
             response = json.loads(body)
@@ -1065,16 +969,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribePrefetchTasks(self, request):
         """查询预热任务状态
 
         :param request: Request instance for DescribePrefetchTasks.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribePrefetchTasksRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribePrefetchTasksResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribePrefetchTasksRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribePrefetchTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribePrefetchTasks", params, headers=headers)
             response = json.loads(body)
@@ -1088,16 +992,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribePurgeTasks(self, request):
         """查询清除缓存历史记录
 
         :param request: Request instance for DescribePurgeTasks.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribePurgeTasksRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribePurgeTasksResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribePurgeTasksRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribePurgeTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribePurgeTasks", params, headers=headers)
             response = json.loads(body)
@@ -1111,16 +1015,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeRules(self, request):
         """查询规则引擎规则。
 
         :param request: Request instance for DescribeRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeRulesResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeRulesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeRulesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeRules", params, headers=headers)
             response = json.loads(body)
@@ -1134,16 +1038,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeRulesSetting(self, request):
         """返回规则引擎可应用匹配请求的设置列表及其详细建议配置信息
 
         :param request: Request instance for DescribeRulesSetting.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeRulesSettingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeRulesSettingResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeRulesSettingRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeRulesSettingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeRulesSetting", params, headers=headers)
             response = json.loads(body)
@@ -1153,160 +1057,112 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSecurityPolicy(self, request):
-        """查询安全防护配置详情
-
-        :param request: Request instance for DescribeSecurityPolicy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSecurityPolicy", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSecurityPolicyResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeSecurityPolicyList(self, request):
-        """查询全部安全实例
+    def DescribeSingleL7AnalysisData(self, request):
+        """本接口（DescribeSingleL7AnalysisData）用于查询七层流量数据分析单值数据列表，单值数据表示：指标在查询时间范围内的单个统计数据，通常表现为接口仅返回一个统计数值。
 
-        :param request: Request instance for DescribeSecurityPolicyList.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyListRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyListResponse`
+        :param request: Request instance for DescribeSingleL7AnalysisData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSingleL7AnalysisDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSingleL7AnalysisDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeSecurityPolicyList", params, headers=headers)
+            body = self.call("DescribeSingleL7AnalysisData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeSecurityPolicyListResponse()
+            model = models.DescribeSingleL7AnalysisDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSecurityPolicyManagedRules(self, request):
-        """分页查询门神规则
+    def DescribeSpeedTestingDetails(self, request):
+        """用于查询拨测分地区数据
 
-        :param request: Request instance for DescribeSecurityPolicyManagedRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyManagedRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyManagedRulesResponse`
+        :param request: Request instance for DescribeSpeedTestingDetails.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingDetailsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingDetailsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeSecurityPolicyManagedRules", params, headers=headers)
+            body = self.call("DescribeSpeedTestingDetails", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeSecurityPolicyManagedRulesResponse()
+            model = models.DescribeSpeedTestingDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSecurityPolicyManagedRulesId(self, request):
-        """规则id查询门神规则详情
+    def DescribeSpeedTestingMetricData(self, request):
+        """查询站点拨测结果
 
-        :param request: Request instance for DescribeSecurityPolicyManagedRulesId.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyManagedRulesIdRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyManagedRulesIdResponse`
+        :param request: Request instance for DescribeSpeedTestingMetricData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingMetricDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingMetricDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeSecurityPolicyManagedRulesId", params, headers=headers)
+            body = self.call("DescribeSpeedTestingMetricData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeSecurityPolicyManagedRulesIdResponse()
+            model = models.DescribeSpeedTestingMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSecurityPolicyRegions(self, request):
-        """查询所有地域信息
+    def DescribeSpeedTestingQuota(self, request):
+        """查询站点拨测配额
 
-        :param request: Request instance for DescribeSecurityPolicyRegions.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyRegionsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPolicyRegionsResponse`
+        :param request: Request instance for DescribeSpeedTestingQuota.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingQuotaRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingQuotaResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeSecurityPolicyRegions", params, headers=headers)
+            body = self.call("DescribeSpeedTestingQuota", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeSecurityPolicyRegionsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeSecurityPortraitRules(self, request):
-        """查询Bot用户画像规则
-
-        :param request: Request instance for DescribeSecurityPortraitRules.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPortraitRulesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeSecurityPortraitRulesResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSecurityPortraitRules", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSecurityPortraitRulesResponse()
+            model = models.DescribeSpeedTestingQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTimingL4Data(self, request):
-        """旧版本的接口已经不兼容，故作下线处理
-
-        四层时序流量数据查询
+        """本接口（DescribeTimingL4Data）用于查询四层时序流量数据列表。
 
         :param request: Request instance for DescribeTimingL4Data.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL4DataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL4DataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL4DataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL4DataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTimingL4Data", params, headers=headers)
             response = json.loads(body)
@@ -1317,19 +1173,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTimingL7AnalysisData(self, request):
-        """查询七层数据分析类时序流量数据
+        """本接口（DescribeTimingL7AnalysisData）查询七层数据分析类时序数据。
 
         :param request: Request instance for DescribeTimingL7AnalysisData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL7AnalysisDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL7AnalysisDataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7AnalysisDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7AnalysisDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTimingL7AnalysisData", params, headers=headers)
             response = json.loads(body)
@@ -1340,19 +1196,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTimingL7CacheData(self, request):
-        """七层查询缓存分析时序类流量数据
+        """本接口（DescribeTimingL7CacheData）用于查询七层缓存分析时序类流量数据。
 
         :param request: Request instance for DescribeTimingL7CacheData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL7CacheDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeTimingL7CacheDataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7CacheDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7CacheDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTimingL7CacheData", params, headers=headers)
             response = json.loads(body)
@@ -1362,89 +1218,89 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeTopL7AnalysisData(self, request):
-        """查询top类流量数据
+    def DescribeTimingL7SourceData(self, request):
+        """本接口（DescribeTimingL7SourceData）查询七层回源分析时序数据。
 
-        :param request: Request instance for DescribeTopL7AnalysisData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeTopL7AnalysisDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeTopL7AnalysisDataResponse`
+        :param request: Request instance for DescribeTimingL7SourceData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7SourceDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7SourceDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeTopL7AnalysisData", params, headers=headers)
+            body = self.call("DescribeTimingL7SourceData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeTopL7AnalysisDataResponse()
+            model = models.DescribeTimingL7SourceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeTopL7CacheData(self, request):
-        """七层查询缓存分析top类流量数据
+    def DescribeTopL7AnalysisData(self, request):
+        """本接口（DescribeTopL7AnalysisData）用于查询七层流量前topN的数据。
 
-        :param request: Request instance for DescribeTopL7CacheData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeTopL7CacheDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeTopL7CacheDataResponse`
+        :param request: Request instance for DescribeTopL7AnalysisData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7AnalysisDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7AnalysisDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeTopL7CacheData", params, headers=headers)
+            body = self.call("DescribeTopL7AnalysisData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeTopL7CacheDataResponse()
+            model = models.DescribeTopL7AnalysisDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebManagedRulesAttackEvents(self, request):
-        """查询Web托管攻击事件
+    def DescribeTopL7CacheData(self, request):
+        """本接口（DescribeTopL7CacheData）用于查询七层缓存分析topN流量数据。
 
-        :param request: Request instance for DescribeWebManagedRulesAttackEvents.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesAttackEventsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesAttackEventsResponse`
+        :param request: Request instance for DescribeTopL7CacheData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7CacheDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7CacheDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeWebManagedRulesAttackEvents", params, headers=headers)
+            body = self.call("DescribeTopL7CacheData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeWebManagedRulesAttackEventsResponse()
+            model = models.DescribeTopL7CacheDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeWebManagedRulesData(self, request):
-        """查询waf攻击时序数据
+        """本接口（DescribeWebManagedRulesData）用于查询WAF攻击的时序数据。
 
         :param request: Request instance for DescribeWebManagedRulesData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesDataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWebManagedRulesData", params, headers=headers)
             response = json.loads(body)
@@ -1454,91 +1310,89 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebManagedRulesLog(self, request):
-        """查询waf攻击日志
+    def DescribeWebManagedRulesHitRuleDetail(self, request):
+        """本接口（DescribeWebManagedRulesHitRuleDetail）用于查询WAF攻击命中规则详情。
 
-        :param request: Request instance for DescribeWebManagedRulesLog.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesLogRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesLogResponse`
+        :param request: Request instance for DescribeWebManagedRulesHitRuleDetail.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesHitRuleDetailRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesHitRuleDetailResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeWebManagedRulesLog", params, headers=headers)
+            body = self.call("DescribeWebManagedRulesHitRuleDetail", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeWebManagedRulesLogResponse()
+            model = models.DescribeWebManagedRulesHitRuleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebManagedRulesTopData(self, request):
-        """此版本的接口已经废弃
-
-        查询waf攻击top数据
+    def DescribeWebManagedRulesLog(self, request):
+        """本接口（DescribeWebManagedRulesLog）用于查询Web攻击日志。
 
-        :param request: Request instance for DescribeWebManagedRulesTopData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesTopDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebManagedRulesTopDataResponse`
+        :param request: Request instance for DescribeWebManagedRulesLog.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesLogRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesLogResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeWebManagedRulesTopData", params, headers=headers)
+            body = self.call("DescribeWebManagedRulesLog", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeWebManagedRulesTopDataResponse()
+            model = models.DescribeWebManagedRulesLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebProtectionAttackEvents(self, request):
-        """查询web防护攻击事件
+    def DescribeWebProtectionClientIpList(self, request):
+        """本接口（DescribeWebProtectionClientIpList）用于查询CC防护客户端（攻击源）IP信息。
 
-        :param request: Request instance for DescribeWebProtectionAttackEvents.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionAttackEventsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionAttackEventsResponse`
+        :param request: Request instance for DescribeWebProtectionClientIpList.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionClientIpListRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionClientIpListResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeWebProtectionAttackEvents", params, headers=headers)
+            body = self.call("DescribeWebProtectionClientIpList", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeWebProtectionAttackEventsResponse()
+            model = models.DescribeWebProtectionClientIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeWebProtectionData(self, request):
-        """查询CC防护时序数据
+        """本接口（DescribeWebProtectionData）用于查询CC防护时序数据。
 
         :param request: Request instance for DescribeWebProtectionData.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionDataResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWebProtectionData", params, headers=headers)
             response = json.loads(body)
@@ -1548,89 +1402,66 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebProtectionLog(self, request):
-        """查询CC防护日志
-
-        :param request: Request instance for DescribeWebProtectionLog.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionLogRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeWebProtectionLogResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebProtectionLog", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebProtectionLogResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeZoneDDoSPolicy(self, request):
-        """查询所有DDoS防护分区
+    def DescribeWebProtectionHitRuleDetail(self, request):
+        """本接口（DescribeWebProtectionHitRuleDetail）用于查询CC防护命中规则详情列表。
 
-        :param request: Request instance for DescribeZoneDDoSPolicy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeZoneDDoSPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeZoneDDoSPolicyResponse`
+        :param request: Request instance for DescribeWebProtectionHitRuleDetail.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionHitRuleDetailRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionHitRuleDetailResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeZoneDDoSPolicy", params, headers=headers)
+            body = self.call("DescribeWebProtectionHitRuleDetail", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeZoneDDoSPolicyResponse()
+            model = models.DescribeWebProtectionHitRuleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeZoneDetails(self, request):
-        """根据站点 ID 查询站点的详细信息
+    def DescribeWebProtectionTopData(self, request):
+        """本接口（DescribeWebProtectionTopData）用于查询CC防护的Top数据。
 
-        :param request: Request instance for DescribeZoneDetails.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeZoneDetailsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeZoneDetailsResponse`
+        :param request: Request instance for DescribeWebProtectionTopData.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionTopDataRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionTopDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeZoneDetails", params, headers=headers)
+            body = self.call("DescribeWebProtectionTopData", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeZoneDetailsResponse()
+            model = models.DescribeWebProtectionTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeZoneSetting(self, request):
         """用于查询站点的所有配置信息。
 
         :param request: Request instance for DescribeZoneSetting.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeZoneSettingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeZoneSettingResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeZoneSettingRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeZoneSettingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeZoneSetting", params, headers=headers)
             response = json.loads(body)
@@ -1641,19 +1472,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeZones(self, request):
-        """用户查询用户站点信息列表，支持分页
+        """用户查询用户站点信息列表，支持分页。
 
         :param request: Request instance for DescribeZones.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DescribeZonesRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DescribeZonesResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeZonesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeZonesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeZones", params, headers=headers)
             response = json.loads(body)
@@ -1663,296 +1494,296 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DownloadL7Logs(self, request):
-        """查询七层离线日志
+    def DownloadL4Logs(self, request):
+        """本接口（DownloadL4Logs）用于下载四层离线日志。
 
-        :param request: Request instance for DownloadL7Logs.
-        :type request: :class:`tencentcloud.teo.v20220106.models.DownloadL7LogsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.DownloadL7LogsResponse`
+        :param request: Request instance for DownloadL4Logs.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DownloadL4LogsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DownloadL4LogsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DownloadL7Logs", params, headers=headers)
+            body = self.call("DownloadL4Logs", params, headers=headers)
             response = json.loads(body)
-            model = models.DownloadL7LogsResponse()
+            model = models.DownloadL4LogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def IdentifyZone(self, request):
-        """用于验证站点所有权
+    def DownloadL7Logs(self, request):
+        """本接口（DownloadL7Logs）下载七层离线日志。
 
-        :param request: Request instance for IdentifyZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.IdentifyZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.IdentifyZoneResponse`
+        :param request: Request instance for DownloadL7Logs.
+        :type request: :class:`tencentcloud.teo.v20220901.models.DownloadL7LogsRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.DownloadL7LogsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("IdentifyZone", params, headers=headers)
+            body = self.call("DownloadL7Logs", params, headers=headers)
             response = json.loads(body)
-            model = models.IdentifyZoneResponse()
+            model = models.DownloadL7LogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ImportDnsRecords(self, request):
-        """导入 DNS 记录
+    def IdentifyZone(self, request):
+        """用于验证站点所有权。
 
-        :param request: Request instance for ImportDnsRecords.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ImportDnsRecordsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ImportDnsRecordsResponse`
+        :param request: Request instance for IdentifyZone.
+        :type request: :class:`tencentcloud.teo.v20220901.models.IdentifyZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.IdentifyZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ImportDnsRecords", params, headers=headers)
+            body = self.call("IdentifyZone", params, headers=headers)
             response = json.loads(body)
-            model = models.ImportDnsRecordsResponse()
+            model = models.IdentifyZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyApplicationProxy(self, request):
-        """修改应用代理
+    def ModifyAccelerationDomain(self, request):
+        """修改加速域名信息
 
-        :param request: Request instance for ModifyApplicationProxy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyResponse`
+        :param request: Request instance for ModifyAccelerationDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyApplicationProxy", params, headers=headers)
+            body = self.call("ModifyAccelerationDomain", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyApplicationProxyResponse()
+            model = models.ModifyAccelerationDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyApplicationProxyRule(self, request):
-        """修改应用代理规则
+    def ModifyAccelerationDomainStatuses(self, request):
+        """批量修改加速域名状态
 
-        :param request: Request instance for ModifyApplicationProxyRule.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyRuleRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyRuleResponse`
+        :param request: Request instance for ModifyAccelerationDomainStatuses.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainStatusesRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainStatusesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyApplicationProxyRule", params, headers=headers)
+            body = self.call("ModifyAccelerationDomainStatuses", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyApplicationProxyRuleResponse()
+            model = models.ModifyAccelerationDomainStatusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyApplicationProxyRuleStatus(self, request):
-        """修改应用代理规则的状态
+    def ModifyAliasDomain(self, request):
+        """修改别称域名。
 
-        :param request: Request instance for ModifyApplicationProxyRuleStatus.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyRuleStatusRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyRuleStatusResponse`
+        :param request: Request instance for ModifyAliasDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyApplicationProxyRuleStatus", params, headers=headers)
+            body = self.call("ModifyAliasDomain", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyApplicationProxyRuleStatusResponse()
+            model = models.ModifyAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyApplicationProxyStatus(self, request):
-        """修改应用代理的状态
+    def ModifyAliasDomainStatus(self, request):
+        """修改别称域名状态。
 
-        :param request: Request instance for ModifyApplicationProxyStatus.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyStatusRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyApplicationProxyStatusResponse`
+        :param request: Request instance for ModifyAliasDomainStatus.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainStatusRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyApplicationProxyStatus", params, headers=headers)
+            body = self.call("ModifyAliasDomainStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyApplicationProxyStatusResponse()
+            model = models.ModifyAliasDomainStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDDoSPolicy(self, request):
-        """修改DDoS防护分区配置
+    def ModifyApplicationProxy(self, request):
+        """修改应用代理
 
-        :param request: Request instance for ModifyDDoSPolicy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyDDoSPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyDDoSPolicyResponse`
+        :param request: Request instance for ModifyApplicationProxy.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDDoSPolicy", params, headers=headers)
+            body = self.call("ModifyApplicationProxy", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDDoSPolicyResponse()
+            model = models.ModifyApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDDoSPolicyHost(self, request):
-        """域名DDoS高可用开关
+    def ModifyApplicationProxyRule(self, request):
+        """修改应用代理规则
 
-        :param request: Request instance for ModifyDDoSPolicyHost.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyDDoSPolicyHostRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyDDoSPolicyHostResponse`
+        :param request: Request instance for ModifyApplicationProxyRule.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDDoSPolicyHost", params, headers=headers)
+            body = self.call("ModifyApplicationProxyRule", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDDoSPolicyHostResponse()
+            model = models.ModifyApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDefaultCertificate(self, request):
-        """修改默认证书状态
+    def ModifyApplicationProxyRuleStatus(self, request):
+        """修改应用代理规则的状态
 
-        :param request: Request instance for ModifyDefaultCertificate.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyDefaultCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyDefaultCertificateResponse`
+        :param request: Request instance for ModifyApplicationProxyRuleStatus.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleStatusRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDefaultCertificate", params, headers=headers)
+            body = self.call("ModifyApplicationProxyRuleStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDefaultCertificateResponse()
+            model = models.ModifyApplicationProxyRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDnsRecord(self, request):
-        """修改 DNS 记录
+    def ModifyApplicationProxyStatus(self, request):
+        """修改应用代理的状态
 
-        :param request: Request instance for ModifyDnsRecord.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyDnsRecordRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyDnsRecordResponse`
+        :param request: Request instance for ModifyApplicationProxyStatus.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyStatusRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDnsRecord", params, headers=headers)
+            body = self.call("ModifyApplicationProxyStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDnsRecordResponse()
+            model = models.ModifyApplicationProxyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDnssec(self, request):
-        """修改 DNSSEC 状态
+    def ModifyDefaultCertificate(self, request):
+        """修改默认证书状态
 
-        :param request: Request instance for ModifyDnssec.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyDnssecRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyDnssecResponse`
+        :param request: Request instance for ModifyDefaultCertificate.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyDefaultCertificateRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyDefaultCertificateResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDnssec", params, headers=headers)
+            body = self.call("ModifyDefaultCertificate", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDnssecResponse()
+            model = models.ModifyDefaultCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyHostsCertificate(self, request):
         """用于修改域名证书
 
         :param request: Request instance for ModifyHostsCertificate.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyHostsCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyHostsCertificateResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyHostsCertificateRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyHostsCertificateResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyHostsCertificate", params, headers=headers)
             response = json.loads(body)
@@ -1962,66 +1793,20 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyLoadBalancing(self, request):
-        """修改负载均衡
-
-        :param request: Request instance for ModifyLoadBalancing.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyLoadBalancingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyLoadBalancingResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyLoadBalancing", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyLoadBalancingResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def ModifyLoadBalancingStatus(self, request):
-        """修改负载均衡状态
-
-        :param request: Request instance for ModifyLoadBalancingStatus.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyLoadBalancingStatusRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyLoadBalancingStatusResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyLoadBalancingStatus", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyLoadBalancingStatusResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def ModifyOriginGroup(self, request):
-        """源站组修改
+        """修改源站组
 
         :param request: Request instance for ModifyOriginGroup.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyOriginGroupRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyOriginGroupResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyOriginGroupRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyOriginGroupResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyOriginGroup", params, headers=headers)
             response = json.loads(body)
@@ -2035,16 +1820,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyRule(self, request):
         """修改规则引擎规则。
 
         :param request: Request instance for ModifyRule.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyRuleRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyRuleResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyRuleRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyRule", params, headers=headers)
             response = json.loads(body)
@@ -2058,16 +1843,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyRulePriority(self, request):
         """修改规则引擎规则优先级
 
         :param request: Request instance for ModifyRulePriority.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyRulePriorityRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyRulePriorityResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyRulePriorityRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyRulePriorityResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyRulePriority", params, headers=headers)
             response = json.loads(body)
@@ -2078,19 +1863,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySecurityPolicy(self, request):
-        """修改Web&Bot安全配置
+        """修改Web&Bot安全配置。
 
         :param request: Request instance for ModifySecurityPolicy.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifySecurityPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifySecurityPolicyResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityPolicyRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifySecurityPolicyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifySecurityPolicy", params, headers=headers)
             response = json.loads(body)
@@ -2100,66 +1885,66 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyZone(self, request):
-        """用该站点信息
+    def ModifySecurityWafGroupPolicy(self, request):
+        """修改安全配置托管规则
 
-        :param request: Request instance for ModifyZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyZoneResponse`
+        :param request: Request instance for ModifySecurityWafGroupPolicy.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityWafGroupPolicyRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifySecurityWafGroupPolicyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyZone", params, headers=headers)
+            body = self.call("ModifySecurityWafGroupPolicy", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyZoneResponse()
+            model = models.ModifySecurityWafGroupPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyZoneCnameSpeedUp(self, request):
-        """开启，关闭 CNAME 加速
+    def ModifyZone(self, request):
+        """修改站点信息。
 
-        :param request: Request instance for ModifyZoneCnameSpeedUp.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyZoneCnameSpeedUpRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyZoneCnameSpeedUpResponse`
+        :param request: Request instance for ModifyZone.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyZoneCnameSpeedUp", params, headers=headers)
+            body = self.call("ModifyZone", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyZoneCnameSpeedUpResponse()
+            model = models.ModifyZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyZoneSetting(self, request):
         """用于修改站点配置
 
         :param request: Request instance for ModifyZoneSetting.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyZoneSettingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyZoneSettingResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneSettingRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyZoneSettingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyZoneSetting", params, headers=headers)
             response = json.loads(body)
@@ -2170,19 +1955,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyZoneStatus(self, request):
-        """用于开启，关闭站点
+        """用于开启，关闭站点。
 
         :param request: Request instance for ModifyZoneStatus.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ModifyZoneStatusRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ModifyZoneStatusResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneStatusRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyZoneStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyZoneStatus", params, headers=headers)
             response = json.loads(body)
@@ -2192,20 +1977,43 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ReclaimAliasDomain(self, request):
+        """当客户取回站定的同时会取回此站点下关联的别称域名，此时入参为ZoneId；当客户接入站点发现已被别称域名接入时通过验证之后可取回域名，此时入参为ZoneName。
+
+        :param request: Request instance for ReclaimAliasDomain.
+        :type request: :class:`tencentcloud.teo.v20220901.models.ReclaimAliasDomainRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ReclaimAliasDomainResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ReclaimAliasDomain", params, headers=headers)
+            response = json.loads(body)
+            model = models.ReclaimAliasDomainResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ReclaimZone(self, request):
-        """站点被其他用户接入后，验证了站点所有权之后，可以找回该站点
+        """站点被其他用户接入后，验证了站点所有权之后，可以找回该站点。
 
         :param request: Request instance for ReclaimZone.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ReclaimZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ReclaimZoneResponse`
+        :type request: :class:`tencentcloud.teo.v20220901.models.ReclaimZoneRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.ReclaimZoneResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ReclaimZone", params, headers=headers)
             response = json.loads(body)
@@ -2215,28 +2023,28 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ScanDnsRecords(self, request):
-        """扫描站点历史解析记录
+    def UpdateOriginProtectionIPWhitelist(self, request):
+        """更新源站防护IP白名单
 
-        :param request: Request instance for ScanDnsRecords.
-        :type request: :class:`tencentcloud.teo.v20220106.models.ScanDnsRecordsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220106.models.ScanDnsRecordsResponse`
+        :param request: Request instance for UpdateOriginProtectionIPWhitelist.
+        :type request: :class:`tencentcloud.teo.v20220901.models.UpdateOriginProtectionIPWhitelistRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.UpdateOriginProtectionIPWhitelistResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ScanDnsRecords", params, headers=headers)
+            body = self.call("UpdateOriginProtectionIPWhitelist", params, headers=headers)
             response = json.loads(body)
-            model = models.ScanDnsRecordsResponse()
+            model = models.UpdateOriginProtectionIPWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.873/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.873/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.872/setup.py` & `tencentcloud-sdk-python-teo-3.0.873/setup.py`

 * *Files identical despite different names*

