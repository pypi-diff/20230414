# Comparing `tmp/hugegraph-python-1.0.0.3.tar.gz` & `tmp/hugegraph-python-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.3.tar", last modified: Fri Apr 14 07:54:58 2023, max compression
+gzip compressed data, was "dist/hugegraph-python-1.0.0.4.tar", last modified: Fri Apr 14 07:59:24 2023, max compression
```

## Comparing `hugegraph-python-1.0.0.3.tar` & `hugegraph-python-1.0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:54:58.940344 hugegraph-python-1.0.0.3/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.3/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1242 2023-04-14 07:54:58.939983 hugegraph-python-1.0.0.3/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      758 2023-04-14 06:18:00.000000 hugegraph-python-1.0.0.3/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:54:58.938644 hugegraph-python-1.0.0.3/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1242 2023-04-14 07:54:58.000000 hugegraph-python-1.0.0.3/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      199 2023-04-14 07:54:58.000000 hugegraph-python-1.0.0.3/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:54:58.000000 hugegraph-python-1.0.0.3/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:54:58.000000 hugegraph-python-1.0.0.3/hugegraph_python.egg-info/top_level.txt
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-04-14 07:54:58.940545 hugegraph-python-1.0.0.3/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-04-14 07:54:46.000000 hugegraph-python-1.0.0.3/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:54:58.939048 hugegraph-python-1.0.0.3/test/
--rw-r--r--   0 zsm        (501) staff       (20)      613 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.3/test/test.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.380616 hugegraph-python-1.0.0.4/
+-rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.4/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     1210 2023-04-14 07:59:24.380208 hugegraph-python-1.0.0.4/PKG-INFO
+-rw-rw-r--   0 zsm        (501) staff       (20)      726 2023-04-14 07:56:21.000000 hugegraph-python-1.0.0.4/README.md
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.378862 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     1210 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      199 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/top_level.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2023-04-14 07:59:24.380715 hugegraph-python-1.0.0.4/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-04-14 07:59:05.000000 hugegraph-python-1.0.0.4/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.379256 hugegraph-python-1.0.0.4/test/
+-rw-r--r--   0 zsm        (501) staff       (20)      613 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.4/test/test.py
```

### Comparing `hugegraph-python-1.0.0.3/LICENSE` & `hugegraph-python-1.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.3/PKG-INFO` & `hugegraph-python-1.0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,25 @@
 License-File: LICENSE
 
 # hugegraph-python
 A Python SDK for Apache HugeGraph, maintained by [cvte research data-mining team](https://github.com/cvte-research-datamining/hugegraph-python).
 
 This project currently in alpha testing, will open source the code soon.
 
-#Installation
-##PyPi
+# Installation
+## PyPi
+https://pypi.org/project/hugegraph-python/
+```shell
+pip3 install hugegraph-python
 ```
-pip3 install gremlinapi
 
-```
-##Install from source
-```
-git clone git@github.com:gremlin/gremlin-python.git
-cd gremlin-python
-python3 setup.py install
-```
+## Install from source
+release soon
 
-#Examples
+# Examples
 ```python
 from hugegraph import PyHugeGraph
 # init client
 client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
```

### Comparing `hugegraph-python-1.0.0.3/README.md` & `hugegraph-python-1.0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # hugegraph-python
 A Python SDK for Apache HugeGraph, maintained by [cvte research data-mining team](https://github.com/cvte-research-datamining/hugegraph-python).
 
 This project currently in alpha testing, will open source the code soon.
 
-#Installation
-##PyPi
+# Installation
+## PyPi
+https://pypi.org/project/hugegraph-python/
+```shell
+pip3 install hugegraph-python
 ```
-pip3 install gremlinapi
 
-```
-##Install from source
-```
-git clone git@github.com:gremlin/gremlin-python.git
-cd gremlin-python
-python3 setup.py install
-```
+## Install from source
+release soon
 
-#Examples
+# Examples
 ```python
 from hugegraph import PyHugeGraph
 # init client
 client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
```

### Comparing `hugegraph-python-1.0.0.3/hugegraph_python.egg-info/PKG-INFO` & `hugegraph-python-1.0.0.4/hugegraph_python.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,25 @@
 License-File: LICENSE
 
 # hugegraph-python
 A Python SDK for Apache HugeGraph, maintained by [cvte research data-mining team](https://github.com/cvte-research-datamining/hugegraph-python).
 
 This project currently in alpha testing, will open source the code soon.
 
-#Installation
-##PyPi
+# Installation
+## PyPi
+https://pypi.org/project/hugegraph-python/
+```shell
+pip3 install hugegraph-python
 ```
-pip3 install gremlinapi
 
-```
-##Install from source
-```
-git clone git@github.com:gremlin/gremlin-python.git
-cd gremlin-python
-python3 setup.py install
-```
+## Install from source
+release soon
 
-#Examples
+# Examples
 ```python
 from hugegraph import PyHugeGraph
 # init client
 client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
```

### Comparing `hugegraph-python-1.0.0.3/setup.py` & `hugegraph-python-1.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hugegraph-python",
-    version="1.0.0.3",
+    version="1.0.0.4",
     author="cvte-research-datamining",
     author_email="ming@apache.org",
     description="A Python SDK for Apache HugeGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cvte-research-datamining/hugegraph-python",
     packages=setuptools.find_packages(),
```

### Comparing `hugegraph-python-1.0.0.3/test/test.py` & `hugegraph-python-1.0.0.4/test/test.py`

 * *Files identical despite different names*

