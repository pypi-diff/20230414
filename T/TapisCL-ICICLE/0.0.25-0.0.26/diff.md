# Comparing `tmp/TapisCL-ICICLE-0.0.25.tar.gz` & `tmp/TapisCL-ICICLE-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.25.tar", last modified: Fri Apr 14 18:30:06 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.26.tar", last modified: Fri Apr 14 18:34:16 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.25.tar` & `TapisCL-ICICLE-0.0.26.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/LICENSE
--rw-rw-rw-   0        0        0    43880 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     1970 2023-04-14 17:01:05.000000 TapisCL-ICICLE-0.0.25/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.519628 TapisCL-ICICLE-0.0.25/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10911 2023-04-14 18:13:31.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5132 2023-04-14 18:06:28.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10402 2023-04-14 18:00:07.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    18763 2023-04-14 18:25:04.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.525608 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43880 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-14 18:29:21.000000 TapisCL-ICICLE-0.0.25/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.720619 TapisCL-ICICLE-0.0.26/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/LICENSE
+-rw-rw-rw-   0        0        0    43880 2023-04-14 18:34:16.720619 TapisCL-ICICLE-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     1970 2023-04-14 17:01:05.000000 TapisCL-ICICLE-0.0.26/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.710651 TapisCL-ICICLE-0.0.26/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10950 2023-04-14 18:32:13.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5132 2023-04-14 18:06:28.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10402 2023-04-14 18:00:07.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    18763 2023-04-14 18:25:04.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.719623 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43880 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-14 18:31:46.000000 TapisCL-ICICLE-0.0.26/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 18:34:16.721612 TapisCL-ICICLE-0.0.26/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.25/LICENSE` & `TapisCL-ICICLE-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/PKG-INFO` & `TapisCL-ICICLE-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.25
+Version: 0.0.26
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.25/README.md` & `TapisCL-ICICLE-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,17 @@
                     startup_flag = True # set the flag to true so the thread runs only once
                     continue
 
     def connect(self):
         """
         connect to the local server
         """
-        #self.connection_initialization() # connect to the server
-        self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
+        self.connection_initialization() # connect to the server
+        if __name__ == "__main__":
+            self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
         connection_info: schemas.StartupData = self.schema_unpack() # receive info from the server whether it is a first time connection
         if connection_info.initial: # if the server is receiving its first connection for the session\
             while True:
                 try:
                     url = str(input("\nEnter the link for the tapis service you are connecting to: ")).strip()
                 except KeyboardInterrupt:
                     url = " "
```

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.26/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.25
+Version: 0.0.26
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.25/pyproject.toml` & `TapisCL-ICICLE-0.0.26/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.25"
+version = "0.0.26"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

