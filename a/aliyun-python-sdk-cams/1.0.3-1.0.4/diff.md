# Comparing `tmp/aliyun-python-sdk-cams-1.0.3.tar.gz` & `tmp/aliyun-python-sdk-cams-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.3.tar", last modified: Mon Oct 12 01:51:59 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.4.tar", last modified: Fri Apr 14 02:21:46 2023, max compression
```

## Comparing `aliyun-python-sdk-cams-1.0.3.tar` & `aliyun-python-sdk-cams-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/
--rw-r--r--   0 root         (0) root         (0)       21 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/
--rw-r--r--   0 root         (0) root         (0)     2333 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/CheckContactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3437 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/SendMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2020-10-12 01:51:59.000000 aliyun-python-sdk-cams-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/setup.py
```

### Comparing `aliyun-python-sdk-cams-1.0.3/PKG-INFO` & `aliyun-python-sdk-cams-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.3
+Version: 1.0.4
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.3/README.rst` & `aliyun-python-sdk-cams-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.3/aliyun_python_sdk_cams.egg-info/PKG-INFO` & `aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.3
+Version: 1.0.4
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/endpoint.py` & `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/CheckContactsRequest.py` & `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,53 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
 
-class CheckContactsRequest(RpcRequest):
+class QueryWabaBusinessInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'CheckContacts','cams')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'QueryWabaBusinessInfo')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_WabaId(self): # String
+		return self.get_query_params().get('WabaId')
 
-	def get_ResourceOwnerId(self):
-		return self.get_query_params().get('ResourceOwnerId')
-
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ChannelType(self):
-		return self.get_body_params().get('ChannelType')
-
-	def set_ChannelType(self,ChannelType):
-		self.add_body_params('ChannelType', ChannelType)
-
-	def get__From(self):
-		return self.get_body_params().get('From')
-
-	def set__From(self,_From):
-		self.add_body_params('From', _From)
-
-	def get_ResourceOwnerAccount(self):
-		return self.get_query_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerId(self):
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Contacts(self):
-		return self.get_body_params().get('Contacts')
+	def set_WabaId(self, WabaId):  # String
+		self.add_query_param('WabaId', WabaId)
+	def get_CustSpaceId(self): # String
+		return self.get_query_params().get('CustSpaceId')
 
-	def set_Contacts(self,Contacts):
-		self.add_body_params('Contacts', Contacts)
+	def set_CustSpaceId(self, CustSpaceId):  # String
+		self.add_query_param('CustSpaceId', CustSpaceId)
```

### Comparing `aliyun-python-sdk-cams-1.0.3/aliyunsdkcams/request/v20200606/SendMessageRequest.py` & `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,96 +15,60 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
+import json
 
-class SendMessageRequest(RpcRequest):
+class ModifyPhoneBusinessProfileRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'SendMessage','cams')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'ModifyPhoneBusinessProfile')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_PhoneNumber(self): # String
+		return self.get_query_params().get('PhoneNumber')
 
-	def get_ResourceOwnerId(self):
-		return self.get_query_params().get('ResourceOwnerId')
-
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_MessageType(self):
-		return self.get_body_params().get('MessageType')
-
-	def set_MessageType(self,MessageType):
-		self.add_body_params('MessageType', MessageType)
-
-	def get_TemplateBodyParams(self):
-		return self.get_body_params().get('TemplateBodyParams')
-
-	def set_TemplateBodyParams(self,TemplateBodyParams):
-		self.add_body_params('TemplateBodyParams', TemplateBodyParams)
-
-	def get_Link(self):
-		return self.get_body_params().get('Link')
-
-	def set_Link(self,Link):
-		self.add_body_params('Link', Link)
-
-	def get_Caption(self):
-		return self.get_body_params().get('Caption')
-
-	def set_Caption(self,Caption):
-		self.add_body_params('Caption', Caption)
-
-	def get_Type(self):
-		return self.get_body_params().get('Type')
-
-	def set_Type(self,Type):
-		self.add_body_params('Type', Type)
-
-	def get_ChannelType(self):
-		return self.get_body_params().get('ChannelType')
-
-	def set_ChannelType(self,ChannelType):
-		self.add_body_params('ChannelType', ChannelType)
-
-	def get__From(self):
-		return self.get_body_params().get('From')
-
-	def set__From(self,_From):
-		self.add_body_params('From', _From)
-
-	def get_Text(self):
-		return self.get_body_params().get('Text')
-
-	def set_Text(self,Text):
-		self.add_body_params('Text', Text)
-
-	def get_ResourceOwnerAccount(self):
-		return self.get_query_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerId(self):
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_To(self):
-		return self.get_body_params().get('To')
-
-	def set_To(self,To):
-		self.add_body_params('To', To)
-
-	def get_TemplateCode(self):
-		return self.get_body_params().get('TemplateCode')
+	def set_PhoneNumber(self, PhoneNumber):  # String
+		self.add_query_param('PhoneNumber', PhoneNumber)
+	def get_Description(self): # String
+		return self.get_query_params().get('Description')
+
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_Vertical(self): # String
+		return self.get_query_params().get('Vertical')
+
+	def set_Vertical(self, Vertical):  # String
+		self.add_query_param('Vertical', Vertical)
+	def get_Email(self): # String
+		return self.get_query_params().get('Email')
+
+	def set_Email(self, Email):  # String
+		self.add_query_param('Email', Email)
+	def get_Address(self): # String
+		return self.get_query_params().get('Address')
+
+	def set_Address(self, Address):  # String
+		self.add_query_param('Address', Address)
+	def get_ProfilePictureUrl(self): # String
+		return self.get_query_params().get('ProfilePictureUrl')
+
+	def set_ProfilePictureUrl(self, ProfilePictureUrl):  # String
+		self.add_query_param('ProfilePictureUrl', ProfilePictureUrl)
+	def get_CustSpaceId(self): # String
+		return self.get_query_params().get('CustSpaceId')
+
+	def set_CustSpaceId(self, CustSpaceId):  # String
+		self.add_query_param('CustSpaceId', CustSpaceId)
+	def get_Websites(self): # Array
+		return self.get_query_params().get('Websites')
 
-	def set_TemplateCode(self,TemplateCode):
-		self.add_body_params('TemplateCode', TemplateCode)
+	def set_Websites(self, Websites):  # Array
+		self.add_query_param("Websites", json.dumps(Websites))
```

### Comparing `aliyun-python-sdk-cams-1.0.3/setup.py` & `aliyun-python-sdk-cams-1.0.4/setup.py`

 * *Files identical despite different names*

