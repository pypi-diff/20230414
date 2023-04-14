# Comparing `tmp/pylife-odbserver-2.0.3rc2.tar.gz` & `tmp/pylife-odbserver-2.0.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylife-odbserver-2.0.3rc2.tar", last modified: Thu Apr 13 11:11:22 2023, max compression
+gzip compressed data, was "pylife-odbserver-2.0.3rc3.tar", last modified: Fri Apr 14 08:12:05 2023, max compression
```

## Comparing `pylife-odbserver-2.0.3rc2.tar` & `pylife-odbserver-2.0.3rc3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/odbserver/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/odbserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/odbserver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/odbserver/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 11:11:22.000000 pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 11:11:22.000000 pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:11:22.000000 pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:11:22.000000 pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:22.576418 pylife-odbserver-2.0.3rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 11:11:18.000000 pylife-odbserver-2.0.3rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/odbserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/odbserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/odbserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/odbserver/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-14 08:12:05.000000 pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 08:12:05.000000 pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:12:05.000000 pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 08:12:05.000000 pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:05.858468 pylife-odbserver-2.0.3rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 08:12:00.000000 pylife-odbserver-2.0.3rc3/tests/conftest.py
```

### Comparing `pylife-odbserver-2.0.3rc2/.coveragerc` & `pylife-odbserver-2.0.3rc3/.coveragerc`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/LICENSE` & `pylife-odbserver-2.0.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/PKG-INFO` & `pylife-odbserver-2.0.3rc3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbserver
-Version: 2.0.3rc2
+Version: 2.0.3rc3
 Summary: A server for odbAccess to be acessed by pylife-odbclient
 Home-page: http://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Classifier: Programming Language :: Python
 Requires-Python: <3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc2 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc3 Summary: A
 server for odbAccess to be acessed by pylife-odbclient Home-page: http://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Classifier: Programming
 Language :: Python Requires-Python: <3 Description-Content-Type: text/markdown;
 charset=UTF-8 License-File: LICENSE License-File: AUTHORS.rst # pylife-
 odbserver A server for odbAccess to be accessed by pylife-odbclient ## Purpose
 Unfortunately Abaqus still comes with a python-2.x engine. So you can't access
```

### Comparing `pylife-odbserver-2.0.3rc2/README.md` & `pylife-odbserver-2.0.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/odbserver/__main__.py` & `pylife-odbserver-2.0.3rc3/odbserver/__main__.py`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/odbserver/interface.py` & `pylife-odbserver-2.0.3rc3/odbserver/interface.py`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/pylife_odbserver.egg-info/PKG-INFO` & `pylife-odbserver-2.0.3rc3/pylife_odbserver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbserver
-Version: 2.0.3rc2
+Version: 2.0.3rc3
 Summary: A server for odbAccess to be acessed by pylife-odbclient
 Home-page: http://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Classifier: Programming Language :: Python
 Requires-Python: <3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc2 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc3 Summary: A
 server for odbAccess to be acessed by pylife-odbclient Home-page: http://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Classifier: Programming
 Language :: Python Requires-Python: <3 Description-Content-Type: text/markdown;
 charset=UTF-8 License-File: LICENSE License-File: AUTHORS.rst # pylife-
 odbserver A server for odbAccess to be accessed by pylife-odbclient ## Purpose
 Unfortunately Abaqus still comes with a python-2.x engine. So you can't access
```

### Comparing `pylife-odbserver-2.0.3rc2/setup.cfg` & `pylife-odbserver-2.0.3rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.3rc2/setup.py` & `pylife-odbserver-2.0.3rc3/setup.py`

 * *Files identical despite different names*

