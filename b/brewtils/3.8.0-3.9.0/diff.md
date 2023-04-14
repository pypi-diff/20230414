# Comparing `tmp/brewtils-3.8.0.tar.gz` & `tmp/brewtils-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brewtils-3.8.0.tar", last modified: Thu Nov 18 14:28:52 2021, max compression
+gzip compressed data, was "dist/brewtils-3.9.0.tar", last modified: Wed Dec  8 15:06:49 2021, max compression
```

## Comparing `brewtils-3.8.0.tar` & `brewtils-3.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     6382 2021-11-18 14:28:52.000000 brewtils-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4555 2021-11-18 14:28:36.000000 brewtils-3.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils/
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7119 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/choices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7561 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    29790 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     9994 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    40432 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    24860 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/pika.py
--rw-r--r--   0 runner    (1001) docker     (121)    40772 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/queues.py
--rw-r--r--   0 runner    (1001) docker     (121)    20024 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/request_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils/resolvers/
--rw-r--r--   0 runner    (1001) docker     (121)      646 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/resolvers/bytes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/resolvers/chunks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/resolvers/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/resolvers/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils/rest/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27122 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    33569 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/rest/easy_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    23422 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/rest/system_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    32182 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    21409 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     6817 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/specification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/stoppable_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12039 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/test/comparable.py
--rw-r--r--   0 runner    (1001) docker     (121)    21654 2021-11-18 14:28:36.000000 brewtils-3.8.0/brewtils/test/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6382 2021-11-18 14:28:51.000000 brewtils-3.8.0/brewtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      893 2021-11-18 14:28:52.000000 brewtils-3.8.0/brewtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 14:28:51.000000 brewtils-3.8.0/brewtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-11-18 14:28:51.000000 brewtils-3.8.0/brewtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-18 14:28:51.000000 brewtils-3.8.0/brewtils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-11-18 14:28:52.000000 brewtils-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-11-18 14:28:36.000000 brewtils-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     6382 2021-12-08 15:06:49.000000 brewtils-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2021-12-08 15:06:41.000000 brewtils-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7119 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/choices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7561 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29790 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5529 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9994 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40432 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24860 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/pika.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40772 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/queues.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20024 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/request_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/resolvers/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/resolvers/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/resolvers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3809 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/resolvers/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils/rest/
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27354 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33734 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/rest/easy_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23422 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/rest/system_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32182 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21424 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6817 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/specification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/stoppable_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12039 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/test/comparable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21654 2021-12-08 15:06:41.000000 brewtils-3.9.0/brewtils/test/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6382 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-08 15:06:49.000000 brewtils-3.9.0/brewtils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-12-08 15:06:49.000000 brewtils-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-12-08 15:06:41.000000 brewtils-3.9.0/setup.py
```

### Comparing `brewtils-3.8.0/PKG-INFO` & `brewtils-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: brewtils
-Version: 3.8.0
+Version: 3.9.0
 Summary: Beer-garden plugin and utility library
 Home-page: https://beer-garden.io/
 Author: The Beer-garden Team
 Author-email:  
 License: MIT
 Description: 
         ========
```

### Comparing `brewtils-3.8.0/README.rst` & `brewtils-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/__init__.py` & `brewtils-3.9.0/brewtils/__init__.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/choices.py` & `brewtils-3.9.0/brewtils/choices.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/config.py` & `brewtils-3.9.0/brewtils/config.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/decorators.py` & `brewtils-3.9.0/brewtils/decorators.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/display.py` & `brewtils-3.9.0/brewtils/display.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/errors.py` & `brewtils-3.9.0/brewtils/errors.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/log.py` & `brewtils-3.9.0/brewtils/log.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/models.py` & `brewtils-3.9.0/brewtils/models.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/pika.py` & `brewtils-3.9.0/brewtils/pika.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/plugin.py` & `brewtils-3.9.0/brewtils/plugin.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/request_handling.py` & `brewtils-3.9.0/brewtils/request_handling.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/resolvers/__init__.py` & `brewtils-3.9.0/brewtils/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/resolvers/bytes.py` & `brewtils-3.9.0/brewtils/resolvers/bytes.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/resolvers/chunks.py` & `brewtils-3.9.0/brewtils/resolvers/chunks.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/resolvers/identity.py` & `brewtils-3.9.0/brewtils/resolvers/identity.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/resolvers/manager.py` & `brewtils-3.9.0/brewtils/resolvers/manager.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/rest/__init__.py` & `brewtils-3.9.0/brewtils/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/rest/client.py` & `brewtils-3.9.0/brewtils/rest/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -614,26 +614,33 @@
             payload: New Job definition
 
         Returns:
             Requests Response object
         """
         return self.session.post(self.job_url, data=payload, headers=self.JSON_HEADERS)
 
-    def post_execute_job(self, job_id):
+    def post_execute_job(self, job_id, reset_interval=False):
         # type: (str) -> Response
         """Performs a POST on the Job Execute URL
 
         Args:
             job_id: The ID of the Job
+            reset_interval: Sets interval of job to restart now
 
         Returns:
             Request Response object
         """
+        url_params = {}
+        if reset_interval:
+            url_params["reset_interval"] = "True"
+
         return self.session.post(
-            self.job_url + job_id + "/execute", headers=self.JSON_HEADERS
+            self.job_url + job_id + "/execute",
+            headers=self.JSON_HEADERS,
+            params=url_params,
         )
 
     @enable_auth
     def post_export_jobs(self, payload):
         # type: (str) -> Response
         """Perform a POST on the Job export URL.
```

### Comparing `brewtils-3.8.0/brewtils/rest/easy_client.py` & `brewtils-3.9.0/brewtils/rest/easy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -839,24 +839,26 @@
 
         Returns:
             Job: The updated Job
 
         """
         return self._patch_job(job_id, [PatchOperation("update", "/status", "RUNNING")])
 
-    def execute_job(self, job_id):
+    def execute_job(self, job_id, reset_interval=False):
         """Execute a Job
 
         Args:
             job_id (str): The Job ID
+            reset_interval (bool): Restarts the job's interval time to now if
+                the job's trigger is an interval
 
         Returns:
             Request: The returned request
         """
-        return self.client.post_execute_job(job_id)
+        return self.client.post_execute_job(job_id, reset_interval)
 
     @wrap_response(parse_method="parse_resolvable")
     def upload_bytes(self, data):
         # type: (bytes) -> Any
         """Upload a file
 
         Args:
```

### Comparing `brewtils-3.8.0/brewtils/rest/system_client.py` & `brewtils-3.9.0/brewtils/rest/system_client.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/schema_parser.py` & `brewtils-3.9.0/brewtils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/schemas.py` & `brewtils-3.9.0/brewtils/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,15 +580,15 @@
         serialization_schema_selector=_domain_identifier_schema_selector,
         deserialization_schema_selector=_domain_identifier_schema_selector,
         required=False,
     )
 
 
 class RoleAssignmentSchema(BaseSchema):
-    domain = fields.Nested(RoleAssignmentDomainSchema)
+    domain = fields.Nested(RoleAssignmentDomainSchema, required=True)
     role = fields.Nested(RoleSchema())
 
 
 class UserSchema(BaseSchema):
     id = fields.Str()
     username = fields.Str()
     role_assignments = fields.List(fields.Nested(RoleAssignmentSchema()))
```

### Comparing `brewtils-3.8.0/brewtils/specification.py` & `brewtils-3.9.0/brewtils/specification.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/stoppable_thread.py` & `brewtils-3.9.0/brewtils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/test/comparable.py` & `brewtils-3.9.0/brewtils/test/comparable.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils/test/fixtures.py` & `brewtils-3.9.0/brewtils/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/brewtils.egg-info/PKG-INFO` & `brewtils-3.9.0/brewtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: brewtils
-Version: 3.8.0
+Version: 3.9.0
 Summary: Beer-garden plugin and utility library
 Home-page: https://beer-garden.io/
 Author: The Beer-garden Team
 Author-email:  
 License: MIT
 Description: 
         ========
```

### Comparing `brewtils-3.8.0/brewtils.egg-info/SOURCES.txt` & `brewtils-3.9.0/brewtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brewtils-3.8.0/setup.py` & `brewtils-3.9.0/setup.py`

 * *Files identical despite different names*

