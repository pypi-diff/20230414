# Comparing `tmp/plone.outputfilters-5.0.1.tar.gz` & `tmp/plone.outputfilters-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.outputfilters-5.0.1.tar", last modified: Tue Mar 21 22:55:15 2023, max compression
+gzip compressed data, was "plone.outputfilters-5.0.2.tar", last modified: Thu Apr 13 23:39:56 2023, max compression
```

## Comparing `plone.outputfilters-5.0.1.tar` & `plone.outputfilters-5.0.2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.585584 plone.outputfilters-5.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     8659 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    16106 2023-03-21 22:55:15.585725 plone.outputfilters-5.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3829 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.572917 plone.outputfilters-5.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      736 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.573199 plone.outputfilters-5.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.578172 plone.outputfilters-5.0.1/plone/outputfilters/
--rw-r--r--   0 maurits    (501) staff       (20)     2753 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.579807 plone.outputfilters-5.0.1/plone/outputfilters/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      240 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/browser/captioned_image.pt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/browser/captioned_image.py
--rw-r--r--   0 maurits    (501) staff       (20)      472 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2266 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/browser/resolveuid.py
--rw-r--r--   0 maurits    (501) staff       (20)      788 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.581522 plone.outputfilters-5.0.1/plone/outputfilters/filters/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/filters/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      865 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/filters/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      373 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/filters/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/filters/picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/filters/resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)      744 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/mimetype.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.569267 plone.outputfilters-5.0.1/plone/outputfilters/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.581941 plone.outputfilters-5.0.1/plone/outputfilters/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/profiles/default/plone.outputfilters.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.584550 plone.outputfilters-5.0.1/plone/outputfilters/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     2772 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/README_py2.rst
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/test_apply_filters.py
--rw-r--r--   0 maurits    (501) staff       (20)      787 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/test_picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    26899 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/test_resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/tests/test_transforms.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.585374 plone.outputfilters-5.0.1/plone/outputfilters/transforms/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/transforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:55:15.575788 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    16106 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      325 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:55:15.000000 plone.outputfilters-5.0.1/plone.outputfilters.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1760 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-03-21 22:55:15.586215 plone.outputfilters-5.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-03-21 22:55:14.000000 plone.outputfilters-5.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.098176 plone.outputfilters-5.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     8768 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    16041 2023-04-13 23:39:56.098310 plone.outputfilters-5.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.086078 plone.outputfilters-5.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.086334 plone.outputfilters-5.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.091596 plone.outputfilters-5.0.2/plone/outputfilters/
+-rw-r--r--   0 maurits    (501) staff       (20)     2752 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      252 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.093166 plone.outputfilters-5.0.2/plone/outputfilters/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/captioned_image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/captioned_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)      472 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2267 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/resolveuid.py
+-rw-r--r--   0 maurits    (501) staff       (20)      788 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.094547 plone.outputfilters-5.0.2/plone/outputfilters/filters/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      373 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1721 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)      744 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/mimetype.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.082955 plone.outputfilters-5.0.2/plone/outputfilters/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.094963 plone.outputfilters-5.0.2/plone/outputfilters/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/profiles/default/plone.outputfilters.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.097051 plone.outputfilters-5.0.2/plone/outputfilters/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_apply_filters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      787 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    27220 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_transforms.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.097948 plone.outputfilters-5.0.2/plone/outputfilters/transforms/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.089336 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    16041 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-04-13 23:39:56.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      325 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1717 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:39:56.098760 plone.outputfilters-5.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/setup.py
```

### Comparing `plone.outputfilters-5.0.1/CHANGES.rst` & `plone.outputfilters-5.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (535edb14)
+
+
 5.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.1/PKG-INFO` & `plone.outputfilters-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.1
+Version: 5.0.2
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,18 +26,16 @@
 ``plone.outputfilters`` provides a framework for registering filters that
 get applied to text as it is rendered.
 
 By default, these filters are wired up to occur when text is transformed from
 the text/html mimetype to the text/x-html-safe mimetype via the
 PortalTransforms machinery.
 
-With both Archetypes TextFields and the RichText field of
-``plone.app.textfield``, this transform is typically applied when the field
-value is first accessed. The result of the transform is then cached in a
-volatile attribute for an hour or until the value is replaced.
+With  the RichText field of ``plone.app.textfield``, this transform is typically applied when the field value is first accessed.
+The result of the transform is then cached in a volatile attribute for an hour or until the value is replaced.
 
 
 Included Filters
 ================
 
 A default filter is included which provides the following features:
 
@@ -63,17 +61,15 @@
 
 Such URLs can be resolved by the ``resolveuid`` view, which resolves the UID to
 an object and then redirects to its URL. However, resolving links in this way
 requires an extra request after the redirect. The resolveuid filter avoids that
 by replacing such URLs with the object's actual full absolute URL as the link
 is rendered.
 
-UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``, with a fallback to
-the Archetypes UID catalog for backwards compatibility. LinguaPlone translations
-are supported when LinguaPlone is present.
+UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``.
 
 The resolveuid filter is enabled if there is at least one
 ``plone.outputfilters.filters.resolveuid_and_caption.IResolveUidsEnabler``
 utility whose ``available`` property returns ``True``.  This mechanism exists
 for compatibility with TinyMCE and kupu, which both provide their own control
 panel setting to enable the link-by-uid feature.
 
@@ -140,19 +136,19 @@
 A filter is a callable which accepts a UTF-8-encoded HTML string as input, and
 returns a modified UTF-8-encoded HTML string. A return value of ``None`` may be
 used to indicate that the input should not be modified.
 
 Example::
 
     import re
-    from zope.interface import implements
+    from zope.interface import implementer
     from plone.outputfilters.interfaces import IFilter
 
+    @implementer(IFilter)
     class EmDashAdder(object):
-        implements(IFilter)
         order = 1000
 
         def __init__(self, context, request):
             pass
 
         def is_enabled(self):
             return True
@@ -222,14 +218,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (535edb14)
+
+
 5.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.1/README.rst` & `plone.outputfilters-5.0.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 ``plone.outputfilters`` provides a framework for registering filters that
 get applied to text as it is rendered.
 
 By default, these filters are wired up to occur when text is transformed from
 the text/html mimetype to the text/x-html-safe mimetype via the
 PortalTransforms machinery.
 
-With both Archetypes TextFields and the RichText field of
-``plone.app.textfield``, this transform is typically applied when the field
-value is first accessed. The result of the transform is then cached in a
-volatile attribute for an hour or until the value is replaced.
+With  the RichText field of ``plone.app.textfield``, this transform is typically applied when the field value is first accessed.
+The result of the transform is then cached in a volatile attribute for an hour or until the value is replaced.
 
 
 Included Filters
 ================
 
 A default filter is included which provides the following features:
 
@@ -41,17 +39,15 @@
 
 Such URLs can be resolved by the ``resolveuid`` view, which resolves the UID to
 an object and then redirects to its URL. However, resolving links in this way
 requires an extra request after the redirect. The resolveuid filter avoids that
 by replacing such URLs with the object's actual full absolute URL as the link
 is rendered.
 
-UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``, with a fallback to
-the Archetypes UID catalog for backwards compatibility. LinguaPlone translations
-are supported when LinguaPlone is present.
+UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``.
 
 The resolveuid filter is enabled if there is at least one
 ``plone.outputfilters.filters.resolveuid_and_caption.IResolveUidsEnabler``
 utility whose ``available`` property returns ``True``.  This mechanism exists
 for compatibility with TinyMCE and kupu, which both provide their own control
 panel setting to enable the link-by-uid feature.
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
 Introduction ============ ``plone.outputfilters`` provides a framework for
 registering filters that get applied to text as it is rendered. By default,
 these filters are wired up to occur when text is transformed from the text/html
 mimetype to the text/x-html-safe mimetype via the PortalTransforms machinery.
-With both Archetypes TextFields and the RichText field of
-``plone.app.textfield``, this transform is typically applied when the field
-value is first accessed. The result of the transform is then cached in a
-volatile attribute for an hour or until the value is replaced. Included Filters
-================ A default filter is included which provides the following
-features: * Resolving UID-based links * Adding captions to images (These are
-implemented as one filter to avoid the overhead of parsing the HTML twice.)
-These features used to be provided by similar transforms in both Products.kupu
-and Products.TinyMCE. New releases of these editors are being prepared which
-depend on the transform in plone.outputfilters, so that bugs don't need to be
-fixed in multiple places. Resolving UID-based links ------------------------
-- Internal links may be inserted with a UID reference rather than the real path
-of the item being linked. For example, a link might look like this::
+With the RichText field of ``plone.app.textfield``, this transform is typically
+applied when the field value is first accessed. The result of the transform is
+then cached in a volatile attribute for an hour or until the value is replaced.
+Included Filters ================ A default filter is included which provides
+the following features: * Resolving UID-based links * Adding captions to images
+(These are implemented as one filter to avoid the overhead of parsing the HTML
+twice.) These features used to be provided by similar transforms in both
+Products.kupu and Products.TinyMCE. New releases of these editors are being
+prepared which depend on the transform in plone.outputfilters, so that bugs
+don't need to be fixed in multiple places. Resolving UID-based links ----------
+--------------- Internal links may be inserted with a UID reference rather than
+the real path of the item being linked. For example, a link might look like
+this::
 Such_URLs_can_be_resolved_by_the_``resolveuid``_view,_which_resolves_the_UID_to
 an_object_and_then_redirects_to_its_URL._However,_resolving_links_in_this_way
 requires_an_extra_request_after_the_redirect._The_resolveuid_filter_avoids_that
 by_replacing_such_URLs_with_the_object's_actual_full_absolute_URL_as_the_link
-is_rendered._UIDs_are_resolved_using_``plone.app.uuid.utils.uuidToURL``,_with_a
-fallback_to_the_Archetypes_UID_catalog_for_backwards_compatibility._LinguaPlone
-translations_are_supported_when_LinguaPlone_is_present._The_resolveuid_filter
-is_enabled_if_there_is_at_least_one
+is_rendered._UIDs_are_resolved_using_``plone.app.uuid.utils.uuidToURL``._The
+resolveuid_filter_is_enabled_if_there_is_at_least_one
 ``plone.outputfilters.filters.resolveuid_and_caption.IResolveUidsEnabler``
 utility_whose_``available``_property_returns_``True``._This_mechanism_exists
 for_compatibility_with_TinyMCE_and_kupu,_which_both_provide_their_own_control
 panel_setting_to_enable_the_link-by-uid_feature._Image_captioning_-------------
 ---_Image_tags_with_the_"captioned"_class_and_a_``src``_attribute_that_resolves
 to_an_image_object_within_the_site_will_be_wrapped_in_a_definition_list_(DL)
 tag_which_includes_a_caption_based_on_the_value_of_the_image's_``description``
```

### Comparing `plone.outputfilters-5.0.1/docs/LICENSE.GPL` & `plone.outputfilters-5.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/docs/LICENSE.txt` & `plone.outputfilters-5.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/README.rst` & `plone.outputfilters-5.0.2/plone/outputfilters/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 A filter is a callable which accepts a UTF-8-encoded HTML string as input, and
 returns a modified UTF-8-encoded HTML string. A return value of ``None`` may be
 used to indicate that the input should not be modified.
 
 Example::
 
     import re
-    from zope.interface import implements
+    from zope.interface import implementer
     from plone.outputfilters.interfaces import IFilter
 
+    @implementer(IFilter)
     class EmDashAdder(object):
-        implements(IFilter)
         order = 1000
 
         def __init__(self, context, request):
             pass
 
         def is_enabled(self):
             return True
```

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/browser/resolveuid.py` & `plone.outputfilters-5.0.2/plone/outputfilters/browser/resolveuid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 from Acquisition import aq_base
 from plone.app.uuid.utils import uuidToObject as new_uuidToObject
+from plone.app.uuid.utils import uuidToURL as new_uuidToURL
+from plone.uuid.interfaces import IUUID
 from Products.CMFCore.utils import getToolByName
 from zExceptions import NotFound
+from zope.component.hooks import getSite
 from zope.deprecation import deprecate
 from zope.interface import implementer
 from zope.publisher.browser import BrowserView
 from zope.publisher.interfaces import IPublishTraverse
 
 
-try:
-    from zope.component.hooks import getSite
-except ImportError:
-    from zope.app.component.hooks import getSite
-
-
 @deprecate(
     "Please use plone.app.uuid.utils.uuidToURL instead. Will be removed in Plone 7"
 )
 def uuidToURL(uuid):
     """Resolves a UUID to a URL via the UID index of portal_catalog."""
     catalog = getToolByName(getSite(), "portal_catalog")
     res = catalog.unrestrictedSearchResults(UID=uuid)
     if res:
         return res[0].getURL()
 
 
-@deprecate("Import from plone.app.uuid.utils instead. Will be removed in Plone 7")
+@deprecate(
+    "Import from plone.app.uuid.utils instead, and call with unrestricted=True. "
+    "Will be removed in Plone 7"
+)
 def uuidToObject(uuid):
     """Resolves a UUID to an object via the Physical Path"""
     return new_uuidToObject(uuid, unrestricted=True)
 
 
-try:
-    from plone.uuid.interfaces import IUUID
-except ImportError:
-
-    def uuidFor(obj):
-        return obj.UID()
-
-else:
-
-    def uuidFor(obj):
-        uuid = IUUID(obj, None)
-        if uuid is None and hasattr(aq_base(obj), "UID"):
-            uuid = obj.UID()
-        return uuid
+@deprecate("uuidFor is not used in core Plone. Will be removed in Plone 7")
+def uuidFor(obj):
+    uuid = IUUID(obj, None)
+    if uuid is None and hasattr(aq_base(obj), "UID"):
+        uuid = obj.UID()
+    return uuid
 
 
 @implementer(IPublishTraverse)
 class ResolveUIDView(BrowserView):
     """Resolve a URL like /resolveuid/<uuid> to a normalized URL."""
 
     subpath = None
@@ -60,15 +52,15 @@
             traverse_subpath = list(traverse_subpath)
             traverse_subpath.reverse()
             self.subpath = traverse_subpath
             self.request["TraversalRequestNameStack"] = []
         return self
 
     def __call__(self):
-        url = uuidToURL(self.uuid)
+        url = new_uuidToURL(self.uuid)
 
         if not url:
             raise NotFound("The link you followed is broken")
 
         if self.subpath:
             url = "/".join([url] + self.subpath)
```

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/configure.zcml` & `plone.outputfilters-5.0.2/plone/outputfilters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/filters/configure.zcml` & `plone.outputfilters-5.0.2/plone/outputfilters/filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/filters/picture_variants.py` & `plone.outputfilters-5.0.2/plone/outputfilters/filters/picture_variants.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         for elem in soup.find_all("img"):
             picture_variant_name = elem.attrs.get("data-picturevariant", "")
             if not picture_variant_name:
                 continue
             picture_variants_config = get_picture_variants().get(picture_variant_name)
             if not picture_variants_config:
-                logger.warn(
+                logger.warning(
                     "Could not find the given picture_variant_name {}, leave tag untouched!".format(
                         picture_variant_name
                     )
                 )
                 continue
             sourceset = picture_variants_config.get("sourceset")
             if not sourceset:
```

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/filters/resolveuid_and_caption.py` & `plone.outputfilters-5.0.2/plone/outputfilters/filters/resolveuid_and_caption.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/interfaces.py` & `plone.outputfilters-5.0.2/plone/outputfilters/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/setuphandlers.py` & `plone.outputfilters-5.0.2/plone/outputfilters/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/testing.py` & `plone.outputfilters-5.0.2/plone/outputfilters/testing.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/image.jpg` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/test_apply_filters.py` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_apply_filters.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/test_docs.py` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/test_picture_variants.py` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_picture_variants.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/test_resolveuid_and_caption.py` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_resolveuid_and_caption.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from plone.namedfile.tests.test_scaling import DummyContent as NFDummyContent
 from plone.outputfilters.filters.resolveuid_and_caption import (  # noqa
     ResolveUIDAndCaptionFilter,
 )
 from plone.outputfilters.testing import PLONE_OUTPUTFILTERS_FUNCTIONAL_TESTING
 from Products.PortalTransforms.tests.utils import normalize_html
 
+import warnings
+
 
 PREFIX = abspath(dirname(__file__))
 
 
 def dummy_image():
     filename = join(PREFIX, "image.jpg")
     data = None
@@ -306,34 +308,40 @@
 
     def test_resolveuid_view_querystring(self):
         res = self.publish("/plone/resolveuid/%s?qs" % self.UID)
         self.assertEqual(301, res.status)
         self.assertEqual("http://nohost/plone/image.jpg?qs", res.headers["location"])
 
     def test_uuidToURL(self):
-        from plone.outputfilters.browser.resolveuid import uuidToURL
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            from plone.outputfilters.browser.resolveuid import uuidToURL
 
-        self.assertEqual("http://nohost/plone/image.jpg", uuidToURL(self.UID))
+            self.assertEqual("http://nohost/plone/image.jpg", uuidToURL(self.UID))
 
     def test_uuidToObject(self):
-        from plone.outputfilters.browser.resolveuid import uuidToObject
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            from plone.outputfilters.browser.resolveuid import uuidToObject
 
-        self.assertTrue(
-            self.portal["image.jpg"].aq_base is uuidToObject(self.UID).aq_base
-        )
+            self.assertTrue(
+                self.portal["image.jpg"].aq_base is uuidToObject(self.UID).aq_base
+            )
 
     def test_uuidToURL_permission(self):
-        from plone.outputfilters.browser.resolveuid import uuidToObject
-        from plone.outputfilters.browser.resolveuid import uuidToURL
-
-        self.portal.invokeFactory("Document", id="page", title="Page")
-        page = self.portal["page"]
-        self.logout()
-        self.assertEqual("http://nohost/plone/page", uuidToURL(page.UID()))
-        self.assertTrue(page.aq_base is uuidToObject(page.UID()).aq_base)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            from plone.outputfilters.browser.resolveuid import uuidToObject
+            from plone.outputfilters.browser.resolveuid import uuidToURL
+
+            self.portal.invokeFactory("Document", id="page", title="Page")
+            page = self.portal["page"]
+            self.logout()
+            self.assertEqual("http://nohost/plone/page", uuidToURL(page.UID()))
+            self.assertTrue(page.aq_base is uuidToObject(page.UID()).aq_base)
 
     def test_image_captioning_in_news_item(self):
         # Create a news item with a relative unscaled image
         self.portal.invokeFactory("News Item", id="a-news-item", title="Title")
         news_item = self.portal["a-news-item"]
         from plone.app.textfield.value import RichTextValue
```

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/tests/test_transforms.py` & `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py` & `plone.outputfilters-5.0.2/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py` & `plone.outputfilters-5.0.2/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.1/plone.outputfilters.egg-info/PKG-INFO` & `plone.outputfilters-5.0.2/plone.outputfilters.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.1
+Version: 5.0.2
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,18 +26,16 @@
 ``plone.outputfilters`` provides a framework for registering filters that
 get applied to text as it is rendered.
 
 By default, these filters are wired up to occur when text is transformed from
 the text/html mimetype to the text/x-html-safe mimetype via the
 PortalTransforms machinery.
 
-With both Archetypes TextFields and the RichText field of
-``plone.app.textfield``, this transform is typically applied when the field
-value is first accessed. The result of the transform is then cached in a
-volatile attribute for an hour or until the value is replaced.
+With  the RichText field of ``plone.app.textfield``, this transform is typically applied when the field value is first accessed.
+The result of the transform is then cached in a volatile attribute for an hour or until the value is replaced.
 
 
 Included Filters
 ================
 
 A default filter is included which provides the following features:
 
@@ -63,17 +61,15 @@
 
 Such URLs can be resolved by the ``resolveuid`` view, which resolves the UID to
 an object and then redirects to its URL. However, resolving links in this way
 requires an extra request after the redirect. The resolveuid filter avoids that
 by replacing such URLs with the object's actual full absolute URL as the link
 is rendered.
 
-UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``, with a fallback to
-the Archetypes UID catalog for backwards compatibility. LinguaPlone translations
-are supported when LinguaPlone is present.
+UIDs are resolved using ``plone.app.uuid.utils.uuidToURL``.
 
 The resolveuid filter is enabled if there is at least one
 ``plone.outputfilters.filters.resolveuid_and_caption.IResolveUidsEnabler``
 utility whose ``available`` property returns ``True``.  This mechanism exists
 for compatibility with TinyMCE and kupu, which both provide their own control
 panel setting to enable the link-by-uid feature.
 
@@ -140,19 +136,19 @@
 A filter is a callable which accepts a UTF-8-encoded HTML string as input, and
 returns a modified UTF-8-encoded HTML string. A return value of ``None`` may be
 used to indicate that the input should not be modified.
 
 Example::
 
     import re
-    from zope.interface import implements
+    from zope.interface import implementer
     from plone.outputfilters.interfaces import IFilter
 
+    @implementer(IFilter)
     class EmDashAdder(object):
-        implements(IFilter)
         order = 1000
 
         def __init__(self, context, request):
             pass
 
         def is_enabled(self):
             return True
@@ -222,14 +218,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (535edb14)
+
+
 5.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.1/plone.outputfilters.egg-info/SOURCES.txt` & `plone.outputfilters-5.0.2/plone.outputfilters.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 plone/outputfilters/browser/resolveuid.py
 plone/outputfilters/filters/__init__.py
 plone/outputfilters/filters/configure.zcml
 plone/outputfilters/filters/example.py
 plone/outputfilters/filters/picture_variants.py
 plone/outputfilters/filters/resolveuid_and_caption.py
 plone/outputfilters/profiles/default/plone.outputfilters.txt
-plone/outputfilters/tests/README_py2.rst
 plone/outputfilters/tests/__init__.py
 plone/outputfilters/tests/image.jpg
 plone/outputfilters/tests/test_apply_filters.py
 plone/outputfilters/tests/test_docs.py
 plone/outputfilters/tests/test_picture_variants.py
 plone/outputfilters/tests/test_resolveuid_and_caption.py
 plone/outputfilters/tests/test_transforms.py
```

### Comparing `plone.outputfilters-5.0.1/pyproject.toml` & `plone.outputfilters-5.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
 [tool.isort]
 profile = "plone"
 
 [tool.black]
 target-version = ["py38"]
 
+[tool.codespell]
+ignore-words-list = "discreet"
+
 [tool.dependencychecker]
 Zope = [
   # Zope own provided namespaces
   'App', 'OFS', 'Products.Five', 'Products.OFSP', 'Products.PageTemplates',
   'Products.SiteAccess', 'Shared', 'Testing', 'ZPublisher', 'ZTUtils',
   'Zope2', 'webdav', 'zmi',
   # Zope dependencies
@@ -56,12 +59,8 @@
   'zope.schema', 'zope.security', 'zope.site', 'zope.traversing', 'AccessControl',
 ]
 'plone.base' = [
   'AccessControl', 'Products.BTreeFolder2', 'Products.CMFCore',
   'Products.CMFDynamicViewFTI', 'zope.deprecation',
 ]
 python-dateutil = ['dateutil']
-beautifulsoup4 = ['bs4', ]
-ignore-packages = ['zope.app.component']
-
-[tool.codespell]
-ignore-words-list = "discreet"
+beautifulsoup4 = ['bs4']
```

### Comparing `plone.outputfilters-5.0.1/setup.py` & `plone.outputfilters-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "5.0.1"
+version = "5.0.2"
 
 
 def read(filename):
     with open(filename) as myfile:
         try:
             return myfile.read()
         except UnicodeDecodeError:
```

