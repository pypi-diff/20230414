# Comparing `tmp/propertysync-0.2.1.tar.gz` & `tmp/propertysync-0.3.0.tar.gz`

## Comparing `propertysync-0.2.1.tar` & `propertysync-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 propertysync-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/__init__.py
--rw-r--r--   0        0        0    14498 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/api.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/batch.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/search.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.2.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.2.1/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.2.1/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 propertysync-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/api.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/batch.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/search.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.3.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.3.0/PKG-INFO
```

### Comparing `propertysync-0.2.1/CHANGELOG.md` & `propertysync-0.3.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 ## [Unreleased]
 
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
+## [0.3.0] - 2023-04-26
+
+### Added
+- Added support to document and batch classes to support find and replace
+
 ## [0.2.1] - 2023-04-26
 
 ### Added
 - Added optional save_to_search and wait_time parameters to create_batch_from_json method that allows you to submit a batch, wait for it's documents to be processed and save the batch to search making those documents live in the plant.
 
 ### Fixed
 - Corrected package requirements
```

### Comparing `propertysync-0.2.1/propertysync/api.py` & `propertysync-0.3.0/propertysync/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,24 @@
             self.save_batch_to_search(batch["id"])
 
             return batch
         else:
             return self.api_call("POST", url, body=json)
     
     # update batch from json
-    def update_batch_from_json(self, json, batch_id):
+    def update_batch_from_json(self, json, batch_id=None):
+        # if batch_id is none, we need to determine from the json
+        if batch_id is None:
+            if "id" in json:
+                batch_id = json["id"]
+       
+        # if we still don't have a batch_id, raise an exception
+        if batch_id is None:
+            raise Exception("Batch ID is not set")
+
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/batches/{batch_id}"
         return self.api_call("PATCH", url, body=json)
     
     # create batch from file at URL
     def create_batch_from_url(self, url):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/batches"
         body = {
```

### Comparing `propertysync-0.2.1/propertysync/batch.py` & `propertysync-0.3.0/propertysync/batch.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # get all of the instrumentNumbers for a given instrumentType, or all instrumentNumbers if no instrumentType is specified
     def instrument_numbers(self, instrument_type_filter = None):
         if instrument_type_filter:
             return [doc.instrumentNumber for doc in self.documents if doc.instrumentType == instrument_type_filter]
         else:
             return [doc.instrumentNumber for doc in self.documents]
         
-    # replace "find" with "replace" in "json.node" for all documents in the batch
-    def replace(self, find, replace, json_node):
+    # replace json_path with "value" in all documents in the batch
+    def replace(self, json_path, value):
         for doc in self.documents:
-            doc.replace(find, replace, json_node)
+            doc.replace(json_path, value)
 
     # find all documents in the batch that have a specific value in a specific json node
-    def find(self, find, json_node):
-        return [doc for doc in self.documents if doc.find(find, json_node)]
+    def find(self, json_path):
+        return [doc for doc in self.documents if doc.find(json_path)]
```

### Comparing `propertysync-0.2.1/propertysync/document.py` & `propertysync-0.3.0/propertysync/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
-from jsonpath_ng import jsonpath, parse
+from jsonpath_ng import jsonpath
+from jsonpath_ng.ext import parse
 
 """
 This is a helper class for working with PropertySync documents.
 """
 
 class Document:
     def __init__(self, json_string=None):
@@ -27,40 +28,34 @@
 
     # use magic methods to make the document properties accessible as attributes
     def __getattr__(self, name):
         if name in self._json["json"]:
             return self._json["json"][name]
         else:
             return None
+
+    # serialize the doc to json    
+    def get_json(self):
+        return self._json
         
     # return subdivisionlegals where parcel matches a value
     def subdivisionlegals_with_parcel(self, parcel):
         return [legal for legal in self.subdivisionlegals if legal["parcel"] == parcel]
     
     def __str__(self):
         return json.dumps(self._json, indent=4)
     
-    # replace "find" with "replace" in "json.node" for this document 
-    def replace(self, find, replace, json_node):
-        jsonpath_expr = parse(json_node)
-        matches = jsonpath_expr.find(self._json["json"])
-        for match in matches:
-            if match.value == find:
-                match.value = replace
-
+    # replace  with "value" in "json_path" for this document 
+    def replace(self, json_path, value):
+        jsonpath_expr = parse(json_path)
+        jsonpath_expr.find(self._json["json"])
+        jsonpath_expr.update(self._json["json"], value)
                 
-        
     # find all nodes in the document that have a specific value
-    def find(self, find, json_node):
-#         expression = json_node + "[?(@== '" + find + "')]"
-
-        print (json_node)
-
-        jsonpath_expr = parse(expression)
+    def find(self, json_path):
+        jsonpath_expr = parse(json_path)
         matches = jsonpath_expr.find(self._json["json"])
         if len(matches) > 0:
-            return True
-        else:
-            return False
-        
-
-       
+            return matches
+            
+        return False
+
```

### Comparing `propertysync-0.2.1/propertysync/search.py` & `propertysync-0.3.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.2.1/LICENSE` & `propertysync-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.2.1/README.md` & `propertysync-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.2.1/pyproject.toml` & `propertysync-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.2.1/PKG-INFO` & `propertysync-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

