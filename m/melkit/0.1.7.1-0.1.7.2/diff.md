# Comparing `tmp/melkit-0.1.7.1.tar.gz` & `tmp/melkit-0.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melkit-0.1.7.1.tar", last modified: Fri Apr 14 08:18:18 2023, max compression
+gzip compressed data, was "melkit-0.1.7.2.tar", last modified: Fri Apr 14 08:41:23 2023, max compression
```

## Comparing `melkit-0.1.7.1.tar` & `melkit-0.1.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:18:18.804560 melkit-0.1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 08:18:14.000000 melkit-0.1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 08:18:14.000000 melkit-0.1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 08:18:18.804560 melkit-0.1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 08:18:14.000000 melkit-0.1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:18:18.804560 melkit-0.1.7.1/melkit/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 08:18:14.000000 melkit-0.1.7.1/melkit/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:18:18.804560 melkit-0.1.7.1/melkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 08:18:18.000000 melkit-0.1.7.1/melkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 08:18:18.000000 melkit-0.1.7.1/melkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:18:18.000000 melkit-0.1.7.1/melkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 08:18:18.000000 melkit-0.1.7.1/melkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 08:18:18.000000 melkit-0.1.7.1/melkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 08:18:14.000000 melkit-0.1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:18:18.804560 melkit-0.1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 08:18:14.000000 melkit-0.1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:41:23.394890 melkit-0.1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 08:41:22.000000 melkit-0.1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 08:41:22.000000 melkit-0.1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 08:41:23.394890 melkit-0.1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 08:41:22.000000 melkit-0.1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:41:23.390890 melkit-0.1.7.2/melkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21263 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 08:41:22.000000 melkit-0.1.7.2/melkit/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:41:23.390890 melkit-0.1.7.2/melkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 08:41:23.000000 melkit-0.1.7.2/melkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 08:41:23.000000 melkit-0.1.7.2/melkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:41:23.000000 melkit-0.1.7.2/melkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 08:41:23.000000 melkit-0.1.7.2/melkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 08:41:23.000000 melkit-0.1.7.2/melkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 08:41:22.000000 melkit-0.1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:41:23.394890 melkit-0.1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 08:41:22.000000 melkit-0.1.7.2/setup.py
```

### Comparing `melkit-0.1.7.1/LICENSE` & `melkit-0.1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `melkit-0.1.7.1/README.md` & `melkit-0.1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `melkit-0.1.7.1/melkit/inputs.py` & `melkit-0.1.7.2/melkit/inputs.py`

 * *Files identical despite different names*

### Comparing `melkit-0.1.7.1/melkit/toolkit.py` & `melkit-0.1.7.2/melkit/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,30 +504,35 @@
         '''
         ids = self.get_available_ids(obj_list)
         df = DataFrame(ids, columns=['IDs'])
         df.to_csv(title, index=False)
 
         return df
 
-    def remove_comments(self, new_file: str = None) -> None:
+    def remove_comments(self, overwrite=False, new_file: str = None) -> None:
         '''
         Remove comments from input file.
         '''
 
+        src_file = self._filename
         new_file = new_file or self._filename + '_NEW'
 
-        with open(self._filename, 'r') as f1, open(new_file, 'w') as f2:
+        with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
             for line in f1:
                 if line.startswith('*') and '*EOR*' not in line:
                     f2.write('')
                 elif '*' in line and '*EOR*' not in line:
                     f2.write(line[:line.find('*')] + '\n')
                 else:
                     f2.write(line)
 
+        if overwrite:
+            remove(src_file)
+            rename(new_file, src_file)
+
     def id_search(self, obj_list: List[Object], id: str) -> Object:
         '''
         Searches for an input object (CV, FL...) by its ID in a list of input elements.
         '''
         return [x for x in obj_list if f'{id}00' in x.records.keys()][0]
 
     def get_duplicated(self, obj_list: List[Object]) -> List[Object]:
```

### Comparing `melkit-0.1.7.1/setup.py` & `melkit-0.1.7.2/setup.py`

 * *Files identical despite different names*

