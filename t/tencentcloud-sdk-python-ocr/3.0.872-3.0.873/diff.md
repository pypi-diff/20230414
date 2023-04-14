# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.872.tar", last modified: Thu Apr 13 00:53:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.873.tar", last modified: Fri Apr 14 00:49:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.872.tar` & `tencentcloud-sdk-python-ocr-3.0.873.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   104266 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   406294 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:53:11.000000 tencentcloud-sdk-python-ocr-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   105698 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   406294 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:49:01.000000 tencentcloud-sdk-python-ocr-3.0.873/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.873/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/README.rst` & `tencentcloud-sdk-python-ocr-3.0.873/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def BizLicenseOCR(self, request):
-        """本接口支持快速精准识别营业执照上的字段，包括统一社会信用代码、公司名称、经营场所、主体类型、法定代表人、注册资金、组成形式、成立日期、营业期限和经营范围等字段。
+        """本接口支持快速精准识别营业执照上的字段，包括统一社会信用代码、公司名称、主体类型、法定代表人、注册资本、组成形式、成立日期、营业期限和经营范围等字段。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for BizLicenseOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.BizLicenseOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.BizLicenseOCRResponse`
 
@@ -148,15 +148,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def BusInvoiceOCR(self, request):
-        """本接口支持识别公路汽车客票的发票代码、发票号码、日期、姓名、票价等字段。
+        """本接口支持识别公路汽车客票关键字段的识别，包括发票代码、发票号码、日期、票价、始发地、目的地、姓名、时间、发票消费类型、身份证号、省、市、开票日期、乘车地点、检票口、客票类型、车型、座位号、车次等。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for BusInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.BusInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.BusInvoiceOCRResponse`
 
@@ -379,15 +379,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def EnterpriseLicenseOCR(self, request):
-        """本接口支持智能化识别各类企业登记证书、许可证书、企业执照、三证合一类证书，结构化输出统一社会信用代码、公司名称、法定代表人、公司地址、注册资金、企业类型、经营范围等关键字段。
+        """本接口支持智能化识别各类企业登记证书、许可证书、企业执照、三证合一类证书，结构化输出统一社会信用代码、公司名称、法定代表人、公司地址、注册资金、企业类型、经营范围、成立日期、有效期、开办资金、经费来源、举办单位等关键字段。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for EnterpriseLicenseOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.EnterpriseLicenseOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.EnterpriseLicenseOCRResponse`
 
@@ -883,15 +883,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def HmtResidentPermitOCR(self, request):
-        """港澳台居住证OCR支持港澳台居住证正反面全字段内容检测识别功能，包括姓名、性别、出生日期、地址、身份证ID、签发机关、有效期限、签发次数、通行证号码关键字段识别。可以应用于港澳台居住证信息有效性校验场景，例如银行开户、用户注册等场景。
+        """港澳台居住证OCR支持港澳台居住证正反面全字段内容检测识别功能，包括姓名、性别、出生日期、地址、身份证号、签发机关、有效期限、签发次数、通行证号码关键字段识别。可以应用于港澳台居住证信息识别场景，例如银行开户、用户注册等。
 
         默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for HmtResidentPermitOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.HmtResidentPermitOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.HmtResidentPermitOCRResponse`
 
@@ -1053,15 +1053,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def InvoiceGeneralOCR(self, request):
-        """本接口支持对通用机打发票的发票代码、发票号码、日期、购买方识别号、销售方识别号、校验码、小写金额等关键字段的识别。
+        """本接口支持对通用机打发票的发票代码、发票号码、日期、合计金额(小写)、合计金额(大写)、购买方识别号、销售方识别号、校验码、购买方名称、销售方名称、时间、种类、发票消费类型、省、市、是否有公司印章、发票名称、购买方地址、电话、销售方地址、电话、购买方开户行及账号、销售方开户行及账号、经办人取票用户、经办人支付信息、经办人商户号、经办人订单号、货物或应税劳务、服务名称、数量、单价、税率、税额、金额、单位、规格型号、合计税额、合计金额、备注、收款人、复核、开票人、密码区、行业分类等字段的识别。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for InvoiceGeneralOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.InvoiceGeneralOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.InvoiceGeneralOCRResponse`
 
@@ -1127,15 +1127,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def MLIDPassportOCR(self, request):
-        """本接口支持中国港澳台地区以及其他国家、地区的护照识别。识别字段包括护照ID、姓名、出生日期、性别、有效期、发行国、国籍，具备护照人像照片的裁剪功能和翻拍、复印件告警功能。
+        """本接口支持中国港澳台地区以及其他国家、地区的护照识别。识别字段包括护照ID、姓名、出生日期、性别、有效期、发行国、国籍、国家地区代码，具备护照人像照片的裁剪功能和翻拍、复印件告警功能。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for MLIDPassportOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.MLIDPassportOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.MLIDPassportOCRResponse`
 
@@ -1551,15 +1551,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizePhilippinesVoteIDOCR(self, request):
-        """菲律宾VoteID识别
+        """本接口支持菲律宾VoteID识别，识别字段包括姓名、姓氏、出生日期、婚姻状况、国籍、地址、地区、菲律宾VoteID的VIN等。
+
+        默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for RecognizePhilippinesVoteIDOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesVoteIDOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesVoteIDOCRResponse`
 
         """
         try:
@@ -1622,15 +1624,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeThaiIDCardOCR(self, request):
-        """本接口支持泰国身份证识别，识别字段包括泰文姓名、英文姓名、地址、出生日期、身份证号码。
+        """本接口支持泰国身份证识别，识别字段包括泰文姓名、英文姓名、地址、出生日期、身份证号码、首次领用日期、签发日期等字段。
         本接口暂未完全对外开放，如需咨询，请[联系商务](https://cloud.tencent.com/about/connect)
 
         :param request: Request instance for RecognizeThaiIDCardOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeThaiIDCardOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeThaiIDCardOCRResponse`
 
         """
@@ -1921,15 +1923,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def TollInvoiceOCR(self, request):
-        """本接口支持对过路过桥费发票的发票代码、发票号码、日期、小写金额等关键字段的识别。
+        """本接口支持过路过桥费发票关键字段的识别，包括发票代码、发票号码、日期、金额、入口、出口、时间、发票消费类型、高速标志等。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for TollInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.TollInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.TollInvoiceOCRResponse`
 
@@ -1946,15 +1948,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def TrainTicketOCR(self, request):
-        """本接口支持火车票全字段的识别，包括编号、票价、姓名、座位号、出发时间、出发站、到达站、车次、席别、发票类型及序列号等。
+        """本接口支持火车票全字段的识别，包括编号、出发站、到达站、出发时间、车次、座位号、姓名、票价、席别、身份证号、发票消费类型、序列号、加收票价、手续费、大写金额、售票站、原票价、发票类型、收据号码、是否仅供报销使用等字段的识别。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for TrainTicketOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.TrainTicketOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.TrainTicketOCRResponse`
 
@@ -2046,15 +2048,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def VatRollInvoiceOCR(self, request):
-        """本接口支持对增值税发票（卷票）的发票代码、发票号码、日期、校验码、合计金额（小写）等关键字段的识别。
+        """本接口支持对增值税发票（卷票）关键字段的识别，包括的发票代码、合计金额(小写)、合计金额(大写)、开票日期、发票号码、购买方识别号、销售方识别号、校验码、销售方名称、购买方名称、发票消费类型、省、市、是否有公司印章、单价、金额、数量、服务类型、品名、种类等。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for VatRollInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VatRollInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.VatRollInvoiceOCRResponse`
 
@@ -2254,15 +2256,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def WaybillOCR(self, request):
-        """本接口支持市面上主流版式电子运单的识别，包括收件人和寄件人的姓名、电话、地址以及运单号等字段，精度均处于业界领先水平，识别准确率达到99%以上。
+        """本接口支持市面上主流版式电子运单的识别，包括收件人和寄件人的姓名、电话、地址以及运单号等字段。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for WaybillOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.WaybillOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.WaybillOCRResponse`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.873/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.873/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.872
+Version: 3.0.873
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.872/setup.py` & `tencentcloud-sdk-python-ocr-3.0.873/setup.py`

 * *Files identical despite different names*

