# Comparing `tmp/ynca-5.4.0.tar.gz` & `tmp/ynca-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynca-5.4.0.tar", last modified: Tue Feb 14 19:48:50 2023, max compression
+gzip compressed data, was "ynca-5.5.0.tar", last modified: Fri Apr 14 18:59:13 2023, max compression
```

## Comparing `ynca-5.4.0.tar` & `ynca-5.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:48:50.373225 ynca-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-14 19:48:35.000000 ynca-5.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-14 19:48:35.000000 ynca-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-02-14 19:48:50.373225 ynca-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-02-14 19:48:35.000000 ynca-5.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-14 19:48:50.377225 ynca-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-14 19:48:35.000000 ynca-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:48:50.369225 ynca-5.4.0/ynca/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/modelinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:48:50.373225 ynca-5.4.0/ynca/subunits/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/airplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/bt.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/dab.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/ipod.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/ipodusb.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/napster.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/netradio.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/pandora.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/pc.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/rhap.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/sirius.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/uaw.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/subunits/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-14 19:48:35.000000 ynca-5.4.0/ynca/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:48:50.369225 ynca-5.4.0/ynca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-02-14 19:48:50.000000 ynca-5.4.0/ynca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-14 19:48:50.000000 ynca-5.4.0/ynca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 19:48:50.000000 ynca-5.4.0/ynca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-14 19:48:50.000000 ynca-5.4.0/ynca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-14 19:48:50.000000 ynca-5.4.0/ynca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.349007 ynca-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 18:59:04.000000 ynca-5.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 18:59:04.000000 ynca-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 18:59:13.349007 ynca-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-14 18:59:04.000000 ynca-5.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 18:59:13.349007 ynca-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 18:59:04.000000 ynca-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.345007 ynca-5.5.0/ynca/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/modelinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.349007 ynca-5.5.0/ynca/subunits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/airplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/bt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/dab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/ipod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/ipodusb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/napster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/netradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/rhap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/sirius.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/uaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.345007 ynca-5.5.0/ynca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/top_level.txt
```

### Comparing `ynca-5.4.0/LICENSE.txt` & `ynca-5.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/PKG-INFO` & `ynca-5.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.4.0
+Version: 5.5.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-Supported receivers according to info found on the internet (not all tested).
+According to reports of users and info found on the internet the following receivers should work (not all tested).
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V671, RX-V673, RX-V677, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
@@ -76,15 +76,15 @@
 Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
-python3 -m ynca.server --host 0.0.0.0 --port 12345 <ynca_repo>/logs/RX-A810.txt
+python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --help
 ```
 
 
 ## Example usage
 
 ```python
```

### Comparing `ynca-5.4.0/README.md` & `ynca-5.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-Supported receivers according to info found on the internet (not all tested).
+According to reports of users and info found on the internet the following receivers should work (not all tested).
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V671, RX-V673, RX-V677, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
@@ -57,15 +57,15 @@
 Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
-python3 -m ynca.server --host 0.0.0.0 --port 12345 <ynca_repo>/logs/RX-A810.txt
+python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --help
 ```
 
 
 ## Example usage
 
 ```python
```

### Comparing `ynca-5.4.0/setup.py` & `ynca-5.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="ynca",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="5.4.0",
+    version="5.5.0",
     description="Package to control Yamaha receivers that support the YNCA protocol.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/mvdwetering/ynca",
     # Author details
     author="Michel van de Wetering",
```

### Comparing `ynca-5.4.0/ynca/__init__.py` & `ynca-5.5.0/ynca/__init__.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/api.py` & `ynca-5.5.0/ynca/api.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/connection.py` & `ynca-5.5.0/ynca/connection.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/constants.py` & `ynca-5.5.0/ynca/constants.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/converters.py` & `ynca-5.5.0/ynca/converters.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/enums.py` & `ynca-5.5.0/ynca/enums.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/errors.py` & `ynca-5.5.0/ynca/errors.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/function.py` & `ynca-5.5.0/ynca/function.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/helpers.py` & `ynca-5.5.0/ynca/helpers.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/modelinfo.py` & `ynca-5.5.0/ynca/modelinfo.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/server.py` & `ynca-5.5.0/ynca/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 import argparse
 import logging
 import re
 import socketserver
 from collections import namedtuple
 from typing import Dict, Tuple
 
+from .enums import Input
+
 RESTRICTED = "@RESTRICTED"
 UNDEFINED = "@UNDEFINED"
 OK = "OK"
 
 YncaCommand = namedtuple("YncaCommand", ["subunit", "function", "value"])
 
+ZONES = ["MAIN", "ZONE2", "ZONE3", "ZONE4"]
+
 
 def line_to_command(line):
     match = re.search(r"@(?P<subunit>.+?):(?P<function>.+?)=(?P<value>.*)", line)
     if match is not None:
         subunit = match.group("subunit")
         function = match.group("function")
         value = match.group("value")
@@ -110,14 +114,35 @@
         "DTSDIALOGUECONTROL",
     ],
     "METAINFO": ["ARTIST", "ALBUM", "SONG", "CHNAME"],
     "RDSINFO": ["RDSPRGTYPE", "RDSPRGSERVICE", "RDSTXTA", "RDSTXTB", "RDSCLOCK"],
 }
 
 
+INPUT_SUBUNITLIST_MAPPING = [
+    (Input.AIRPLAY, ["AIRPLAY"]),
+    (Input.BLUETOOTH, ["BT"]),
+    (Input.IPOD, ["IPOD"]),
+    (Input.IPOD_USB, ["IPODUSB"]),
+    (Input.NAPSTER, ["NAPSTER"]),
+    (Input.NETRADIO, ["NETRADIO"]),
+    (Input.PANDORA, ["PANDORA"]),
+    (Input.PC, ["PC"]),
+    (Input.RHAPSODY, ["RHAP"]),
+    (Input.SERVER, ["SERVER"]),
+    (Input.SIRIUS, ["SIRIUS"]),
+    (Input.SIRIUS_IR, ["SIRIUSIR"]),
+    (Input.SIRIUS_XM, ["SIRIUSXM"]),
+    (Input.SPOTIFY, ["SPOTIFY"]),
+    (Input.TUNER, ["TUN", "DAB"]),
+    (Input.UAW, ["UAW"]),
+    (Input.USB, ["USB"]),
+]
+
+
 class YncaCommandHandler(socketserver.StreamRequestHandler):
     """
     The request handler class for our server.
 
     It is instantiated once per connection to the server, and must
     override the handle() method to implement communication to the
     client.
@@ -186,19 +211,37 @@
             up = value.startswith("Up")
 
             parts = value.split(" ")
             amount = 0.5 if len(parts) == 1 else (int(parts[1]))
 
             value = float(self.store.get_data(subunit, function))
             value = str(value + (amount * (1 if up else -1)))
+
         result = self.store.put_data(subunit, function, value)
+
         if result[0].startswith("@"):
             self.write_line(result[0])
-        elif result[1]:
-            # Value change so send a report
+        elif result[1]:  # Value change so send a report
+
+            if function == "PLAYBACK":
+                # Response is PLAYBACKINFO
+                function = "PLAYBACKINFO"
+
+                # Not for Fwd or others as they are not a state
+                if value not in ["Play", "Pause", "Stop"]:
+                    return
+
+                # When received on a Zone the response is on INP subunit
+                if subunit in ZONES:
+                    subunit = [
+                        m[1][0]
+                        for m in INPUT_SUBUNITLIST_MAPPING
+                        if m[0].value == self.store.get_data(subunit, "INP")
+                    ][0]
+
             self.write_line(f"@{subunit}:{function}={value}")
 
     def handle(self):
         # self.rfile is a file-like object created by the handler;
         # we can now use e.g. readline() instead of raw recv() calls
         #
         # Note that the connection is closed when this handler returns!
@@ -314,16 +357,16 @@
     parser.add_argument(
         "initfile",
         help="File to use to initialize the YncaDatastore. Needs to contain Ynca command logging in format `@SUBUNIT:FUNCTION=VALUE`. E.g. output of example script with loglevel DEBUG.",
     )
 
     parser.add_argument(
         "--host",
-        help="Host interface to bind to, default is localhost",
-        default="localhost",
+        help="Host interface to bind to, default is 0.0.0.0 for all interfaces",
+        default="0.0.0.0",
     )
     parser.add_argument(
         "--port",
         help="Port to use, default is the standard port 50000",
         default=50000,
         type=int,
     )
```

### Comparing `ynca-5.4.0/ynca/subunit.py` & `ynca-5.5.0/ynca/subunit.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/subunits/__init__.py` & `ynca-5.5.0/ynca/subunits/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     song = StrFunction("SONG", Cmd.GET, init="METAINFO")
 
 
 class StationFunction:
     station = StrFunction("STATION", Cmd.GET)
 
 
+class TrackFunction:
+    track = StrFunction("TRACK", Cmd.GET, init="METAINFO")
+
+
 # A number of subunits have the same/similar featureset
 # so make a common base that only needs to be tested once
 class MediaPlaybackSubunitBase(
     PlaybackFunction,
     PlaybackInfoFunction,
     RepeatFunction,
     ShuffleFunction,
@@ -57,15 +61,14 @@
     SongFunction,
     SubunitBase,
 ):
     pass
 
 
 class FmFreqFunction:
-
     fmfreq = FloatFunction(
         "FMFREQ",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 2, 0.2)
         ),
     )
     """Read/write FM frequency. Values will be aligned to a valid stepsize."""
```

### Comparing `ynca-5.4.0/ynca/subunits/dab.py` & `ynca-5.5.0/ynca/subunits/dab.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/subunits/sirius.py` & `ynca-5.5.0/ynca/subunits/sirius.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/subunits/system.py` & `ynca-5.5.0/ynca/subunits/system.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/subunits/tun.py` & `ynca-5.5.0/ynca/subunits/tun.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/subunits/zone.py` & `ynca-5.5.0/ynca/subunits/zone.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca/terminal.py` & `ynca-5.5.0/ynca/terminal.py`

 * *Files identical despite different names*

### Comparing `ynca-5.4.0/ynca.egg-info/PKG-INFO` & `ynca-5.5.0/ynca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.4.0
+Version: 5.5.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
-Supported receivers according to info found on the internet (not all tested).
+According to reports of users and info found on the internet the following receivers should work (not all tested).
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> RX-A700, RX-A710, RX-A720, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V671, RX-V673, RX-V677, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700
+> RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
 
 Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
@@ -76,15 +76,15 @@
 Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
-python3 -m ynca.server --host 0.0.0.0 --port 12345 <ynca_repo>/logs/RX-A810.txt
+python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --help
 ```
 
 
 ## Example usage
 
 ```python
```

### Comparing `ynca-5.4.0/ynca.egg-info/SOURCES.txt` & `ynca-5.5.0/ynca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

