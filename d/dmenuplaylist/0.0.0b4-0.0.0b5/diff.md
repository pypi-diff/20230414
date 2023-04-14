# Comparing `tmp/dmenuplaylist-0.0.0b4.tar.gz` & `tmp/dmenuplaylist-0.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmenuplaylist-0.0.0b4.tar", last modified: Fri Apr 14 00:31:34 2023, max compression
+gzip compressed data, was "dmenuplaylist-0.0.0b5.tar", last modified: Fri Apr 14 00:39:25 2023, max compression
```

## Comparing `dmenuplaylist-0.0.0b4.tar` & `dmenuplaylist-0.0.0b5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/
--rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 dmenuplaylist-0.0.0b4/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      741 2023-01-25 06:34:34.000000 dmenuplaylist-0.0.0b4/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      549 2023-04-14 00:30:46.000000 dmenuplaylist-0.0.0b4/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/dmenuplaylist/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1351 2023-01-11 06:43:22.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1599 2023-01-11 05:09:52.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      992 2023-01-11 06:15:40.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1615 2023-04-14 00:27:25.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      657 2023-01-11 06:56:33.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4408 2023-01-30 05:36:22.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      516 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       62 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       17 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       14 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:39:25.916164 dmenuplaylist-0.0.0b5/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 dmenuplaylist-0.0.0b5/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:39:25.916164 dmenuplaylist-0.0.0b5/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      741 2023-01-25 06:34:34.000000 dmenuplaylist-0.0.0b5/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      556 2023-04-14 00:38:53.000000 dmenuplaylist-0.0.0b5/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:39:25.916164 dmenuplaylist-0.0.0b5/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:39:25.912831 dmenuplaylist-0.0.0b5/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:39:25.912831 dmenuplaylist-0.0.0b5/src/dmenuplaylist/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1351 2023-01-11 06:43:22.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1599 2023-01-11 05:09:52.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      992 2023-01-11 06:15:40.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1615 2023-04-14 00:27:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      657 2023-01-11 06:56:33.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4408 2023-01-30 05:36:22.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:39:25.916164 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      516 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       62 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       24 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       14 2023-04-14 00:39:25.000000 dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/top_level.txt
```

### Comparing `dmenuplaylist-0.0.0b4/LICENSE` & `dmenuplaylist-0.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/PKG-INFO` & `dmenuplaylist-0.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmenuplaylist
-Version: 0.0.0b4
+Version: 0.0.0b5
 Summary: Simple playlist manager, meant to be used with mpv.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/dmenuplaylist
 Keywords: mpv,dmenu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dmenuplaylist-0.0.0b4/README.md` & `dmenuplaylist-0.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/pyproject.toml` & `dmenuplaylist-0.0.0b5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmenuplaylist"
-version = "0.0.0.b4"
+version = "0.0.0.b5"
 description = "Simple playlist manager, meant to be used with mpv."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv", "dmenu" ]
 dependencies = [
     "loadconf",
-    "promptx"
+    "promptx>=0.0.5"
 ]
 
 [project.optional-dependencies]
 
 [project.scripts]
 dmenuplaylist = "dmenuplaylist.__main__:main"
```

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/__main__.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/__main__.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/config.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/config.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/options.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/options.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/prompts.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/prompts.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/system.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/system.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist/utils.py` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist/utils.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/PKG-INFO` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmenuplaylist
-Version: 0.0.0b4
+Version: 0.0.0b5
 Summary: Simple playlist manager, meant to be used with mpv.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/dmenuplaylist
 Keywords: mpv,dmenu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/SOURCES.txt` & `dmenuplaylist-0.0.0b5/src/dmenuplaylist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

