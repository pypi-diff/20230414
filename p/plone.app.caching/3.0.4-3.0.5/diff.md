# Comparing `tmp/plone.app.caching-3.0.4.tar.gz` & `tmp/plone.app.caching-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.caching-3.0.4.tar", last modified: Tue Mar 14 16:09:32 2023, max compression
+gzip compressed data, was "plone.app.caching-3.0.5.tar", last modified: Thu Apr 13 23:32:45 2023, max compression
```

## Comparing `plone.app.caching-3.0.4.tar` & `plone.app.caching-3.0.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.827955 plone.app.caching-3.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)    14810 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18873 2023-03-14 16:09:32.828118 plone.app.caching-3.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3056 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.807770 plone.app.caching-3.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      674 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      308 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/docs/changelog_template.jinja
--rw-r--r--   0 maurits    (501) staff       (20)      230 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/lint-requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.808078 plone.app.caching-3.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.810845 plone.app.caching-3.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.814057 plone.app.caching-3.0.4/plone/app/caching/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.817259 plone.app.caching-3.0.4/plone/app/caching/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    41005 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21546 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      656 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9575 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     5523 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/import.pt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/plone.app.caching.gif
--rw-r--r--   0 maurits    (501) staff       (20)     6307 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/purge.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4622 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/browser/ramcache.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4468 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/caching.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3021 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3867 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)     3985 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/lookup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.818978 plone.app.caching-3.0.4/plone/app/caching/operations/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2783 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13296 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/default.py
--rw-r--r--   0 maurits    (501) staff       (20)     8040 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/ramcache.py
--rw-r--r--   0 maurits    (501) staff       (20)    24136 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/operations/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.803942 plone.app.caching-3.0.4/plone/app/caching/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.819920 plone.app.caching-3.0.4/plone/app/caching/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      594 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/plone.app.caching.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.821733 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     1934 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/basesettings.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/generic.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/moderate.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2486 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/strong.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/terse.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1792 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/weak.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.803604 plone.app.caching-3.0.4/plone/app/caching/profiles/v2/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.822039 plone.app.caching-3.0.4/plone/app/caching/profiles/v2/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/v2/registry/terse.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.822334 plone.app.caching-3.0.4/plone/app/caching/profiles/with-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4971 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/with-caching-proxy/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.822637 plone.app.caching-3.0.4/plone/app/caching/profiles/without-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4581 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles/without-caching-proxy/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1504 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     8396 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2171 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.826999 plone.app.caching-3.0.4/plone/app/caching/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      668 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.827683 plone.app.caching-3.0.4/plone/app/caching/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)     9819 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/data/plone-app-caching.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      189 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/data/testfile.csv
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test.css
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test.gif
--rw-r--r--   0 maurits    (501) staff       (20)    11871 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     9866 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_integration.py
--rw-r--r--   0 maurits    (501) staff       (20)     7101 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)    10537 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_lookup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2992 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_default.py
--rw-r--r--   0 maurits    (501) staff       (20)     6912 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_parameters.py
--rw-r--r--   0 maurits    (501) staff       (20)    55900 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    25361 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_profile_with_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    22166 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_profile_without_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    13490 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     5674 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone/app/caching/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:09:32.810550 plone.app.caching-3.0.4/plone.app.caching.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18873 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      695 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/plone.app.caching.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-03-14 16:09:32.828707 plone.app.caching-3.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-03-14 16:09:32.000000 plone.app.caching-3.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.017500 plone.app.caching-3.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)    14892 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    18955 2023-04-13 23:32:45.017643 plone.app.caching-3.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3056 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.997074 plone.app.caching-3.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      674 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/docs/changelog_template.jinja
+-rw-r--r--   0 maurits    (501) staff       (20)      230 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/lint-requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.997375 plone.app.caching-3.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.000164 plone.app.caching-3.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.003755 plone.app.caching-3.0.5/plone/app/caching/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.006962 plone.app.caching-3.0.5/plone/app/caching/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    41005 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21546 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      656 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/edit.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9575 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5523 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/import.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/plone.app.caching.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     6307 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/purge.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4622 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/browser/ramcache.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4468 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/caching.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3021 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3867 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/lastmodified.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3985 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/lookup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.008716 plone.app.caching-3.0.5/plone/app/caching/operations/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2783 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13297 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/default.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8040 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/etags.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/ramcache.py
+-rw-r--r--   0 maurits    (501) staff       (20)    24136 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/operations/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.993223 plone.app.caching-3.0.5/plone/app/caching/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.009676 plone.app.caching-3.0.5/plone/app/caching/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      594 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/plone.app.caching.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.011475 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)     1934 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/basesettings.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/generic.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/moderate.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2486 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/strong.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/terse.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1792 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/weak.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.992892 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.011779 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/terse.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.012088 plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/
+-rw-r--r--   0 maurits    (501) staff       (20)     4971 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.012390 plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/
+-rw-r--r--   0 maurits    (501) staff       (20)     4581 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1504 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     8396 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/purge.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2171 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.016693 plone.app.caching-3.0.5/plone/app/caching/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      668 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:45.017272 plone.app.caching-3.0.5/plone/app/caching/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)     9819 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/data/plone-app-caching.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      189 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/data/testfile.csv
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test.css
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    11871 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_etags.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9866 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_integration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7101 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_lastmodified.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10537 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_lookup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2992 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_default.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6912 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_parameters.py
+-rw-r--r--   0 maurits    (501) staff       (20)    55900 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25361 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_with_caching_proxy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22166 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_without_caching_proxy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13490 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_purge.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5674 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone/app/caching/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:32:44.999863 plone.app.caching-3.0.5/plone.app.caching.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    18955 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      695 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/plone.app.caching.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-13 23:32:45.018220 plone.app.caching-3.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-04-13 23:32:44.000000 plone.app.caching-3.0.5/setup.py
```

### Comparing `plone.app.caching-3.0.4/CHANGES.md` & `plone.app.caching-3.0.5/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,23 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.0.5 (2023-04-14)
+
+
+### Bug fixes:
+
+- Fix spelling error.
+  [gforcada] #124
+
+
 ## 3.0.4 (2023-03-14)
 
 
 ### Bug fixes:
 
 - Do not mention Squid but mentions CDNs in the descriptions. [jensens] #119
```

### Comparing `plone.app.caching-3.0.4/PKG-INFO` & `plone.app.caching-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.0.4
+Version: 3.0.5
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,23 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.0.5 (2023-04-14)
+
+
+### Bug fixes:
+
+- Fix spelling error.
+  [gforcada] #124
+
+
 ## 3.0.4 (2023-03-14)
 
 
 ### Bug fixes:
 
 - Do not mention Squid but mentions CDNs in the descriptions. [jensens] #119
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.4 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.5 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
```

### Comparing `plone.app.caching-3.0.4/README.md` & `plone.app.caching-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/docs/LICENSE.GPL` & `plone.app.caching-3.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/docs/LICENSE.txt` & `plone.app.caching-3.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/configure.zcml` & `plone.app.caching-3.0.5/plone/app/caching/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/controlpanel.pt` & `plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/controlpanel.py` & `plone.app.caching-3.0.5/plone/app/caching/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/edit.pt` & `plone.app.caching-3.0.5/plone/app/caching/browser/edit.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/edit.py` & `plone.app.caching-3.0.5/plone/app/caching/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/import.pt` & `plone.app.caching-3.0.5/plone/app/caching/browser/import.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/purge.pt` & `plone.app.caching-3.0.5/plone/app/caching/browser/purge.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/browser/ramcache.pt` & `plone.app.caching-3.0.5/plone/app/caching/browser/ramcache.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/caching.zcml` & `plone.app.caching-3.0.5/plone/app/caching/caching.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/configure.zcml` & `plone.app.caching-3.0.5/plone/app/caching/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/interfaces.py` & `plone.app.caching-3.0.5/plone/app/caching/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/lastmodified.py` & `plone.app.caching-3.0.5/plone/app/caching/lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/lookup.py` & `plone.app.caching-3.0.5/plone/app/caching/lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/operations/configure.zcml` & `plone.app.caching-3.0.5/plone/app/caching/operations/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/operations/default.py` & `plone.app.caching-3.0.5/plone/app/caching/operations/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     operation to help make the UI approachable by mortals
     """
 
     title = _("Moderate caching")
     description = _(
         "Cache in browser but expire immediately (same as 'weak caching'), "
         "and cache in proxy (default: 24 hrs). "
-        "Use a purgable caching reverse proxy for best results. "
+        "Use a purgeable caching reverse proxy for best results. "
         "Caution: If proxy cannot be purged, or cannot be configured "
         "to remove the 's-maxage' token from the response, then stale "
         "responses might be seen until the cached entry expires."
     )
     prefix = "plone.app.caching.moderateCaching"
     sort = 2
```

### Comparing `plone.app.caching-3.0.4/plone/app/caching/operations/etags.py` & `plone.app.caching-3.0.5/plone/app/caching/operations/etags.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/operations/ramcache.py` & `plone.app.caching-3.0.5/plone/app/caching/operations/ramcache.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/operations/utils.py` & `plone.app.caching-3.0.5/plone/app/caching/operations/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/controlpanel.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/basesettings.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/basesettings.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/generic.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/generic.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/moderate.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/moderate.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/strong.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/strong.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/terse.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/default/registry/weak.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/default/registry/weak.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/v2/registry/terse.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/v2/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/with-caching-proxy/registry.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/with-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles/without-caching-proxy/registry.xml` & `plone.app.caching-3.0.5/plone/app/caching/profiles/without-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/profiles.zcml` & `plone.app.caching-3.0.5/plone/app/caching/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/purge.py` & `plone.app.caching-3.0.5/plone/app/caching/purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/setuphandlers.py` & `plone.app.caching-3.0.5/plone/app/caching/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/testing.py` & `plone.app.caching-3.0.5/plone/app/caching/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/__init__.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/data/plone-app-caching.jpg` & `plone.app.caching-3.0.5/plone/app/caching/tests/data/plone-app-caching.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_etags.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_integration.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_lastmodified.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_lookup.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_default.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_default.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_parameters.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_parameters.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_operation_utils.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_operation_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_profile_with_caching_proxy.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_with_caching_proxy.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_profile_without_caching_proxy.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_profile_without_caching_proxy.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_purge.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/tests/test_utils.py` & `plone.app.caching-3.0.5/plone/app/caching/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone/app/caching/utils.py` & `plone.app.caching-3.0.5/plone/app/caching/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone.app.caching.egg-info/PKG-INFO` & `plone.app.caching-3.0.5/plone.app.caching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.0.4
+Version: 3.0.5
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,23 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.0.5 (2023-04-14)
+
+
+### Bug fixes:
+
+- Fix spelling error.
+  [gforcada] #124
+
+
 ## 3.0.4 (2023-03-14)
 
 
 ### Bug fixes:
 
 - Do not mention Squid but mentions CDNs in the descriptions. [jensens] #119
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.4 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.0.5 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
```

### Comparing `plone.app.caching-3.0.4/plone.app.caching.egg-info/SOURCES.txt` & `plone.app.caching-3.0.5/plone.app.caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/plone.app.caching.egg-info/requires.txt` & `plone.app.caching-3.0.5/plone.app.caching.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/pyproject.toml` & `plone.app.caching-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.0.4/setup.py` & `plone.app.caching-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.4"
+version = "3.0.5"
 
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
```

