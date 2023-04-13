# Comparing `tmp/ezbeq-0.9.2.tar.gz` & `tmp/ezbeq-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ezbeq-0.9.2.tar", last modified: Sun Jun 27 09:16:47 2021, max compression
+gzip compressed data, was "dist/ezbeq-0.9.3.tar", last modified: Wed Aug 11 18:57:06 2021, max compression
```

## Comparing `ezbeq-0.9.2.tar` & `ezbeq-0.9.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-06-27 09:13:38.000000 ezbeq-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-06-27 09:13:38.000000 ezbeq-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-06-27 09:16:47.000000 ezbeq-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-06-27 09:13:38.000000 ezbeq-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-27 09:15:31.000000 ezbeq-0.9.2/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    17190 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (121)    11689 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)     8306 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (121)    22580 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7070 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    24634 2021-06-27 09:13:38.000000 ezbeq-0.9.2/ezbeq/minidsp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)    14091 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-06-27 09:15:01.000000 ezbeq-0.9.2/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/css/2.c2136c50.chunk.css
--rw-r--r--   0 runner    (1001) docker     (121)     5955 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/css/2.c2136c50.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)   623905 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     4762 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2426595 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)    45911 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/main.a57863b7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)   134396 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/main.a57863b7.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/runtime-main.51078455.js
--rw-r--r--   0 runner    (1001) docker     (121)     8270 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/js/runtime-main.51078455.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    66044 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-all-400-normal.b5a0a0df.woff
--rw-r--r--   0 runner    (1001) docker     (121)     9900 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-cyrillic-400-normal.3605d18d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15520 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     7296 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-greek-400-normal.352cc77a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15736 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-latin-400-normal.176f8f5b.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    12200 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-06-27 09:15:30.000000 ezbeq-0.9.2/ezbeq/ui/static/media/roboto-vietnamese-400-normal.52cebac0.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-27 09:16:47.000000 ezbeq-0.9.2/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-27 09:16:47.000000 ezbeq-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-06-27 09:13:38.000000 ezbeq-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-08-11 18:54:08.000000 ezbeq-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-08-11 18:54:08.000000 ezbeq-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-08-11 18:57:06.000000 ezbeq-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-08-11 18:54:08.000000 ezbeq-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17190 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4718 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11689 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8306 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11982 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22580 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7070 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24652 2021-08-11 18:54:08.000000 ezbeq-0.9.3/ezbeq/minidsp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14091 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3262 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7406 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2533 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-08-11 18:55:19.000000 ezbeq-0.9.3/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     3911 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (121)     5955 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)   623905 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4762 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  2426595 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (121)    45911 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)   134396 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8270 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js.map
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (121)    66044 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-all-400-normal.b5a0a0df.woff
+-rw-r--r--   0 runner    (1001) docker     (121)     9900 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-400-normal.3605d18d.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    15520 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)     7296 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-400-normal.352cc77a.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    15736 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-400-normal.176f8f5b.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    12200 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-08-11 18:55:44.000000 ezbeq-0.9.3/ezbeq/ui/static/media/roboto-vietnamese-400-normal.52cebac0.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-11 18:57:06.000000 ezbeq-0.9.3/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 18:57:06.000000 ezbeq-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-08-11 18:54:08.000000 ezbeq-0.9.3/setup.py
```

### Comparing `ezbeq-0.9.2/LICENSE` & `ezbeq-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/PKG-INFO` & `ezbeq-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 0.9.2
+Version: 0.9.3
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Description: # ezbeq
```

### Comparing `ezbeq-0.9.2/README.md` & `ezbeq-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/audiotypes.py` & `ezbeq-0.9.3/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/catalogue.py` & `ezbeq-0.9.3/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/contenttypes.py` & `ezbeq-0.9.3/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/devices.py` & `ezbeq-0.9.3/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/meta.py` & `ezbeq-0.9.3/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/search.py` & `ezbeq-0.9.3/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/ws.py` & `ezbeq-0.9.3/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/apis/years.py` & `ezbeq-0.9.3/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/catalogue.py` & `ezbeq-0.9.3/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/config.py` & `ezbeq-0.9.3/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/device.py` & `ezbeq-0.9.3/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/htp1.py` & `ezbeq-0.9.3/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/jriver.py` & `ezbeq-0.9.3/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/main.py` & `ezbeq-0.9.3/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/minidsp.py` & `ezbeq-0.9.3/ezbeq/minidsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,27 +192,27 @@
         return True
 
     def __load_state(self) -> MinidspState:
         result = self.__executor.submit(self.__read_state_from_device).result(timeout=self.__cmd_timeout)
         return result if result else MinidspState(self.name)
 
     def __read_state_from_device(self) -> Optional[MinidspState]:
-        lines = None
+        output = None
         try:
             kwargs = {'retcode': None} if self.__ignore_retcode else {}
             output = self.__runner['-o', 'jsonline'](timeout=self.__cmd_timeout, **kwargs)
-            status = json.loads(output)
+            status = json.loads(output.splitlines()[0])
             values = {
                 'active_slot': str(status['master']['preset'] + 1),
                 'mute': status['master']['mute'],
                 'mv': status['master']['volume']
             }
             return MinidspState(self.name, **values)
         except:
-            logger.exception(f"Unable to parse device state {lines}")
+            logger.exception(f"Unable to parse device state {output}")
             return None
 
     @staticmethod
     def __as_idx(idx: Union[int, str]):
         return int(idx) - 1
 
     def __send_cmds(self, target_slot_idx: Optional[int], cmds: List[str]):
```

### Comparing `ezbeq-0.9.2/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-0.9.3/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-0.9.3/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/apple-touch-icon.png` & `ezbeq-0.9.3/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/asset-manifest.json` & `ezbeq-0.9.3/ezbeq/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/favicon-16x16.png` & `ezbeq-0.9.3/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/favicon-32x32.png` & `ezbeq-0.9.3/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/favicon.ico` & `ezbeq-0.9.3/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/index.html` & `ezbeq-0.9.3/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/mstile-150x150.png` & `ezbeq-0.9.3/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-0.9.3/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/css/2.c2136c50.chunk.css` & `ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/css/2.c2136c50.chunk.css.map` & `ezbeq-0.9.3/ezbeq/ui/static/css/2.c2136c50.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js` & `ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.LICENSE.txt` & `ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.map` & `ezbeq-0.9.3/ezbeq/ui/static/js/2.d43f1ad6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/main.a57863b7.chunk.js` & `ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/main.a57863b7.chunk.js.map` & `ezbeq-0.9.3/ezbeq/ui/static/js/main.a57863b7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/runtime-main.51078455.js` & `ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/js/runtime-main.51078455.js.map` & `ezbeq-0.9.3/ezbeq/ui/static/js/runtime-main.51078455.js.map`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-all-400-normal.b5a0a0df.woff` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-all-400-normal.b5a0a0df.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-cyrillic-400-normal.3605d18d.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-400-normal.3605d18d.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.dd55ea0a.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-greek-400-normal.352cc77a.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-400-normal.352cc77a.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-greek-ext-400-normal.bc7ace6e.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-latin-400-normal.176f8f5b.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-400-normal.176f8f5b.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-latin-ext-400-normal.dcc07bcf.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq/ui/static/media/roboto-vietnamese-400-normal.52cebac0.woff2` & `ezbeq-0.9.3/ezbeq/ui/static/media/roboto-vietnamese-400-normal.52cebac0.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq.egg-info/PKG-INFO` & `ezbeq-0.9.3/ezbeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 0.9.2
+Version: 0.9.3
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Description: # ezbeq
```

### Comparing `ezbeq-0.9.2/ezbeq.egg-info/SOURCES.txt` & `ezbeq-0.9.3/ezbeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/ezbeq.egg-info/requires.txt` & `ezbeq-0.9.3/ezbeq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-0.9.2/setup.py` & `ezbeq-0.9.3/setup.py`

 * *Files identical despite different names*

