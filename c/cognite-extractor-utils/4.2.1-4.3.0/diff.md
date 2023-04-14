# Comparing `tmp/cognite_extractor_utils-4.2.1.tar.gz` & `tmp/cognite_extractor_utils-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-4.2.1.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-4.3.0.tar", max compression
```

## Comparing `cognite_extractor_utils-4.2.1.tar` & `cognite_extractor_utils-4.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10173 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/LICENSE
--rw-r--r--   0        0        0     4091 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/README.md
--rw-r--r--   0        0        0      739 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1431 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0     3954 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/authentication.py
--rw-r--r--   0        0        0    15891 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/base.py
--rw-r--r--   0        0        0    30025 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/configtools.py
--rw-r--r--   0        0        0     1061 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0     4528 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/extraction_pipelines.py
--rw-r--r--   0        0        0     1003 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/logging_prometheus.py
--rw-r--r--   0        0        0    14598 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1005 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0     2853 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/retry.py
--rw-r--r--   0        0        0    17450 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     2083 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/throttle.py
--rw-r--r--   0        0        0    54282 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader.py
--rw-r--r--   0        0        0     7405 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0     5588 2023-03-30 10:29:28.016180 cognite_extractor_utils-4.2.1/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2073 2023-03-30 10:29:28.020180 cognite_extractor_utils-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 cognite_extractor_utils-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/LICENSE
+-rw-r--r--   0        0        0     4091 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/README.md
+-rw-r--r--   0        0        0      739 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1431 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0     3954 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/authentication.py
+-rw-r--r--   0        0        0    15891 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0    32146 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/configtools.py
+-rw-r--r--   0        0        0     1061 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0     4528 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/extraction_pipelines.py
+-rw-r--r--   0        0        0     1003 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/logging_prometheus.py
+-rw-r--r--   0        0        0    14598 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1005 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0     2853 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/retry.py
+-rw-r--r--   0        0        0    17450 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     2083 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/throttle.py
+-rw-r--r--   0        0        0    54282 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader.py
+-rw-r--r--   0        0        0     7405 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0     5588 2023-04-14 07:52:41.942182 cognite_extractor_utils-4.3.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2073 2023-04-14 07:52:41.946182 cognite_extractor_utils-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 cognite_extractor_utils-4.3.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-4.2.1/LICENSE` & `cognite_extractor_utils-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/README.md` & `cognite_extractor_utils-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "4.0.1"
+__version__ = "4.3.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/authentication.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/authentication.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/base.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/configtools.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/configtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,14 +245,92 @@
     def __str__(self) -> str:
         return self._expression
 
     def __repr__(self) -> str:
         return self._expression
 
 
+class FileSizeConfig(yaml.YAMLObject):
+    def __init__(self, expression):
+        self._bytes, self._expression = FileSizeConfig._parse_expression(expression)
+
+    @classmethod
+    def _parse_expression(cls, expression: str) -> Tuple[int, str]:
+        # First, try to parse pure number and assume bytes
+        try:
+            return int(expression), f"{expression}s"
+        except ValueError:
+            pass
+
+        sizes = {
+            "kb": 1000,
+            "mb": 1_000_000,
+            "gb": 1_000_000_000,
+            "tb": 1_000_000_000_000,
+            "kib": 1024,
+            "mib": 1_048_576,  # 1024 ^ 2
+            "gib": 1_073_741_824,  # 1024 ^ 3
+            "tib": 1_099_511_627_776,  # 1024 ^ 4
+        }
+        expression_lower = expression.lower()
+        for size in sizes:
+            if expression_lower.endswith(size):
+                return int(float(expression_lower.replace(size, "")) * sizes[size]), expression
+        else:
+            raise InvalidConfigError(f"Invalid unit for file size: {expression}. Valid units: {sizes.keys()}")
+
+    @property
+    def bytes(self) -> int:
+        return self._bytes
+
+    @property
+    def kilobytes(self) -> float:
+        return self._bytes / 1000
+
+    @property
+    def megabytes(self) -> float:
+        return self._bytes / 1_000_000
+
+    @property
+    def gigabytes(self) -> float:
+        return self._bytes / 1_000_000_000
+
+    @property
+    def terabytes(self) -> float:
+        return self._bytes / 1_000_000_000_000
+
+    @property
+    def kibibytes(self) -> float:
+        return self._bytes / 1024
+
+    @property
+    def mebibytes(self) -> float:
+        return self._bytes / 1_048_576
+
+    @property
+    def gibibytes(self) -> float:
+        return self._bytes / 1_073_741_824
+
+    @property
+    def tebibytes(self) -> float:
+        return self._bytes / 1_099_511_627_776
+
+    def __int__(self) -> int:
+        return int(self._bytes)
+
+    def __float__(self) -> float:
+        return float(self._bytes)
+
+    def __str__(self) -> str:
+        return self._expression
+
+    def __repr__(self) -> str:
+        return self._expression
+
+
 def _load_certificate_data(cert_path: str, password: Optional[str]) -> Tuple[str, str]:
     path = Path(cert_path)
     cert_data = Path(path).read_bytes()
 
     if path.suffix == ".pem":
         cert = load_pem_x509_certificate(cert_data)
         private_key = serialization.load_pem_private_key(cert_data, password=password.encode() if password else None)
```

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/extraction_pipelines.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/extraction_pipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/logging_prometheus.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/logging_prometheus.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/retry.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/retry.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/throttle.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/throttle.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/cognite/extractorutils/util.py` & `cognite_extractor_utils-4.3.0/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.2.1/pyproject.toml` & `cognite_extractor_utils-4.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "4.2.1"
+version = "4.3.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
```

### Comparing `cognite_extractor_utils-4.2.1/PKG-INFO` & `cognite_extractor_utils-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 4.2.1
+Version: 4.3.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 4.2.1 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 4.3.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

