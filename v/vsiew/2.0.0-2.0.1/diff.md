# Comparing `tmp/vsiew-2.0.0.tar.gz` & `tmp/vsiew-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.0.0.tar", last modified: Mon Apr 10 12:00:52 2023, max compression
+gzip compressed data, was "vsiew-2.0.1.tar", last modified: Fri Apr 14 16:07:31 2023, max compression
```

## Comparing `vsiew-2.0.0.tar` & `vsiew-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 12:00:31.000000 vsiew-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-10 12:00:52.663651 vsiew-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 12:00:31.000000 vsiew-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:00:52.663651 vsiew-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-10 12:00:31.000000 vsiew-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.506685 vsiew-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 16:07:06.000000 vsiew-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-14 16:07:31.506685 vsiew-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 16:07:06.000000 vsiew-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:31.506685 vsiew-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 16:07:06.000000 vsiew-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.502685 vsiew-2.0.1/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.506685 vsiew-2.0.1/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.0.0/LICENSE` & `vsiew-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.0.0/PKG-INFO` & `vsiew-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.0.0
+Version: 2.0.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.0.0/setup.py` & `vsiew-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.0.0/vsiew/init.py` & `vsiew-2.0.1/vsiew/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 
 def update(latest_git: bool = False) -> None:
     import sys
     from subprocess import check_call
     from http.client import HTTPSConnection
 
     def _get_call(package: str, do_git: bool) -> int:
+        args = list[str]()
+
         if do_git:
             package = f'git+https://github.com/{base_org}/{package}.git'
+            args.extend(['--force', '--no-deps'])
 
         try:
-            return check_call([sys.executable, '-m', 'pip', 'install', package, '-U', '--no-cache-dir'])
+            return check_call([sys.executable, '-m', 'pip', 'install', package, '-U', '--no-cache-dir', *args])
         except Exception:
             return 1
 
     if latest_git:
         err = 0
 
         conn = HTTPSConnection('raw.githubusercontent.com', 443)
```

### Comparing `vsiew-2.0.0/vsiew.egg-info/PKG-INFO` & `vsiew-2.0.1/vsiew.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.0.0
+Version: 2.0.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

