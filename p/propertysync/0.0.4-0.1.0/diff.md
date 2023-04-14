# Comparing `tmp/propertysync-0.0.4.tar.gz` & `tmp/propertysync-0.1.0.tar.gz`

## Comparing `propertysync-0.0.4.tar` & `propertysync-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/__init__.py
--rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/api.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/batch.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/document.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 propertysync-0.0.4/propertysync/search.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.0.4/README.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 propertysync-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 propertysync-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 propertysync-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/api.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/batch.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.1.0/propertysync/search.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.1.0/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propertysync-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 propertysync-0.1.0/PKG-INFO
```

### Comparing `propertysync-0.0.4/propertysync/api.py` & `propertysync-0.1.0/propertysync/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests, os
+import requests, os, time
 
 """
 This is a helper for interacting with the PropertySync API
 """
 
 # TODO: Follow styleguide: https://google.github.io/styleguide/pyguide.html#316-naming
 
@@ -77,36 +77,35 @@
 
         credentials = {"email":self.email,"password":self.password}
         
         headers = {
             "User-Agent": self.user_agent,
             "Content-Type": "application/json"
             }
-        # if the token is already set, return
-        if os.environ.get("PROPERTYSYNC_API_TOKEN") is not None:
-            self.token = os.environ.get("PROPERTYSYNC_API_TOKEN")
-            return
         
         login_request = requests.post(self.login_url,json=credentials, headers=headers)
 
         if login_request.status_code != 200:
             raise Exception("Login failed: "+login_request.text)
 
         self.token = login_request.json()["token"]
-        os.environ["PROPERTYSYNC_API_TOKEN"] = self.token
 
     # make a call to the API
     def api_call(self, method, url, params=None, body=None, tries=1):
         # create a header with the token
         headers = {
             "User-Agent": self.user_agent,
             "Authorization": "Bearer "+self.token, 
             "Content-Type": "application/json"
         }
 
+        # append our trailing slash if it is not already there and must be set
+        if self.trailing_slash != "" and url[-1] != self.trailing_slash:
+            url += self.trailing_slash
+
         if (method == "GET"):
             request = requests.get(url,params=params,headers=headers, json=body)
         elif (method == "POST"):
             request = requests.post(url,params=params,headers=headers, json=body)
         elif (method == "DELETE"):
             request = requests.delete(url,params=params,headers=headers, json=body)    
         elif (method == "PATCH"):
@@ -224,17 +223,35 @@
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/auto-completes"
         body = {
             "type":type,
             "value":value
         }
         return self.api_call("POST", url, body=body)
     
+    # get landvalidations
+    def get_landvalidations(self, type=None):
+        url = f"{self.indexing_url}/document-groups/{self.document_group_id}/land-validations"
+        params = {}
+
+        if type is not None:
+            params["type"] = type
+
+        validations = self.api_call("GET", url, params=params)
+
+        # strip out all fields that are not "id" or "json"
+        for validation in validations:
+            for key in list(validation.keys()):
+                if key != "id" and key != "json":
+                    del validation[key]
+
+        return validations
+
     # get document IDs from a search ID
     def get_document_ids_from_search(self, search_id):
-        url = f"{self.search_url}/document-groups/{self.document_group_id}/searches/{search_id}/document-ids{self.trailing_slash}"
+        url = f"{self.search_url}/document-groups/{self.document_group_id}/searches/{search_id}/document-ids"
         return self.api_call("GET", url)
     
     # get JSON from a document ID
     def get_json_from_document_id(self, document_id):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/{document_id}"
         return self.api_call("GET", url)
     
@@ -253,46 +270,70 @@
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/{document_id}/versions"
         return self.api_call("GET", url)
 
     # get orders (requires a company ID)
     def get_orders(self):
         if self.company_id is None:
             raise Exception("You must set a company ID to use this method")
-        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders{self.trailing_slash}"
+        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders"
         return self.api_call("GET", url)
 
     # close an order
     def close_order(self, order_id):
         if self.company_id is None:
             raise Exception("You must set a company ID to use this method")
-        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders/{order_id}/close{self.trailing_slash}"
+        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders/{order_id}/close"
         return self.api_call("POST", url)
 
     # reopen an order
     def reopen_order(self, order_id):
         if self.company_id is None:
             raise Exception("You must set a company ID to use this method")
-        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders/{order_id}/re-open{self.trailing_slash}"
+        url = f"{self.search_url}/document-groups/{self.document_group_id}/companies/{self.company_id}/orders/{order_id}/re-open"
         return self.api_call("POST", url)
     
     # get document group meta data
     def get_document_group_metadata(self):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/plant-info"
         return self.api_call("GET", url)
     
     # run a report
     def run_report(self, report_id, params=None):
-        url = f"{self.search_url}/reports/{report_id}/run{self.trailing_slash}"
+        url = f"{self.search_url}/reports/{report_id}/run"
         return self.api_call("GET", url, params=params)
     
     # run a search
     def run_search(self, search_query):
-        url = f"{self.search_url}/document-groups/{self.document_group_id}/searches{self.trailing_slash}"
+        url = f"{self.search_url}/document-groups/{self.document_group_id}/searches"
         return self.api_call("POST", url, body=search_query)
 
+    # run a search, then create a batch and wait for the batch to fully hydrate, then retrieve the batch and optionally delete it
+    def run_search_and_create_batch(self, search_query, minimum_results=1,wait_time=2,batch_name='python-api-client temp batch', delete_batch=True):
+        search = self.run_search(search_query)
+        search_id = search["id"]
+
+        # if we don't have enough results in the search, throw an exception
+        if search["count"] < minimum_results:
+            raise Exception(f"Search returned {search['count']} results, but we need at least {minimum_results} to create a batch")
+
+        batch_id = self.create_batch(batch_name,search_id)["id"]
+        batch_info = self.get_batch_info(batch_id)
+        while batch_info["numOfDocs"] < search["count"]:
+            time.sleep(wait_time)
+            batch_info = self.get_batch_info(batch_id)
+
+        ## once here, we should be complete
+        batch = self.get_batch(batch_id)
+
+        # optionally delete the batch
+        if delete_batch:
+            self.delete_batch(batch_id)
+
+        return batch
+
     # run the user-activity report
     def run_user_activity_report(self, start_date, end_date, format="json"):
         params = {
             "companyId":self.company_id,
             "plantId":self.document_group_id,
             "responseType":format,
             "startDate":start_date,
```

### Comparing `propertysync-0.0.4/propertysync/search.py` & `propertysync-0.1.0/propertysync/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,28 +100,31 @@
     def add_legal(self, full_text_legal=None, parcel=None):
         legal = {}
         if full_text_legal:
             legal["fullTextLegal"] = full_text_legal
         self.legals.append(legal)
 
     # add acreage
-    def add_acreage(self, section=None, township=None, range=None, quarter=None, arb=None, comment=None):
+    def add_acreage(self, section=None, township=None, range=None, quarter=None, arb=None, govlot=None, comment=None):
         acreage = {}
         if township:
             acreage["township"] = township
         if range:
             acreage["range"] = range
         if section:
             acreage["section"] = section
         if quarter:
             acreage["quarter"] = quarter
         if arb:
             acreage["arb"] = arb
+        if govlot:
+            acreage["govLot"] = govlot
         if comment:
             acreage["acreageComment"] = comment
+        
 
         self.acreages.append(acreage)
   
     # add address
     def add_address(self, address=None, city=None, state=None, zip=None):
         addressRecord = {}
         if address:
@@ -167,15 +170,15 @@
 
         # add parties
         if len(self.parties) > 0:
             query["queryParams"]["parties"] = self.parties
 
         # add subdivision
         if len(self.subdivisions) > 0:
-            query["queryParams"]["subdivision"] = self.subdivisions
+            query["queryParams"]["subdivisions"] = self.subdivisions
 
         # add acreage
         if len(self.acreages) > 0:
             query["queryParams"]["acreages"] = self.acreages
 
         # add parcels
         if len(self.parcels) > 0:
```

### Comparing `propertysync-0.0.4/LICENSE.txt` & `propertysync-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.0.4/README.md` & `propertysync-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.0.4/pyproject.toml` & `propertysync-0.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "propertysync"
-description = 'A package for interacting with the [PropertySync API](https://developer.propertysync.com/api.html)'
+description = 'A package for interacting with the PropertySync API.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Rob Martinson", email = "rob@limelyte.com" },
 ]
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://developer.propertysync.com/"
+Documentation = "https://developer.propertysync.com/python/index.html"
 
 [tool.hatch.version]
 path = "propertysync/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
@@ -53,7 +53,13 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.hatch.build]
+exclude = [
+  ".gitignore",
+  "README.dev.md",
+]
```

### Comparing `propertysync-0.0.4/PKG-INFO` & `propertysync-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.0.4
-Summary: A package for interacting with the [PropertySync API](https://developer.propertysync.com/api.html)
-Project-URL: Documentation, https://developer.propertysync.com/
+Version: 0.1.0
+Summary: A package for interacting with the PropertySync API.
+Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
-License-File: LICENSE.txt
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

