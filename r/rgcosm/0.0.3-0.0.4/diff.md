# Comparing `tmp/rgcosm-0.0.3.tar.gz` & `tmp/rgcosm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.3.tar", last modified: Thu Apr 13 22:51:14 2023, max compression
+gzip compressed data, was "rgcosm-0.0.4.tar", last modified: Thu Apr 13 23:01:45 2023, max compression
```

## Comparing `rgcosm-0.0.3.tar` & `rgcosm-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.908955 rgcosm-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 22:51:01.000000 rgcosm-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 22:51:14.908955 rgcosm-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-13 22:51:01.000000 rgcosm-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:51:01.000000 rgcosm-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.904955 rgcosm-0.0.3/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.904955 rgcosm-0.0.3/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 22:51:14.908955 rgcosm-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:01:45.988295 rgcosm-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 23:01:35.000000 rgcosm-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 23:01:45.988295 rgcosm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-13 23:01:35.000000 rgcosm-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 23:01:35.000000 rgcosm-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:01:45.988295 rgcosm-0.0.4/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 23:01:35.000000 rgcosm-0.0.4/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 23:01:35.000000 rgcosm-0.0.4/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-13 23:01:35.000000 rgcosm-0.0.4/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-13 23:01:35.000000 rgcosm-0.0.4/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:01:45.988295 rgcosm-0.0.4/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 23:01:45.000000 rgcosm-0.0.4/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 23:01:45.992295 rgcosm-0.0.4/setup.cfg
```

### Comparing `rgcosm-0.0.3/LICENSE` & `rgcosm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.3/PKG-INFO` & `rgcosm-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.3
+Version: 0.0.4
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.3/README.md` & `rgcosm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.3/rgcosm/__main__.py` & `rgcosm-0.0.4/rgcosm/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 if len(sys.argv) == 1:
 	print('Help: rgosm -h/--help')
 	exit(1)
 
 import argparse
 
-from convert import parser as conv_parser
-from geocoder import parser as ltln_parser
+from .convert import parser as conv_parser
+from .geocoder import parser as ltln_parser
 
 parser = argparse.ArgumentParser(description='rgcosm cli', parents=[conv_parser, ltln_parser])
 
 args = parser.parse_args()
 
 
 # Converter
 if args.cinput:
-	from convert import osm2sqlite3
-	from convert import init_args as converter_init_args
+	from .convert import osm2sqlite3
+	from .convert import init_args as converter_init_args
 	converter_init_args(args)
 	osm2sqlite3(args.cinput, args.coutput, args.add_indexes)
 
 
 # Geocoder
 elif args.database:
-	from geocoder import get_address
-	from geocoder import init_args as geocoder_init_args
+	from .geocoder import get_address
+	from .geocoder import init_args as geocoder_init_args
 	geocoder_init_args(args)
 	addr = get_address(args.database, (args.latitude, args.longitude), args.search_tags, args.min_tags_count)
 	print(addr)
```

### Comparing `rgcosm-0.0.3/rgcosm/convert.py` & `rgcosm-0.0.4/rgcosm/convert.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.3/rgcosm/geocoder.py` & `rgcosm-0.0.4/rgcosm/geocoder.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.3/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.0.4/rgcosm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.3
+Version: 0.0.4
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.3/setup.cfg` & `rgcosm-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.3
+version = 0.0.4
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

