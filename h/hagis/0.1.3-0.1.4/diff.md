# Comparing `tmp/hagis-0.1.3.tar.gz` & `tmp/hagis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.1.3.tar", last modified: Thu Apr 13 14:54:04 2023, max compression
+gzip compressed data, was "hagis-0.1.4.tar", last modified: Fri Apr 14 01:32:29 2023, max compression
```

## Comparing `hagis-0.1.3.tar` & `hagis-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:54:04.783027 hagis-0.1.3/
--rw-rw-rw-   0        0        0      958 2023-04-13 14:54:04.782026 hagis-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.3/README.md
--rw-rw-rw-   0        0        0      589 2023-04-13 14:53:26.000000 hagis-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:54:04.784027 hagis-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 14:54:04.753023 hagis-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:54:04.762263 hagis-0.1.3/src/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.1.3/src/hagis/__init__.py
--rw-rw-rw-   0        0        0     8706 2023-04-12 12:19:11.000000 hagis-0.1.3/src/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:54:04.780024 hagis-0.1.3/src/hagis.egg-info/
--rw-rw-rw-   0        0        0      958 2023-04-13 14:54:04.000000 hagis-0.1.3/src/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-13 14:54:04.000000 hagis-0.1.3/src/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:54:04.000000 hagis-0.1.3/src/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 14:54:04.000000 hagis-0.1.3/src/hagis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.728299 hagis-0.1.4/
+-rw-rw-rw-   0        0        0      958 2023-04-14 01:32:29.728299 hagis-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.682832 hagis-0.1.4/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.1.4/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8731 2023-04-14 01:10:13.000000 hagis-0.1.4/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-14 01:32:29.720400 hagis-0.1.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 01:32:29.000000 hagis-0.1.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-14 01:31:42.000000 hagis-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 01:32:29.728299 hagis-0.1.4/setup.cfg
```

### Comparing `hagis-0.1.3/PKG-INFO` & `hagis-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.1.3/pyproject.toml` & `hagis-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hagis-0.1.3/src/hagis/hagis.py` & `hagis-0.1.4/hagis/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
                 else:
                     # Normal classes require the parameterless constructor.
                     item = self._model()
                     for property_name, property_value in dictionary.items():
                         setattr(item, property_name, property_value)
                 yield item
 
-    def find(self, oid: int) -> Optional[T]:
-        items = [item for item in self.query(f"{self._oid_field}={oid}")]
+    def find(self, oid: int, **kwargs: Any) -> Optional[T]:
+        items = [item for item in self.query(f"{self._oid_field}={oid}", **kwargs)]
         if items:
             return items[0]
 
     def apply_edits(self, adds: Optional[List[T]] = None, updates: Optional[List[T]] = None, deletes: Union[List[int], List[str], None] = None, **kwargs: Any) -> SimpleNamespace:
         adds_json = "" if adds is None else dumps([self._to_dict(x) for x in adds])
         updates_json = "" if updates is None else dumps([self._to_dict(x) for x in updates])
         deletes_json = "" if deletes is None else dumps([x for x in deletes])
```

### Comparing `hagis-0.1.3/src/hagis.egg-info/PKG-INFO` & `hagis-0.1.4/hagis.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

