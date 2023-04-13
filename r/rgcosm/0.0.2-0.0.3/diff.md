# Comparing `tmp/rgcosm-0.0.2.tar.gz` & `tmp/rgcosm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.2.tar", last modified: Thu Apr 13 21:55:12 2023, max compression
+gzip compressed data, was "rgcosm-0.0.3.tar", last modified: Thu Apr 13 22:51:14 2023, max compression
```

## Comparing `rgcosm-0.0.2.tar` & `rgcosm-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:55:12.394521 rgcosm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 21:54:59.000000 rgcosm-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-13 21:55:12.394521 rgcosm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-13 21:54:59.000000 rgcosm-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 21:54:59.000000 rgcosm-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:55:12.394521 rgcosm-0.0.2/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 21:54:59.000000 rgcosm-0.0.2/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 21:54:59.000000 rgcosm-0.0.2/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-13 21:54:59.000000 rgcosm-0.0.2/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-13 21:54:59.000000 rgcosm-0.0.2/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:55:12.394521 rgcosm-0.0.2/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 21:55:12.000000 rgcosm-0.0.2/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 21:55:12.394521 rgcosm-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.908955 rgcosm-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 22:51:01.000000 rgcosm-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 22:51:14.908955 rgcosm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-13 22:51:01.000000 rgcosm-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:51:01.000000 rgcosm-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.904955 rgcosm-0.0.3/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-13 22:51:01.000000 rgcosm-0.0.3/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:51:14.904955 rgcosm-0.0.3/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 22:51:14.000000 rgcosm-0.0.3/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 22:51:14.908955 rgcosm-0.0.3/setup.cfg
```

### Comparing `rgcosm-0.0.2/LICENSE` & `rgcosm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.2/rgcosm/__main__.py` & `rgcosm-0.0.3/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.2/rgcosm/convert.py` & `rgcosm-0.0.3/rgcosm/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import osmium
+import json
 import sqlite3
 
 import argparse
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -52,20 +53,20 @@
 		self.cursor = self.conn.cursor()
 		self.cursor.execute('''CREATE TABLE IF NOT EXISTS nodes (id INTEGER PRIMARY KEY, lat REAL, lon REAL, tags TEXT)''')
 		self.cursor.execute('''CREATE TABLE IF NOT EXISTS ways (id INTEGER PRIMARY KEY, nodes INTEGER, tags TEXT)''')
 		self.conn.commit()
 
 
 	def node(self, n):
-		self.cursor.execute('''INSERT INTO nodes (id, lat, lon, tags) VALUES (?, ?, ?, ?)''', (n.id, n.location.lat, n.location.lon, str(dict(n.tags))))
+		self.cursor.execute('''INSERT INTO nodes (id, lat, lon, tags) VALUES (?, ?, ?, ?)''', (n.id, n.location.lat, n.location.lon, json.dumps(dict(n.tags))))
 		self.conn.commit()
 
 
 	def way(self, w):
-		self.cursor.execute('''INSERT INTO ways (id, nodes, tags) VALUES (?, ?, ?)''', (w.id, ' '.join(map(str, w.nodes)), str(dict(w.tags))))
+		self.cursor.execute('''INSERT INTO ways (id, nodes, tags) VALUES (?, ?, ?)''', (w.id, ' '.join(map(str, w.nodes)), json.dumps(dict(w.tags))))
 		self.conn.commit()
 
 
 	def save(self):
 		if self.output:
 			self.conn.backup(self.conn_file)
 		else:
```

### Comparing `rgcosm-0.0.2/rgcosm/geocoder.py` & `rgcosm-0.0.3/rgcosm/geocoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlite3
+import json
 import math
 
 import argparse
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -93,14 +94,16 @@
 
 		# Parse the tags column to find the address
 		#address = {}
 		#for tag in min_address['tags'].split(','):
 		#    k, v = tag.split(':', 1)
 		#    address[k] = v
 
+		min_address['tags'] = json.loads(min_address['tags'])
+
 		# Return the address
 		return min_address
 
 
 	def locate(self, coordinates: 'Union[Mapping[float, float], Mapping[Tuple[float, float]]]', search_tags: str = 'addr:', min_tags_count: int = 1) -> 'Optional[List[dict]]':
 		if hasattr(coordinates, '__getitem__'):
 			if isinstance(coordinates[0], float):
```

### Comparing `rgcosm-0.0.2/setup.cfg` & `rgcosm-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.2
+version = 0.0.3
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

