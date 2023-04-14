# Comparing `tmp/mpire-2.7.0.tar.gz` & `tmp/mpire-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpire-2.7.0.tar", last modified: Fri Mar 17 14:31:22 2023, max compression
+gzip compressed data, was "dist/mpire-2.7.1.tar", last modified: Fri Apr 14 12:29:46 2023, max compression
```

## Comparing `mpire-2.7.0.tar` & `mpire-2.7.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11685 2023-03-17 14:31:12.000000 mpire-2.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14893 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/bin/
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-03-17 14:31:12.000000 mpire-2.7.0/bin/mpire-dashboard
--rw-r--r--   0 runner    (1001) docker     (122)    14893 2023-03-17 14:31:22.000000 mpire-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-03-17 14:31:12.000000 mpire-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-03-17 14:31:12.000000 mpire-2.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire/
--rw-r--r--   0 runner    (1001) docker     (122)     9657 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/async_result.py
--rw-r--r--   0 runner    (1001) docker     (122)    14409 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13340 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/insights.py
--rw-r--r--   0 runner    (1001) docker     (122)    32497 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/context.py
--rw-r--r--   0 runner    (1001) docker     (122)    16630 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    71279 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     7967 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/style.css
--rw-r--r--   0 runner    (1001) docker     (122)   155756 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/refresh.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire/dashboard/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   108738 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (122)    18028 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    23424 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)    45404 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    20127 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (122)    13740 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/glyphicons.css
--rw-r--r--   0 runner    (1001) docker     (122)    16857 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    88145 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    78635 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/mpire/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     9516 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/templates/progress_bar.html
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/templates/menu_top_right.html
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/templates/mpire.html
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     8789 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/dashboard/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    30122 2023-03-17 14:31:12.000000 mpire-2.7.0/mpire/comms.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-03-17 14:31:12.000000 mpire-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-03-17 14:31:12.000000 mpire-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:22.000000 mpire-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)    14011 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_async_result.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    25622 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23133 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_insights.py
--rw-r--r--   0 runner    (1001) docker     (122)    79205 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)    23233 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    33534 2023-03-17 14:31:12.000000 mpire-2.7.0/tests/test_comms.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-03-17 14:31:22.000000 mpire-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    14920 2023-04-14 12:29:46.000000 mpire-2.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23233 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14011 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_async_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33534 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_comms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79205 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25622 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23133 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/test_insights.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-04-14 12:29:36.000000 mpire-2.7.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire/
+-rw-r--r--   0 runner    (1001) docker     (122)    13340 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/insights.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32497 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71279 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9657 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/async_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/templates/menu_top_right.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9516 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/templates/progress_bar.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/templates/mpire.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/refresh.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16857 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13740 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/glyphicons.css
+-rw-r--r--   0 runner    (1001) docker     (122)   155756 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    78635 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire/dashboard/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    18028 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    23424 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   108738 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    45404 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    20127 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (122)    88145 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/static/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8789 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30122 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/comms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7967 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16630 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14409 2023-04-14 12:29:36.000000 mpire-2.7.1/mpire/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/mpire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14920 2023-04-14 12:29:45.000000 mpire-2.7.1/mpire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-04-14 12:29:45.000000 mpire-2.7.1/mpire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-04-14 12:29:45.000000 mpire-2.7.1/mpire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-14 12:29:45.000000 mpire-2.7.1/mpire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 12:29:45.000000 mpire-2.7.1/mpire.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:29:46.000000 mpire-2.7.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-04-14 12:29:36.000000 mpire-2.7.1/bin/mpire-dashboard
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-14 12:29:46.000000 mpire-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-14 12:29:36.000000 mpire-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-14 12:29:36.000000 mpire-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11707 2023-04-14 12:29:36.000000 mpire-2.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-14 12:29:36.000000 mpire-2.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-04-14 12:29:36.000000 mpire-2.7.1/setup.py
```

### Comparing `mpire-2.7.0/README.rst` & `mpire-2.7.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 MPIRE (MultiProcessing Is Really Easy)
 ======================================
 
 |Build status| |Docs status| |Pypi status| |Python versions|
 
-.. |Build status| image:: https://github.com/Slimmer-AI/mpire/workflows/Build/badge.svg?branch=master
-.. |Docs status| image:: https://github.com/Slimmer-AI/mpire/workflows/Docs/badge.svg?branch=master
+.. |Build status| image:: https://github.com/sybrenjansen/mpire/workflows/Build/badge.svg?branch=master
+.. |Docs status| image:: https://github.com/sybrenjansen/mpire/workflows/Docs/badge.svg?branch=master
 .. |Pypi status| image:: https://img.shields.io/pypi/v/mpire
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/mpire
 
 ``MPIRE``, short for MultiProcessing Is Really Easy, is a Python package for multiprocessing. ``MPIRE`` is faster in
 most scenarios, packs more features, and is generally more user-friendly than the default multiprocessing package. It
 combines the convenient map like functions of ``multiprocessing.Pool`` with the benefits of using copy-on-write shared
 objects of ``multiprocessing.Process``, together with easy-to-use worker state, worker insights, worker init and exit
 functions, timeouts, and progress bar functionality.
 
-Full documentation is available at https://slimmer-ai.github.io/mpire/.
+Full documentation is available at https://sybrenjansen.github.io/mpire/.
 
 Features
 --------
 
 - Faster execution than other multiprocessing libraries. See benchmarks_.
 - Intuitive, Pythonic syntax
 - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
@@ -44,15 +44,15 @@
 MPIRE has been tested on both Linux and Windows. There are a few minor known caveats for Windows users, which can be
 found here_.
 
 .. _benchmarks: https://towardsdatascience.com/mpire-for-python-multiprocessing-is-really-easy-d2ae7999a3e9
 .. _multiprocess: https://github.com/uqfoundation/multiprocess
 .. _dill: https://pypi.org/project/dill/
 .. _tqdm: https://tqdm.github.io/
-.. _here: https://slimmer-ai.github.io/mpire/troubleshooting.html#windows
+.. _here: https://sybrenjansen.github.io/mpire/troubleshooting.html#windows
 
 
 Installation
 ------------
 
 Through pip (PyPi):
 
@@ -114,16 +114,16 @@
         results = pool.map(time_consuming_function, range(10), progress_bar=True)
 
 And it will output a nicely formatted tqdm_ progress bar.
 
 MPIRE also offers a dashboard, for which you need to install additional dependencies_. See Dashboard_ for more
 information.
 
-.. _dependencies: https://slimmer-ai.github.io/mpire/install.html#dashboard
-.. _Dashboard: https://slimmer-ai.github.io/mpire/usage/dashboard.html
+.. _dependencies: https://sybrenjansen.github.io/mpire/install.html#dashboard
+.. _Dashboard: https://sybrenjansen.github.io/mpire/usage/dashboard.html
 
 
 Shared objects
 ~~~~~~~~~~~~~~
 
 Note: Copy-on-write shared objects is only available for start method ``fork``. For ``threading`` the objects are shared
 as-is. For other start methods the shared objects are copied once for each worker, which can still be better than once
@@ -142,15 +142,15 @@
     def main():
         some_object = ...
         with WorkerPool(n_jobs=5, shared_objects=some_object) as pool:
             results = pool.map(time_consuming_function, range(10), progress_bar=True)
 
 See shared_objects_ for more details.
 
-.. _shared_objects: https://slimmer-ai.github.io/mpire/usage/workerpool/shared_objects.html
+.. _shared_objects: https://sybrenjansen.github.io/mpire/usage/workerpool/shared_objects.html
 
 Worker initialization
 ~~~~~~~~~~~~~~~~~~~~~
 
 Workers can be initialized using the ``worker_init`` feature. Together with ``worker_state`` you can load a model, or
 set up a database connection, etc.:
 
@@ -168,15 +168,15 @@
     with WorkerPool(n_jobs=5, use_worker_state=True) as pool:
         results = pool.map(task, range(10), worker_init=init)
 
 Similarly, you can use the ``worker_exit`` feature to let MPIRE call a function whenever a worker terminates. You can
 even let this exit function return results, which can be obtained later on. See the `worker_init and worker_exit`_
 section for more information.
 
-.. _worker_init and worker_exit: https://slimmer-ai.github.io/mpire/usage/map/worker_init_exit.html
+.. _worker_init and worker_exit: https://sybrenjansen.github.io/mpire/usage/map/worker_init_exit.html
 
 
 Worker insights
 ~~~~~~~~~~~~~~~
 
 When your multiprocessing setup isn't performing as you want it to and you have no clue what's causing it, there's the
 worker insights functionality. This will give you insight in your setup, but it will not profile the function you're
@@ -191,15 +191,15 @@
 
     with WorkerPool(n_jobs=5, enable_insights=True) as pool:
         results = pool.map(time_consuming_function, range(10))
         insights = pool.get_insights()
 
 See `worker insights`_ for a more detailed example and expected output.
 
-.. _worker insights: https://slimmer-ai.github.io/mpire/usage/workerpool/worker_insights.html
+.. _worker insights: https://sybrenjansen.github.io/mpire/usage/workerpool/worker_insights.html
 
 
 Timeouts
 ~~~~~~~~
 
 Timeouts can be set separately for the target, ``worker_init`` and ``worker_exit`` functions. When a timeout has been
 set and reached, it will throw a ``TimeoutError``:
@@ -224,15 +224,15 @@
         pool.map(time_consuming_function, range(10), worker_init=init, worker_exit=exit_,
                  worker_init_timeout=3.0, worker_exit_timeout=150.5)
 
 When using ``threading`` as start method MPIRE won't be able to interrupt certain functions, like ``time.sleep``.
 
 See timeouts_ for more details.
 
-.. _timeouts: https://slimmer-ai.github.io/mpire/usage/map/timeouts.html
+.. _timeouts: https://sybrenjansen.github.io/mpire/usage/map/timeouts.html
 
 Benchmarks
 ----------
 
 MPIRE has been benchmarked on three different benchmarks: numerical computation, stateful computation, and expensive
 initialization. More details on these benchmarks can be found in this `blog post`_. All code for these benchmarks can
 be found in this project_.
@@ -258,15 +258,15 @@
 .. _project: https://github.com/sybrenjansen/multiprocessing_benchmarks
 
 
 
 Documentation
 -------------
 
-See the full documentation at https://slimmer-ai.github.io/mpire/ for information on all the other features of MPIRE.
+See the full documentation at https://sybrenjansen.github.io/mpire/ for information on all the other features of MPIRE.
 
 If you want to build the documentation yourself, please install the documentation dependencies by executing:
 
 .. code-block:: bash
 
     pip install mpire[docs]
```

### Comparing `mpire-2.7.0/mpire.egg-info/PKG-INFO` & `mpire-2.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: mpire
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Python package for easy multiprocessing, but faster than multiprocessing
-Home-page: https://github.com/Slimmer-AI/mpire
-Author: Slimmer AI
+Home-page: https://github.com/sybrenjansen/mpire
+Author: Sybren Jansen
 License: MIT
 Description: MPIRE (MultiProcessing Is Really Easy)
         ======================================
         
         |Build status| |Docs status| |Pypi status| |Python versions|
         
-        .. |Build status| image:: https://github.com/Slimmer-AI/mpire/workflows/Build/badge.svg?branch=master
-        .. |Docs status| image:: https://github.com/Slimmer-AI/mpire/workflows/Docs/badge.svg?branch=master
+        .. |Build status| image:: https://github.com/sybrenjansen/mpire/workflows/Build/badge.svg?branch=master
+        .. |Docs status| image:: https://github.com/sybrenjansen/mpire/workflows/Docs/badge.svg?branch=master
         .. |Pypi status| image:: https://img.shields.io/pypi/v/mpire
         .. |Python versions| image:: https://img.shields.io/pypi/pyversions/mpire
         
         ``MPIRE``, short for MultiProcessing Is Really Easy, is a Python package for multiprocessing. ``MPIRE`` is faster in
         most scenarios, packs more features, and is generally more user-friendly than the default multiprocessing package. It
         combines the convenient map like functions of ``multiprocessing.Pool`` with the benefits of using copy-on-write shared
         objects of ``multiprocessing.Process``, together with easy-to-use worker state, worker insights, worker init and exit
         functions, timeouts, and progress bar functionality.
         
-        Full documentation is available at https://slimmer-ai.github.io/mpire/.
+        Full documentation is available at https://sybrenjansen.github.io/mpire/.
         
         Features
         --------
         
         - Faster execution than other multiprocessing libraries. See benchmarks_.
         - Intuitive, Pythonic syntax
         - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
@@ -51,15 +51,15 @@
         MPIRE has been tested on both Linux and Windows. There are a few minor known caveats for Windows users, which can be
         found here_.
         
         .. _benchmarks: https://towardsdatascience.com/mpire-for-python-multiprocessing-is-really-easy-d2ae7999a3e9
         .. _multiprocess: https://github.com/uqfoundation/multiprocess
         .. _dill: https://pypi.org/project/dill/
         .. _tqdm: https://tqdm.github.io/
-        .. _here: https://slimmer-ai.github.io/mpire/troubleshooting.html#windows
+        .. _here: https://sybrenjansen.github.io/mpire/troubleshooting.html#windows
         
         
         Installation
         ------------
         
         Through pip (PyPi):
         
@@ -121,16 +121,16 @@
                 results = pool.map(time_consuming_function, range(10), progress_bar=True)
         
         And it will output a nicely formatted tqdm_ progress bar.
         
         MPIRE also offers a dashboard, for which you need to install additional dependencies_. See Dashboard_ for more
         information.
         
-        .. _dependencies: https://slimmer-ai.github.io/mpire/install.html#dashboard
-        .. _Dashboard: https://slimmer-ai.github.io/mpire/usage/dashboard.html
+        .. _dependencies: https://sybrenjansen.github.io/mpire/install.html#dashboard
+        .. _Dashboard: https://sybrenjansen.github.io/mpire/usage/dashboard.html
         
         
         Shared objects
         ~~~~~~~~~~~~~~
         
         Note: Copy-on-write shared objects is only available for start method ``fork``. For ``threading`` the objects are shared
         as-is. For other start methods the shared objects are copied once for each worker, which can still be better than once
@@ -149,15 +149,15 @@
             def main():
                 some_object = ...
                 with WorkerPool(n_jobs=5, shared_objects=some_object) as pool:
                     results = pool.map(time_consuming_function, range(10), progress_bar=True)
         
         See shared_objects_ for more details.
         
-        .. _shared_objects: https://slimmer-ai.github.io/mpire/usage/workerpool/shared_objects.html
+        .. _shared_objects: https://sybrenjansen.github.io/mpire/usage/workerpool/shared_objects.html
         
         Worker initialization
         ~~~~~~~~~~~~~~~~~~~~~
         
         Workers can be initialized using the ``worker_init`` feature. Together with ``worker_state`` you can load a model, or
         set up a database connection, etc.:
         
@@ -175,15 +175,15 @@
             with WorkerPool(n_jobs=5, use_worker_state=True) as pool:
                 results = pool.map(task, range(10), worker_init=init)
         
         Similarly, you can use the ``worker_exit`` feature to let MPIRE call a function whenever a worker terminates. You can
         even let this exit function return results, which can be obtained later on. See the `worker_init and worker_exit`_
         section for more information.
         
-        .. _worker_init and worker_exit: https://slimmer-ai.github.io/mpire/usage/map/worker_init_exit.html
+        .. _worker_init and worker_exit: https://sybrenjansen.github.io/mpire/usage/map/worker_init_exit.html
         
         
         Worker insights
         ~~~~~~~~~~~~~~~
         
         When your multiprocessing setup isn't performing as you want it to and you have no clue what's causing it, there's the
         worker insights functionality. This will give you insight in your setup, but it will not profile the function you're
@@ -198,15 +198,15 @@
         
             with WorkerPool(n_jobs=5, enable_insights=True) as pool:
                 results = pool.map(time_consuming_function, range(10))
                 insights = pool.get_insights()
         
         See `worker insights`_ for a more detailed example and expected output.
         
-        .. _worker insights: https://slimmer-ai.github.io/mpire/usage/workerpool/worker_insights.html
+        .. _worker insights: https://sybrenjansen.github.io/mpire/usage/workerpool/worker_insights.html
         
         
         Timeouts
         ~~~~~~~~
         
         Timeouts can be set separately for the target, ``worker_init`` and ``worker_exit`` functions. When a timeout has been
         set and reached, it will throw a ``TimeoutError``:
@@ -231,15 +231,15 @@
                 pool.map(time_consuming_function, range(10), worker_init=init, worker_exit=exit_,
                          worker_init_timeout=3.0, worker_exit_timeout=150.5)
         
         When using ``threading`` as start method MPIRE won't be able to interrupt certain functions, like ``time.sleep``.
         
         See timeouts_ for more details.
         
-        .. _timeouts: https://slimmer-ai.github.io/mpire/usage/map/timeouts.html
+        .. _timeouts: https://sybrenjansen.github.io/mpire/usage/map/timeouts.html
         
         Benchmarks
         ----------
         
         MPIRE has been benchmarked on three different benchmarks: numerical computation, stateful computation, and expensive
         initialization. More details on these benchmarks can be found in this `blog post`_. All code for these benchmarks can
         be found in this project_.
@@ -265,15 +265,15 @@
         .. _project: https://github.com/sybrenjansen/multiprocessing_benchmarks
         
         
         
         Documentation
         -------------
         
-        See the full documentation at https://slimmer-ai.github.io/mpire/ for information on all the other features of MPIRE.
+        See the full documentation at https://sybrenjansen.github.io/mpire/ for information on all the other features of MPIRE.
         
         If you want to build the documentation yourself, please install the documentation dependencies by executing:
         
         .. code-block:: bash
         
             pip install mpire[docs]
         
@@ -306,11 +306,11 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: docs
 Provides-Extra: dill
-Provides-Extra: dashboard
+Provides-Extra: docs
 Provides-Extra: testing
+Provides-Extra: dashboard
```

### Comparing `mpire-2.7.0/mpire.egg-info/requires.txt` & `mpire-2.7.1/mpire.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire.egg-info/SOURCES.txt` & `mpire-2.7.1/mpire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/bin/mpire-dashboard` & `mpire-2.7.1/bin/mpire-dashboard`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/PKG-INFO` & `mpire-2.7.1/mpire.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: mpire
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Python package for easy multiprocessing, but faster than multiprocessing
-Home-page: https://github.com/Slimmer-AI/mpire
-Author: Slimmer AI
+Home-page: https://github.com/sybrenjansen/mpire
+Author: Sybren Jansen
 License: MIT
 Description: MPIRE (MultiProcessing Is Really Easy)
         ======================================
         
         |Build status| |Docs status| |Pypi status| |Python versions|
         
-        .. |Build status| image:: https://github.com/Slimmer-AI/mpire/workflows/Build/badge.svg?branch=master
-        .. |Docs status| image:: https://github.com/Slimmer-AI/mpire/workflows/Docs/badge.svg?branch=master
+        .. |Build status| image:: https://github.com/sybrenjansen/mpire/workflows/Build/badge.svg?branch=master
+        .. |Docs status| image:: https://github.com/sybrenjansen/mpire/workflows/Docs/badge.svg?branch=master
         .. |Pypi status| image:: https://img.shields.io/pypi/v/mpire
         .. |Python versions| image:: https://img.shields.io/pypi/pyversions/mpire
         
         ``MPIRE``, short for MultiProcessing Is Really Easy, is a Python package for multiprocessing. ``MPIRE`` is faster in
         most scenarios, packs more features, and is generally more user-friendly than the default multiprocessing package. It
         combines the convenient map like functions of ``multiprocessing.Pool`` with the benefits of using copy-on-write shared
         objects of ``multiprocessing.Process``, together with easy-to-use worker state, worker insights, worker init and exit
         functions, timeouts, and progress bar functionality.
         
-        Full documentation is available at https://slimmer-ai.github.io/mpire/.
+        Full documentation is available at https://sybrenjansen.github.io/mpire/.
         
         Features
         --------
         
         - Faster execution than other multiprocessing libraries. See benchmarks_.
         - Intuitive, Pythonic syntax
         - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
@@ -51,15 +51,15 @@
         MPIRE has been tested on both Linux and Windows. There are a few minor known caveats for Windows users, which can be
         found here_.
         
         .. _benchmarks: https://towardsdatascience.com/mpire-for-python-multiprocessing-is-really-easy-d2ae7999a3e9
         .. _multiprocess: https://github.com/uqfoundation/multiprocess
         .. _dill: https://pypi.org/project/dill/
         .. _tqdm: https://tqdm.github.io/
-        .. _here: https://slimmer-ai.github.io/mpire/troubleshooting.html#windows
+        .. _here: https://sybrenjansen.github.io/mpire/troubleshooting.html#windows
         
         
         Installation
         ------------
         
         Through pip (PyPi):
         
@@ -121,16 +121,16 @@
                 results = pool.map(time_consuming_function, range(10), progress_bar=True)
         
         And it will output a nicely formatted tqdm_ progress bar.
         
         MPIRE also offers a dashboard, for which you need to install additional dependencies_. See Dashboard_ for more
         information.
         
-        .. _dependencies: https://slimmer-ai.github.io/mpire/install.html#dashboard
-        .. _Dashboard: https://slimmer-ai.github.io/mpire/usage/dashboard.html
+        .. _dependencies: https://sybrenjansen.github.io/mpire/install.html#dashboard
+        .. _Dashboard: https://sybrenjansen.github.io/mpire/usage/dashboard.html
         
         
         Shared objects
         ~~~~~~~~~~~~~~
         
         Note: Copy-on-write shared objects is only available for start method ``fork``. For ``threading`` the objects are shared
         as-is. For other start methods the shared objects are copied once for each worker, which can still be better than once
@@ -149,15 +149,15 @@
             def main():
                 some_object = ...
                 with WorkerPool(n_jobs=5, shared_objects=some_object) as pool:
                     results = pool.map(time_consuming_function, range(10), progress_bar=True)
         
         See shared_objects_ for more details.
         
-        .. _shared_objects: https://slimmer-ai.github.io/mpire/usage/workerpool/shared_objects.html
+        .. _shared_objects: https://sybrenjansen.github.io/mpire/usage/workerpool/shared_objects.html
         
         Worker initialization
         ~~~~~~~~~~~~~~~~~~~~~
         
         Workers can be initialized using the ``worker_init`` feature. Together with ``worker_state`` you can load a model, or
         set up a database connection, etc.:
         
@@ -175,15 +175,15 @@
             with WorkerPool(n_jobs=5, use_worker_state=True) as pool:
                 results = pool.map(task, range(10), worker_init=init)
         
         Similarly, you can use the ``worker_exit`` feature to let MPIRE call a function whenever a worker terminates. You can
         even let this exit function return results, which can be obtained later on. See the `worker_init and worker_exit`_
         section for more information.
         
-        .. _worker_init and worker_exit: https://slimmer-ai.github.io/mpire/usage/map/worker_init_exit.html
+        .. _worker_init and worker_exit: https://sybrenjansen.github.io/mpire/usage/map/worker_init_exit.html
         
         
         Worker insights
         ~~~~~~~~~~~~~~~
         
         When your multiprocessing setup isn't performing as you want it to and you have no clue what's causing it, there's the
         worker insights functionality. This will give you insight in your setup, but it will not profile the function you're
@@ -198,15 +198,15 @@
         
             with WorkerPool(n_jobs=5, enable_insights=True) as pool:
                 results = pool.map(time_consuming_function, range(10))
                 insights = pool.get_insights()
         
         See `worker insights`_ for a more detailed example and expected output.
         
-        .. _worker insights: https://slimmer-ai.github.io/mpire/usage/workerpool/worker_insights.html
+        .. _worker insights: https://sybrenjansen.github.io/mpire/usage/workerpool/worker_insights.html
         
         
         Timeouts
         ~~~~~~~~
         
         Timeouts can be set separately for the target, ``worker_init`` and ``worker_exit`` functions. When a timeout has been
         set and reached, it will throw a ``TimeoutError``:
@@ -231,15 +231,15 @@
                 pool.map(time_consuming_function, range(10), worker_init=init, worker_exit=exit_,
                          worker_init_timeout=3.0, worker_exit_timeout=150.5)
         
         When using ``threading`` as start method MPIRE won't be able to interrupt certain functions, like ``time.sleep``.
         
         See timeouts_ for more details.
         
-        .. _timeouts: https://slimmer-ai.github.io/mpire/usage/map/timeouts.html
+        .. _timeouts: https://sybrenjansen.github.io/mpire/usage/map/timeouts.html
         
         Benchmarks
         ----------
         
         MPIRE has been benchmarked on three different benchmarks: numerical computation, stateful computation, and expensive
         initialization. More details on these benchmarks can be found in this `blog post`_. All code for these benchmarks can
         be found in this project_.
@@ -265,15 +265,15 @@
         .. _project: https://github.com/sybrenjansen/multiprocessing_benchmarks
         
         
         
         Documentation
         -------------
         
-        See the full documentation at https://slimmer-ai.github.io/mpire/ for information on all the other features of MPIRE.
+        See the full documentation at https://sybrenjansen.github.io/mpire/ for information on all the other features of MPIRE.
         
         If you want to build the documentation yourself, please install the documentation dependencies by executing:
         
         .. code-block:: bash
         
             pip install mpire[docs]
         
@@ -306,11 +306,11 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: docs
 Provides-Extra: dill
-Provides-Extra: dashboard
+Provides-Extra: docs
 Provides-Extra: testing
+Provides-Extra: dashboard
```

### Comparing `mpire-2.7.0/LICENSE` & `mpire-2.7.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Slimmer-AI
+Copyright (c) 2023 Sybren Jansen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mpire-2.7.0/mpire/async_result.py` & `mpire-2.7.1/mpire/async_result.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/progress_bar.py` & `mpire-2.7.1/mpire/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/utils.py` & `mpire-2.7.1/mpire/utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/insights.py` & `mpire-2.7.1/mpire/insights.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/worker.py` & `mpire-2.7.1/mpire/worker.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/context.py` & `mpire-2.7.1/mpire/context.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/params.py` & `mpire-2.7.1/mpire/params.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/pool.py` & `mpire-2.7.1/mpire/pool.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/tqdm_utils.py` & `mpire-2.7.1/mpire/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/exception.py` & `mpire-2.7.1/mpire/exception.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/signal.py` & `mpire-2.7.1/mpire/signal.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/style.css` & `mpire-2.7.1/mpire/dashboard/static/style.css`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/bootstrap.min.css` & `mpire-2.7.1/mpire/dashboard/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/refresh.js` & `mpire-2.7.1/mpire/dashboard/static/refresh.js`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg` & `mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2` & `mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff` & `mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf` & `mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot` & `mpire-2.7.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/glyphicons.css` & `mpire-2.7.1/mpire/dashboard/static/glyphicons.css`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/jquery-ui.min.js` & `mpire-2.7.1/mpire/dashboard/static/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/jquery.min.js` & `mpire-2.7.1/mpire/dashboard/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/static/bootstrap.bundle.min.js` & `mpire-2.7.1/mpire/dashboard/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/templates/progress_bar.html` & `mpire-2.7.1/mpire/dashboard/templates/progress_bar.html`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/templates/mpire.html` & `mpire-2.7.1/mpire/dashboard/templates/mpire.html`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/templates/index.html` & `mpire-2.7.1/mpire/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/dashboard.py` & `mpire-2.7.1/mpire/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/utils.py` & `mpire-2.7.1/mpire/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/connection_utils.py` & `mpire-2.7.1/mpire/dashboard/connection_utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/dashboard/manager.py` & `mpire-2.7.1/mpire/dashboard/manager.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/mpire/comms.py` & `mpire-2.7.1/mpire/comms.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/setup.py` & `mpire-2.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
         return file.read()
 
 
 if __name__ == '__main__':
     # For Python < 3.7 we need dataclasses. On Windows, we need pywin32 for CPU pinning
     setup(
         name='mpire',
-        version='2.7.0',
-        author='Slimmer AI',
+        version='2.7.1',
+        author='Sybren Jansen',
         description='A Python package for easy multiprocessing, but faster than multiprocessing',
         long_description=read_description(),
-        url='https://github.com/Slimmer-AI/mpire',
+        url='https://github.com/sybrenjansen/mpire',
         license='MIT',
         packages=find_packages(),
         scripts=['bin/mpire-dashboard'],
         install_requires=['dataclasses; python_version<"3.7"',
                           'pywin32==225; platform_system=="Windows" and python_version=="3.6"',
                           'pywin32>=301; platform_system=="Windows" and python_version>"3.6"',
                           'pygments>=2.0',
```

### Comparing `mpire-2.7.0/tests/test_signal.py` & `mpire-2.7.1/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_async_result.py` & `mpire-2.7.1/tests/test_async_result.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/utils.py` & `mpire-2.7.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_utils.py` & `mpire-2.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_insights.py` & `mpire-2.7.1/tests/test_insights.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_pool.py` & `mpire-2.7.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_params.py` & `mpire-2.7.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `mpire-2.7.0/tests/test_comms.py` & `mpire-2.7.1/tests/test_comms.py`

 * *Files identical despite different names*

