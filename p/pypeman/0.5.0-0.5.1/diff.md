# Comparing `tmp/pypeman-0.5.0.tar.gz` & `tmp/pypeman-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypeman-0.5.0.tar", last modified: Tue Jan 24 15:36:11 2023, max compression
+gzip compressed data, was "pypeman-0.5.1.tar", last modified: Fri Apr 14 14:08:17 2023, max compression
```

## Comparing `pypeman-0.5.0.tar` & `pypeman-0.5.1.tar`

### file list

```diff
@@ -1,65 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/
--rw-rw-r--   0 root         (0) root         (0)       41 2023-01-24 14:46:09.000000 pypeman-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3654 2023-01-24 15:36:11.000000 pypeman-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1928 2023-01-24 14:46:09.000000 pypeman-0.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/
--rw-rw-r--   0 root         (0) root         (0)       68 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32595 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/client/dist/
--rw-r--r--   0 root         (0) root         (0)      500 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/client/dist/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/client/dist/static/css/
--rw-r--r--   0 root         (0) root         (0)   270614 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/css/app.defc68847669cfeb2125a9467d83dbc7.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/client/dist/static/js/
--rw-r--r--   0 root         (0) root         (0)    10393 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/app.2965bd65336b53120b76.js
--rw-r--r--   0 root         (0) root         (0)    40949 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/app.2965bd65336b53120b76.js.map
--rw-r--r--   0 root         (0) root         (0)     1484 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/manifest.17bd3cecf2fcdba25f20.js
--rw-r--r--   0 root         (0) root         (0)     7803 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/manifest.17bd3cecf2fcdba25f20.js.map
--rw-r--r--   0 root         (0) root         (0)   431168 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/vendor.c74b4e5567de22bd0921.js
--rw-r--r--   0 root         (0) root         (0)  1842534 2023-01-24 15:35:44.000000 pypeman-0.5.0/pypeman/client/dist/static/js/vendor.c74b4e5567de22bd0921.js.map
--rwxrwxr-x   0 root         (0) root         (0)    12351 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/commands.py
--rw-rw-r--   0 root         (0) root         (0)     2443 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/contrib/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3606 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/csv.py
--rw-rw-r--   0 root         (0) root         (0)     2178 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/ctx.py
--rw-rw-r--   0 root         (0) root         (0)     8624 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/ftp.py
--rw-rw-r--   0 root         (0) root         (0)     6374 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/hl7.py
--rw-rw-r--   0 root         (0) root         (0)     9212 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/http.py
--rw-rw-r--   0 root         (0) root         (0)      803 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/time.py
--rw-rw-r--   0 root         (0) root         (0)      971 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/contrib/xml.py
--rw-rw-r--   0 root         (0) root         (0)     2126 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/debug.py
--rw-rw-r--   0 root         (0) root         (0)     1451 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/default_settings.py
--rw-rw-r--   0 root         (0) root         (0)     2967 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)      189 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/errors.py
--rw-rw-r--   0 root         (0) root         (0)     1395 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/events.py
--rw-rw-r--   0 root         (0) root         (0)     2577 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman/helpers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      421 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/aio_compat.py
--rw-rw-r--   0 root         (0) root         (0)     3247 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/cli.py
--rw-rw-r--   0 root         (0) root         (0)      235 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/itertools.py
--rw-rw-r--   0 root         (0) root         (0)     1894 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/lazyload.py
--rw-rw-r--   0 root         (0) root         (0)      663 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/logging.py
--rw-rw-r--   0 root         (0) root         (0)     3005 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/reloader.py
--rw-rw-r--   0 root         (0) root         (0)     1216 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/sleeper.py
--rw-rw-r--   0 root         (0) root         (0)      315 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/helpers/tempfile.py
--rw-rw-r--   0 root         (0) root         (0)     1335 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/map_item.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/message.py
--rw-rw-r--   0 root         (0) root         (0)    16408 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/msgstore.py
--rw-rw-r--   0 root         (0) root         (0)    27921 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/nodes.py
--rw-rw-r--   0 root         (0) root         (0)     3713 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/persistence.py
--rw-rw-r--   0 root         (0) root         (0)     3946 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/pjt_templates.py
--rw-rw-r--   0 root         (0) root         (0)     3008 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/plugin_mgr.py
--rw-rw-r--   0 root         (0) root         (0)    19018 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/remoteadmin.py
--rw-rw-r--   0 root         (0) root         (0)     3790 2023-01-24 14:46:09.000000 pypeman-0.5.0/pypeman/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3654 2023-01-24 15:36:10.000000 pypeman-0.5.0/pypeman.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1527 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 15:36:10.000000 pypeman-0.5.0/pypeman.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-01-24 15:36:10.000000 pypeman-0.5.0/pypeman.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-24 15:36:10.000000 pypeman-0.5.0/pypeman.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-24 15:36:11.000000 pypeman-0.5.0/pypeman.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      279 2023-01-24 15:36:11.000000 pypeman-0.5.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-01-24 14:46:09.000000 pypeman-0.5.0/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-04-14 13:27:05.000000 pypeman-0.5.1/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-04-14 13:27:05.000000 pypeman-0.5.1/MANIFEST.in
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-04-14 14:08:17.465996 pypeman-0.5.1/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-04-14 13:27:05.000000 pypeman-0.5.1/README.rst
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.461996 pypeman-0.5.1/pypeman/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    34065 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/channels.py
+-rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/commands.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/conf.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman/contrib/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/csv.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/ctx.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/ftp.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6612 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/hl7.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10057 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/http.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/time.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/xml.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/debug.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/default_settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3437 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/endpoints.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/errors.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/events.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/graph.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman/helpers/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/aio_compat.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/cli.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/itertools.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/lazyload.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/logging.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/reloader.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/sleeper.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/tempfile.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/map_item.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/message.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16408 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/msgstore.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    27977 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/persistence.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/pjt_templates.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3008 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/plugin_mgr.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19018 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/remoteadmin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/test.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman.egg-info/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1056 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/entry_points.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-04-14 14:08:17.465996 pypeman-0.5.1/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2216 2023-04-14 13:27:05.000000 pypeman-0.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pypeman-0.5.0/PKG-INFO` & `pypeman-0.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,16 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.0
+Version: 0.5.1
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
-Description: Welcome to Pypeman
-        ==================
-        
-        Pypeman is a minimalist but pragmatic ESB / ETL / EAI in python.
-        
-        .. image:: https://travis-ci.org/mhcomm/pypeman.svg?branch=master
-            :target: https://travis-ci.org/mhcomm/pypeman
-        
-        .. image:: https://badge.fury.io/py/pypeman.svg
-            :target: https://badge.fury.io/py/pypeman
-        
-        .. image:: https://codecov.io/gh/mhcomm/pypeman/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/mhcomm/pypeman
-        
-        .. image:: https://img.shields.io/badge/license-Apache%202-blue.svg
-            :target: https://raw.githubusercontent.com/mhcomm/pypeman/master/LICENSE
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        .. image:: https://img.shields.io/pypi/wheel/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        .. image:: https://img.shields.io/pypi/status/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        See `documentation <http://pypeman.readthedocs.org/en/latest/>`_ for more information.
-        
-        Getting started
-        ===============
-        
-        Installation
-        ------------
-        
-        With pip ::
-        
-            pip install pypeman # or
-            pip install pypeman[all] # To install with all optional dependencies
-        
-        Basic usage
-        -----------
-        
-        Create a fresh project with: ::
-        
-            pypeman startproject <project_dirname>
-        
-        Above command will create a new directory with a "settings.py" file containing
-        local configs and a "project.py" file with a channel example that
-        you can uncomment to test pypeman. Follow the commented instructions then execute: ::
-        
-            pypeman start # You can use the --reload option for auto-reloading on changes
-        
-        Quick command overview
-        -----------------------
-        
-        To get command help and more details about commands: ::
-        
-            pypeman --help
-        
-        To create a fresh project (partially implemented): ::
-        
-            pypeman startproject <project_name>
-        
-        To start pypeman: ::
-        
-            pypeman start
-        
-        To show a channel graph: ::
-        
-            pypeman graph
-        
-        
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -95,7 +22,80 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Programming Language :: Python
 Provides-Extra: hl7
 Provides-Extra: xml
 Provides-Extra: time
 Provides-Extra: all
+License-File: LICENSE
+
+Welcome to Pypeman
+==================
+
+Pypeman is a minimalist but pragmatic ESB / ETL / EAI in python.
+
+.. image:: https://travis-ci.org/mhcomm/pypeman.svg?branch=master
+    :target: https://travis-ci.org/mhcomm/pypeman
+
+.. image:: https://badge.fury.io/py/pypeman.svg
+    :target: https://badge.fury.io/py/pypeman
+
+.. image:: https://codecov.io/gh/mhcomm/pypeman/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/mhcomm/pypeman
+
+.. image:: https://img.shields.io/badge/license-Apache%202-blue.svg
+    :target: https://raw.githubusercontent.com/mhcomm/pypeman/master/LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+.. image:: https://img.shields.io/pypi/wheel/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+.. image:: https://img.shields.io/pypi/status/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+See `documentation <http://pypeman.readthedocs.org/en/latest/>`_ for more information.
+
+Getting started
+===============
+
+Installation
+------------
+
+With pip ::
+
+    pip install pypeman # or
+    pip install pypeman[all] # To install with all optional dependencies
+
+Basic usage
+-----------
+
+Create a fresh project with: ::
+
+    pypeman startproject <project_dirname>
+
+Above command will create a new directory with a "settings.py" file containing
+local configs and a "project.py" file with a channel example that
+you can uncomment to test pypeman. Follow the commented instructions then execute: ::
+
+    pypeman start # You can use the --reload option for auto-reloading on changes
+
+Quick command overview
+-----------------------
+
+To get command help and more details about commands: ::
+
+    pypeman --help
+
+To create a fresh project (partially implemented): ::
+
+    pypeman startproject <project_name>
+
+To start pypeman: ::
+
+    pypeman start
+
+To show a channel graph: ::
+
+    pypeman graph
+
```

### Comparing `pypeman-0.5.0/README.rst` & `pypeman-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/channels.py` & `pypeman-0.5.1/pypeman/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,22 @@
         self.interruptable_sleeper = Sleeper(loop)  # for interruptable sleeps
         self.join_nodes = None
         self.fail_nodes = None
         self.drop_nodes = None
         self.reject_nodes = None
         self.final_nodes = None
         self.wait_subchans = wait_subchans
+        self.raise_dropped = False
 
         if name:
             self.name = name
         else:
-            warnings.warn("Channels without names are deprecated", DeprecationWarning)
+            warnings.warn(
+                "Channels without names are deprecated and will be removed in version 0.5.2",
+                DeprecationWarning)
             self.name = self.__class__.__name__ + "_" + str(len(all_channels))
 
         self.parent = None
         if parent_channel:
             # Use dot name hierarchy
             self.name = ".".join([parent_channel.name, self.name])
 
@@ -170,21 +173,23 @@
         return self.status in (BaseChannel.STOPPING, BaseChannel.STOPPED,)
 
     async def start(self):
         """
         Start the channel. Called before starting processus. Can be overloaded to specify specific
         start procedure.
         """
+        self.logger.debug("Channel %s starting ...", str(self))
         self.lock = asyncio.Lock()
         self.status = BaseChannel.STARTING
         if self._first_start:
             self.init_node_graph()
             self._first_start = False
         await self.message_store.start()
         self.status = BaseChannel.WAITING
+        self.logger.info("Channel %s started", str(self))
 
     def init_node_graph(self):
         if self._nodes:
             previous_node = self._nodes[0]
 
             for node in self._nodes[1:]:
                 previous_node.next_node = node
@@ -193,26 +198,44 @@
     async def stop(self):
         """
         Stop the channel.
         Called when
         - pypeman shuts down.
         - a channel is stopped (e.g. via the admin interface)
         """
+        self.logger.debug("Channel %s stopping ...", str(self))
         self.status = BaseChannel.STOPPING
         # Verify that all messages are processed
         async with self.lock:
             self.status = BaseChannel.STOPPED
         # stop all pending sleeps
         await self.interruptable_sleeper.cancel_all()
+        self.logger.info("Channel %s stopped", str(self))
 
     def _reset_test(self):
         """ Enable test mode and reset node data.
         """
+        self.raise_dropped = True
         for node in self._nodes:
             node._reset_test()
+        if self.join_nodes:
+            for node in self.join_nodes:
+                node._reset_test()
+        if self.drop_nodes:
+            for node in self.drop_nodes:
+                node._reset_test()
+        if self.reject_nodes:
+            for node in self.reject_nodes:
+                node._reset_test()
+        if self.final_nodes:
+            for node in self.final_nodes:
+                node._reset_test()
+        if self.final_nodes:
+            for node in self.fail_nodes:
+                node._reset_test()
 
     def add(self, *args):
         """
         Add specified nodes to channel (Shortcut for append).
 
         :param args: Nodes to add.
         """
@@ -336,15 +359,15 @@
         # TODO If store fails, do we stop processing ?
         # TODO Do we store message even if channel is stopped ?
         msg_store_id = await self.message_store.store(msg)
 
         if self.status in [BaseChannel.STOPPED, BaseChannel.STOPPING]:
             raise ChannelStopped("Channel is stopped so you can't send message.")
 
-        self.logger.info("%s handle %s", self, msg)
+        self.logger.info("chan %s handle %s", str(self), str(msg))
         has_callback = hasattr(self, "_callback")
         setattr(msg, "chan_rslt", None)
         setattr(msg, "chan_exc", None)
         setattr(msg, "chan_exc_traceback", None)
         # Only one message processing at time
         async with self.lock:
             self.status = BaseChannel.PROCESSING
@@ -352,31 +375,34 @@
                 result = await self.subhandle(msg)
                 await self.message_store.change_message_state(msg_store_id, message.Message.PROCESSED)
                 msg.chan_rslt = result
                 if self.join_nodes and not has_callback:
                     await self.join_nodes[0].handle(result.copy())
                 return result
             except Dropped as exc:
+                self.logger.info("%s DROP msg %s", str(self), str(msg))
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 await self.message_store.change_message_state(msg_store_id, message.Message.PROCESSED)
                 if self.drop_nodes and not has_callback:
                     await self.drop_nodes[0].handle(msg.copy())
-                raise
+                if self.raise_dropped:
+                    raise
             except Rejected as exc:
+                self.logger.info("%s REJECT msg %s", str(self), str(msg))
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 await self.message_store.change_message_state(msg_store_id, message.Message.REJECTED)
                 if self.reject_nodes and not has_callback:
                     await self.reject_nodes[0].handle(msg.copy())
                 raise
             except Exception as exc:
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
-                self.logger.exception('Error while processing message %s', msg)
+                self.logger.exception('Error while processing message %s (chan %s)', str(msg), str(self))
                 await self.message_store.change_message_state(msg_store_id, message.Message.ERROR)
                 if self.fail_nodes and not has_callback:
                     await self.fail_nodes[0].handle(msg.copy())
                 raise
             finally:
                 self.status = BaseChannel.WAITING
                 self.processed_msgs += 1
@@ -391,14 +417,15 @@
                 finally:
                     if self.sub_chan_endnodes:
                         # Launch and wait for sub chans callbacks
                         subchan_endnodes_fut = asyncio.gather(*self.sub_chan_endnodes)
                         subchan_endnodes_fut.add_done_callback(self._reset_sub_chan_endnodes)
                         if self.wait_subchans:
                             await subchan_endnodes_fut
+                    self.logger.info("%s end handle %s", str(self), str(msg))
 
     async def subhandle(self, msg):
         """ Overload this method only if you know what you are doing. Called by ``handle`` method.
 
         :param msg: To be processed msg.
 
         :return: Processed message
@@ -439,15 +466,15 @@
         """
         This method allows you to replay a message from channel `message_store`.
 
         :param msg_id: Message id to replay.
 
         :return: The result of the processing.
         """
-        logger.info("try to replay %s", str(msg_id))
+        self.logger.info("try to replay %s", str(msg_id))
         msg_dict = await self.message_store.get(msg_id)
         new_message = msg_dict['message'].renew()
         result = await self.handle(new_message)
         return result
 
     def to_dict(self):
         return {
@@ -653,44 +680,49 @@
         endnodes_tasks = []
         try:
             result = fut.result()
             entrymsg.chan_rslt = result
             if self.join_nodes:
                 endnode_task = asyncio.create_task(self.join_nodes[0].handle(result.copy()))
                 endnodes_tasks.append(endnode_task)
-            logger.info("Subchannel %s end process message %s", repr(self), result)
+            logger.info(
+                "Subchannel %s end process message %s, rslt is msg %s",
+                str(self), str(entrymsg), str(result))
         except Dropped as exc:
             entrymsg.chan_exc = exc
             entrymsg.chan_exc_traceback = traceback.format_exc()
             if self.drop_nodes:
                 endnode_task = asyncio.create_task(self.drop_nodes[0].handle(entrymsg.copy()))
                 endnodes_tasks.append(endnode_task)
-            self.logger.info("Subchannel %s. Msg was dropped", repr(self))
+            self.logger.info("Subchannel %s. Msg %s was dropped", str(self), str(entrymsg))
         except Rejected as exc:
             entrymsg.chan_exc = exc
             entrymsg.chan_exc_traceback = traceback.format_exc()
             if self.reject_nodes:
                 endnode_task = asyncio.create_task(self.reject_nodes[0].handle(entrymsg.copy()))
                 endnodes_tasks.append(endnode_task)
-            self.logger.info("Subchannel %s. Msg was Rejected", repr(self))
+            self.logger.info("Subchannel %s. Msg %s was Rejected", str(self), str(entrymsg))
             raise
         except Exception as exc:
             entrymsg.chan_exc = exc
             entrymsg.chan_exc_traceback = traceback.format_exc()
             if self.fail_nodes:
                 endnode_task = asyncio.create_task(self.fail_nodes[0].handle(entrymsg.copy()))
                 endnodes_tasks.append(endnode_task)
-            self.logger.exception("Error while processing msg in subchannel %s", self)
+            self.logger.exception(
+                "Error while processing msg %s in subchannel %s", str(entrymsg), str(self))
             raise
         finally:
             if self.final_nodes:
                 endnode_task = asyncio.create_task(self.final_nodes[0].handle(entrymsg.copy()))
                 endnodes_tasks.append(endnode_task)
             self.parent.sub_chan_endnodes.extend(endnodes_tasks)
             self.parent.sub_chan_tasks.remove(fut)
+            self.logger.info(
+                "subchan %s end process msg %s", str(self), str(entrymsg))
 
     async def process(self, msg):
         if self._nodes:
             msgctxvartoken = MSG_CTXVAR.set(msg.copy())
             ctx = contextvars.copy_context()
             fut = asyncio.create_task(self._nodes[0].handle(msg.copy()))
             fut.add_done_callback(self._callback, context=ctx)
```

### Comparing `pypeman-0.5.0/pypeman/commands.py` & `pypeman-0.5.1/pypeman/commands.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/conf.py` & `pypeman-0.5.1/pypeman/conf.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/contrib/csv.py` & `pypeman-0.5.1/pypeman/contrib/csv.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/contrib/ctx.py` & `pypeman-0.5.1/pypeman/contrib/ctx.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/contrib/ftp.py` & `pypeman-0.5.1/pypeman/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/contrib/hl7.py` & `pypeman-0.5.1/pypeman/contrib/hl7.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import asyncio
+import logging
 import sys
 
 import warnings
 
 import hl7
 
 from pypeman import endpoints, channels, nodes, message
 from pypeman.errors import PypemanParamError
 
 
+logger = logging.getLogger(__name__)
+
+
 class MLLPProtocol(asyncio.Protocol):
     """
     Minimal Lower-Layer Protocol (MLLP) takes the form:
         <VT>[HL7 Message]<FS><CR>
 
     References:
         - http://www.hl7standards.com/blog/2007/05/02/hl7-mlp-minimum-layer-protocol-defined/
@@ -53,48 +57,49 @@
 
         for raw_message in messages:
             # strip the rest of the MLLP shell from the HL7 message
             raw_message = raw_message.strip(self.start_block + self.carriage_return)
 
             # only pass messages with data
             if len(raw_message) > 0:
-                result = asyncio.create_task(self.handler(raw_message), loop=self.loop)
+                result = asyncio.create_task(self.handler(raw_message))
                 result.add_done_callback(self.process_response)
 
     def writeMessage(self, message):
         # convert back to a byte string
         # wrap message in payload container
         self.transport.write(self.start_block + message + self.end_block + self.carriage_return)
 
     def connection_lost(self, exc):
         """
         Called when the connection is lost or closed.
         The argument is an exception object or None (the latter
         meaning a regular EOF is received or the connection was
         aborted or closed).
         """
+        logger.info("MLLP: connection lost (exc=%s)", repr(exc))
         super().connection_lost(exc)
 
 
 class MLLPEndpoint(endpoints.SocketEndpoint):
 
     def __init__(
             self,
             address=None, port=None,  # obsolete params
             encoding='utf-8',
             loop=None,
             host=None,
             sock=None,
             reuse_port=None,
             ):
-
         self.handlers = []
         self.address = address
         self.port = port
         self.loop = loop or asyncio.get_event_loop()
+        self.handler = None
         if address or port:
             warnings.warn(
                 "HTTPEndpoint 'address', 'adress' and 'port' params are deprecated. "
                 "Replace it by 'host' or 'sock'", DeprecationWarning)
             if host or sock:
                 raise PypemanParamError(
                     "Obsolete params ('adress', 'address', 'port') "
@@ -116,18 +121,18 @@
     async def start(self):
         self.make_socket()
         if self.handler:
             srv = await self.loop.create_server(
                 protocol_factory=lambda: MLLPProtocol(self.handler, loop=self.loop),
                 sock=self.sock_obj,
             )
-            print("MLLP server started at http://{}:{}".format(self.address, self.port))
+            logger.debug("MLLP server started at %s", repr(self.sock))
             return srv
         else:
-            print("No MLLP handlers.")
+            logger.error("No MLLP handlers.")
 
 
 class MLLPChannel(channels.BaseChannel):
 
     def __init__(self, *args, endpoint=None, encoding='utf-8', **kwargs):
         super().__init__(*args, **kwargs)
         if endpoint is None:
@@ -151,14 +156,16 @@
         except channels.Dropped:
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AA')).encode(self.encoding)
         except channels.Rejected:
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AR')).encode(self.encoding)
         except Exception:
+            logger.exception(
+                "MLLPChannel %s raise an error, will send AE speed response", str(self))
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AE')).encode(self.encoding)
 
 
 class HL7ToPython(nodes.BaseNode):
     """ Convert hl7 payload to python struct."""
```

### Comparing `pypeman-0.5.0/pypeman/contrib/http.py` & `pypeman-0.5.1/pypeman/contrib/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,16 +122,19 @@
         try:
             result = await self.handle(msg)
             encoding = self.encoding or 'utf-8'
             return web.Response(body=result.payload.encode(encoding), status=result.meta.get('status', 200))
 
         except channels.Dropped:
             return web.Response(body="Dropped".encode('utf-8'), status=200)
-        except Exception as e:
-            return web.Response(body=str(e).encode('utf-8'), status=503)
+        except Exception as exc:
+            logger.exception(
+                "HttpChannel %s raise an error, cannot send 200 speed response, will return 503",
+                str(self))
+            return web.Response(body=str(exc).encode('utf-8'), status=503)
 
 
 class HttpRequest(nodes.BaseNode):
     """
         Http request node
         :param url: url to send.
         :param method: 'get', 'put' or 'post', use meta['method'] if None, Default to 'get'.
@@ -139,32 +142,36 @@
         :param cookies: cookies for request, use meta.get('cookies') if None.
         :param auth: tuple or aiohttp.BasicAuth object.
         :param verify: verify ssl. Default True.
         :param params: get params in dict. List for multiple elements, ex :
                        {'param1': 'omega', param2: ['alpha', 'beta']}
         :param client_cert: tuple with .crt and .key path
         :param binary: bool, Get response content as bytes
+        :param send_as_json: bool, If the method is a PATCH/POST/PUT, send data as json
+        :param json: bool, Parse Json response content
+        # TODO maybe add an auto parser if for example Content-Type header is application/json
     """
 
     def __init__(self, url, *args, method=None, headers=None, auth=None,
                  verify=True, params=None, client_cert=None, cookies=None,
-                 binary=False, json=False, **kwargs):
+                 binary=False, json=False, send_as_json=False, **kwargs):
         super().__init__(*args, **kwargs)
         self.url = url
         self.method = method
         self.headers = headers
         self.cookies = cookies
         self.auth = auth
         self.verify = verify
         self.params = params
         self.client_cert = client_cert
         self.url = self.url.replace('%(meta.', '%(')
         self.payload_in_url_dict = 'payload.' in self.url
         self.binary = binary
         self.json = json
+        self.send_as_json = send_as_json
         # TODO: create used payload keys for better perf of generate_request_url()
 
     def generate_request_url(self, msg):
         url_dict = msg.meta
         if self.payload_in_url_dict:
             url_dict = dict(url_dict)
             try:
@@ -218,22 +225,32 @@
         else:
             basic_auth = self.auth
 
         data = None
         if method.lower() in ['put', 'post']:
             data = msg.payload
         async with aiohttp.ClientSession(connector=conn, cookies=cookies) as session:
-            resp = await session.request(
-                    method=method,
-                    url=url,
-                    auth=basic_auth,
-                    headers=headers,
-                    params=get_params,
-                    data=data
-                    )
+            if self.send_as_json:
+                resp = await session.request(
+                        method=method,
+                        url=url,
+                        auth=basic_auth,
+                        headers=headers,
+                        params=get_params,
+                        json=data
+                        )
+            else:
+                resp = await session.request(
+                        method=method,
+                        url=url,
+                        auth=basic_auth,
+                        headers=headers,
+                        params=get_params,
+                        data=data
+                        )
             if self.binary:
                 resp_content = await resp.read()
             else:
                 resp_content = str(await resp.text())
             if self.json:
                 try:
                     resp_content = json.loads(resp_content)
```

### Comparing `pypeman-0.5.0/pypeman/contrib/time.py` & `pypeman-0.5.1/pypeman/contrib/time.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/contrib/xml.py` & `pypeman-0.5.1/pypeman/contrib/xml.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/debug.py` & `pypeman-0.5.1/pypeman/debug.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/default_settings.py` & `pypeman-0.5.1/pypeman/default_settings.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/endpoints.py` & `pypeman-0.5.1/pypeman/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
     def __init__(self):
         all_endpoints.append(self)
 
     async def start(self):
         pass
 
+    async def stop(self):
+        pass
+
 
 class SocketEndpoint(BaseEndpoint):
     def __init__(self, loop=None, sock=None, default_port='8080', reuse_port=None):
         """
             :param reuse_port: bool if true then the listening port specified in the url parameter)
                 will be shared with other processes on same port
                 no effect with bound socket object
@@ -37,14 +40,15 @@
                 or bound socket object
         """
         super().__init__()
         self.loop = loop or asyncio.get_event_loop()
         self.reuse_port = reuse_port
 
         self.sock = self.normalize_socket(sock, default_port=default_port)
+        self.sock_obj = None
 
     @staticmethod
     def normalize_socket(sock, default_port="8080"):
         if isinstance(sock, str):
             if not sock.startswith('unix:'):
                 if ':' not in sock:
                     sock += ':'
@@ -57,43 +61,51 @@
     @staticmethod
     def mk_socket(sock, reuse_port):
         """
             make, bind and return socket if string object is passed
             if not return sock as is
         """
         if isinstance(sock, str):
+            logger.debug("trying to create socket %s", sock)
             if not sock.startswith('unix:'):
                 try:
                     host, port = sock.split(":")
                     port = int(port)
                     if not host:
                         raise
                     bind_param = (host, port)
                 except Exception:
                     logger.exception('error on sock params in socket endpoint')
                     raise
                 sock_obj = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                sock_obj.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             else:
                 bind_param = sock.split(":", 1)[1]
                 sock_obj = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             if reuse_port:
                 SO_REUSEPORT = 15
                 sock_obj.setsockopt(socket.SOL_SOCKET, SO_REUSEPORT, 1)
             sock_obj.bind(bind_param)
+            logger.debug("socket %s created and binded", sock)
         else:
+            logger.debug("no socket to create, keeping socket %s", repr(sock))
             sock_obj = sock
-
         return sock_obj
 
     def make_socket(self):
         """
             make and bind socket if string object is passed
         """
         self.sock_obj = self.mk_socket(self.sock, self.reuse_port)
 
+    async def stop(self):
+        if self.sock_obj:
+            self.sock_obj.close()
+            self.sock_obj = None
+
 
 from pypeman.helpers import lazyload  # noqa: E402
 
 wrap = lazyload.Wrapper(__name__)
 
 wrap.add_lazy('pypeman.contrib.http', 'HTTPEndpoint', ['aiohttp'])
```

### Comparing `pypeman-0.5.0/pypeman/events.py` & `pypeman-0.5.1/pypeman/events.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/graph.py` & `pypeman-0.5.1/pypeman/graph.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/helpers/cli.py` & `pypeman-0.5.1/pypeman/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/helpers/lazyload.py` & `pypeman-0.5.1/pypeman/helpers/lazyload.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/helpers/logging.py` & `pypeman-0.5.1/pypeman/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/helpers/reloader.py` & `pypeman-0.5.1/pypeman/helpers/reloader.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/helpers/sleeper.py` & `pypeman-0.5.1/pypeman/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/map_item.py` & `pypeman-0.5.1/pypeman/map_item.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/message.py` & `pypeman-0.5.1/pypeman/message.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/msgstore.py` & `pypeman-0.5.1/pypeman/msgstore.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/nodes.py` & `pypeman-0.5.1/pypeman/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,18 @@
             result = self.run(msg)
 
         self.processed += 1
 
         if isinstance(result, asyncio.Future):
             result = await result
 
+        self.channel.logger.debug(
+            '%s node end handle msg %s, result is msg %s',
+            str(self), str(msg), str(result))
+
         if self.next_node:
             if isinstance(result, types.GeneratorType):
                 gene = result
                 result = msg  # Necessary if all nodes result are dropped
                 for res in gene:
                     try:
                         result = await self.next_node.handle(res)
@@ -199,16 +203,14 @@
 
     async def _log_handle(self, msg):
         """
         Used when node logging is enabled. Log after node processing.
         """
         result = await self._handle_without_log(msg)
 
-        self.channel.logger.info('%s node from handles %s', str(self), str(result))
-
         # Log message
         result.log(logger=self.channel.logger, log_level=logging.DEBUG)
 
         return result
 
     async def _test_handle(self, msg):
         """ Specific handle for TEST mode to enable some testing and introspection operations
```

### Comparing `pypeman-0.5.0/pypeman/persistence.py` & `pypeman-0.5.1/pypeman/persistence.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/pjt_templates.py` & `pypeman-0.5.1/pypeman/pjt_templates.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/plugin_mgr.py` & `pypeman-0.5.1/pypeman/plugin_mgr.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/remoteadmin.py` & `pypeman-0.5.1/pypeman/remoteadmin.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman/test.py` & `pypeman-0.5.1/pypeman/test.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.0/pypeman.egg-info/PKG-INFO` & `pypeman-0.5.1/pypeman.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,16 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.0
+Version: 0.5.1
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
-Description: Welcome to Pypeman
-        ==================
-        
-        Pypeman is a minimalist but pragmatic ESB / ETL / EAI in python.
-        
-        .. image:: https://travis-ci.org/mhcomm/pypeman.svg?branch=master
-            :target: https://travis-ci.org/mhcomm/pypeman
-        
-        .. image:: https://badge.fury.io/py/pypeman.svg
-            :target: https://badge.fury.io/py/pypeman
-        
-        .. image:: https://codecov.io/gh/mhcomm/pypeman/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/mhcomm/pypeman
-        
-        .. image:: https://img.shields.io/badge/license-Apache%202-blue.svg
-            :target: https://raw.githubusercontent.com/mhcomm/pypeman/master/LICENSE
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        .. image:: https://img.shields.io/pypi/wheel/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        .. image:: https://img.shields.io/pypi/status/pypeman.svg
-            :target: http://pypeman.readthedocs.org/en/latest/
-        
-        See `documentation <http://pypeman.readthedocs.org/en/latest/>`_ for more information.
-        
-        Getting started
-        ===============
-        
-        Installation
-        ------------
-        
-        With pip ::
-        
-            pip install pypeman # or
-            pip install pypeman[all] # To install with all optional dependencies
-        
-        Basic usage
-        -----------
-        
-        Create a fresh project with: ::
-        
-            pypeman startproject <project_dirname>
-        
-        Above command will create a new directory with a "settings.py" file containing
-        local configs and a "project.py" file with a channel example that
-        you can uncomment to test pypeman. Follow the commented instructions then execute: ::
-        
-            pypeman start # You can use the --reload option for auto-reloading on changes
-        
-        Quick command overview
-        -----------------------
-        
-        To get command help and more details about commands: ::
-        
-            pypeman --help
-        
-        To create a fresh project (partially implemented): ::
-        
-            pypeman startproject <project_name>
-        
-        To start pypeman: ::
-        
-            pypeman start
-        
-        To show a channel graph: ::
-        
-            pypeman graph
-        
-        
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -95,7 +22,80 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Programming Language :: Python
 Provides-Extra: hl7
 Provides-Extra: xml
 Provides-Extra: time
 Provides-Extra: all
+License-File: LICENSE
+
+Welcome to Pypeman
+==================
+
+Pypeman is a minimalist but pragmatic ESB / ETL / EAI in python.
+
+.. image:: https://travis-ci.org/mhcomm/pypeman.svg?branch=master
+    :target: https://travis-ci.org/mhcomm/pypeman
+
+.. image:: https://badge.fury.io/py/pypeman.svg
+    :target: https://badge.fury.io/py/pypeman
+
+.. image:: https://codecov.io/gh/mhcomm/pypeman/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/mhcomm/pypeman
+
+.. image:: https://img.shields.io/badge/license-Apache%202-blue.svg
+    :target: https://raw.githubusercontent.com/mhcomm/pypeman/master/LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+.. image:: https://img.shields.io/pypi/wheel/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+.. image:: https://img.shields.io/pypi/status/pypeman.svg
+    :target: http://pypeman.readthedocs.org/en/latest/
+
+See `documentation <http://pypeman.readthedocs.org/en/latest/>`_ for more information.
+
+Getting started
+===============
+
+Installation
+------------
+
+With pip ::
+
+    pip install pypeman # or
+    pip install pypeman[all] # To install with all optional dependencies
+
+Basic usage
+-----------
+
+Create a fresh project with: ::
+
+    pypeman startproject <project_dirname>
+
+Above command will create a new directory with a "settings.py" file containing
+local configs and a "project.py" file with a channel example that
+you can uncomment to test pypeman. Follow the commented instructions then execute: ::
+
+    pypeman start # You can use the --reload option for auto-reloading on changes
+
+Quick command overview
+-----------------------
+
+To get command help and more details about commands: ::
+
+    pypeman --help
+
+To create a fresh project (partially implemented): ::
+
+    pypeman startproject <project_name>
+
+To start pypeman: ::
+
+    pypeman start
+
+To show a channel graph: ::
+
+    pypeman graph
+
```

### Comparing `pypeman-0.5.0/pypeman.egg-info/SOURCES.txt` & `pypeman-0.5.1/pypeman.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 pypeman/__init__.py
 pypeman/channels.py
 pypeman/commands.py
@@ -23,22 +24,14 @@
 pypeman/test.py
 pypeman.egg-info/PKG-INFO
 pypeman.egg-info/SOURCES.txt
 pypeman.egg-info/dependency_links.txt
 pypeman.egg-info/entry_points.txt
 pypeman.egg-info/requires.txt
 pypeman.egg-info/top_level.txt
-pypeman/client/dist/index.html
-pypeman/client/dist/static/css/app.defc68847669cfeb2125a9467d83dbc7.css
-pypeman/client/dist/static/js/app.2965bd65336b53120b76.js
-pypeman/client/dist/static/js/app.2965bd65336b53120b76.js.map
-pypeman/client/dist/static/js/manifest.17bd3cecf2fcdba25f20.js
-pypeman/client/dist/static/js/manifest.17bd3cecf2fcdba25f20.js.map
-pypeman/client/dist/static/js/vendor.c74b4e5567de22bd0921.js
-pypeman/client/dist/static/js/vendor.c74b4e5567de22bd0921.js.map
 pypeman/contrib/__init__.py
 pypeman/contrib/csv.py
 pypeman/contrib/ctx.py
 pypeman/contrib/ftp.py
 pypeman/contrib/hl7.py
 pypeman/contrib/http.py
 pypeman/contrib/time.py
```

### Comparing `pypeman-0.5.0/setup.py` & `pypeman-0.5.1/setup.py`

 * *Files identical despite different names*

