# Comparing `tmp/adafruit-blinka-bleio-4.0.0.tar.gz` & `tmp/adafruit-blinka-bleio-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-blinka-bleio-4.0.0.tar", last modified: Mon Apr  3 20:20:18 2023, max compression
+gzip compressed data, was "adafruit-blinka-bleio-4.0.1.tar", last modified: Fri Apr 14 13:18:08 2023, max compression
```

## Comparing `adafruit-blinka-bleio-4.0.0.tar` & `adafruit-blinka-bleio-4.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.358081 adafruit-blinka-bleio-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.346081 adafruit-blinka-bleio-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.350081 adafruit-blinka-bleio-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.350081 adafruit-blinka-bleio-4.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-03 20:20:18.358081 adafruit-blinka-bleio-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.354081 adafruit-blinka-bleio-4.0.0/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/characteristic_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34364 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/packet_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/scan_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/_bleio/uuid_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.354081 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-03 20:20:18.000000 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-03 20:20:18.000000 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:20:18.000000 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 20:20:18.000000 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 20:20:18.000000 adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.354081 adafruit-blinka-bleio-4.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.354081 adafruit-blinka-bleio-4.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:20:18.358081 adafruit-blinka-bleio-4.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/examples/blinka_bleio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-03 20:20:08.000000 adafruit-blinka-bleio-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 20:19:56.000000 adafruit-blinka-bleio-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:20:18.358081 adafruit-blinka-bleio-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.968387 adafruit-blinka-bleio-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.968387 adafruit-blinka-bleio-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/characteristic_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34364 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/packet_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/scan_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/uuid_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/examples/blinka_bleio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/setup.cfg
```

### Comparing `adafruit-blinka-bleio-4.0.0/.github/workflows/build.yml` & `adafruit-blinka-bleio-4.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/.github/workflows/release.yml` & `adafruit-blinka-bleio-4.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/.pre-commit-config.yaml` & `adafruit-blinka-bleio-4.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/.pylintrc` & `adafruit-blinka-bleio-4.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/CODE_OF_CONDUCT.md` & `adafruit-blinka-bleio-4.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-blinka-bleio-4.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/LICENSES/MIT.txt` & `adafruit-blinka-bleio-4.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/LICENSES/Unlicense.txt` & `adafruit-blinka-bleio-4.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/PKG-INFO` & `adafruit-blinka-bleio-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-bleio
-Version: 4.0.0
+Version: 4.0.1
 Summary: `_bleio` for Blinka based on `bleak`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Blinka_bleio.git
 Keywords: adafruit,blinka,circuitpython,micropython,blinka_bleio,bleio,bleak
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-blinka-bleio-4.0.0/README.rst` & `adafruit-blinka-bleio-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/__init__.py` & `adafruit-blinka-bleio-4.0.1/_bleio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     RoleError,
     SecurityError,
 )
 from _bleio.packet_buffer import PacketBuffer
 from _bleio.scan_entry import ScanEntry
 from _bleio.uuid_ import UUID
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 def set_adapter(new_adapter: Optional[Adapter]) -> None:
     """Set the adapter to use for BLE, such as when using an HCI adapter.
     Raises `NotImplementedError` when the adapter is a singleton and cannot be set.
     """
```

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/address.py` & `adafruit-blinka-bleio-4.0.1/_bleio/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from typing import Any, Optional, Union
 
 import re
 
 Buf = Union[bytes, bytearray, memoryview]
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 class Address:
     PUBLIC = 0x0
     RANDOM_STATIC = 0x1
     RANDOM_PRIVATE_RESOLVABLE = 0x2
```

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/attribute.py` & `adafruit-blinka-bleio-4.0.1/_bleio/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ================================================================================
 
 `_bleio` for Blinka based on ``bleak``
 
 * Author(s): Dan Halbert
 """
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 from enum import Enum
 
 
 class Attribute(Enum):
     NO_ACCESS = 0x00
```

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/characteristic_buffer.py` & `adafruit-blinka-bleio-4.0.1/_bleio/characteristic_buffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,18 @@
         because it will be faster.
 
         :return: Data read
         """
         buffer = bytearray(
             min(nbytes, self._buffer_size) if nbytes else self._buffer_size
         )
-        if self.readinto(buffer) == 0:
+        bytes_read = self.readinto(buffer)
+        if bytes_read == 0:
             return None
-        return buffer
+        return buffer[:bytes_read]
 
     def readinto(self, buf: Buf) -> Union[int, None]:
         """Read bytes into the ``buf``. Read at most ``len(buf)`` bytes.
 
         :return: number of bytes read and stored into ``buf``
         """
         length = len(buf)
```

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/common.py` & `adafruit-blinka-bleio-4.0.1/_bleio/common.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/descriptor.py` & `adafruit-blinka-bleio-4.0.1/_bleio/descriptor.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/exceptions.py` & `adafruit-blinka-bleio-4.0.1/_bleio/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 =======================================================================
 
 _bleio implementation for Adafruit_Blinka_bleio
 
 * Author(s): Dan Halbert for Adafruit Industries
 """
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 class BluetoothError(Exception):
     """Catch-all exception for Bluetooth related errors."""
```

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/packet_buffer.py` & `adafruit-blinka-bleio-4.0.1/_bleio/packet_buffer.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/scan_entry.py` & `adafruit-blinka-bleio-4.0.1/_bleio/scan_entry.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/_bleio/uuid_.py` & `adafruit-blinka-bleio-4.0.1/_bleio/uuid_.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from __future__ import annotations
 from typing import Any, Union
 
 import re
 
 Buf = Union[bytes, bytearray, memoryview]
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 _UUID_RE = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", flags=re.IGNORECASE
 )
 
 _STANDARD_UUID_RE = re.compile(
```

### Comparing `adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/PKG-INFO` & `adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-bleio
-Version: 4.0.0
+Version: 4.0.1
 Summary: `_bleio` for Blinka based on `bleak`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Blinka_bleio.git
 Keywords: adafruit,blinka,circuitpython,micropython,blinka_bleio,bleio,bleak
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-blinka-bleio-4.0.0/adafruit_blinka_bleio.egg-info/SOURCES.txt` & `adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/docs/_static/favicon.ico` & `adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/docs/api.rst` & `adafruit-blinka-bleio-4.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/docs/conf.py` & `adafruit-blinka-bleio-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/docs/index.rst` & `adafruit-blinka-bleio-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.0/pyproject.toml` & `adafruit-blinka-bleio-4.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "setuptools-scm",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adafruit-blinka-bleio"
 description = "`_bleio` for Blinka based on `bleak`"
-version = "4.0.0"
+version = "4.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"}
 keywords = [
     "adafruit",
```

