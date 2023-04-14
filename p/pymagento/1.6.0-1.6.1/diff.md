# Comparing `tmp/pymagento-1.6.0.tar.gz` & `tmp/pymagento-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.6.0.tar", max compression
+gzip compressed data, was "pymagento-1.6.1.tar", max compression
```

## Comparing `pymagento-1.6.0.tar` & `pymagento-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-14 13:08:03.926197 pymagento-1.6.0/LICENSE
--rw-r--r--   0        0        0      908 2023-04-14 13:08:03.926197 pymagento-1.6.0/README.md
--rw-r--r--   0        0        0     1189 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/__init__.py
--rw-r--r--   0        0        0     4645 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/batches.py
--rw-r--r--   0        0        0    35623 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/client.py
--rw-r--r--   0        0        0     1768 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/queries.py
--rw-r--r--   0        0        0      357 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/types.py
--rw-r--r--   0        0        0       22 2023-04-14 13:08:03.930197 pymagento-1.6.0/magento/version.py
--rw-r--r--   0        0        0     1219 2023-04-14 13:08:03.930197 pymagento-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 pymagento-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-14 13:46:01.789723 pymagento-1.6.1/LICENSE
+-rw-r--r--   0        0        0      908 2023-04-14 13:46:01.789723 pymagento-1.6.1/README.md
+-rw-r--r--   0        0        0     1189 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/batches.py
+-rw-r--r--   0        0        0    35623 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/types.py
+-rw-r--r--   0        0        0       22 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-04-14 13:46:01.793723 pymagento-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 pymagento-1.6.1/PKG-INFO
```

### Comparing `pymagento-1.6.0/LICENSE` & `pymagento-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/README.md` & `pymagento-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/__init__.py` & `pymagento-1.6.1/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/attributes.py` & `pymagento-1.6.1/magento/attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     OrderedDict as OrderedDictType, overload, TypeVar
 
 T = TypeVar('T')
 
 
 @overload
 def get_custom_attribute(item: dict, attribute_code: str,
-                         coerce_as: Callable[[str], T]) -> Optional[T]:
+                         coerce_as: Callable[[str], T]) -> Union[None, T, List[T]]:
     ...
 
 
 @overload
-def get_custom_attribute(item: dict, attribute_code: str) -> Optional[str]:
+def get_custom_attribute(item: dict, attribute_code: str) -> Union[None, str, List[str]]:
     ...
 
 
 def get_custom_attribute(item, attribute_code, coerce_as=None):
     """
     Get a custom attribute from an item given its code.
 
@@ -32,23 +32,28 @@
 
     :param item:
     :param attribute_code:
     :param coerce_as: optional callable that is called on the attribute value if it's set.
       This is useful to circumvent Magento's limitation where all attribute values are strings.
     :return: attribute value or None.
     """
+    if coerce_as == bool:
+        # "0" -> False / "1" -> True
+        coerce_as = lambda s: bool(int(s))
+
     for attribute in item.get("custom_attributes", []):
         if attribute["attribute_code"] == attribute_code:
-            value = attribute["value"]
-            if coerce_as:
-                if coerce_as == bool:
-                    # "0" -> False / "1" -> True
-                    return bool(int(value))
-                return coerce_as(value)
-            return value
+            value: Union[str, List[str]] = attribute["value"]
+            if coerce_as is None:
+                return value
+
+            if isinstance(value, list):
+                return [coerce_as(s) for s in value]
+
+            return coerce_as(value)
     return None
 
 
 def get_boolean_custom_attribute(item: dict, attribute_code: str) -> Optional[bool]:
     """
     Equivalent of ``get_custom_attribute(item, attribute_code, coerce_as=bool)`` with proper typing.
     """
```

### Comparing `pymagento-1.6.0/magento/batches.py` & `pymagento-1.6.1/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/client.py` & `pymagento-1.6.1/magento/client.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/exceptions.py` & `pymagento-1.6.1/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/order_helpers.py` & `pymagento-1.6.1/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/magento/queries.py` & `pymagento-1.6.1/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.0/pyproject.toml` & `pymagento-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.6.0"
+version = "1.6.1"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.6.0/PKG-INFO` & `pymagento-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

