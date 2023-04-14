# Comparing `tmp/invokify-0.1.0.tar.gz` & `tmp/invokify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokify-0.1.0.tar", max compression
+gzip compressed data, was "invokify-0.1.1.tar", max compression
```

## Comparing `invokify-0.1.0.tar` & `invokify-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      125 2023-04-13 18:07:57.679195 invokify-0.1.0/invokify/__init__.py
--rw-r--r--   0        0        0     6759 2023-04-14 14:22:54.857854 invokify-0.1.0/invokify/invokify.py
--rw-r--r--   0        0        0     2178 2023-04-14 14:17:52.140139 invokify-0.1.0/invokify/parser.py
--rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.0/LICENSE
--rw-r--r--   0        0        0      346 2023-04-14 19:41:32.906525 invokify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1937 2023-04-13 20:57:27.279919 invokify-0.1.0/README.md
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 invokify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-14 21:08:33.165762 invokify-0.1.1/invokify/__init__.py
+-rw-r--r--   0        0        0     6886 2023-04-14 20:37:10.251034 invokify-0.1.1/invokify/invokify.py
+-rw-r--r--   0        0        0     2208 2023-04-14 20:15:39.083725 invokify-0.1.1/invokify/parser.py
+-rw-r--r--   0        0        0     1082 2023-04-14 19:28:07.595190 invokify-0.1.1/LICENSE
+-rw-r--r--   0        0        0      346 2023-04-14 21:08:44.870955 invokify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2125 2023-04-14 21:08:46.184136 invokify-0.1.1/README.md
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 invokify-0.1.1/PKG-INFO
```

### Comparing `invokify-0.1.0/invokify/invokify.py` & `invokify-0.1.1/invokify/invokify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Invokify
 
 Allows the creation of parsible commands using decorators.
 """
+__all__ = ["CommandAlreadyExists", "EngineRequired", "meta", "Command", "InvokeEngine"]
 
 import functools
 from dataclasses import dataclass, field
 
 
 class CommandAlreadyExists(Exception):
     """
@@ -213,14 +214,17 @@
             return (_command, command_list, tuple(_callstack))
 
         return self.parse(
             command_list=command_list[1:], _command=command, _callstack=_callstack
         )
 
     def command(
-        self, func: callable = None, name: str = None, aliases: list[str] = None
+        self,
+        func: callable | Command = None,
+        name: str = None,
+        aliases: list[str] = None,
     ) -> Command:
         """A decorator that turns a function into a command"""
 
         return create_command(
             func=func, commanddict=self.commands, name=name, aliases=aliases
         )
```

### Comparing `invokify-0.1.0/invokify/parser.py` & `invokify-0.1.1/invokify/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tokenstream import Token, TokenStream
 import re
 
+__all__ = ["string_to_args"]
 
 ESCAPE_REGEX = re.compile(r"\\.")
 
 ESCAPE_SEQUENCES = {
     r"\n": "\n",
     r"\"": '"',
     r"\\": "\\",
```

### Comparing `invokify-0.1.0/LICENSE` & `invokify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invokify-0.1.0/README.md` & `invokify-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Welcome to Invokify
 
 Invokify is a lightweight library that allows you to run functions from a string or list of values.
 
+
+---
+
+## Installing
+Invokify is published on PyPI so you can easily install it with either `pip` or `poetry`.
+```shell
+pip install invokify
+```
+```shell
+poetry add invokify
+```
+---
 ## Getting started
 
-Let's create a few simple command-line commands.
+Let's create a simple command-line command.
 
 We can start by importing the `InvokeEngine` from invokify:
 
 ```py
 from invokify import InvokeEngine
 ```
 Now we need to create an engine to hold our commands:
```

### Comparing `invokify-0.1.0/PKG-INFO` & `invokify-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokify
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: iRedSC
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,17 +12,29 @@
 Requires-Dist: tokenstream (>=1.5.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to Invokify
 
 Invokify is a lightweight library that allows you to run functions from a string or list of values.
 
+
+---
+
+## Installing
+Invokify is published on PyPI so you can easily install it with either `pip` or `poetry`.
+```shell
+pip install invokify
+```
+```shell
+poetry add invokify
+```
+---
 ## Getting started
 
-Let's create a few simple command-line commands.
+Let's create a simple command-line command.
 
 We can start by importing the `InvokeEngine` from invokify:
 
 ```py
 from invokify import InvokeEngine
 ```
 Now we need to create an engine to hold our commands:
```

