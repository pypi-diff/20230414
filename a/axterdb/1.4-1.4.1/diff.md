# Comparing `tmp/axterdb-1.4.tar.gz` & `tmp/axterdb-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axterdb-1.4.tar", last modified: Fri Apr 14 14:34:04 2023, max compression
+gzip compressed data, was "axterdb-1.4.1.tar", last modified: Fri Apr 14 15:08:36 2023, max compression
```

## Comparing `axterdb-1.4.tar` & `axterdb-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.056156 axterdb-1.4/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.686857 axterdb-1.4/.github/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.788861 axterdb-1.4/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0     2518 2023-04-14 13:31:34.000000 axterdb-1.4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.4/.gitignore
--rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.4/.readthedocs
--rw-rw-rw-   0        0        0     1794 2023-04-14 14:34:04.045160 axterdb-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.813441 axterdb-1.4/axterdb/
--rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.4/axterdb/__init__.py
--rw-rw-rw-   0        0        0    13152 2023-04-14 14:32:53.000000 axterdb-1.4/axterdb/client.py
--rw-rw-rw-   0        0        0     2279 2023-04-13 06:34:17.000000 axterdb-1.4/axterdb/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:02.996054 axterdb-1.4/axterdb.egg-info/
--rw-rw-rw-   0        0        0     1794 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 14:34:02.000000 axterdb-1.4/axterdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:03.338054 axterdb-1.4/docs/
--rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.4/docs/Makefile
--rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.4/docs/clients.rst
--rw-rw-rw-   0        0        0     2003 2023-04-14 14:33:14.000000 axterdb-1.4/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.012159 axterdb-1.4/docs/images/
--rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.4/docs/images/axterdb_logo.ico
--rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.4/docs/images/axterdb_logo.png
--rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.4/docs/index.rst
--rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.4/docs/installing.rst
--rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.4/docs/make.bat
--rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.4/docs/quickstart.rst
--rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.4/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:34:04.044159 axterdb-1.4/examples/
--rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.4/examples/basic.py
--rw-rw-rw-   0        0        0     1741 2023-04-14 14:33:19.000000 axterdb-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:34:04.057158 axterdb-1.4/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:36.172302 axterdb-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:35.595291 axterdb-1.4.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:35.608292 axterdb-1.4.1/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     2518 2023-04-14 13:31:34.000000 axterdb-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.4.1/.gitignore
+-rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.4.1/.readthedocs
+-rw-rw-rw-   0        0        0     1796 2023-04-14 15:08:36.171303 axterdb-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:35.804315 axterdb-1.4.1/axterdb/
+-rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.4.1/axterdb/__init__.py
+-rw-rw-rw-   0        0        0    13588 2023-04-14 15:05:17.000000 axterdb-1.4.1/axterdb/client.py
+-rw-rw-rw-   0        0        0     2279 2023-04-13 06:34:17.000000 axterdb-1.4.1/axterdb/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:35.871314 axterdb-1.4.1/axterdb.egg-info/
+-rw-rw-rw-   0        0        0     1796 2023-04-14 15:08:35.000000 axterdb-1.4.1/axterdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-04-14 15:08:35.000000 axterdb-1.4.1/axterdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:08:35.000000 axterdb-1.4.1/axterdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 15:08:35.000000 axterdb-1.4.1/axterdb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:36.022315 axterdb-1.4.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.4.1/docs/Makefile
+-rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.4.1/docs/clients.rst
+-rw-rw-rw-   0        0        0     2005 2023-04-14 15:07:55.000000 axterdb-1.4.1/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:36.038318 axterdb-1.4.1/docs/images/
+-rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.4.1/docs/images/axterdb_logo.ico
+-rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.4.1/docs/images/axterdb_logo.png
+-rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.4.1/docs/index.rst
+-rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.4.1/docs/installing.rst
+-rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.4.1/docs/make.bat
+-rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.4.1/docs/quickstart.rst
+-rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.4.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:36.157317 axterdb-1.4.1/examples/
+-rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.4.1/examples/basic.py
+-rw-rw-rw-   0        0        0     1743 2023-04-14 15:08:20.000000 axterdb-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 15:08:36.173308 axterdb-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.4.1/setup.py
```

### Comparing `axterdb-1.4/.github/ISSUE_TEMPLATE/bug_report.yml` & `axterdb-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/.gitignore` & `axterdb-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/PKG-INFO` & `axterdb-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.4
+Version: 1.4.1
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.4/README.rst` & `axterdb-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/axterdb/client.py` & `axterdb-1.4.1/axterdb/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,14 +264,24 @@
         data = data
         headers = self._headers
         headers["table"] = table
         async with self._session.get(self.route(f"/database/{self.name}/delete"), headers=headers, json=data) as response:
             if response.status == 200:
                 return True
             raise UnknownError(response.status)
+        
+    async def delete_table(self, table: str) -> bool:
+        if not self._connected:
+            raise NotConnected()
+        headers = self._headers
+        headers["table"] = table
+        async with self._session.get(self.route(f"/database/{self.name}/delete_table"), headers=headers) as response:
+            if response.status == 200:
+                return True
+            raise UnknownError(response.status)
 
     async def get_all_tables(self) -> None:
         """|coro|
         Get all tables of the database
             
         Returns
         -------
```

### Comparing `axterdb-1.4/axterdb/errors.py` & `axterdb-1.4.1/axterdb/errors.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/axterdb.egg-info/PKG-INFO` & `axterdb-1.4.1/axterdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.4
+Version: 1.4.1
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.4/docs/Makefile` & `axterdb-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/conf.py` & `axterdb-1.4.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import os
 
 project = 'AxterDB'
 copyright = '2023, AxterDB'
 author = 'ItsNeil'
-release = '1.4'
+release = '1.4.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 sys.path.insert(0, os.path.abspath(".."))
 sys.path.append(os.path.abspath("extensions"))
```

### Comparing `axterdb-1.4/docs/images/axterdb_logo.ico` & `axterdb-1.4.1/docs/images/axterdb_logo.ico`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/images/axterdb_logo.png` & `axterdb-1.4.1/docs/images/axterdb_logo.png`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/index.rst` & `axterdb-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/installing.rst` & `axterdb-1.4.1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/make.bat` & `axterdb-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/docs/quickstart.rst` & `axterdb-1.4.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/examples/basic.py` & `axterdb-1.4.1/examples/basic.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.4/pyproject.toml` & `axterdb-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62.6,<66",
     "setuptools-scm>=6.2,<8",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axterdb"
-version = "1.4"
+version = "1.4.1"
 authors = [
     {name = "AxterDB Development"}
 ]
 description = "A Python wrapper for AxterDB"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

