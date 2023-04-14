# Comparing `tmp/datamarket-0.2.4.tar.gz` & `tmp/datamarket-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.2.4.tar", last modified: Tue Mar 14 14:58:35 2023, max compression
+gzip compressed data, was "datamarket-0.2.5.tar", last modified: Fri Apr 14 11:22:22 2023, max compression
```

## Comparing `datamarket-0.2.4.tar` & `datamarket-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-14 14:58:35.031161 datamarket-0.2.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.2.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-03-14 14:58:35.031161 datamarket-0.2.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2022-08-18 10:42:29.000000 datamarket-0.2.4/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-14 14:58:35.031161 datamarket-0.2.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1019 2023-03-14 06:48:34.000000 datamarket-0.2.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-14 14:58:35.023161 datamarket-0.2.4/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-14 14:58:35.027161 datamarket-0.2.4/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.2.4/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-14 14:58:35.031161 datamarket-0.2.4/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.2.4/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.2.4/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.2.4/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.2.4/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2787 2022-08-08 10:00:49.000000 datamarket-0.2.4/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.2.4/src/datamarket/interfaces/tinybird.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1898 2023-02-09 08:25:23.000000 datamarket-0.2.4/src/datamarket/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-14 14:58:35.027161 datamarket-0.2.4/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-03-14 14:58:35.000000 datamarket-0.2.4/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-14 14:58:35.000000 datamarket-0.2.4/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-14 14:58:35.000000 datamarket-0.2.4/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-03-14 14:58:35.000000 datamarket-0.2.4/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-03-14 14:58:35.000000 datamarket-0.2.4/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.827882 datamarket-0.2.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.2.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-04-14 11:22:22.823882 datamarket-0.2.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2022-08-18 10:42:29.000000 datamarket-0.2.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-14 11:22:22.827882 datamarket-0.2.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1019 2023-04-14 11:21:39.000000 datamarket-0.2.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.2.5/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.2.5/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.2.5/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.2.5/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.2.5/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.2.5/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.2.5/src/datamarket/interfaces/tinybird.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1898 2023-02-09 08:25:23.000000 datamarket-0.2.5/src/datamarket/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.2.4/LICENSE` & `datamarket-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/PKG-INFO` & `datamarket-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.2.4/README.md` & `datamarket-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/setup.py` & `datamarket-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "retry",
     "stem",
     "pydrive",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.2.4",
+    version="0.2.5",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.2.4/src/datamarket/interfaces/alchemy.py` & `datamarket-0.2.5/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/src/datamarket/interfaces/drive.py` & `datamarket-0.2.5/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/src/datamarket/interfaces/ftp.py` & `datamarket-0.2.5/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/src/datamarket/interfaces/proxy.py` & `datamarket-0.2.5/src/datamarket/interfaces/proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ########################################################################################################################
 # IMPORTS
 
 import logging
+import random
 import time
 
 import requests
 from stem import Signal
 from stem.control import Controller
 
 ########################################################################################################################
@@ -18,52 +19,51 @@
 class ProxyInterface:
     CHECK_IP_URL = "https://wtfismyip.com/json"
 
     def __init__(self, config):
         if "proxy" in config:
             self.config = config["proxy"]
 
-            if "host" in self.config and "port" in self.config:
+            if "hosts" in self.config:
                 self.proxies = self.get_proxies(use_tor=False)
 
             elif "tor_password" in self.config:
                 self.proxies = self.get_proxies()
 
             else:
                 raise Exception(
-                    "either host and port or tor_password should be set in proxy configuration"
+                    "either hosts or tor_password should be set in proxy configuration"
                 )
 
         else:
             logger.warning("no proxy section in config")
 
     @staticmethod
     def get_proxy_url(host, port, user=None, password=None, use_socks=True):
         proxy_url = f"{host}:{port}"
 
         if user and password:
             proxy_url = f"{user}:{password}@{proxy_url}"
 
-        if use_socks:
-            proxy_url = f"socks5://{proxy_url}"
-
+        proxy_url = f"socks5://{proxy_url}" if use_socks else f"http://{proxy_url}"
         return proxy_url
 
     def get_proxies(self, use_tor=True):
         if use_tor:
             proxy_url = self.get_proxy_url("127.0.0.1", 9050)
 
         else:
-            host = self.config["host"]
-            port = self.config["port"]
+            host_port_pairs = [hp.split(":") for hp in self.config["hosts"].split(",")]
+            random_host, random_port = random.choice(host_port_pairs)
+
             user = self.config["user"] if "user" in self.config else None
             password = self.config["password"] if "password" in self.config else None
-            use_socks = self.config["socks"].lower() == "true"
+            use_socks = self.config["socks"].lower() == "true" if "socks" in self.config else False
 
-            proxy_url = self.get_proxy_url(host, port, user, password, use_socks)
+            proxy_url = self.get_proxy_url(random_host, random_port, user, password, use_socks)
 
         return {
             "http": proxy_url,
             "https": proxy_url,
         }
 
     def check_current_ip(self):
```

### Comparing `datamarket-0.2.4/src/datamarket/interfaces/tinybird.py` & `datamarket-0.2.5/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/src/datamarket/utils.py` & `datamarket-0.2.5/src/datamarket/utils.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.4/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.2.5/src/datamarket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

