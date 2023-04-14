# Comparing `tmp/oai_tools-0.1.0.tar.gz` & `tmp/oai_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oai_tools-0.1.0.tar", last modified: Fri Apr 14 15:30:51 2023, max compression
+gzip compressed data, was "oai_tools-0.1.1.tar", last modified: Fri Apr 14 18:05:42 2023, max compression
```

## Comparing `oai_tools-0.1.0.tar` & `oai_tools-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 filip     (1000) filip     (1000)        0 2023-04-14 15:30:51.626100 oai_tools-0.1.0/
--rw-r--r--   0 filip     (1000) filip     (1000)     1898 2023-04-14 15:30:51.626100 oai_tools-0.1.0/PKG-INFO
--rw-r--r--   0 filip     (1000) filip     (1000)      925 2023-04-14 09:36:14.000000 oai_tools-0.1.0/README.md
-drwxr-xr-x   0 filip     (1000) filip     (1000)        0 2023-04-14 15:30:51.626100 oai_tools-0.1.0/oai_tools/
--rw-r--r--   0 filip     (1000) filip     (1000)      766 2023-04-14 09:36:14.000000 oai_tools-0.1.0/oai_tools/__init__.py
--rw-r--r--   0 filip     (1000) filip     (1000)     5889 2023-04-14 12:35:01.000000 oai_tools-0.1.0/oai_tools/cligpt.py
-drwxr-xr-x   0 filip     (1000) filip     (1000)        0 2023-04-14 15:30:51.626100 oai_tools-0.1.0/oai_tools.egg-info/
--rw-r--r--   0 filip     (1000) filip     (1000)     1898 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/PKG-INFO
--rw-r--r--   0 filip     (1000) filip     (1000)      275 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 filip     (1000) filip     (1000)        1 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 filip     (1000) filip     (1000)       50 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/entry_points.txt
--rw-r--r--   0 filip     (1000) filip     (1000)       35 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/requires.txt
--rw-r--r--   0 filip     (1000) filip     (1000)       10 2023-04-14 15:30:51.000000 oai_tools-0.1.0/oai_tools.egg-info/top_level.txt
--rw-r--r--   0 filip     (1000) filip     (1000)      530 2023-04-14 08:14:04.000000 oai_tools-0.1.0/pyproject.toml
--rw-r--r--   0 filip     (1000) filip     (1000)       38 2023-04-14 15:30:51.626100 oai_tools-0.1.0/setup.cfg
--rw-r--r--   0 filip     (1000) filip     (1000)     1172 2023-04-14 15:22:39.000000 oai_tools-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.607755 oai_tools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-14 18:05:33.000000 oai_tools-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-14 18:05:42.603754 oai_tools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-14 18:05:33.000000 oai_tools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.603754 oai_tools-0.1.1/oai_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 18:05:33.000000 oai_tools-0.1.1/oai_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-14 18:05:33.000000 oai_tools-0.1.1/oai_tools/cligpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.603754 oai_tools-0.1.1/oai_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-14 18:05:33.000000 oai_tools-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:05:42.607755 oai_tools-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-14 18:05:33.000000 oai_tools-0.1.1/setup.py
```

### Comparing `oai_tools-0.1.0/PKG-INFO` & `oai_tools-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oai_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
@@ -20,20 +20,14 @@
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
         
         ### API Key
         OpenAI's API key is required. 
         The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
         
-        ## Development
-        ### Pre-commit hooks
-        pip install pre-commit pylint mypy black isort
-        pre-commit install
-        pre-commit run --all-files
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oai_tools-0.1.0/README.md` & `oai_tools-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,13 +11,7 @@
 
 ## Configuration
 Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
 
 ### API Key
 OpenAI's API key is required. 
 The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
-
-## Development
-### Pre-commit hooks
-pip install pre-commit pylint mypy black isort
-pre-commit install
-pre-commit run --all-files
```

### Comparing `oai_tools-0.1.0/oai_tools/__init__.py` & `oai_tools-0.1.1/oai_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.0/oai_tools/cligpt.py` & `oai_tools-0.1.1/oai_tools/cligpt.py`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.0/oai_tools.egg-info/PKG-INFO` & `oai_tools-0.1.1/oai_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oai-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
@@ -20,20 +20,14 @@
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
         
         ### API Key
         OpenAI's API key is required. 
         The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
         
-        ## Development
-        ### Pre-commit hooks
-        pip install pre-commit pylint mypy black isort
-        pre-commit install
-        pre-commit run --all-files
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oai_tools-0.1.0/pyproject.toml` & `oai_tools-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.0/setup.py` & `oai_tools-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="oai_tools",
-    version="0.1.0",
+    version="0.1.1",
     author="Filip Granö",
     author_email="filip-accounts@grano.me",
     description="Collection of useful tools built on top of OpenAI's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipgrano/oai_tools/tree/main",
     packages=find_packages(),
```

