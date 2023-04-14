# Comparing `tmp/HCP-Packer-0.0.7.tar.gz` & `tmp/HCP-Packer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HCP-Packer-0.0.7.tar", last modified: Mon Mar 27 19:36:57 2023, max compression
+gzip compressed data, was "HCP-Packer-0.0.8.tar", last modified: Mon Mar 27 20:28:20 2023, max compression
```

## Comparing `HCP-Packer-0.0.7.tar` & `HCP-Packer-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:36:57.834860 HCP-Packer-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-27 19:36:41.000000 HCP-Packer-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-27 19:36:57.834860 HCP-Packer-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 19:36:41.000000 HCP-Packer-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-27 19:36:57.834860 HCP-Packer-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-27 19:36:41.000000 HCP-Packer-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:36:57.830860 HCP-Packer-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:36:57.834860 HCP-Packer-0.0.7/src/HCP_Packer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-27 19:36:57.000000 HCP-Packer-0.0.7/src/HCP_Packer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-27 19:36:57.000000 HCP-Packer-0.0.7/src/HCP_Packer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:36:57.000000 HCP-Packer-0.0.7/src/HCP_Packer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 19:36:57.000000 HCP-Packer-0.0.7/src/HCP_Packer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:36:57.834860 HCP-Packer-0.0.7/src/hcp_packer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 19:36:41.000000 HCP-Packer-0.0.7/src/hcp_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-03-27 19:36:41.000000 HCP-Packer-0.0.7/src/hcp_packer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-27 20:28:09.000000 HCP-Packer-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-27 20:28:09.000000 HCP-Packer-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-27 20:28:09.000000 HCP-Packer-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/src/HCP_Packer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-27 20:28:20.000000 HCP-Packer-0.0.8/src/HCP_Packer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-27 20:28:20.000000 HCP-Packer-0.0.8/src/HCP_Packer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:28:20.000000 HCP-Packer-0.0.8/src/HCP_Packer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 20:28:20.000000 HCP-Packer-0.0.8/src/HCP_Packer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:28:20.337670 HCP-Packer-0.0.8/src/hcp_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 20:28:09.000000 HCP-Packer-0.0.8/src/hcp_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-03-27 20:28:09.000000 HCP-Packer-0.0.8/src/hcp_packer/client.py
```

### Comparing `HCP-Packer-0.0.7/LICENSE` & `HCP-Packer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `HCP-Packer-0.0.7/PKG-INFO` & `HCP-Packer-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,9 @@
-Metadata-Version: 2.1
-Name: HCP-Packer
-Version: 0.0.7
-Summary: HCP Packer API Client
-Home-page: https://github.com/KBA-IT/hcp-packer
-Author: Billy Austin
-Author-email: billy@kba-it.com
-License: MIT
-Keywords: Hashicorp Packer
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![Workflow Status](https://github.com/KBA-IT/hcp-packer/actions/workflows/build_and_deploy.yml/badge.svg?branch=develop)
+[![PyPI version](https://badge.fury.io/py/HCP-Packer.svg)](https://badge.fury.io/py/HCP-Packer)
 
 # HCP-Packer API Client
 
 Implements a Python client for the HCP Packer API.
 
 
 The full API spec can be found [here](https://developer.hashicorp.com/hcp/api-docs/packer)
```

### Comparing `HCP-Packer-0.0.7/setup.py` & `HCP-Packer-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 long_description = (this_folder / "README.md").read_text()
 
 setup(
     name='HCP-Packer',
     description='HCP Packer API Client',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
-    author="Billy Austin",
-    author_email="billy@kba-it.com",
+    author="KBA IT",
+    author_email="info@kba-it.com",
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    url="https://github.com/KBA-IT/hcp-packer",
+    url='https://kba-it.com',
+    project_urls={
+        'Source': 'https://github.com/KBA-IT/hcp-packer',
+    },
     keywords="Hashicorp Packer",
     install_requires=[],
 )
```

### Comparing `HCP-Packer-0.0.7/src/hcp_packer/client.py` & `HCP-Packer-0.0.8/src/hcp_packer/client.py`

 * *Files identical despite different names*

