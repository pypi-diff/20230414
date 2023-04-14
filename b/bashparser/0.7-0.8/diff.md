# Comparing `tmp/bashparser-0.7.tar.gz` & `tmp/bashparser-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bashparser-0.7.tar", last modified: Fri Mar 31 23:48:26 2023, max compression
+gzip compressed data, was "bashparser-0.8.tar", last modified: Fri Apr 14 20:38:56 2023, max compression
```

## Comparing `bashparser-0.7.tar` & `bashparser-0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:48:26.139674 bashparser-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 23:48:08.000000 bashparser-0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-31 23:48:26.139674 bashparser-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-03-31 23:48:08.000000 bashparser-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:48:26.135674 bashparser-0.7/bashparser/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2200 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20757 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/ast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7410 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/chunk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/complexity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8432 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5761 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/generalize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:48:26.139674 bashparser-0.7/bashparser/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_unroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/test/test_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1981 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/unroll.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13378 2023-03-31 23:48:08.000000 bashparser-0.7/bashparser/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:48:26.139674 bashparser-0.7/bashparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 23:48:26.000000 bashparser-0.7/bashparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-31 23:48:26.139674 bashparser-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-31 23:48:08.000000 bashparser-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 20:38:43.000000 bashparser-0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 20:38:56.216926 bashparser-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-04-14 20:38:43.000000 bashparser-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2200 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20757 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/ast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7410 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/chunk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/complexity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8432 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5761 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/generalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_unroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1981 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/unroll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13416 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 20:38:56.216926 bashparser-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-14 20:38:43.000000 bashparser-0.8/setup.py
```

### Comparing `bashparser-0.7/LICENSE.txt` & `bashparser-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/README.md` & `bashparser-0.8/README.md`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/__init__.py` & `bashparser-0.8/bashparser/__init__.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/ast.py` & `bashparser-0.8/bashparser/ast.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/chunk.py` & `bashparser-0.8/bashparser/chunk.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/commands.py` & `bashparser-0.8/bashparser/commands.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/complexity.py` & `bashparser-0.8/bashparser/complexity.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/functions.py` & `bashparser-0.8/bashparser/functions.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/generalize.py` & `bashparser-0.8/bashparser/generalize.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/template.py` & `bashparser-0.8/bashparser/template.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_ast.py` & `bashparser-0.8/bashparser/test/test_ast.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_command.py` & `bashparser-0.8/bashparser/test/test_command.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_features.py` & `bashparser-0.8/bashparser/test/test_features.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_functions.py` & `bashparser-0.8/bashparser/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_unroll.py` & `bashparser-0.8/bashparser/test/test_unroll.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/test/test_variable.py` & `bashparser-0.8/bashparser/test/test_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         # test two updates in a row doesn't append the new values
         var_list = {}
         node = bashparser.parse('a=3')[0]
         new_var_list = update_variable_list(node, var_list)
         self.assertTrue({'a':['3']} == new_var_list)
         node = bashparser.parse('a=4')[0]
         new_var_list = update_variable_list(node, new_var_list)
-        self.assertTrue({'a':['3', '4']} == new_var_list)
+        self.assertTrue({'a':['4']} == new_var_list)
     
 
     def test_update_var_list_with_for_loop(self):
         # Test that for loops work
         for_node = bashlex.parse('for a in "one two three"\n do\n echo something\n done')[0].list[0]
         new_var_list = update_variable_list(for_node, {})
         self.assertTrue(new_var_list == {'a':['one', 'two', 'three']})
```

### Comparing `bashparser-0.7/bashparser/unroll.py` & `bashparser-0.8/bashparser/unroll.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/bashparser/variables.py` & `bashparser-0.8/bashparser/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,36 +157,36 @@
         if type(node) is not bashlex.ast.node: raise ValueError('Error! bashparser.variables.update_variable_list(node != list of bashlex.ast.node)')
     if type(var_list) is not dict: raise ValueError('Error! bashparser.variables.update_variable_list(var_list != dict)')
 
     def apply_fn(node, var_list):
         """ We need to treat a variable and for loop seperately because a string in a for loop is actually an array """
         if node.kind == 'assignment':
             name, value = node.word.split('=', maxsplit=1)
-            var_list = add_variable_to_list(var_list, name, value)
+            var_list = add_variable_to_list(var_list, name, value, append=False)
         elif node.kind == 'for':
             var_list = update_var_list_with_for_loop(node, var_list)
         return CONT
     for node in nodes:
         NodeVisitor(node).apply(apply_fn, var_list)
     return var_list
 
 
-def add_variable_to_list(var_list, name, values): 
+def add_variable_to_list(var_list, name, values, append=True): 
     """ (variable dict, name, value) Adds the corresponding name and value to dictionary. If name exists in 
         the dictionary, the value is added. Prevents bugs with use of the var_list """
 
     if type(var_list) is not dict: raise ValueError('Error! bashparser.variables.add_variable_to_list(var_list != dict)')
     if type(name) is not str: raise ValueError('Error! bashparser.variables.add_variable_to_list(name != str)')
     if type(values) is not list: values = [ values ]
     
     """ We are only going to save things as arrays. This makes the unwrapping/replacing in the node structure easier """
     for i, val in enumerate(values):
         if type(val) is not str and type(val) is not bashlex.ast.node: values[i] = str(val)    
 
-    if name in var_list:
+    if name in var_list and append:
         for val in values:
             if val not in var_list[name]:
                 var_list[name] += [ val ]
     else: 
         var_list[name] = values
     return var_list
```

### Comparing `bashparser-0.7/bashparser.egg-info/SOURCES.txt` & `bashparser-0.8/bashparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bashparser-0.7/setup.cfg` & `bashparser-0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bashparser
-version = 0.7
+version = 0.8
 author = Spencer Stingley
 description = A framework for manipulating and analysing bash scripts
 long_description = A framework for manipulating and analysing bash scripts
 url = https://github.com/BlankCanvasStudio/bashparse
 keywords = bash, parsing, analysis
 python_requires = >=3.6
 classifiers =
```

### Comparing `bashparser-0.7/setup.py` & `bashparser-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bashparser",
-    version="0.7",
+    version="0.8",
     author="Spencer Stingley",
     author_email="sstingle@usc.edu",
     description="A framework for manipulating and analysing bash scripts",
     long_description="A framework for manipulating and analysing bash scripts",
     long_description_content_type="text/markdown",
     url="https://github.com/BlankCanvasStudio/bashparse",
     packages=setuptools.find_packages(),
```

