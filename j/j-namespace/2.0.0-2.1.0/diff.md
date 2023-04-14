# Comparing `tmp/j-namespace-2.0.0.tar.gz` & `tmp/j-namespace-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "j-namespace-2.0.0.tar", last modified: Sun Mar 26 10:40:00 2023, max compression
+gzip compressed data, was "j-namespace-2.1.0.tar", last modified: Fri Apr 14 14:07:15 2023, max compression
```

## Comparing `j-namespace-2.0.0.tar` & `j-namespace-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 10:40:00.215163 j-namespace-2.0.0/
--rw-rw-rw-   0        0        0      158 2023-03-26 10:40:00.214669 j-namespace-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-26 10:40:00.203491 j-namespace-2.0.0/j_namespace.egg-info/
--rw-rw-rw-   0        0        0      158 2023-03-26 10:40:00.000000 j-namespace-2.0.0/j_namespace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-03-26 10:40:00.000000 j-namespace-2.0.0/j_namespace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 10:40:00.000000 j-namespace-2.0.0/j_namespace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-26 10:40:00.000000 j-namespace-2.0.0/j_namespace.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-26 10:40:00.204317 j-namespace-2.0.0/namespace/
--rw-rw-rw-   0        0        0       73 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 10:40:00.207721 j-namespace-2.0.0/namespace/source/
--rw-rw-rw-   0        0        0       76 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/source/__init__.py
--rw-rw-rw-   0        0        0     3743 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/source/namespace.py
--rw-rw-rw-   0        0        0     4408 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/source/pretty_dict.py
-drwxrwxrwx   0        0        0        0 2023-03-26 10:40:00.213179 j-namespace-2.0.0/namespace/tests/
--rw-rw-rw-   0        0        0       42 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/tests/__init__.py
--rw-rw-rw-   0        0        0     1593 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/tests/fixtures.py
--rw-rw-rw-   0        0        0     1933 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/tests/test_namespace.py
--rw-rw-rw-   0        0        0      116 2023-03-26 10:38:09.000000 j-namespace-2.0.0/namespace/tests/test_pretty_dict.py
--rw-rw-rw-   0        0        0       42 2023-03-26 10:40:00.215659 j-namespace-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-03-26 10:38:09.000000 j-namespace-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:07:15.160896 j-namespace-2.1.0/
+-rw-rw-rw-   0        0        0      158 2023-04-14 14:07:15.160400 j-namespace-2.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 14:07:15.135236 j-namespace-2.1.0/j_namespace.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-04-14 14:07:15.000000 j-namespace-2.1.0/j_namespace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-14 14:07:15.000000 j-namespace-2.1.0/j_namespace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:07:15.000000 j-namespace-2.1.0/j_namespace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 14:07:15.000000 j-namespace-2.1.0/j_namespace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:07:15.140691 j-namespace-2.1.0/namespace/
+-rw-rw-rw-   0        0        0       73 2023-03-26 10:43:32.000000 j-namespace-2.1.0/namespace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:07:15.144671 j-namespace-2.1.0/namespace/source/
+-rw-rw-rw-   0        0        0       76 2023-03-26 10:43:32.000000 j-namespace-2.1.0/namespace/source/__init__.py
+-rw-rw-rw-   0        0        0     3685 2023-04-14 14:03:09.000000 j-namespace-2.1.0/namespace/source/namespace.py
+-rw-rw-rw-   0        0        0     4510 2023-04-01 17:13:41.000000 j-namespace-2.1.0/namespace/source/pretty_dict.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:07:15.159407 j-namespace-2.1.0/namespace/tests/
+-rw-rw-rw-   0        0        0       42 2023-03-26 10:43:32.000000 j-namespace-2.1.0/namespace/tests/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-03-26 10:43:32.000000 j-namespace-2.1.0/namespace/tests/fixtures.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 13:59:41.000000 j-namespace-2.1.0/namespace/tests/test_namespace.py
+-rw-rw-rw-   0        0        0      116 2023-03-26 10:43:32.000000 j-namespace-2.1.0/namespace/tests/test_pretty_dict.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:07:15.160896 j-namespace-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-04-14 14:06:29.000000 j-namespace-2.1.0/setup.py
```

### Comparing `j-namespace-2.0.0/namespace/source/namespace.py` & `j-namespace-2.1.0/namespace/source/namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,28 @@
   """
   Unified data format.
   Enabled access of elements with both attribute syntax and dictionary syntax.
   Provides methods for loading and dumping into serial formats.
   Easy way for pretty printing of complex structures.
   """
 
-  def __init__(self, **data):
+  def __init__(self, data):
     """
-    Creates a namespace with all keyword parameters as elements
+    Creates a namespace from a dictionary.
     """
-    super().__init__(**data)
+    super().__init__(data)
 
   # alternative constructors
 
   @classmethod
-  def Dict(cls, data):
+  def Kwargs(cls, **kwargs):
     """
-    Creates a namespace with all elements from the dictionary
-    (no recursive traversing)
+    Creates a flat namespace with all keyword arguments as elements.
     """
-    obj = cls(**data)
-    return obj
+    return cls(kwargs)
 
   @classmethod
   def Recursive(cls, data, _parents=None):
     """
     Creates a namespace with recursive traversing. This means that nested dictionaries and objects
     will also be converted to a namespace. Including the ones that are inside iterables.
     Input can be either an object or a dictionary.
@@ -57,15 +55,15 @@
       if isinstance(val, TYPES["iterables"]):
         properties[key] = []
         for entry in val:
           properties[key] += [convert(entry)]
         properties[key] = type(val)(properties[key])
         continue
       properties[key] = convert(val)
-    obj.__init__(**properties)
+    obj.__init__(properties)
     return obj
 
   # object attribute syntax support
 
   def __getattr__(self, item):
     return self[item]
```

### Comparing `j-namespace-2.0.0/namespace/source/pretty_dict.py` & `j-namespace-2.1.0/namespace/source/pretty_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Jakub21, 2023Q1
 Namespace package
 """
 
 from types import NoneType, FunctionType, MethodType, LambdaType
+from datetime import datetime, date, time, timedelta
 from re import match
 
 TYPES = {
   "iterables": (list, tuple, set, bytes, bytearray),
 }
 ITER_MAX_LINE_WIDTH = 70
 
 
 class PrettyDict(dict):
 
-  def __init__(self, **data):
+  def __init__(self, data):
     """
-    Creates a namespace with all keyword parameters as elements
+    Creates a pretty dictionary.
     """
     super().__init__(data)
 
   @staticmethod
   def _get_properties(data):
     """
     Converts anything to a dictionary. Builtin properties are omitted.
@@ -54,14 +55,15 @@
     if value in _visited_containers:
       return '(...)'
 
     primitive_types = {
       (int, float, bool, NoneType): lambda val: str(val),
       (str,): lambda val: f'"{val}"',
       (type,): lambda val: f'<class {val.__name__}>',
+      (datetime, date, time, timedelta): lambda val: f'<{type(val).__name__} {val}>',
       (dict,):
         lambda val: self._convert_dict(val, indent, _depth + 1, _visited_containers),
       TYPES["iterables"]:
         lambda val: self._convert_iterable(val, indent, _depth + 1, _visited_containers),
       (FunctionType, MethodType):
         lambda val: f'{val.__name__}()'
     }
@@ -74,15 +76,15 @@
     return self._convert_object(value, indent, _depth, _visited_containers)
 
   def _convert_dict(self, data, indent=2, _depth=0, _visited_containers=None):
     _visited_containers = _visited_containers or []
     if not data:
       return 'dict (empty) { }'
     _visited_containers += [data]
-    return self.__class__(**self._get_properties(data)).to_str(indent, _depth, _visited_containers)
+    return self.__class__(self._get_properties(data)).to_str(indent, _depth, _visited_containers)
 
   def _convert_iterable(self, data, indent=2, _depth=0, _visited_containers=None):
     _visited_containers = _visited_containers or []
     SEPARATOR = ", "
     if not data:
       return f'{data.__class__.__name__} (empty)'
 
@@ -116,9 +118,9 @@
     for elm in elements:
       result += f'{" " * indent * (_depth + 1)}- {elm.strip()}\n'
     return result + ' ' * (indent * _depth) + ']'
 
   def _convert_object(self, data, indent=2, _depth=0, _visited_containers=None):
     _visited_containers = _visited_containers or []
     _visited_containers += [data]
-    ns = self.__class__(**self._get_properties(data))
+    ns = self.__class__(self._get_properties(data))
     return ns.to_str(indent, _depth + 1, _visited_containers, data.__class__.__name__)
```

### Comparing `j-namespace-2.0.0/namespace/tests/fixtures.py` & `j-namespace-2.1.0/namespace/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `j-namespace-2.0.0/namespace/tests/test_namespace.py` & `j-namespace-2.1.0/namespace/tests/test_namespace.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from .fixtures import Animal, fruits, get_circular, serial_value, json_string, yaml_string
 
 
 # constructors
 
 
 def test_constructor():
-  ns = Namespace(**fruits)
+  ns = Namespace(fruits)
   assert isinstance(ns, Namespace)
   assert not isinstance(ns.banana, Namespace) and isinstance(ns.banana, dict)
   assert not isinstance(ns.banana["colors"][0], Namespace) and isinstance(ns.banana["colors"][0], dict)
 
 
-def test_dict_factory_with_dict():
-  ns = Namespace.Dict(fruits)
-  assert isinstance(ns, Namespace)
-  assert not isinstance(ns.banana, Namespace) and isinstance(ns.banana, dict)
-  assert not isinstance(ns.banana["colors"][0], Namespace) and isinstance(ns.banana["colors"][0], dict)
+def test_kwargs_factory():
+  ns = Namespace.Kwargs(apples = 5, bananas = 4, berries = 32)
+  assert ns.apples == 5
+  assert ns["bananas"] == 4
+  assert ns.get("berries") == 32
 
 
 def test_recursive_factory_with_dict():
   ns = Namespace.Recursive(fruits)
   assert isinstance(ns, Namespace)
   assert isinstance(ns.banana, Namespace)
   assert isinstance(ns.banana.colors[0], Namespace)
@@ -36,34 +36,34 @@
   ns = Namespace.Recursive(get_circular())
 
 
 # object attribute & dict indexing syntax
 
 
 def test_getters_are_synonymous():
-  ns = Namespace(**fruits)
+  ns = Namespace(fruits)
   with_index = ns["banana"]
   with_getattr = getattr(ns, "banana")
   with_get = ns.get("banana")
   with_dot = ns.banana
 
   assert with_index is with_getattr
   assert with_getattr is with_get
   assert with_get is with_dot
 
 
 def test_setters_are_synonymous():
   value = "UniqueValue"
-  ns_index = Namespace(**fruits)
+  ns_index = Namespace(fruits)
   ns_index["unique"] = value
 
-  ns_setattr = Namespace(**fruits)
+  ns_setattr = Namespace(fruits)
   setattr(ns_setattr, "unique", value)
 
-  ns_dot = Namespace(**fruits)
+  ns_dot = Namespace(fruits)
   ns_dot.unique = value
 
   assert ns_index.unique is ns_setattr.unique
   assert ns_setattr.unique is ns_dot.unique
 
 
 # loading from serial data formats
```

