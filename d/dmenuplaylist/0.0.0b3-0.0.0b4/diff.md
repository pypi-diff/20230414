# Comparing `tmp/dmenuplaylist-0.0.0b3.tar.gz` & `tmp/dmenuplaylist-0.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmenuplaylist-0.0.0b3.tar", last modified: Mon Jan 23 06:27:46 2023, max compression
+gzip compressed data, was "dmenuplaylist-0.0.0b4.tar", last modified: Fri Apr 14 00:31:34 2023, max compression
```

## Comparing `dmenuplaylist-0.0.0b3.tar` & `dmenuplaylist-0.0.0b4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-01-23 06:27:46.811115 dmenuplaylist-0.0.0b3/
--rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 dmenuplaylist-0.0.0b3/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      621 2023-01-23 06:27:46.811115 dmenuplaylist-0.0.0b3/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      300 2023-01-11 07:53:32.000000 dmenuplaylist-0.0.0b3/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      549 2023-01-23 06:09:11.000000 dmenuplaylist-0.0.0b3/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-01-23 06:27:46.811115 dmenuplaylist-0.0.0b3/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-01-23 06:27:46.807782 dmenuplaylist-0.0.0b3/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-01-23 06:27:46.811115 dmenuplaylist-0.0.0b3/src/dmenuplaylist/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1351 2023-01-11 06:43:22.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1599 2023-01-11 05:09:52.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      992 2023-01-11 06:15:40.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1612 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      657 2023-01-11 06:56:33.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4365 2023-01-23 06:23:34.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-01-23 06:27:46.811115 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      621 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      516 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       62 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       17 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       14 2023-01-23 06:27:46.000000 dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 dmenuplaylist-0.0.0b4/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      741 2023-01-25 06:34:34.000000 dmenuplaylist-0.0.0b4/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      549 2023-04-14 00:30:46.000000 dmenuplaylist-0.0.0b4/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/dmenuplaylist/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1351 2023-01-11 06:43:22.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1599 2023-01-11 05:09:52.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      992 2023-01-11 06:15:40.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1615 2023-04-14 00:27:25.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      657 2023-01-11 06:56:33.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4408 2023-01-30 05:36:22.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:31:34.545925 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     1062 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      516 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       62 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       17 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       14 2023-04-14 00:31:34.000000 dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/top_level.txt
```

### Comparing `dmenuplaylist-0.0.0b3/LICENSE` & `dmenuplaylist-0.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b3/pyproject.toml` & `dmenuplaylist-0.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmenuplaylist"
-version = "0.0.0.b3"
+version = "0.0.0.b4"
 description = "Simple playlist manager, meant to be used with mpv."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv", "dmenu" ]
 dependencies = [
     "loadconf",
     "promptx"
```

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/__main__.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/__main__.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/config.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/config.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/options.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/options.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/prompts.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 
     choice = p.ask(
         options=options,
         prompt=prompt,
         additional_args=cmd_args,
     )
 
-    return choice
+    return choice[0]
```

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/system.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/system.py`

 * *Files identical despite different names*

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist/utils.py` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+from yt_dlp import YoutubeDL as YTDL
 import json
 import re
 import string
 import sys
 from urllib import parse
 import urllib.request as request
 from .prompts import user_choice, InvalidCmdPrompt, InputError
@@ -119,25 +120,26 @@
 def process_url(url):
     """
     Process urls
     """
     # use some regex and urllib.parse.unquote to get titles for magnet links
     # figure out some way to get titles for youtube videos
     # change structure to dict with title as the key and actual url/file as the value
+    title = url
     if is_magnet(url):
         raw_title = parse.unquote(url)
         prog = re.compile(r"&dn=(.*)&xl=")
+        title_match = prog.search(raw_title)
+        if title_match is not None:
+            return title_match.group(1)
     else:
-        page = request.urlopen(url)
-        raw_title = page.read().decode("utf8")
-        prog = re.compile(r"<meta property=\"og:title\" content=\"(.*)\">\n")
-    title_match = prog.search(raw_title)
-    if title_match is not None:
-        return title_match.group(1)
-    return url
+        with YTDL({}) as ydl:
+            info_dict = ydl.extract_info(url, download=False)
+        title = info_dict.get("title", None)
+    return title
 
 
 def remove_item(user):
     """
     Remove selected items from user's playlist
     """
     with open(user.files["playlist_file"], "r") as data:
```

### Comparing `dmenuplaylist-0.0.0b3/src/dmenuplaylist.egg-info/SOURCES.txt` & `dmenuplaylist-0.0.0b4/src/dmenuplaylist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

