# Comparing `tmp/pyvts-0.2.2.macosx-13-arm64.tar.gz` & `tmp/pyvts-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.2.macosx-13-arm64.tar", last modified: Mon Apr 10 22:16:39 2023, max compression
+gzip compressed data, was "pyvts-0.2.4.tar", last modified: Fri Apr 14 15:39:51 2023, max compression
```

## Comparing `pyvts-0.2.2.macosx-13-arm64.tar` & `pyvts-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198736 ./
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198759 ./Users/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198783 ./Users/genteki/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198805 ./Users/genteki/.virtualenvs/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198829 ./Users/genteki/.virtualenvs/live2d/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198856 ./Users/genteki/.virtualenvs/live2d/lib/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198882 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198950 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.199900 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:16:39.195509 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:16:39.198613 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195626 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:16:39.195767 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195844 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:39:51.795604 pyvts-0.2.4/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.4/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:39:51.795467 pyvts-0.2.4/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     2658 2023-04-14 15:36:17.000000 pyvts-0.2.4/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:39:51.794639 pyvts-0.2.4/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-14 15:39:43.000000 pyvts-0.2.4/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.4/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.4/pyvts/error.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.2.4/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10148 2023-04-14 15:36:17.000000 pyvts-0.2.4/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:39:51.795254 pyvts-0.2.4/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:39:51.000000 pyvts-0.2.4/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-14 15:39:51.000000 pyvts-0.2.4/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:39:51.000000 pyvts-0.2.4/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-14 15:39:51.000000 pyvts-0.2.4/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:39:51.000000 pyvts-0.2.4/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 15:39:51.795645 pyvts-0.2.4/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1222 2023-04-14 15:39:40.000000 pyvts-0.2.4/setup.py
```

### Comparing `./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO` & `pyvts-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.2
+Version: 0.2.4
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyvts
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
 [![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
@@ -45,29 +46,37 @@
 
 First import library you need,
 ```
 import pyvts
 import asyncio
 ```
 
-Then specify your plugin information
+Create an instance with default values, and do whateveer you want!
 ```
-plugin_info = {
-    "plugin_name": "[plugin name]",
-    "developer": "[your name]",
-    "authentication_token_path": "./token.txt",
-}
+async def main():
+    vts = pyvts.vts()
+    await vts.connect()
+    # Implement what you want to do
+    await vts.close()
+
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
-Create an instance and do whateveer you want!
+
+Example of a call animation by emulating pressing HotKeys
 ```
 async def main():
     vts = pyvts.vts(plugin_info=plugin_info)
     await vts.connect()
-    # Implement what you want to do
-    await vts.close()
+    await vts.request_authenticate_token()  # get token
+    await vts.request_authenticate()  # use token
+    b = await vts.request(vts.vts_request.requestHotKeyList())
+    hotKeyList = [hotKey['name'] for hotKey in b['data']['availableHotkeys']]
+    print(hotKeyList) # ['My Animation 1', 'My Animation 2', 'My Animation 3']
+    await vts.request(vts.vts_request.requestTriggerHotKey(hotKeyList[0])) # send request to play 'My Animation 1'
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 
 ### Demo
```

