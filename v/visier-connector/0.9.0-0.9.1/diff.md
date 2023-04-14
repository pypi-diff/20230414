# Comparing `tmp/visier-connector-0.9.0.tar.gz` & `tmp/visier-connector-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.0.tar", last modified: Thu Apr 13 18:14:39 2023, max compression
+gzip compressed data, was "visier-connector-0.9.1.tar", last modified: Fri Apr 14 00:25:50 2023, max compression
```

## Comparing `visier-connector-0.9.0.tar` & `visier-connector-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.422876 visier-connector-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 18:14:30.000000 visier-connector-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 18:14:39.418876 visier-connector-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-13 18:14:30.000000 visier-connector-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-13 18:14:30.000000 visier-connector-0.9.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 18:14:30.000000 visier-connector-0.9.0/examples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:14:39.422876 visier-connector-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 18:14:30.000000 visier-connector-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:25:50.365758 visier-connector-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 00:25:36.000000 visier-connector-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 00:25:50.365758 visier-connector-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-14 00:25:36.000000 visier-connector-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:25:50.365758 visier-connector-0.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 00:25:36.000000 visier-connector-0.9.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-14 00:25:36.000000 visier-connector-0.9.1/examples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:25:50.365758 visier-connector-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 00:25:36.000000 visier-connector-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:25:50.365758 visier-connector-0.9.1/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 00:25:36.000000 visier-connector-0.9.1/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:25:50.365758 visier-connector-0.9.1/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 00:25:36.000000 visier-connector-0.9.1/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 00:25:36.000000 visier-connector-0.9.1/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-14 00:25:36.000000 visier-connector-0.9.1/visier/connector/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:25:50.365758 visier-connector-0.9.1/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 00:25:50.000000 visier-connector-0.9.1/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 00:25:50.000000 visier-connector-0.9.1/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:25:50.000000 visier-connector-0.9.1/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 00:25:50.000000 visier-connector-0.9.1/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 00:25:50.000000 visier-connector-0.9.1/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.0/LICENSE` & `visier-connector-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/PKG-INFO` & `visier-connector-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.0
+Version: 0.9.1
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

### Comparing `visier-connector-0.9.0/README.md` & `visier-connector-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/examples/__init__.py` & `visier-connector-0.9.1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/examples/util.py` & `visier-connector-0.9.1/examples/util.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/setup.py` & `visier-connector-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/visier/__init__.py` & `visier-connector-0.9.1/visier/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `visier-connector-0.9.0/visier/connector/__init__.py` & `visier-connector-0.9.1/visier/connector/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
 from .authentication import Authentication
-from .sessions import VisierSession, ResultTable, QueryExecutionError
+from .sessions import VisierSession, ResultTable, SessionContext, QueryExecutionError
```

### Comparing `visier-connector-0.9.0/visier/connector/authentication.py` & `visier-connector-0.9.1/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.0/visier/connector/sessions.py` & `visier-connector-0.9.1/visier/connector/sessions.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,55 +55,69 @@
 
     def rows(self):
         """Returns a row tuple generator"""
         for line in self._generator:
             yield json.loads(line)
 
 
+class SessionContext:
+    """
+    Context object passed to the user-defined function in the execute() method.
+    """
+    def __init__(self, session: Session, host: str) -> None:
+        self._session = session
+        self._host = host
+
+    def session(self) -> Session:
+        """Returns the current session object"""
+        return self._session
+
+    def mk_url(self, path: str) -> str:
+        """Returns a URL for the given path"""
+        return self._host + path
+
 class VisierSession:
     """Visier Session object through which SQL-like queries are executed.
     
     Keyword arguments:
     auth -- Authentication configuration
     """
     HEADER = {"Accept": "application/jsonlines, application/json"}
 
     def __init__(self, auth: Authentication) -> None:
         self._auth = auth
         self._session = None
 
     def execute_aggregate(self, query_def: object):
         """Execute a Visier aggregate query and return a tabular result."""
-        url = self._auth.host + "/v1/data/query/aggregate"
-        return self._execute_query_api(url, query_def)
+        return self._execute_query_api("/v1/data/query/aggregate", query_def)
 
     def execute_list(self, query_def: object):
         """Execute a Visier list query and return a tabular result."""
-        url = self._auth.host + "/v1/data/query/list"
-        return self._execute_query_api(url, query_def)
+        return self._execute_query_api("/v1/data/query/list", query_def)
 
     def execute_sqllike(self, sql_query: str, options = None):
         """Execute a Visier SQL-like query statement and return a tabular result."""
-        url = self._auth.host + "/v1/data/query/sql"
         body = {"query" : sql_query}
         if options:
             body["options"] = options
-        return self._execute_query_api(url, body)
+        return self._execute_query_api("/v1/data/query/sql", body)
 
-    def execute(self, call_function: Callable[[Session], Response]) -> Response:
+    def execute(self, call_function: Callable[[SessionContext], Response]) -> Response:
         """Execute a custom function with the current session.
 
         Keyword arguments:
-        call_function -- Function that takes a Session object as input and
+        call_function -- Function that takes a SessionContext object as input and
                          returns a Response object.
         """
         num_attempts_left = 2
         is_ok = False
+        context = SessionContext(self._session, self._auth.host)
         while not is_ok and num_attempts_left > 0:
-            result = call_function(self._session)
+            result = call_function(context)
             num_attempts_left -= 1
             is_ok = result.ok
             if not is_ok:
                 if result.status_code == 401 and num_attempts_left > 0:
                     self._connect()
                 else:
                     raise QueryExecutionError(result.status_code, result.text)
@@ -112,17 +126,19 @@
     def __enter__(self):
         self._connect()
         return self
 
     def __exit__(self, ex_type, ex_value, trace_back):
         self._close()
 
-    def _execute_query_api(self, url: str, body: object):
+    def _execute_query_api(self, path: str, body: object):
         """Helper method for executing a query API with flattened result."""
-        result = self.execute(lambda s: s.post(url=url, json=body, headers=self.HEADER))
+        result = self.execute(lambda s: s.session().post(url=s.mk_url(path),
+                                                         json=body,
+                                                         headers=self.HEADER))
         return ResultTable(result.iter_lines())
 
     def _connect(self):
         url = self._auth.host + "/v1/admin/visierSecureToken"
         body = {'username': self._auth.username, 'password': self._auth.password}
         if self._auth.vanity:
             body["vanityName"] = self._auth.vanity
```

### Comparing `visier-connector-0.9.0/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.1/visier_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.0
+Version: 0.9.1
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

