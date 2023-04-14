# Comparing `tmp/lvlspy-1.3.0.tar.gz` & `tmp/lvlspy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvlspy-1.3.0.tar", last modified: Tue Mar 28 20:16:18 2023, max compression
+gzip compressed data, was "lvlspy-1.4.0.tar", last modified: Fri Apr 14 03:34:36 2023, max compression
```

## Comparing `lvlspy-1.3.0.tar` & `lvlspy-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-03-28 20:16:18.602135 lvlspy-1.3.0/
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)    35149 2023-03-28 17:56:37.000000 lvlspy-1.3.0/LICENSE
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      131 2023-03-28 17:56:37.000000 lvlspy-1.3.0/MANIFEST.in
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2118 2023-03-28 20:16:18.602135 lvlspy-1.3.0/PKG-INFO
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     1023 2023-03-28 17:56:37.000000 lvlspy-1.3.0/README.rst
-drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-03-28 20:16:18.598135 lvlspy-1.3.0/lvlspy/
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      276 2023-03-28 17:57:49.000000 lvlspy-1.3.0/lvlspy/__about__.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      400 2023-03-28 17:56:37.000000 lvlspy-1.3.0/lvlspy/__init__.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2966 2023-03-28 17:57:49.000000 lvlspy-1.3.0/lvlspy/level.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      762 2023-03-28 17:56:37.000000 lvlspy-1.3.0/lvlspy/properties.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)    10465 2023-03-28 17:57:49.000000 lvlspy-1.3.0/lvlspy/spcoll.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     4691 2023-03-28 17:56:37.000000 lvlspy-1.3.0/lvlspy/species.py
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     4505 2023-03-28 17:57:49.000000 lvlspy-1.3.0/lvlspy/transition.py
-drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-03-28 20:16:18.602135 lvlspy-1.3.0/lvlspy/xsd_pub/
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      794 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/catalog
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     6731 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/level_types.xsd
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2695 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/levels.xsd
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     3682 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/liblvls_input.xsd
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2771 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/spcoll.xsd
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     5095 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/zone_types.xsd
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2769 2023-03-28 20:16:11.000000 lvlspy-1.3.0/lvlspy/xsd_pub/zones.xsd
-drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-03-28 20:16:18.598135 lvlspy-1.3.0/lvlspy.egg-info/
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2118 2023-03-28 20:16:18.000000 lvlspy-1.3.0/lvlspy.egg-info/PKG-INFO
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      514 2023-03-28 20:16:18.000000 lvlspy-1.3.0/lvlspy.egg-info/SOURCES.txt
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)        1 2023-03-28 20:16:18.000000 lvlspy-1.3.0/lvlspy.egg-info/dependency_links.txt
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)       60 2023-03-28 20:16:18.000000 lvlspy-1.3.0/lvlspy.egg-info/requires.txt
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)        7 2023-03-28 20:16:18.000000 lvlspy-1.3.0/lvlspy.egg-info/top_level.txt
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)       38 2023-03-28 20:16:18.602135 lvlspy-1.3.0/setup.cfg
--rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     6353 2023-03-28 17:57:49.000000 lvlspy-1.3.0/setup.py
+drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-04-14 03:34:36.796099 lvlspy-1.4.0/
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)    35149 2023-03-28 17:56:37.000000 lvlspy-1.4.0/LICENSE
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      131 2023-03-28 17:56:37.000000 lvlspy-1.4.0/MANIFEST.in
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2226 2023-04-14 03:34:36.796099 lvlspy-1.4.0/PKG-INFO
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     1131 2023-04-14 03:33:10.000000 lvlspy-1.4.0/README.rst
+drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-04-14 03:34:36.796099 lvlspy-1.4.0/lvlspy/
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      276 2023-04-14 03:33:10.000000 lvlspy-1.4.0/lvlspy/__about__.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      400 2023-03-28 17:56:37.000000 lvlspy-1.4.0/lvlspy/__init__.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2966 2023-03-28 17:57:49.000000 lvlspy-1.4.0/lvlspy/level.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      762 2023-03-28 17:56:37.000000 lvlspy-1.4.0/lvlspy/properties.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)    10465 2023-03-28 17:57:49.000000 lvlspy-1.4.0/lvlspy/spcoll.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     4691 2023-03-28 17:56:37.000000 lvlspy-1.4.0/lvlspy/species.py
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     4505 2023-03-28 17:57:49.000000 lvlspy-1.4.0/lvlspy/transition.py
+drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-04-14 03:34:36.796099 lvlspy-1.4.0/lvlspy/xsd_pub/
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      794 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/catalog
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     6731 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/level_types.xsd
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2695 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/levels.xsd
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     3682 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/liblvls_input.xsd
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2771 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/spcoll.xsd
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     5095 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/zone_types.xsd
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2769 2023-04-14 03:34:29.000000 lvlspy-1.4.0/lvlspy/xsd_pub/zones.xsd
+drwxrwxr-x   0 jaadt7    (1000) jaadt7    (1000)        0 2023-04-14 03:34:36.796099 lvlspy-1.4.0/lvlspy.egg-info/
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     2226 2023-04-14 03:34:36.000000 lvlspy-1.4.0/lvlspy.egg-info/PKG-INFO
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)      514 2023-04-14 03:34:36.000000 lvlspy-1.4.0/lvlspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)        1 2023-04-14 03:34:36.000000 lvlspy-1.4.0/lvlspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)       60 2023-04-14 03:34:36.000000 lvlspy-1.4.0/lvlspy.egg-info/requires.txt
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)        7 2023-04-14 03:34:36.000000 lvlspy-1.4.0/lvlspy.egg-info/top_level.txt
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)       38 2023-04-14 03:34:36.796099 lvlspy-1.4.0/setup.cfg
+-rw-rw-r--   0 jaadt7    (1000) jaadt7    (1000)     6353 2023-03-28 17:57:49.000000 lvlspy-1.4.0/setup.py
```

### Comparing `lvlspy-1.3.0/LICENSE` & `lvlspy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/PKG-INFO` & `lvlspy-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvlspy
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python project to work with quantum level system data
 Home-page: https://github.com/jaadt7/lvlspy
 Author: Clemson University
 Author-email: jtannou@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/jaadt7/lvlspy/issues
 Project-URL: Source, https://github.com/jaadt7/lvlspy/
@@ -64,7 +64,12 @@
 - Source Code: `<https://github.com/jaadt7/lvlspy/>`_
 
 License
 -------
 
 The project is licensed under the GNU Public License v3 (or later).
 
+Documentation
+-------------
+
+The project documentation is available at `<https://lvlspy.readthedocs.io>`_.
+
```

### Comparing `lvlspy-1.3.0/README.rst` & `lvlspy-1.4.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -37,7 +37,12 @@
 - Source Code: `<https://github.com/jaadt7/lvlspy/>`_
 
 License
 -------
 
 The project is licensed under the GNU Public License v3 (or later).
 
+Documentation
+-------------
+
+The project documentation is available at `<https://lvlspy.readthedocs.io>`_.
+
```

### Comparing `lvlspy-1.3.0/lvlspy/level.py` & `lvlspy-1.4.0/lvlspy/level.py`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/properties.py` & `lvlspy-1.4.0/lvlspy/properties.py`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/spcoll.py` & `lvlspy-1.4.0/lvlspy/spcoll.py`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/species.py` & `lvlspy-1.4.0/lvlspy/species.py`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/transition.py` & `lvlspy-1.4.0/lvlspy/transition.py`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/catalog` & `lvlspy-1.4.0/lvlspy/xsd_pub/catalog`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/level_types.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/level_types.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/levels.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/levels.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/liblvls_input.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/liblvls_input.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/spcoll.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/spcoll.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/zone_types.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/zone_types.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy/xsd_pub/zones.xsd` & `lvlspy-1.4.0/lvlspy/xsd_pub/zones.xsd`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/lvlspy.egg-info/PKG-INFO` & `lvlspy-1.4.0/lvlspy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvlspy
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python project to work with quantum level system data
 Home-page: https://github.com/jaadt7/lvlspy
 Author: Clemson University
 Author-email: jtannou@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/jaadt7/lvlspy/issues
 Project-URL: Source, https://github.com/jaadt7/lvlspy/
@@ -64,7 +64,12 @@
 - Source Code: `<https://github.com/jaadt7/lvlspy/>`_
 
 License
 -------
 
 The project is licensed under the GNU Public License v3 (or later).
 
+Documentation
+-------------
+
+The project documentation is available at `<https://lvlspy.readthedocs.io>`_.
+
```

### Comparing `lvlspy-1.3.0/lvlspy.egg-info/SOURCES.txt` & `lvlspy-1.4.0/lvlspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lvlspy-1.3.0/setup.py` & `lvlspy-1.4.0/setup.py`

 * *Files identical despite different names*

