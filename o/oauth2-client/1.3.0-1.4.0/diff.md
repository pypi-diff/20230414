# Comparing `tmp/oauth2-client-1.3.0.tar.gz` & `tmp/oauth2-client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oauth2-client-1.3.0.tar", last modified: Thu Feb  2 15:05:31 2023, max compression
+gzip compressed data, was "dist/oauth2-client-1.4.0.tar", last modified: Fri Apr 14 08:57:25 2023, max compression
```

## Comparing `oauth2-client-1.3.0.tar` & `oauth2-client-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/
--rw-rw-r--   0     1000 root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.3.0/LICENSE
--rw-rw-r--   0     1000 root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.3.0/MANIFEST.in
--rw-r--r--   0     1000 root         (0)     7870 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/PKG-INFO
--rw-rw-r--   0     1000 root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.3.0/README.rst
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/main/
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/main/oauth2_client/
--rw-rw-r--   0     1000 root         (0)       22 2022-12-03 17:43:53.000000 oauth2-client-1.3.0/main/oauth2_client/__init__.py
--rw-rw-r--   0     1000 root         (0)    12777 2022-12-03 11:03:06.000000 oauth2-client-1.3.0/main/oauth2_client/credentials_manager.py
--rw-rw-r--   0     1000 root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.3.0/main/oauth2_client/http_server.py
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/
--rw-r--r--   0     1000 root         (0)     7870 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/PKG-INFO
--rw-r--r--   0     1000 root         (0)      383 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/SOURCES.txt
--rw-r--r--   0     1000 root         (0)        1 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/dependency_links.txt
--rw-r--r--   0     1000 root         (0)        1 2023-02-02 14:52:14.000000 oauth2-client-1.3.0/oauth2_client.egg-info/not-zip-safe
--rw-r--r--   0     1000 root         (0)       16 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/requires.txt
--rw-r--r--   0     1000 root         (0)       14 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/oauth2_client.egg-info/top_level.txt
--rw-rw-r--   0     1000 root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.3.0/requirements.txt
--rw-r--r--   0     1000 root         (0)       38 2023-02-02 15:05:31.000000 oauth2-client-1.3.0/setup.cfg
--rw-rw-r--   0     1000 root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/
+-rw-rw-r--   0 root         (0) root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/main/oauth2_client/
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-04-14 08:49:18.000000 oauth2-client-1.4.0/main/oauth2_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12958 2023-04-14 08:48:55.000000 oauth2-client-1.4.0/main/oauth2_client/credentials_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/main/oauth2_client/http_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:55:11.000000 oauth2-client-1.4.0/oauth2_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.4.0/setup.py
```

### Comparing `oauth2-client-1.3.0/LICENSE` & `oauth2-client-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.3.0/PKG-INFO` & `oauth2-client-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.3.0
+Version: 1.4.0
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.3.0/README.rst` & `oauth2-client-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.3.0/main/oauth2_client/credentials_manager.py` & `oauth2-client-1.4.0/main/oauth2_client/credentials_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,18 @@
     def __init__(self, state: str, port: int, host: str):
         self.state = state
         self.results = AuthorizeResponseCallback()
         self.server = start_http_server(port, host, self.results.register_parameters)
 
 
 class CredentialManager(object):
-    def __init__(self, service_information: ServiceInformation, proxies: Optional[dict] = None):
+    def __init__(self, service_information: ServiceInformation, proxies: Optional[dict] = None, user_agent: Optional[str] = None):
         self.service_information = service_information
         self.proxies = proxies if proxies is not None else dict(http='', https='')
+        self.user_agent = user_agent
         self.authorization_code_context = None
         self.refresh_token = None
         self._session = None
         if not service_information.verify:
             from requests.packages.urllib3.exceptions import InsecureRequestWarning
             import warnings
 
@@ -217,14 +218,16 @@
     @_access_token.setter
     def _access_token(self, access_token: str):
         if self._session is None:
             self._session = requests.Session()
             self._session.proxies = self.proxies
             self._session.verify = self.service_information.verify
             self._session.trust_env = False
+            if self.user_agent:
+                self._session.headers.update({'User-Agent': self.user_agent})
         if access_token is not None and len(access_token) > 0:
             self._session.headers.update(dict(Authorization='Bearer %s' % access_token))
 
     def get(self, url: str, params: Optional[dict] = None, **kwargs) -> Response:
         kwargs['params'] = params
         return self._bearer_request(self._get_session().get, url, **kwargs)
```

### Comparing `oauth2-client-1.3.0/main/oauth2_client/http_server.py` & `oauth2-client-1.4.0/main/oauth2_client/http_server.py`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.3.0/oauth2_client.egg-info/PKG-INFO` & `oauth2-client-1.4.0/oauth2_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.3.0
+Version: 1.4.0
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.3.0/setup.py` & `oauth2-client-1.4.0/setup.py`

 * *Files identical despite different names*

