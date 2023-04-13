# Comparing `tmp/plone.app.i18n-4.0.0a1.tar.gz` & `tmp/plone.app.i18n-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.i18n-4.0.0a1.tar", last modified: Tue Jun  7 17:59:35 2022, max compression
+gzip compressed data, was "plone.app.i18n-4.0.1.tar", last modified: Thu Apr 13 23:06:24 2023, max compression
```

## Comparing `plone.app.i18n-4.0.0a1.tar` & `plone.app.i18n-4.0.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.454417 plone.app.i18n-4.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)       79 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)     5427 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      145 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     6326 2022-06-07 17:59:35.454534 plone.app.i18n-4.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       51 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6023 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/bootstrap.py
--rw-r--r--   0 maurits    (501) staff       (20)      188 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.447274 plone.app.i18n-4.0.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      676 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.447618 plone.app.i18n-4.0.0a1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.449681 plone.app.i18n-4.0.0a1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.450459 plone.app.i18n-4.0.0a1/plone/app/i18n/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      191 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.451870 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.453171 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      382 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/languageselector.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4147 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/selector.py
--rw-r--r--   0 maurits    (501) staff       (20)      410 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)      106 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1021 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/countries.py
--rw-r--r--   0 maurits    (501) staff       (20)      778 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2601 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/languages.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.454191 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      777 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/countries.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/languages.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1025 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)      940 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/plone/app/i18n/tool.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-07 17:59:35.449425 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6326 2022-06-07 17:59:34.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1128 2022-06-07 17:59:35.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-06-07 17:59:34.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-06-07 17:59:35.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-06-07 17:59:34.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       65 2022-06-07 17:59:35.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-06-07 17:59:35.000000 plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      172 2022-06-07 17:59:35.455016 plone.app.i18n-4.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1341 2022-06-07 17:59:33.000000 plone.app.i18n-4.0.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.044674 plone.app.i18n-4.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)       79 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)     5628 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     6580 2023-04-13 23:06:24.044785 plone.app.i18n-4.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.036028 plone.app.i18n-4.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      676 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.036605 plone.app.i18n-4.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.039384 plone.app.i18n-4.0.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.040279 plone.app.i18n-4.0.1/plone/app/i18n/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.041710 plone.app.i18n-4.0.1/plone/app/i18n/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.043220 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      387 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1365 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/languageselector.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4147 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/selector.py
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      100 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1021 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/countries.py
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2601 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/languages.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.044395 plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/countries.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/languages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1015 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      940 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone/app/i18n/tool.gif
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:06:24.039138 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     6580 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/plone.app.i18n.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:06:24.045186 plone.app.i18n-4.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1472 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1282 2023-04-13 23:06:23.000000 plone.app.i18n-4.0.1/tox.ini
```

### Comparing `plone.app.i18n-4.0.0a1/CHANGES.rst` & `plone.app.i18n-4.0.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,34 @@
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
+  [plone devs] (de0ac4e7)
+
+
+4.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 4.0.0a1 (2022-06-07)
 --------------------
 
 Breaking changes:
 
 
 - Use SVG Flags in Language Selector
@@ -44,15 +64,15 @@
 ------------------
 
 Bug fixes:
 
 - Remove zopetestcase.
   [ivanteoh, maurits]
 
-- Add coding header to pyton files.
+- Add coding header to python files.
   [gforcada]
 
 
 3.0.3 (2016-08-18)
 ------------------
 
 Fixes:
```

### Comparing `plone.app.i18n-4.0.0a1/PKG-INFO` & `plone.app.i18n-4.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.app.i18n
-Version: 4.0.0a1
+Version: 4.0.1
 Summary: Plone specific i18n extensions.
 Home-page: https://github.com/plone/plone.app.i18n
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Keywords: plone i18n
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 Plone specific i18n extensions.
 
@@ -33,14 +34,34 @@
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
+  [plone devs] (de0ac4e7)
+
+
+4.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 4.0.0a1 (2022-06-07)
 --------------------
 
 Breaking changes:
 
 
 - Use SVG Flags in Language Selector
@@ -73,15 +94,15 @@
 ------------------
 
 Bug fixes:
 
 - Remove zopetestcase.
   [ivanteoh, maurits]
 
-- Add coding header to pyton files.
+- Add coding header to python files.
   [gforcada]
 
 
 3.0.3 (2016-08-18)
 ------------------
 
 Fixes:
@@ -282,9 +303,7 @@
 ---------------------
 
 - Initial implementation.
   [hannosch]
 
 - Initial package structure.
   [zopeskel]
-
-
```

### Comparing `plone.app.i18n-4.0.0a1/docs/LICENSE.GPL` & `plone.app.i18n-4.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/docs/LICENSE.txt` & `plone.app.i18n-4.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/languageselector.pt` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/languageselector.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 <tal:language tal:condition="view/available">
-  <ul
-      id="portal-languageselector"
-      tal:define="showFlags view/showFlags;
-                languages view/languages;
-                here_url context/@@plone_context_state/view_url;
-                portal_url view/portal_url;
-                icons python:context.restrictedTraverse('@@iconresolver');">
+  <ul id="portal-languageselector"
+      tal:define="
+        showFlags view/showFlags;
+        languages view/languages;
+        here_url context/@@plone_context_state/view_url;
+        portal_url view/portal_url;
+        icons python:context.restrictedTraverse('@@iconresolver');
+      "
+  >
     <tal:language repeat="lang languages">
-      <li
-          tal:define="code lang/code;
-                    selected lang/selected;
-                    codeclass string:language-${code};
-                    current python: selected and 'currentLanguage ' or '';"
-          tal:attributes="class string:${current}${codeclass}">
-        <a
-            href=""
-            tal:define="flag lang/flag|nothing;
-                       name lang/native|lang/name;
-                       showflag python:showFlags and flag;"
-            tal:attributes="href string:${here_url}?set_language=${code};
-                           title name">
+      <li tal:define="
+            code lang/code;
+            selected lang/selected;
+            codeclass string:language-${code};
+            current python: selected and 'currentLanguage ' or '';
+          "
+          tal:attributes="
+            class string:${current}${codeclass};
+          "
+      >
+        <a href=""
+           tal:define="
+             flag lang/flag|nothing;
+             name lang/native|lang/name;
+             showflag python:showFlags and flag;
+           "
+           tal:attributes="
+             href string:${here_url}?set_language=${code};
+             title name;
+           "
+        >
           <tal:flag condition="showflag">
             <img tal:replace="structure python:icons.tag(flag, tag_class='plone-icon-flag')" />
           </tal:flag>
-          <tal:nonflag
-              condition="not: showflag"
-              replace="name">language name</tal:nonflag>
+          <tal:nonflag condition="not: showflag"
+                       replace="name"
+          >language name</tal:nonflag>
         </a>
       </li>
     </tal:language>
   </ul>
 </tal:language>
```

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/browser/selector.py` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/browser/selector.py`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/countries.py` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/countries.py`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/interfaces.py` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/languages.py` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/languages.py`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/countries.txt` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/countries.txt`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/languages.txt` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/languages.txt`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/locales/tests/test_doctests.py` & `plone.app.i18n-4.0.1/plone/app/i18n/locales/tests/test_doctests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from plone.app.testing import PLONE_INTEGRATION_TESTING
 from plone.testing import layered
 
 import doctest
-import re
 import unittest
 
 
 OPTIONFLAGS = (
     doctest.REPORT_ONLY_FIRST_FAILURE | doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
 )
```

### Comparing `plone.app.i18n-4.0.0a1/plone/app/i18n/tool.gif` & `plone.app.i18n-4.0.1/plone/app/i18n/tool.gif`

 * *Files identical despite different names*

### Comparing `plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/PKG-INFO` & `plone.app.i18n-4.0.1/plone.app.i18n.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.app.i18n
-Version: 4.0.0a1
+Version: 4.0.1
 Summary: Plone specific i18n extensions.
 Home-page: https://github.com/plone/plone.app.i18n
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Keywords: plone i18n
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 Plone specific i18n extensions.
 
@@ -33,14 +34,34 @@
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
+  [plone devs] (de0ac4e7)
+
+
+4.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 4.0.0a1 (2022-06-07)
 --------------------
 
 Breaking changes:
 
 
 - Use SVG Flags in Language Selector
@@ -73,15 +94,15 @@
 ------------------
 
 Bug fixes:
 
 - Remove zopetestcase.
   [ivanteoh, maurits]
 
-- Add coding header to pyton files.
+- Add coding header to python files.
   [gforcada]
 
 
 3.0.3 (2016-08-18)
 ------------------
 
 Fixes:
@@ -282,9 +303,7 @@
 ---------------------
 
 - Initial implementation.
   [hannosch]
 
 - Initial package structure.
   [zopeskel]
-
-
```

### Comparing `plone.app.i18n-4.0.0a1/plone.app.i18n.egg-info/SOURCES.txt` & `plone.app.i18n-4.0.1/plone.app.i18n.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+.editorconfig
 .gitignore
+.meta.toml
+.pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
-bootstrap.py
 buildout.cfg
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.i18n.egg-info/PKG-INFO
 plone.app.i18n.egg-info/SOURCES.txt
 plone.app.i18n.egg-info/dependency_links.txt
 plone.app.i18n.egg-info/namespace_packages.txt
```

### Comparing `plone.app.i18n-4.0.0a1/setup.py` & `plone.app.i18n-4.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.0a1"
+version = "4.0.1"
 
 setup(
     name="plone.app.i18n",
     version=version,
     description="Plone specific i18n extensions.",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
@@ -15,31 +15,35 @@
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="plone i18n",
     author="Plone Foundation",
     author_email="releaseteam@plone.org",
     url="https://github.com/plone/plone.app.i18n",
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "Products.CMFCore",
         "plone.i18n",
+        "zope.viewlet",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
+            "plone.testing",
         ]
     },
 )
```

