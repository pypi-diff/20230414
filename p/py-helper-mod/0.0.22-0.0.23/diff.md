# Comparing `tmp/py-helper-mod-0.0.22.tar.gz` & `tmp/py-helper-mod-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp9e0sn1ti/py-helper-mod-0.0.22.tar", last modified: Thu Dec  8 15:30:38 2022, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp3rjnqx8j/py-helper-mod-0.0.23.tar", last modified: Fri Apr 14 20:29:57 2023, max compression
```

## Comparing `py-helper-mod-0.0.22.tar` & `py-helper-mod-0.0.23.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.22/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.22/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.22/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.22/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2022-12-08 15:30:38.000000 py-helper-mod-0.0.22/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    78282 2022-12-08 15:29:54.000000 py-helper-mod-0.0.22/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.23/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    78400 2023-04-14 20:29:24.000000 py-helper-mod-0.0.23/py_helper.py
```

### Comparing `py-helper-mod-0.0.22/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.23/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.22
+Version: 0.0.23
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.22/LICENSE` & `py-helper-mod-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.22/PKG-INFO` & `py-helper-mod-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.22
+Version: 0.0.23
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.22/setup.cfg` & `py-helper-mod-0.0.23/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.22
+version = 0.0.23
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

### Comparing `py-helper-mod-0.0.22/py_helper.py` & `py-helper-mod-0.0.23/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,22)
+VERSION=(0,0,23)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -2214,43 +2214,49 @@
 		if expr.search(str(row[column])):
 			result = row
 			break
 
 	return result
 
 # Search a column of tabular data, return all matching results
-def SearchColumn(item,rows,column=0):
+def SearchColumn(item,rows,column=0,return_all=True):
 	"""
 	Wrapper function to look for an item in tabular/columnar data.
 	The function looks for all occurrences and returns the rows in
 	a list.
 	"""
 	results = list()
 
 	for row in rows:
 		if item == row[column]:
-			results.append(row)
+			if return_all:
+				results.append(row)
+			else:
+				return row
 
 	return results
 
 # Search Tabular/Columnar Data With a Regular Expresion
-def SearchColumnRe(expresion,rows,column=0):
+def SearchColumnRe(expresion,rows,column=0,return_all=True):
 	"""
 	Wrapper function to search a column of tabular/columnar data with
 	a regular expression. If a cell is not a string, it will be converted
 	into one first.
 	"""
 
 	results = list()
 
 	expr = re.compile(expression)
 
 	for row in rows:
 		if expr.search(str(row[column])):
-			results.append(row)
+			if return_all:
+				results.append(row)
+			else:
+				return row
 
 	return results
 
 # Check Entire CSV for an Item
 def IsIn(item,rows):
 	"""
 	Seach Entire CSV (all columns of all rows) for an item
```

