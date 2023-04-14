# Comparing `tmp/quorum_mininode_py-1.2.1.tar.gz` & `tmp/quorum_mininode_py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.1.tar", last modified: Thu Apr  6 13:41:15 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.2.2.tar", last modified: Fri Apr 14 14:10:04 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.1.tar` & `quorum_mininode_py-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.732454 quorum_mininode_py-1.2.1/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-04-06 13:41:15.731456 quorum_mininode_py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.678598 quorum_mininode_py-1.2.1/quorum_mininode_py/
--rw-rw-rw-   0        0        0      607 2023-04-06 13:36:39.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.697547 quorum_mininode_py-1.2.1/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     2339 2023-03-30 11:03:37.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.706525 quorum_mininode_py-1.2.1/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-03-30 05:11:33.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     3377 2023-04-06 13:36:11.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.719490 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.724476 quorum_mininode_py-1.2.1/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.729462 quorum_mininode_py-1.2.1/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-06 11:35:51.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.1/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:41:15.691566 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-04-06 13:41:15.000000 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-06 13:41:15.000000 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:41:15.000000 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-06 13:41:15.000000 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-06 13:41:15.000000 quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 13:41:15.732454 quorum_mininode_py-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-04-06 13:16:19.000000 quorum_mininode_py-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.680225 quorum_mininode_py-1.2.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-04-14 14:10:04.679228 quorum_mininode_py-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.610412 quorum_mininode_py-1.2.2/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      607 2023-04-14 13:58:34.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.628366 quorum_mininode_py-1.2.2/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     2339 2023-03-30 11:03:37.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.635346 quorum_mininode_py-1.2.2/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-03-30 05:11:33.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     3486 2023-04-14 13:57:42.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.647313 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.672247 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.676262 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-06 11:35:51.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.622381 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:10:04.681223 quorum_mininode_py-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1301 2023-04-14 13:58:23.000000 quorum_mininode_py-1.2.2/setup.py
```

### Comparing `quorum_mininode_py-1.2.1/LICENSE` & `quorum_mininode_py-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/PKG-INFO` & `quorum_mininode_py-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_mininode_py
-Version: 1.2.1
+Version: 1.2.2
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.1/README.md` & `quorum_mininode_py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/__init__.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     create_age_keypair,
     create_private_key,
     private_key_to_pubkey,
     public_key_to_address,
 )
 from quorum_mininode_py.utils import decode_seed_url, update_seed_url
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __author__ = "liujuanjuan1984, zhangwm404"
 
 # Set default logging handler to avoid "No handler found" warnings.
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 logger.info("Version: %s", __version__)
```

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/api/base.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/api/base.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/api/lightnode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/client/_http.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/client/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/client/mininode.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/client/mininode.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     seed_url: str = None
     group_id: str = None
     aes_key: str = None
     encryption_type: str = None
     chain_urls: list = None
 
     def __init__(self, seed_url: str):
-        info = utils.decode_seed_url(seed_url)
+        try:
+            info = utils.decode_seed_url(seed_url)
+        except KeyError as err:
+            raise ValueError(f"invalid seed_url: {err}")
         seed = info["seed"]
         self.seed = seed
         self.seed_url = seed_url
         self.group_id = seed["group_id"]
         self.aes_key = bytes.fromhex(seed["cipher_key"])
         self.encryption_type = seed["encryption_type"]
         self.chain_urls = info["chain_urls"]
```

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/account.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/age.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/age.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/crypto/trx.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/trx.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.2.2/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-mininode-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.1/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.1/setup.py` & `quorum_mininode_py-1.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.1",
+    version="1.2.2",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
```

