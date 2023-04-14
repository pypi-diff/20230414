# Comparing `tmp/hyperparse-0.0.1.tar.gz` & `tmp/hyperparse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparse-0.0.1.tar", last modified: Thu Apr 13 11:41:33 2023, max compression
+gzip compressed data, was "hyperparse-0.0.2.tar", last modified: Fri Apr 14 07:05:45 2023, max compression
```

## Comparing `hyperparse-0.0.1.tar` & `hyperparse-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-13 11:41:33.241222 hyperparse-0.0.1/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1938 2023-04-13 11:41:33.238222 hyperparse-0.0.1/PKG-INFO
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1610 2023-04-13 11:40:21.000000 hyperparse-0.0.1/README.md
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-13 11:41:33.206221 hyperparse-0.0.1/hyperparse/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.1/hyperparse/__init__.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1573 2023-04-13 11:09:31.000000 hyperparse-0.0.1/hyperparse/hyperparse.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       21 2023-04-13 09:28:46.000000 hyperparse-0.0.1/hyperparse/version.py
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-13 11:41:33.228222 hyperparse-0.0.1/hyperparse.egg-info/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1938 2023-04-13 11:41:32.000000 hyperparse-0.0.1/hyperparse.egg-info/PKG-INFO
--rw-r--r--   0 zhfu     (32413) info_fil (10015)      237 2023-04-13 11:41:33.000000 hyperparse-0.0.1/hyperparse.egg-info/SOURCES.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)        1 2023-04-13 11:41:32.000000 hyperparse-0.0.1/hyperparse.egg-info/dependency_links.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       11 2023-04-13 11:41:32.000000 hyperparse-0.0.1/hyperparse.egg-info/top_level.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       38 2023-04-13 11:41:33.242221 hyperparse-0.0.1/setup.cfg
--rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.1/setup.py
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-13 11:41:33.234221 hyperparse-0.0.1/test/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1449 2023-04-13 11:38:47.000000 hyperparse-0.0.1/test/test.py
+drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.419588 hyperparse-0.0.2/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2016 2023-04-14 07:05:45.417588 hyperparse-0.0.2/PKG-INFO
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     1725 2023-04-14 07:04:57.000000 hyperparse-0.0.2/README.md
+drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.386588 hyperparse-0.0.2/hyperparse/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.2/hyperparse/__init__.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2510 2023-04-13 20:00:07.000000 hyperparse-0.0.2/hyperparse/hyperparse.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       21 2023-04-13 15:01:26.000000 hyperparse-0.0.2/hyperparse/version.py
+drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.409588 hyperparse-0.0.2/hyperparse.egg-info/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2016 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/PKG-INFO
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)      237 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/SOURCES.txt
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)        1 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/dependency_links.txt
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       11 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/top_level.txt
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       38 2023-04-14 07:05:45.419588 hyperparse-0.0.2/setup.cfg
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.2/setup.py
+drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.413588 hyperparse-0.0.2/test/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2111 2023-04-13 19:08:23.000000 hyperparse-0.0.2/test/test.py
```

### Comparing `hyperparse-0.0.1/PKG-INFO` & `hyperparse-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
-License: UNKNOWN
 Keywords: Shell env
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# Hyperparse : a Simple Shell Environment Variables Parser 
+# Hyperparse : A Simple Shell Environment Variables Parser 
 
 ## Introduction
 This script provides a way to parse environment variables and use them as hyperparameters in Python scripts.
 
 The script parses a string that contains a comma-separated list of key-value pairs, where each key-value pair is separated by an equal sign (=). The keys should be strings, and the values can be integers, floats, lists of integers or floats, booleans, or None. The script can handle values that are enclosed in single or double quotes.
 
 The script also provides a set_hyper function that allows you to set the variables in your Python script. You can pass in a dictionary of hyperparameters and a namespace or dictionary of arguments. The function will update the namespace or dictionary with the hyperparameters.
@@ -27,36 +25,38 @@
 export usermode="a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
 python main.py
 ```
 
 ### Parse variables
 ```python
 # main.py
-from hyperparser import usermode
+from hyperparser import get_hyper
+usermode = get_hyper("usermode")
 print(usermode)
 # {"a": 1, "b": None, "c": [1, 2, 3], "d": 4, "e": 3.2, "f": "itud"}
 ```
 
 ### Reset argparse elements
 
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 parser = argparse.ArgumentParser()
 parser.add_argument('--a', type=int, default=5)
 parser.add_argument('--f', type=str, default="hello")
 args = parser.parse_args()
 set_hyper(usermode, args)
 print(args) # Namespace(a=1, f='itud')
 ```
 
 ### Reset Local Variables
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 a = 5
 f = "stk"
 set_hyper(usermode)
 print(a) # 1
 print(f) # itud
-```
-
+```# hyperparse
```

### Comparing `hyperparse-0.0.1/README.md` & `hyperparse-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Hyperparse : a Simple Shell Environment Variables Parser 
+# Hyperparse : A Simple Shell Environment Variables Parser 
 
 ## Introduction
 This script provides a way to parse environment variables and use them as hyperparameters in Python scripts.
 
 The script parses a string that contains a comma-separated list of key-value pairs, where each key-value pair is separated by an equal sign (=). The keys should be strings, and the values can be integers, floats, lists of integers or floats, booleans, or None. The script can handle values that are enclosed in single or double quotes.
 
 The script also provides a set_hyper function that allows you to set the variables in your Python script. You can pass in a dictionary of hyperparameters and a namespace or dictionary of arguments. The function will update the namespace or dictionary with the hyperparameters.
@@ -14,35 +14,38 @@
 export usermode="a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
 python main.py
 ```
 
 ### Parse variables
 ```python
 # main.py
-from hyperparser import usermode
+from hyperparser import get_hyper
+usermode = get_hyper("usermode")
 print(usermode)
 # {"a": 1, "b": None, "c": [1, 2, 3], "d": 4, "e": 3.2, "f": "itud"}
 ```
 
 ### Reset argparse elements
 
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 parser = argparse.ArgumentParser()
 parser.add_argument('--a', type=int, default=5)
 parser.add_argument('--f', type=str, default="hello")
 args = parser.parse_args()
 set_hyper(usermode, args)
 print(args) # Namespace(a=1, f='itud')
 ```
 
 ### Reset Local Variables
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 a = 5
 f = "stk"
 set_hyper(usermode)
 print(a) # 1
 print(f) # itud
-```
+```# hyperparse
```

### Comparing `hyperparse-0.0.1/hyperparse/hyperparse.py` & `hyperparse-0.0.2/hyperparse/hyperparse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import re
 import os
 import inspect
 import argparse
 import ctypes
+import sys
+
+global var_list
+var_list = {}
 
 def parse_value(value):
     if value.isdigit():
         return int(value)
     elif "." in value and value.replace(".", "", 1).isdigit():
         return float(value)
     elif value.lower() == "none":
@@ -30,23 +34,56 @@
             value = [parse_value(v) for v in value]
         else:
             value = parse_value(value)
         d[key] = value
     return d
 
 #s = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-env_vars = os.environ
-for key, value in env_vars.items():
+def parse_env(name):
+    env_vars = os.environ
+    value = env_vars[name]
+    result = parse_string(value)
+    var_list[name] = result
+    var_list[name + "_str"] = value
+
+"""for key, value in env_vars.items():
     result = parse_string(value)
     if key not in globals():
         globals()[key] = result
+        globals()[key + "_str"] = value"""
+
+
+def get_hyper(name):
+    if name not in var_list:
+        if name in os.environ:
+            parse_env(name)
+        elif f"--{name}" in sys.argv:
+            parse_arg(name)
+        else:
+            return {}
+    return var_list[name]
+
+def get_hyper_str(name):
+    if name not in var_list:
+        get_hyper(name)
+    return var_list[name + "_str"]
+
+def parse_arg(name):
+    parser = argparse.ArgumentParser()
+    parser.add_argument(f"--{name}", type=str, default="")
+    args, unknown_args = parser.parse_known_args()
+    value = getattr(args, name)
+    result = parse_string(value)
+    var_list[name] = result
+    var_list[name + "_str"] = value
+    sys.argv = [sys.argv[0]] + unknown_args
 
-def set_hyper(hyper, pargs=None):
+def reset_hyper(hyper, pargs=None):
     if type(hyper) is str:
-        hyper = globals()[hyper]
+        hyper = get_hyper(hyper)
     if pargs is None:
         frame = inspect.currentframe().f_back
         pargs = frame.f_locals
     for k in hyper:
         v = hyper[k]
         if isinstance(pargs, argparse.Namespace) and hasattr(pargs, k):
             setattr(pargs, k, v)
```

### Comparing `hyperparse-0.0.1/hyperparse.egg-info/PKG-INFO` & `hyperparse-0.0.2/hyperparse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
-License: UNKNOWN
 Keywords: Shell env
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# Hyperparse : a Simple Shell Environment Variables Parser 
+# Hyperparse : A Simple Shell Environment Variables Parser 
 
 ## Introduction
 This script provides a way to parse environment variables and use them as hyperparameters in Python scripts.
 
 The script parses a string that contains a comma-separated list of key-value pairs, where each key-value pair is separated by an equal sign (=). The keys should be strings, and the values can be integers, floats, lists of integers or floats, booleans, or None. The script can handle values that are enclosed in single or double quotes.
 
 The script also provides a set_hyper function that allows you to set the variables in your Python script. You can pass in a dictionary of hyperparameters and a namespace or dictionary of arguments. The function will update the namespace or dictionary with the hyperparameters.
@@ -27,36 +25,38 @@
 export usermode="a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
 python main.py
 ```
 
 ### Parse variables
 ```python
 # main.py
-from hyperparser import usermode
+from hyperparser import get_hyper
+usermode = get_hyper("usermode")
 print(usermode)
 # {"a": 1, "b": None, "c": [1, 2, 3], "d": 4, "e": 3.2, "f": "itud"}
 ```
 
 ### Reset argparse elements
 
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 parser = argparse.ArgumentParser()
 parser.add_argument('--a', type=int, default=5)
 parser.add_argument('--f', type=str, default="hello")
 args = parser.parse_args()
 set_hyper(usermode, args)
 print(args) # Namespace(a=1, f='itud')
 ```
 
 ### Reset Local Variables
 ```python
 # main.py
-from hyperparse import usermode, set_hyper
+from hyperparse import get_hyper, set_hyper
+usermode = get_hyper("usermode")
 a = 5
 f = "stk"
 set_hyper(usermode)
 print(a) # 1
 print(f) # itud
-```
-
+```# hyperparse
```

### Comparing `hyperparse-0.0.1/setup.py` & `hyperparse-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `hyperparse-0.0.1/test/test.py` & `hyperparse-0.0.2/test/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,41 +4,56 @@
 import argparse
 sys.path.append(".")
 
 class TestHyperParse(unittest.TestCase):
 
     def test_basic(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import usermode
-        self.assertDictEqual(usermode, {'a': 1, 'b': None, 'c': [1, 2, 3], 'd': 4, 'e': 3.2, 'f': 'itud', 'g': False})
+        from hyperparse import get_hyper
+        self.assertDictEqual(get_hyper("usermode"), {'a': 1, 'b': None, 'c': [1, 2, 3], 'd': 4, 'e': 3.2, 'f': 'itud', 'g': False})
 
     def test_argparse(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import usermode, set_hyper
+        from hyperparse import get_hyper, reset_hyper
+        get_hyper("usermode")
         parser = argparse.ArgumentParser()
         parser.add_argument('--a', type=int, default=5)
         parser.add_argument('--f', type=str, default="hello")
         args = parser.parse_args()
-        set_hyper(usermode, args)
+        reset_hyper(get_hyper("usermode"), args)
         self.assertEqual(args.a, 1)
         self.assertEqual(args.f, "itud")
 
     def test_func(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import usermode, set_hyper
+        from hyperparse import get_hyper, reset_hyper
+        usermode = get_hyper("usermode")
         a = 5
         f = "stk"
-        set_hyper(usermode)
+        reset_hyper(usermode)
         self.assertEqual(a, 1)
         self.assertEqual(f, "itud")
 
     def test_func_strname(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import set_hyper
+        from hyperparse import reset_hyper
         a = 5
         f = "stk"
-        set_hyper("usermode")
+        reset_hyper("usermode")
         self.assertEqual(a, 1)
         self.assertEqual(f, "itud")
 
+    def test_parse_arg(self):
+        sys.argv += ["--usermode", "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"]
+        import hyperparse 
+        hyperparse.parse_arg("usermode")
+        parser = argparse.ArgumentParser()
+        parser.add_argument('--a', type=int, default=5)
+        parser.add_argument('--f', type=str, default="hello")
+        args = parser.parse_args()
+        usermode = hyperparse.get_hyper("usermode")
+        hyperparse.reset_hyper(usermode, args)
+        self.assertEqual(args.a, 1)
+        self.assertEqual(args.f, "itud")
+
 if __name__ == '__main__':
     unittest.main()
```

