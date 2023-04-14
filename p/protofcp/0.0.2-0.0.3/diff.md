# Comparing `tmp/protofcp-0.0.2.tar.gz` & `tmp/protofcp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protofcp-0.0.2.tar", last modified: Fri Apr 14 14:07:17 2023, max compression
+gzip compressed data, was "protofcp-0.0.3.tar", last modified: Fri Apr 14 16:01:03 2023, max compression
```

## Comparing `protofcp-0.0.2.tar` & `protofcp-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:07:17.751561 protofcp-0.0.2/
--rw-rw-rw-   0        0        0    11542 2023-04-14 13:43:37.000000 protofcp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1723 2023-04-14 14:07:17.750550 protofcp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2023-04-14 14:02:43.000000 protofcp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 14:07:17.738891 protofcp-0.0.2/protofcp/
--rw-rw-rw-   0        0        0     1211 2023-04-14 14:01:26.000000 protofcp-0.0.2/protofcp/FCPSocket.py
--rw-rw-rw-   0        0        0      243 2023-04-14 14:01:04.000000 protofcp-0.0.2/protofcp/__init__.py
--rw-rw-rw-   0        0        0      499 2023-04-13 23:30:51.000000 protofcp-0.0.2/protofcp/assemblr.py
--rw-rw-rw-   0        0        0      444 2023-04-14 12:04:20.000000 protofcp-0.0.2/protofcp/consts.py
--rw-rw-rw-   0        0        0      826 2023-04-13 23:41:00.000000 protofcp-0.0.2/protofcp/disassemblr.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:07:17.748550 protofcp-0.0.2/protofcp.egg-info/
--rw-rw-rw-   0        0        0     1723 2023-04-14 14:07:17.000000 protofcp-0.0.2/protofcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-14 14:07:17.000000 protofcp-0.0.2/protofcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:07:17.000000 protofcp-0.0.2/protofcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 14:07:17.000000 protofcp-0.0.2/protofcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 14:07:17.000000 protofcp-0.0.2/protofcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 14:07:17.751561 protofcp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-14 14:06:04.000000 protofcp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.747518 protofcp-0.0.3/
+-rw-rw-rw-   0        0        0    11542 2023-04-14 13:43:37.000000 protofcp-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1723 2023-04-14 16:01:03.747518 protofcp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2023-04-14 14:02:43.000000 protofcp-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.725694 protofcp-0.0.3/protofcp/
+-rw-rw-rw-   0        0        0     1277 2023-04-14 15:56:52.000000 protofcp-0.0.3/protofcp/FCPSocket.py
+-rw-rw-rw-   0        0        0      243 2023-04-14 14:01:04.000000 protofcp-0.0.3/protofcp/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 23:30:51.000000 protofcp-0.0.3/protofcp/assemblr.py
+-rw-rw-rw-   0        0        0      444 2023-04-14 12:04:20.000000 protofcp-0.0.3/protofcp/consts.py
+-rw-rw-rw-   0        0        0      826 2023-04-13 23:41:00.000000 protofcp-0.0.3/protofcp/disassemblr.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.745510 protofcp-0.0.3/protofcp.egg-info/
+-rw-rw-rw-   0        0        0     1723 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:01:03.747518 protofcp-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-04-14 15:06:11.000000 protofcp-0.0.3/setup.py
```

### Comparing `protofcp-0.0.2/LICENSE` & `protofcp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.2/PKG-INFO` & `protofcp-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protofcp
-Version: 0.0.2
+Version: 0.0.3
 Summary: FCP is a protocol used to route on "channels" and send or receive data.
 Home-page: https://github.com/ANDRVV/FCP
 Author: Andrea Vaccaro
 License: Apache 2.0
 Keywords: python,socket,protocol,proto,channel,scapy,packet
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `protofcp-0.0.2/README.md` & `protofcp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.2/protofcp/disassemblr.py` & `protofcp-0.0.3/protofcp/disassemblr.py`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.2/protofcp.egg-info/PKG-INFO` & `protofcp-0.0.3/protofcp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protofcp
-Version: 0.0.2
+Version: 0.0.3
 Summary: FCP is a protocol used to route on "channels" and send or receive data.
 Home-page: https://github.com/ANDRVV/FCP
 Author: Andrea Vaccaro
 License: Apache 2.0
 Keywords: python,socket,protocol,proto,channel,scapy,packet
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `protofcp-0.0.2/setup.py` & `protofcp-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os, codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = 'FCP is a protocol used to route on "channels" and send or receive data.'
 
 setup(
     name = "protofcp",
     version = VERSION,
     url = "https://github.com/ANDRVV/FCP",
     author = "Andrea Vaccaro",
```

