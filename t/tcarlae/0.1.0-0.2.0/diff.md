# Comparing `tmp/tcarlae-0.1.0.tar.gz` & `tmp/tcarlae-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcarlae-0.1.0.tar", last modified: Wed Mar 22 13:01:08 2023, max compression
+gzip compressed data, was "tcarlae-0.2.0.tar", last modified: Fri Apr 14 12:51:42 2023, max compression
```

## Comparing `tcarlae-0.1.0.tar` & `tcarlae-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      714 2023-03-22 12:52:08.599963 tcarlae-0.1.0/README.md
--rw-r--r--   0        0        0      488 2023-03-15 21:12:52.827388 tcarlae-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-12 13:28:26.804352 tcarlae-0.1.0/src/tcarlae/__init__.py
--rw-r--r--   0        0        0      191 2023-03-15 20:47:06.714973 tcarlae-0.1.0/src/tcarlae/cli.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 tcarlae-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      814 2023-04-14 12:50:24.711957 tcarlae-0.2.0/README.md
+-rw-r--r--   0        0        0      494 2023-04-14 12:51:42.945882 tcarlae-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-12 13:28:26.804352 tcarlae-0.2.0/src/tcarlae/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-15 20:47:06.714973 tcarlae-0.2.0/src/tcarlae/cli.py
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 tcarlae-0.2.0/PKG-INFO
```

### Comparing `tcarlae-0.1.0/PKG-INFO` & `tcarlae-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: tcarlae
-Version: 0.1.0
+Version: 0.2.0
 Summary: Minimal Python repository with a simple development workflow. Share and enjoy!
+Author-Email: David Seaward <david@librem.one>
 License: CC0-1.0
-Author-email: David Seaward <david@librem.one>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # T. carlae
 
 Minimal Python repository with a simple development workflow. Share and enjoy!
 
-As of 2008, the Barbados threadsnake (Tetracheilostoma carlae, or T. carlae) is
-the smallest known snake species in the world.
-
 ## Workflow
 
 ```bash
 $ git clone https://gitlab.com/lfdo/tcarlae.git
 $ cd tcarlae
 $ pdm install --dev
 $ pdm run tcarlae
@@ -30,21 +27,27 @@
 $ pdm run python -m tcarlae.cli
 Hello world!
 ```
 
 And to publish:
 
 ```bash
-$ pdm publish
+$ git tag -a 2.0.0 -m "Version 2.0.0"
+$ pdm publish  # uses tag for version number
 ```
 
 # Sharing and contributions
 
 ```
 T. carlae
 https://lofidevops.neocities.org
 Copyright 2023 David Seaward and contributors
 SPDX-License-Identifier: CC0-1.0
 ```
 
-You can copy this freely without credit. It's mostly uncopyrightable anyway.
+You can copy and modify this project freely and without credit. It's mostly
+uncopyrightable anyway.
+
+# Colophon
 
+The Barbados threadsnake (known as Tetracheilostoma carlae or T. carlae) is the
+smallest known snake species in the world.
```

