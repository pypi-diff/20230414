# Comparing `tmp/curl_arguments_url-0.1.0a1.tar.gz` & `tmp/curl_arguments_url-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_arguments_url-0.1.0a1.tar", last modified: Fri Apr 14 16:41:34 2023, max compression
+gzip compressed data, was "curl_arguments_url-0.1.1.tar", last modified: Fri Apr 14 16:47:07 2023, max compression
```

## Comparing `curl_arguments_url-0.1.0a1.tar` & `curl_arguments_url-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:41:34.823196 curl_arguments_url-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-14 16:41:34.823196 curl_arguments_url-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:41:34.823196 curl_arguments_url-0.1.0a1/curl_arguments_url/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/curl_arguments_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/curl_arguments_url/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/curl_arguments_url/click_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    55084 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/curl_arguments_url/curl_arguments_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:41:34.823196 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:41:34.000000 curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 16:41:34.823196 curl_arguments_url-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 16:41:28.000000 curl_arguments_url-0.1.0a1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.088325 curl_arguments_url-0.1.1/curl_arguments_url/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/click_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55084 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/curl_arguments_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/version.txt
```

### Comparing `curl_arguments_url-0.1.0a1/LICENSE` & `curl_arguments_url-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.0a1/PKG-INFO` & `curl_arguments_url-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_arguments_url
-Version: 0.1.0a1
+Version: 0.1.1
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `curl_arguments_url-0.1.0a1/README.md` & `curl_arguments_url-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.0a1/curl_arguments_url/cli.py` & `curl_arguments_url-0.1.1/curl_arguments_url/cli.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.0a1/curl_arguments_url/click_test.py` & `curl_arguments_url-0.1.1/curl_arguments_url/click_test.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.0a1/curl_arguments_url/curl_arguments_url.py` & `curl_arguments_url-0.1.1/curl_arguments_url/curl_arguments_url.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.0a1/curl_arguments_url.egg-info/PKG-INFO` & `curl_arguments_url-0.1.1/curl_arguments_url.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl-arguments-url
-Version: 0.1.0a1
+Version: 0.1.1
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `curl_arguments_url-0.1.0a1/setup.py` & `curl_arguments_url-0.1.1/setup.py`

 * *Files identical despite different names*

