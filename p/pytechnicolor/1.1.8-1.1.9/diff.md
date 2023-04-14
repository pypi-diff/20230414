# Comparing `tmp/pytechnicolor-1.1.8.tar.gz` & `tmp/pytechnicolor-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytechnicolor-1.1.8.tar", last modified: Wed Jan 11 21:27:18 2023, max compression
+gzip compressed data, was "pytechnicolor-1.1.9.tar", last modified: Fri Apr 14 18:59:24 2023, max compression
```

## Comparing `pytechnicolor-1.1.8.tar` & `pytechnicolor-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 21:27:18.312835 pytechnicolor-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-11 21:27:18.312835 pytechnicolor-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-11 21:27:03.000000 pytechnicolor-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 21:27:18.312835 pytechnicolor-1.1.8/pytechnicolor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-11 21:27:18.000000 pytechnicolor-1.1.8/pytechnicolor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-11 21:27:18.000000 pytechnicolor-1.1.8/pytechnicolor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 21:27:18.000000 pytechnicolor-1.1.8/pytechnicolor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-11 21:27:18.000000 pytechnicolor-1.1.8/pytechnicolor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-11 21:27:18.000000 pytechnicolor-1.1.8/pytechnicolor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 21:27:18.312835 pytechnicolor-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-11 21:27:03.000000 pytechnicolor-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 21:27:18.312835 pytechnicolor-1.1.8/technicolorgateway/
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-01-11 21:27:03.000000 pytechnicolor-1.1.8/technicolorgateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-11 21:27:03.000000 pytechnicolor-1.1.8/technicolorgateway/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-01-11 21:27:03.000000 pytechnicolor-1.1.8/technicolorgateway/mysrp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:24.149783 pytechnicolor-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:59:24.149783 pytechnicolor-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:24.145782 pytechnicolor-1.1.9/pytechnicolor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:59:24.000000 pytechnicolor-1.1.9/pytechnicolor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 18:59:24.000000 pytechnicolor-1.1.9/pytechnicolor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:59:24.000000 pytechnicolor-1.1.9/pytechnicolor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 18:59:24.000000 pytechnicolor-1.1.9/pytechnicolor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 18:59:24.000000 pytechnicolor-1.1.9/pytechnicolor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:59:24.149783 pytechnicolor-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:24.149783 pytechnicolor-1.1.9/technicolorgateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/technicolorgateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/technicolorgateway/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/technicolorgateway/mysrp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:24.149783 pytechnicolor-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/tests/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-14 18:59:14.000000 pytechnicolor-1.1.9/tests/test_modal.py
```

### Comparing `pytechnicolor-1.1.8/PKG-INFO` & `pytechnicolor-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytechnicolor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Technicolor Gateway library
 Home-page: https://github.com/shaiu/techicolorgateway
 Author: Shai Ungar
 Author-email: shaiungar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytechnicolor-1.1.8/README.md` & `pytechnicolor-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pytechnicolor-1.1.8/pytechnicolor.egg-info/PKG-INFO` & `pytechnicolor-1.1.9/pytechnicolor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytechnicolor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Technicolor Gateway library
 Home-page: https://github.com/shaiu/techicolorgateway
 Author: Shai Ungar
 Author-email: shaiungar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytechnicolor-1.1.8/setup.py` & `pytechnicolor-1.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pytechnicolor",
-    version="1.1.8",
+    version="1.1.9",
     description="Technicolor Gateway library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/shaiu/techicolorgateway",
     author="Shai Ungar",
     author_email="shaiungar@gmail.com",
     license="MIT",
```

### Comparing `pytechnicolor-1.1.8/technicolorgateway/__init__.py` & `pytechnicolor-1.1.9/technicolorgateway/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,64 +7,72 @@
 from robobrowser import RoboBrowser
 
 from technicolorgateway import mysrp as srp
 from technicolorgateway.modal import get_device_modal, get_broadband_modal
 
 _LOGGER = logging.getLogger(__name__)
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 
 class TechnicolorGateway:
     def __init__(self, host, port, user, password) -> None:
         self._host = host
         self._port = port
         self._uri = f'http://{host}:{port}'
         self._user = user
         self._password = password
         self._br = RoboBrowser(history=True, parser="html.parser")
 
     def srp6authenticate(self):
-        try:
-            self._br.open(self._uri)
-            token_tag = self._br.find(lambda tag: tag.has_attr('name')
-                                                  and tag['name'] == 'CSRFtoken')
-            token = token_tag['content']
-            _LOGGER.debug('Got CSRF token: %s', token)
-
-            usr = srp.User(self._user, self._password, hash_alg=srp.SHA256, ng_type=srp.NG_2048)
-            uname, A = usr.start_authentication()
-            _LOGGER.debug('A value %s', binascii.hexlify(A))
-
-            self._br.open(f'{self._uri}/authenticate', method='post',
-                          data=urlencode({'CSRFtoken': token,
-                                          'I': uname, 'A': binascii.hexlify(A)}))
-            _LOGGER.debug("br.response %s", self._br.response)
-            j = json.decoder.JSONDecoder().decode(self._br.parsed.decode())
-            _LOGGER.debug("Challenge received: %s", j)
-
-            M = usr.process_challenge(binascii.unhexlify(j['s']), binascii.unhexlify(j['B']))
-            _LOGGER.debug("M value %s", binascii.hexlify(M))
-            self._br.open(f'{self._uri}/authenticate', method='post',
-                          data=urlencode({'CSRFtoken': token, 'M': binascii.hexlify(M)}))
-            _LOGGER.debug("br.response %s", self._br.response)
-            j = json.decoder.JSONDecoder().decode(self._br.parsed.decode())
-            _LOGGER.debug("Got response %s", j)
 
-            if 'error' in j:
-                raise Exception("Unable to authenticate (check password?), message:", j)
+        self._br.open(self._uri)
+        token_tag = self._br.find(lambda tag: tag.has_attr('name') and tag['name'] == 'CSRFtoken')
+        token = token_tag['content']
+        _LOGGER.debug('Got CSRF token: %s', token)
+
+        usr = srp.User(self._user, self._password, hash_alg=srp.SHA256, ng_type=srp.NG_2048)
+        uname, A = usr.start_authentication()
+        _LOGGER.debug('A value %s', binascii.hexlify(A))
+
+        self._br.open(f'{self._uri}/authenticate', method='post',
+                      data=urlencode({'CSRFtoken': token,
+                                      'I': uname, 'A': binascii.hexlify(A)}))
+        _LOGGER.debug("br.response %s", self._br.response)
+        j = json.decoder.JSONDecoder().decode(self._br.parsed.decode())
+        _LOGGER.debug("Challenge received: %s", j)
+
+        M = usr.process_challenge(binascii.unhexlify(j['s']), binascii.unhexlify(j['B']))
+        _LOGGER.debug("M value %s", binascii.hexlify(M))
+        self._br.open(f'{self._uri}/authenticate', method='post',
+                      data=urlencode({'CSRFtoken': token, 'M': binascii.hexlify(M)}))
+        _LOGGER.debug("br.response %s", self._br.response)
+        j = json.decoder.JSONDecoder().decode(self._br.parsed.decode())
+        _LOGGER.debug("Got response %s", j)
+
+        if 'error' in j:
+            raise Exception("Unable to authenticate (check password?), message:", j)
+
+        usr.verify_session(binascii.unhexlify(j['M']))
+        if not usr.authenticated():
+            raise Exception("Unable to authenticate")
 
-            usr.verify_session(binascii.unhexlify(j['M']))
-            if not usr.authenticated():
-                raise Exception("Unable to authenticate")
+        return True
 
+    def authenticate(self):
+        try:
+            self._br.open(f'{self._uri}', method='POST',
+                          data={"username": self._user, "password": self._password})
+            _LOGGER.debug("br.response %s", self._br.response)
+            if self._br.response.status_code != 200:
+                return self.srp6authenticate()
             return True
 
-        except Exception as execption:
-            _LOGGER.error("Authentication failed. Exception: %s", execption)
+        except Exception as exception:
+            _LOGGER.error("Authentication failed. Exception: %s", exception)
             traceback.print_exc()
             raise
 
     def get_device_modal(self):
         data = self.get_device_modals(f"{self._uri}/modals/device-modal.lp")
         if len(data) == 0:
             data = self.get_device_modals(f"{self._uri}/modals/ipv6devices-modal.lp")
```

### Comparing `pytechnicolor-1.1.8/technicolorgateway/modal.py` & `pytechnicolor-1.1.9/technicolorgateway/modal.py`

 * *Files identical despite different names*

### Comparing `pytechnicolor-1.1.8/technicolorgateway/mysrp.py` & `pytechnicolor-1.1.9/technicolorgateway/mysrp.py`

 * *Files identical despite different names*

