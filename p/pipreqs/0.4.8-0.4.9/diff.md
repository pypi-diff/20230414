# Comparing `tmp/pipreqs-0.4.8.tar.gz` & `tmp/pipreqs-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipreqs-0.4.8.tar", last modified: Fri Jun 30 12:27:49 2017, max compression
+gzip compressed data, was "dist/pipreqs-0.4.9.tar", last modified: Fri Jun 30 18:20:03 2017, max compression
```

## Comparing `pipreqs-0.4.8.tar` & `pipreqs-0.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/
--rw-r--r--   0 wutwut     (501) staff       (20)      166 2017-03-20 19:45:20.000000 pipreqs-0.4.8/AUTHORS.rst
--rw-r--r--   0 wutwut     (501) staff       (20)     3149 2017-03-20 19:45:20.000000 pipreqs-0.4.8/CONTRIBUTING.rst
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/docs/
--rw-r--r--   0 wutwut     (501) staff       (20)       28 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/authors.rst
--rwxr-xr-x   0 wutwut     (501) staff       (20)     8399 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/conf.py
--rw-r--r--   0 wutwut     (501) staff       (20)       33 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/contributing.rst
--rw-r--r--   0 wutwut     (501) staff       (20)       28 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/history.rst
--rw-r--r--   0 wutwut     (501) staff       (20)      501 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/index.rst
--rw-r--r--   0 wutwut     (501) staff       (20)      191 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/installation.rst
--rw-r--r--   0 wutwut     (501) staff       (20)     6461 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/make.bat
--rw-r--r--   0 wutwut     (501) staff       (20)     6766 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/Makefile
--rw-r--r--   0 wutwut     (501) staff       (20)       27 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/readme.rst
--rw-r--r--   0 wutwut     (501) staff       (20)       75 2017-03-20 19:45:20.000000 pipreqs-0.4.8/docs/usage.rst
--rw-r--r--   0 wutwut     (501) staff       (20)     3269 2017-06-30 12:26:32.000000 pipreqs-0.4.8/HISTORY.rst
--rw-r--r--   0 wutwut     (501) staff       (20)    11358 2017-03-20 19:45:20.000000 pipreqs-0.4.8/LICENSE
--rw-r--r--   0 wutwut     (501) staff       (20)      306 2017-03-20 19:45:20.000000 pipreqs-0.4.8/MANIFEST.in
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs/
--rwxr-xr-x   0 wutwut     (501) staff       (20)      118 2017-06-30 12:24:22.000000 pipreqs-0.4.8/pipreqs/__init__.py
--rw-r--r--   0 wutwut     (501) staff       (20)    26296 2017-06-30 12:23:23.000000 pipreqs-0.4.8/pipreqs/mapping
--rwxr-xr-x   0 wutwut     (501) staff       (20)    13821 2017-06-30 12:23:23.000000 pipreqs-0.4.8/pipreqs/pipreqs.py
--rw-r--r--   0 wutwut     (501) staff       (20)    12204 2017-03-20 19:45:20.000000 pipreqs-0.4.8/pipreqs/stdlib
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/
--rw-r--r--   0 wutwut     (501) staff       (20)        1 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/dependency_links.txt
--rw-r--r--   0 wutwut     (501) staff       (20)       50 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/entry_points.txt
--rw-r--r--   0 wutwut     (501) staff       (20)        1 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/not-zip-safe
--rw-r--r--   0 wutwut     (501) staff       (20)     8489 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/PKG-INFO
--rw-r--r--   0 wutwut     (501) staff       (20)       12 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/requires.txt
--rw-r--r--   0 wutwut     (501) staff       (20)      805 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/SOURCES.txt
--rw-r--r--   0 wutwut     (501) staff       (20)        8 2017-06-30 12:27:49.000000 pipreqs-0.4.8/pipreqs.egg-info/top_level.txt
--rw-r--r--   0 wutwut     (501) staff       (20)     8489 2017-06-30 12:27:49.000000 pipreqs-0.4.8/PKG-INFO
--rw-r--r--   0 wutwut     (501) staff       (20)     2459 2017-06-30 12:23:23.000000 pipreqs-0.4.8/README.rst
--rw-r--r--   0 wutwut     (501) staff       (20)       61 2017-06-30 12:27:49.000000 pipreqs-0.4.8/setup.cfg
--rwxr-xr-x   0 wutwut     (501) staff       (20)     1682 2017-03-20 19:45:20.000000 pipreqs-0.4.8/setup.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/
--rwxr-xr-x   0 wutwut     (501) staff       (20)       24 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/__init__.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_data/
--rw-r--r--   0 wutwut     (501) staff       (20)        0 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data/models.py
--rw-r--r--   0 wutwut     (501) staff       (20)     1524 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data/test.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_data_duplicated_deps/
--rw-r--r--   0 wutwut     (501) staff       (20)      176 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data_duplicated_deps/db.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_data_ignore/
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_data_ignore/.ignore_second/
--rw-r--r--   0 wutwut     (501) staff       (20)       81 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data_ignore/.ignore_second/ignored.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_data_ignore/.ignored_dir/
--rw-r--r--   0 wutwut     (501) staff       (20)       51 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data_ignore/.ignored_dir/ignored.py
--rw-r--r--   0 wutwut     (501) staff       (20)     1524 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_data_ignore/test.py
-drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 12:27:49.000000 pipreqs-0.4.8/tests/_invalid_data/
--rw-r--r--   0 wutwut     (501) staff       (20)       38 2017-03-20 19:45:20.000000 pipreqs-0.4.8/tests/_invalid_data/invalid.py
--rwxr-xr-x   0 wutwut     (501) staff       (20)     8023 2017-06-30 12:23:23.000000 pipreqs-0.4.8/tests/test_pipreqs.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/
+-rw-r--r--   0 wutwut     (501) staff       (20)      166 2017-03-20 19:45:20.000000 pipreqs-0.4.9/AUTHORS.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)     3149 2017-03-20 19:45:20.000000 pipreqs-0.4.9/CONTRIBUTING.rst
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/docs/
+-rw-r--r--   0 wutwut     (501) staff       (20)       28 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/authors.rst
+-rwxr-xr-x   0 wutwut     (501) staff       (20)     8399 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/conf.py
+-rw-r--r--   0 wutwut     (501) staff       (20)       33 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/contributing.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)       28 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/history.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)      501 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/index.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)      191 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/installation.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)     6461 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/make.bat
+-rw-r--r--   0 wutwut     (501) staff       (20)     6766 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/Makefile
+-rw-r--r--   0 wutwut     (501) staff       (20)       27 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/readme.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)       75 2017-03-20 19:45:20.000000 pipreqs-0.4.9/docs/usage.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)     3269 2017-06-30 12:26:32.000000 pipreqs-0.4.9/HISTORY.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)    11358 2017-03-20 19:45:20.000000 pipreqs-0.4.9/LICENSE
+-rw-r--r--   0 wutwut     (501) staff       (20)      306 2017-03-20 19:45:20.000000 pipreqs-0.4.9/MANIFEST.in
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs/
+-rwxr-xr-x   0 wutwut     (501) staff       (20)      118 2017-06-30 18:19:04.000000 pipreqs-0.4.9/pipreqs/__init__.py
+-rw-r--r--   0 wutwut     (501) staff       (20)    26296 2017-06-30 12:23:23.000000 pipreqs-0.4.9/pipreqs/mapping
+-rwxr-xr-x   0 wutwut     (501) staff       (20)    13981 2017-06-30 18:17:53.000000 pipreqs-0.4.9/pipreqs/pipreqs.py
+-rw-r--r--   0 wutwut     (501) staff       (20)    12204 2017-03-20 19:45:20.000000 pipreqs-0.4.9/pipreqs/stdlib
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/
+-rw-r--r--   0 wutwut     (501) staff       (20)        1 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/dependency_links.txt
+-rw-r--r--   0 wutwut     (501) staff       (20)       50 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/entry_points.txt
+-rw-r--r--   0 wutwut     (501) staff       (20)        1 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/not-zip-safe
+-rw-r--r--   0 wutwut     (501) staff       (20)     8489 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/PKG-INFO
+-rw-r--r--   0 wutwut     (501) staff       (20)       12 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/requires.txt
+-rw-r--r--   0 wutwut     (501) staff       (20)      805 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/SOURCES.txt
+-rw-r--r--   0 wutwut     (501) staff       (20)        8 2017-06-30 18:20:03.000000 pipreqs-0.4.9/pipreqs.egg-info/top_level.txt
+-rw-r--r--   0 wutwut     (501) staff       (20)     8489 2017-06-30 18:20:03.000000 pipreqs-0.4.9/PKG-INFO
+-rw-r--r--   0 wutwut     (501) staff       (20)     2459 2017-06-30 12:23:23.000000 pipreqs-0.4.9/README.rst
+-rw-r--r--   0 wutwut     (501) staff       (20)       61 2017-06-30 18:20:03.000000 pipreqs-0.4.9/setup.cfg
+-rwxr-xr-x   0 wutwut     (501) staff       (20)     1682 2017-03-20 19:45:20.000000 pipreqs-0.4.9/setup.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/
+-rwxr-xr-x   0 wutwut     (501) staff       (20)       24 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/__init__.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_data/
+-rw-r--r--   0 wutwut     (501) staff       (20)        0 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data/models.py
+-rw-r--r--   0 wutwut     (501) staff       (20)     1524 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data/test.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_data_duplicated_deps/
+-rw-r--r--   0 wutwut     (501) staff       (20)      176 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data_duplicated_deps/db.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_data_ignore/
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_data_ignore/.ignore_second/
+-rw-r--r--   0 wutwut     (501) staff       (20)       81 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data_ignore/.ignore_second/ignored.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_data_ignore/.ignored_dir/
+-rw-r--r--   0 wutwut     (501) staff       (20)       51 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data_ignore/.ignored_dir/ignored.py
+-rw-r--r--   0 wutwut     (501) staff       (20)     1524 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_data_ignore/test.py
+drwxr-xr-x   0 wutwut     (501) staff       (20)        0 2017-06-30 18:20:03.000000 pipreqs-0.4.9/tests/_invalid_data/
+-rw-r--r--   0 wutwut     (501) staff       (20)       38 2017-03-20 19:45:20.000000 pipreqs-0.4.9/tests/_invalid_data/invalid.py
+-rwxr-xr-x   0 wutwut     (501) staff       (20)     8023 2017-06-30 12:23:23.000000 pipreqs-0.4.9/tests/test_pipreqs.py
```

### Comparing `pipreqs-0.4.8/CONTRIBUTING.rst` & `pipreqs-0.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/docs/conf.py` & `pipreqs-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/docs/make.bat` & `pipreqs-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/docs/Makefile` & `pipreqs-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/HISTORY.rst` & `pipreqs-0.4.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/LICENSE` & `pipreqs-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/pipreqs/mapping` & `pipreqs-0.4.9/pipreqs/mapping`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/pipreqs/pipreqs.py` & `pipreqs-0.4.9/pipreqs/pipreqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,19 @@
 REGEXP = [
     re.compile(r'^import (.+)$'),
     re.compile(r'^from ((?!\.+).*?) import (?:.*)$')
 ]
 
 if sys.version_info[0] > 2:
     open_func = open
+    py2 = False
 else:
     open_func = codecs.open
+    py2 = True
+    py2_exclude = ["concurrent", "concurrent.futures"]
 
 
 def get_all_imports(path, encoding=None, extra_ignore_dirs=None):
     imports = set()
     raw_imports = set()
     candidates = []
     ignore_errors = False
@@ -98,14 +101,15 @@
         imports.add(cleaned_name)
 
     packages = set(imports) - set(set(candidates) & set(imports))
     logging.debug('Found packages: {0}'.format(packages))
 
     with open(join("stdlib"), "r") as f:
         data = [x.strip() for x in f.readlines()]
+        data = [x for x in data if x not in py2_exclude] if py2 else data
         return sorted(list(set(packages) - set(data)))
 
 
 def filter_line(l):
     return len(l) > 0 and l[0] != "#"
```

### Comparing `pipreqs-0.4.8/pipreqs/stdlib` & `pipreqs-0.4.9/pipreqs/stdlib`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/pipreqs.egg-info/PKG-INFO` & `pipreqs-0.4.9/pipreqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pipreqs
-Version: 0.4.8
+Version: 0.4.9
 Summary: Pip requirements.txt generator based on imports in project
 Home-page: https://github.com/bndr/pipreqs
 Author: Vadim Kravcenko
 Author-email: vadim.kravcenko@gmail.com
 License: Apache License
 Description: ===============================
         ``pipreqs`` - Generate requirements.txt file for any project based on imports
```

### Comparing `pipreqs-0.4.8/pipreqs.egg-info/SOURCES.txt` & `pipreqs-0.4.9/pipreqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/PKG-INFO` & `pipreqs-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pipreqs
-Version: 0.4.8
+Version: 0.4.9
 Summary: Pip requirements.txt generator based on imports in project
 Home-page: https://github.com/bndr/pipreqs
 Author: Vadim Kravcenko
 Author-email: vadim.kravcenko@gmail.com
 License: Apache License
 Description: ===============================
         ``pipreqs`` - Generate requirements.txt file for any project based on imports
```

### Comparing `pipreqs-0.4.8/README.rst` & `pipreqs-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/setup.py` & `pipreqs-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/tests/_data/test.py` & `pipreqs-0.4.9/tests/_data/test.py`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/tests/_data_ignore/test.py` & `pipreqs-0.4.9/tests/_data_ignore/test.py`

 * *Files identical despite different names*

### Comparing `pipreqs-0.4.8/tests/test_pipreqs.py` & `pipreqs-0.4.9/tests/test_pipreqs.py`

 * *Files identical despite different names*

