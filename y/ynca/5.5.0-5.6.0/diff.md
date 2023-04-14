# Comparing `tmp/ynca-5.5.0.tar.gz` & `tmp/ynca-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynca-5.5.0.tar", last modified: Fri Apr 14 18:59:13 2023, max compression
+gzip compressed data, was "ynca-5.6.0.tar", last modified: Fri Apr 14 19:25:52 2023, max compression
```

## Comparing `ynca-5.5.0.tar` & `ynca-5.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.349007 ynca-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 18:59:04.000000 ynca-5.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 18:59:04.000000 ynca-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 18:59:13.349007 ynca-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-14 18:59:04.000000 ynca-5.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 18:59:13.349007 ynca-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 18:59:04.000000 ynca-5.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.345007 ynca-5.5.0/ynca/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/modelinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.349007 ynca-5.5.0/ynca/subunits/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/airplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/bt.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/dab.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/ipod.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/ipodusb.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/napster.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/netradio.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/pandora.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/pc.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/rhap.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/sirius.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/uaw.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/subunits/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-14 18:59:04.000000 ynca-5.5.0/ynca/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:59:13.345007 ynca-5.5.0/ynca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 18:59:13.000000 ynca-5.5.0/ynca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 19:25:41.000000 ynca-5.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 19:25:41.000000 ynca-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 19:25:52.607591 ynca-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-14 19:25:41.000000 ynca-5.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 19:25:52.607591 ynca-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 19:25:41.000000 ynca-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.603591 ynca-5.6.0/ynca/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/modelinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/ynca/subunits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/airplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/bt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/dab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/ipod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/ipodusb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/napster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/netradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/rhap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/sirius.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/uaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/subunits/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-14 19:25:41.000000 ynca-5.6.0/ynca/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:52.607591 ynca-5.6.0/ynca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 19:25:52.000000 ynca-5.6.0/ynca.egg-info/top_level.txt
```

### Comparing `ynca-5.5.0/LICENSE.txt` & `ynca-5.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/PKG-INFO` & `ynca-5.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.5.0
+Version: 5.6.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ynca-5.5.0/README.md` & `ynca-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/setup.py` & `ynca-5.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="ynca",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="5.5.0",
+    version="5.6.0",
     description="Package to control Yamaha receivers that support the YNCA protocol.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/mvdwetering/ynca",
     # Author details
     author="Michel van de Wetering",
```

### Comparing `ynca-5.5.0/ynca/__init__.py` & `ynca-5.6.0/ynca/__init__.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/api.py` & `ynca-5.6.0/ynca/api.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/connection.py` & `ynca-5.6.0/ynca/connection.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/constants.py` & `ynca-5.6.0/ynca/constants.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/converters.py` & `ynca-5.6.0/ynca/converters.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/enums.py` & `ynca-5.6.0/ynca/enums.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/errors.py` & `ynca-5.6.0/ynca/errors.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/function.py` & `ynca-5.6.0/ynca/function.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/helpers.py` & `ynca-5.6.0/ynca/helpers.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/modelinfo.py` & `ynca-5.6.0/ynca/modelinfo.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/server.py` & `ynca-5.6.0/ynca/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         "SPBASS",
         "SPTREBLE",
         "EXBASS",
         "ADAPTIVEDRC",
         "DIALOGUELVL",
         "DTSDIALOGUECONTROL",
     ],
-    "METAINFO": ["ARTIST", "ALBUM", "SONG", "CHNAME"],
+    "METAINFO": ["ARTIST", "ALBUM", "SONG", "TRACK", "CHNAME"],
     "RDSINFO": ["RDSPRGTYPE", "RDSPRGSERVICE", "RDSTXTA", "RDSTXTB", "RDSCLOCK"],
 }
 
 
 INPUT_SUBUNITLIST_MAPPING = [
     (Input.AIRPLAY, ["AIRPLAY"]),
     (Input.BLUETOOTH, ["BT"]),
```

### Comparing `ynca-5.5.0/ynca/subunit.py` & `ynca-5.6.0/ynca/subunit.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/__init__.py` & `ynca-5.6.0/ynca/subunits/__init__.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/dab.py` & `ynca-5.6.0/ynca/subunits/dab.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/sirius.py` & `ynca-5.6.0/ynca/subunits/sirius.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/system.py` & `ynca-5.6.0/ynca/subunits/system.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/tun.py` & `ynca-5.6.0/ynca/subunits/tun.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/subunits/zone.py` & `ynca-5.6.0/ynca/subunits/zone.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca/terminal.py` & `ynca-5.6.0/ynca/terminal.py`

 * *Files identical despite different names*

### Comparing `ynca-5.5.0/ynca.egg-info/PKG-INFO` & `ynca-5.6.0/ynca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.5.0
+Version: 5.6.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ynca-5.5.0/ynca.egg-info/SOURCES.txt` & `ynca-5.6.0/ynca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

