# Comparing `tmp/python_netonix_api-0.2.0.tar.gz` & `tmp/python_netonix_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_netonix_api-0.2.0.tar", last modified: Tue Dec  6 10:21:10 2022, max compression
+gzip compressed data, was "python_netonix_api-0.2.1.tar", last modified: Fri Apr 14 02:36:24 2023, max compression
```

## Comparing `python_netonix_api-0.2.0.tar` & `python_netonix_api-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 salathe   (1000) salathe   (1000)        0 2022-12-06 10:21:10.747551 python_netonix_api-0.2.0/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     1211 2022-12-06 10:20:48.000000 python_netonix_api-0.2.0/LICENSE
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     2941 2022-12-06 10:21:10.747551 python_netonix_api-0.2.0/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      993 2022-12-06 10:20:48.000000 python_netonix_api-0.2.0/README.md
--rwxrwxr-x   0 salathe   (1000) salathe   (1000)     7815 2022-12-06 10:20:48.000000 python_netonix_api-0.2.0/netonix_api.py
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      679 2022-12-06 10:20:48.000000 python_netonix_api-0.2.0/pyproject.toml
-drwxrwxr-x   0 salathe   (1000) salathe   (1000)        0 2022-12-06 10:21:10.747551 python_netonix_api-0.2.0/python_netonix_api.egg-info/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     2941 2022-12-06 10:21:10.000000 python_netonix_api-0.2.0/python_netonix_api.egg-info/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      265 2022-12-06 10:21:10.000000 python_netonix_api-0.2.0/python_netonix_api.egg-info/SOURCES.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)        1 2022-12-06 10:21:10.000000 python_netonix_api-0.2.0/python_netonix_api.egg-info/dependency_links.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       41 2022-12-06 10:21:10.000000 python_netonix_api-0.2.0/python_netonix_api.egg-info/requires.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       12 2022-12-06 10:21:10.000000 python_netonix_api-0.2.0/python_netonix_api.egg-info/top_level.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       38 2022-12-06 10:21:10.747551 python_netonix_api-0.2.0/setup.cfg
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      333 2022-12-04 18:11:55.000000 python_netonix_api-0.2.0/setup.py
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 02:36:24.290776 python_netonix_api-0.2.1/
+-rw-r--r--   0 salathe   (1000) salathe   (1000)     1211 2023-04-14 02:25:34.000000 python_netonix_api-0.2.1/LICENSE
+-rw-r--r--   0 salathe   (1000) salathe   (1000)     2941 2023-04-14 02:36:24.289776 python_netonix_api-0.2.1/PKG-INFO
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      993 2023-04-14 02:25:34.000000 python_netonix_api-0.2.1/README.md
+-rwxr-xr-x   0 salathe   (1000) salathe   (1000)     7875 2023-04-14 02:35:25.000000 python_netonix_api-0.2.1/netonix_api.py
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      679 2023-04-14 02:35:51.000000 python_netonix_api-0.2.1/pyproject.toml
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 02:36:24.289776 python_netonix_api-0.2.1/python_netonix_api.egg-info/
+-rw-r--r--   0 salathe   (1000) salathe   (1000)     2941 2023-04-14 02:36:24.000000 python_netonix_api-0.2.1/python_netonix_api.egg-info/PKG-INFO
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      265 2023-04-14 02:36:24.000000 python_netonix_api-0.2.1/python_netonix_api.egg-info/SOURCES.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)        1 2023-04-14 02:36:24.000000 python_netonix_api-0.2.1/python_netonix_api.egg-info/dependency_links.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       41 2023-04-14 02:36:24.000000 python_netonix_api-0.2.1/python_netonix_api.egg-info/requires.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       12 2023-04-14 02:36:24.000000 python_netonix_api-0.2.1/python_netonix_api.egg-info/top_level.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       38 2023-04-14 02:36:24.290776 python_netonix_api-0.2.1/setup.cfg
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      333 2023-04-14 02:25:34.000000 python_netonix_api-0.2.1/setup.py
```

### Comparing `python_netonix_api-0.2.0/LICENSE` & `python_netonix_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_netonix_api-0.2.0/PKG-INFO` & `python_netonix_api-0.2.1/python_netonix_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_netonix_api
-Version: 0.2.0
+Name: python-netonix-api
+Version: 0.2.1
 Summary: Python class to access Netonix WISP Switch WebAPI
 Home-page: https://github.com/shrank/python_netonix_api
 Author: shrank
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `python_netonix_api-0.2.0/README.md` & `python_netonix_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_netonix_api-0.2.0/netonix_api.py` & `python_netonix_api-0.2.1/netonix_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         print(r.json())
         if(r.status_code != requests.codes.ok):
             raise Exception("Restore Request Failed")
         r = self._get("reboot")
         return r.json()
 
     def getMAC(self):
-        r = self._get("mac")
+        r = self._get("mac", timeout=60)
         if(r.status_code != requests.codes.ok):
             raise Exception("Action failed")
         self.mac = r.json()["MACTable"]
 
     def getID(self):
         r = self._get("id", params={"_": time.time()})
         if(r.status_code != requests.codes.ok):
@@ -228,9 +228,11 @@
 
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     ip = str(input("switch ip:"))
     user = str(input("user:"))
     pw = getpass.getpass("password:")
     n = Netonix()
     n.open(ip, user, pw)
-    n.getStatus()
-    print(json.dumps(n.status, indent=4))
+    n.getMAC()
+    print(json.dumps(n.mac, indent=4))
+    n.getMAC()
+    print(json.dumps(n.mac, indent=4))
```

### Comparing `python_netonix_api-0.2.0/pyproject.toml` & `python_netonix_api-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_netonix_api"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="shrank", email="info@murxs.ch" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 description = "Python class to access Netonix WISP Switch WebAPI"
 requires-python = ">=3.0"
```

### Comparing `python_netonix_api-0.2.0/python_netonix_api.egg-info/PKG-INFO` & `python_netonix_api-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-netonix-api
-Version: 0.2.0
+Name: python_netonix_api
+Version: 0.2.1
 Summary: Python class to access Netonix WISP Switch WebAPI
 Home-page: https://github.com/shrank/python_netonix_api
 Author: shrank
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

