# Comparing `tmp/py-mlm-0.0.5.tar.gz` & `tmp/py-mlm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-mlm-0.0.5.tar", last modified: Fri Apr 14 00:33:03 2023, max compression
+gzip compressed data, was "py-mlm-0.0.6.tar", last modified: Fri Apr 14 00:46:25 2023, max compression
```

## Comparing `py-mlm-0.0.5.tar` & `py-mlm-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.237342 py-mlm-0.0.5/
--rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.5/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:33:03.237342 py-mlm-0.0.5/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.5/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      558 2023-04-14 00:32:04.000000 py-mlm-0.0.5/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:33:03.237342 py-mlm-0.0.5/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.230675 py-mlm-0.0.5/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.234009 py-mlm-0.0.5/src/mlm/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.5/src/mlm/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2335 2023-04-10 21:07:50.000000 py-mlm-0.0.5/src/mlm/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.5/src/mlm/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2216 2023-03-23 03:17:40.000000 py-mlm-0.0.5/src/mlm/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.5/src/mlm/g_dl.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.5/src/mlm/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3526 2023-03-26 06:19:39.000000 py-mlm-0.0.5/src/mlm/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6582 2023-04-10 20:40:11.000000 py-mlm-0.0.5/src/mlm/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1651 2023-04-14 00:27:42.000000 py-mlm-0.0.5/src/mlm/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.5/src/mlm/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     5963 2023-04-10 21:06:52.000000 py-mlm-0.0.5/src/mlm/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4224 2023-03-26 06:30:48.000000 py-mlm-0.0.5/src/mlm/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.237342 py-mlm-0.0.5/src/py_mlm.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       30 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/
+-rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.6/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:46:25.582291 py-mlm-0.0.6/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.6/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      565 2023-04-14 00:45:35.000000 py-mlm-0.0.6/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:46:25.582291 py-mlm-0.0.6/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.578957 py-mlm-0.0.6/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/src/mlm/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.6/src/mlm/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2335 2023-04-10 21:07:50.000000 py-mlm-0.0.6/src/mlm/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.6/src/mlm/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2216 2023-03-23 03:17:40.000000 py-mlm-0.0.6/src/mlm/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.6/src/mlm/g_dl.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.6/src/mlm/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3526 2023-03-26 06:19:39.000000 py-mlm-0.0.6/src/mlm/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6582 2023-04-10 20:40:11.000000 py-mlm-0.0.6/src/mlm/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1651 2023-04-14 00:27:42.000000 py-mlm-0.0.6/src/mlm/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.6/src/mlm/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5963 2023-04-10 21:06:52.000000 py-mlm-0.0.6/src/mlm/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4224 2023-03-26 06:30:48.000000 py-mlm-0.0.6/src/mlm/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/src/py_mlm.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/top_level.txt
```

### Comparing `py-mlm-0.0.5/LICENSE` & `py-mlm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/pyproject.toml` & `py-mlm-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-mlm"
-version = "0.0.5"
+version = "0.0.6"
 description = "mlm - Manga Library Manager. Local, and simple method for reading and tracking manga."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "zathura" ]
 dependencies = [
     "python-magic",
     "loadconf",
-    "promptx"
+    "promptx>=0.0.5"
 ]
 
 [project.optional-dependencies]
 
 [project.scripts]
 mlm = "mlm.__main__:main"
```

### Comparing `py-mlm-0.0.5/src/mlm/__main__.py` & `py-mlm-0.0.6/src/mlm/__main__.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/build.py` & `py-mlm-0.0.6/src/mlm/build.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/config.py` & `py-mlm-0.0.6/src/mlm/config.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/g_dl.py` & `py-mlm-0.0.6/src/mlm/g_dl.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/media.py` & `py-mlm-0.0.6/src/mlm/media.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/options.py` & `py-mlm-0.0.6/src/mlm/options.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/prompts.py` & `py-mlm-0.0.6/src/mlm/prompts.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/search.py` & `py-mlm-0.0.6/src/mlm/search.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/system.py` & `py-mlm-0.0.6/src/mlm/system.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.5/src/mlm/utils.py` & `py-mlm-0.0.6/src/mlm/utils.py`

 * *Files identical despite different names*

