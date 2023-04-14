# Comparing `tmp/unigui-1.3.5.tar.gz` & `tmp/unigui-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigui-1.3.5.tar", last modified: Sun Mar 26 00:36:38 2023, max compression
+gzip compressed data, was "unigui-1.3.6.tar", last modified: Fri Apr 14 15:04:56 2023, max compression
```

## Comparing `unigui-1.3.5.tar` & `unigui-1.3.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.5/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.5/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-03-26 00:36:38.444654 unigui-1.3.5/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)    18581 2023-03-08 16:33:36.000000 unigui-1.3.5/README.md
--rw-r--r--   0 george    (1000) george    (1000)       38 2023-03-26 00:36:38.444654 unigui-1.3.5/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      565 2023-03-26 00:35:05.000000 unigui-1.3.5/setup.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.441321 unigui-1.3.5/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.5/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     7493 2023-03-08 16:33:36.000000 unigui-1.3.5/unigui/guielements.py
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.5/unigui/manager.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.5/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.5/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.5/unigui/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui/web/
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui/web/css/
--rw-r--r--   0 george    (1000) george    (1000)     3290 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/css/366.84f6b400.css
--rw-r--r--   0 george    (1000) george    (1000)        0 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/css/app.31d6cfe0.css
--rw-r--r--   0 george    (1000) george    (1000)   219590 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/css/vendor.49a52e8f.css
--rw-r--r--   0 george    (1000) george    (1000)    64483 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/favicon.ico
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui/web/fonts/
--rw-r--r--   0 george    (1000) george    (1000)    20436 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 george    (1000) george    (1000)    20544 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 george    (1000) george    (1000)    20416 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 george    (1000) george    (1000)    20408 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 george    (1000) george    (1000)    20424 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 george    (1000) george    (1000)    20344 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 george    (1000) george    (1000)   164912 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 george    (1000) george    (1000)   128360 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui/web/icons/
--rw-r--r--   0 george    (1000) george    (1000)    12324 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/icons/favicon-128x128.png
--rw-r--r--   0 george    (1000) george    (1000)      859 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/icons/favicon-16x16.png
--rw-r--r--   0 george    (1000) george    (1000)     2039 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/icons/favicon-32x32.png
--rw-r--r--   0 george    (1000) george    (1000)     9643 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/icons/favicon-96x96.png
--rw-r--r--   0 george    (1000) george    (1000)      907 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/index.html
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui/web/js/
--rw-r--r--   0 george    (1000) george    (1000)      763 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/js/193.b4cc3ffe.js
--rw-r--r--   0 george    (1000) george    (1000)    39474 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/js/366.8fcd6776.js
--rw-r--r--   0 george    (1000) george    (1000)     6560 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/js/430.4be6e8a8.js
--rw-r--r--   0 george    (1000) george    (1000)     5867 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/js/app.03336b1a.js
--rw-r--r--   0 george    (1000) george    (1000)   847622 2023-03-26 00:31:14.000000 unigui-1.3.5/unigui/web/js/vendor.c0de6c67.js
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-03-26 00:36:38.444654 unigui-1.3.5/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-03-26 00:36:38.000000 unigui-1.3.5/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-03-26 00:36:38.000000 unigui-1.3.5/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-03-26 00:36:38.000000 unigui-1.3.5/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.5/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-03-26 00:36:38.000000 unigui-1.3.5/unigui.egg-info/top_level.txt
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.218741 unigui-1.3.6/
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.6/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.6/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-14 15:04:56.218741 unigui-1.3.6/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)    18581 2023-03-08 16:33:36.000000 unigui-1.3.6/README.md
+-rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-14 15:04:56.218741 unigui-1.3.6/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-14 15:04:24.000000 unigui-1.3.6/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.212074 unigui-1.3.6/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.6/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     7493 2023-03-08 16:33:36.000000 unigui-1.3.6/unigui/guielements.py
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.6/unigui/manager.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.6/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.6/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.6/unigui/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/css/
+-rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/993.ac2fa104.css
+-rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/app.31d6cfe0.css
+-rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/css/vendor.49a52e8f.css
+-rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/favicon.ico
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/fonts/
+-rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/icons/
+-rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-128x128.png
+-rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-16x16.png
+-rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-32x32.png
+-rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/icons/favicon-96x96.png
+-rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/index.html
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui/web/js/
+-rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/193.b4cc3ffe.js
+-rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/430.4be6e8a8.js
+-rw-r--r--   0 george    (1000) george    (1000)    39467 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/993.814659bd.js
+-rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/app.f2f7d718.js
+-rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-14 15:00:21.000000 unigui-1.3.6/unigui/web/js/vendor.c0de6c67.js
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-14 15:04:56.215407 unigui-1.3.6/unigui.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.6/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-14 15:04:56.000000 unigui-1.3.6/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.3.5/LICENSE` & `unigui-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/PKG-INFO` & `unigui-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.5
+Version: 1.3.6
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `unigui-1.3.5/README.md` & `unigui-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/setup.py` & `unigui-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.3.5',      
+      version='1.3.6',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.3.5/unigui/guielements.py` & `unigui-1.3.6/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/manager.py` & `unigui-1.3.6/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/server.py` & `unigui-1.3.6/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/utils.py` & `unigui-1.3.6/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/css/366.84f6b400.css` & `unigui-1.3.6/unigui/web/css/993.ac2fa104.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-3bf1da74]{display:flex;justify-content:center}.custom-caption[data-v-3bf1da74]{padding:5px!important}.web-camera-container[data-v-3bf1da74]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-3bf1da74]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-3bf1da74]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-3bf1da74]{opacity:1}.web-camera-container .camera-shoot[data-v-3bf1da74]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-3bf1da74]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-3bf1da74]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-3bf1da74]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-3bf1da74]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-3bf1da74]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]{animation:preload-3bf1da74 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(3){animation-delay:.4s}@keyframes preload-3bf1da74{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-3bf1da74]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}body{overflow-y:hidden}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-3bf1da74]{display:flex;justify-content:center}.custom-caption[data-v-3bf1da74]{padding:5px!important}.web-camera-container[data-v-3bf1da74]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-3bf1da74]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-3bf1da74]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-3bf1da74]{opacity:1}.web-camera-container .camera-shoot[data-v-3bf1da74]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-3bf1da74]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-3bf1da74]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-3bf1da74]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-3bf1da74]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-3bf1da74]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]{animation:preload-3bf1da74 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-3bf1da74]:nth-child(3){animation-delay:.4s}@keyframes preload-3bf1da74{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-3bf1da74]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.3.5/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.3.6/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/favicon.ico` & `unigui-1.3.6/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.3.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.3.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.3.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.3.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/icons/favicon-128x128.png` & `unigui-1.3.6/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/icons/favicon-16x16.png` & `unigui-1.3.6/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/icons/favicon-32x32.png` & `unigui-1.3.6/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/icons/favicon-96x96.png` & `unigui-1.3.6/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/index.html` & `unigui-1.3.6/unigui/web/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.03336b1a.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.f2f7d718.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.3.5/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.3.6/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/js/366.8fcd6776.js` & `unigui-1.3.6/unigui/web/js/993.814659bd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [366], {
-        366: (e, t, a) => {
+    [993], {
+        4993: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Ot
             });
             var l = a(3673),
                 s = a(2323);
             const o = (0, l._)("div", {
                 class: "q-pa-lg"
@@ -54,15 +54,15 @@
                                 _: 1
                             }, 8, ["modelValue"])])),
                             _: 1
                         })])),
                         _: 1
                     }), (0, l.Wm)(f, null, {
                         default: (0, l.w5)((() => [(0, l.Wm)(m, {
-                            class: "flex q-pa-sm justify-center centers"
+                            class: "flex justify-center centers"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Wm)(g, {
                                 data: e.screen.blocks
                             }, null, 8, ["data"])])),
                             _: 1
                         })])),
                         _: 1
```

### Comparing `unigui-1.3.5/unigui/web/js/430.4be6e8a8.js` & `unigui-1.3.6/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui/web/js/app.03336b1a.js` & `unigui-1.3.6/unigui/web/js/app.f2f7d718.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(366)]).then(r.bind(r, 366)),
+                        component: () => Promise.all([r.e(736), r.e(993)]).then(r.bind(r, 4993)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -159,25 +159,25 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
-            366: "8fcd6776",
-            430: "4be6e8a8"
+            430: "4be6e8a8",
+            993: "814659bd"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            366: "84f6b400",
-            736: "49a52e8f"
+            736: "49a52e8f",
+            993: "ac2fa104"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                366: 1
+                993: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.3.5/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.3.6/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.5/unigui.egg-info/PKG-INFO` & `unigui-1.3.6/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.5
+Version: 1.3.6
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `unigui-1.3.5/unigui.egg-info/SOURCES.txt` & `unigui-1.3.6/unigui.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/366.84f6b400.css
+unigui/web/css/993.ac2fa104.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +27,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
-unigui/web/js/366.8fcd6776.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/app.03336b1a.js
+unigui/web/js/993.814659bd.js
+unigui/web/js/app.f2f7d718.js
 unigui/web/js/vendor.c0de6c67.js
```

