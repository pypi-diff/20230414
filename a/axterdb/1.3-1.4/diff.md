# Comparing `tmp/axterdb-1.3.tar.gz` & `tmp/axterdb-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axterdb-1.3.tar", last modified: Thu Apr 13 06:35:27 2023, max compression
+gzip compressed data, was "axterdb-1.4.tar", last modified: Fri Apr 14 14:34:04 2023, max compression
```

## Comparing `axterdb-1.3.tar` & `axterdb-1.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.938663 axterdb-1.3/
--rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.3/.gitignore
--rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.3/.readthedocs
--rw-rw-rw-   0        0        0     1794 2023-04-13 06:35:27.937658 axterdb-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.794629 axterdb-1.3/axterdb/
--rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.3/axterdb/__init__.py
--rw-rw-rw-   0        0        0    12502 2023-04-13 06:34:22.000000 axterdb-1.3/axterdb/client.py
--rw-rw-rw-   0        0        0     2279 2023-04-13 06:34:17.000000 axterdb-1.3/axterdb/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.826614 axterdb-1.3/axterdb.egg-info/
--rw-rw-rw-   0        0        0     1794 2023-04-13 06:35:27.000000 axterdb-1.3/axterdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-13 06:35:27.000000 axterdb-1.3/axterdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:35:27.000000 axterdb-1.3/axterdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 06:35:27.000000 axterdb-1.3/axterdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.890614 axterdb-1.3/docs/
--rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.3/docs/Makefile
--rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.3/docs/clients.rst
--rw-rw-rw-   0        0        0     2003 2023-04-13 06:34:52.000000 axterdb-1.3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.903608 axterdb-1.3/docs/images/
--rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.3/docs/images/axterdb_logo.ico
--rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.3/docs/images/axterdb_logo.png
--rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.3/docs/index.rst
--rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.3/docs/installing.rst
--rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.3/docs/make.bat
--rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.3/docs/quickstart.rst
--rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.3/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:35:27.927613 axterdb-1.3/examples/
--rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.3/examples/basic.py
--rw-rw-rw-   0        0        0     1741 2023-04-13 06:34:59.000000 axterdb-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:35:27.938663 axterdb-1.3/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.056156 axterdb-1.4/
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.686857 axterdb-1.4/.github/
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.788861 axterdb-1.4/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     2518 2023-04-14 13:31:34.000000 axterdb-1.4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.4/.gitignore
+-rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.4/.readthedocs
+-rw-rw-rw-   0        0        0     1794 2023-04-14 14:34:04.045160 axterdb-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.813441 axterdb-1.4/axterdb/
+-rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.4/axterdb/__init__.py
+-rw-rw-rw-   0        0        0    13152 2023-04-14 14:32:53.000000 axterdb-1.4/axterdb/client.py
+-rw-rw-rw-   0        0        0     2279 2023-04-13 06:34:17.000000 axterdb-1.4/axterdb/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.996054 axterdb-1.4/axterdb.egg-info/
+-rw-rw-rw-   0        0        0     1794 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:03.338054 axterdb-1.4/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.4/docs/Makefile
+-rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.4/docs/clients.rst
+-rw-rw-rw-   0        0        0     2003 2023-04-14 14:33:14.000000 axterdb-1.4/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.012159 axterdb-1.4/docs/images/
+-rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.4/docs/images/axterdb_logo.ico
+-rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.4/docs/images/axterdb_logo.png
+-rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.4/docs/index.rst
+-rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.4/docs/installing.rst
+-rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.4/docs/make.bat
+-rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.4/docs/quickstart.rst
+-rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.4/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.044159 axterdb-1.4/examples/
+-rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.4/examples/basic.py
+-rw-rw-rw-   0        0        0     1741 2023-04-14 14:33:19.000000 axterdb-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:34:04.057158 axterdb-1.4/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.4/setup.py
```

### Comparing `axterdb-1.3/.gitignore` & `axterdb-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/PKG-INFO` & `axterdb-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.3
+Version: 1.4
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.3/README.rst` & `axterdb-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/axterdb/client.py` & `axterdb-1.4/axterdb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 import aiohttp
 from aiohttp.client_exceptions import ClientConnectionError
 import asyncio
 
 import ipaddress
 import atexit
 import logging
+import time
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(filename="axterdb.log", filemode="w", level=logging.INFO, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 class Client():
     def __init__(self, *, name: str, key: str, host: str, show_keys: bool = False):
 
         self.name: str = name
         self.key: str = key
         self.host: str = host
         self.show_keys: bool = show_keys
+        self.latency: float
 
         self._headers: dict = {"KEY": f"{self.key}"}
         self._session: aiohttp.ClientSession = None
         self._connected: bool = False
         self._accepted_types = ["TEXT", "INT", "REAL", "NULL"]
 
     async def connect(self):
@@ -85,15 +87,18 @@
             Key specified does not have access to the specified database
         AlreadyConnected
             Already connected to the specified database.
         """
         logger.log(logging.INFO, f"Checking access for key {self.key if self.show_keys else '[HIDDEN]'} to {self.name}")
         if self._connected:
             raise AlreadyConnected(self.host, self.key, self.name, self.show_keys)
+        start_time = time.time()
         async with self._session.get(self.route(f"/me"), headers=self._headers) as response:
+            end_time = time.time()
+            self.latency: float = end_time - start_time
             if response.status == 200:
                 data = await response.json()
                 databases = data["detail"]["data"]["Databases"]
                 if self.name not in databases:
                     raise NoAccess(self.host, self.key, self.name, self.show_keys)
                 else:
                     print(f"Connected to {self.name}! (Instance: {self.host} | Key: {self.key if self.show_keys else '[HIDDEN]'})")
@@ -173,30 +178,29 @@
             Returns a list of lists containing data, or an empty list if no data was found.
 
         Raises
         ------
         NotConnected
             Not connected to the database.
         """
-        print(asyncio.get_event_loop().is_closed())
         if not self._connected:
             raise NotConnected()
         data = kwargs
         headers = self._headers
         headers["table"] = table
         if amount: headers["amount"] = str(amount)
         async with self._session.get(self.route(f"/database/{self.name}/select"), headers=headers, json=data) as response:
             if response.status == 200:
                 data = await response.json()
                 rows = data["detail"]["rows"]
                 return rows
             elif response.status == 422:
                 data = await response.json()
                 error = data["detail"]["message"]
-                table_name = error.replace("No such column found with the name", "")
+                table_name = error.replace("No column found with the name ", "")
                 raise InvalidColumn(table_name)
             raise UnknownError(response.status)
             # TODO: Add errors for this
             
     async def insert(self, table: str, **data) -> bool:
         """|coro|
         Insert data into a table
@@ -231,22 +235,43 @@
             elif response.status == 422:
                 data = await response.json()
                 raise InvalidColumn(data["detail"].split(' ').pop(0))
             raise UnknownError(response.status)
             # TODO: Add errors from status codes.
 
     async def delete(self, table: str, **data) -> bool:
+        """|coro|
+        Deletes data from a table
+
+        Parameters
+        ----------
+        table: :class:`str`
+            The table to delete data from.
+        **data
+            Additional arguments are used as data to delete. 
+            
+        Returns
+        -------
+        :class:`bool`
+            Returns True if query executed sucessfully.
+
+        Raises
+        ------
+        NotConnected
+            Not connected to the database.
+        """
         if not self._connected:
             raise NotConnected()
         data = data
         headers = self._headers
         headers["table"] = table
         async with self._session.get(self.route(f"/database/{self.name}/delete"), headers=headers, json=data) as response:
             if response.status == 200:
                 return True
+            raise UnknownError(response.status)
 
     async def get_all_tables(self) -> None:
         """|coro|
         Get all tables of the database
             
         Returns
         -------
```

### Comparing `axterdb-1.3/axterdb/errors.py` & `axterdb-1.4/axterdb/errors.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/axterdb.egg-info/PKG-INFO` & `axterdb-1.4/axterdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.3
+Version: 1.4
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.3/docs/Makefile` & `axterdb-1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/conf.py` & `axterdb-1.4/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import os
 
 project = 'AxterDB'
 copyright = '2023, AxterDB'
 author = 'ItsNeil'
-release = '1.3'
+release = '1.4'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 sys.path.insert(0, os.path.abspath(".."))
 sys.path.append(os.path.abspath("extensions"))
```

### Comparing `axterdb-1.3/docs/images/axterdb_logo.ico` & `axterdb-1.4/docs/images/axterdb_logo.ico`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/images/axterdb_logo.png` & `axterdb-1.4/docs/images/axterdb_logo.png`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/index.rst` & `axterdb-1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/installing.rst` & `axterdb-1.4/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/make.bat` & `axterdb-1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/docs/quickstart.rst` & `axterdb-1.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/examples/basic.py` & `axterdb-1.4/examples/basic.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.3/pyproject.toml` & `axterdb-1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62.6,<66",
     "setuptools-scm>=6.2,<8",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axterdb"
-version = "1.3"
+version = "1.4"
 authors = [
     {name = "AxterDB Development"}
 ]
 description = "A Python wrapper for AxterDB"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

