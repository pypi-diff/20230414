# Comparing `tmp/doe-dap-dl-0.1.0.tar.gz` & `tmp/doe-dap-dl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doe-dap-dl-0.1.0.tar", last modified: Fri Apr 14 20:16:21 2023, max compression
+gzip compressed data, was "doe-dap-dl-0.3.0.tar", last modified: Thu Apr  6 22:09:45 2023, max compression
```

## Comparing `doe-dap-dl-0.1.0.tar` & `doe-dap-dl-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:21.530741 doe-dap-dl-0.1.0/
--rw-rw-rw-   0        0        0     1103 2023-03-23 22:00:38.000000 doe-dap-dl-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     1866 2023-04-14 20:16:21.528743 doe-dap-dl-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-04-11 20:24:02.000000 doe-dap-dl-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:21.465748 doe-dap-dl-0.1.0/doe_dap_dl/
--rw-rw-rw-   0        0        0       22 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/doe_dap_dl/__init__.py
--rw-rw-rw-   0        0        0    25076 2023-04-14 20:14:24.000000 doe-dap-dl-0.1.0/doe_dap_dl/dap.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:21.514744 doe-dap-dl-0.1.0/doe_dap_dl/plot/
--rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/doe_dap_dl/plot/__init__.py
--rw-rw-rw-   0        0        0    11499 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/doe_dap_dl/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:21.524744 doe-dap-dl-0.1.0/doe_dap_dl/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/doe_dap_dl/utils/__init__.py
--rw-rw-rw-   0        0        0      944 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/doe_dap_dl/utils/scraper.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:21.508746 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/
--rw-rw-rw-   0        0        0     1866 2023-04-14 20:16:21.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-14 20:16:21.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:16:21.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-06 21:30:01.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-14 20:16:21.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 20:16:21.000000 doe-dap-dl-0.1.0/doe_dap_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 20:16:21.530741 doe-dap-dl-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1617 2023-04-11 16:40:22.000000 doe-dap-dl-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-06 22:09:45.595138 doe-dap-dl-0.3.0/
+-rw-rw-rw-   0        0        0     1103 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1617 2023-04-06 22:09:45.593141 doe-dap-dl-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-04-06 22:01:36.000000 doe-dap-dl-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-06 22:09:45.536144 doe-dap-dl-0.3.0/doe_dap_dl/
+-rw-rw-rw-   0        0        0       22 2023-03-30 00:32:00.000000 doe-dap-dl-0.3.0/doe_dap_dl/__init__.py
+-rw-rw-rw-   0        0        0    24462 2023-04-06 19:28:19.000000 doe-dap-dl-0.3.0/doe_dap_dl/dap.py
+drwxrwxrwx   0        0        0        0 2023-04-06 22:09:45.586138 doe-dap-dl-0.3.0/doe_dap_dl/plot/
+-rw-rw-rw-   0        0        0        0 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.0/doe_dap_dl/plot/__init__.py
+-rw-rw-rw-   0        0        0    11499 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.0/doe_dap_dl/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-04-06 22:09:45.591137 doe-dap-dl-0.3.0/doe_dap_dl/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.0/doe_dap_dl/utils/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.0/doe_dap_dl/utils/scraper.py
+drwxrwxrwx   0        0        0        0 2023-04-06 22:09:45.582138 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/
+-rw-rw-rw-   0        0        0     1617 2023-04-06 22:09:45.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-06 22:09:45.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-06 22:09:45.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-06 21:30:01.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-06 22:09:45.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-06 22:09:45.000000 doe-dap-dl-0.3.0/doe_dap_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-06 22:09:45.595138 doe-dap-dl-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2023-04-06 22:09:05.000000 doe-dap-dl-0.3.0/setup.py
```

### Comparing `doe-dap-dl-0.1.0/LICENSE.md` & `doe-dap-dl-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.1.0/PKG-INFO` & `doe-dap-dl-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doe-dap-dl
-Version: 0.1.0
+Version: 0.3.0
 Summary: Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.
 Home-page: https://github.com/DAP-platform/dap-py
 Author: DAP-Platform
 Author-email: dapteam@pnnl.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -19,20 +19,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # doe-dap-dl
 
 This repository contains useful packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform. Users will be able to import these packages and call high-level functions that handle all of the api calls, graphing, and interpolations to stream-line the end user's ability to analyze data.
 
-## Example
+### Example:
 
 ```python
 from doe_dap_dl import DAP
 a2e = DAP('a2e.energy.gov')
 
+# authentication
 a2e.setup_basic_auth(username='username', password='password')
 
 # Search for files
 filter = {
     'Dataset': 'wfip2/lidar.z04.a0',
     'date_time': {
         'between': ['20151004000000', '20151004020000']
@@ -42,12 +43,8 @@
 
 file_names = a2e.search(filter)
 
 # download files
 files = a2e.download_files(file_names)
 ```
 
-[Main docs](https://github.com/DAP-platform/dap-py/blob/master/docs/doe_dap_dl.md)
-[Search query docs](https://github.com/DAP-platform/dap-py/blob/master/docs/download-README.md)
-[Plotting docs](https://github.com/DAP-platform/dap-py/blob/master/docs/plotting.md)
-
```

### Comparing `doe-dap-dl-0.1.0/doe_dap_dl/dap.py` & `doe-dap-dl-0.3.0/doe_dap_dl/dap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import base64
-import json
 import os
+import json
+import base64
+from pathlib import Path
 import requests
-import sys
-import traceback
-
 from getpass import getpass
-from pathlib import Path
+import traceback
 
 from .utils.scraper import get_api_url
 
 
 class BadStatusCodeError(RuntimeError):
     def __init__(self, req):
         self.status_code = req.status_code
@@ -30,25 +28,27 @@
 class DAP:
     def __init__(
         self,
         host_URL,
         cert_path=None,
         save_cert_dir=None,
         download_dir=None,
+        setup_guest_auth=True,
         quiet=False,
         spp=False,
         confirm_downloads=True,
     ):
         """initializes connection with DAP server and performs authentication
 
         Args:
             host_URL (str): The url of the host, e.g. "livewire.energy.gov"
             cert_path (str, optional): path to authentication certificate file. Defaults to None.
             save_cert_dir (str, optional): Path to directory where certificates are stored. Defaults to None
             download_dir (str, optional): Path to directory where files will be downloaded. Defaults to None
+            setup_guest_auth (bool, optional): Whether to set up guest auth if the certificate is invalid or not provided. Defaults to True
             quiet (bool, optional): suppresses output print statemens. Useful for scripting. Defaults to False.
             spp (bool, optional): If this is a dap for the Solid Phase Processing data. Defaults to False.
             confirm_downloads (bool, optional): Whether or not to confirm before downloading. Defaults to True.
         """
         self.host_URL = host_URL
         if spp:
             self._api_url = (
@@ -84,67 +84,63 @@
         self.__print(f"Looking for a certificate: {self._cert_path}...")
         found_cert = False
         if os.path.isfile(self._cert_path):
             self.__print("Found it!")
             found_cert = True
         else:
             self.__print("Certificate not found.")
-            self.__print_setup_authentication()
+            if setup_guest_auth:
+                self.__print(
+                    "Setting up guest authentication since no certificate was found..."
+                )
+                self.setup_guest_auth()
 
         if found_cert:
             self.__read_cert()
 
             if self.__cert_is_valid():
                 self.__create_cert_auth()
                 self.__print(
                     "Authenticaion successfully created using valid certificate."
                 )
             else:
                 self.__print("Certificate was invalid.")
-                self.__print_setup_authentication()
+                if setup_guest_auth:
+                    self.__print(
+                        "Setting up guest authentication since the certificate was invalid..."
+                    )
+                    self.setup_guest_auth()
 
     def __print(self, *args, sep="", end="\n", file=None):
         if not self._quiet:
             for arg in args:
                 print(arg, sep=sep, end=end, file=file)
 
     def __create_dirs(self):
         Path(self.save_cert_dir).mkdir(parents=True, exist_ok=True)
         Path(self.download_dir).mkdir(parents=True, exist_ok=True)
 
     # --------------------------------------------------------------
     # Getting Authenticated
     # --------------------------------------------------------------
 
-    def __validate_response(self, response):
-        if response.status_code != 200:
-            raise BadStatusCodeError(response)
-
-        text = response.text
-        if "errorMessage" in text:
-            error = text.split(",")[0].split("=")[1]
-            self.__print(f"Error: {error}")
-            return False
-
-        return True
-
     def __request_cert(self, params):
         """Request a certificate"""
-        response = requests.put(f"{self._api_url}/creds", params=params)
+        req = requests.put(f"{self._api_url}/creds", params=params)
 
-        if not self.__validate_response(response):
-            return
+        if req.status_code != 200:
+            raise BadStatusCodeError(req)
 
-        self._cert = json.loads(response.text)["cert"]
+        self._cert = json.loads(req.text)["cert"]
         self.__save_cert()
 
     def __create_cert_auth(self):
         """Given an existing certificate, create an auth token"""
         if not self._cert:
-            raise ValueError("Could not create cert auth, missing certificate.")
+            raise ValueError("cert cannot be None")
 
         encoded_cert = base64.b64encode(self._cert.encode("utf-8")).decode("ascii")
         self._auth = {"Authorization": f"Cert {encoded_cert}"}
 
     def __request_cert_auth(self, params):
         """Requests certificate and creates auth token"""
         try:
@@ -177,14 +173,18 @@
 
         self._auth = {"Authorization": f"Basic {user_pass_encoded}"}
         self.__print(f"Authentication created for {username}.")
         # TODO: check if the creds are valid
         # without a certificate
         # should we try a query? low priority
 
+    def setup_guest_auth(self):
+        """Set up basic auth as a guest"""
+        self.setup_basic_auth("guest", "guest")
+
     def setup_cert_auth(self, username=None, password=None):
         """Given username and password request a cert token and generate a
            certificate
 
         Args:
             username (str, optional): Username, if None it will prompt. Defaults to None.
             password (str, optional): Password, if None it will prompt. Defaults to None.
@@ -314,16 +314,15 @@
             table (str, optional): Which table to query. Either 'inventory' or 'stats'. Defaults to 'inventory'.
             latest (bool, optional): Whether to only include the latest files. Defaults to True.
 
         Returns:
             list: The list of file information returned by the filter.
         """
 
-        if not self.__check_for_auth(action="search"):
-            return
+        self.__check_for_auth()
 
         if "livewire" not in self.host_URL:
             filter_arg["latest"] = latest
 
         if "test" in self.host_URL and not table.endswith("-test"):
             self.__print(
                 "You're trying to access data on a test server, but the table name doesn't include 'test', adding it."
@@ -359,33 +358,35 @@
 
     # --------------------------------------------------------------
     # Placing Orders
     # --------------------------------------------------------------
 
     def __place_order(self, dataset, filter_arg):
         """Place an order and return the order ID"""
+        self.__check_for_auth()
 
         params = {"datasets": {f"{dataset}": {"query": filter_arg}}}
 
-        response = requests.put(
+        req = requests.put(
             f"{self._api_url}/orders", headers=self._auth, data=json.dumps(params)
         )
 
-        if not self.__validate_response(response):
-            return
+        if req.status_code != 200:
+            raise BadStatusCodeError(req)
 
-        ID = json.loads(response.text)["id"]
+        ID = json.loads(req.text)["id"]
         return ID
 
     # --------------------------------------------------------------
     # Getting download URLs
     # --------------------------------------------------------------
 
     def __get_download_urls(self, ID, page_size=500):
         """Given order ID, return the download urls"""
+        self.__check_for_auth()
 
         urls = []
         cursor = None
 
         while True:
             try:
                 new_urls, cursor = self.__get_page_of_download_urls(
@@ -408,42 +409,40 @@
 
     def __get_page_of_download_urls(self, ID, page_size, cursor=None):
         """Return one page of download urls given the order id, cursor and page size"""
         cursor_param = "" if cursor is None else f"&cursor={cursor}"
 
         # self._print(f"cursor param: {cursor_param}")
 
-        response = requests.get(
+        req = requests.get(
             f"{self._api_url}/orders/{ID}/urls?page_size={page_size}{cursor_param}",
             headers=self._auth,
         )
 
-        if not self.__validate_response(response):
-            return
+        if req.status_code != 200:
+            raise BadStatusCodeError(req)
 
-        response = json.loads(response.text)
+        response = json.loads(req.text)
         urls = response["urls"]
         cursor = response["cursor"]
 
         return urls, cursor
 
     # --------------------------------------------------------------
     # Download from URLs
     # --------------------------------------------------------------
 
     def __download(self, url, path):
         """Actually download the files"""
-        response = requests.get(url, stream=True)
-
-        if not self.__validate_response(response):
-            return
-
+        req = requests.get(url, stream=True)
+        if req.status_code != 200:
+            raise BadStatusCodeError(req)
         while True:  # is this needed?
             with open(path, "wb") as fp:
-                for chunk in response.iter_content(chunk_size=1024):
+                for chunk in req.iter_content(chunk_size=1024):
                     fp.write(chunk)
             self.__print(f"Download successful! {path}")
             break
 
     def __download_from_urls(self, urls, path="/var/tmp/", replace=False):
         """Given a list of urls, download them
         Returns the successfully downloaded file paths
@@ -494,49 +493,41 @@
             files (list): A list of files obtained via search()
             path (str, optional): The download path. Defaults to "/var/tmp/".
             replace (bool, optional): Whether to redownload and replace existing files. Defaults to False.
 
         Returns:
             list: The list of paths to the downloaded files.
         """
-        if not self.__check_for_auth("download files"):
-            return
+        self.__check_for_auth()
 
         if not files:
             self.__print("No files provided.")
 
         filter = {
             "output": "json",
             "filter": None,
         }
 
         urls = []
         found = 0
         not_found = 0
         for f in files:
             filename = f["Filename"]
-            dataset = f["Dataset"]
 
-            filter["filter"] = {
-                "Filename" : filename,
-                "Dataset" : dataset,
-            }
-            if "date_time" in f:
-                filter["filter"]["date_time"] = f["date_time"]
+            filter["filter"] = f
 
-            response = requests.post(
+            req = requests.post(
                 f"{self._api_url}/downloads",
                 headers=self._auth,
                 data=json.dumps(filter),
             )
 
-            if not self.__validate_response(response):
-                return
+            req.raise_for_status()
 
-            url = json.loads(response.text)["urls"].values()
+            url = json.loads(req.text)["urls"].values()
 
             # this should only return one url
             if len(url) != 1:
                 self.__print(
                     f"found {len(url)} urls instead of one for file {filename}"
                 )
                 not_found += 1
@@ -569,40 +560,40 @@
     # --------------------------------------------------------------
 
     def __search_for_urls(self, filter_arg):
         """uses the alternative api /downloads method
         to search the inventory table and return
         the download urls to files in s3
         """
+        self.__check_for_auth()
 
-        response = requests.post(
+        req = requests.post(
             f"{self._api_url}/downloads",
             headers=self._auth,
             data=json.dumps(filter_arg),
         )
 
-        if not self.__validate_response(response):
-            return
+        if req.status_code != 200:
+            raise BadStatusCodeError(req)
 
-        urls = json.loads(response.text)["urls"].values()
+        urls = json.loads(req.text)["urls"].values()
         return urls
 
     def download_search(self, filter_arg, path="/var/tmp/", replace=False):
         """Download files straight from a search without placing an order
 
         Args:
             filter_arg (dict): The filter argument. For information on how to construct this see download-README.md
             path (str, optional): The download path. Defaults to '/var/tmp/'.
             replace (bool, optional): Whether to redownload and replace existing files. Defaults to False.
 
         Returns:
             list: The list of paths to the downloaded files.
         """
-        if not self.__check_for_auth("download via search"):
-            return
+
         try:
             urls = self.__search_for_urls(
                 {
                     "output": "json",
                     "filter": filter_arg,
                 }
             )
@@ -641,18 +632,14 @@
         filter_arg (dict): The filter argument. For information on how to construct this see download-README.md
         path (str, optional): The download path. Defaults to '/var/tmp/'.
         replace (bool, optional): Whether to redownload and replace existing files. Defaults to False.
 
         Returns:
             list: The list of paths to the downloaded files.
         """
-
-        if not self.__check_for_auth("download by placing an order"):
-            return
-
         dataset = filter_arg["Dataset"]
 
         if not dataset:
             raise Exception("No dataset provided!")
 
         self.__print("Attempting to place an order for the data...")
 
@@ -698,21 +685,12 @@
             if proceed.lower() not in ("y", "n"):
                 print("Enter either y or n")
             else:
                 break
 
         return proceed == "y"
 
-    def __check_for_auth(self, action=""):
+    def __check_for_auth(self):
         if not self._auth:
-            self.__print_setup_authentication(action)
-            return False
-        return True
-
-    def __print_setup_authentication(self, action=""):
-        if action != "":
-            start = f"You will need to authenticate to {action}."
-        else:
-            start = f"You will need to authenticate to use this module further."
-
-        self.__print(f"{start} Set up authentication with setup_basic_auth(), setup_cert_auth(), or setup_two_factor_auth().")
-        self.__print("More information available in the docs: https://github.com/DAP-platform/dap-py/blob/master/docs/doe_dap_dl.md")
+            raise Exception(
+                "No authentication has been set up. To create authentication use either setup_guest_auth(), setup_basic_auth(), setup_cert_auth(), or setup_two_factor_auth()"
+            )
```

### Comparing `doe-dap-dl-0.1.0/doe_dap_dl/plot/plot.py` & `doe-dap-dl-0.3.0/doe_dap_dl/plot/plot.py`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.1.0/doe_dap_dl/utils/scraper.py` & `doe-dap-dl-0.3.0/doe_dap_dl/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.1.0/doe_dap_dl.egg-info/PKG-INFO` & `doe-dap-dl-0.3.0/doe_dap_dl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doe-dap-dl
-Version: 0.1.0
+Version: 0.3.0
 Summary: Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.
 Home-page: https://github.com/DAP-platform/dap-py
 Author: DAP-Platform
 Author-email: dapteam@pnnl.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -19,20 +19,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # doe-dap-dl
 
 This repository contains useful packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform. Users will be able to import these packages and call high-level functions that handle all of the api calls, graphing, and interpolations to stream-line the end user's ability to analyze data.
 
-## Example
+### Example:
 
 ```python
 from doe_dap_dl import DAP
 a2e = DAP('a2e.energy.gov')
 
+# authentication
 a2e.setup_basic_auth(username='username', password='password')
 
 # Search for files
 filter = {
     'Dataset': 'wfip2/lidar.z04.a0',
     'date_time': {
         'between': ['20151004000000', '20151004020000']
@@ -42,12 +43,8 @@
 
 file_names = a2e.search(filter)
 
 # download files
 files = a2e.download_files(file_names)
 ```
 
-[Main docs](https://github.com/DAP-platform/dap-py/blob/master/docs/doe_dap_dl.md)
-[Search query docs](https://github.com/DAP-platform/dap-py/blob/master/docs/download-README.md)
-[Plotting docs](https://github.com/DAP-platform/dap-py/blob/master/docs/plotting.md)
-
```

### Comparing `doe-dap-dl-0.1.0/setup.py` & `doe-dap-dl-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the list of dependencies from the requirements.txt file
 with open(os.path.join(CWD, "requirements.txt")) as requirements_file:
     # Parse requirements.txt, ignoring any commented-out lines.
     REQUIREMENTS = [
         line for line in requirements_file.read().splitlines() if not line.startswith("#")
     ]
 
-version = "0.1.0"
+version = "0.3.0"
 assert "." in version
 
 setuptools.setup(
     name="doe-dap-dl",
     version=version,
     description="Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.",
     long_description=README,
```

