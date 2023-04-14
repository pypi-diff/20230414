# Comparing `tmp/pylife-odbclient-2.0.3rc2.tar.gz` & `tmp/pylife-odbclient-2.0.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylife-odbclient-2.0.3rc2.tar", last modified: Thu Apr 13 11:11:21 2023, max compression
+gzip compressed data, was "pylife-odbclient-2.0.3rc3.tar", last modified: Fri Apr 14 08:12:11 2023, max compression
```

## Comparing `pylife-odbclient-2.0.3rc2.tar` & `pylife-odbclient-2.0.3rc3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/odbclient/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/src/odbclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/src/odbclient/odbclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   238316 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/beam_3d_hex_quad.odb
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/connectivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/node_coordinates.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/stress_element_nodal.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/stress_integration_point.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/test_odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:11.478937 pylife-odbclient-2.0.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-14 08:12:11.478937 pylife-odbclient-2.0.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-14 08:12:11.478937 pylife-odbclient-2.0.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:11.470937 pylife-odbclient-2.0.3rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:11.474937 pylife-odbclient-2.0.3rc3/src/odbclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/src/odbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/src/odbclient/odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:11.474937 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 08:12:11.000000 pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:12:11.478937 pylife-odbclient-2.0.3rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   238316 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/beam_3d_hex_quad.odb
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/connectivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/node_coordinates.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/stress_element_nodal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/stress_integration_point.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-14 08:11:59.000000 pylife-odbclient-2.0.3rc3/tests/test_odbclient.py
```

### Comparing `pylife-odbclient-2.0.3rc2/.coveragerc` & `pylife-odbclient-2.0.3rc3/.coveragerc`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/.gitignore` & `pylife-odbclient-2.0.3rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/LICENSE` & `pylife-odbclient-2.0.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/PKG-INFO` & `pylife-odbclient-2.0.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.3rc2
+Version: 2.0.3rc3
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc2 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc3 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
```

### Comparing `pylife-odbclient-2.0.3rc2/README.md` & `pylife-odbclient-2.0.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/demo.ipynb` & `pylife-odbclient-2.0.3rc3/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/setup.cfg` & `pylife-odbclient-2.0.3rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/setup.py` & `pylife-odbclient-2.0.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/src/odbclient/__init__.py` & `pylife-odbclient-2.0.3rc3/src/odbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/src/odbclient/odbclient.py` & `pylife-odbclient-2.0.3rc3/src/odbclient/odbclient.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/PKG-INFO` & `pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.3rc2
+Version: 2.0.3rc3
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc2 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc3 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
```

### Comparing `pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/SOURCES.txt` & `pylife-odbclient-2.0.3rc3/src/pylife_odbclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/tests/beam_3d_hex_quad.odb` & `pylife-odbclient-2.0.3rc3/tests/beam_3d_hex_quad.odb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/tests/node_coordinates.csv` & `pylife-odbclient-2.0.3rc3/tests/node_coordinates.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/tests/stress_element_nodal.csv` & `pylife-odbclient-2.0.3rc3/tests/stress_element_nodal.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/tests/stress_integration_point.csv` & `pylife-odbclient-2.0.3rc3/tests/stress_integration_point.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc2/tests/test_odbclient.py` & `pylife-odbclient-2.0.3rc3/tests/test_odbclient.py`

 * *Files identical despite different names*

