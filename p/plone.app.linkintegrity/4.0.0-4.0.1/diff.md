# Comparing `tmp/plone.app.linkintegrity-4.0.0.tar.gz` & `tmp/plone.app.linkintegrity-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.linkintegrity-4.0.0.tar", last modified: Mon Mar 13 17:11:47 2023, max compression
+gzip compressed data, was "plone.app.linkintegrity-4.0.1.tar", last modified: Thu Apr 13 23:38:57 2023, max compression
```

## Comparing `plone.app.linkintegrity-4.0.0.tar` & `plone.app.linkintegrity-4.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.724029 plone.app.linkintegrity-4.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)    18526 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      150 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    23709 2023-03-13 17:11:47.724150 plone.app.linkintegrity-4.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4030 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.713875 plone.app.linkintegrity-4.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      685 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.714162 plone.app.linkintegrity-4.0.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.716895 plone.app.linkintegrity-4.0.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.719453 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.721118 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      510 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3258 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/delete_confirmation_info.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7573 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)     1229 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/update.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2562 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/update.py
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      673 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/exceptions.py
--rw-r--r--   0 maurits    (501) staff       (20)     5779 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      205 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1887 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/parser.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.711014 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.721800 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      236 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1546 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/retriever.py
--rw-r--r--   0 maurits    (501) staff       (20)     2969 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.723633 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      225 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4373 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_circular.py
--rw-r--r--   0 maurits    (501) staff       (20)    17073 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     2362 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2357 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_imagescales.py
--rw-r--r--   0 maurits    (501) staff       (20)     9195 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_references.py
--rw-r--r--   0 maurits    (501) staff       (20)      167 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2585 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:11:47.716651 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    23709 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1598 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      158 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      110 2023-03-13 17:11:47.724609 plone.app.linkintegrity-4.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1980 2023-03-13 17:11:47.000000 plone.app.linkintegrity-4.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.922919 plone.app.linkintegrity-4.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    18634 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      150 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    23818 2023-04-13 23:38:57.923220 plone.app.linkintegrity-4.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4031 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.909153 plone.app.linkintegrity-4.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      685 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.909547 plone.app.linkintegrity-4.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.913302 plone.app.linkintegrity-4.0.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.916972 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.919326 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      498 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4158 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/delete_confirmation_info.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7457 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1581 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/update.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/update.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1300 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5789 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      174 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1887 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/parser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.905037 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.920187 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      253 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1533 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/retriever.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.922682 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      201 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4324 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_circular.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17112 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2352 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_imagescales.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9317 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_references.py
+-rw-r--r--   0 maurits    (501) staff       (20)      167 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:38:57.912956 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    23818 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1598 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      300 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:38:57.923667 plone.app.linkintegrity-4.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2206 2023-04-13 23:38:57.000000 plone.app.linkintegrity-4.0.1/setup.py
```

### Comparing `plone.app.linkintegrity-4.0.0/CHANGES.rst` & `plone.app.linkintegrity-4.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 4.0.0 (2023-03-13)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility for Plone 5.2.  Support Plone 6 only.
@@ -534,15 +544,15 @@
   [davisagli]
 
 - Use the `get` method to retrieve the field value if the instance
   does not provide an accessor method. This is the case for instance
   for fields which have been added via schema extension.
   [malthe]
 
-- Support resolveuid/UID references explicitely, by parsing and resolving
+- Support resolveuid/UID references explicitly, by parsing and resolving
   these ourselves instead of relying on a view or script (which doesn't work).
   This fixes linkintegrity for sites with link-by-uid turned on.
   This closes https://dev.plone.org/ticket/12104
   [mj]
 
 1.4.4 - 2011-10-04
 ------------------
```

### Comparing `plone.app.linkintegrity-4.0.0/PKG-INFO` & `plone.app.linkintegrity-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.0
+Version: 4.0.1
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -90,15 +90,15 @@
 interface for your contenttype. Look at the ``retriever`` module in this
 package for examples.
 
 API
 ---
 
 To check if there would be breaches when deleting one or more objects
-you can use the follwing code:
+you can use the following code:
 
 .. code-block:: python
 
     from plone import api
     portal = api.portal.get()
     view = api.content.get_view(
         'delete_confirmation_info',
@@ -146,14 +146,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 4.0.0 (2023-03-13)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility for Plone 5.2.  Support Plone 6 only.
@@ -676,15 +686,15 @@
   [davisagli]
 
 - Use the `get` method to retrieve the field value if the instance
   does not provide an accessor method. This is the case for instance
   for fields which have been added via schema extension.
   [malthe]
 
-- Support resolveuid/UID references explicitely, by parsing and resolving
+- Support resolveuid/UID references explicitly, by parsing and resolving
   these ourselves instead of relying on a view or script (which doesn't work).
   This fixes linkintegrity for sites with link-by-uid turned on.
   This closes https://dev.plone.org/ticket/12104
   [mj]
 
 1.4.4 - 2011-10-04
 ------------------
```

### Comparing `plone.app.linkintegrity-4.0.0/README.rst` & `plone.app.linkintegrity-4.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 interface for your contenttype. Look at the ``retriever`` module in this
 package for examples.
 
 API
 ---
 
 To check if there would be breaches when deleting one or more objects
-you can use the follwing code:
+you can use the following code:
 
 .. code-block:: python
 
     from plone import api
     portal = api.portal.get()
     view = api.content.get_view(
         'delete_confirmation_info',
```

### Comparing `plone.app.linkintegrity-4.0.0/docs/LICENSE.GPL` & `plone.app.linkintegrity-4.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.0/docs/LICENSE.txt` & `plone.app.linkintegrity-4.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/delete_confirmation_info.pt` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/delete_confirmation_info.pt`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,135 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    i18n:domain="plone"
-    tal:omit-tag="">
-<body tal:omit-tag="" tal:define="breaches python:view.breaches">
-
-  <h2 tal:condition="breaches" i18n:translate="linkintegrity_breaches_title">Potential link breakage</h2>
-
-  <div id="content-core">
-
-    <p tal:condition="breaches" i18n:translate="linkintegrity_instructions">
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      xml:lang="en"
+      tal:omit-tag=""
+      i18n:domain="plone"
+>
+  <body tal:define="
+          breaches python:view.breaches;
+        "
+        tal:omit-tag=""
+  >
+
+    <h2 tal:condition="breaches"
+        i18n:translate="linkintegrity_breaches_title"
+    >Potential link breakage</h2>
+
+    <div id="content-core">
+
+      <p tal:condition="breaches"
+         i18n:translate="linkintegrity_instructions"
+      >
       By deleting this item, you will break links that exist in the items listed
       below. If this is indeed what you want to do, we recommend that you remove
       these references first.
-    </p>
+      </p>
 
-    <div tal:define="token context/@@authenticator/token">
-      <article tal:repeat="breach breaches" class="breach-container">
+      <div tal:define="
+             token context/@@authenticator/token;
+           ">
+        <article class="breach-container"
+                 tal:repeat="breach breaches"
+        >
+
+          <tal:target tal:define="
+                        target breach/target;
+                      ">
+            <header><a href="${target/url}"
+                 tal:content="target/title"
+              ></a></header>
+            <p>
+              <span i18n:translate="linkintegrity_is_referenced">
+              This
+                <span tal:content="target/type_title"
+                      i18n:name="portal_type"
+                ></span>
+              is referenced by the following items:
+              </span>
+            </p>
+          </tal:target>
+
+          <ul>
+            <li class="breach-item"
+                tal:repeat="source python:breach['sources']"
+            >
+              <tal:visible condition="source/accessible">
+                <a tal:content="source/title"
+                   tal:attributes="
+                     href source/url;
+                   "
+                ></a>
+                [<a target="_blank"
+                   tal:attributes="
+                     href string:${source/url}/edit?_authenticator=${token};
+                   "
+                   i18n:translate="linkintegrity_edit_in_new_window"
+                >Edit in new window</a>]
+              </tal:visible>
+              <tal:private condition="not: source/accessible"
+                           i18n:translate="linkintegrity_item_not_accessible"
+              >
+              The item is not accessible.
+              </tal:private>
+            </li>
+          </ul>
+
+        </article>
+
+        <div tal:define="
+               breach_count view/breach_count;
+             "
+             tal:condition="breach_count"
+        >
 
-        <tal:target  tal:define="target breach/target">
-          <header><a href="${target/url}" tal:content="target/title" /></header>
+          <h2 i18n:translate="deleting_overview">Deleting overview</h2>
           <p>
-            <span i18n:translate="linkintegrity_is_referenced">
-              This <span i18n:name="portal_type" tal:content="target/type_title" />
-              is referenced by the following items:
+            <span tal:define="
+                    refs python:len(breach_count);
+                  "
+                  i18n:translate="selected_folders_with_content"
+            >
+            Number of selected, non-empty folders:
+              <strong><span tal:replace="refs"
+                      i18n:name="refs"
+                ></span></strong>
             </span>
           </p>
-        </tal:target>
-
-        <ul>
-          <li tal:repeat="source python:breach['sources']" class="breach-item">
-            <tal:visible condition="source/accessible">
-              <a tal:attributes="href source/url" tal:content="source/title" />
-              [<a
-                  tal:attributes="href string:${source/url}/edit?_authenticator=${token}"
-                  i18n:translate="linkintegrity_edit_in_new_window"
-                  target="_blank">Edit in new window</a>]
-            </tal:visible>
-            <tal:private
-                condition="not: source/accessible"
-                i18n:translate="linkintegrity_item_not_accessible">
-              The item is not accessible.
-            </tal:private>
-          </li>
-        </ul>
-
-      </article>
-
-      <div tal:define="breach_count view/breach_count" tal:condition="breach_count">
-
-        <h2 i18n:translate="deleting_overview" >Deleting overview</h2>
-        <p>
-          <span tal:define="refs python:len(breach_count)"
-              i18n:translate="selected_folders_with_content">
-            Number of selected, non-empty folders: <strong><span tal:replace="refs" i18n:name="refs" /></strong>
-          </span>
+          <ul>
+            <li tal:repeat="content python:breach_count">
+              <span i18n:translate="deleting_contents">
+                 Following content within
+                <strong><span tal:replace="content"
+                        i18n:name="content"
+                  ></span></strong>
+                  will also be deleted:
+              </span><br />
+              <ul>
+                <li tal:define="
+                      objects view/objects;
+                    "
+                    tal:repeat="item python:range(3) "
+                >
+                  <span tal:replace="python: breach_count[content][item]"></span>
+                  <span tal:replace="python: objects[item]"></span>
+                </li>
+              </ul>
+            </li>
+          </ul>
+
+        </div>
+
+        <p tal:condition="breaches"
+           i18n:translate="linkintegrity_delete_anyway"
+        >
+        Would you like to delete it anyway?
         </p>
-        <ul>
-          <li tal:repeat="content python:breach_count">
-            <span i18n:translate="deleting_contents"> Following content within
-              <strong><span tal:replace="content" i18n:name="content" /></strong>  will also be deleted:
-            </span><br/>
-            <ul>
-              <li tal:define="objects view/objects"
-                  tal:repeat="item python:range(3) ">
-                <span tal:replace="python: breach_count[content][item]" /> <span tal:replace="python: objects[item]" />
-              </li>
-            </ul>
-          </li>
-        </ul>
 
       </div>
 
-      <p tal:condition="breaches" i18n:translate="linkintegrity_delete_anyway">
-        Would you like to delete it anyway?
-      </p>
-
     </div>
 
-  </div>
-
-</body>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ***** Potential link breakage *****
 By deleting this item, you will break links that exist in the items listed
 below. If this is indeed what you want to do, we recommend that you remove
 these references first.
 
- This__is_referenced_by_the_following_items:
-    *__[Edit_in_new_window]___The_item_is_not_accessible.
-*****_Deleting_overview_*****
- Number_of_selected,_non-empty_folders:
-    *__Following_content_within__will_also_be_deleted:
+ This  is referenced by the following items:
+    *   [Edit in new window]   The item is not accessible.
+***** Deleting overview *****
+ Number of selected, non-empty folders:
+    *  Following content within  will also be deleted:
           o
-Would_you_like_to_delete_it_anyway?
+Would you like to delete it anyway?
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/info.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_inner
 from OFS.interfaces import IFolder
 from plone.app.linkintegrity.utils import getIncomingLinks
 from plone.app.linkintegrity.utils import linkintegrity_enabled
+from plone.base import PloneMessageFactory as _
+from plone.base.interfaces import IPloneSiteRoot
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.permissions import AccessContentsInformation
 from Products.CMFCore.utils import _checkPermission
 from Products.CMFCore.utils import getToolByName
-from plone.base import PloneMessageFactory as _
-from plone.base.interfaces import IPloneSiteRoot
 from Products.Five import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.i18n import translate
+
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteConfirmationInfo(BrowserView):
-
-    template = ViewPageTemplateFile('delete_confirmation_info.pt')
+    template = ViewPageTemplateFile("delete_confirmation_info.pt")
     breach_count = {}
 
     def __init__(self, context, request):
         self.linkintegrity_enabled = linkintegrity_enabled()
         self.context = context
         self.request = request
 
@@ -44,94 +43,87 @@
         """Return breaches for multiple items.
 
         Breaches coming from objects in the list of items
         or their children (if a object is a folder) will be ignored.
         """
         if items is None:
             items = [self.context]
-        catalog = getToolByName(self.context, 'portal_catalog')
+        catalog = getToolByName(self.context, "portal_catalog")
         results = []
         uids_to_ignore = []
         uids_visited = set()
         self.breach_count = {}
         for obj in items:
-            obj_path = '/'.join(obj.getPhysicalPath())
-            brains_to_delete = catalog(path={'query': obj_path})
-            # add the current items uid and all its childrens uids to the
+            obj_path = "/".join(obj.getPhysicalPath())
+            brains_to_delete = catalog(path={"query": obj_path})
+            # add the current items uid and all its children's uids to the
             # list of uids that are ignored
             uids_to_ignore.extend([i.UID for i in brains_to_delete])
             for brain_to_delete in brains_to_delete:
                 try:
                     obj_to_delete = brain_to_delete.getObject()  # noqa
                 except (AttributeError, KeyError):
                     logger.exception(
-                        'No object found for %s! Skipping', brain_to_delete)
+                        "No object found for %s! Skipping", brain_to_delete
+                    )
                     continue
                 for breach in self.get_breaches_for_item(obj):
                     add_breach = False
-                    for source in breach['sources']:
+                    for source in breach["sources"]:
                         # Only add the breach if one the sources is not in the
                         # list of items that are to be deleted.
-                        if source['uid'] not in uids_to_ignore and \
-                           source['uid'] not in uids_visited:
+                        if (
+                            source["uid"] not in uids_to_ignore
+                            and source["uid"] not in uids_visited
+                        ):
                             add_breach = True
-                            uids_visited.add(source['uid'])
+                            uids_visited.add(source["uid"])
                             break
                     if add_breach:
                         results.append(breach)
             if IFolder.providedBy(obj):
-                count = len(catalog(
-                    path={'query': obj_path}
-                ))
-                count_dirs = len(catalog(
-                    path={'query': obj_path},
-                    is_folderish=True
-                ))
-                count_public = len(catalog(
-                    path={'query': obj_path},
-                    review_state='published'
-                ))
+                count = len(catalog(path={"query": obj_path}))
+                count_dirs = len(catalog(path={"query": obj_path}, is_folderish=True))
+                count_public = len(
+                    catalog(path={"query": obj_path}, review_state="published")
+                )
                 if count:
-                    self.breach_count[obj_path] = [
-                        count,
-                        count_dirs,
-                        count_public
-                    ]
+                    self.breach_count[obj_path] = [count, count_dirs, count_public]
 
         # Cleanup: Some breaches where added before it was known
         # that their source will be deleted too.
         for result in results:
-            for source in result['sources']:
-                if source['uid'] in uids_to_ignore:
+            for source in result["sources"]:
+                if source["uid"] in uids_to_ignore:
                     # Drop sources that are also being deleted
-                    result['sources'].remove(source)
-                    if not result['sources']:
+                    result["sources"].remove(source)
+                    if not result["sources"]:
                         # Remove the breach is there are no more sources
                         # This check is necessary since there can be multiple
                         # sources for a breach
                         results.remove(result)
         return results
 
     def get_breaches_for_item(self, obj=None):
         """Get breaches for one object and its children.
 
         Breaches coming from the children of a folder are ignored by default.
         """
         if obj is None:
             obj = self.context
         results = []
-        catalog = getToolByName(obj, 'portal_catalog')
-        obj_path = '/'.join(obj.getPhysicalPath())
+        catalog = getToolByName(obj, "portal_catalog")
+        obj_path = "/".join(obj.getPhysicalPath())
 
         breaches = self.check_object(obj)
         if breaches:
             results.append(breaches)
 
         if IFolder.providedBy(obj):
-            brains = catalog(path={'query': obj_path})
+            brains = catalog(path={"query": obj_path})
             for brain in brains:
                 try:
                     child = brain.getObject()
                 except (AttributeError, KeyError):
                     continue
                 if child == obj:
                     continue
@@ -153,44 +145,45 @@
             if not source_path:
                 # link is broken
                 continue
             if excluded_path and source_path.startswith(excluded_path):
                 # source is in excluded_path
                 continue
             source = direct_link.from_object
-            if not breaches.get('sources'):
-                breaches['sources'] = []
-            breaches['sources'].append({
-                'uid': IUUID(source),
-                'title': source.Title(),
-                'url': source.absolute_url(),
-                'accessible': self.is_accessible(source),
-            })
+            if not breaches.get("sources"):
+                breaches["sources"] = []
+            breaches["sources"].append(
+                {
+                    "uid": IUUID(source),
+                    "title": source.Title(),
+                    "url": source.absolute_url(),
+                    "accessible": self.is_accessible(source),
+                }
+            )
             has_breaches = True
         if has_breaches:
-            breaches['target'] = {
-                'uid': IUUID(obj),
-                'title': obj.Title(),
-                'url': obj.absolute_url(),
-                'portal_type': obj.portal_type,
-                'type_title': self.get_portal_type_title(obj),
+            breaches["target"] = {
+                "uid": IUUID(obj),
+                "title": obj.Title(),
+                "url": obj.absolute_url(),
+                "portal_type": obj.portal_type,
+                "type_title": self.get_portal_type_title(obj),
             }
             return breaches
 
     def get_portal_type_title(self, obj):
-        """Get the portal type title of the object.
-        """
+        """Get the portal type title of the object."""
         context = aq_inner(self.context)
-        portal_types = getToolByName(context, 'portal_types')
+        portal_types = getToolByName(context, "portal_types")
         fti = portal_types.get(obj.portal_type)
         if fti is not None:
             type_title_msgid = fti.Title()
         else:
             type_title_msgid = obj.portal_type
         type_title = translate(type_title_msgid, context=self.request)
         return type_title
 
     def is_accessible(self, obj):
         return _checkPermission(AccessContentsInformation, obj)
 
     def objects(self):
-        return [_('Objects in all'), _('Folders'), _('Published objects')]
+        return [_("Objects in all"), _("Folders"), _("Published objects")]
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/browser/update.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/browser/update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_inner
 from datetime import datetime
 from datetime import timedelta
 from plone.app.linkintegrity.handlers import modifiedContent
-from Products.CMFCore.utils import getToolByName
 from plone.base import PloneMessageFactory as _
+from Products.CMFCore.utils import getToolByName
 from Products.Five import BrowserView
 from Products.statusmessages.interfaces import IStatusMessage
 from transaction import savepoint
 from zExceptions import NotFound
 
 import logging
+
+
 logger = logging.getLogger(__name__)
 
 
 class UpdateView(BrowserView):
-    """Iterate over all catalogued items and update linkintegrity-information.
-    """
+    """Iterate over all catalogued items and update linkintegrity-information."""
 
     def __call__(self):
         context = aq_inner(self.context)
         request = aq_inner(self.request)
-        if 'update' in request.form or 'delete_all' in request.form:
+        if "update" in request.form or "delete_all" in request.form:
             starttime = datetime.now()
             count = self.update()
             duration = timedelta(seconds=(datetime.now() - starttime).seconds)
             msg = _(
-                u'linkintegrity_update_info',
-                default=u'Link integrity information updated for ${count} ' +
-                        u'items in ${time} seconds.',
-                mapping={'count': count, 'time': str(duration)},
+                "linkintegrity_update_info",
+                default="Link integrity information updated for ${count} "
+                + "items in ${time} seconds.",
+                mapping={"count": count, "time": str(duration)},
             )
-            IStatusMessage(request).add(msg, type='info')
-            msg = 'Updated {0} items in {1} seconds'.format(
+            IStatusMessage(request).add(msg, type="info")
+            msg = "Updated {} items in {} seconds".format(
                 count,
                 str(duration),
             )
             logger.info(msg)
-            request.RESPONSE.redirect(getToolByName(context, 'portal_url')())
-        elif 'cancel' in request.form:
-            msg = _(u'Update cancelled.')
-            IStatusMessage(request).add(msg, type='info')
-            request.RESPONSE.redirect(getToolByName(context, 'portal_url')())
+            request.RESPONSE.redirect(getToolByName(context, "portal_url")())
+        elif "cancel" in request.form:
+            msg = _("Update cancelled.")
+            IStatusMessage(request).add(msg, type="info")
+            request.RESPONSE.redirect(getToolByName(context, "portal_url")())
         else:
             return self.index()
 
     def update(self):
-        catalog = getToolByName(self.context, 'portal_catalog')
+        catalog = getToolByName(self.context, "portal_catalog")
         count = 0
 
         for brain in catalog():
             try:
                 obj = brain.getObject()
             except (AttributeError, NotFound, KeyError):
-                msg = 'Catalog inconsistency: {0} not found!'
+                msg = "Catalog inconsistency: {0} not found!"
                 logger.error(msg.format(brain.getPath()), exc_info=1)
                 continue
             try:
-                modifiedContent(obj, 'dummy event parameter')
+                modifiedContent(obj, "dummy event parameter")
                 count += 1
             except Exception:
-                msg = 'Error updating linkintegrity-info for {0}.'
+                msg = "Error updating linkintegrity-info for {0}."
                 logger.error(msg.format(obj.absolute_url()), exc_info=1)
             if count % 1000 == 0:
                 savepoint(optimistic=True)
         return count
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/configure.zcml` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,43 @@
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     >
 
   <include package="plone.app.intid" />
   <include package="plone.app.relationfield" />
-  <include package="Products.CMFCore" file="permissions.zcml" />
+  <include
+      package="Products.CMFCore"
+      file="permissions.zcml"
+      />
 
   <include package=".browser" />
 
   <adapter factory=".retriever.DXGeneral" />
 
   <subscriber
       for="plone.app.relationfield.interfaces.IDexterityHasRelations
-            zope.lifecycleevent.interfaces.IObjectCopiedEvent"
-      handler=".handlers.modifiedContent" />
+           zope.lifecycleevent.interfaces.IObjectCopiedEvent"
+      handler=".handlers.modifiedContent"
+      />
 
   <subscriber
       for="plone.app.relationfield.interfaces.IDexterityHasRelations
-            zope.lifecycleevent.interfaces.IObjectAddedEvent"
-      handler=".handlers.modifiedContent" />
+           zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler=".handlers.modifiedContent"
+      />
 
   <subscriber
       for="plone.app.relationfield.interfaces.IDexterityHasRelations
-            zope.lifecycleevent.interfaces.IObjectModifiedEvent"
-      handler=".handlers.modifiedContent" />
+           zope.lifecycleevent.interfaces.IObjectModifiedEvent"
+      handler=".handlers.modifiedContent"
+      />
 
   <genericsetup:registerProfile
       name="default"
       title="plone.app.linkintegrity"
-      directory="profiles/default"
       description="Installs the plone.app.linkintegrity add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       />
 
 </configure>
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/exceptions.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# -*- coding: utf-8 -*-
 from OFS.ObjectManager import BeforeDeleteException
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 class ILinkIntegrityNotificationException(Interface):
-    """An exception indicating a prevented link integrity breach.
-    """
+    """An exception indicating a prevented link integrity breach."""
 
 
 @implementer(ILinkIntegrityNotificationException)
 class LinkIntegrityNotificationException(BeforeDeleteException):
-    """An exception indicating a prevented link integrity breach.
-    """
+    """An exception indicating a prevented link integrity breach."""
 
     def __str__(self):
         args = self.args
         if args and isinstance(args, tuple):
             return repr(args[0])
-        return super(LinkIntegrityNotificationException, self).__str__()
+        return super().__str__()
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/handlers.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from Acquisition import aq_get
 from Acquisition import aq_parent
 from plone.app.linkintegrity.interfaces import IRetriever
 from plone.app.linkintegrity.utils import ensure_intid
 from plone.app.linkintegrity.utils import referencedRelationship
 from plone.app.uuid.utils import uuidToCatalogBrain
+from plone.base.interfaces import IEditingSchema
+from plone.base.interfaces import IPloneSiteRoot
 from plone.dexterity.interfaces import IDexterityContent
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.interfaces import IEditingSchema
-from plone.base.interfaces import IPloneSiteRoot
 from urllib.parse import unquote
 from urllib.parse import urlsplit
 from z3c.relationfield import RelationValue
 from z3c.relationfield.event import _setRelation
 from zc.relation.interfaces import ICatalog
 from zExceptions import NotFound
 from ZODB.POSException import ConflictError
@@ -24,30 +24,30 @@
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 def findObject(base, path):
-    """ traverse to given path and find the upmost object """
-    if path.startswith('/'):
+    """traverse to given path and find the upmost object"""
+    if path.startswith("/"):
         # Make an absolute path relative to the portal root
-        obj = getToolByName(base, 'portal_url').getPortalObject()
-        portal_path = obj.absolute_url_path() + '/'
+        obj = getToolByName(base, "portal_url").getPortalObject()
+        portal_path = obj.absolute_url_path() + "/"
         if path.startswith(portal_path):
-            path = path[len(portal_path):]
+            path = path[len(portal_path) :]
     else:
-        obj = aq_parent(base)   # relative urls start at the parent...
+        obj = aq_parent(base)  # relative urls start at the parent...
 
-    components = path.split('/')
+    components = path.split("/")
 
-    # Support resolveuid/UID paths explicitely, without relying
+    # Support resolveuid/UID paths explicitly, without relying
     # on a view or skinscript to do this for us.
-    if 'resolveuid' in components:
-        uid = components[components.index('resolveuid') + 1]
+    if "resolveuid" in components:
+        uid = components[components.index("resolveuid") + 1]
         # This may be a link to a page that once was published but not anymore,
         # or the current editor does not have View permission.
         # In that case uuidToObject(uid) could fail with Unauthorized.
         brain = uuidToCatalogBrain(uid)
         if brain is not None:
             # Note: _unrestrictedGetObject starts with an underscore,
             # but it is documented in ZCatalog.interfaces,
@@ -58,31 +58,31 @@
 
     while components:
         child_id = unquote(components[0])
         try:
             try:
                 child = obj.unrestrictedTraverse(child_id)
             except AttributeError:
-                request = aq_get(obj, 'REQUEST')
+                request = aq_get(obj, "REQUEST")
                 child = request.traverseName(obj, child_id)
         except ConflictError:
             raise
-        except (AttributeError, KeyError,
-                NotFound, ztkNotFound, UnicodeEncodeError):
+        except (AttributeError, KeyError, NotFound, ztkNotFound, UnicodeEncodeError):
             return None, None
-        if not IDexterityContent.providedBy(child) and \
-                not IPloneSiteRoot.providedBy(child):
+        if not IDexterityContent.providedBy(child) and not IPloneSiteRoot.providedBy(
+            child
+        ):
             break
         obj = child
         components.pop(0)
-    return obj, '/'.join(components)
+    return obj, "/".join(components)
 
 
 def getObjectsFromLinks(base, links):
-    """ determine actual objects refered to by given links """
+    """determine actual objects referred to by given links"""
     intids = getUtility(IIntIds)
     objects = set()
     url = base.absolute_url()
     scheme, host, path, query, frag = urlsplit(url)
     for link in links:
         s, h, path, q, f = urlsplit(link)
         # relative or local url
@@ -124,32 +124,35 @@
     TODO: Might be improved by not changing anything if the links are the same.
     """
     int_id = ensure_intid(obj)
     if int_id is None:
         return
     catalog = getUtility(ICatalog)
     # unpack the rels before deleting
-    old_rels = [i for i in catalog.findRelations(
-        {'from_id': int_id,
-         'from_attribute': referencedRelationship})]
+    old_rels = [
+        i
+        for i in catalog.findRelations(
+            {"from_id": int_id, "from_attribute": referencedRelationship}
+        )
+    ]
     for old_rel in old_rels:
         catalog.unindex(old_rel)
     for ref in refs:
         _setRelation(obj, referencedRelationship, ref)
 
 
 def check_linkintegrity_dependencies(obj):
     try:
         reg = getUtility(IRegistry)
-        editing_settings = reg.forInterface(IEditingSchema, prefix='plone')
+        editing_settings = reg.forInterface(IEditingSchema, prefix="plone")
     except (ComponentLookupError, KeyError):
         return False
     if not editing_settings.enable_link_integrity_checks:
         return False
-    if not getToolByName(obj, 'portal_url', None):
+    if not getToolByName(obj, "portal_url", None):
         # `getObjectFromLinks` is not possible without access
         # to `portal_url`
         return False
     try:
         getUtility(IIntIds)
         getUtility(ICatalog)
     except ComponentLookupError:
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/parser.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/parser.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/retriever.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/retriever.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.schema import getFieldsInOrder
 
 
 @implementer(IRetriever)
 @adapter(IDexterityContent)
-class DXGeneral(object):
-    """General retriever for DX that extracts URLs from (rich) text fields.
-    """
+class DXGeneral:
+    """General retriever for DX that extracts URLs from (rich) text fields."""
 
     def __init__(self, context):
         self.context = context
 
     def retrieveLinks(self):
-        """Finds all links from the object and return them.
-        """
+        """Finds all links from the object and return them."""
         fti = getUtility(IDexterityFTI, name=self.context.portal_type)
         schema = fti.lookupSchema()
         additional_schema = getAdditionalSchemata(
-            context=self.context, portal_type=self.context.portal_type)
+            context=self.context, portal_type=self.context.portal_type
+        )
         schemas = [i for i in additional_schema] + [schema]
         links = set()
         for schema in schemas:
             for name, field in getFieldsInOrder(schema):
                 if isinstance(field, RichText):
                     value = getattr(schema(self.context), name)
-                    if not value or not getattr(value, 'raw', None):
+                    if not value or not getattr(value, "raw", None):
                         continue
                     links |= set(extractLinks(value.raw))
         return links
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_circular.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_circular.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 class CircularReferencesTestCase(unittest.TestCase):
     """Circular reference testcase"""
 
     layer = testing.PLONE_APP_LINKINTEGRITY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.request = self.layer['request']
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
 
     def _set_text(self, obj, text):
         obj.text = RichTextValue(text)
         modified(obj)
 
     def test_circular_reference_manages_relations(self):
-        doc1 = self.portal['doc1']
-        doc2 = self.portal['doc2']
-        doc3 = self.portal['doc3']
+        doc1 = self.portal["doc1"]
+        doc2 = self.portal["doc2"]
+        doc3 = self.portal["doc3"]
         self.assertFalse(hasIncomingLinks(doc1))
         self.assertFalse(hasIncomingLinks(doc2))
         self.assertFalse(hasIncomingLinks(doc3))
         set_text(doc1, '<a href="doc2">doc2</a>')
         set_text(doc2, '<a href="doc3">doc3</a>')
         set_text(doc3, '<a href="doc1">doc1</a>')
         self.assertTrue(hasIncomingLinks(doc1))
@@ -54,44 +54,41 @@
         self.assertEqual([r.to_object for r in getOutgoingLinks(doc1)], [doc2])
         self.assertEqual([r.to_object for r in getOutgoingLinks(doc2)], [doc3])
         self.assertEqual([r.to_object for r in getOutgoingLinks(doc3)], [doc4])
         self.assertEqual([r.to_object for r in getOutgoingLinks(doc4)], [doc1])
 
         view = DeleteConfirmationInfo(self.portal, self.request)
         self.assertEqual(len(view.get_breaches([folder1])), 1)
-        self.assertEqual(
-            len(view.get_breaches([doc1, doc2, doc3, folder1])), 0)
+        self.assertEqual(len(view.get_breaches([doc1, doc2, doc3, folder1])), 0)
         self.assertEqual(len(view.get_breaches([doc2, folder1])), 2)
 
     def test_internal_breaches_are_dropped(self):
         folder1 = self.portal.folder1
-        create(folder1, 'Document', id='doc5', title='Test Page 5')
+        create(folder1, "Document", id="doc5", title="Test Page 5")
         doc1 = self.portal.doc1
         doc4 = self.portal.folder1.doc4
         doc5 = self.portal.folder1.doc5
         set_text(doc1, '<a href="folder1">f1</a>')
         set_text(doc4, '<a href="doc5">d5</a><a href="../doc1">d1</a>')
         set_text(doc5, '<a href="../folder1">f1</a>')
 
-        doc4_breaches = set([r.to_object for r in getOutgoingLinks(doc4)])
+        doc4_breaches = {r.to_object for r in getOutgoingLinks(doc4)}
         # the order of breaches is non-deterministic
-        self.assertEqual(set([doc1, doc5]), doc4_breaches)
-        self.assertEqual(
-            [r.to_object for r in getOutgoingLinks(doc5)], [folder1])
-        self.assertEqual(
-            [r.to_object for r in getOutgoingLinks(doc1)], [folder1])
+        self.assertEqual({doc1, doc5}, doc4_breaches)
+        self.assertEqual([r.to_object for r in getOutgoingLinks(doc5)], [folder1])
+        self.assertEqual([r.to_object for r in getOutgoingLinks(doc1)], [folder1])
         view = DeleteConfirmationInfo(self.portal, self.request)
         self.assertEqual(len(view.get_breaches([doc4])), 0)
         self.assertEqual(len(view.get_breaches([doc5])), 1)
         self.assertEqual(len(view.get_breaches([doc4, doc5])), 0)
         self.assertEqual(len(view.get_breaches([folder1])), 1)
         self.assertEqual(len(view.get_breaches([doc1])), 1)
         self.assertEqual(len(view.get_breaches([doc1, folder1])), 0)
 
-        view = folder1.restrictedTraverse('delete_confirmation')
-        self.assertIn('Potential link breakage', view())
-        view = folder1.restrictedTraverse('delete_confirmation_info')
-        self.assertIn('Potential link breakage', view())
-        view = doc4.restrictedTraverse('delete_confirmation')
-        self.assertNotIn('Potential link breakage', view())
-        view = doc4.restrictedTraverse('delete_confirmation_info')
-        self.assertNotIn('Potential link breakage', view())
+        view = folder1.restrictedTraverse("delete_confirmation")
+        self.assertIn("Potential link breakage", view())
+        view = folder1.restrictedTraverse("delete_confirmation_info")
+        self.assertIn("Potential link breakage", view())
+        view = doc4.restrictedTraverse("delete_confirmation")
+        self.assertNotIn("Potential link breakage", view())
+        view = doc4.restrictedTraverse("delete_confirmation_info")
+        self.assertNotIn("Potential link breakage", view())
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_functional.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,157 +3,167 @@
 from plone.app.linkintegrity.utils import getIncomingLinks
 from plone.app.linkintegrity.utils import getOutgoingLinks
 from plone.app.linkintegrity.utils import hasOutgoingLinks
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
+from plone.base.interfaces import IEditingSchema
 from plone.registry.interfaces import IRegistry
 from plone.testing.zope import Browser
-from plone.base.interfaces import IEditingSchema
 from zc.relation.interfaces import ICatalog
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 
+import re
 import transaction
 import unittest
 
 
 class FunctionalReferenceTestCase(unittest.TestCase):
     """functional reference testcase"""
 
     layer = testing.PLONE_APP_LINKINTEGRITY_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.request = self.layer['request']
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
         # alsoProvides(self.request, IFormLayer)
 
         # Get a testbrowser
-        self.browser = Browser(self.layer['app'])
+        self.browser = Browser(self.layer["app"])
         self.browser.handleErrors = False
-        self.browser.addHeader('Referer', self.portal.absolute_url())
+        self.browser.addHeader("Referer", self.portal.absolute_url())
         self.browser.addHeader(
-            'Authorization',
-            'Basic {0:s}:{1:s}'.format(TEST_USER_NAME, TEST_USER_PASSWORD))
+            "Authorization", f"Basic {TEST_USER_NAME:s}:{TEST_USER_PASSWORD:s}"
+        )
 
         # Do an initial page load to make sure the bundles get compiled
         # (which currently commits a transaction)
         # before we render exception views
         self.browser.open(self.portal.absolute_url())
 
-        setRoles(self.portal, TEST_USER_ID, ['Manager', ])
+        setRoles(
+            self.portal,
+            TEST_USER_ID,
+            [
+                "Manager",
+            ],
+        )
 
     def _get_token(self, obj):
-        return getMultiAdapter(
-            (obj, self.request), name='authenticator').token()
+        return getMultiAdapter((obj, self.request), name="authenticator").token()
 
-    @unittest.skip('Re-enable after https://github.com/plone/plone.app.content/issues/38')  # noqa
+    @unittest.skip(
+        "Re-enable after https://github.com/plone/plone.app.content/issues/38"
+    )  # noqa
     def test_file_reference_linkintegrity_page_is_shown(self):
         doc1 = self.portal.doc1
-        file2 = testing.create(self.portal, 'File',
-                               id='file2', file=testing.GIF)
+        file2 = testing.create(self.portal, "File", id="file2", file=testing.GIF)
 
         self.assertFalse(hasOutgoingLinks(doc1))
         set_text(doc1, '<a href="file2">A File</a>')
         self.assertTrue(hasOutgoingLinks(doc1))
-        self.assertIn('file2', self.portal.objectIds())
+        self.assertIn("file2", self.portal.objectIds())
 
         token = self._get_token(file2)
-        self.request['_authenticator'] = token
+        self.request["_authenticator"] = token
 
         # Make changes visible to test browser
         transaction.commit()
 
         self.browser.handleErrors = True
         self.browser.addHeader(
-            'Authorization',
-            'Basic {0:s}:{1:s}'.format(TEST_USER_NAME, TEST_USER_PASSWORD))
+            "Authorization", f"Basic {TEST_USER_NAME:s}:{TEST_USER_PASSWORD:s}"
+        )
 
-        delete_url = '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
-            file2.absolute_url(), token)
+        delete_url = "{:s}/delete_confirmation?_authenticator={:s}".format(
+            file2.absolute_url(), token
+        )
 
         # Try to remove but cancel
         self.browser.open(delete_url)
 
         # Validate text
-        self.assertIn('Potential link breakage', self.browser.contents)
-        self.assertIn('<a href="http://nohost/plone/doc1">Test Page 1</a>',
-                      self.browser.contents)
-        self.assertIn('Would you like to delete it anyway?',
-                      self.browser.contents)
+        self.assertIn("Potential link breakage", self.browser.contents)
+        self.assertIn(
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', self.browser.contents
+        )
+        self.assertIn("Would you like to delete it anyway?", self.browser.contents)
 
         # Click cancel button, item should stay in place
         # FIXME! This fails in Plone 6 with an internal server error,
         # but maybe no longer for the original reasons for which we skip this test.
-        self.browser.getControl(name='form.buttons.Cancel').click()
-        self.assertEqual(self.browser.url, file2.absolute_url() + '/view')
-        self.assertIn('Removal cancelled.', self.browser.contents)
-        self.assertIn('file2', self.portal.objectIds())
+        self.browser.getControl(name="form.buttons.Cancel").click()
+        self.assertEqual(self.browser.url, file2.absolute_url() + "/view")
+        self.assertIn("Removal cancelled.", self.browser.contents)
+        self.assertIn("file2", self.portal.objectIds())
 
         # Try to remove and confirm
         self.browser.open(delete_url)
-        self.browser.getControl(name='form.buttons.Delete').click()
-        self.assertNotIn('file2', self.portal.objectIds())
+        self.browser.getControl(name="form.buttons.Delete").click()
+        self.assertNotIn("file2", self.portal.objectIds())
 
     def test_unreferenced_removal(self):
         # This tests against #6666 and #7784, simple removal of a not
         # referenced file, which broke zeo-based installations.
 
         # We simply use a browser to try to delete a content item.
         self.browser.open(self.portal.doc1.absolute_url())
-        self.browser.getLink('Delete').click()
-        self.assertIn(
-            'Do you really want to delete this item?', self.browser.contents)
-        self.browser.getControl(name='form.buttons.Delete').click()
+        self.browser.getLink("Delete").click()
+        self.assertIn("Do you really want to delete this item?", self.browser.contents)
+        self.browser.getControl(name="form.buttons.Delete").click()
 
         # The resulting page should confirm the removal:
-        self.assertIn('Test Page 1 has been deleted', self.browser.contents)
-        self.assertNotIn('doc1', self.portal.objectIds())
+        self.assertIn("Test Page 1 has been deleted", self.browser.contents)
+        self.assertNotIn("doc1", self.portal.objectIds())
 
     def test_renaming_referenced_item(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
 
         # This tests makes sure items that are linked to can still be
         # renamed (see the related bug report in #6608).  First we need
         # to create the necessary links:
         set_text(doc1, '<a href="doc2">doc2</a>')
-        self.assertEqual(
-            [i.from_object for i in getIncomingLinks(doc2)], [doc1])
+        self.assertEqual([i.from_object for i in getIncomingLinks(doc2)], [doc1])
 
         # Make changes visible to testbrowseropen
         transaction.commit()
 
         # Then we use a browser to rename the referenced image:
         self.browser.handleErrors = True
-        self.browser.open('{0:s}/object_rename?_authenticator={1:s}'.format(
-            doc1.absolute_url(), self._get_token(doc1)))
+        self.browser.open(
+            "{:s}/object_rename?_authenticator={:s}".format(
+                doc1.absolute_url(), self._get_token(doc1)
+            )
+        )
 
-        self.browser.getControl(name='form.widgets.new_id').value = 'nuname'
-        self.browser.getControl(name='form.buttons.Rename').click()
+        self.browser.getControl(name="form.widgets.new_id").value = "nuname"
+        self.browser.getControl(name="form.buttons.Rename").click()
         self.assertIn("Renamed 'doc1' to 'nuname'.", self.browser.contents)
         transaction.commit()
 
-        self.assertNotIn('doc1', self.portal.objectIds())
-        self.assertIn('nuname', self.portal.objectIds())
+        self.assertNotIn("doc1", self.portal.objectIds())
+        self.assertIn("nuname", self.portal.objectIds())
         self.assertIn(doc1, [i.from_object for i in getIncomingLinks(doc2)])
 
         # We simply use a browser to try to delete a content item.
         self.browser.open(doc2.absolute_url())
-        self.browser.getLink('Delete').click()
-        self.assertIn(
-            'Do you really want to delete this item?', self.browser.contents)
-        self.assertIn('nuname', self.portal.objectIds())
+        self.browser.getLink("Delete").click()
+        self.assertIn("Do you really want to delete this item?", self.browser.contents)
+        self.assertIn("nuname", self.portal.objectIds())
         # Link breakabe page should be shown
-        self.assertIn('Potential link breakage', self.browser.contents)
-        self.assertIn('<a href="http://nohost/plone/nuname">Test Page 1</a>',
-                      self.browser.contents)
-        self.browser.getControl(name='form.buttons.Delete').click()
-        self.assertNotIn('doc2', self.portal.objectIds())
+        self.assertIn("Potential link breakage", self.browser.contents)
+        self.assertIn(
+            '<a href="http://nohost/plone/nuname">Test Page 1</a>',
+            self.browser.contents,
+        )
+        self.browser.getControl(name="form.buttons.Delete").click()
+        self.assertNotIn("doc2", self.portal.objectIds())
 
     def test_removal_in_subfolder(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
         folder1 = self.portal.folder1
 
         # This tests ensuring link integrity when removing an referenced
@@ -167,62 +177,66 @@
         # Then we try to delete the folder holding the referenced
         # document. Before we can do this we need to prevent the test
         # framework from choking on the exception we intentionally
         # throw.
         self.browser.handleErrors = True
 
         self.browser.open(
-            '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
                 folder1.absolute_url(), self._get_token(folder1)
             )
         )
-        self.assertIn('Potential link breakage', self.browser.contents)
-        self.assertIn('<a href="http://nohost/plone/doc1">Test Page 1</a>',
-                      self.browser.contents)
-        self.assertIn('<a href="http://nohost/plone/doc2">Test Page 2</a>',
-                      self.browser.contents)
-        self.browser.getControl(name='form.buttons.Delete').click()
-        self.assertNotIn('folder1', self.portal.objectIds())
+        self.assertIn("Potential link breakage", self.browser.contents)
+        self.assertIn(
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', self.browser.contents
+        )
+        self.assertIn(
+            '<a href="http://nohost/plone/doc2">Test Page 2</a>', self.browser.contents
+        )
+        self.browser.getControl(name="form.buttons.Delete").click()
+        self.assertNotIn("folder1", self.portal.objectIds())
 
     def test_removal_with_cookie_auth(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
 
         # This tests ensures link integrity working correctly without
         # http basic authentication (see the bug report in #6607).
         set_text(doc1, '<a href="doc2">doc2</a>')
         transaction.commit()
 
-        browser = Browser(self.layer['app'])
+        browser = Browser(self.layer["app"])
         browser.handleErrors = True
-        browser.addHeader('Referer', self.portal.absolute_url())
-        browser.open(
-            '{0:s}/folder_contents'.format(self.portal.absolute_url()))
+        browser.addHeader("Referer", self.portal.absolute_url())
+        browser.open(f"{self.portal.absolute_url():s}/folder_contents")
 
         # At this point we shouldn't be able to look at the folder
         # contents (as an anonymous user):
-        self.assertIn('login?came_from', browser.url)
+        self.assertIn("login?came_from", browser.url)
 
         # So we log in via the regular plone login form and additionally check
         # that there is no 'authorization' header set afterwards:
-        browser.getControl(name='__ac_name').value = TEST_USER_NAME
-        browser.getControl(name='__ac_password').value = TEST_USER_PASSWORD
-        browser.getControl('Log in').click()
-        self.assertNotIn(
-            'authorization', [h.lower() for h in browser.headers.keys()])
+        browser.getControl(name="__ac_name").value = TEST_USER_NAME
+        browser.getControl(name="__ac_password").value = TEST_USER_PASSWORD
+        browser.getControl("Log in").click()
+        self.assertNotIn("authorization", [h.lower() for h in browser.headers.keys()])
 
         # This should lead us back to the "folder contents" listing,
         # where we try to delete the referenced document.
-        browser.open('{0:s}/delete_confirmation?_authenticator={1:s}'.format(
-            doc2.absolute_url(), self._get_token(doc2)))
-        self.assertIn('Potential link breakage', browser.contents)
-        self.assertIn('<a href="http://nohost/plone/doc1">Test Page 1</a>',
-                      browser.contents)
-        browser.getControl(name='form.buttons.Delete').click()
-        self.assertNotIn('doc2', self.portal.objectIds())
+        browser.open(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
+                doc2.absolute_url(), self._get_token(doc2)
+            )
+        )
+        self.assertIn("Potential link breakage", browser.contents)
+        self.assertIn(
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', browser.contents
+        )
+        browser.getControl(name="form.buttons.Delete").click()
+        self.assertNotIn("doc2", self.portal.objectIds())
 
     def test_linkintegrity_on_off_switch(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
 
         # This tests switching link integrity checking on and off.
         set_text(doc1, '<a href="doc2">a document</a>')
@@ -231,30 +245,31 @@
         # This should lead us back to the "folder contents" listing,
         # where we try to delete the referenced document. Before we can
         # do this we need to prevent the test framework from choking on
         # the exception we intentionally throw.
         self.browser.handleErrors = True
 
         self.browser.open(
-            '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
                 doc2.absolute_url(), self._get_token(doc2)
             )
         )
-        self.assertIn('Potential link breakage', self.browser.contents)
-        self.assertIn('<a href="http://nohost/plone/doc1">Test Page 1</a>',
-                      self.browser.contents)
+        self.assertIn("Potential link breakage", self.browser.contents)
+        self.assertIn(
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', self.browser.contents
+        )
 
         # Now we turn the switch for link integrity checking off via the site
         # properties and try again:
         registry = getUtility(IRegistry)
-        settings = registry.forInterface(IEditingSchema, prefix='plone')
+        settings = registry.forInterface(IEditingSchema, prefix="plone")
         settings.enable_link_integrity_checks = False
         transaction.commit()
         self.browser.reload()
-        self.assertNotIn('Potential link breakage', self.browser.contents)
+        self.assertNotIn("Potential link breakage", self.browser.contents)
 
     def test_update(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
         doc4 = self.portal.folder1.doc4
 
         # This tests updating link integrity information for all site content,
@@ -271,108 +286,108 @@
         # these documents at this point:
         self.assertEqual([i.to_object for i in getOutgoingLinks(doc1)], [])
         self.assertEqual([i.to_object for i in getOutgoingLinks(doc2)], [])
 
         # An update of link integrity information for all content is triggered
         # by browsing a specific url:
         transaction.commit()
-        self.browser.open('{0:s}/updateLinkIntegrityInformation'.format(
-            self.portal.absolute_url()))
-        self.browser.getControl('Update').click()
-        self.assertIn('Link integrity information updated for',
-                      self.browser.contents)
+        self.browser.open(
+            f"{self.portal.absolute_url():s}/updateLinkIntegrityInformation"
+        )
+        self.browser.getControl("Update").click()
+        self.assertIn("Link integrity information updated for", self.browser.contents)
 
         # Now the linking documents should hold the correct link integrity
         # references:
         self.assertEqual(
             [i.to_object for i in getOutgoingLinks(doc1)],
-            [doc2, ],
+            [
+                doc2,
+            ],
         )
         self.assertEqual(
             [i.to_object for i in getOutgoingLinks(doc2)],
-            [doc4, ],
+            [
+                doc4,
+            ],
         )
 
     def test_references_on_cloned_objects(self):
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
 
         # This tests ensures that link integrity is correctly setup when
         # cloning an object.
         set_text(doc1, '<a href="doc2">a document</a>')
 
         # Next we clone the document:
         token = self._get_token(doc1)
-        self.request['_authenticator'] = token
-        doc1.restrictedTraverse('object_copy')()
+        self.request["_authenticator"] = token
+        doc1.restrictedTraverse("object_copy")()
 
-        self.request['_authenticator'] = token
-        self.portal.restrictedTraverse('object_paste')()
-        self.assertIn('copy_of_doc1', self.portal)
+        self.request["_authenticator"] = token
+        self.portal.restrictedTraverse("object_paste")()
+        self.assertIn("copy_of_doc1", self.portal)
         transaction.commit()
 
         # Then we try to delete the document linked by the original document
         # and its clone. Before we can do this we need to prevent the test
         # framework from choking on the exception we intentionally throw.
         self.browser.handleErrors = True
 
         # Now we can continue and "click" the "delete" action. The confirmation
         # page should list both documents:
         self.browser.open(
-            '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
                 doc2.absolute_url(), self._get_token(doc2)
             )
         )
+        self.assertIn("is referenced by the following items:", self.browser.contents)
+        self.assertIn("Potential link breakage", self.browser.contents)
         self.assertIn(
-            'is referenced by the following items:', self.browser.contents)
-        self.assertIn('Potential link breakage', self.browser.contents)
-        self.assertIn(
-            '<a href="http://nohost/plone/doc1">Test Page 1</a>',
-            self.browser.contents
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', self.browser.contents
         )
         self.assertIn(
-            '<a href="http://nohost/plone/copy_of_doc1"',
-            self.browser.contents
+            '<a href="http://nohost/plone/copy_of_doc1"', self.browser.contents
         )
 
     def test_files_with_spaces_removal(self):
         doc1 = self.portal.doc1
 
         # This tests the behaviour when removing a referenced file that has
         # spaces in its id.  First we need to rename the existing file:
         self.portal.invokeFactory(
-            'Document', id='some spaces.doc', title='A spaces doc')
+            "Document", id="some spaces.doc", title="A spaces doc"
+        )
 
-        self.assertIn('some spaces.doc', self.portal.objectIds())
-        spaces1 = self.portal['some spaces.doc']
+        self.assertIn("some spaces.doc", self.portal.objectIds())
+        spaces1 = self.portal["some spaces.doc"]
 
         set_text(doc1, '<a href="some spaces.doc">a document</a>')
 
         # The document should now have a reference to the file:
-        self.assertEqual(
-            [i.to_object for i in getOutgoingLinks(doc1)], [spaces1])
+        self.assertEqual([i.to_object for i in getOutgoingLinks(doc1)], [spaces1])
         transaction.commit()
 
         # Then we use a browser to try to delete the referenced file.
         # Before we can do this we need to prevent the test framework
         # from choking on the exception we intentionally throw.
         self.browser.handleErrors = True
 
         self.browser.open(
-            '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
                 spaces1.absolute_url(), self._get_token(spaces1)
             )
         )
-        self.assertIn('Potential link breakage', self.browser.contents)
+        self.assertIn("Potential link breakage", self.browser.contents)
         self.assertIn(
-            '<a href="http://nohost/plone/doc1">Test Page 1</a>',
-            self.browser.contents
+            '<a href="http://nohost/plone/doc1">Test Page 1</a>', self.browser.contents
         )
-        self.browser.getControl(name='form.buttons.Delete').click()
-        self.assertNotIn('some spaces.doc', self.portal.objectIds())
+        self.browser.getControl(name="form.buttons.Delete").click()
+        self.assertNotIn("some spaces.doc", self.portal.objectIds())
 
     def test_removal_via_zmi(self):
         """Delete via ZMI is no longer protedted!"""
         doc1 = self.portal.doc1
         doc2 = self.portal.doc2
 
         # This tests ensuring link integrity when removing an object via
@@ -382,26 +397,26 @@
 
         transaction.commit()
         # Then we use a browser to try to delete the referenced
         # document. Before we can do this we need to prevent the test
         # framework from choking on the exception we intentionally throw.
         self.browser.handleErrors = True
 
-        self.browser.open('http://nohost/plone/manage_main')
-        self.browser\
-            .getControl(name='ids:list')\
-            .getControl(value='doc2').selected = True
+        self.browser.open("http://nohost/plone/manage_main")
+        self.browser.getControl(name="ids:list").getControl(
+            value="doc2"
+        ).selected = True
 
-        self.browser.getControl('Delete').click()
-        self.assertNotIn('doc2', self.portal.objectIds())
+        self.browser.getControl("Delete").click()
+        self.assertNotIn("doc2", self.portal.objectIds())
 
     def test_warn_about_content(self):
         folder1 = self.portal.folder1
         self.browser.open(
-            '{0:s}/delete_confirmation?_authenticator={1:s}'.format(
+            "{:s}/delete_confirmation?_authenticator={:s}".format(
                 folder1.absolute_url(), self._get_token(folder1)
             )
         )
-        self.assertIn('Number of selected', self.browser.contents)
-        self.assertIn('2 Objects in all', self.browser.contents)
-        self.assertIn('1 Folders', self.browser.contents)
-        self.assertIn('0 Published objects', self.browser.contents)
+        self.assertIn("Number of selected", self.browser.contents)
+        self.assertTrue(re.search(r"2\s+Objects in all", self.browser.contents))
+        self.assertTrue(re.search(r"1\s+Folders", self.browser.contents))
+        self.assertTrue(re.search(r"0\s+Published objects", self.browser.contents))
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_handlers.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_handlers.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,52 +3,52 @@
 from plone.app.linkintegrity.testing import create
 from plone.app.testing import logout
 
 import unittest
 
 
 class ReferenceGenerationTestCase(unittest.TestCase):
-    """ testing the handlers.findObject function """
+    """testing the handlers.findObject function"""
 
     layer = testing.PLONE_APP_LINKINTEGRITY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
 
     def test_relative_to_portal_root_1(self):
-        obj, components = findObject(self.portal.doc1, '/plone/doc2')
-        self.assertEqual(obj.absolute_url_path(), '/plone/doc2')
-        self.assertEqual(components, '')
+        obj, components = findObject(self.portal.doc1, "/plone/doc2")
+        self.assertEqual(obj.absolute_url_path(), "/plone/doc2")
+        self.assertEqual(components, "")
 
     def test_relative_to_portal_root_2(self):
         # Prevent regression.
         # See https://github.com/plone/plone.app.linkintegrity/pull/17
-        obj, components = findObject(self.portal.doc1, '/doc2')
-        self.assertEqual(obj.absolute_url_path(), '/plone/doc2')
-        self.assertEqual(components, '')
+        obj, components = findObject(self.portal.doc1, "/doc2")
+        self.assertEqual(obj.absolute_url_path(), "/plone/doc2")
+        self.assertEqual(components, "")
 
     def test_webserver_rewrites_portal_name(self):
         # test the case where a webserver rewrites the portal name,
         # e.g. for Apache:
         # RewriteRule ^/wssitename(.*)$ http://localhost:8080/VirtualHostBase/http/my.domain.com:80/plonesitename/VirtualHostRoot/_vh_wssitename$1  # noqa
-        self.portal.REQUEST.other['VirtualRootPhysicalPath'] = ('', 'plone')
-        self.portal.REQUEST._script = ['plone_foo']
-        obj, components = findObject(self.portal.doc1, '/plone_foo/doc2')
-        self.assertEqual(obj.absolute_url_path(), '/plone_foo/doc2')
-        self.assertEqual(obj.getPhysicalPath(), ('', 'plone', 'doc2'))
-        self.assertEqual(components, '')
+        self.portal.REQUEST.other["VirtualRootPhysicalPath"] = ("", "plone")
+        self.portal.REQUEST._script = ["plone_foo"]
+        obj, components = findObject(self.portal.doc1, "/plone_foo/doc2")
+        self.assertEqual(obj.absolute_url_path(), "/plone_foo/doc2")
+        self.assertEqual(obj.getPhysicalPath(), ("", "plone", "doc2"))
+        self.assertEqual(components, "")
 
     def test_uuid_link(self):
         # Test that objects can be found from uuid links.
-        create(self.portal, 'Document', id='target', title='Target')
+        create(self.portal, "Document", id="target", title="Target")
         target = self.portal.target
         target_uid = target.UID()
-        path = "../resolveuid/{}".format(target_uid)
+        path = f"../resolveuid/{target_uid}"
 
         # We logout.  This is to check that findObject also finds objects
         # that are not visible to the current user, like a private page.
         # See https://github.com/plone/plone.app.linkintegrity/issues/79
         logout()
 
         obj, components = findObject(self.portal.doc1, path)
-        self.assertEqual(obj.absolute_url_path(), '/plone/target')
+        self.assertEqual(obj.absolute_url_path(), "/plone/target")
         self.assertEqual(components, path)
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_imagescales.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_imagescales.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,61 +9,69 @@
 
 class ImageReferenceTestCase(unittest.TestCase):
     """image reference testcase"""
 
     layer = testing.PLONE_APP_LINKINTEGRITY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
 
     def test_image_tag_reference_creation(self):
         doc1 = self.portal.doc1
         img1 = self.portal.image1
 
         # This tests the correct creation of references used for
         # ensuring link integrity. Any archetype-based content object
         # which refers to other (local) objects by `<img>` or `<a>` tags
         # should create references between those objects on save.
-        set_text(doc1, img1.restrictedTraverse('@@images').tag())
+        set_text(doc1, img1.restrictedTraverse("@@images").tag())
 
         self.assertEqual(
             [r.to_object for r in getOutgoingLinks(doc1)],
-            [img1, ],
+            [
+                img1,
+            ],
         )
         self.assertEqual([r.to_object for r in getIncomingLinks(doc1)], [])
         self.assertEqual([r.to_object for r in getOutgoingLinks(img1)], [])
         self.assertEqual(
             [r.from_object for r in getIncomingLinks(img1)],
             [doc1],
         )
 
     def test_image_scale_reference_creation(self):
         doc1 = self.portal.doc1
         img1 = self.portal.image1
 
         # Linking image scales should also work:
-        set_text(
-            doc1, '<a href="image1/@@images/image_thumb">an image</a>')
+        set_text(doc1, '<a href="image1/@@images/image_thumb">an image</a>')
         self.assertEqual(
             [r.to_object for r in getOutgoingLinks(doc1)],
-            [img1, ],
+            [
+                img1,
+            ],
         )
         self.assertEqual(
             [r.from_object for r in getIncomingLinks(img1)],
-            [doc1, ],
+            [
+                doc1,
+            ],
         )
 
     def test_image_resolveuid_reference_creation(self):
         doc1 = self.portal.doc1
         img1 = self.portal.image1
 
         # Linking via the "resolveuid/UID" method should also work:
-        set_text(doc1, '<a href="resolveuid/{0:s}">an image</a>'.format(
-            IUUID(img1)))
+        set_text(doc1, f'<a href="resolveuid/{IUUID(img1):s}">an image</a>')
         self.assertEqual(
             [r.to_object for r in getOutgoingLinks(doc1)],
-            [img1, ],
+            [
+                img1,
+            ],
         )
         self.assertEqual(
             [r.from_object for r in getIncomingLinks(img1)],
-            [doc1, ],
+            [
+                doc1,
+            ],
         )
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/tests/test_references.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/tests/test_references.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,74 +9,75 @@
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import TEST_USER_NAME
 from z3c.relationfield import RelationValue
 from z3c.relationfield.event import _setRelation
 from zc.relation.interfaces import ICatalog
 from zope.component import getUtility
-from zope.lifecycleevent import modified
 from zope.intid.interfaces import IIntIds
+from zope.lifecycleevent import modified
 
 import unittest
 
 
 class ReferenceGenerationTestCase(unittest.TestCase):
     """reference generation testcase"""
 
     layer = testing.PLONE_APP_LINKINTEGRITY_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
 
     def _set_related_items(self, obj, items):
         assert IRelatedItems.providedBy(obj)
-        setattr(obj, 'relatedItems', items)
+        setattr(obj, "relatedItems", items)
         modified(obj)
 
     def _get_related_items(self, obj):
         return obj.relatedItems
 
     def test_is_linked(self):
-        img1 = self.portal['image1']
-        doc1 = self.portal['doc1']
+        img1 = self.portal["image1"]
+        doc1 = self.portal["doc1"]
         set_text(doc1, '<img src="image1"></img>')
         self.assertTrue(hasIncomingLinks(img1))
 
     def test_referal_to_private_files(self):
         # This tests the behaviour of the link integrity code when a to
         # be deleted item is referred to by some page the current user
         # has no permission to view. In this case the privacy of the
         # linking user should be protected, so neither the name or url
         # of the linking page should be shown. First we need to create
         # the link in question and set up the permissions accordingly.
         doc = self.portal.doc1
         img = self.portal.image1
         set_text(doc, '<a href="image1">Image 1</a>')
 
-        roles = ('Member', )
-        self.portal.manage_permission('List folder contents', roles=roles)
-        self.portal.manage_permission('Delete objects', roles=roles)
-        doc.manage_permission('View', roles=('Manager',), acquire=0)
-        doc.manage_permission('Access contents information',
-                              roles=('Manager', ), acquire=0)
+        roles = ("Member",)
+        self.portal.manage_permission("List folder contents", roles=roles)
+        self.portal.manage_permission("Delete objects", roles=roles)
+        doc.manage_permission("View", roles=("Manager",), acquire=0)
+        doc.manage_permission(
+            "Access contents information", roles=("Manager",), acquire=0
+        )
 
         logout()
-        login(self.portal, 'member')
+        login(self.portal, "member")
         checkPermission = self.portal.portal_membership.checkPermission
-        self.assertFalse(checkPermission('View', doc))
-        self.assertFalse(checkPermission('Access contents information', doc))
-        self.assertTrue(checkPermission('View', img))
-        self.assertTrue(checkPermission('Access contents information', img))
+        self.assertFalse(checkPermission("View", doc))
+        self.assertFalse(checkPermission("Access contents information", doc))
+        self.assertTrue(checkPermission("View", img))
+        self.assertTrue(checkPermission("Access contents information", img))
 
         # The warning is shown.
         self.assertTrue(hasOutgoingLinks(doc))
-        view = img.restrictedTraverse('delete_confirmation')
+        view = img.restrictedTraverse("delete_confirmation")
         results = view()
-        self.assertIn('Potential link breakage', results)
-        self.assertIn('The item is not accessible.', results)
+        self.assertIn("Potential link breakage", results)
+        self.assertIn("The item is not accessible.", results)
 
         # delete linked item and check if the source still has the relation
 
         # TODO: There is a permission-problem. Deleting the relation
         # When deleting the linked obj the relation is deleted by
         # z3c.relationfield.event.breakRelations. That also fires
         # ObjectModifiedEvent on the linked obj even though the user might not
@@ -93,129 +94,141 @@
         modified(doc)
         self.assertFalse(hasOutgoingLinks(doc))
         # doc now has a broken link and no relation :-(
 
     def test_link_extraction_easy(self):
         doc1 = self.portal.doc1
         set_text(doc1, '<a href="doc2">Doc 2</a>')
-        self.assertEqual(
-            extractLinks(doc1.text.raw),
-            ('doc2', )
-        )
+        self.assertEqual(extractLinks(doc1.text.raw), ("doc2",))
 
     def test_link_extraction_more_complex(self):
         doc2 = self.portal.doc2
         set_text(
             doc2,
-            '<a href="doc1">Doc 2</a>' +
-            '<a href="folder1/doc3"><img src="image1" /></a>',
+            '<a href="doc1">Doc 2</a>'
+            + '<a href="folder1/doc3"><img src="image1" /></a>',
         )
         self.assertEqual(
-            extractLinks(doc2.text.raw),
-            ('doc1',
-             'folder1/doc3',
-             'image1')
+            extractLinks(doc2.text.raw), ("doc1", "folder1/doc3", "image1")
         )
 
     def test_broken_references(self):
         # create a temporary document to test with
-        doc1a = testing.create(self.portal, 'Document', id='doc1a')
+        doc1a = testing.create(self.portal, "Document", id="doc1a")
         doc1 = self.portal.doc1
 
         self.assertEqual(len(list(getOutgoingLinks(doc1))), 0)
         set_text(doc1, '<a href="doc1a">Doc 1a</a>')
         self.assertEqual(len(list(getOutgoingLinks(doc1))), 1)
-        self.assertEqual([link.to_object for link in getOutgoingLinks(doc1)],
-                         [self.portal.doc1a])
+        self.assertEqual(
+            [link.to_object for link in getOutgoingLinks(doc1)], [self.portal.doc1a]
+        )
 
         # Now delete the target item, suppress events and test again,
         # The reference should be a ghost not in any folder anymore.
-        # check if it has no acquition parent!
+        # check if it has no acquisition parent!
         self.portal._delObject(doc1a.id, suppress_events=True)
         objs = [link.to_object for link in getOutgoingLinks(doc1)]
         self.assertEqual(len(objs), 1)
         obj = objs[0]
         if obj is not None:
             # Plone with fixed five.intid
             # if object is None: all fine as well.
-            self.assertEqual(obj.portal_type, 'Document')
+            self.assertEqual(obj.portal_type, "Document")
             _marker = dict()
-            self.assertEqual(getattr(obj, 'aq_parent', _marker), _marker)
+            self.assertEqual(getattr(obj, "aq_parent", _marker), _marker)
 
     def test_relative_upwards_link_generates_matching_reference(self):
         doc1 = self.portal.doc1
         doc3 = self.portal.folder1.doc3
         set_text(doc3, '<a href="../doc1">go!</a>')
         self.assertEqual(len(list(getOutgoingLinks(doc1))), 0)
-        self.assertEqual([link.to_object for link in getOutgoingLinks(doc3)],
-                         [doc1])
+        self.assertEqual([link.to_object for link in getOutgoingLinks(doc3)], [doc1])
 
     def test_unicode_links(self):
         doc1 = self.portal.doc1
 
         # This tests checks that hasIncomingLinks can now be used safely as it
         # eventually plays well with transaction machinery.
         # Add bad link, should not raise exception and there should not
         # be any references added.
-        set_text(
-            doc1,
-            '<a href="ö?foo=bar&baz=bam">bug</a>')
+        set_text(doc1, '<a href="ö?foo=bar&baz=bam">bug</a>')
 
         self.assertEqual([link for link in getOutgoingLinks(doc1)], [])
 
     def test_reference_orthogonality(self):
         doc = self.portal.doc1
         img = self.portal.image1
-        tag = img.restrictedTraverse('@@images').tag()
+        tag = img.restrictedTraverse("@@images").tag()
 
         # This tests the behavior when other references already exist.
         self.assertEqual([link for link in getOutgoingLinks(doc)], [])
         self.assertEqual([link for link in getIncomingLinks(doc)], [])
         self.assertEqual([link for link in getOutgoingLinks(img)], [])
         self.assertEqual([link for link in getOutgoingLinks(img)], [])
 
         # Then establish a reference between the document and image as
         # a related item:
-        self._set_related_items(doc, [img, ])
-        self.assertEqual(self._get_related_items(doc), [img, ])
+        self._set_related_items(
+            doc,
+            [
+                img,
+            ],
+        )
+        self.assertEqual(
+            self._get_related_items(doc),
+            [
+                img,
+            ],
+        )
 
         # Next edit the document body and insert a link to the image,
         # which should trigger the creation of a link integrity reference:
         set_text(doc, tag)
 
         self.assertEqual([link.to_object for link in getOutgoingLinks(doc)], [img])
 
         # And the related item reference remains in place:
-        self.assertEqual(self._get_related_items(doc), [img, ])
+        self.assertEqual(
+            self._get_related_items(doc),
+            [
+                img,
+            ],
+        )
 
         # Finally, edit the document body again, this time removing the
         # link to the image, which should trigger the removal of the
         # link integrity reference:
-        set_text(doc, 'where did my link go?')
+        set_text(doc, "where did my link go?")
         self.assertEqual([link.to_object for link in getOutgoingLinks(doc)], [])
 
         # And again the related item reference remains in place:
-        self.assertEqual(self._get_related_items(doc), [img, ])
+        self.assertEqual(
+            self._get_related_items(doc),
+            [
+                img,
+            ],
+        )
 
     def test_delete_confirmation_for_any_reference(self):
         """Test, if delete confirmation shows also a warning if items are
         deleted, which are referenced by other items via a reference field.
         """
-        img1 = self.portal['image1']
-        doc1 = self.portal['doc1']
+        img1 = self.portal["image1"]
+        doc1 = self.portal["doc1"]
 
         intids_tool = getUtility(IIntIds)
         to_id = intids_tool.getId(img1)
         rel = RelationValue(to_id)
-        _setRelation(doc1, 'related_image', rel)
+        _setRelation(doc1, "related_image", rel)
 
         # Test, if relation is present in the relation catalog
         catalog = getUtility(ICatalog)
-        rels = list(catalog.findRelations({'to_id': to_id}))
+        rels = list(catalog.findRelations({"to_id": to_id}))
         self.assertEqual(len(rels), 1)
 
         # Test, if delete_confirmation_info shows also other relations than
         # ``isReferencing``.
-        info = img1.restrictedTraverse('@@delete_confirmation_info')
+        info = img1.restrictedTraverse("@@delete_confirmation_info")
         breaches = info.get_breaches()
         self.assertEqual(len(breaches), 1)
-        self.assertEqual(len(info.get_breaches()[0]['sources']), 1)
+        self.assertEqual(len(info.get_breaches()[0]["sources"]), 1)
```

### Comparing `plone.app.linkintegrity-4.0.0/plone/app/linkintegrity/utils.py` & `plone.app.linkintegrity-4.0.1/plone/app/linkintegrity/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-# -*- coding: utf-8 -*-
-from plone.registry.interfaces import IRegistry
 from plone.base.interfaces import IEditingSchema
+from plone.registry.interfaces import IRegistry
 from zc.relation.interfaces import ICatalog
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 from zope.keyreference.interfaces import NotYet
 
-referencedRelationship = 'isReferencing'
+
+referencedRelationship = "isReferencing"
 
 
-def getIncomingLinks(
-    obj=None,
-    intid=None,
-    from_attribute=referencedRelationship
-):
+def getIncomingLinks(obj=None, intid=None, from_attribute=referencedRelationship):
     """Return a generator of incoming relations created using
     plone.app.linkintegrity (Links in Richtext-Fields).
     """
     catalog = getUtility(ICatalog)
     intid = intid if intid is not None else getUtility(IIntIds).getId(obj)
-    query = {'to_id': intid}
+    query = {"to_id": intid}
     if from_attribute:
-        query['from_attribute'] = from_attribute
+        query["from_attribute"] = from_attribute
     return catalog.findRelations(query)
 
 
 def hasIncomingLinks(obj=None, intid=None):
     """Test if an object is linked to by other objects using
     plone.app.linkintegrity (Links in Richtext-Fields).
 
     Way to give bool without loading generator into list.
     """
     for it in getIncomingLinks(obj=obj, intid=intid):
         return True
     return False
 
 
-def getOutgoingLinks(
-    obj=None,
-    intid=None,
-    from_attribute=referencedRelationship
-):
+def getOutgoingLinks(obj=None, intid=None, from_attribute=referencedRelationship):
     """Return a generator of outgoing relations created using
     plone.app.linkintegrity (Links in Richtext-Fields).
     """
     catalog = getUtility(ICatalog)
     intid = intid if intid is not None else getUtility(IIntIds).getId(obj)
-    query = {'from_id': intid}
+    query = {"from_id": intid}
     if from_attribute:
-        query['from_attribute'] = from_attribute
+        query["from_attribute"] = from_attribute
     return catalog.findRelations(query)
 
 
 def hasOutgoingLinks(obj=None, intid=None):
     """Test if an object links to other objects using plone.app.linkintegrity
     (Links in Richtext-Fields).
     """
     for it in getOutgoingLinks(obj=obj, intid=intid):
         return True
     return False
 
 
 def linkintegrity_enabled():
     reg = getUtility(IRegistry)
-    editing_settings = reg.forInterface(IEditingSchema, prefix='plone')
+    editing_settings = reg.forInterface(IEditingSchema, prefix="plone")
     return editing_settings.enable_link_integrity_checks
 
 
 def ensure_intid(obj, intids=None):
     if intids is None:
         intids = getUtility(IIntIds)
     try:
```

### Comparing `plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/PKG-INFO` & `plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.0
+Version: 4.0.1
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -90,15 +90,15 @@
 interface for your contenttype. Look at the ``retriever`` module in this
 package for examples.
 
 API
 ---
 
 To check if there would be breaches when deleting one or more objects
-you can use the follwing code:
+you can use the following code:
 
 .. code-block:: python
 
     from plone import api
     portal = api.portal.get()
     view = api.content.get_view(
         'delete_confirmation_info',
@@ -146,14 +146,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 4.0.0 (2023-03-13)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility for Plone 5.2.  Support Plone 6 only.
@@ -676,15 +686,15 @@
   [davisagli]
 
 - Use the `get` method to retrieve the field value if the instance
   does not provide an accessor method. This is the case for instance
   for fields which have been added via schema extension.
   [malthe]
 
-- Support resolveuid/UID references explicitely, by parsing and resolving
+- Support resolveuid/UID references explicitly, by parsing and resolving
   these ourselves instead of relying on a view or script (which doesn't work).
   This fixes linkintegrity for sites with link-by-uid turned on.
   This closes https://dev.plone.org/ticket/12104
   [mj]
 
 1.4.4 - 2011-10-04
 ------------------
```

### Comparing `plone.app.linkintegrity-4.0.0/plone.app.linkintegrity.egg-info/SOURCES.txt` & `plone.app.linkintegrity-4.0.1/plone.app.linkintegrity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.0/setup.py` & `plone.app.linkintegrity-4.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '4.0.0'
+version = "4.0.1"
 
 setup(
-    name='plone.app.linkintegrity',
+    name="plone.app.linkintegrity",
     version=version,
-    description='Manage link integrity in Plone.',
-    long_description='\n\n'.join([
-        open("README.rst").read(),
-        open('CHANGES.rst').read(),
-    ]),
+    description="Manage link integrity in Plone.",
+    long_description="\n\n".join(
+        [
+            open("README.rst").read(),
+            open("CHANGES.rst").read(),
+        ]
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
@@ -27,37 +28,47 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking",
     ],
-    keywords='link integrity plone',
-    author='Plone Foundation',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://github.com/plone/plone.app.linkintegrity',
-    license='GPL version 2',
+    keywords="link integrity plone",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://github.com/plone/plone.app.linkintegrity",
+    license="GPL version 2",
     packages=find_packages(),
-    namespace_packages=['plone', 'plone.app'],
+    namespace_packages=["plone", "plone.app"],
     include_package_data=True,
-    python_requires='>=3.8',
+    python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'plone.app.intid',
-        'plone.app.relationfield',
-        'plone.base',
-        'plone.dexterity',
+        "setuptools",
+        "plone.app.intid",
+        "plone.app.relationfield",
+        "plone.base",
+        "plone.dexterity",
+        "Products.GenericSetup",
+        "Products.statusmessages",
+        "plone.app.textfield",
+        "plone.app.uuid",
+        "plone.registry",
+        "plone.uuid",
+        "z3c.relationfield",
+        "zc.relation",
+        "zope.intid",
+        "zope.keyreference",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
-            'plone.app.contenttypes',
-            'plone.app.dexterity [relations]',  # related items in dx 2.0
+        "test": [
+            "plone.app.testing",
+            "plone.namedfile",
+            "plone.testing",
         ],
     },
-    platforms='Any',
+    platforms="Any",
     zip_safe=False,
-    entry_points='''
+    entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
-    ''',
+    """,
 )
```

