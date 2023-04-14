# Comparing `tmp/boa_fm-0.0.8.tar.gz` & `tmp/boa_fm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boa_fm-0.0.8.tar", last modified: Mon Mar 27 12:15:52 2023, max compression
+gzip compressed data, was "boa_fm-0.0.9.tar", last modified: Mon Mar 27 18:13:40 2023, max compression
```

## Comparing `boa_fm-0.0.8.tar` & `boa_fm-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.396403 boa_fm-0.0.8/
--rw-r--r--   0 dmkamath   (501) staff       (20)      527 2023-03-27 12:15:52.395918 boa_fm-0.0.8/PKG-INFO
--rw-r--r--   0 dmkamath   (501) staff       (20)      772 2023-03-27 12:15:45.000000 boa_fm-0.0.8/pyproject.toml
--rw-r--r--   0 dmkamath   (501) staff       (20)       38 2023-03-27 12:15:52.396532 boa_fm-0.0.8/setup.cfg
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.386954 boa_fm-0.0.8/src/
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.389883 boa_fm-0.0.8/src/boa_fm.egg-info/
--rw-r--r--   0 dmkamath   (501) staff       (20)      527 2023-03-27 12:15:52.000000 boa_fm-0.0.8/src/boa_fm.egg-info/PKG-INFO
--rw-r--r--   0 dmkamath   (501) staff       (20)      328 2023-03-27 12:15:52.000000 boa_fm-0.0.8/src/boa_fm.egg-info/SOURCES.txt
--rw-r--r--   0 dmkamath   (501) staff       (20)        1 2023-03-27 12:15:52.000000 boa_fm-0.0.8/src/boa_fm.egg-info/dependency_links.txt
--rw-r--r--   0 dmkamath   (501) staff       (20)       28 2023-03-27 12:15:52.000000 boa_fm-0.0.8/src/boa_fm.egg-info/top_level.txt
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.386429 boa_fm-0.0.8/src/external/
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.386550 boa_fm-0.0.8/src/external/shared/
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.392833 boa_fm-0.0.8/src/external/shared/fixtures/
--rw-r--r--   0 dmkamath   (501) staff       (20)      904 2022-10-14 15:57:06.000000 boa_fm-0.0.8/src/external/shared/fixtures/env_helper.py
--rw-r--r--   0 dmkamath   (501) staff       (20)     4683 2023-03-16 04:39:37.000000 boa_fm-0.0.8/src/external/shared/fixtures/sys_path_helper.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.393985 boa_fm-0.0.8/src/message_mgr/
--rw-r--r--   0 dmkamath   (501) staff       (20)      121 2023-03-24 20:53:42.000000 boa_fm-0.0.8/src/message_mgr/message.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.394958 boa_fm-0.0.8/src/plugin/
--rw-r--r--   0 dmkamath   (501) staff       (20)     3428 2023-03-27 12:14:29.000000 boa_fm-0.0.8/src/plugin/plugin_manager.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 12:15:52.395446 boa_fm-0.0.8/tests/
--rw-r--r--   0 dmkamath   (501) staff       (20)     2006 2023-03-27 12:14:56.000000 boa_fm-0.0.8/tests/test_plugin_framework.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.469893 boa_fm-0.0.9/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      527 2023-03-27 18:13:40.469235 boa_fm-0.0.9/PKG-INFO
+-rw-r--r--   0 dmkamath   (501) staff       (20)      772 2023-03-27 18:13:27.000000 boa_fm-0.0.9/pyproject.toml
+-rw-r--r--   0 dmkamath   (501) staff       (20)       38 2023-03-27 18:13:40.470248 boa_fm-0.0.9/setup.cfg
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.455537 boa_fm-0.0.9/src/
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.459722 boa_fm-0.0.9/src/boa_fm.egg-info/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      527 2023-03-27 18:13:40.000000 boa_fm-0.0.9/src/boa_fm.egg-info/PKG-INFO
+-rw-r--r--   0 dmkamath   (501) staff       (20)      328 2023-03-27 18:13:40.000000 boa_fm-0.0.9/src/boa_fm.egg-info/SOURCES.txt
+-rw-r--r--   0 dmkamath   (501) staff       (20)        1 2023-03-27 18:13:40.000000 boa_fm-0.0.9/src/boa_fm.egg-info/dependency_links.txt
+-rw-r--r--   0 dmkamath   (501) staff       (20)       28 2023-03-27 18:13:40.000000 boa_fm-0.0.9/src/boa_fm.egg-info/top_level.txt
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.454385 boa_fm-0.0.9/src/external/
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.454800 boa_fm-0.0.9/src/external/shared/
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.463780 boa_fm-0.0.9/src/external/shared/fixtures/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      904 2022-10-14 15:57:06.000000 boa_fm-0.0.9/src/external/shared/fixtures/env_helper.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)     4683 2023-03-16 04:39:37.000000 boa_fm-0.0.9/src/external/shared/fixtures/sys_path_helper.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.465310 boa_fm-0.0.9/src/message_mgr/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      121 2023-03-24 20:53:42.000000 boa_fm-0.0.9/src/message_mgr/message.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.466634 boa_fm-0.0.9/src/plugin/
+-rw-r--r--   0 dmkamath   (501) staff       (20)     3428 2023-03-27 12:14:29.000000 boa_fm-0.0.9/src/plugin/plugin_manager.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-27 18:13:40.467755 boa_fm-0.0.9/tests/
+-rw-r--r--   0 dmkamath   (501) staff       (20)     2006 2023-03-27 12:14:56.000000 boa_fm-0.0.9/tests/test_plugin_framework.py
```

### Comparing `boa_fm-0.0.8/PKG-INFO` & `boa_fm-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boa_fm
-Version: 0.0.8
+Version: 0.0.9
 Summary: framework for making monads. this provides the brains for the application
 Author-email: Dinesh Kamath <dmkamath@gmail.com>
 Project-URL: Homepage, https://github.com/dmkamath/quick_bytes
 Project-URL: Bug Tracker, https://github.com/dmkamath/quick_bytes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `boa_fm-0.0.8/pyproject.toml` & `boa_fm-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # build-backend = "hatchling.build"
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "boa_fm"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dinesh Kamath", email="dmkamath@gmail.com" },
 ]
 description = "framework for making monads. this provides the brains for the application"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `boa_fm-0.0.8/src/boa_fm.egg-info/PKG-INFO` & `boa_fm-0.0.9/src/boa_fm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boa-fm
-Version: 0.0.8
+Version: 0.0.9
 Summary: framework for making monads. this provides the brains for the application
 Author-email: Dinesh Kamath <dmkamath@gmail.com>
 Project-URL: Homepage, https://github.com/dmkamath/quick_bytes
 Project-URL: Bug Tracker, https://github.com/dmkamath/quick_bytes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `boa_fm-0.0.8/src/external/shared/fixtures/env_helper.py` & `boa_fm-0.0.9/src/external/shared/fixtures/env_helper.py`

 * *Files identical despite different names*

### Comparing `boa_fm-0.0.8/src/external/shared/fixtures/sys_path_helper.py` & `boa_fm-0.0.9/src/external/shared/fixtures/sys_path_helper.py`

 * *Files identical despite different names*

### Comparing `boa_fm-0.0.8/src/plugin/plugin_manager.py` & `boa_fm-0.0.9/src/plugin/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `boa_fm-0.0.8/tests/test_plugin_framework.py` & `boa_fm-0.0.9/tests/test_plugin_framework.py`

 * *Files identical despite different names*

