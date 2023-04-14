# Comparing `tmp/propertysync-0.1.0.tar.gz` & `tmp/propertysync-0.2.1.tar.gz`

## Comparing `propertysync-0.1.0.tar` & `propertysync-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 propertysync-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/__init__.py
--rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/api.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/batch.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/search.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.1.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.1.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.1.0/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propertysync-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 propertysync-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 propertysync-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/__init__.py
+-rw-r--r--   0        0        0    14498 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/api.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/batch.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.2.1/propertysync/search.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.2.1/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.2.1/PKG-INFO
```

### Comparing `propertysync-0.1.0/CHANGELOG.md` & `propertysync-0.2.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 ## [Unreleased]
 
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
-## [0.1.0] - 2023-03-26
+## [0.2.1] - 2023-04-26
+
+### Added
+- Added optional save_to_search and wait_time parameters to create_batch_from_json method that allows you to submit a batch, wait for it's documents to be processed and save the batch to search making those documents live in the plant.
+
+### Fixed
+- Corrected package requirements
+
+## [0.1.0] - 2023-04-25
 
 ### Added
 - Added instrument_numbers method to Batch class to return a list of instrument numbers
 - Add govLot to acreage searches
 - Added package specific documentation
 
 ### Fixed
```

### Comparing `propertysync-0.1.0/propertysync/api.py` & `propertysync-0.2.1/propertysync/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,18 +148,36 @@
     def create_batch(self, batch_name, search_id=None):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/batches"
         params = {"name":batch_name}
         if search_id is not None:
             params["searchId"] = search_id
         return self.api_call("POST", url, params)
     
-    # create batch from json
-    def create_batch_from_json(self, json):
+    # create batch from json, optionally save to search
+    def create_batch_from_json(self, json, save_to_search=False, wait_time=2):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/batches"
-        return self.api_call("POST", url, body=json)
+
+        #if they want to save to search, we need to count the number of documents in the batch
+        if save_to_search:
+            num_documents = len(json["documents"])
+
+            # create the batch
+            batch = self.api_call("POST", url, body=json)
+
+            # check the status of the batch until numOfDocs is equal to the number of documents in the batch
+            while batch["numOfDocs"] != num_documents:
+                time.sleep(wait_time)
+                batch = self.get_batch_info(batch["id"])
+
+            # update the batch to save to search
+            self.save_batch_to_search(batch["id"])
+
+            return batch
+        else:
+            return self.api_call("POST", url, body=json)
     
     # update batch from json
     def update_batch_from_json(self, json, batch_id):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/batches/{batch_id}"
         return self.api_call("PATCH", url, body=json)
     
     # create batch from file at URL
```

### Comparing `propertysync-0.1.0/propertysync/batch.py` & `propertysync-0.2.1/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.1.0/propertysync/document.py` & `propertysync-0.2.1/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.1.0/propertysync/search.py` & `propertysync-0.2.1/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.1.0/LICENSE` & `propertysync-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.1.0/README.md` & `propertysync-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.1.0/pyproject.toml` & `propertysync-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = ["jsonpath_ng", "requests"]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://developer.propertysync.com/python/index.html"
 
 [tool.hatch.version]
 path = "propertysync/__about__.py"
```

### Comparing `propertysync-0.1.0/PKG-INFO` & `propertysync-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.1.0
+Version: 0.2.1
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: jsonpath-ng
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # PropertySync Python Client
 
 [![PyPI version](https://badge.fury.io/py/propertysync.svg)](https://badge.fury.io/py/propertysync)
 [![PyPI](https://img.shields.io/pypi/pyversions/propertysync.svg)](https://pypi.python.org/pypi/propertysync)
```

