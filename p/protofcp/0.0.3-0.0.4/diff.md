# Comparing `tmp/protofcp-0.0.3.tar.gz` & `tmp/protofcp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protofcp-0.0.3.tar", last modified: Fri Apr 14 16:01:03 2023, max compression
+gzip compressed data, was "protofcp-0.0.4.tar", last modified: Fri Apr 14 16:57:23 2023, max compression
```

## Comparing `protofcp-0.0.3.tar` & `protofcp-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.747518 protofcp-0.0.3/
--rw-rw-rw-   0        0        0    11542 2023-04-14 13:43:37.000000 protofcp-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1723 2023-04-14 16:01:03.747518 protofcp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2023-04-14 14:02:43.000000 protofcp-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.725694 protofcp-0.0.3/protofcp/
--rw-rw-rw-   0        0        0     1277 2023-04-14 15:56:52.000000 protofcp-0.0.3/protofcp/FCPSocket.py
--rw-rw-rw-   0        0        0      243 2023-04-14 14:01:04.000000 protofcp-0.0.3/protofcp/__init__.py
--rw-rw-rw-   0        0        0      499 2023-04-13 23:30:51.000000 protofcp-0.0.3/protofcp/assemblr.py
--rw-rw-rw-   0        0        0      444 2023-04-14 12:04:20.000000 protofcp-0.0.3/protofcp/consts.py
--rw-rw-rw-   0        0        0      826 2023-04-13 23:41:00.000000 protofcp-0.0.3/protofcp/disassemblr.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:01:03.745510 protofcp-0.0.3/protofcp.egg-info/
--rw-rw-rw-   0        0        0     1723 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 16:01:03.000000 protofcp-0.0.3/protofcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 16:01:03.747518 protofcp-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-14 15:06:11.000000 protofcp-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:57:23.640780 protofcp-0.0.4/
+-rw-rw-rw-   0        0        0    11542 2023-04-14 13:43:37.000000 protofcp-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1723 2023-04-14 16:57:23.639780 protofcp-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2023-04-14 14:02:43.000000 protofcp-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 16:57:23.628786 protofcp-0.0.4/protofcp/
+-rw-rw-rw-   0        0        0     1290 2023-04-14 16:54:48.000000 protofcp-0.0.4/protofcp/FCPSocket.py
+-rw-rw-rw-   0        0        0      243 2023-04-14 14:01:04.000000 protofcp-0.0.4/protofcp/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 23:30:51.000000 protofcp-0.0.4/protofcp/assemblr.py
+-rw-rw-rw-   0        0        0      444 2023-04-14 12:04:20.000000 protofcp-0.0.4/protofcp/consts.py
+-rw-rw-rw-   0        0        0      826 2023-04-13 23:41:00.000000 protofcp-0.0.4/protofcp/disassemblr.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:57:23.638782 protofcp-0.0.4/protofcp.egg-info/
+-rw-rw-rw-   0        0        0     1723 2023-04-14 16:57:23.000000 protofcp-0.0.4/protofcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-14 16:57:23.000000 protofcp-0.0.4/protofcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:57:23.000000 protofcp-0.0.4/protofcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 16:57:23.000000 protofcp-0.0.4/protofcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 16:57:23.000000 protofcp-0.0.4/protofcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:57:23.640780 protofcp-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-04-14 16:54:08.000000 protofcp-0.0.4/setup.py
```

### Comparing `protofcp-0.0.3/LICENSE` & `protofcp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.3/PKG-INFO` & `protofcp-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protofcp
-Version: 0.0.3
+Version: 0.0.4
 Summary: FCP is a protocol used to route on "channels" and send or receive data.
 Home-page: https://github.com/ANDRVV/FCP
 Author: Andrea Vaccaro
 License: Apache 2.0
 Keywords: python,socket,protocol,proto,channel,scapy,packet
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `protofcp-0.0.3/README.md` & `protofcp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.3/protofcp/FCPSocket.py` & `protofcp-0.0.4/protofcp/FCPSocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class FCPSocket:
     def __init__(self, channel: Channels):
         self.ch = channel
         self.sock = conf.L2socket()
 
     def send(self, raw: bytes):
         packet = assemblr.buildPacket(self.ch, raw).assembly()
-        sendp(Ether(dst = "ff:ff:ff:ff:ff:ff")/(packet))
+        sendp(Ether(dst = "ff:ff:ff:ff:ff:ff")/(packet), verbose = 0)
 
     def recv(self):
         while True:
             data = self.sock.recv()
             if data is not None:
                 try: 
                     data = data[Raw].load
```

### Comparing `protofcp-0.0.3/protofcp/disassemblr.py` & `protofcp-0.0.4/protofcp/disassemblr.py`

 * *Files identical despite different names*

### Comparing `protofcp-0.0.3/protofcp.egg-info/PKG-INFO` & `protofcp-0.0.4/protofcp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protofcp
-Version: 0.0.3
+Version: 0.0.4
 Summary: FCP is a protocol used to route on "channels" and send or receive data.
 Home-page: https://github.com/ANDRVV/FCP
 Author: Andrea Vaccaro
 License: Apache 2.0
 Keywords: python,socket,protocol,proto,channel,scapy,packet
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `protofcp-0.0.3/setup.py` & `protofcp-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os, codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = 'FCP is a protocol used to route on "channels" and send or receive data.'
 
 setup(
     name = "protofcp",
     version = VERSION,
     url = "https://github.com/ANDRVV/FCP",
     author = "Andrea Vaccaro",
```

