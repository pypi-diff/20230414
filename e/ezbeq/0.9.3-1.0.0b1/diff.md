# Comparing `tmp/ezbeq-0.9.3.tar.gz` & `tmp/ezbeq-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ezbeq-0.9.3.tar", last modified: Wed Aug 11 18:57:06 2021, max compression
+gzip compressed data, was "ezbeq-1.0.0b1.tar", last modified: Fri Apr 14 19:57:49 2023, max compression
```

## Comparing `ezbeq-0.9.3.tar` & `ezbeq-1.0.0b1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-08-11 18:54:08.000000 ezbeq-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-08-11 18:54:08.000000 ezbeq-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-08-11 18:57:06.000000 ezbeq-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-08-11 18:54:08.000000 ezbeq-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    17190 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (121)    11689 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)     8306 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (121)    22580 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7070 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    24652 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/minidsp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)    14091 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css
--rw-r--r--   0 runner    (1001) docker     (121)     5955 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)   623905 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     4762 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2426595 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)    45911 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)   134396 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js
--rw-r--r--   0 runner    (1001) docker     (121)     8270 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    66044 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-all-400-normal.b5a0a0df.woff
--rw-r--r--   0 runner    (1001) docker     (121)     9900 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-400-normal.3605d18d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15520 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     7296 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-400-normal.352cc77a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15736 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-400-normal.176f8f5b.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    12200 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-vietnamese-400-normal.52cebac0.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 18:57:06.000000 ezbeq-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-08-11 18:54:08.000000 ezbeq-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.107607 ezbeq-1.0.0b1/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.111607 ezbeq-1.0.0b1/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/iir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/minidsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/qsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.115607 ezbeq-1.0.0b1/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.103607 ezbeq-1.0.0b1/ezbeq/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.115607 ezbeq-1.0.0b1/ezbeq/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.119608 ezbeq-1.0.0b1/ezbeq/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   937350 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4111826 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/ezbeq/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.111607 ezbeq-1.0.0b1/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/tests/test_minidsp_api.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ezbeq-0.9.3/LICENSE` & `ezbeq-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.0b1/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/catalogue.py` & `ezbeq-1.0.0b1/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.0b1/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/meta.py` & `ezbeq-1.0.0b1/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/search.py` & `ezbeq-1.0.0b1/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/ws.py` & `ezbeq-1.0.0b1/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/apis/years.py` & `ezbeq-1.0.0b1/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/catalogue.py` & `ezbeq-1.0.0b1/ezbeq/catalogue.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         self.the_movie_db = vals.get('theMovieDB', '')
         self.rating = vals.get('rating', '')
         self.genres = vals.get('genres', [])
         self.altTitle = vals.get('altTitle', '')
         self.created_at = vals.get('created_at', 0)
         self.updated_at = vals.get('updated_at', 0)
         self.digest = vals.get('digest', '')
+        self.collection = vals.get('collection', {})
+        self.formatted_title = self.__format_title()
         now = time.time()
         if self.created_at >= (now - TWO_WEEKS_AGO_SECONDS):
             self.freshness = 'Fresh'
         elif self.updated_at >= (now - TWO_WEEKS_AGO_SECONDS):
             self.freshness = 'Updated'
         else:
             self.freshness = 'Stale'
@@ -77,15 +79,16 @@
             'sortTitle': self.sort_title,
             'audioTypes': self.audio_types,
             'contentType': self.content_type,
             'author': self.author,
             'created_at': self.created_at,
             'updated_at': self.updated_at,
             'freshness': self.freshness,
-            'digest': self.digest
+            'digest': self.digest,
+            'formattedTitle': self.formatted_title
         }
         if self.beqc_url:
             self.for_search['beqcUrl'] = self.beqc_url
         if self.images:
             self.for_search['images'] = self.images
         if self.warning:
             self.for_search['warning'] = self.warning
@@ -117,14 +120,16 @@
             self.for_search['genres'] = self.genres
         if self.altTitle:
             self.for_search['altTitle'] = self.altTitle
         if self.note:
             self.for_search['note'] = self.note
         if self.warning:
             self.for_search['warning'] = self.warning
+        if self.collection and 'name' in self.collection:
+            self.for_search['collection'] = self.collection['name']
 
     def matches(self, authors: List[str], years: List[int], audio_types: List[str], content_types: List[str]):
         if not authors or self.author in authors:
             if not years or self.year in years:
                 if not audio_types or any(a_t in audio_types for a_t in self.audio_types):
                     return not content_types or self.content_type in content_types
         return False
@@ -163,19 +168,18 @@
                         else:
                             formatted += self.__format_episodes(formatted, working)
                             working = []
                 if len(working) > 0:
                     formatted += self.__format_episodes(formatted, working)
             else:
                 formatted += f"{self.episodes}"
-            return f"{season} {formatted}"
+            return f"{season}{formatted}"
         return season
 
-    @property
-    def formatted_title(self) -> str:
+    def __format_title(self) -> str:
         if self.content_type == 'TV':
             return f"{self.title} {self.__format_tv_meta()}"
         return self.title
 
 
 class CatalogueProvider:
 
@@ -219,24 +223,24 @@
 
     @property
     def version(self) -> Optional[str]:
         return self.__version
 
     @property
     def catalogue(self) -> List[CatalogueEntry]:
-        self.__executor.submit(self.__refresh_catalogue_if_stale).result(timeout=60)
+        self.__executor.submit(self.__refresh_catalogue_if_stale)
         return self.__catalogue
 
     def __refresh_catalogue_if_stale(self):
         if self.__loaded_at is None or (datetime.now() - self.__loaded_at) > timedelta(minutes=15):
             try:
                 self.__reload()
             except Exception as e:
+                logger.exception(f"Failed to refresh catalogue,[last loaded at {self.__loaded_at}]", e)
                 self.__loaded_at = None
-                raise e
 
 
 class DatabaseDownloader:
 
     def __init__(self, download_url: str, cached_db_file, cached_version_file):
         self.__download_url = download_url
         if download_url[-1] != '/':
@@ -259,30 +263,33 @@
         '''
         Hit the BEQ Catalogue database and compare to the local cached version.
         if there is an updated database then download it.
         '''
         remote_version = self.__get_remote_catalogue_version()
         if remote_version is None or self.__cached_version is None or remote_version != self.__cached_version:
             logger.info(f"Reloading from {self.__db_url}")
-            r = requests.get(self.__db_url, allow_redirects=True)
-            if r.status_code == 200:
-                logger.info(f"Writing database to {self.__cached_db_file}")
-                with open(self.__cached_db_file, 'wb') as f:
-                    f.write(r.content)
-                if remote_version:
-                    logger.info(f"Writing version {remote_version} to {self.__cached_version_file}")
-                    with open(self.__cached_version_file, 'w') as f:
-                        f.write(remote_version)
+            try:
+                r = requests.get(self.__db_url, allow_redirects=True)
+                if r.status_code == 200:
+                    logger.info(f"Writing database to {self.__cached_db_file}")
+                    with open(self.__cached_db_file, 'wb') as f:
+                        f.write(r.content)
+                    if remote_version:
+                        logger.info(f"Writing version {remote_version} to {self.__cached_version_file}")
+                        with open(self.__cached_version_file, 'w') as f:
+                            f.write(remote_version)
+                    else:
+                        logger.warning(f"No remote version to write")
+                    self.__cached_version = remote_version
+                    logger.info(f"Downloaded {self.__db_url} @ {remote_version}")
+                    return True
                 else:
-                    logger.warning(f"No remote version to write")
-                self.__cached_version = remote_version
-                logger.info(f"Downloaded {self.__db_url} @ {remote_version}")
-                return True
-            else:
-                logger.warning(f"Unable to download catalogue, response is {r.status_code}")
+                    logger.warning(f"Unable to download catalogue, response is {r.status_code}")
+            except:
+                logger.exception(f"Unable to download catalogue, unexpected error")
         else:
             logger.info(f"No reload required {remote_version} vs {self.__cached_version}")
         return False
 
     def __get_remote_catalogue_version(self) -> Optional[str]:
         '''
         gets version.txt to discover the remote catalogue version.
```

### Comparing `ezbeq-0.9.3/ezbeq/config.py` & `ezbeq-1.0.0b1/ezbeq/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         self.logger = logging.getLogger(name + '.config')
         self.config = self.load_config()
         self.icon_path = self.config.get('iconPath')
         self.__hostname = self.config.get('host', self.default_hostname)
         self.__port = self.config.get('port', default_port)
         self.__service_url = f"http://{self.hostname}:{self.port}"
         self.__beqcatalogue_url = beqcatalogue_url
+        if 'catalogueUrl' in self.config:
+            self.__beqcatalogue_url = self.config['catalogueUrl']
+            self.logger.warning(f"Loading catalogue from custom location {self.__beqcatalogue_url}")
         self.devices = self.config['devices']
         self.webapp_path = self.config.get('webappPath', None)
         self.use_twisted = self.config.get('useTwisted', True)
 
     @staticmethod
     def ensure_dir_exists(d) -> None:
         if not os.path.exists(d):
@@ -99,15 +102,15 @@
                     shutil.copyfile(config_path, path.join(self.config_path, self._name + ".yml.bak"))
                     self.__store_config(cfg, config_path)
         if cfg is None:
             cfg = self.load_default_config()
             self.__store_config(cfg, config_path)
         for name, device in cfg['devices'].items():
             if device['type'] == 'minidsp':
-                device['make_runner'] = lambda: self.create_minidsp_runner(device)
+                device['make_runner'] = self.create_minidsp_runner
         return cfg
 
     def __store_config(self, config, config_path):
         """
         Writes the config to the configPath.
         :param config a dict of config.
         :param config_path the path to the file to write to, intermediate dirs will be created as necessary.
@@ -176,18 +179,18 @@
         fh.setFormatter(formatter)
         ch.setFormatter(formatter)
         # add the handlers to the logger
         logger.addHandler(fh)
         logger.addHandler(ch)
         return logger
 
-    def create_minidsp_runner(self, device: dict):
+    def create_minidsp_runner(self, exe: str, options: str):
         from plumbum import local
-        cmd = local[device['exe']]
-        return cmd[device['options'].split(' ')] if device.get('options', None) else cmd
+        cmd = local[exe]
+        return cmd[options.split(' ')] if options else cmd
 
     @property
     def version(self):
         if getattr(sys, 'frozen', False):
             # pyinstaller lets you copy files to arbitrary locations under the _MEIPASS root dir
             root = os.path.join(sys._MEIPASS)
         else:
```

### Comparing `ezbeq-0.9.3/ezbeq/device.py` & `ezbeq-1.0.0b1/ezbeq/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         pass
 
     @property
     def supports_gain(self) -> bool:
         return False
 
     @abstractmethod
-    def state(self) -> T:
+    def state(self, refresh: bool = False) -> T:
         pass
 
     @abstractmethod
     def activate(self, slot: str) -> None:
         pass
 
     @abstractmethod
@@ -82,14 +82,18 @@
         pass
 
     @abstractmethod
     def load_biquads(self, slot: str, overwrite: bool, inputs: List[int], outputs: List[int], biquads: List[dict]) -> None:
         pass
 
     @abstractmethod
+    def send_commands(self, slot: str, inputs: List[int], outputs: List[int], commands: List[str]) -> None:
+        pass
+
+    @abstractmethod
     def clear_filter(self, slot: str) -> None:
         pass
 
     @abstractmethod
     def mute(self, slot: Optional[str], channel: Optional[int]) -> None:
         pass
 
@@ -128,27 +132,30 @@
 
     def supports_gain(self, name: str) -> bool:
         return self.__get_device(name).supports_gain
 
     def state(self, name: str) -> DeviceState:
         return self.__get_device(name).state()
 
-    def all_devices(self) -> Dict[str, DeviceState]:
-        return {n: d.state() for n, d in self.__devices.items()}
+    def all_devices(self, refresh: bool = False) -> Dict[str, DeviceState]:
+        return {n: d.state(refresh=refresh) for n, d in self.__devices.items()}
 
     def activate(self, name: str, slot: str) -> None:
         self.__get_device(name).activate(slot)
 
     def load_filter(self, name: str, slot: str, entry: CatalogueEntry) -> None:
         self.__get_device(name).load_filter(slot, entry)
 
     def load_biquads(self, name: str, slot: str, overwrite: bool, inputs: List[int], outputs: List[int],
                      biquads: List[dict]) -> None:
         self.__get_device(name).load_biquads(slot, overwrite, inputs, outputs, biquads)
 
+    def send_commands(self, name: str, slot: str, inputs: List[int], outputs: List[int], commands: List[str]) -> None:
+        self.__get_device(name).send_commands(slot, inputs, outputs, commands)
+
     def clear_filter(self, name: str, slot: str) -> None:
         self.__get_device(name).clear_filter(slot)
 
     def mute(self, name: str, slot: Optional[str], channel: Optional[int]) -> None:
         self.__get_device(name).mute(slot, channel)
 
     def unmute(self, name: str, slot: Optional[str], channel: Optional[int]) -> None:
@@ -173,14 +180,17 @@
             devices.append(Minidsp(name, cfg.config_path, values, ws_server, catalogue))
         elif d_type == 'htp1':
             from ezbeq.htp1 import Htp1
             devices.append(Htp1(name, cfg.config_path, values, ws_server, catalogue))
         elif d_type == 'jriver':
             from ezbeq.jriver import JRiver
             devices.append(JRiver(name, cfg.config_path, values, ws_server, catalogue))
+        elif d_type == 'qsys':
+            from ezbeq.qsys import Qsys
+            devices.append(Qsys(name, cfg.config_path, values, ws_server, catalogue))
     if not devices:
         raise ValueError('No device configured')
     else:
         return devices
 
 
 class InvalidRequestError(Exception):
@@ -200,30 +210,31 @@
         self._current_state: Optional[T] = None
         self.__ws_server = ws_server
 
     @property
     def name(self) -> str:
         return self.__name
 
-    def state(self) -> T:
-        self._hydrate()
+    def state(self, refresh: bool = False) -> T:
+        self._hydrate(refresh=refresh)
         return self._current_state
 
-    def _hydrate(self) -> bool:
-        if not self.__hydrated:
+    def _hydrate(self, refresh: bool = False) -> bool:
+        if not self.__hydrated or refresh is True:
             self._current_state = self._load_initial_state()
             if os.path.exists(self.__file_name):
                 with open(self.__file_name, 'r') as f:
                     cached_state = json.load(f)
                 logger.info(f"Loaded {cached_state} from {self.__file_name}")
                 self._current_state = self._merge_state(self._current_state, cached_state)
             else:
                 logger.info(f"No cached state found at {self.__file_name}")
-            self.__ws_server.factory.init(self.__get_state_msg)
-            self.__hydrated = True
+            if refresh is False:
+                self.__ws_server.factory.init(self.__get_state_msg)
+                self.__hydrated = True
             return True
         return False
 
     @abstractmethod
     def _load_initial_state(self) -> T:
         pass
```

### Comparing `ezbeq-0.9.3/ezbeq/htp1.py` & `ezbeq-1.0.0b1/ezbeq/htp1.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,25 +97,28 @@
         def __do_it():
             self._current_state.slot.active = True
         self._hydrate_cache_broadcast(__do_it)
 
     def load_biquads(self, slot: str, overwrite: bool, inputs: List[int], outputs: List[int], biquads: List[dict]) -> None:
         raise NotImplementedError()
 
+    def send_commands(self, slot: str, inputs: List[int], outputs: List[int], commands: List[str]) -> None:
+        raise NotImplementedError()
+
     def load_filter(self, slot: str, entry: CatalogueEntry) -> None:
         to_load = [PEQ(idx, fc=f['freq'], q=f['q'], gain=f['gain'], filter_type_name=f['type'])
                    for idx, f in enumerate(entry.filters)]
         self._hydrate_cache_broadcast(lambda: self.__do_it(to_load, entry.formatted_title))
 
     def __do_it(self, to_load: List['PEQ'], title: str):
         try:
             self.__send(to_load)
             self._current_state.slot.last = title
         except Exception as e:
-            self._current_state.slot.last = 'ERRUR'
+            self._current_state.slot.last = 'ERROR'
             raise e
 
     def clear_filter(self, slot: str) -> None:
         self._hydrate_cache_broadcast(lambda: self.__do_it([], 'Empty'))
 
     def mute(self, slot: Optional[str], channel: Optional[int]) -> None:
         raise NotImplementedError()
```

### Comparing `ezbeq-0.9.3/ezbeq/jriver.py` & `ezbeq-1.0.0b1/ezbeq/jriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,17 @@
                             self.clear_filter(slot['id'])
                             any_update = True
         return any_update
 
     def load_biquads(self, slot: str, overwrite: bool, inputs: List[int], outputs: List[int], biquads: List[dict]) -> None:
         raise NotImplementedError()
 
+    def send_commands(self, slot: str, inputs: List[int], outputs: List[int], commands: List[str]) -> None:
+        raise NotImplementedError()
+
     def load_filter(self, slot: str, entry: CatalogueEntry) -> None:
         def __do_it():
             mc_filts = [make_meta(entry.title, True)] \
                        + [convert_filter_to_mc_dsp(f, self.__channels) for f in entry.filters] \
                        + [make_meta(entry.title, False)]
             xml_filts = [filts_to_xml(f) for f in mc_filts]
             zone_id = self._current_state.get_zone_id(slot)
@@ -126,15 +129,15 @@
             new_config_txt = self.__remove_all_beq(current_config_txt)
             new_config_txt = include_filters_in_dsp(self.__peq_block, new_config_txt, xml_filts, replace=False)
             logger.info(new_config_txt)
             try:
                 self.__mcws.set_dsp(zone_id, new_config_txt)
                 self._current_state.set_title(slot, entry.formatted_title)
             except Exception as e:
-                self._current_state.slot.last = 'ERRUR'
+                self._current_state.slot.last = 'ERROR'
                 raise e
         self._hydrate_cache_broadcast(__do_it)
 
     def __remove_all_beq(self, current_config_txt) -> str:
         tries = 0
         final_config_txt = current_config_txt
         while tries < 100:
```

### Comparing `ezbeq-0.9.3/ezbeq/main.py` & `ezbeq-1.0.0b1/ezbeq/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import faulthandler
 from autobahn.twisted.resource import WebSocketResource
 from flask import Flask
 from flask_compress import Compress
 from flask_restx import Api
 
-from ezbeq.apis import search, version, devices, authors, audiotypes, years, contenttypes, meta, catalogue as cat_api
+from ezbeq.apis import search, version, devices, authors, audiotypes, years, contenttypes, languages, meta, catalogue as cat_api
 from ezbeq.apis.ws import WsServer
 from ezbeq.catalogue import CatalogueProvider
 from ezbeq.config import Config
 from ezbeq.device import DeviceRepository
 
 faulthandler.enable()
 if hasattr(faulthandler, 'register'):
@@ -47,14 +47,15 @@
     decorate_ns(devices.v2_api)
     decorate_ns(search.api)
     decorate_ns(version.api)
     decorate_ns(authors.api)
     decorate_ns(audiotypes.api)
     decorate_ns(years.api)
     decorate_ns(contenttypes.api)
+    decorate_ns(languages.api)
     decorate_ns(meta.api)
     decorate_ns(cat_api.api)
     return app, ws_server
 
 
 def main(args=None):
     """ The main routine. """
```

### Comparing `ezbeq-0.9.3/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.0b1/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.0b1/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.0b1/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.0b1/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.0b1/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/favicon.ico` & `ezbeq-1.0.0b1/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.0b1/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.0b1/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css` & `ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+0460-052f,U+1c80-1c88,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-cyrillic-400-normal.3605d18d.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+1f??}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-greek-400-normal.352cc77a.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+0370-03ff}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-vietnamese-400-normal.52cebac0.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+1ea0-1ef9,U+20ab}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+0100-024f,U+0259,U+1e??,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:"Roboto";font-style:normal;font-display:swap;font-weight:400;src:url(/static/media/roboto-latin-400-normal.176f8f5b.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.b5a0a0df.woff) format("woff");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}.uplot,.uplot *,.uplot :after,.uplot :before{box-sizing:border-box}.uplot{font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";line-height:1.5;width:-webkit-min-content;width:min-content}.u-title{text-align:center;font-size:18px;font-weight:700}.u-wrap{position:relative;-webkit-user-select:none;-ms-user-select:none;user-select:none}.u-over,.u-under{position:absolute}.u-under{overflow:hidden}.uplot canvas{display:block;position:relative;width:100%;height:100%}.u-legend{font-size:14px;margin:auto;text-align:center}.u-inline{display:block}.u-inline *{display:inline-block}.u-inline tr{margin-right:16px}.u-legend th{font-weight:600}.u-legend th>*{vertical-align:middle;display:inline-block}.u-legend .u-marker{width:1em;height:1em;margin-right:4px;background-clip:content-box!important}.u-inline.u-live th:after{content:":";vertical-align:middle}.u-inline:not(.u-live) .u-value{display:none}.u-series>*{padding:4px}.u-series th{cursor:pointer}.u-legend .u-off>*{opacity:.3}.u-select{background:rgba(0,0,0,.07)}.u-cursor-x,.u-cursor-y,.u-select{position:absolute;pointer-events:none}.u-cursor-x,.u-cursor-y{left:0;top:0;will-change:transform;z-index:100}.u-hz .u-cursor-x,.u-vt .u-cursor-y{height:100%;border-right:1px dashed #607d8b}.u-hz .u-cursor-y,.u-vt .u-cursor-x{width:100%;border-bottom:1px dashed #607d8b}.u-cursor-pt{position:absolute;top:0;left:0;border-radius:50%;pointer-events:none;will-change:transform;z-index:100;background-clip:content-box!important}.u-cursor-pt.u-off,.u-cursor-x.u-off,.u-cursor-y.u-off,.u-select.u-off{display:none}
-/*# sourceMappingURL=2.c2136c50.chunk.css.map */
+@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+0460-052f,u+1c80-1c88,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+1f??}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+0370-03ff}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+1ea0-1ef9,u+20ab}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+0100-024f,u+0259,u+1e??,u+2020,u+20a0-20ab,u+20ad-20cf,u+2113,u+2c60-2c7f,u+a720-a7ff}@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2) format("woff2"),url(/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff) format("woff");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+2000-206f,u+2074,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}.uplot,.uplot *,.uplot :after,.uplot :before{box-sizing:border-box}.uplot{font-family:system-ui,-apple-system,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;width:-webkit-min-content;width:min-content}.u-title{font-size:18px;font-weight:700;text-align:center}.u-wrap{position:relative;-webkit-user-select:none;user-select:none}.u-over,.u-under{position:absolute}.u-under{overflow:hidden}.uplot canvas{display:block;height:100%;position:relative;width:100%}.u-axis{position:absolute}.u-legend{font-size:14px;margin:auto;text-align:center}.u-inline{display:block}.u-inline *{display:inline-block}.u-inline tr{margin-right:16px}.u-legend th{font-weight:600}.u-legend th>*{display:inline-block;vertical-align:middle}.u-legend .u-marker{background-clip:padding-box!important;height:1em;margin-right:4px;width:1em}.u-inline.u-live th:after{content:":";vertical-align:middle}.u-inline:not(.u-live) .u-value{display:none}.u-series>*{padding:4px}.u-series th{cursor:pointer}.u-legend .u-off>*{opacity:.3}.u-select{background:rgba(0,0,0,.07)}.u-cursor-x,.u-cursor-y,.u-select{pointer-events:none;position:absolute}.u-cursor-x,.u-cursor-y{left:0;top:0;will-change:transform;z-index:100}.u-hz .u-cursor-x,.u-vt .u-cursor-y{border-right:1px dashed #607d8b;height:100%}.u-hz .u-cursor-y,.u-vt .u-cursor-x{border-bottom:1px dashed #607d8b;width:100%}.u-cursor-pt{background-clip:padding-box!important;border:0 solid;border-radius:50%;left:0;pointer-events:none;position:absolute;top:0;will-change:transform;z-index:100}.u-axis.u-off,.u-cursor-pt.u-off,.u-cursor-x.u-off,.u-cursor-y.u-off,.u-select.u-off{display:none}
+/*# sourceMappingURL=main.79943053.css.map*/
```

### Comparing `ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css.map` & `ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'file'": "'static/css/main.79943053.css'",*

 * * "'mappings'": "'AACA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,kLAAkI,CAClI,gFACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,8KAA8H,CAC9H,+DACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,+KAA+H,CAC/H,oBACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,2KAA2H,CAC3H,yBACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,gLAAgI,CAChI,wGACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,e […]*

```diff
@@ -1,14 +1,15 @@
 {
-    "file": "2.c2136c50.chunk.css",
-    "mappings": "AACA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,0JAAkI,CAClI,gFACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,sJAA8H,CAC9H,wDACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,uJAA+H,CAC/H,oBACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,mJAA2H,CAC3H,yBACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,wJAAgI,CAChI,wGACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,uJAA+H,CAC/H,qGACF,CAEA,WACE,oBAAqB,CACrB,iBAAkB,CAClB,iBAAkB,CAClB,eAAgB,CAChB,mJAA2H,CAC3H,mJACF,CC9DA,6CAAqD,qBAAuB,CAAC,OAAQ,6KAAyL,CAAC,eAAgB,CAAC,yBAAkB,CAAlB,iBAAmB,CAAC,SAAU,iBAAkB,CAAC,cAAe,CAAC,eAAkB,CAAC,QAAS,iBAAkB,CAAC,wBAAiB,CAAjB,oBAAiB,CAAjB,gBAAkB,CAAC,iBAAmB,iBAAmB,CAAC,SAAU,eAAiB,CAAC,cAAe,aAAc,CAAC,iBAAkB,CAAC,UAAW,CAAC,WAAa,CAAC,UAAW,cAAe,CAAC,WAAY,CAAC,iBAAmB,CAAC,UAAW,aAAe,CAAC,YAAa,oBAAsB,CAAC,aAAc,iBAAmB,CAAC,aAAc,eAAiB,CAAC,eAAkB,qBAAsB,CAAC,oBAAsB,CAAC,oBAAqB,SAAU,CAAC,UAAW,CAAC,gBAAiB,CAAC,qCAAwC,CAAC,0BAA4B,WAAY,CAAC,qBAAuB,CAAC,gCAAiC,YAAc,CAAC,YAAe,WAAa,CAAC,aAAc,cAAgB,CAAC,mBAAsB,UAAa,CAAC,UAAW,0BAAqE,CAAC,kCAAzC,iBAAkB,CAAC,mBAA2I,CAArH,wBAA6C,MAAO,CAAC,KAAM,CAAsB,qBAAsB,CAAC,WAAa,CAAC,oCAAsC,WAAY,CAAC,+BAAiC,CAAC,oCAAsC,UAAW,CAAC,gCAAkC,CAAC,aAAc,iBAAkB,CAAC,KAAM,CAAC,MAAO,CAAC,iBAAkB,CAAC,mBAAoB,CAAC,qBAAsB,CAAC,WAAY,CAA0E,qCAAwC,CAAC,uEAA2E,YAAc",
+    "file": "static/css/main.79943053.css",
+    "mappings": "AACA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,kLAAkI,CAClI,gFACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,8KAA8H,CAC9H,+DACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,+KAA+H,CAC/H,oBACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,2KAA2H,CAC3H,yBACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,gLAAgI,CAChI,wGACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,+KAA+H,CAC/H,qGACF,CAEA,WAGE,iBAAkB,CAFlB,kBAAqB,CACrB,iBAAkB,CAElB,eAAgB,CAChB,2KAA2H,CAC3H,mJACF,CC9DA,6CAAqD,qBAAuB,CAAC,OAAQ,+JAAyL,CAAC,eAAgB,CAAC,yBAAkB,CAAlB,iBAAmB,CAAC,SAA6B,cAAe,CAAC,eAAiB,CAApD,iBAAqD,CAAC,QAAS,iBAAkB,CAAC,wBAAiB,CAAjB,gBAAkB,CAAC,iBAAmB,iBAAmB,CAAC,SAAU,eAAiB,CAAC,cAAe,aAAc,CAAgC,WAAY,CAA3C,iBAAkB,CAAC,UAAyB,CAAC,QAAS,iBAAmB,CAAC,UAAW,cAAe,CAAC,WAAY,CAAC,iBAAmB,CAAC,UAAW,aAAe,CAAC,YAAa,oBAAsB,CAAC,aAAc,iBAAmB,CAAC,aAAc,eAAiB,CAAC,eAAyC,oBAAqB,CAA5C,qBAA6C,CAAC,oBAA8D,qCAAuC,CAArE,UAAW,CAAC,gBAAiB,CAAxC,SAAiF,CAAC,0BAA4B,WAAY,CAAC,qBAAuB,CAAC,gCAAiC,YAAc,CAAC,YAAe,WAAa,CAAC,aAAc,cAAgB,CAAC,mBAAsB,UAAa,CAAC,UAAW,0BAAqE,CAAC,kCAAtB,mBAAoB,CAAvC,iBAA8J,CAArH,wBAA6C,MAAO,CAAC,KAAM,CAAsB,qBAAsB,CAAC,WAAa,CAAC,oCAAmD,+BAAgC,CAA7C,WAA8C,CAAC,oCAAkD,gCAAiC,CAA7C,UAA8C,CAAC,aAAqN,qCAAuC,CAAzL,cAAe,CAAlC,iBAAkB,CAA1B,MAAO,CAAoC,mBAAoB,CAAzF,iBAAkB,CAAC,KAAM,CAAiE,qBAAsB,CAAC,WAA8H,CAAC,qFAA0F,YAAc",
     "names": [],
+    "sourceRoot": "",
     "sources": [
-        "webpack://node_modules/@fontsource/roboto/index.css",
-        "webpack://node_modules/uplot/dist/uPlot.min.css"
+        "../node_modules/@fontsource/roboto/index.css",
+        "../node_modules/uplot/dist/uPlot.min.css"
     ],
     "sourcesContent": [
-        "/* roboto-cyrillic-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-cyrillic-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;\n}\n/* roboto-cyrillic-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-cyrillic-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;\n}\n/* roboto-greek-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-greek-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+1F00-1FFF;\n}\n/* roboto-greek-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-greek-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0370-03FF;\n}\n/* roboto-vietnamese-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-vietnamese-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+1EA0-1EF9, U+20AB;\n}\n/* roboto-latin-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-latin-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;\n}\n/* roboto-latin-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-latin-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;\n}\n",
-        ".uplot, .uplot *, .uplot *::before, .uplot *::after {box-sizing: border-box;}.uplot {font-family: system-ui, -apple-system, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, \"Noto Sans\", sans-serif, \"Apple Color Emoji\", \"Segoe UI Emoji\", \"Segoe UI Symbol\", \"Noto Color Emoji\";line-height: 1.5;width: min-content;}.u-title {text-align: center;font-size: 18px;font-weight: bold;}.u-wrap {position: relative;user-select: none;}.u-over, .u-under {position: absolute;}.u-under {overflow: hidden;}.uplot canvas {display: block;position: relative;width: 100%;height: 100%;}.u-legend {font-size: 14px;margin: auto;text-align: center;}.u-inline {display: block;}.u-inline * {display: inline-block;}.u-inline tr {margin-right: 16px;}.u-legend th {font-weight: 600;}.u-legend th > * {vertical-align: middle;display: inline-block;}.u-legend .u-marker {width: 1em;height: 1em;margin-right: 4px;background-clip: content-box !important;}.u-inline.u-live th::after {content: \":\";vertical-align: middle;}.u-inline:not(.u-live) .u-value {display: none;}.u-series > * {padding: 4px;}.u-series th {cursor: pointer;}.u-legend .u-off > * {opacity: 0.3;}.u-select {background: rgba(0,0,0,0.07);position: absolute;pointer-events: none;}.u-cursor-x, .u-cursor-y {position: absolute;left: 0;top: 0;pointer-events: none;will-change: transform;z-index: 100;}.u-hz .u-cursor-x, .u-vt .u-cursor-y {height: 100%;border-right: 1px dashed #607D8B;}.u-hz .u-cursor-y, .u-vt .u-cursor-x {width: 100%;border-bottom: 1px dashed #607D8B;}.u-cursor-pt {position: absolute;top: 0;left: 0;border-radius: 50%;pointer-events: none;will-change: transform;z-index: 100;/*this has to be !important since we set inline \"background\" shorthand */background-clip: content-box !important;}.u-select.u-off, .u-cursor-x.u-off, .u-cursor-y.u-off, .u-cursor-pt.u-off {display: none;}"
+        "/* roboto-cyrillic-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-cyrillic-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F;\n}\n/* roboto-cyrillic-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-cyrillic-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;\n}\n/* roboto-greek-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-greek-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+1F00-1FFF;\n}\n/* roboto-greek-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-greek-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0370-03FF;\n}\n/* roboto-vietnamese-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-vietnamese-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;\n}\n/* roboto-latin-ext-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-latin-ext-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;\n}\n/* roboto-latin-400-normal*/\n@font-face {\n  font-family: 'Roboto';\n  font-style: normal;\n  font-display: swap;\n  font-weight: 400;\n  src: url('./files/roboto-latin-400-normal.woff2') format('woff2'), url('./files/roboto-all-400-normal.woff') format('woff');\n  unicode-range: U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;\n}\n",
+        ".uplot, .uplot *, .uplot *::before, .uplot *::after {box-sizing: border-box;}.uplot {font-family: system-ui, -apple-system, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, \"Noto Sans\", sans-serif, \"Apple Color Emoji\", \"Segoe UI Emoji\", \"Segoe UI Symbol\", \"Noto Color Emoji\";line-height: 1.5;width: min-content;}.u-title {text-align: center;font-size: 18px;font-weight: bold;}.u-wrap {position: relative;user-select: none;}.u-over, .u-under {position: absolute;}.u-under {overflow: hidden;}.uplot canvas {display: block;position: relative;width: 100%;height: 100%;}.u-axis {position: absolute;}.u-legend {font-size: 14px;margin: auto;text-align: center;}.u-inline {display: block;}.u-inline * {display: inline-block;}.u-inline tr {margin-right: 16px;}.u-legend th {font-weight: 600;}.u-legend th > * {vertical-align: middle;display: inline-block;}.u-legend .u-marker {width: 1em;height: 1em;margin-right: 4px;background-clip: padding-box !important;}.u-inline.u-live th::after {content: \":\";vertical-align: middle;}.u-inline:not(.u-live) .u-value {display: none;}.u-series > * {padding: 4px;}.u-series th {cursor: pointer;}.u-legend .u-off > * {opacity: 0.3;}.u-select {background: rgba(0,0,0,0.07);position: absolute;pointer-events: none;}.u-cursor-x, .u-cursor-y {position: absolute;left: 0;top: 0;pointer-events: none;will-change: transform;z-index: 100;}.u-hz .u-cursor-x, .u-vt .u-cursor-y {height: 100%;border-right: 1px dashed #607D8B;}.u-hz .u-cursor-y, .u-vt .u-cursor-x {width: 100%;border-bottom: 1px dashed #607D8B;}.u-cursor-pt {position: absolute;top: 0;left: 0;border-radius: 50%;border: 0 solid;pointer-events: none;will-change: transform;z-index: 100;/*this has to be !important since we set inline \"background\" shorthand */background-clip: padding-box !important;}.u-axis.u-off, .u-select.u-off, .u-cursor-x.u-off, .u-cursor-y.u-off, .u-cursor-pt.u-off {display: none;}"
     ],
     "version": 3
 }
```

### Comparing `ezbeq-0.9.3/ezbeq.egg-info/requires.txt` & `ezbeq-1.0.0b1/ezbeq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.3/setup.py` & `ezbeq-1.0.0b1/setup.py`

 * *Files identical despite different names*

