# Comparing `tmp/g42cloudsdkcore-0.0.4b0-py2.py3-none-any.whl.zip` & `tmp/g42cloudsdkcore-0.0.5b0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,62 +1,43 @@
-Zip file size: 63463 bytes, number of entries: 60
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/__init__.py
--rw-------  2.0 unx    23460 b- defN 23-Feb-20 02:50 g42cloudsdkcore/client.py
--rw-------  2.0 unx     1283 b- defN 23-Feb-20 02:50 g42cloudsdkcore/sdk_request.py
--rw-------  2.0 unx     2385 b- defN 23-Feb-20 02:50 g42cloudsdkcore/sdk_response.py
--rw-------  2.0 unx      951 b- defN 23-Feb-20 02:50 g42cloudsdkcore/sdk_stream_request.py
--rw-------  2.0 unx     1139 b- defN 23-Feb-20 02:50 g42cloudsdkcore/sdk_stream_response.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/auth/__init__.py
--rw-------  2.0 unx     1070 b- defN 23-Feb-20 02:50 g42cloudsdkcore/auth/cache.py
--rw-------  2.0 unx    12929 b- defN 23-Feb-20 02:50 g42cloudsdkcore/auth/credentials.py
--rw-------  2.0 unx     8167 b- defN 23-Feb-20 02:50 g42cloudsdkcore/auth/internal.py
--rw-------  2.0 unx     8899 b- defN 23-Feb-20 02:50 g42cloudsdkcore/auth/provider.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/exceptions/__init__.py
--rw-------  2.0 unx     7446 b- defN 23-Feb-20 02:50 g42cloudsdkcore/exceptions/exceptions.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/__init__.py
--rw-------  2.0 unx     2491 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/formdata.py
--rw-------  2.0 unx     1130 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/future_session.py
--rw-------  2.0 unx     8582 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/http_client.py
--rw-------  2.0 unx     4040 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/http_config.py
--rw-------  2.0 unx     1842 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/http_handler.py
--rw-------  2.0 unx     1173 b- defN 23-Feb-20 02:50 g42cloudsdkcore/http/primitive_types.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/region/__init__.py
--rw-------  2.0 unx     2500 b- defN 23-Feb-20 02:50 g42cloudsdkcore/region/cache.py
--rw-------  2.0 unx     2599 b- defN 23-Feb-20 02:50 g42cloudsdkcore/region/provider.py
--rw-------  2.0 unx     1423 b- defN 23-Feb-20 02:50 g42cloudsdkcore/region/region.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/signer/__init__.py
--rw-------  2.0 unx     2930 b- defN 23-Feb-20 02:50 g42cloudsdkcore/signer/hkdf.py
--rw-------  2.0 unx     9271 b- defN 23-Feb-20 02:50 g42cloudsdkcore/signer/signer.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/__init__.py
--rw-------  2.0 unx      893 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/core_utils.py
--rw-------  2.0 unx     4323 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/http_utils.py
--rw-------  2.0 unx     1195 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/path_utils.py
--rw-------  2.0 unx     1418 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/six_utils.py
--rw-------  2.0 unx     1289 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/string_utils.py
--rw-------  2.0 unx      203 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/time_utils.py
--rw-------  2.0 unx     5631 b- defN 23-Feb-20 02:50 g42cloudsdkcore/utils/xml_utils.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 tests/__init__.py
--rw-------  2.0 unx     3481 b- defN 23-Feb-20 02:50 tests/test_client_build.py
--rw-------  2.0 unx     9115 b- defN 23-Feb-20 02:50 tests/test_credential_provider.py
--rw-------  2.0 unx     1602 b- defN 23-Feb-20 02:50 tests/test_endpoint_without_scheme.py
--rw-------  2.0 unx     3175 b- defN 23-Feb-20 02:50 tests/test_federal_credentials.py
--rw-------  2.0 unx     3771 b- defN 23-Feb-20 02:50 tests/test_region_provider.py
--rw-------  2.0 unx     3897 b- defN 23-Feb-20 02:50 tests/test_region_with_project_id.py
--rw-------  2.0 unx     2346 b- defN 23-Feb-20 02:50 tests/test_region_without_project_id.py
--rw-------  2.0 unx     7291 b- defN 23-Feb-20 02:50 tests/test_request_and_exceptions.py
--rw-------  2.0 unx     2053 b- defN 23-Feb-20 02:50 tests/test_signer.py
--rw-------  2.0 unx     2013 b- defN 23-Feb-20 02:50 tests/test_upload_download.py
--rw-------  2.0 unx     3557 b- defN 23-Feb-20 02:50 tests/test_xml_transfer.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 tests/model/__init__.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 tests/model/obs/__init__.py
--rw-------  2.0 unx     4787 b- defN 23-Feb-20 02:50 tests/model/obs/model.py
--rw-------  2.0 unx        0 b- defN 23-Feb-20 02:50 tests/model/service/__init__.py
--rw-------  2.0 unx     1443 b- defN 23-Feb-20 02:50 tests/model/service/service_client.py
--rw-------  2.0 unx     1483 b- defN 23-Feb-20 02:50 tests/model/service/service_region.py
--rw-------  2.0 unx       76 b- defN 23-Feb-20 02:50 tests/model/vpc/__init__.py
--rw-------  2.0 unx     2388 b- defN 23-Feb-20 02:50 tests/model/vpc/list_vpcs_response.py
--rwxrwxrwx  2.0 unx      584 b- defN 23-Feb-20 02:50 g42cloudsdkcore-0.0.4b0.dist-info/LICENSE
--rw-------  2.0 unx     1489 b- defN 23-Feb-20 02:50 g42cloudsdkcore-0.0.4b0.dist-info/METADATA
--rw-------  2.0 unx      110 b- defN 23-Feb-20 02:50 g42cloudsdkcore-0.0.4b0.dist-info/WHEEL
--rw-------  2.0 unx       22 b- defN 23-Feb-20 02:50 g42cloudsdkcore-0.0.4b0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5317 b- defN 23-Feb-20 02:50 g42cloudsdkcore-0.0.4b0.dist-info/RECORD
-60 files, 180662 bytes uncompressed, 54899 bytes compressed:  69.6%
+Zip file size: 45372 bytes, number of entries: 41
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/__init__.py
+-rw-------  2.0 unx    25097 b- defN 23-Apr-14 02:24 g42cloudsdkcore/client.py
+-rw-------  2.0 unx     1283 b- defN 23-Apr-14 02:24 g42cloudsdkcore/sdk_request.py
+-rw-------  2.0 unx     2385 b- defN 23-Apr-14 02:24 g42cloudsdkcore/sdk_response.py
+-rw-------  2.0 unx      951 b- defN 23-Apr-14 02:24 g42cloudsdkcore/sdk_stream_request.py
+-rw-------  2.0 unx     1139 b- defN 23-Apr-14 02:24 g42cloudsdkcore/sdk_stream_response.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/auth/__init__.py
+-rw-------  2.0 unx     1070 b- defN 23-Apr-14 02:24 g42cloudsdkcore/auth/cache.py
+-rw-------  2.0 unx    12929 b- defN 23-Apr-14 02:24 g42cloudsdkcore/auth/credentials.py
+-rw-------  2.0 unx     8167 b- defN 23-Apr-14 02:24 g42cloudsdkcore/auth/internal.py
+-rw-------  2.0 unx     8899 b- defN 23-Apr-14 02:24 g42cloudsdkcore/auth/provider.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/exceptions/__init__.py
+-rw-------  2.0 unx     3045 b- defN 23-Apr-14 02:24 g42cloudsdkcore/exceptions/exception_handler.py
+-rw-------  2.0 unx     7557 b- defN 23-Apr-14 02:24 g42cloudsdkcore/exceptions/exceptions.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/__init__.py
+-rw-------  2.0 unx     2491 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/formdata.py
+-rw-------  2.0 unx     1130 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/future_session.py
+-rw-------  2.0 unx     6043 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/http_client.py
+-rw-------  2.0 unx     4040 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/http_config.py
+-rw-------  2.0 unx     1842 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/http_handler.py
+-rw-------  2.0 unx     1173 b- defN 23-Apr-14 02:24 g42cloudsdkcore/http/primitive_types.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/region/__init__.py
+-rw-------  2.0 unx     2500 b- defN 23-Apr-14 02:24 g42cloudsdkcore/region/cache.py
+-rw-------  2.0 unx     2599 b- defN 23-Apr-14 02:24 g42cloudsdkcore/region/provider.py
+-rw-------  2.0 unx     3103 b- defN 23-Apr-14 02:24 g42cloudsdkcore/region/region.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/signer/__init__.py
+-rw-------  2.0 unx     2930 b- defN 23-Apr-14 02:24 g42cloudsdkcore/signer/hkdf.py
+-rw-------  2.0 unx     9837 b- defN 23-Apr-14 02:24 g42cloudsdkcore/signer/signer.py
+-rw-------  2.0 unx        0 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/__init__.py
+-rw-------  2.0 unx      893 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/core_utils.py
+-rw-------  2.0 unx     4323 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/http_utils.py
+-rw-------  2.0 unx     1195 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/path_utils.py
+-rw-------  2.0 unx     1418 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/six_utils.py
+-rw-------  2.0 unx     1289 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/string_utils.py
+-rw-------  2.0 unx      203 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/time_utils.py
+-rw-------  2.0 unx     5631 b- defN 23-Apr-14 02:24 g42cloudsdkcore/utils/xml_utils.py
+-rwxrwxrwx  2.0 unx      584 b- defN 23-Apr-14 02:25 g42cloudsdkcore-0.0.5b0.dist-info/LICENSE
+-rw-------  2.0 unx     1489 b- defN 23-Apr-14 02:25 g42cloudsdkcore-0.0.5b0.dist-info/METADATA
+-rw-------  2.0 unx      110 b- defN 23-Apr-14 02:25 g42cloudsdkcore-0.0.5b0.dist-info/WHEEL
+-rw-------  2.0 unx       16 b- defN 23-Apr-14 02:25 g42cloudsdkcore-0.0.5b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3691 b- defN 23-Apr-14 02:25 g42cloudsdkcore-0.0.5b0.dist-info/RECORD
+41 files, 131052 bytes uncompressed, 39366 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: g42cloudsdkcore/auth/provider.py
 Comment: 
 
 Filename: g42cloudsdkcore/exceptions/__init__.py
 Comment: 
 
+Filename: g42cloudsdkcore/exceptions/exception_handler.py
+Comment: 
+
 Filename: g42cloudsdkcore/exceptions/exceptions.py
 Comment: 
 
 Filename: g42cloudsdkcore/http/__init__.py
 Comment: 
 
 Filename: g42cloudsdkcore/http/formdata.py
@@ -99,83 +102,23 @@
 
 Filename: g42cloudsdkcore/utils/time_utils.py
 Comment: 
 
 Filename: g42cloudsdkcore/utils/xml_utils.py
 Comment: 
 
-Filename: tests/__init__.py
-Comment: 
-
-Filename: tests/test_client_build.py
-Comment: 
-
-Filename: tests/test_credential_provider.py
-Comment: 
-
-Filename: tests/test_endpoint_without_scheme.py
-Comment: 
-
-Filename: tests/test_federal_credentials.py
-Comment: 
-
-Filename: tests/test_region_provider.py
-Comment: 
-
-Filename: tests/test_region_with_project_id.py
-Comment: 
-
-Filename: tests/test_region_without_project_id.py
-Comment: 
-
-Filename: tests/test_request_and_exceptions.py
-Comment: 
-
-Filename: tests/test_signer.py
-Comment: 
-
-Filename: tests/test_upload_download.py
-Comment: 
-
-Filename: tests/test_xml_transfer.py
-Comment: 
-
-Filename: tests/model/__init__.py
-Comment: 
-
-Filename: tests/model/obs/__init__.py
-Comment: 
-
-Filename: tests/model/obs/model.py
-Comment: 
-
-Filename: tests/model/service/__init__.py
-Comment: 
-
-Filename: tests/model/service/service_client.py
-Comment: 
-
-Filename: tests/model/service/service_region.py
-Comment: 
-
-Filename: tests/model/vpc/__init__.py
-Comment: 
-
-Filename: tests/model/vpc/list_vpcs_response.py
-Comment: 
-
-Filename: g42cloudsdkcore-0.0.4b0.dist-info/LICENSE
+Filename: g42cloudsdkcore-0.0.5b0.dist-info/LICENSE
 Comment: 
 
-Filename: g42cloudsdkcore-0.0.4b0.dist-info/METADATA
+Filename: g42cloudsdkcore-0.0.5b0.dist-info/METADATA
 Comment: 
 
-Filename: g42cloudsdkcore-0.0.4b0.dist-info/WHEEL
+Filename: g42cloudsdkcore-0.0.5b0.dist-info/WHEEL
 Comment: 
 
-Filename: g42cloudsdkcore-0.0.4b0.dist-info/top_level.txt
+Filename: g42cloudsdkcore-0.0.5b0.dist-info/top_level.txt
 Comment: 
 
-Filename: g42cloudsdkcore-0.0.4b0.dist-info/RECORD
+Filename: g42cloudsdkcore-0.0.5b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## g42cloudsdkcore/client.py

```diff
@@ -16,59 +16,61 @@
  KIND, either express or implied.  See the LICENSE for the
  specific language governing permissions and limitations
  under the LICENSE.
 """
 
 import datetime
 import decimal
-import importlib
 import logging
 import re
 import sys
+import threading
+import warnings
 from collections import OrderedDict
 from logging.handlers import RotatingFileHandler
 
 import simplejson as json
 import six
 from requests_toolbelt import MultipartEncoder
 from six.moves.urllib.parse import quote, urlparse
 
 from g42cloudsdkcore.auth.credentials import BasicCredentials, DerivedCredentials
 from g42cloudsdkcore.auth.provider import CredentialProviderChain
+from g42cloudsdkcore.exceptions.exceptions import HostUnreachableException
+from g42cloudsdkcore.exceptions import exception_handler
 from g42cloudsdkcore.http.formdata import FormFile
 from g42cloudsdkcore.http.http_client import HttpClient
 from g42cloudsdkcore.http.http_config import HttpConfig
 from g42cloudsdkcore.http.http_handler import HttpHandler
 from g42cloudsdkcore.http.primitive_types import native_types_mapping
 from g42cloudsdkcore.http.primitive_types import primitive_types
 from g42cloudsdkcore.sdk_request import SdkRequest
 from g42cloudsdkcore.sdk_response import FutureSdkResponse
 from g42cloudsdkcore.sdk_stream_response import SdkStreamResponse
 from g42cloudsdkcore.utils import http_utils, core_utils
 from g42cloudsdkcore.utils.xml_utils import XmlTransfer
 
 
 class ClientBuilder(object):
+    _HTTP_SCHEME = "http"
+    _HTTPS_SCHEME = "https"
 
     def __init__(self, client_type, credential_type=BasicCredentials.__name__):
         self._client_type = client_type
         self._credential_type = credential_type.split(',')
         self._derived_auth_service_name = None
         self._config = None
         self._credentials = None
         self._region = None
-        self._endpoint = None
+        self._endpoints = []
 
         self._http_handler = None
         self._file_logger_handler = None
         self._stream_logger_handler = None
 
-        self._http_scheme = "http"
-        self._https_scheme = "https"
-
     def with_http_config(self, config):
         """
         :param config: Config for ClientBuilder
         :type config: :class:`g42cloudsdkcore.http.http_config.HttpConfig`
         """
         self._config = config
         return self
@@ -90,15 +92,20 @@
         return self
 
     def with_endpoint(self, endpoint):
         """
         :param endpoint: Endpoint for ClientBuilder
         :type endpoint: str
         """
-        self._endpoint = endpoint
+        warnings.warn("As of 3.1.27, because of the support of the multi-endpoint feature, use with_endpoints instead",
+                      DeprecationWarning)
+        return self.with_endpoints([endpoint])
+
+    def with_endpoints(self, endpoints):
+        self._endpoints = endpoints
         return self
 
     def with_http_handler(self, http_handler):
         """
         :param http_handler: HttpHandler for ClientBuilder
         :type http_handler: :class:`g42cloudsdkcore.http.http_handler.HttpHandler`
         """
@@ -145,62 +152,62 @@
         if not self._credentials:
             raise ValueError("credential can not be None, %s credential objects are required"
                              % ",".join(self._credential_type))
         if self._credentials.__class__.__name__ not in self._credential_type:
             raise TypeError("credential type error, supported credential type is %s" % ",".join(self._credential_type))
 
         if self._region is not None:
-            self._endpoint = self._region.endpoint
+            self._endpoints += self._region.endpoints
             self._credentials = self._credentials.process_auth_params(client.get_http_client(), self._region.id)
 
             if isinstance(self._credentials, DerivedCredentials):
                 self._credentials._process_derived_auth_params(self._derived_auth_service_name, self._region.id)
 
-        if not self._endpoint.startswith(self._http_scheme):
-            self._endpoint = self._https_scheme + "://" + self._endpoint
+        if not self._endpoints:
+            raise ValueError("Could not find any endpoints, at least one endpoint is required")
+        self._endpoints = [endpoint if endpoint.startswith(self._HTTP_SCHEME) else self._HTTPS_SCHEME + "://" + endpoint
+                           for endpoint in self._endpoints]
 
-        client.with_endpoint(self._endpoint) \
-            .with_credentials(self._credentials)
+        client.with_endpoints(self._endpoints).with_credentials(self._credentials)
 
         if self._file_logger_handler is not None:
             client.add_file_logger(**self._file_logger_handler)
         if self._stream_logger_handler is not None:
             client.add_stream_logger(**self._stream_logger_handler)
 
         return client
 
 
 class Client(object):
     _CONTENT_TYPE = "Content-Type"
     _APPLICATION_JSON = "application/json"
     _APPLICATION_XML = "application/xml"
-    _MULTIPART_FORMDATA = "multipart/form-data"
+    _APPLICATION_OCTET_STREAM = "application/octet-stream"
+    _MULTIPART_FORM_DATA = "multipart/form-data"
     _XML_NAME = "xml_name"
     _AUTHORIZATION = "Authorization"
     _HEADERS = "headers"
 
     def __init__(self):
         self.preset_headers = {}
 
         self._agent = {"User-Agent": "g42cloud-usdk-python/3.0"}
         self._logger = self._init_logger()
 
         self._credentials = None
         self._config = None
-        self._endpoint = None
+        self._endpoint_index = 0
+        self._endpoints = []
+        self._mutex = threading.Lock()
 
         self._http_client = None
         self._http_handler = None
 
         self.model_package = None
-        try:
-            exception_handler_model_name = "%s.exception_handler" % self.__module__[:self.__module__.rindex('.')]
-            self.exception_handler_model = importlib.import_module(exception_handler_model_name)
-        except ImportError:
-            self.exception_handler_model = None
+        self.exception_handler = None
 
     @classmethod
     def _init_logger(cls):
         logger_name = 'G42Cloud-SDK-%s' % cls.__name__
         logger = logging.getLogger(logger_name)
         logger.propagate = False
         return logger
@@ -217,34 +224,34 @@
         """
         :param credentials: Credential for Client
         :type credentials: :class:`g42cloudsdkcore.auth.credentials.Credentials`
         """
         self._credentials = credentials
         return self
 
-    def with_endpoint(self, endpoint):
+    def with_endpoints(self, endpoints):
         """
-        :param endpoint: Endpoint for Client
-        :type endpoint: str
+        :param endpoints: Endpoint for Client
+        :type endpoints: str
         """
-        self._endpoint = endpoint
+        self._endpoints += endpoints
         return self
 
     def with_http_handler(self, http_handler):
         """
         :param http_handler: HttpHandler for Client
         :type http_handler: :class:`g42cloudsdkcore.http.http_handler.HttpHandler`
         """
         self._http_handler = http_handler if http_handler is not None else HttpHandler()
         return self
 
     def init_http_client(self):
-        exception_handler = None \
-            if self.exception_handler_model is None else getattr(self.exception_handler_model, "handle_exception")
-        self._http_client = HttpClient(self._config, self._http_handler, exception_handler, self._logger)
+        if not self.exception_handler or not isinstance(self.exception_handler, exception_handler.ExceptionHandler):
+            self.exception_handler = exception_handler.DefaultExceptionHandler()
+        self._http_client = HttpClient(self._config, self._http_handler, self.exception_handler, self._logger)
 
     def add_stream_logger(self, stream, log_level, format_string):
         self._logger.setLevel(log_level)
         stream_handler = logging.StreamHandler(stream)
         stream_handler.setLevel(log_level)
         formatter = logging.Formatter(format_string if format_string is not None else core_utils.LOG_FORMAT)
         stream_handler.setFormatter(formatter)
@@ -368,58 +375,78 @@
             return params
         elif type(params) == list:
             list_filter = filter(lambda x: type(x) == tuple and len(x) == 2 and x[1] is not None, params)
             return [i for i in list_filter]
         return None
 
     def _url_parse(self, cname):
-        parse_result = urlparse(self._endpoint)
+        parse_result = urlparse(self._endpoints[self._endpoint_index])
         if cname:
             endpoint = "%s://%s.%s" % (parse_result.scheme, cname, parse_result.netloc)
             parse_result = urlparse(endpoint)
         return parse_result
 
     def do_http_request(self, method, resource_path, path_params=None, query_params=None, header_params=None,
                         body=None, post_params=None, cname=None, response_type=None, response_headers=None,
                         collection_formats=None, request_type=None, async_request=False):
+
+        if async_request:
+            future_request = self.build_future_request(method, resource_path, path_params, query_params, header_params,
+                                                       body, post_params, cname, response_type, collection_formats)
+            future_response = self._http_client.executor.submit(self._do_http_request_async, future_request,
+                                                                response_type, response_headers)
+            return FutureSdkResponse(future_response, self._logger)
+
+        while True:
+            try:
+                request = self.build_future_request(method, resource_path, path_params, query_params, header_params,
+                                                    body, post_params, cname, response_type,
+                                                    collection_formats).result()
+                response = self._do_http_request_sync(request)
+                break
+            except HostUnreachableException as e:
+                with self._mutex:
+                    if self._endpoint_index < len(self._endpoints) - 1:
+                        self._endpoint_index += 1
+                    else:
+                        self._endpoint_index = 0
+                        raise e
+
+        return self.sync_response_handler(response, response_type, response_headers)
+
+    def build_future_request(self, method, resource_path, path_params, query_params, header_params,
+                             request_body, post_params, cname, response_type, collection_formats):
         url_parse_result = self._url_parse(cname)
         schema = url_parse_result.scheme
         host = url_parse_result.netloc
 
         header_params = self._parse_header_params(collection_formats, header_params)
         resource_path = self._parse_path_params(collection_formats, path_params, resource_path,
                                                 self._credentials.get_update_path_params())
         query_params = self._parse_query_params(collection_formats, query_params)
         post_params = self._parse_post_params(collection_formats, post_params)
 
         content_type = header_params.setdefault(self._CONTENT_TYPE, self._APPLICATION_JSON)
-        if content_type == self._MULTIPART_FORMDATA:
-            body = self._parse_formdata_body(body)
+        if content_type == self._MULTIPART_FORM_DATA:
+            body = self._parse_formdata_body(request_body)
             header_params[self._CONTENT_TYPE] = body.content_type
         elif content_type == self._APPLICATION_XML:
-            body = self._parse_xml_body(body)
+            body = self._parse_xml_body(request_body)
+        elif content_type == self._APPLICATION_OCTET_STREAM:
+            body = request_body
         else:
-            body = self._parse_body(body, post_params)
+            body = self._parse_body(request_body, post_params)
 
         stream = self._is_stream(response_type)
         sdk_request = SdkRequest(method=method, schema=schema, host=host, resource_path=resource_path,
                                  query_params=query_params, header_params=header_params, body=body, stream=stream)
         if self._AUTHORIZATION not in header_params:
-            future_request = self._credentials.process_auth_request(sdk_request, self._http_client)
-        else:
-            future_request = self._http_client.executor.submit(lambda: sdk_request)
-
-        if async_request:
-            future_response = self._http_client.executor.submit(self._do_http_request_async, future_request,
-                                                                response_type, response_headers)
-            return FutureSdkResponse(future_response, self._logger)
+            return self._credentials.process_auth_request(sdk_request, self._http_client)
         else:
-            request = future_request.result()
-            response = self._do_http_request_sync(request)
-            return self.sync_response_handler(response, response_type, response_headers)
+            return self._http_client.executor.submit(lambda: sdk_request)
 
     def _do_http_request_sync(self, request):
         response = self._http_client.do_request_sync(request)
         return response
 
     def _do_http_request_async(self, future_request, response_type, response_headers):
         request = future_request.result()
```

## g42cloudsdkcore/exceptions/exceptions.py

```diff
@@ -220,11 +220,12 @@
         self.err_message = err_message
 
     def __str__(self):
         return "RetryOutageException - %s" % self.err_message
 
 
 class SdkError(object):
-    def __init__(self, request_id=None, error_code=None, error_msg=None):
+    def __init__(self, request_id=None, error_code=None, error_msg=None, encoded_authorization_message=None):
         self.error_msg = error_msg
         self.error_code = error_code
         self.request_id = request_id
+        self.encoded_authorization_message = encoded_authorization_message
```

## g42cloudsdkcore/http/http_client.py

```diff
@@ -14,28 +14,25 @@
  software distributed under the LICENSE is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the LICENSE for the
  specific language governing permissions and limitations
  under the LICENSE.
 """
 
-import json
+from concurrent.futures import ThreadPoolExecutor
 
-import six
 import requests
 from requests import HTTPError, Timeout, TooManyRedirects
 from requests.adapters import HTTPAdapter
 from requests.exceptions import ConnectionError
 from requests.packages.urllib3.util import Retry
 from urllib3.exceptions import SSLError, NewConnectionError
-from concurrent.futures import ThreadPoolExecutor
 
 from g42cloudsdkcore.exceptions import exceptions
 from g42cloudsdkcore.http.future_session import FutureSession
-from g42cloudsdkcore.utils.xml_utils import XmlTransfer
 
 
 class HttpClient(object):
     def __init__(self, config, http_handler, exception_handler, logger):
         self._logger = logger
         self._exception_handler = exception_handler
         self._http_handler = http_handler
@@ -68,37 +65,41 @@
         return sdk_session
 
     @property
     def executor(self):
         return self._executor
 
     def do_request_sync(self, request):
-        fun = getattr(self._session, request.method.lower())
+        invoke = getattr(self._session, request.method.lower())
 
         try:
             if self._http_handler is not None:
                 self._http_handler.process_request(request=request, logger=self._logger)
-            response = fun(
-                "%s://%s%s" % (request.schema, request.host, request.uri),
+            url = "%s://%s%s" % (request.schema, request.host, request.uri)
+            response = invoke(
+                url,
                 timeout=self._timeout,
                 headers=request.header_params,
                 proxies=self._proxy,
                 verify=self._verify,
                 cert=self._cert,
                 data=request.body,
                 stream=request.stream
             )
         except ConnectionError as connectionError:
             for each in connectionError.args:
+                reason_str = str(each.reason)
                 if isinstance(each.reason, SSLError):
-                    self._logger.error("SslHandShakeException occurred. %s" % str(each.reason))
-                    raise exceptions.SslHandShakeException(str(each.reason))
+                    self._logger.error("SslHandShakeException occurred. %s" % reason_str)
+                    raise exceptions.SslHandShakeException(reason_str)
                 if isinstance(each.reason, NewConnectionError):
-                    self._logger.error("ConnectionException occurred. %s" % str(each.reason))
-                    raise exceptions.ConnectionException(str(each.reason))
+                    if reason_str.endswith("getaddrinfo failed") or reason_str.endswith("Name or service not known"):
+                        raise exceptions.HostUnreachableException(reason_str)
+                    self._logger.error("ConnectionException occurred. %s" % reason_str)
+                    raise exceptions.ConnectionException(reason_str)
             self._logger.error("ConnectionException occurred. %s" % str(connectionError))
             raise exceptions.ConnectionException(str(connectionError))
 
         self.response_error_hook_factory()(response)
         return response
 
     def do_request_async(self, request, hooks):
@@ -122,75 +123,18 @@
         def response_hook(resp, *args, **kwargs):
             if self._http_handler is not None:
                 self._http_handler.process_response(response=resp, logger=self._logger)
 
             try:
                 resp.raise_for_status()
             except HTTPError as httpError:
-                sdk_error = self._get_sdk_error_from_xml_response(httpError.response) \
-                    if httpError.response.headers.get("Content-Type") == "application/xml" \
-                    else self._get_sdk_error_from_response(httpError.response)
+                sdk_error = self._exception_handler.handle_exception(httpError.request, httpError.response)
                 if 400 <= httpError.response.status_code < 500:
                     raise exceptions.ClientRequestException(httpError.response.status_code, sdk_error)
                 else:
                     raise exceptions.ServerResponseException(httpError.response.status_code, sdk_error)
             except Timeout as timeout:
                 raise exceptions.CallTimeoutException(str(timeout))
             except TooManyRedirects as tooManyRedirects:
                 raise exceptions.RetryOutageException(str(tooManyRedirects))
 
         return response_hook
-
-    def _get_sdk_error_from_xml_response(self, resp):
-        request_id = resp.headers.get("x-obs-request-id")
-        sdk_error = exceptions.SdkError(request_id=request_id)
-        try:
-            sdk_error_dict = XmlTransfer().to_dict(resp.text, ignore_root=True)
-            self._process_sdk_error_from_xml(sdk_error, sdk_error_dict)
-        except Exception:
-            sdk_error.error_msg = six.ensure_str(resp.text)
-            raise exceptions.ServerResponseException(resp.status_code, sdk_error)
-
-        return self._handle_sdk_error_msg(sdk_error, resp.text)
-
-    @classmethod
-    def _process_sdk_error_from_xml(cls, sdk_error, sdk_error_dict):
-        if not sdk_error.request_id:
-            sdk_error.request_id = sdk_error_dict.get("RequestId")
-        if "Code" in sdk_error_dict and "Message" in sdk_error_dict:
-            sdk_error.error_code = sdk_error_dict.get("Code")
-            sdk_error.error_msg = sdk_error_dict.get("Message")
-
-    def _get_sdk_error_from_response(self, resp):
-        request_id = resp.headers.get("X-Request-Id")
-        sdk_error = exceptions.SdkError(request_id=request_id)
-        try:
-            sdk_error_dict = json.loads(resp.text)
-            self._process_sdk_error(sdk_error, sdk_error_dict)
-        except Exception:
-            sdk_error.error_msg = six.ensure_str(resp.text)
-            raise exceptions.ServerResponseException(resp.status_code, sdk_error)
-
-        return self._handle_sdk_error_msg(sdk_error, resp.text)
-
-    def _handle_sdk_error_msg(self, sdk_error, response_body):
-        if sdk_error.error_msg:
-            return sdk_error
-        if not sdk_error.error_msg and self._exception_handler:
-            sdk_error = self._exception_handler(response_body)
-        if not sdk_error.error_msg:
-            sdk_error = exceptions.SdkError(error_msg=response_body)
-        return sdk_error
-
-    @classmethod
-    def _process_sdk_error(cls, sdk_error, sdk_error_dict):
-        if "error_code" in sdk_error_dict and "error_msg" in sdk_error_dict:
-            sdk_error.error_code = sdk_error_dict.get("error_code")
-            sdk_error.error_msg = sdk_error_dict.get("error_msg")
-        elif "code" in sdk_error_dict and "message" in sdk_error_dict:
-            sdk_error.error_code = sdk_error_dict.get("code")
-            sdk_error.error_msg = sdk_error_dict.get("message")
-        else:
-            for value in sdk_error_dict.values():
-                if not isinstance(value, dict):
-                    continue
-                cls._process_sdk_error(sdk_error, value)
```

## g42cloudsdkcore/region/region.py

```diff
@@ -14,37 +14,78 @@
  software distributed under the LICENSE is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the LICENSE for the
  specific language governing permissions and limitations
  under the LICENSE.
 """
 
+import warnings
+
 
 class Region(object):
-    def __init__(self, id=None, endpoint=None):
+    def __init__(self, *args, **kwargs):
+        """
+        There are two ways to initialize the region object.
+
+        In the first way, only one region and one endpoint can be specified.
+        region1 = Region(id="region-id", endpoint="region-endpoint")
+
+        In the second way, one region and multiple endpoints can be specified.
+        region2 = Region("region-id", "endpoint1", "endpoint2")
+
+        It is not recommended to mix the two initialization ways.
+        If two initialization ways are mixed, the first way has priority over the second.
+        """
         self._id = None
-        self._endpoint = None
+        self._endpoints = None
 
-        if id is not None:
-            self.id = id
-        if endpoint is not None:
-            self.endpoint = endpoint
+        if len(args) > 1:
+            self._id = args[0]
+            self._endpoints = list(args[1:])
+
+        if kwargs:
+            if "id" in kwargs:
+                self._id = kwargs.get("id")
+            if "endpoint" in kwargs:
+                self._endpoints = [kwargs.get("endpoint")]
+
+        if not self._id:
+            raise ValueError("id is required")
+        if not self.endpoints:
+            raise ValueError("at lease one endpoint is required")
 
     @property
     def id(self):
         return self._id
 
     @id.setter
-    def id(self, id):
-        self._id = id
+    def id(self, _id):
+        self._id = _id
 
     @property
     def endpoint(self):
-        return self._endpoint
+        warnings.warn("As of 3.1.27, because of the support of the multi-endpoint feature, use endpoints instead",
+                      DeprecationWarning)
+        return self.endpoints[0] if self.endpoints else None
 
     @endpoint.setter
     def endpoint(self, endpoint):
-        self._endpoint = endpoint
+        warnings.warn("As of 3.1.27, because of the support of the multi-endpoint feature, use endpoints instead",
+                      DeprecationWarning)
+        self.endpoints = [endpoint]
+
+    @property
+    def endpoints(self):
+        return self._endpoints
+
+    @endpoints.setter
+    def endpoints(self, endpoints):
+        self._endpoints = endpoints
 
     def with_endpoint_override(self, endpoint):
-        self._endpoint = endpoint
+        warnings.warn("As of 3.1.27, because of the support of the multi-endpoint feature,"
+                      "use with_endpoints_override instead", DeprecationWarning)
+        return self.with_endpoints_override([endpoint])
+
+    def with_endpoints_override(self, endpoints):
+        self.endpoints = endpoints
         return self
```

## g42cloudsdkcore/signer/signer.py

```diff
@@ -42,15 +42,22 @@
     HeaderAuthorization = "Authorization"
     HeaderContentSha256 = "X-Sdk-Content-Sha256"
 
     def __init__(self, credentials):
         self._ak = credentials.ak
         self._sk = credentials.sk
 
+    def _verify_required(self):
+        if not self._ak:
+            raise ValueError("ak is required in credentials")
+        if not self._sk:
+            raise ValueError("sk is required in credentials")
+
     def sign(self, request):
+        self._verify_required()
         if isinstance(request.body, six.text_type):
             request.body = six.ensure_binary(request.body)
 
         t = self.process_header_time(request)
         self.process_header_host(request)
 
         signed_headers = self.process_signed_headers(request)
@@ -229,14 +236,20 @@
 
     @classmethod
     def process_auth_header_value(cls, signature, app_key, signed_headers, info=None):
         return "%s Credential=%s/%s, SignedHeaders=%s, Signature=%s" % (
             cls.Algorithm, app_key, info, ";".join(signed_headers), signature)
 
     def sign(self, request, derived_auth_service_name=None, region_id=None):
+        super(DerivationAKSKSigner, self)._verify_required()
+        if not derived_auth_service_name:
+            raise ValueError("derivedAuthServiceName is required in credentials when using derived auth")
+        if not region_id:
+            raise ValueError("regionId is required in credentials when using derived auth")
+
         request.body = six.ensure_binary(request.body)
 
         t = self.process_header_time(request)
         self.process_header_host(request)
 
         signed_headers = self.process_signed_headers(request)
         canonical_request = self.process_canonical_request(request, signed_headers)
@@ -247,8 +260,7 @@
         signature = self.sign_string_to_sign(string_to_sign, derivation_key)
         auth_value = self.process_auth_header_value(signature, self._ak, signed_headers, info_str)
         request.header_params[self.HeaderAuthorization] = auth_value
 
         self.process_request_uri(request)
 
         return request
-
```

## Comparing `g42cloudsdkcore-0.0.4b0.dist-info/LICENSE` & `g42cloudsdkcore-0.0.5b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `g42cloudsdkcore-0.0.4b0.dist-info/METADATA` & `g42cloudsdkcore-0.0.5b0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g42cloudsdkcore
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: G42Cloud SDK Python Core
 Home-page: https://github.com/g42cloud-sdk/g42cloud-sdk-python
 Author: G42Cloud SDK
 Author-email: unionsdk@outlook.com
 License: Apache LICENSE 2.0
 Keywords: g42cloud,sdk,core
 Platform: any
```

