# Comparing `tmp/hagis-0.1.4.tar.gz` & `tmp/hagis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.1.4.tar", last modified: Fri Apr 14 01:32:29 2023, max compression
+gzip compressed data, was "hagis-0.2.0.tar", last modified: Fri Apr 14 11:32:14 2023, max compression
```

## Comparing `hagis-0.1.4.tar` & `hagis-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.728299 hagis-0.1.4/
--rw-rw-rw-   0        0        0      958 2023-04-14 01:32:29.728299 hagis-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.682832 hagis-0.1.4/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.1.4/hagis/__init__.py
--rw-rw-rw-   0        0        0     8731 2023-04-14 01:10:13.000000 hagis-0.1.4/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.720400 hagis-0.1.4/hagis.egg-info/
--rw-rw-rw-   0        0        0      958 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-14 01:31:42.000000 hagis-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 01:32:29.728299 hagis-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.963352 hagis-0.2.0/
+-rw-rw-rw-   0        0        0      958 2023-04-14 11:32:14.955397 hagis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.915308 hagis-0.2.0/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.0/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8620 2023-04-14 11:28:06.000000 hagis-0.2.0/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.955397 hagis-0.2.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-14 11:31:43.000000 hagis-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:32:14.963352 hagis-0.2.0/setup.cfg
```

### Comparing `hagis-0.1.4/PKG-INFO` & `hagis-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.4
+Version: 0.2.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.1.4/hagis/hagis.py` & `hagis-0.2.0/hagis/hagis.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from json import dumps, loads
 from requests import post
 from types import SimpleNamespace
 from typing import Any, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
 
 T = TypeVar("T")
 
-class Mapper(Generic[T]):
+class Layer(Generic[T]):
     """ 
 
     Args:
         Generic (T): Type argument.
         AttGeoBase: Base class.
     """
 
-    def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace, oid_field: str = "objectid", shape_property_name: str = "shape", mapping: Optional[Dict[str, str]] = None) -> None:
+    def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace, oid_field: str = "objectid", shape_property_name: str = "shape", **mapping: str) -> None:
         """ Creates a new instance of the AttGeo class.
 
         Args:
             layer_url (str): Layer url (e.g. .../FeatureServer/0).
             model (Type[T], optional): Model to map to.  Defaults to SimpleNamespace.
             oid_field (str, optional): Name of the Object ID field.  Defaults to "objectid".
             shape_property_name (str, optional): Name of the shape property.  Defaults to "shape".
@@ -32,34 +32,33 @@
         self._fields: Dict[str, str] = {}
         self._is_dynamic = model == SimpleNamespace
 
         if self._is_dynamic:
             return
         
         # List of custom mapping properties that have been handled.
-        custom_mapping = {} if mapping is None else mapping
         mapped: List[str] = []
 
         for type in reversed(model.__mro__):
             if hasattr(type, "__annotations__"):
                 for property_name, property_type in type.__annotations__.items():
                     key = property_name.lower()
 
-                    if property_name in custom_mapping:
-                        self._fields[key] = custom_mapping[property_name]
+                    if property_name in mapping:
+                        self._fields[key] = mapping[property_name]
                         mapped.append(property_name)
                     else:
                         self._fields[key] = property_name
 
                     if key == shape_property_name.lower():
                         self._shape_property_name = property_name
                         self._shape_property_type = property_type
 
         # Add custom properties that have not been handled as dynamically handled propeties.
-        for (property, field) in custom_mapping.items():
+        for property, field in mapping.items():
             if property not in mapped:
                 self._fields[property.lower()] = field
 
     def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterator[T]:
         """ Queries the feature layer and yields the results as typed objects.
 
         Args:
```

### Comparing `hagis-0.1.4/hagis.egg-info/PKG-INFO` & `hagis-0.2.0/hagis.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.4
+Version: 0.2.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.1.4/pyproject.toml` & `hagis-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

