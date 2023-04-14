# Comparing `tmp/cbmc.py-0.0.1.tar.gz` & `tmp/cbmc.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmc.py-0.0.1.tar", last modified: Thu Apr 13 22:25:45 2023, max compression
+gzip compressed data, was "cbmc.py-0.0.2.tar", last modified: Fri Apr 14 01:13:09 2023, max compression
```

## Comparing `cbmc.py-0.0.1.tar` & `cbmc.py-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-04-13 22:25:45.592307 cbmc.py-0.0.1/
--rw-r--r--   0 ryan       (501) staff       (20)     1084 2023-04-13 22:25:10.000000 cbmc.py-0.0.1/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      981 2023-04-13 22:25:45.591939 cbmc.py-0.0.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      475 2023-04-13 22:12:47.000000 cbmc.py-0.0.1/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-04-13 22:25:45.588483 cbmc.py-0.0.1/cbmc/
--rw-r--r--   0 ryan       (501) staff       (20)      303 2023-04-13 22:25:11.000000 cbmc.py-0.0.1/cbmc/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     6401 2023-04-13 22:25:11.000000 cbmc.py-0.0.1/cbmc/api.py
--rw-r--r--   0 ryan       (501) staff       (20)     1587 2023-04-13 22:25:10.000000 cbmc.py-0.0.1/cbmc/exception.py
--rw-r--r--   0 ryan       (501) staff       (20)     5103 2023-04-13 22:25:11.000000 cbmc.py-0.0.1/cbmc/post.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-04-13 22:25:45.591199 cbmc.py-0.0.1/cbmc.py.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      981 2023-04-13 22:25:45.000000 cbmc.py-0.0.1/cbmc.py.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      240 2023-04-13 22:25:45.000000 cbmc.py-0.0.1/cbmc.py.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-04-13 22:25:45.000000 cbmc.py-0.0.1/cbmc.py.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       17 2023-04-13 22:25:45.000000 cbmc.py-0.0.1/cbmc.py.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        5 2023-04-13 22:25:45.000000 cbmc.py-0.0.1/cbmc.py.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-04-13 22:25:45.592421 cbmc.py-0.0.1/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      786 2023-04-13 22:25:11.000000 cbmc.py-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/cbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/cbmc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/setup.py
```

### Comparing `cbmc.py-0.0.1/LICENSE` & `cbmc.py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.1/PKG-INFO` & `cbmc.py-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial 麥塊匿名發文平台 API wrapper.
 Home-page: https://github.com/ItsRqtl/cbmc.py
 Author: ItsRqtl
 Author-email: itsrql@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 # cbmc.py
 
 Unofficial 麥塊匿名發文平台 API Wrapper for Python
 
 ## Installation
 
 ```sh
-pip install cbmc
+pip install cbmc.py
 ```
 
 ## Usage
 
 ```py
 # Import the library
 from cbmc import AsyncCbmc, SyncCbmc
```

### Comparing `cbmc.py-0.0.1/cbmc/api.py` & `cbmc.py-0.0.2/cbmc/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         if limit > 300 or limit < 1:
             raise ValueError("The maximum number of posts to return must be between 1 and 300.")
         url = f"{cls.base_url}/latest?limit={limit}"
         with requests.get(url) as resp:
             if resp.status_code == 200:
                 data = resp.json()
                 if data["status"] == "success" and "posts" in data:
-                    return [Post(i) for i in data["posts"]]
+                    return [Post(i["post"]) for i in data["posts"].values()]
             raise HTTPException(f"HTTP request failed with status code {resp.status_code}.")
 
     @classmethod
     def get_status(cls, code: str) -> dict:
         """
         Get a status by its code.
 
@@ -169,15 +169,15 @@
             raise ValueError("The maximum number of posts to return must be between 1 and 300.")
         url = f"{cls.base_url}/latest?limit={limit}"
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
                 if resp.status == 200:
                     data = await resp.json()
                     if data["status"] == "success" and "posts" in data:
-                        return [Post(i) for i in data["posts"]]
+                        return [Post(i["post"]) for i in data["posts"].values()]
                 raise HTTPException(f"HTTP request failed with status code {resp.status}.")
 
     @classmethod
     async def get_status(cls, code: str) -> dict:
         """
         Get a status by its code.
```

### Comparing `cbmc.py-0.0.1/cbmc/exception.py` & `cbmc.py-0.0.2/cbmc/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 SOFTWARE.
 """
 
 __all__ = [
     "CbmcException",
     "CbmcAPIException",
     "NotFound",
+    "HTTPException",
 ]
 
 
 class CbmcException(Exception):
     """
     The base exception class for the CBMC API.
     """
```

### Comparing `cbmc.py-0.0.1/cbmc/post.py` & `cbmc.py-0.0.2/cbmc/post.py`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.1/cbmc.py.egg-info/PKG-INFO` & `cbmc.py-0.0.2/cbmc.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial 麥塊匿名發文平台 API wrapper.
 Home-page: https://github.com/ItsRqtl/cbmc.py
 Author: ItsRqtl
 Author-email: itsrql@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 # cbmc.py
 
 Unofficial 麥塊匿名發文平台 API Wrapper for Python
 
 ## Installation
 
 ```sh
-pip install cbmc
+pip install cbmc.py
 ```
 
 ## Usage
 
 ```py
 # Import the library
 from cbmc import AsyncCbmc, SyncCbmc
```

### Comparing `cbmc.py-0.0.1/setup.py` & `cbmc.py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 setup(
     name="cbmc.py",
     version=VERSION,
     author="ItsRqtl",
     author_email="itsrql@gmail.com",
     description="An unofficial 麥塊匿名發文平台 API wrapper.",
```

