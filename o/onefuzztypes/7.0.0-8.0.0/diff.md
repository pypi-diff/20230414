# Comparing `tmp/onefuzztypes-7.0.0.tar.gz` & `tmp/onefuzztypes-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onefuzztypes-7.0.0.tar", last modified: Tue Mar 21 20:47:37 2023, max compression
+gzip compressed data, was "dist/onefuzztypes-8.0.0.tar", last modified: Wed Apr 12 01:45:19 2023, max compression
```

## Comparing `onefuzztypes-7.0.0.tar` & `onefuzztypes-8.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-03-21 20:47:30.000000 onefuzztypes-7.0.0/onefuzztypes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    11453 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     8236 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    25245 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/onefuzztypes/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/onefuzztypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:37.000000 onefuzztypes-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/tests/test_alnum_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/tests/test_container_def.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/tests/test_instance_config_update.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2820 2023-03-21 20:47:29.000000 onefuzztypes-7.0.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/consts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11453 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8236 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25245 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_alnum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_container_def.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_instance_config_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2820 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_models.py
```

### Comparing `onefuzztypes-7.0.0/PKG-INFO` & `onefuzztypes-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 7.0.0
+Version: 8.0.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-7.0.0/README.md` & `onefuzztypes-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/_monkeypatch.py` & `onefuzztypes-8.0.0/onefuzztypes/_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/enums.py` & `onefuzztypes-8.0.0/onefuzztypes/enums.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/events.py` & `onefuzztypes-8.0.0/onefuzztypes/events.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/job_templates.py` & `onefuzztypes-8.0.0/onefuzztypes/job_templates.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/models.py` & `onefuzztypes-8.0.0/onefuzztypes/models.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/primitives.py` & `onefuzztypes-8.0.0/onefuzztypes/primitives.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/requests.py` & `onefuzztypes-8.0.0/onefuzztypes/requests.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/responses.py` & `onefuzztypes-8.0.0/onefuzztypes/responses.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/validators.py` & `onefuzztypes-8.0.0/onefuzztypes/validators.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes/webhooks.py` & `onefuzztypes-8.0.0/onefuzztypes/webhooks.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/onefuzztypes.egg-info/PKG-INFO` & `onefuzztypes-8.0.0/onefuzztypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 7.0.0
+Version: 8.0.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-7.0.0/onefuzztypes.egg-info/SOURCES.txt` & `onefuzztypes-8.0.0/onefuzztypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/setup.py` & `onefuzztypes-8.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/tests/test_alnum_filter.py` & `onefuzztypes-8.0.0/tests/test_alnum_filter.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/tests/test_container_def.py` & `onefuzztypes-8.0.0/tests/test_container_def.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/tests/test_instance_config_update.py` & `onefuzztypes-8.0.0/tests/test_instance_config_update.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-7.0.0/tests/test_models.py` & `onefuzztypes-8.0.0/tests/test_models.py`

 * *Files identical despite different names*

