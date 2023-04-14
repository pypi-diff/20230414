# Comparing `tmp/luau-0.2.0.tar.gz` & `tmp/luau-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.0.tar", last modified: Fri Apr 14 03:20:29 2023, max compression
+gzip compressed data, was "luau-0.2.1.tar", last modified: Fri Apr 14 21:49:34 2023, max compression
```

## Comparing `luau-0.2.0.tar` & `luau-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.765372 luau-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-14 03:20:29.765372 luau-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.0/README.md
--rw-rw-rw-   0        0        0      494 2023-04-14 03:20:09.000000 luau-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 03:20:29.766369 luau-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.728628 luau-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.739314 luau-0.2.0/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.0/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.0/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.0/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.763381 luau-0.2.0/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.0/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.0/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.0/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      839 2023-04-14 02:57:33.000000 luau-0.2.0/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2464 2023-04-14 03:14:17.000000 luau-0.2.0/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.756397 luau-0.2.0/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 21:49:34.008348 luau-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-14 21:49:34.007351 luau-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.1/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-14 21:48:10.000000 luau-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 21:49:34.008348 luau-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.921402 luau-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.952318 luau-0.2.1/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.1/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.1/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.1/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:49:34.005357 luau-0.2.1/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.1/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.1/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.1/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      839 2023-04-14 02:57:33.000000 luau-0.2.1/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2478 2023-04-14 21:47:59.000000 luau-0.2.1/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.980390 luau-0.2.1/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.0/LICENSE` & `luau-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/__init__.py` & `luau-0.2.1/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/convert.py` & `luau-0.2.1/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/path.py` & `luau-0.2.1/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/roblox/__init__.py` & `luau-0.2.1/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/roblox/rojo.py` & `luau-0.2.1/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/roblox/tool.py` & `luau-0.2.1/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/roblox/util.py` & `luau-0.2.1/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.0/src/luau/roblox/wally.py` & `luau-0.2.1/src/luau/roblox/wally.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import toml
 from .tool import get_tool_name
 from .rojo import get_rojo_project_path, get_rojo_name, build_sourcemap
 
 WALLY_SOURCE = "UpliftGames/wally"
 WALLY_VERSION = "0.3.1"
-WPT_SOURCE = "wally-package-types"
+WPT_SOURCE = "JohnnyMorganz/wally-package-types"
 WPT_VERSION = "1.2.0"
 
 def get_wally_name():
 	return get_tool_name(WALLY_SOURCE, WALLY_VERSION)
 
 def get_wally_package_types_name():
 	return get_tool_name(WPT_SOURCE, WPT_VERSION)
```

