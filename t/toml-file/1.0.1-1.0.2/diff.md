# Comparing `tmp/toml_file-1.0.1.tar.gz` & `tmp/toml_file-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_file-1.0.1.tar", last modified: Thu Apr 13 15:19:06 2023, max compression
+gzip compressed data, was "toml_file-1.0.2.tar", last modified: Fri Apr 14 09:23:32 2023, max compression
```

## Comparing `toml_file-1.0.1.tar` & `toml_file-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.733468 toml_file-1.0.1/
--rw-rw-rw-   0        0        0     1456 2023-04-13 15:19:06.733468 toml_file-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2023-04-13 10:05:41.000000 toml_file-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 15:19:06.733468 toml_file-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4206 2023-04-13 15:19:02.000000 toml_file-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.717849 toml_file-1.0.1/toml_file/
--rw-rw-rw-   0        0        0      890 2023-03-20 12:20:34.000000 toml_file-1.0.1/toml_file/__init__.py
--rw-rw-rw-   0        0        0    10745 2023-04-13 15:14:12.000000 toml_file-1.0.1/toml_file/config.py
--rw-rw-rw-   0        0        0     2822 2023-04-13 08:21:31.000000 toml_file-1.0.1/toml_file/encoder.py
--rw-rw-rw-   0        0        0    39307 2023-04-13 13:02:28.000000 toml_file-1.0.1/toml_file/parser.py
--rw-rw-rw-   0        0        0    45989 2023-04-13 11:14:37.000000 toml_file-1.0.1/toml_file/types.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.733468 toml_file-1.0.1/toml_file.egg-info/
--rw-rw-rw-   0        0        0     1456 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:23:32.260177 toml_file-1.0.2/
+-rw-rw-rw-   0        0        0     1497 2023-04-14 09:23:32.260177 toml_file-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2023-04-13 10:05:41.000000 toml_file-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:23:32.260177 toml_file-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4206 2023-04-14 09:21:32.000000 toml_file-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:23:32.244553 toml_file-1.0.2/toml_file/
+-rw-rw-rw-   0        0        0      890 2023-03-20 12:20:34.000000 toml_file-1.0.2/toml_file/__init__.py
+-rw-rw-rw-   0        0        0    10778 2023-04-14 09:18:54.000000 toml_file-1.0.2/toml_file/config.py
+-rw-rw-rw-   0        0        0     2822 2023-04-13 08:21:31.000000 toml_file-1.0.2/toml_file/encoder.py
+-rw-rw-rw-   0        0        0    39307 2023-04-13 13:02:28.000000 toml_file-1.0.2/toml_file/parser.py
+-rw-rw-rw-   0        0        0    45989 2023-04-13 11:14:37.000000 toml_file-1.0.2/toml_file/types.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:23:32.244553 toml_file-1.0.2/toml_file.egg-info/
+-rw-rw-rw-   0        0        0     1497 2023-04-14 09:23:32.000000 toml_file-1.0.2/toml_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-14 09:23:32.000000 toml_file-1.0.2/toml_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:23:32.000000 toml_file-1.0.2/toml_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:23:32.000000 toml_file-1.0.2/toml_file.egg-info/top_level.txt
```

### Comparing `toml_file-1.0.1/PKG-INFO` & `toml_file-1.0.2/toml_file.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: toml_file
-Version: 1.0.1
+Name: toml-file
+Version: 1.0.2
 Summary: TOML file reader - python module to read/write toml configuration files
 Home-page: https://gitlab.com/tcharrett/totoml
 Author: Tom Charrett
 Author-email: tcharrett@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 
 
 TOML file reader - python module to read/write toml configuration files
@@ -28,7 +30,9 @@
 Config object interface:
     - allows seamless use of template/data via custom dictlike interface
     - use cfg = Config(filename) to open
     - access subtables/keys via exteneded key indexing e.g. cfg['Table1.subtable.key'] = 1
     - if a template has been set any value will be validated when it is set.
     - if a template has been set any missing values will return the defualt and be created.
     - use cfg.save(filename) to save
+
+
```

### Comparing `toml_file-1.0.1/README.md` & `toml_file-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.1/setup.py` & `toml_file-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 # Package meta-data.
 NAME = "toml_file"
 DESCRIPTION = "TOML file reader - python module to read/write toml configuration files"
 URL = "https://gitlab.com/tcharrett/totoml"
 EMAIL = "tcharrett@gmail.com"
 AUTHOR = "Tom Charrett"
 REQUIRES_PYTHON = ">=3.7.6"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {}
```

### Comparing `toml_file-1.0.1/toml_file/__init__.py` & `toml_file-1.0.2/toml_file/__init__.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.1/toml_file/config.py` & `toml_file-1.0.2/toml_file/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,19 @@
         
         data - dictionary of values to store in Config
         template - option templating dictionary/TableType
         """
         if file is not None:
             self.load(file)
         else:
-            self.data = {}
+            self.data = data
             if template is None:
-                template = {}
-            self.template = types.TableType(template)
-            self.update(data)
+                template = template
+            else:
+                self.template = types.TableType()
     
     # --- interface methods
     def load(self, file, update=False):
         """
         Load the filename or open file object given.
         
         [optional] update=True to update the current configuration with the 
@@ -156,22 +156,23 @@
             #check for dotted part
             else: 
                 parent, *rest = key.split('.',1)
                 if rest==[]:#no remaining parts get current key
                     key = parent
                     break
                 key = rest[0]
-                
+                 
             #get parent
             table = table[parent]
-            ttable = ttable[parent]
+            ttable = ttable.get(parent, {})
            
             #print('parent ', repr(parent),'key', repr(key))
         
-        #get the value and template type
+        #get the value and template type
+        #print('key', repr(key))
         value = table.get( key, None)
         tvalue = ttable.get( key, None)
         
         # no value - try template for default
         if (value is None) and (tvalue is not None):
             value = tvalue.get_default()
```

### Comparing `toml_file-1.0.1/toml_file/encoder.py` & `toml_file-1.0.2/toml_file/encoder.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.1/toml_file/parser.py` & `toml_file-1.0.2/toml_file/parser.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.1/toml_file/types.py` & `toml_file-1.0.2/toml_file/types.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.1/toml_file.egg-info/PKG-INFO` & `toml_file-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: toml-file
-Version: 1.0.1
+Name: toml_file
+Version: 1.0.2
 Summary: TOML file reader - python module to read/write toml configuration files
 Home-page: https://gitlab.com/tcharrett/totoml
 Author: Tom Charrett
 Author-email: tcharrett@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 
 
 TOML file reader - python module to read/write toml configuration files
@@ -28,7 +30,9 @@
 Config object interface:
     - allows seamless use of template/data via custom dictlike interface
     - use cfg = Config(filename) to open
     - access subtables/keys via exteneded key indexing e.g. cfg['Table1.subtable.key'] = 1
     - if a template has been set any value will be validated when it is set.
     - if a template has been set any missing values will return the defualt and be created.
     - use cfg.save(filename) to save
+
+
```

