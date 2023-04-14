# Comparing `tmp/bnipython-0.5.0.tar.gz` & `tmp/bnipython-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/tmpzl9o4z6s/bnipython-0.5.0.tar", last modified: Mon Nov 14 15:30:27 2022, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-4nzqzhe0/bnipython-0.6.0.tar", last modified: Fri Apr 14 09:13:26 2023, max compression
```

## Comparing `bnipython-0.5.0.tar` & `bnipython-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.117976 bnipython-0.5.0/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.5.0/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2022-11-14 15:30:27.117360 bnipython-0.5.0/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11602 2022-11-14 15:21:13.000000 bnipython-0.5.0/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.100579 bnipython-0.5.0/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2022-09-12 17:25:56.000000 bnipython-0.5.0/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.104832 bnipython-0.5.0/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.108117 bnipython-0.5.0/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2022-11-14 10:59:20.000000 bnipython-0.5.0/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2022-09-12 17:25:56.000000 bnipython-0.5.0/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      956 2022-11-11 07:06:47.000000 bnipython-0.5.0/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.110446 bnipython-0.5.0/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2022-11-14 11:04:46.000000 bnipython-0.5.0/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.113573 bnipython-0.5.0/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1203 2022-11-11 07:12:55.000000 bnipython-0.5.0/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2022-11-14 11:04:07.000000 bnipython-0.5.0/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2450 2022-11-14 15:17:58.000000 bnipython-0.5.0/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2022-11-14 15:30:27.104368 bnipython-0.5.0/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2022-11-14 15:30:27.000000 bnipython-0.5.0/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      426 2022-11-14 15:30:27.000000 bnipython-0.5.0/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2022-11-14 15:30:27.000000 bnipython-0.5.0/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2022-11-14 15:30:27.000000 bnipython-0.5.0/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2022-11-14 15:30:27.000000 bnipython-0.5.0/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2022-11-14 15:30:27.118181 bnipython-0.5.0/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2022-11-14 15:22:06.000000 bnipython-0.5.0/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.058801 bnipython-0.6.0/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.0/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-14 09:13:26.058397 bnipython-0.6.0/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11494 2023-04-14 08:52:10.000000 bnipython-0.6.0/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.045296 bnipython-0.6.0/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.048055 bnipython-0.6.0/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.049881 bnipython-0.6.0/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1056 2023-04-14 08:56:09.000000 bnipython-0.6.0/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.051244 bnipython-0.6.0/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-14 08:52:10.000000 bnipython-0.6.0/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.053787 bnipython-0.6.0/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1251 2023-04-14 08:52:51.000000 bnipython-0.6.0/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-14 08:52:10.000000 bnipython-0.6.0/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.047704 bnipython-0.6.0/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-14 09:13:26.058905 bnipython-0.6.0/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-14 09:12:57.000000 bnipython-0.6.0/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.057023 bnipython-0.6.0/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-14 08:52:16.000000 bnipython-0.6.0/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_util.py
```

### Comparing `bnipython-0.5.0/LICENSE` & `bnipython-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.5.0/PKG-INFO` & `bnipython-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.5.0
+Version: 0.6.0
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,22 +39,14 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
-### 1.3 Using PyPI Install Third Party
-
-```
-pip install requests
-pip install pyOpenSSL
-pip install pytz
-```
-
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
```

### Comparing `bnipython-0.5.0/README.md` & `bnipython-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,14 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
-### 1.3 Using PyPI Install Third Party
-
-```
-pip install requests
-pip install pyOpenSSL
-pip install pytz
-```
-
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
@@ -379,8 +371,8 @@
 ```
 
 ## Get help
 
 * [Digital Services](https://digitalservices.bni.co.id/en/)
 * [API documentation](https://digitalservices.bni.co.id/documentation/public/en)
 * [Stackoverflow](https://stackoverflow.com/users/19817167/bni-api-management)
-* Can't find answer you looking for? email to [apisupport@bni.co.id](mailto:apisupport@bni.co.id)
+* Can't find answer you looking for? email to [apisupport@bni.co.id](mailto:apisupport@bni.co.id)
```

### Comparing `bnipython-0.5.0/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.0/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.5.0/bnipython/lib/api/snapBI.py` & `bnipython-0.6.0/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.5.0/bnipython/lib/bniClient.py` & `bnipython-0.6.0/bnipython/lib/bniClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
         return self.config
 
     def getBaseUrl(self):
         if self.config['env'] == 'dev':
             return constants.DEV_BASE_URL
         elif self.config['env'] == 'sandbox':
             return constants.SANDBOX_BASE_URL
+        elif self.config['env'] == 'sandbox-dev':
+            return constants.SANDBOX_DEV_BASE_URL
         elif self.config['env'] == 'prod':
             return constants.PRODUCTION_BASE_URL
 
     def getToken(self):
         token = self.httpClient.tokenRequest({
             'url': self.getBaseUrl(),
             'path': '/api/oauth/token',
```

### Comparing `bnipython-0.5.0/bnipython/lib/net/httpClient.py` & `bnipython-0.6.0/bnipython/lib/net/httpClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             'Content-Type': 'application/x-www-form-urlencoded'
         }
         payload = 'grant_type=client_credentials'
 
         httpClient.request('POST', options['path'], payload, headers)
         res = httpClient.getresponse()
         data = res.read()
+        print(data)
         return json.loads(str(data.decode('utf-8')))
 
     def request(self, options={'method', 'apiKey', 'accessToken', 'url', 'path', 'data'}):
         url = str(options['url']).replace(
             'http://', '').replace('https://', '')
         httpClient = http.client.HTTPSConnection(
             url, context=ssl._create_unverified_context())
```

### Comparing `bnipython-0.5.0/bnipython/lib/util/constants.py` & `bnipython-0.6.0/bnipython/lib/util/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 DEV_BASE_URL = 'https://newapidev.bni.co.id:8066';
 SANDBOX_BASE_URL = 'https://sandbox.bni.co.id';
+SANDBOX_DEV_BASE_URL = 'http://localhost:8080';
 PRODUCTION_BASE_URL = 'https://api.bni.co.id';
 # DEV_OGP_URL = 'https://sandbox.harismawan.com'
 # DEV_SNAP_BI = 'https://dev.harismawan.com'
 TOKEN_JWT = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjbGllbnRJZCI6IklEQk5JVkdWemRDQkJVRkE9IiwiYWNjb3VudE5vIjoiMDExNTQ3NjExNyJ9.ljWtFHL0dHhLPw97U8SVWsFV3fRIJItHlQ-HPqCRUwc'
 APP_NAME = 'Test APP'
 APP_NAME_TEST = 'Test Wawat'
```

### Comparing `bnipython-0.5.0/bnipython/lib/util/response.py` & `bnipython-0.6.0/bnipython/lib/util/response.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.5.0/bnipython/lib/util/utils.py` & `bnipython-0.6.0/bnipython/lib/util/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def getTimestamp():
     return datetime.now(pytz.timezone('Asia/Jakarta')).strftime('%Y-%m-%dT%H:%M:%S+07:00')
 
 
 def generateTokenSignature(params={'privateKeyPath', 'clientId', 'timeStamp'}):
     privateKeyPath = params['privateKeyPath']
     rsaPrivate = privateKeyPath.replace('./', '')
-    keyFile = open(f'./{rsaPrivate}', 'rb')
+    keyFile = open(f'./bnipython/lib/{rsaPrivate}', 'rb')
     key = keyFile.read()
     keyFile.close()
 
     pkey = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
     clienId = params['clientId']
     times = params['timeStamp']
     data = f"{clienId}|{times}"
```

### Comparing `bnipython-0.5.0/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.0/bnipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.5.0
+Version: 0.6.0
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,22 +39,14 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
-### 1.3 Using PyPI Install Third Party
-
-```
-pip install requests
-pip install pyOpenSSL
-pip install pytz
-```
-
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
```

### Comparing `bnipython-0.5.0/setup.py` & `bnipython-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.5.0",
+    version="0.6.0",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

