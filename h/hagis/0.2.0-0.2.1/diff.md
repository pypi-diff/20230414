# Comparing `tmp/hagis-0.2.0.tar.gz` & `tmp/hagis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.0.tar", last modified: Fri Apr 14 11:32:14 2023, max compression
+gzip compressed data, was "hagis-0.2.1.tar", last modified: Fri Apr 14 13:20:06 2023, max compression
```

## Comparing `hagis-0.2.0.tar` & `hagis-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.963352 hagis-0.2.0/
--rw-rw-rw-   0        0        0      958 2023-04-14 11:32:14.955397 hagis-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.915308 hagis-0.2.0/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.0/hagis/__init__.py
--rw-rw-rw-   0        0        0     8620 2023-04-14 11:28:06.000000 hagis-0.2.0/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:32:14.955397 hagis-0.2.0/hagis.egg-info/
--rw-rw-rw-   0        0        0      958 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 11:32:14.000000 hagis-0.2.0/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-14 11:31:43.000000 hagis-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 11:32:14.963352 hagis-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.679693 hagis-0.2.1/
+-rw-rw-rw-   0        0        0      958 2023-04-14 13:20:06.678693 hagis-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.661475 hagis-0.2.1/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.1/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8515 2023-04-14 13:00:48.000000 hagis-0.2.1/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.676699 hagis-0.2.1/hagis.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-14 13:19:21.000000 hagis-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:20:06.680535 hagis-0.2.1/setup.cfg
```

### Comparing `hagis-0.2.0/PKG-INFO` & `hagis-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.0/hagis/hagis.py` & `hagis-0.2.1/hagis/hagis.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,22 +55,14 @@
 
         # Add custom properties that have not been handled as dynamically handled propeties.
         for property, field in mapping.items():
             if property not in mapped:
                 self._fields[property.lower()] = field
 
     def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterator[T]:
-        """ Queries the feature layer and yields the results as typed objects.
-
-        Args:
-            where_clause (str, optional): Where clause.  Defaults to "1=1".
-
-        Yields:
-            Iterator[T]: Lazily generated objects of specified type.
-        """
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
             fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
 
@@ -88,14 +80,18 @@
                 else:
                     # Normal classes require the parameterless constructor.
                     item = self._model()
                     for property_name, property_value in dictionary.items():
                         setattr(item, property_name, property_value)
                 yield item
 
+    def count(self, where_clause: str = "1=1") -> int:
+        obj = self._post("query", where=where_clause, returnCountOnly=True, f="json")
+        return obj.count
+
     def find(self, oid: int, **kwargs: Any) -> Optional[T]:
         items = [item for item in self.query(f"{self._oid_field}={oid}", **kwargs)]
         if items:
             return items[0]
 
     def apply_edits(self, adds: Optional[List[T]] = None, updates: Optional[List[T]] = None, deletes: Union[List[int], List[str], None] = None, **kwargs: Any) -> SimpleNamespace:
         adds_json = "" if adds is None else dumps([self._to_dict(x) for x in adds])
```

### Comparing `hagis-0.2.0/hagis.egg-info/PKG-INFO` & `hagis-0.2.1/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.0/pyproject.toml` & `hagis-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

