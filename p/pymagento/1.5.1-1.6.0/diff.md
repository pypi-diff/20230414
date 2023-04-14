# Comparing `tmp/pymagento-1.5.1.tar.gz` & `tmp/pymagento-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.5.1.tar", max compression
+gzip compressed data, was "pymagento-1.6.0.tar", max compression
```

## Comparing `pymagento-1.5.1.tar` & `pymagento-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-04 11:57:03.660945 pymagento-1.5.1/LICENSE
--rw-r--r--   0        0        0      908 2023-04-04 11:57:03.660945 pymagento-1.5.1/README.md
--rw-r--r--   0        0        0     1215 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/__init__.py
--rw-r--r--   0        0        0     4743 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/batches.py
--rw-r--r--   0        0        0    36027 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/client.py
--rw-r--r--   0        0        0     1768 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/queries.py
--rw-r--r--   0        0        0      357 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/types.py
--rw-r--r--   0        0        0       22 2023-04-04 11:57:03.660945 pymagento-1.5.1/magento/version.py
--rw-r--r--   0        0        0     1219 2023-04-04 11:57:03.660945 pymagento-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 pymagento-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-14 13:08:03.926197 pymagento-1.6.0/LICENSE
+-rw-r--r--   0        0        0      908 2023-04-14 13:08:03.926197 pymagento-1.6.0/README.md
+-rw-r--r--   0        0        0     1189 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/__init__.py
+-rw-r--r--   0        0        0     4645 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/batches.py
+-rw-r--r--   0        0        0    35623 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/types.py
+-rw-r--r--   0        0        0       22 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-04-14 13:08:03.930197 pymagento-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 pymagento-1.6.0/PKG-INFO
```

### Comparing `pymagento-1.5.1/LICENSE` & `pymagento-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/README.md` & `pymagento-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/magento/__init__.py` & `pymagento-1.6.0/magento/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from magento.attributes import (
     get_custom_attribute, get_boolean_custom_attribute, get_custom_attributes_dict,
-    pretty_custom_attributes, set_custom_attribute, set_custom_attributes, serialize_attribute_value
+    set_custom_attribute, set_custom_attributes, serialize_attribute_value
 )
 from magento.client import Magento
 from magento.exceptions import MagentoException, MagentoAssertionError
 from magento.order_helpers import is_order_on_hold, is_order_cash_on_delivery, get_order_shipping_address
 from magento.queries import Query, make_field_value_query, make_search_query
 from magento.version import __version__
```

### Comparing `pymagento-1.5.1/magento/attributes.py` & `pymagento-1.6.0/magento/attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 """
 Custom attributes utilities.
 """
 from collections import OrderedDict
 from typing import Callable, Optional, cast, Dict, Any, Union, Sequence, List, Tuple, Iterable, \
-    OrderedDict as OrderedDictType
+    OrderedDict as OrderedDictType, overload, TypeVar
 
+T = TypeVar('T')
 
-def get_custom_attribute(item: dict, attribute_code: str, coerce_as: Optional[Callable] = None):
+
+@overload
+def get_custom_attribute(item: dict, attribute_code: str,
+                         coerce_as: Callable[[str], T]) -> Optional[T]:
+    ...
+
+
+@overload
+def get_custom_attribute(item: dict, attribute_code: str) -> Optional[str]:
+    ...
+
+
+def get_custom_attribute(item, attribute_code, coerce_as=None):
     """
     Get a custom attribute from an item given its code.
 
     For example:
         >>> get_custom_attribute(..., "my_custom_attribute")
         "0"
 
@@ -28,14 +41,15 @@
             value = attribute["value"]
             if coerce_as:
                 if coerce_as == bool:
                     # "0" -> False / "1" -> True
                     return bool(int(value))
                 return coerce_as(value)
             return value
+    return None
 
 
 def get_boolean_custom_attribute(item: dict, attribute_code: str) -> Optional[bool]:
     """
     Equivalent of ``get_custom_attribute(item, attribute_code, coerce_as=bool)`` with proper typing.
     """
     return cast(Optional[bool], get_custom_attribute(item, attribute_code, coerce_as=bool))
@@ -48,22 +62,14 @@
     d = OrderedDict()
     for attribute in item.get("custom_attributes", []):
         d[attribute["attribute_code"]] = attribute["value"]
 
     return d
 
 
-def pretty_custom_attributes(custom_attributes: List[Dict[str, Any]]):  # pragma: nocover
-    """
-    [Deprecated] Return a human-friendly compact representation of a sequence of custom attributes.
-    """
-    attributes = get_custom_attributes_dict({"custom_attributes": custom_attributes})
-    return ", ".join(f"{k}={repr(v)}" for k, v in attributes.items())
-
-
 def serialize_attribute_value(value: Union[str, int, float, bool, None], force_none=False):
     """
     Serialize a value to be stored in a Magento attribute.
     """
     if isinstance(value, bool):
         return "1" if value else "0"
     elif value is None:
```

### Comparing `pymagento-1.5.1/magento/batches.py` & `pymagento-1.6.0/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/magento/client.py` & `pymagento-1.6.0/magento/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,46 +92,40 @@
     def __init__(self,
                  token: Optional[str] = None,
                  base_url: Optional[str] = None,
                  scope: Optional[str] = None,
                  logger: Optional[Logger] = None,
                  read_only=False,
                  user_agent=None,
-                 verbose=False,
-                 # Deprecated
-                 log_progress=False):
+                 verbose=False):
         """
         Create a Magento client instance. All arguments are optional and fall back on environment variables named
         ``PYMAGENTO_ + argument.upper()`` (``PYMAGENTO_TOKEN``, ``PYMAGENTO_BASE_URL``, etc).
         The ``token`` and ``base_url`` **must** be given either as arguments or environment variables.
 
         :param token: API integration token
         :param base_url: base URL of the Magento instance
         :param scope: API scope
         :param logger: optional logger.
         :param verbose: if True, log the progress of get_paginated. This has no effect if logger is not set.
         :param read_only: if True,
         :param user_agent: User-Agent
-        :param log_progress: deprecated alias for `verbose`.
         """
         token = token or environ.get("PYMAGENTO_TOKEN")
         base_url = base_url or environ.get("PYMAGENTO_BASE_URL")
         scope = scope or environ.get("PYMAGENTO_SCOPE") or DEFAULT_SCOPE
         user_agent = user_agent or environ.get("PYMAGENTO_USER_AGENT") or USER_AGENT
 
         if token is None:
             raise RuntimeError("Missing API token")
         if base_url is None:
             raise RuntimeError("Missing API base URL")
 
         super().__init__(base_url=base_url, user_agent=user_agent, read_only=read_only)
 
-        if log_progress:
-            verbose = True
-
         self.scope = scope
         self.logger = logger
         self.verbose = verbose if logger else False
         self.headers['Authorization'] = f"Bearer {token}"
 
     # Attributes
     # ==========
@@ -641,20 +635,14 @@
 
         :param product_updates: sequence of product data dicts. They MUST contain an 'sku' key.
         :return:
         """
         payload = [{"product": product_update} for product_update in product_updates]
         return self.put_api('/V1/products/bySku', json=payload, throw=True, async_bulk=True).json()
 
-    def get_product_source_items(self, sku) -> Iterable[SourceItem]:
-        """
-        Deprecated. Use `.get_source_items(sku=sku)` instead, which is equivalent.
-        """
-        return self.get_source_items(sku=sku)
-
     def set_product_stock_item(self, sku: Sku, quantity: int, is_in_stock=1):
         """
         :param sku:
         :param quantity:
         :param is_in_stock:
         :return: requests.Response
         """
```

### Comparing `pymagento-1.5.1/magento/exceptions.py` & `pymagento-1.6.0/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/magento/order_helpers.py` & `pymagento-1.6.0/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/magento/queries.py` & `pymagento-1.6.0/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.5.1/pyproject.toml` & `pymagento-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.5.1"
+version = "1.6.0"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.5.1/PKG-INFO` & `pymagento-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

