# Comparing `tmp/phoebusgen-2.5.tar.gz` & `tmp/phoebusgen-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoebusgen-2.5.tar", last modified: Thu Apr 13 23:45:52 2023, max compression
+gzip compressed data, was "phoebusgen-2.5.1.tar", last modified: Fri Apr 14 00:07:22 2023, max compression
```

## Comparing `phoebusgen-2.5.tar` & `phoebusgen-2.5.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.409371 phoebusgen-2.5/
--rw-rw-r--   0 tford     (1000) tford     (1000)    17987 2022-05-20 06:18:45.000000 phoebusgen-2.5/LICENSE
--rw-rw-r--   0 tford     (1000) tford     (1000)      209 2022-05-20 06:18:45.000000 phoebusgen-2.5/MANIFEST.in
--rw-r--r--   0 tford     (1000) tford     (1000)     4778 2023-04-13 23:45:52.409371 phoebusgen-2.5/PKG-INFO
--rw-rw-r--   0 tford     (1000) tford     (1000)     4207 2023-04-12 05:14:47.000000 phoebusgen-2.5/README.md
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.409371 phoebusgen-2.5/phoebusgen/
--rw-rw-r--   0 tford     (1000) tford     (1000)     4515 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/__init__.py
--rw-rw-r--   0 tford     (1000) tford     (1000)     8107 2022-06-28 02:59:04.000000 phoebusgen-2.5/phoebusgen/_shared_property_helpers.py
--rw-r--r--   0 tford     (1000) tford     (1000)      495 2023-04-13 23:45:52.409371 phoebusgen-2.5/phoebusgen/_version.py
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.407370 phoebusgen-2.5/phoebusgen/config/
--rw-rw-r--   0 tford     (1000) tford     (1000)     3150 2022-05-20 06:18:45.000000 phoebusgen-2.5/phoebusgen/config/classes.bcf
--rw-rw-r--   0 tford     (1000) tford     (1000)     1911 2022-05-20 06:18:45.000000 phoebusgen-2.5/phoebusgen/config/color.def
--rw-rw-r--   0 tford     (1000) tford     (1000)     2103 2023-04-12 05:14:47.000000 phoebusgen-2.5/phoebusgen/config/font.def
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.408370 phoebusgen-2.5/phoebusgen/screen/
--rw-rw-r--   0 tford     (1000) tford     (1000)     1237 2023-04-12 05:20:13.000000 phoebusgen-2.5/phoebusgen/screen/__init__.py
--rw-rw-r--   0 tford     (1000) tford     (1000)     4372 2023-04-12 05:20:13.000000 phoebusgen-2.5/phoebusgen/screen/screen.py
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.408370 phoebusgen-2.5/phoebusgen/widget/
--rw-rw-r--   0 tford     (1000) tford     (1000)     1273 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/widget/__init__.py
--rw-rw-r--   0 tford     (1000) tford     (1000)    65736 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/widget/properties.py
--rw-rw-r--   0 tford     (1000) tford     (1000)     9033 2023-04-13 22:44:54.000000 phoebusgen-2.5/phoebusgen/widget/widget.py
--rw-rw-r--   0 tford     (1000) tford     (1000)    27623 2023-04-12 05:14:47.000000 phoebusgen-2.5/phoebusgen/widget/widgets.py
-drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.407370 phoebusgen-2.5/phoebusgen.egg-info/
--rw-r--r--   0 tford     (1000) tford     (1000)     4778 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/PKG-INFO
--rw-r--r--   0 tford     (1000) tford     (1000)      562 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/SOURCES.txt
--rw-r--r--   0 tford     (1000) tford     (1000)        1 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/dependency_links.txt
--rw-r--r--   0 tford     (1000) tford     (1000)       11 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/top_level.txt
--rw-rw-r--   0 tford     (1000) tford     (1000)        0 2022-05-20 06:18:45.000000 phoebusgen-2.5/requirements.txt
--rw-rw-r--   0 tford     (1000) tford     (1000)      198 2023-04-13 23:45:52.409371 phoebusgen-2.5/setup.cfg
--rw-rw-r--   0 tford     (1000) tford     (1000)     1019 2023-04-12 05:20:14.000000 phoebusgen-2.5/setup.py
--rw-rw-r--   0 tford     (1000) tford     (1000)    81180 2023-04-12 05:20:14.000000 phoebusgen-2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/phoebusgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/_shared_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/phoebusgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/classes.bcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/color.def
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/font.def
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/screen/screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65736 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/versioneer.py
```

### Comparing `phoebusgen-2.5/LICENSE` & `phoebusgen-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/PKG-INFO` & `phoebusgen-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.5
+Version: 2.5.1
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.5/README.md` & `phoebusgen-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/__init__.py` & `phoebusgen-2.5.1/phoebusgen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/_shared_property_helpers.py` & `phoebusgen-2.5.1/phoebusgen/_shared_property_helpers.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/config/classes.bcf` & `phoebusgen-2.5.1/phoebusgen/config/classes.bcf`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/config/color.def` & `phoebusgen-2.5.1/phoebusgen/config/color.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/config/font.def` & `phoebusgen-2.5.1/phoebusgen/config/font.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/screen/__init__.py` & `phoebusgen-2.5.1/phoebusgen/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/screen/screen.py` & `phoebusgen-2.5.1/phoebusgen/screen/screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/widget/__init__.py` & `phoebusgen-2.5.1/phoebusgen/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/widget/properties.py` & `phoebusgen-2.5.1/phoebusgen/widget/properties.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/widget/widget.py` & `phoebusgen-2.5.1/phoebusgen/widget/widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen/widget/widgets.py` & `phoebusgen-2.5.1/phoebusgen/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/phoebusgen.egg-info/PKG-INFO` & `phoebusgen-2.5.1/phoebusgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.5
+Version: 2.5.1
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.5/phoebusgen.egg-info/SOURCES.txt` & `phoebusgen-2.5.1/phoebusgen.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 phoebusgen/config/color.def
 phoebusgen/config/font.def
 phoebusgen/screen/__init__.py
 phoebusgen/screen/screen.py
 phoebusgen/widget/__init__.py
 phoebusgen/widget/properties.py
 phoebusgen/widget/widget.py
-phoebusgen/widget/widgets.py
+phoebusgen/widget/widgets.py
+tests/test_screen.py
+tests/test_widget.py
+tests/test_widgets.py
```

### Comparing `phoebusgen-2.5/setup.py` & `phoebusgen-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5/versioneer.py` & `phoebusgen-2.5.1/versioneer.py`

 * *Files identical despite different names*

