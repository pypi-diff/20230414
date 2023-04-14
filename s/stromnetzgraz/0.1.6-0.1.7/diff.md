# Comparing `tmp/stromnetzgraz-0.1.6.tar.gz` & `tmp/stromnetzgraz-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stromnetzgraz-0.1.6.tar", last modified: Tue Apr 11 18:43:25 2023, max compression
+gzip compressed data, was "stromnetzgraz-0.1.7.tar", last modified: Fri Apr 14 16:09:33 2023, max compression
```

## Comparing `stromnetzgraz-0.1.6.tar` & `stromnetzgraz-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:25.715670 stromnetzgraz-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-11 18:43:25.715670 stromnetzgraz-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 18:43:25.715670 stromnetzgraz-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:25.711670 stromnetzgraz-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:25.715670 stromnetzgraz-0.1.6/src/sngraz/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/src/sngraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/src/sngraz/certchain.crt
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-11 18:43:14.000000 stromnetzgraz-0.1.6/src/sngraz/sngraz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:43:25.715670 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-11 18:43:25.000000 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 18:43:25.000000 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:43:25.000000 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 18:43:25.000000 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 18:43:25.000000 stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:09:33.954211 stromnetzgraz-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-14 16:09:33.954211 stromnetzgraz-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 16:09:33.954211 stromnetzgraz-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:09:33.950211 stromnetzgraz-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:09:33.954211 stromnetzgraz-0.1.7/src/sngraz/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/src/sngraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/src/sngraz/certchain.crt
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-14 16:09:20.000000 stromnetzgraz-0.1.7/src/sngraz/sngraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:09:33.954211 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-14 16:09:33.000000 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 16:09:33.000000 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:09:33.000000 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 16:09:33.000000 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 16:09:33.000000 stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/top_level.txt
```

### Comparing `stromnetzgraz-0.1.6/LICENSE` & `stromnetzgraz-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stromnetzgraz-0.1.6/PKG-INFO` & `stromnetzgraz-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stromnetzgraz
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client library for Stromnetz Graz API
 Home-page: https://github.com/dreautall/stromnetzgraz
 Author: dreautall
 Author-email: michael@online-net.eu
 Project-URL: Documentation, https://github.com/dreautall/stromnetzgraz
 Project-URL: Bug Reports, https://github.com/dreautall/stromnetzgraz/issues
 Project-URL: Source Code, https://github.com/dreautall/stromnetzgraz
```

### Comparing `stromnetzgraz-0.1.6/README.md` & `stromnetzgraz-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `stromnetzgraz-0.1.6/setup.py` & `stromnetzgraz-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
-    install_requires=["pyjwt"],
+    install_requires=["pyjwt", "aiohttp"],
     extras_require={
         "dev": ["check-manifest"],
         # 'test': ['coverage'],
     },
 )
```

### Comparing `stromnetzgraz-0.1.6/src/sngraz/certchain.crt` & `stromnetzgraz-0.1.7/src/sngraz/certchain.crt`

 * *Files identical despite different names*

### Comparing `stromnetzgraz-0.1.6/src/sngraz/sngraz.py` & `stromnetzgraz-0.1.7/src/sngraz/sngraz.py`

 * *Files identical despite different names*

### Comparing `stromnetzgraz-0.1.6/src/stromnetzgraz.egg-info/PKG-INFO` & `stromnetzgraz-0.1.7/src/stromnetzgraz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stromnetzgraz
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client library for Stromnetz Graz API
 Home-page: https://github.com/dreautall/stromnetzgraz
 Author: dreautall
 Author-email: michael@online-net.eu
 Project-URL: Documentation, https://github.com/dreautall/stromnetzgraz
 Project-URL: Bug Reports, https://github.com/dreautall/stromnetzgraz/issues
 Project-URL: Source Code, https://github.com/dreautall/stromnetzgraz
```

