# Comparing `tmp/murfey-0.7.6.tar.gz` & `tmp/murfey-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.7.6.tar", last modified: Tue Apr 11 12:43:24 2023, max compression
+gzip compressed data, was "murfey-0.7.7.tar", last modified: Fri Apr 14 14:47:34 2023, max compression
```

## Comparing `murfey-0.7.6.tar` & `murfey-0.7.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-11 12:43:14.000000 murfey-0.7.6/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-11 12:43:14.000000 murfey-0.7.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 12:43:24.633490 murfey-0.7.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-11 12:43:14.000000 murfey-0.7.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-11 12:43:14.000000 murfey-0.7.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-11 12:43:24.633490 murfey-0.7.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-11 12:43:14.000000 murfey-0.7.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.617489 murfey-0.7.6/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    10515 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12051 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    46554 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7814 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18326 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4475 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21322 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (122)    17869 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16460 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11248 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3518 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-14 14:47:27.000000 murfey-0.7.7/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-14 14:47:27.000000 murfey-0.7.7/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-14 14:47:34.259859 murfey-0.7.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-14 14:47:27.000000 murfey-0.7.7/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-14 14:47:27.000000 murfey-0.7.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-14 14:47:34.259859 murfey-0.7.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-14 14:47:27.000000 murfey-0.7.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.247859 murfey-0.7.7/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10265 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12051 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    45471 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7058 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19403 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5094 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26660 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (122)    17866 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18289 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11850 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3682 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.7.6/LICENSE` & `murfey-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/PKG-INFO` & `murfey-0.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.6
+Version: 0.7.7
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.6/README.md` & `murfey-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/setup.cfg` & `murfey-0.7.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.7.6
+version = 0.7.7
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `murfey-0.7.6/src/murfey/bootstrap/__main__.py` & `murfey-0.7.7/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/cli/dummy.py` & `murfey-0.7.7/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/cli/transfer.py` & `murfey-0.7.7/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/__init__.py` & `murfey-0.7.7/src/murfey/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from rich.prompt import Confirm
 
 import murfey.client.rsync
 import murfey.client.update
 import murfey.client.watchdir
 import murfey.client.websocket
 from murfey.client.customlogging import CustomHandler, DirectableRichHandler
-from murfey.client.gain_ref import determine_gain_ref
 from murfey.client.instance_environment import MurfeyInstanceEnvironment
 from murfey.client.tui.app import MurfeyTUI
 from murfey.client.tui.status_bar import StatusBar
 from murfey.util import _get_visit_list
 
 # from asyncio import Queue
 
@@ -244,19 +243,14 @@
 
     log.info("Starting Websocket connection")
 
     status_bar = StatusBar()
 
     machine_data = requests.get(f"{murfey_url.geturl()}/machine/").json()
     gain_ref: Path | None = None
-    if machine_data.get("gain_reference_directory"):
-        try:
-            gain_ref = determine_gain_ref(machine_data["gain_reference_directory"])
-        except RuntimeError:
-            pass
 
     instance_environment = MurfeyInstanceEnvironment(
         url=murfey_url,
         software_versions=machine_data.get("software_versions", {}),
         # sources=[Path(args.source)],
         # watchers=source_watchers,
         default_destination=args.destination
```

### Comparing `murfey-0.7.6/src/murfey/client/analyser.py` & `murfey-0.7.7/src/murfey/client/analyser.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/context.py` & `murfey-0.7.7/src/murfey/client/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,22 @@
         ProcessingParameter(
             "mask_diameter", "Mask Diameter (2D classification)", default=190
         ),
         ProcessingParameter("downscale", "Downscale Extracted Particles", default=True),
         ProcessingParameter(
             "small_boxsize", "Downscaled Extracted Particle Size (pixels)", default=128
         ),
+        ProcessingParameter(
+            "estimate_particle_diameter",
+            "Use crYOLO to Estimate Particle Diameter",
+            default=True,
+        ),
+        ProcessingParameter(
+            "particle_diameter", "Particle Diameter (Angstroms)", default=0
+        ),
     ]
     metadata_params = [
         ProcessingParameter("voltage", "Voltage"),
         ProcessingParameter("image_size_x", "Image Size X"),
         ProcessingParameter("image_size_y", "Image Size Y"),
         ProcessingParameter("pixel_size_on_image", "Pixel Size"),
         ProcessingParameter("motion_corr_binning", "Motion Correction Binning"),
@@ -106,63 +114,23 @@
 
     def __init__(self, acquisition_software: str, basepath: Path):
         super().__init__(acquisition_software)
         self._basepath = basepath
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
 
-    def _flush_processing_job(
-        self,
-        tag: str,
-        environment: MurfeyInstanceEnvironment,
-        parameters: Dict[str, Any] | None = None,
-    ):
-        if parameters:
-            proc_job_future = self._processing_job_stash[tag]
-            machine_config = get_machine_config(
-                str(environment.url.geturl()), demo=environment.demo
-            )
-            image_directory = str(
-                Path(machine_config.get("rsync_basepath", "."))
-                / environment.default_destinations[Path(tag)]
-            )
-            if self._acquisition_software == "epu":
-                import_images = f"{Path(image_directory).resolve()}/GridSquare*/Data/*{parameters['file_extension']}"
-            else:
-                import_images = (
-                    f"{Path(image_directory).resolve()}/*{parameters['file_extension']}"
-                )
-            msg = {
-                **proc_job_future.message,
-                "parameters": {
-                    "acquisition_software": parameters["acquisition_software"],
-                    "voltage": parameters["voltage"],
-                    "motioncor_gainreference": parameters["gain_ref"],
-                    "motioncor_doseperframe": parameters["dose_per_frame"],
-                    "eer_grouping": parameters["eer_grouping"],
-                    "import_images": import_images,
-                    "angpix": parameters["pixel_size_on_image"],
-                    "symmetry": parameters["symmetry"],
-                    "extract_boxsize": parameters["boxsize"],
-                    "extract_downscale": parameters["downscale"],
-                    "extract_small_boxsize": parameters["small_boxsize"],
-                    "mask_diameter": parameters["mask_diameter"],
-                    "autopick_do_cryolo": parameters["use_cryolo"],
-                },
-            }
-            requests.post(proc_job_future.url, json=msg)
-
     def _register_data_collection(
         self,
         tag: str,
         url: str,
         data: dict,
         environment: MurfeyInstanceEnvironment,
     ):
         logger.info(f"registering data collection with data {data}")
+        environment.id_tag_registry["data_collection"].append(tag)
         machine_config = get_machine_config(
             str(environment.url.geturl()), demo=environment.demo
         )
         image_directory = str(
             Path(machine_config.get("rsync_basepath", "."))
             / environment.default_destinations[Path(tag)]
         )
@@ -189,69 +157,71 @@
     def post_transfer(
         self,
         transferred_file: Path,
         role: str = "",
         environment: MurfeyInstanceEnvironment | None = None,
         **kwargs,
     ):
-        if role == "detector" and environment:
-            source = ""
-            for s in environment.sources:
-                if transferred_file.is_relative_to(s):
-                    source = str(s)
-                    break
-            proc_url = f"{str(environment.url.geturl())}/visits/{environment.visit}/register_processing_job"
-            if environment.data_collection_ids.get(source) is None:
-                self._processing_job_stash[source] = FutureRequest(
-                    proc_url,
-                    {"tag": source, "recipe": "ispyb-relion"},
-                )
-            elif environment.data_collection_parameters:
-                if self._processing_job_stash.get(source):
-                    # self._flush_processing_job(source)
-                    pass
-                requests.post(
-                    proc_url,
-                    json={
-                        "tag": source,
-                        "recipe": "ispyb-relion",
-                        "parameters": environment.data_collection_parameters,
-                    },
-                )
+        return
 
     def _register_processing_job(
         self,
         tag: str,
         environment: MurfeyInstanceEnvironment,
         parameters: Dict[str, Any] | None = None,
     ):
         logger.info(f"registering processing job with parameters: {parameters}")
+        parameters = parameters or {}
+        environment.id_tag_registry["processing_job"].append(tag)
+        proc_url = f"{str(environment.url.geturl())}/visits/{environment.visit}/register_processing_job"
         machine_config = get_machine_config(
             str(environment.url.geturl()), demo=environment.demo
         )
         image_directory = str(
             Path(machine_config.get("rsync_basepath", "."))
             / environment.default_destinations[Path(tag)]
         )
-        if self._processing_job_stash.get(tag):
-            params = {
-                "tag": tag,
-                "source": tag,
-                "image_directory": image_directory,
-            }
-            if parameters:
-                params.update(parameters)
-            self._flush_processing_job(
-                tag,
-                environment,
-                parameters=params,
+        if self._acquisition_software == "epu":
+            import_images = f"{Path(image_directory).resolve()}/GridSquare*/Data/*{parameters['file_extension']}"
+        else:
+            import_images = (
+                f"{Path(image_directory).resolve()}/*{parameters['file_extension']}"
             )
-            self._processing_job_stash.pop(tag)
+        msg: Dict[str, Any] = {
+            "tag": tag,
+            "recipe": "ispyb-relion",
+            "parameters": {
+                "acquisition_software": parameters["acquisition_software"],
+                "voltage": parameters["voltage"],
+                "motioncor_gainreference": parameters["gain_ref"],
+                "motioncor_doseperframe": parameters["dose_per_frame"],
+                "eer_grouping": parameters["eer_grouping"],
+                "import_images": import_images,
+                "angpix": parameters["pixel_size_on_image"] * 1e10,
+                "symmetry": parameters["symmetry"],
+                "extract_boxsize": parameters["boxsize"],
+                "extract_downscale": parameters["downscale"],
+                "extract_small_boxsize": parameters["small_boxsize"],
+                "mask_diameter": parameters["mask_diameter"],
+                "autopick_do_cryolo": parameters["use_cryolo"],
+                "estimate_particle_diameter": parameters["estimate_particle_diameter"],
+            },
+        }
+        if parameters["particle_diameter"]:
+            msg["parameters"]["particle_diameter"] = parameters["particle_diameter"]
+        requests.post(proc_url, json=msg)
 
-    def _launch_spa_pipeline(self, tag: str, jobid: int, url: str = ""):
+    def _launch_spa_pipeline(
+        self,
+        tag: str,
+        jobid: int,
+        environment: MurfeyInstanceEnvironment,
+        url: str = "",
+    ):
+        environment.id_tag_registry["auto_proc_program"].append(tag)
         data = {"job_id": jobid}
         requests.post(url, json=data)
 
     def gather_metadata(
         self, metadata_file: Path, environment: MurfeyInstanceEnvironment | None = None
     ):
         if metadata_file.suffix != ".xml":
@@ -366,14 +336,16 @@
         metadata["symmetry"] = TUIFormValue("C1")
         metadata["mask_diameter"] = TUIFormValue(190)
         metadata["boxsize"] = TUIFormValue(256)
         metadata["downscale"] = TUIFormValue(False)
         metadata["small_boxsize"] = TUIFormValue(128)
         metadata["eer_grouping"] = TUIFormValue(20)
         metadata["source"] = TUIFormValue(str(self._basepath))
+        metadata["particle_diameter"] = TUIFormValue(0)
+        metadata["estimate_particle_diameter"] = TUIFormValue(True)
         metadata.move_to_end("gain_ref", last=False)
         metadata.move_to_end("dose_per_frame", last=False)
         return metadata
 
 
 class ProcessFileIncomplete(BaseModel):
     dest: Path
@@ -385,15 +357,15 @@
 
 
 class TomographyContext(Context):
     user_params = [
         ProcessingParameter(
             "dose_per_frame", "Dose Per Frame (e- / Angstrom^2 / frame)"
         ),
-        ProcessingParameter("tilt_offset", "Tilt Offset"),
+        ProcessingParameter("manual_tilt_offset", "Tilt Offset"),
     ]
     metadata_params = [
         ProcessingParameter("voltage", "Voltage"),
         ProcessingParameter("image_size_x", "Image Size X"),
         ProcessingParameter("image_size_y", "Image Size Y"),
         ProcessingParameter("pixel_size_on_image", "Pixel Size"),
         ProcessingParameter("motion_corr_binning", "Motion Correction Binning"),
```

### Comparing `murfey-0.7.6/src/murfey/client/contexts/tomo.py` & `murfey-0.7.7/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/customlogging.py` & `murfey-0.7.7/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/gain_ref.py` & `murfey-0.7.7/src/murfey/client/gain_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 
 def determine_gain_ref(gain_ref_dir: Path) -> Path:
-    candidates = list(gain_ref_dir.glob("*"))
+    candidates = list(gain_ref_dir.glob("**/*"))
     candidates = sorted(candidates, key=lambda x: x.stat().st_mtime, reverse=True)
     viable_candidates = candidates[:3]
     viable_candidates = sorted(
         viable_candidates, key=lambda x: x.stat().st_size, reverse=True
     )
     if viable_candidates:
         return viable_candidates[0]
```

### Comparing `murfey-0.7.6/src/murfey/client/instance_environment.py` & `murfey-0.7.7/src/murfey/client/instance_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,20 @@
     destination_registry: Dict[str, str] = {}
     watchers: Dict[Path, DirWatcher] = {}
     demo: bool = False
     data_collection_group_ids: Dict[str, int] = {}
     data_collection_ids: Dict[str, int] = {}
     processing_job_ids: Dict[str, Dict[str, int]] = {}
     autoproc_program_ids: Dict[str, Dict[str, int]] = {}
+    id_tag_registry: Dict[str, List[str]] = {
+        "data_collection_group": [],
+        "data_collection": [],
+        "processing_job": [],
+        "auto_proc_program": [],
+    }
     data_collection_parameters: dict = {}
     movies: Dict[Path, MovieTracker] = {}
     motion_corrected_movies: Dict[Path, List[str]] = {}
     listeners: Dict[str, Set[Callable]] = {}
     movie_tilt_pair: Dict[Path, str] = {}
     tilt_angles: Dict[str, List[List[str]]] = {}
     visit: str = ""
@@ -70,79 +76,59 @@
         self.visit = ""
         self.gain_ref = None
 
     @validator("data_collection_group_ids")
     def dcg_callback(cls, v, values):
         with global_env_lock:
             for l in values.get("listeners", {}).get("data_collection_group_ids", []):
-                if values.get("data_collection_group_ids"):
-                    for k in set(values["data_collection_group_ids"].keys()) ^ set(
-                        v.keys()
-                    ):
-                        l(k)
-                else:
-                    for k in v.keys():
+                for k in v.keys():
+                    if k not in values["id_tag_registry"]["data_collection"]:
                         l(k)
         return v
 
     @validator("data_collection_ids")
     def dc_callback(cls, v, values):
         with global_env_lock:
             for l in values.get("listeners", {}).get("data_collection_ids", []):
-                if values.get("data_collection_ids"):
-                    for k in set(values["data_collection_ids"].keys()) ^ set(v.keys()):
-                        l(k)
-                else:
-                    for k in v.keys():
+                for k in v.keys():
+                    if k not in values["id_tag_registry"]["processing_job"]:
                         l(k)
         return v
 
     @validator("processing_job_ids")
     def job_callback(cls, v, values):
         with global_env_lock:
             for l in values.get("listeners", {}).get("processing_job_ids", []):
-                if values.get("processing_job_ids"):
-                    for k in set(values["processing_job_ids"].keys()) ^ set(v.keys()):
-                        l(k, v[k]["relion"])
-                else:
-                    for k in v.keys():
-                        l(k, v[k]["relion"])
+                for k in v.keys():
+                    if k not in values["id_tag_registry"]["auto_proc_program"]:
+                        l(k, v[k]["ispyb-relion"])
         return v
 
     @validator("autoproc_program_ids")
     def app_callback(cls, v, values):
         # logger.info(f"autoproc program ids validator: {v}")
         with global_env_lock:
             for l in values.get("listeners", {}).get("autoproc_program_ids", []):
-                if values.get("autoproc_program_ids"):
-                    for k in set(values["autoproc_program_ids"].keys()) ^ set(v.keys()):
-                        if v[k].get("em-tomo-preprocess"):
-                            l(k, v[k]["em-tomo-preprocess"])
-                else:
-                    for k in v.keys():
-                        if v[k].get("em-tomo-preprocess"):
-                            l(k, v[k]["em-tomo-preprocess"])
+                for k in v.keys():
+                    if v[k].get("em-tomo-preprocess"):
+                        l(k, v[k]["em-tomo-preprocess"])
         return v
 
     @validator("motion_corrected_movies")
     def motion_corrected_callback(cls, v, values):
-        # logger.info("motion corrected callback")
         _url = f"{str(values['url'].geturl())}/visits/{values['visit']}/align"
         for l in values.get("listeners", {}).get("motion_corrected_movies", []):
             if values.get("motion_corrected_movies"):
                 for k in set(values["motion_corrected_movies"].keys()) ^ set(
                     v.keys()
                 ):  # k is a path (key), v[k] is the value matching the key
                     tilt = values["movie_tilt_pair"][k]
                     file_tilt_list = []
                     for movie, angle in values["tilt_angles"][tilt]:
                         if movie in v:  # values["motion_corrected_movies"]:
-                            # file_tilt_list.append(
-                            #    [values["motion_corrected_movies"][movie], angle]
-                            # )
                             file_tilt_list.append(
                                 [
                                     str(v[Path(movie)][0]),
                                     angle,
                                     str(v[Path(movie)][1]),
                                 ]
                             )
```

### Comparing `murfey-0.7.6/src/murfey/client/rsync.py` & `murfey-0.7.7/src/murfey/client/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/tui/app.py` & `murfey-0.7.7/src/murfey/client/tui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from __future__ import annotations
 
-import asyncio
-
-# import contextlib
 import logging
 from datetime import datetime
 from functools import partial
 from pathlib import Path
 from queue import Queue
 from typing import Dict, List, OrderedDict, TypeVar
 from urllib.parse import urlparse
@@ -18,24 +15,25 @@
 from textual.widgets import Button, Input
 
 from murfey.client.analyser import Analyser
 from murfey.client.context import SPAContext, TomographyContext
 from murfey.client.instance_environment import MurfeyInstanceEnvironment
 from murfey.client.rsync import RSyncer, RSyncerUpdate, TransferResult
 from murfey.client.tui.screens import (
+    ConfirmScreen,
     InputResponse,
     MainScreen,
     ProcessingForm,
     VisitSelection,
     determine_default_destination,
 )
 from murfey.client.tui.status_bar import StatusBar
 from murfey.client.watchdir import DirWatcher
 from murfey.client.watchdir_multigrid import MultigridDirWatcher
-from murfey.util import _get_visit_list, get_machine_config
+from murfey.util import _get_visit_list
 
 log = logging.getLogger("murfey.tui.app")
 
 ReactiveType = TypeVar("ReactiveType")
 
 
 class MurfeyTUI(App):
@@ -247,14 +245,23 @@
 
     def _data_collection_form(self, response: dict):
         log.info("data collection form ready")
         if self._data_collection_form_complete:
             return
         if self._register_dc and response.get("form"):
             self._form_values = {k: str(v) for k, v in response.get("form", {}).items()}
+            log.info(
+                f"gain reference is set to {self._form_values.get('gain_ref')}, {self._environment.data_collection_parameters.get('gain_ref')}"
+            )
+            if self._form_values.get("gain_ref") in (None, "None"):
+                log.info(self._form_values)
+                self._form_values[
+                    "gain_ref"
+                ] = self._environment.data_collection_parameters.get("gain_ref")
+            log.info(self._form_values)
             self.processing_btn.disabled = False
             self._data_collection_form_complete = True
         elif self._register_dc is None:
             self._tmp_responses.append(response)
             self._data_collection_form_complete = True
 
     def _start_dc_confirm_prompt(self, json: dict):
@@ -289,33 +296,27 @@
             }
             self._environment.listeners["autoproc_program_ids"] = {
                 context._flush_preprocess
             }
             self._environment.listeners["motion_corrected_movies"] = {
                 context._check_for_alignment
             }
+            self._environment.id_tag_registry["data_collection_group"].append(
+                str(source)
+            )
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/register_data_collection_group"
             dcg_data = {
                 "experiment_type": "tomo",
                 "experiment_type_id": 36,
                 "tag": str(source),
             }
             requests.post(url, json=dcg_data)
         elif isinstance(context, SPAContext):
             source = Path(json["source"])
-            machine_config = get_machine_config(
-                str(self._url.geturl()), demo=self._environment.demo
-            )
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/start_data_collection"
-            json = {
-                "image_directory": Path(
-                    machine_config.get("rsync_basepath", ".")
-                ).resolve(),
-                **json,
-            }
             self._environment.listeners["data_collection_group_ids"] = {
                 partial(
                     context._register_data_collection,
                     url=url,
                     data=json,
                     environment=self._environment,
                 )
@@ -377,15 +378,28 @@
     async def on_mount(self) -> None:
         self.install_screen(VisitSelection(self.visits), "visit-select-screen")
         self.push_screen("visit-select-screen")
 
     def on_log_book_log(self, message):
         self.log_book.write(message.renderable)
 
+    def _clear_state(self):
+        url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/clear_state"
+        data = {
+            "data_collection_group": self._environment.id_tag_registry[
+                "data_collection_group"
+            ],
+            "data_collection": self._environment.id_tag_registry["data_collection"],
+            "processing_job": self._environment.id_tag_registry["processing_job"],
+            "autoproc_program": self._environment.id_tag_registry["auto_proc_program"],
+        }
+        requests.post(url, json=data)
+
     def reset(self):
+        self._clear_state()
         self._environment.clear()
         if self.rsync_processes:
             for rp in self.rsync_processes.values():
                 rp.stop()
             self.rsync_processes = {}
         if self.analysers:
             for a in self.analysers.values():
@@ -414,55 +428,59 @@
             for rp in self.rsync_processes.values():
                 rp.stop()
         if self.analysers:
             for a in self.analysers.values():
                 a.stop()
         if self._multigrid_watcher:
             self._multigrid_watcher.stop()
+        self._clear_state()
         self.exit()
         exit()
 
     async def action_clear(self) -> None:
-        destination = ""
-        if self.rsync_process:
-            destination = (
-                self.rsync_process._remote.split("::")[1]
-                if "::" in self.rsync_process._remote
-                else self.rsync_process._remote
-            )
-        self._queues["input"].put_nowait(
-            InputResponse(
-                question=f"Are you sure you want to remove all copied data? [{self._source} -> {destination}]",
-                allowed_responses=["y", "n"],
-                callback=partial(self._confirm_clear),
+        if self.rsync_processes:
+            sources = "\n".join(str(k) for k in self.rsync_processes.keys())
+            prompt = f"Remove files from the following: {sources}"
+            self.install_screen(
+                ConfirmScreen(
+                    prompt,
+                    pressed_callback=self._remove_data,
+                    button_names={"launch": "Yes", "quit": "No"},
+                ),
+                "clear-confirm",
             )
-        )
+            self.push_screen("clear-confirm")
 
-    async def action_process(self) -> None:
-        self.processing_btn.disabled = False
-
-    def _confirm_clear(self, response: str):
-        if response == "y":
-            if self._do_transfer and self.rsync_process:
-                destination = self.rsync_process._remote
-                self.rsync_process.stop()
-                if self.analyser:
-                    self.analyser.stop()
+    def _remove_data(self, **kwargs):
+        log.info(
+            f"Starting to remove data files {self._environment.demo}, {len(self.rsync_processes)}"
+        )
+        if self.rsync_processes or self._environment.demo:
+            for k, rp in self.rsync_processes.items():
+                rp.stop()
+                if self.analysers.get(k):
+                    self.analysers[k].stop()
                 cmd = [
                     "rsync",
                     "-iiv",
                     "-o",  # preserve ownership
                     "-p",  # preserve permissions
                     "--remove-source-files",
                 ]
                 cmd.extend(
-                    str(f.relative_to(self._source.absolute()))
-                    for f in self._source.absolute().glob("**/*")
-                )
-                cmd.append(destination)
-                result = procrunner.run(cmd)
-                log.info(
-                    f"rsync with removal finished with return code {result.returncode}"
+                    str(f.relative_to(k.absolute())) for f in k.absolute().glob("**/*")
                 )
+                cmd.append(rp._remote)
+                if self._environment.demo:
+                    log.info(
+                        f"rsync command {' '.join(cmd)} with removal in working directory {rp._basepath}"
+                    )
+                else:
+                    result = procrunner.run(cmd, working_directory=str(rp._basepath))
+                    log.info(
+                        f"rsync command {' '.join(cmd)} with removal finished with return code {result.returncode}"
+                    )
+        self.exit()
+        exit()
 
-            loop = asyncio.get_running_loop()
-            loop.create_task(self.action_quit())
+    async def action_process(self) -> None:
+        self.processing_btn.disabled = False
```

### Comparing `murfey-0.7.6/src/murfey/client/tui/controller.css` & `murfey-0.7.7/src/murfey/client/tui/controller.css`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 LaunchScreen {
     layout: grid;
     grid-size: 3;
     padding: 2;
     border: hidden;
 }
 
+GainReference {
+    layout: grid;
+    grid-size: 2;
+    padding: 2;
+    border: hidden;
+}
+
 ConfirmScreen {
     layout: grid;
     grid-size: 2;
     padding: 2;
     border: hidden;
 }
 
@@ -80,14 +87,38 @@
     border: solid black;
 }
 
 #launch:hover {
     background: purple;
 }
 
+#skip-gain {
+    width: 100%;
+    height: 100%;
+    column-span: 1;
+    background: teal;
+    border: solid black;
+}
+
+#skip-gain:hover {
+    background: purple;
+}
+
+#clear {
+    width: 100%;
+    height: 20%;
+    column-span: 1;
+    background: teal;
+    border: solid black;
+}
+
+#clear:hover {
+    background: purple;
+}
+
 #dir-select {
     width: 100%;
     height: 100%;
     column-span: 2;
     row-span: 2;
 }
 
@@ -251,26 +282,31 @@
     row-span: 3;
     content-align: left top;
     background: gray;
 }
 
 #selected-directories {
     width: 100%;
-    height: 100%;
+    height:75%;
     column-span: 1;
     row-span: 2;
 }
 
 #switch-directory {
     width: 100%;
     height: 100%;
     column-span: 3;
     row-span: 1;
 }
 
+#superres {
+    width: 50%;
+    height: 10fr;
+}
+
 #label-directory {
     width: 100%;
     height: 100%;
     column-span: 1;
     row-span: 1;
     content-align: center middle;
     text-style: bold;
@@ -278,14 +314,21 @@
 
 #input-form {
     width: 100%;
     height: 100%;
     background: black;
 }
 
+#selected-directories-vert {
+    width: 100%;
+    height: 100%;
+    row-span: 2;
+    background: black;
+}
+
 #destination-holder {
     width: 100%;
     height: 100%;
     column-span: 7;
     row-span: 3;
     background: black;
 }
@@ -316,7 +359,13 @@
     width: 100%;
     content-align: center middle;
 }
 
 .input {
     width: 100%;
 }
+
+
+#gain-select {
+    width: 100%;
+    column-span: 2;
+}
```

### Comparing `murfey-0.7.6/src/murfey/client/tui/forms.py` & `murfey-0.7.7/src/murfey/client/tui/forms.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/tui/progress.py` & `murfey-0.7.7/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/tui/screens.py` & `murfey-0.7.7/src/murfey/client/tui/screens.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # import contextlib
 import logging
 from datetime import datetime
 from pathlib import Path
 from typing import Callable, Dict, List, NamedTuple, OrderedDict, TypeVar
 
+import procrunner
 import requests
 from pydantic import BaseModel, ValidationError
 from rich.box import SQUARE
 from rich.panel import Panel
 from textual.app import ScreenStackError
 from textual.containers import Vertical
 from textual.message import Message
@@ -28,14 +29,15 @@
     Switch,
     TextLog,
     Tree,
 )
 
 from murfey.client.analyser import Analyser
 from murfey.client.context import SPAContext
+from murfey.client.gain_ref import determine_gain_ref
 from murfey.client.instance_environment import (
     MurfeyInstanceEnvironment,
     global_env_lock,
 )
 from murfey.client.tui.forms import TUIFormValue
 
 log = logging.getLogger("murfey.tui.screens")
@@ -194,15 +196,33 @@
                 if Path(self._selected_path).resolve().is_relative_to(d):
                     self.valid_selection = True
                     break
             else:
                 self.valid_selection = False
         else:
             self.valid_selection = False
-            self.post_message(self.FileSelected(dir_entry.path))
+
+
+class _DirectoryTreeGain(DirectoryTree):
+    valid_selection = reactive(False)
+
+    def __init__(self, gain_reference: Path, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._gain_reference = gain_reference
+
+    def on_tree_node_selected(self, event: Tree.NodeSelected) -> None:
+        event.stop()
+        dir_entry = event.node.data
+        if dir_entry is None:
+            return
+        if not dir_entry.is_dir:
+            self.valid_selection = True
+            self._gain_reference = Path(dir_entry.path)
+        else:
+            self.valid_selection = False
 
 
 class LaunchScreen(Screen):
     _launch_btn: Button | None = None
 
     def __init__(
         self, *args, basepath: Path = Path("."), add_basepath: bool = False, **kwargs
@@ -221,15 +241,18 @@
             if self.app._strict
             else {},
             id="dir-select",
         )
 
         yield self._dir_tree
         text_log = TextLog(id="selected-directories")
-        yield text_log
+        text_log_block = Vertical(
+            text_log, Button("Clear", id="clear"), id="selected-directories-vert"
+        )
+        yield text_log_block
 
         text_log.write("Selected directories:\n")
         btn_disabled = True
         for d in machine_data.get("data_directories", {}).keys():
             if Path(self._dir_tree._selected_path).resolve().is_relative_to(d):
                 btn_disabled = False
                 break
@@ -288,45 +311,57 @@
                     self.app._start_rsyncer(_default, visit_path=visit_path)
                 transfer_routes[s] = _default
             self.app.install_screen(
                 DestinationSelect(transfer_routes), "destination-select-screen"
             )
             self.app.pop_screen()
             self.app.push_screen("destination-select-screen")
+        elif event.button.id == "clear":
+            sel_dir = self.query_one("#selected-directories")
+            for line in sel_dir.lines[1:]:
+                source = Path(line.text)
+                if source in self.app._environment.sources:
+                    self.app._environment.sources.remove(source)
+                    del self.app._default_destinations[source]
+            sel_dir.clear()
+            sel_dir.write("Selected directories:\n")
 
 
 class ConfirmScreen(Screen):
     def __init__(
         self,
         prompt: str,
         *args,
         params: dict | None = None,
         pressed_callback: Callable | None = None,
+        button_names: dict | None = None,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self._prompt = prompt
         self._params = params or {}
         self._callback = pressed_callback
+        self._button_names = button_names or {}
 
     def compose(self):
         if self._params:
             dt = DataTable(id="prompt")
             keys = list(self._params.keys())
             dt.add_columns(*keys)
             dt.add_rows([[self._params[k] for k in keys]])
             yield dt
         else:
             yield Static(self._prompt, id="prompt")
-        yield Button("Launch", id="launch")
-        yield Button("Back", id="quit")
+        yield Button(self._button_names.get("launch") or "Launch", id="launch")
+        yield Button(self._button_names.get("quit") or "Back", id="quit")
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "quit":
             self.app.pop_screen()
+            self.app.uninstall_screen("confirm")
         else:
             while True:
                 try:
                     if self.app.screen._name == "main":
                         break
                     self.app.pop_screen()
                 except ScreenStackError:
@@ -348,30 +383,50 @@
 
     def compose(self):
         inputs = []
         analyser = list(self.app.analysers.values())[0]
         for k in analyser._context.user_params + analyser._context.metadata_params:
             t = k.label
             inputs.append(Label(t, classes="label"))
-            i = Input(placeholder=t, classes="input")
+            i = Input(placeholder=t, classes="input", id=f"input_{k.name}")
             self._inputs[i] = k.name
-            i.value = self._form.get(k.name)
+            default = self._form.get(k.name)
+            i.value = "None" if default is None else default
             inputs.append(i)
         confirm_btn = Button("Confirm", id="confirm-btn")
-        self._vert = Vertical(*inputs, confirm_btn, id="input-form")
+        if self._form.get("motion_corr_binning") == "2":
+            self._vert = Vertical(
+                *inputs,
+                Label("Collected in super resoultion mode:"),
+                Switch(id="superres", value=True),
+                confirm_btn,
+                id="input-form",
+            )
+        else:
+            self._vert = Vertical(*inputs, confirm_btn, id="input-form")
         yield self._vert
-        yield confirm_btn
+        # yield confirm_btn
 
     def _write_params(self, params: dict | None = None):
         if params:
             analyser = list(self.app.analysers.values())[0]
             for k in analyser._context.user_params + analyser._context.metadata_params:
                 self.app.query_one("#info").write(f"{k.label}: {params.get(k.name)}")
             self.app._start_dc(params)
 
+    def on_switch_changed(self, event):
+        pix_size = self.query_one("#input_pixel_size_on_image")
+        motion_corr_binning = self.query_one("#input_motion_corr_binning")
+        if event.value:
+            pix_size.value = str(float(pix_size.value) / 2)
+            motion_corr_binning.value = "2"
+        else:
+            pix_size.value = str(float(pix_size.value) * 2)
+            motion_corr_binning.value = "1"
+
     def on_input_changed(self, event):
         k = self._inputs[event.input]
         self._form[k] = event.value
 
     def on_button_pressed(self, event):
         if "confirm" not in self.app._installed_screens:
             self.app.install_screen(
@@ -428,29 +483,107 @@
             **kwargs,
         )
 
     def on_button_pressed(self, event: Button.Pressed):
         text = str(event.button.label)
         self.app._visit = text
         self.app._environment.visit = text
+        machine_data = requests.get(
+            f"{self.app._environment.url.geturl()}/machine/"
+        ).json()
         if self._switch_status:
-            machine_data = requests.get(
-                f"{self.app._environment.url.geturl()}/machine/"
-            ).json()
             self.app.install_screen(
                 DirectorySelection(
                     [
                         p[0]
                         for p in machine_data.get("data_directories", {}).items()
                         if p[1] == "detector" and Path(p[0]).exists()
                     ]
                 ),
                 "directory-select",
             )
         self.app.pop_screen()
+
+        if machine_data.get("gain_reference_directory"):
+            self.app.install_screen(
+                GainReference(
+                    determine_gain_ref(Path(machine_data["gain_reference_directory"])),
+                    self._switch_status,
+                ),
+                "gain-ref-select",
+            )
+            self.app.push_screen("gain-ref-select")
+        else:
+            if self._switch_status:
+                self.app.push_screen("directory-select")
+            else:
+                self.app.install_screen(LaunchScreen(basepath=Path("./")), "launcher")
+                self.app.push_screen("launcher")
+
+
+class GainReference(Screen):
+    def __init__(self, gain_reference: Path, switch_status: bool, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._gain_reference = gain_reference
+        self._switch_status = switch_status
+
+    def compose(self):
+        self._dir_tree = _DirectoryTreeGain(
+            self._gain_reference,
+            str(self._gain_reference.parent.parent),
+            id="gain-select",
+        )
+        yield self._dir_tree
+        self._launch_btn = Button("Launch", id="launch")
+        self.watch(self._dir_tree, "valid_selection", self._check_valid_selection)
+        yield self._launch_btn
+        yield Button("No gain", id="skip-gain")
+
+    def _check_valid_selection(self, valid: bool):
+        if self._launch_btn:
+            if valid:
+                self._launch_btn.disabled = False
+            else:
+                self._launch_btn.disabled = True
+
+    def on_button_pressed(self, event):
+        if event.button.id == "skip-gain":
+            self.app.pop_screen()
+        else:
+            visit_path = f"data/{datetime.now().year}/{self.app._environment.visit}"
+            cmd = [
+                "rsync",
+                str(self._dir_tree._gain_reference),
+                f"{self.app._environment.url.hostname}::{visit_path}/processing",
+            ]
+            if self.app._environment.demo:
+                log.info(f"Would perform {' '.join(cmd)}")
+            else:
+                gain_rsync = procrunner.run(cmd)
+                if gain_rsync.returncode:
+                    log.warning(
+                        f"Gain reference file {self._dir_tree._gain_reference} was not successfully transferred to {visit_path}/processing"
+                    )
+        process_gain_response = requests.post(
+            url=f"{str(self.app._environment.url.geturl())}/visits/{self.app._environment.visit}/process_gain",
+            json={
+                "gain_ref": str(self._dir_tree._gain_reference),
+            },
+        )
+        if str(process_gain_response.status_code).startswith("4"):
+            log.warning(
+                f"Gain processing failed: status code {process_gain_response.status_code}"
+            )
+        else:
+            log.info(
+                f"Gain reference file {process_gain_response.json().get('gain_ref')}"
+            )
+            self.app._environment.data_collection_parameters[
+                "gain_ref"
+            ] = process_gain_response.json().get("gain_ref")
         if self._switch_status:
             self.app.push_screen("directory-select")
         else:
             self.app.install_screen(LaunchScreen(basepath=Path("./")), "launcher")
             self.app.push_screen("launcher")
```

### Comparing `murfey-0.7.6/src/murfey/client/tui/status_bar.py` & `murfey-0.7.7/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/update.py` & `murfey-0.7.7/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/watchdir.py` & `murfey-0.7.7/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/watchdir_multigrid.py` & `murfey-0.7.7/src/murfey/client/watchdir_multigrid.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/client/websocket.py` & `murfey-0.7.7/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/__init__.py` & `murfey-0.7.7/src/murfey/server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
                 }
             else:
                 global_state["data_collection_group_ids"] = {message.get("tag"): dcgid}
             _transport_object.transport.ack(header)
         return None
     elif message["register"] == "data_collection":
         dcgid = global_state.get("data_collection_group_ids", {}).get(  # type: ignore
-            message["source"]
+            message["tag"]
         )
         if dcgid is None:
             raise ValueError(
                 f"No data collection group ID was found for image directory {message['image_directory']}"
             )
         record = DataCollection(
             SESSIONID=message["session_id"],
```

### Comparing `murfey-0.7.6/src/murfey/server/api.py` & `murfey-0.7.7/src/murfey/server/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 import murfey.server.websocket as ws
 from murfey.server import _transport_object, get_hostname, get_microscope
 from murfey.server import shutdown as _shutdown
 from murfey.server import templates
 from murfey.server.config import MachineConfig, from_file
 from murfey.server.gain import Camera, prepare_gain
 from murfey.util.models import (
+    ClearanceKeys,
     ConnectionFileParameters,
     ContextInfo,
     DCGroupParameters,
     DCParameters,
     File,
     GainReference,
     ProcessFile,
     ProcessingJobParameters,
     RegistrationMessage,
     SPAProcessingParameters,
     SuggestedPathParameters,
     TiltSeries,
     Visit,
 )
+from murfey.util.state import global_state
 
 log = logging.getLogger("murfey.server.api")
 
 
 class Settings(BaseSettings):
     murfey_machine_configuration: str = ""
 
@@ -453,25 +455,72 @@
         )
     return proc_params
 
 
 @router.post("/visits/{visit_name}/write_connections_file")
 def write_conn_file(visit_name, params: ConnectionFileParameters):
     filepath = (
-        Path(machine_config["rsync_basepath"])
-        / (machine_config.get("rsync_module") or "data")
+        Path(machine_config.rsync_basepath)
+        / (machine_config.rsync_module or "data")
         / str(datetime.datetime.now().year)
         / secure_filename(visit_name)
     )
     with open(filepath / secure_filename(params.filename), "w") as f:
         for d in params.destinations:
             f.write(f"{d}\n")
 
 
 @router.post("/visits/{visit_name}/process_gain")
 async def process_gain(visit_name, gain_reference_params: GainReference):
     camera = getattr(Camera, machine_config.camera)
     executables = machine_config.external_executables
+    filepath = (
+        Path(machine_config.rsync_basepath)
+        / (machine_config.rsync_module or "data")
+        / str(datetime.datetime.now().year)
+        / secure_filename(visit_name)
+    )
     new_gain_ref = await prepare_gain(
-        camera, gain_reference_params.gain_ref, executables
+        camera, filepath / gain_reference_params.gain_ref.name, executables
     )
-    return {"gain_ref": new_gain_ref}
+    if new_gain_ref:
+        return {
+            "gain_ref": new_gain_ref.relative_to(Path(machine_config.rsync_basepath))
+        }
+    else:
+        return {"gain_ref": new_gain_ref}
+
+
+@router.post("/visits/{visit_name}/clean_state")
+async def clean_state(visit_name, for_clearance: ClearanceKeys):
+    if global_state.get("data_collection_group_ids") and isinstance(
+        global_state["data_collection_group_ids"], dict
+    ):
+        global_state["data_collection_group_ids"] = {
+            k: v
+            for k, v in global_state["data_collection_group_ids"].items()
+            if k not in for_clearance.data_collection_group
+        }
+    if global_state.get("data_collection_ids") and isinstance(
+        global_state["data_collection_ids"], dict
+    ):
+        global_state["data_collection_ids"] = {
+            k: v
+            for k, v in global_state["data_collection_ids"].items()
+            if k not in for_clearance.data_collection
+        }
+    if global_state.get("processing_job_ids") and isinstance(
+        global_state["processing_job_ids"], dict
+    ):
+        global_state["processing_job_ids"] = {
+            k: v
+            for k, v in global_state["processing_job_ids"].items()
+            if k not in for_clearance.processing_job
+        }
+    if global_state.get("autoproc_program_ids") and isinstance(
+        global_state["autoproc_program_ids"], dict
+    ):
+        global_state["autoproc_program_ids"] = {
+            k: v
+            for k, v in global_state["autoproc_program_ids"].items()
+            if k not in for_clearance.autoproc_program
+        }
```

### Comparing `murfey-0.7.6/src/murfey/server/bootstrap.py` & `murfey-0.7.7/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/config.py` & `murfey-0.7.7/src/murfey/server/config.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/demo_api.py` & `murfey-0.7.7/src/murfey/server/demo_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from murfey.server.config import from_file
 from murfey.util.models import (
     ConnectionFileParameters,
     ContextInfo,
     DCGroupParameters,
     DCParameters,
     File,
+    GainReference,
     ProcessFile,
     ProcessingJobParameters,
     RegistrationMessage,
     SPAProcessingParameters,
     SuggestedPathParameters,
     TiltSeries,
     Visit,
@@ -346,7 +347,25 @@
 def write_conn_file(visit_name, params: ConnectionFileParameters):
     filepath = (
         Path(machine_config["rsync_basepath"])
         / (machine_config.get("rsync_module") or "data")
         / str(datetime.datetime.now().year)
     )
     log.info(f"Write to connection file at {filepath}")
+
+
+@router.post("/visits/{visit_name}/process_gain")
+async def process_gain(visit_name, gain_reference_params: GainReference):
+    if machine_config.get("rsync_basepath"):
+        filepath = (
+            Path(machine_config["rsync_basepath"])
+            / (machine_config.get("rsync_module") or "data")
+            / str(datetime.datetime.now().year)
+            / visit_name
+        )
+    else:
+        return {"gain_ref": None}
+    return {
+        "gain_ref": (filepath / "processing" / "gain.mrc").relative_to(
+            Path(machine_config["rsync_basepath"])
+        )
+    }
```

### Comparing `murfey-0.7.6/src/murfey/server/gain.py` & `murfey-0.7.7/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/ispyb.py` & `murfey-0.7.7/src/murfey/server/ispyb.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/main.py` & `murfey-0.7.7/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/server/websocket.py` & `murfey-0.7.7/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/activevisits.html` & `murfey-0.7.7/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/base.html` & `murfey-0.7.7/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/bootstrap.html` & `murfey-0.7.7/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/images/diamond.png` & `murfey-0.7.7/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/images/icon_268.png` & `murfey-0.7.7/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/static/styles.css` & `murfey-0.7.7/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/templates/visit.html` & `murfey-0.7.7/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/__init__.py` & `murfey-0.7.7/src/murfey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/dummy_setup.py` & `murfey-0.7.7/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/file_monitor.py` & `murfey-0.7.7/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/mdoc.py` & `murfey-0.7.7/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/models.py` & `murfey-0.7.7/src/murfey/util/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 
 
 class ContextInfo(BaseModel):
     experiment_type: str
     acquisition_software: str
 
 
+class ClearanceKeys(BaseModel):
+    data_collection_group: List[str]
+    data_collection: List[str]
+    processing_job: List[str]
+    autoproc_program: List[str]
+
+
 class File(BaseModel):
     name: str
     description: str
     size: int
     timestamp: float
```

### Comparing `murfey-0.7.6/src/murfey/util/rsync.py` & `murfey-0.7.7/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey/util/state.py` & `murfey-0.7.7/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.6/src/murfey.egg-info/PKG-INFO` & `murfey-0.7.7/src/murfey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.6
+Version: 0.7.7
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.6/src/murfey.egg-info/SOURCES.txt` & `murfey-0.7.7/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

