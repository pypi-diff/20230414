# Comparing `tmp/im-data-manager-job-decoder-1.8.1.tar.gz` & `tmp/im-data-manager-job-decoder-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-data-manager-job-decoder-1.8.1.tar", last modified: Tue May  3 13:56:06 2022, max compression
+gzip compressed data, was "im-data-manager-job-decoder-1.9.0.tar", last modified: Tue May  3 17:57:09 2022, max compression
```

## Comparing `im-data-manager-job-decoder-1.8.1.tar` & `im-data-manager-job-decoder-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:56:06.359986 im-data-manager-job-decoder-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 13:56:06.359986 im-data-manager-job-decoder-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:56:06.359986 im-data-manager-job-decoder-1.8.1/decoder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/decoder/decode_jinja2_3_0.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/decoder/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     9070 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/decoder/job-definition-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/decoder/manifest-schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 13:56:06.359986 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 13:56:05.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-03 13:56:06.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 13:56:05.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 13:56:04.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-03 13:56:06.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-03 13:56:06.000000 im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-03 13:56:06.359986 im-data-manager-job-decoder-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-03 13:55:50.000000 im-data-manager-job-decoder-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.916736 im-data-manager-job-decoder-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/decoder/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/decode_jinja2_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/job-definition-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/manifest-schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 17:57:07.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-03 17:57:09.916736 im-data-manager-job-decoder-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/setup.py
```

### Comparing `im-data-manager-job-decoder-1.8.1/LICENSE` & `im-data-manager-job-decoder-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.8.1/PKG-INFO` & `im-data-manager-job-decoder-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-data-manager-job-decoder
-Version: 1.8.1
+Version: 1.9.0
 Summary: Job decoding logic
 Home-page: https://github.com/informaticsmatters/data-manager-job-decoder
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: jinja2 decoder
 Platform: any
```

### Comparing `im-data-manager-job-decoder-1.8.1/README.rst` & `im-data-manager-job-decoder-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.8.1/decoder/decode_jinja2_3_0.py` & `im-data-manager-job-decoder-1.9.0/decoder/decode_jinja2_3_0.py`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.8.1/decoder/decoder.py` & `im-data-manager-job-decoder-1.9.0/decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.8.1/decoder/job-definition-schema.yaml` & `im-data-manager-job-decoder-1.9.0/decoder/job-definition-schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,20 @@
   description:
     type: string
   collection:
     type: string
     minLength: 1
     maxLength: 80
     pattern: '^[a-z]{1}[a-z0-9-]*$'
-  repository-url:
-    type: string
-    maxlength: 2048
-    format: uri
-  repository-tag:
-    type: string
-    minLength: 1
-    maxLength: 24
   jobs:
     $ref: '#/definitions/job-identity'
 required:
 - kind
 - kind-version
 - collection
-- repository-url
-- repository-tag
 - jobs
 
 # Sub-object definitions ------------------------------------------------------
 # Things like the Job structure, Image structure etc.
 
 definitions:
```

### Comparing `im-data-manager-job-decoder-1.8.1/decoder/manifest-schema.yaml` & `im-data-manager-job-decoder-1.9.0/decoder/manifest-schema.yaml`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.8.1/im_data_manager_job_decoder.egg-info/PKG-INFO` & `im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-data-manager-job-decoder
-Version: 1.8.1
+Version: 1.9.0
 Summary: Job decoding logic
 Home-page: https://github.com/informaticsmatters/data-manager-job-decoder
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: jinja2 decoder
 Platform: any
```

### Comparing `im-data-manager-job-decoder-1.8.1/setup.py` & `im-data-manager-job-decoder-1.9.0/setup.py`

 * *Files identical despite different names*

