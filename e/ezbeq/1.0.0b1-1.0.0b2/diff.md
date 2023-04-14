# Comparing `tmp/ezbeq-1.0.0b1.tar.gz` & `tmp/ezbeq-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.0b1.tar", last modified: Fri Apr 14 19:57:49 2023, max compression
+gzip compressed data, was "ezbeq-1.0.0b2.tar", last modified: Fri Apr 14 20:15:49 2023, max compression
```

## Comparing `ezbeq-1.0.0b1.tar` & `ezbeq-1.0.0b2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.107607 ezbeq-1.0.0b1/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.111607 ezbeq-1.0.0b1/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/iir.py
--rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/minidsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/ezbeq/qsys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.115607 ezbeq-1.0.0b1/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 19:56:07.000000 ezbeq-1.0.0b1/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.103607 ezbeq-1.0.0b1/ezbeq/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.115607 ezbeq-1.0.0b1/ezbeq/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.119608 ezbeq-1.0.0b1/ezbeq/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   937350 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  4111826 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/ezbeq/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-14 19:56:58.000000 ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.111607 ezbeq-1.0.0b1/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 19:57:49.000000 ezbeq-1.0.0b1/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:57:49.127607 ezbeq-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-04-14 19:54:40.000000 ezbeq-1.0.0b1/tests/test_minidsp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.592962 ezbeq-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 20:15:49.592962 ezbeq-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.576962 ezbeq-1.0.0b2/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 20:15:08.000000 ezbeq-1.0.0b2/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.580962 ezbeq-1.0.0b2/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/iir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/minidsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/ezbeq/qsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.584962 ezbeq-1.0.0b2/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 20:14:26.000000 ezbeq-1.0.0b2/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.576962 ezbeq-1.0.0b2/ezbeq/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.584962 ezbeq-1.0.0b2/ezbeq/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/css/main.79943053.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/css/main.79943053.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.584962 ezbeq-1.0.0b2/ezbeq/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   937350 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4111826 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.592962 ezbeq-1.0.0b2/ezbeq/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-14 20:15:07.000000 ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.580962 ezbeq-1.0.0b2/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 20:15:49.000000 ezbeq-1.0.0b2/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:15:49.592962 ezbeq-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:15:49.592962 ezbeq-1.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-04-14 20:13:13.000000 ezbeq-1.0.0b2/tests/test_minidsp_api.py
```

### Comparing `ezbeq-1.0.0b1/LICENSE` & `ezbeq-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/PKG-INFO` & `ezbeq-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b1/README.md` & `ezbeq-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.0b2/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/catalogue.py` & `ezbeq-1.0.0b2/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.0b2/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/devices.py` & `ezbeq-1.0.0b2/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/languages.py` & `ezbeq-1.0.0b2/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/meta.py` & `ezbeq-1.0.0b2/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/search.py` & `ezbeq-1.0.0b2/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/ws.py` & `ezbeq-1.0.0b2/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/apis/years.py` & `ezbeq-1.0.0b2/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/catalogue.py` & `ezbeq-1.0.0b2/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/config.py` & `ezbeq-1.0.0b2/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/device.py` & `ezbeq-1.0.0b2/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/htp1.py` & `ezbeq-1.0.0b2/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/iir.py` & `ezbeq-1.0.0b2/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/jriver.py` & `ezbeq-1.0.0b2/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/main.py` & `ezbeq-1.0.0b2/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/minidsp.py` & `ezbeq-1.0.0b2/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/qsys.py` & `ezbeq-1.0.0b2/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.0b2/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.0b2/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.0b2/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/asset-manifest.json` & `ezbeq-1.0.0b2/ezbeq/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.0b2/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.0b2/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/favicon.ico` & `ezbeq-1.0.0b2/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/index.html` & `ezbeq-1.0.0b2/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.0b2/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.0b2/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css` & `ezbeq-1.0.0b2/ezbeq/ui/static/css/main.79943053.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/css/main.79943053.css.map` & `ezbeq-1.0.0b2/ezbeq/ui/static/css/main.79943053.css.map`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js` & `ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.LICENSE.txt` & `ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/js/main.592660fa.js.map` & `ezbeq-1.0.0b2/ezbeq/ui/static/js/main.592660fa.js.map`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2` & `ezbeq-1.0.0b2/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/ezbeq.egg-info/PKG-INFO` & `ezbeq-1.0.0b2/ezbeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b1/ezbeq.egg-info/SOURCES.txt` & `ezbeq-1.0.0b2/ezbeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b1/setup.py` & `ezbeq-1.0.0b2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,46 +27,51 @@
     author_email="mattkhan+ezbeq@gmail.com",
     license="MIT",
     packages=find_packages(exclude=("test", "docs")),
     python_requires=">=3.7",
     entry_points={"console_scripts": ["ezbeq = ezbeq.main:main",],},
     install_requires=[
         "aniso8601==9.0.1; python_version >= '3.5'",
-        "attrs==21.2.0",
-        "autobahn[twisted]==21.3.1",
-        "automat==20.2.0",
+        "attrs==22.2.0; python_version >= '3.6'",
+        "autobahn[twisted]==23.1.2",
+        "automat==22.10.0",
         "brotli==1.0.9",
-        "certifi==2020.12.5",
-        "cffi==1.14.5",
-        "chardet==4.0.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-        "click==7.1.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+        "certifi==2022.12.7; python_version >= '3.6'",
+        "cffi==1.15.1",
+        "charset-normalizer==3.1.0; python_version >= '3.7'",
+        "click==8.1.3; python_version >= '3.7'",
         "constantly==15.1.0",
-        "cryptography==3.4.7; python_version >= '3.6'",
-        "flask==1.1.4; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-        "flask-compress==1.9.0",
-        "flask-restx==0.4.0",
+        "cryptography==40.0.2; python_version >= '3.6'",
+        "flask==2.2.3; python_version >= '3.7'",
+        "flask-compress==1.13",
+        "flask-restx==1.1.0",
         "hyperlink==21.0.0",
-        "idna==2.10; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-        "incremental==21.3.0",
-        "itsdangerous==1.1.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-        "jinja2==2.11.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-        "jsonschema==3.2.0",
-        "markupsafe==2.0.1; python_version >= '3.6'",
-        "plumbum==1.7.0",
-        "pycparser==2.20; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-        "pyrsistent==0.17.3; python_version >= '3.5'",
-        "python-dateutil==2.8.1",
-        "pytz==2021.1",
-        "pyyaml==5.4.1",
-        "requests==2.25.1",
-        "semver==2.13.0",
+        "idna==3.4; python_version >= '3.5'",
+        "importlib-metadata==6.3.0; python_version < '3.10'",
+        "importlib-resources==5.12.0",
+        "incremental==22.10.0",
+        "itsdangerous==2.1.2; python_version >= '3.7'",
+        "jinja2==3.1.2; python_version >= '3.7'",
+        "jsonschema==4.17.3; python_version >= '3.7'",
+        "markupsafe==2.1.2; python_version >= '3.7'",
+        "plumbum==1.8.1",
+        "pycparser==2.21; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+        "pyrsistent==0.19.3; python_version >= '3.7'",
+        "python-dateutil==2.8.2",
+        "pytz==2023.3",
+        "pyyaml==6.0",
+        "requests==2.28.2",
+        "semver==3.0.0",
+        "setuptools==67.6.1; python_version >= '3.7'",
         "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-        "twisted==21.2.0",
-        "txaio==21.2.1; python_version >= '3.6'",
-        "urllib3==1.26.5; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-        "werkzeug==1.0.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-        "zope.interface==5.4.0",
+        "twisted==22.10.0",
+        "txaio==23.1.1; python_version >= '3.7'",
+        "typing-extensions==4.5.0; python_version >= '3.7'",
+        "urllib3==1.26.15; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+        "werkzeug==2.2.3; python_version >= '3.7'",
+        "zipp==3.15.0; python_version < '3.10'",
+        "zope.interface==6.0; python_version >= '3.7'"
     ],
     tests_require=["pytest", "pytest-httpserver"],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `ezbeq-1.0.0b1/tests/test_minidsp_api.py` & `ezbeq-1.0.0b2/tests/test_minidsp_api.py`

 * *Files identical despite different names*

