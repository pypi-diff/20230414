# Comparing `tmp/cronuseosdk-0.0.1.tar.gz` & `tmp/cronuseosdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronuseosdk-0.0.1.tar", last modified: Sat Feb 11 12:44:49 2023, max compression
+gzip compressed data, was "cronuseosdk-0.0.2.tar", last modified: Fri Apr 14 10:15:30 2023, max compression
```

## Comparing `cronuseosdk-0.0.1.tar` & `cronuseosdk-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 12:44:49.609407 cronuseosdk-0.0.1/
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      362 2023-02-11 12:44:49.609068 cronuseosdk-0.0.1/PKG-INFO
--rw-r--r--   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 11:38:46.000000 cronuseosdk-0.0.1/README.md
-drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 12:44:49.602595 cronuseosdk-0.0.1/cronuseosdk/
--rw-r--r--   0 thilinashashimal   (501) staff       (20)       41 2023-02-11 11:57:51.000000 cronuseosdk-0.0.1/cronuseosdk/__init__.py
--rw-r--r--   0 thilinashashimal   (501) staff       (20)     1686 2023-02-11 12:11:01.000000 cronuseosdk-0.0.1/cronuseosdk/cronuseo.py
-drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 12:44:49.605952 cronuseosdk-0.0.1/cronuseosdk.egg-info/
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      362 2023-02-11 12:44:49.000000 cronuseosdk-0.0.1/cronuseosdk.egg-info/PKG-INFO
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      245 2023-02-11 12:44:49.000000 cronuseosdk-0.0.1/cronuseosdk.egg-info/SOURCES.txt
--rw-r--r--   0 thilinashashimal   (501) staff       (20)        1 2023-02-11 12:44:49.000000 cronuseosdk-0.0.1/cronuseosdk.egg-info/dependency_links.txt
--rw-r--r--   0 thilinashashimal   (501) staff       (20)       17 2023-02-11 12:44:49.000000 cronuseosdk-0.0.1/cronuseosdk.egg-info/top_level.txt
--rw-r--r--   0 thilinashashimal   (501) staff       (20)       38 2023-02-11 12:44:49.609539 cronuseosdk-0.0.1/setup.cfg
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      643 2023-02-11 12:38:32.000000 cronuseosdk-0.0.1/setup.py
-drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 12:44:49.607471 cronuseosdk-0.0.1/test/
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      137 2023-02-11 12:00:06.000000 cronuseosdk-0.0.1/test/__init__.py
--rw-r--r--   0 thilinashashimal   (501) staff       (20)      353 2023-02-11 12:12:26.000000 cronuseosdk-0.0.1/test/test_cronuseo.py
+drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-04-14 10:15:30.601559 cronuseosdk-0.0.2/
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      362 2023-04-14 10:15:30.600991 cronuseosdk-0.0.2/PKG-INFO
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)        0 2023-02-11 11:38:46.000000 cronuseosdk-0.0.2/README.md
+drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-04-14 10:15:30.593857 cronuseosdk-0.0.2/cronuseosdk/
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)       41 2023-02-11 11:57:51.000000 cronuseosdk-0.0.2/cronuseosdk/__init__.py
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      884 2023-04-14 09:50:10.000000 cronuseosdk-0.0.2/cronuseosdk/cronuseo.py
+drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-04-14 10:15:30.596810 cronuseosdk-0.0.2/cronuseosdk.egg-info/
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      362 2023-04-14 10:15:30.000000 cronuseosdk-0.0.2/cronuseosdk.egg-info/PKG-INFO
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      245 2023-04-14 10:15:30.000000 cronuseosdk-0.0.2/cronuseosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)        1 2023-04-14 10:15:30.000000 cronuseosdk-0.0.2/cronuseosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)       17 2023-04-14 10:15:30.000000 cronuseosdk-0.0.2/cronuseosdk.egg-info/top_level.txt
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)       38 2023-04-14 10:15:30.601802 cronuseosdk-0.0.2/setup.cfg
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      643 2023-04-14 10:13:02.000000 cronuseosdk-0.0.2/setup.py
+drwxr-xr-x   0 thilinashashimal   (501) staff       (20)        0 2023-04-14 10:15:30.599246 cronuseosdk-0.0.2/test/
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      137 2023-02-11 12:00:06.000000 cronuseosdk-0.0.2/test/__init__.py
+-rw-r--r--   0 thilinashashimal   (501) staff       (20)      233 2023-04-14 09:51:10.000000 cronuseosdk-0.0.2/test/test_cronuseo.py
```

### Comparing `cronuseosdk-0.0.1/cronuseosdk/cronuseo.py` & `cronuseosdk-0.0.2/cronuseosdk/cronuseo.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,36 +5,18 @@
 
     def __init__(self, endpoint, organization, token):
         
         self.__endpoint = endpoint
         self.__organization = organization
         self.__token = token
 
-    def checkPermission(self,username, permission, resource):
+    def checkPermission(self,username, action, resource):
 
-        url = f"{self.__endpoint}/{self.__organization}/permission/check/username"
-        data = json.dumps({"username": username, "permission": permission, "resource": resource})
-        try: 
-            response = requests.post(url, 
-                                data= data, 
-                                headers={"API_KEY": f"{self.__token}",
-                                        "Content-Type": "application/json"}
-                            )
-            response.raise_for_status()
-            return response.json()
-        except requests.exceptions.RequestException as e:
-            raise SystemExit(e)
-
-    def checkPermissions(self,username, permissions, resource):
-
-        url = f"{self.__endpoint}/{self.__organization}/permission/check/multi_actions"
-
-        permissions = [{"permission": permission} for permission in permissions]
-
-        data = json.dumps({"username": username, "permissions": permissions, "resource": resource})
+        url = f"{self.__endpoint}/{self.__organization}/permission/check"
+        data = json.dumps({"username": username, "action": action, "resource": resource})
         try: 
             response = requests.post(url, 
                                 data= data, 
                                 headers={"API_KEY": f"{self.__token}",
                                         "Content-Type": "application/json"}
                             )
             response.raise_for_status()
```

### Comparing `cronuseosdk-0.0.1/setup.py` & `cronuseosdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Cronuseo python SDK'
 LONG_DESCRIPTION = 'Cronuseo python SDK for permission checking'
 
 # Setting up
 setup(
     name="cronuseosdk",
     version=VERSION,
```

