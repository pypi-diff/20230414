# Comparing `tmp/asyncinject-0.5.tar.gz` & `tmp/asyncinject-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncinject-0.5.tar", last modified: Fri Apr 22 18:49:01 2022, max compression
+gzip compressed data, was "asyncinject-0.6.tar", last modified: Fri Apr 14 01:23:14 2023, max compression
```

## Comparing `asyncinject-0.5.tar` & `asyncinject-0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 18:49:01.064359 asyncinject-0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-22 18:48:45.000000 asyncinject-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-04-22 18:49:01.064359 asyncinject-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-04-22 18:48:45.000000 asyncinject-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 18:49:01.064359 asyncinject-0.5/asyncinject/
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-04-22 18:48:45.000000 asyncinject-0.5/asyncinject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-04-22 18:48:45.000000 asyncinject-0.5/asyncinject/vendored_graphlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 18:49:01.064359 asyncinject-0.5/asyncinject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-04-22 18:49:00.000000 asyncinject-0.5/asyncinject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-04-22 18:49:01.000000 asyncinject-0.5/asyncinject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-22 18:49:00.000000 asyncinject-0.5/asyncinject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-04-22 18:49:00.000000 asyncinject-0.5/asyncinject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-22 18:49:00.000000 asyncinject-0.5/asyncinject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-22 18:49:01.064359 asyncinject-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-04-22 18:48:45.000000 asyncinject-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:23:14.938423 asyncinject-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 01:23:00.000000 asyncinject-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-14 01:23:14.938423 asyncinject-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-14 01:23:00.000000 asyncinject-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:23:14.938423 asyncinject-0.6/asyncinject/
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 01:23:00.000000 asyncinject-0.6/asyncinject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-04-14 01:23:00.000000 asyncinject-0.6/asyncinject/vendored_graphlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:23:14.938423 asyncinject-0.6/asyncinject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-14 01:23:14.000000 asyncinject-0.6/asyncinject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 01:23:14.000000 asyncinject-0.6/asyncinject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:23:14.000000 asyncinject-0.6/asyncinject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 01:23:14.000000 asyncinject-0.6/asyncinject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 01:23:14.000000 asyncinject-0.6/asyncinject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:23:14.938423 asyncinject-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-14 01:23:00.000000 asyncinject-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:23:14.938423 asyncinject-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-14 01:23:00.000000 asyncinject-0.6/tests/test_asyncinject.py
```

### Comparing `asyncinject-0.5/LICENSE` & `asyncinject-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncinject-0.5/PKG-INFO` & `asyncinject-0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: asyncinject
-Version: 0.5
+Version: 0.6
 Summary: Run async workflows using pytest-fixtures-style dependency injection
 Home-page: https://github.com/simonw/asyncinject
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/asyncinject/issues
 Project-URL: CI, https://github.com/simonw/asyncinject/actions
 Project-URL: Changelog, https://github.com/simonw/asyncinject/releases
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # asyncinject
 
@@ -56,20 +55,55 @@
 async def both(example, simonwillison):
     return example + "\n\n" + simonwillison
 
 registry = Registry(example, simonwillison, both)
 combined = await registry.resolve(both)
 print(combined)
 ```
-If you run this in `ipython` (which supports top-level await) you will see output that combines HTML from both of those pages.
+If you run this in `ipython` or `python -m asyncio` (to enable top-level await in the console) you will see output that combines HTML from both of those pages.
 
 The HTTP requests to `www.example.com` and `simonwillison.net` will be performed in parallel.
 
 The library notices that `both()` takes two arguments which are the names of other registered `async def` functions, and will construct an execution plan that executes those two functions in parallel, then passes their results to the `both()` method.
 
+### Registry.from_dict()
+
+Passing a list of functions to the `Registry` constructor will register each function under their introspected function name, using `fn.__name__`.
+
+You can set explicit names instead using a dictionary:
+
+```python
+registry = Registry.from_dict({
+    "example": example,
+    "simonwillison": simonwillison,
+    "both": both
+})
+```
+Those string names will be used to match parameters, so each function will need to accept parameters named after the keys used in that dictionary.
+
+### Registering additional functions
+
+Functions that are registered can be regular functions or `async def` functions.
+
+In addition to registering functions by passing them to the constructor, you can also add them to a registry using the `.register()` method:
+
+```python
+async def another():
+    return "another"
+
+registry.register(another)
+```
+To register them with a name other than the name of the function, pass the `name=` argument:
+```python
+async def another():
+    return "another 2"
+
+registry.register(another, name="another_2")
+```
+
 ### Resolving an unregistered function
 
 You don't need to register the final function that you pass to `.resolve()` - if you pass an unregistered function, the library will introspect the function's parameters and resolve them directly.
 
 This works with both regular and async functions:
 
 ```python
@@ -170,9 +204,7 @@
 Now install the dependencies and test dependencies:
 
     pip install -e '.[test]'
 
 To run the tests:
 
     pytest
-
-
```

### Comparing `asyncinject-0.5/README.md` & `asyncinject-0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -40,20 +40,55 @@
 async def both(example, simonwillison):
     return example + "\n\n" + simonwillison
 
 registry = Registry(example, simonwillison, both)
 combined = await registry.resolve(both)
 print(combined)
 ```
-If you run this in `ipython` (which supports top-level await) you will see output that combines HTML from both of those pages.
+If you run this in `ipython` or `python -m asyncio` (to enable top-level await in the console) you will see output that combines HTML from both of those pages.
 
 The HTTP requests to `www.example.com` and `simonwillison.net` will be performed in parallel.
 
 The library notices that `both()` takes two arguments which are the names of other registered `async def` functions, and will construct an execution plan that executes those two functions in parallel, then passes their results to the `both()` method.
 
+### Registry.from_dict()
+
+Passing a list of functions to the `Registry` constructor will register each function under their introspected function name, using `fn.__name__`.
+
+You can set explicit names instead using a dictionary:
+
+```python
+registry = Registry.from_dict({
+    "example": example,
+    "simonwillison": simonwillison,
+    "both": both
+})
+```
+Those string names will be used to match parameters, so each function will need to accept parameters named after the keys used in that dictionary.
+
+### Registering additional functions
+
+Functions that are registered can be regular functions or `async def` functions.
+
+In addition to registering functions by passing them to the constructor, you can also add them to a registry using the `.register()` method:
+
+```python
+async def another():
+    return "another"
+
+registry.register(another)
+```
+To register them with a name other than the name of the function, pass the `name=` argument:
+```python
+async def another():
+    return "another 2"
+
+registry.register(another, name="another_2")
+```
+
 ### Resolving an unregistered function
 
 You don't need to register the final function that you pass to `.resolve()` - if you pass an unregistered function, the library will introspect the function's parameters and resolve them directly.
 
 This works with both regular and async functions:
 
 ```python
```

### Comparing `asyncinject-0.5/asyncinject/__init__.py` & `asyncinject-0.6/asyncinject/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,23 @@
         self._graph = None
         self._reversed = None
         self.parallel = parallel
         self.timer = timer
         for fn in fns:
             self.register(fn)
 
-    def register(self, fn):
-        self._registry[fn.__name__] = fn
+    @classmethod
+    def from_dict(cls, d, parallel=True, timer=None):
+        instance = cls(parallel=parallel, timer=timer)
+        for key, fn in d.items():
+            instance.register(fn, name=key)
+        return instance
+
+    def register(self, fn, *, name=None):
+        self._registry[name or fn.__name__] = fn
         # Clear caches:
         self._graph = None
         self._reversed = None
 
     def _make_time_logger(self, awaitable):
         async def inner():
             start = time.perf_counter()
@@ -82,17 +89,28 @@
             done.add(item)
             # Add any not-done dependencies to the queue
             to_do.update({k for k in dependencies if k not in done})
 
         return ts
 
     def _get_awaitable(self, name, results):
-        aw = self._registry[name](
-            **{k: v for k, v in results.items() if k in self.graph[name]},
-        )
+        fn = self._registry[name]
+        kwargs = {k: v for k, v in results.items() if k in self.graph[name]}
+
+        awaitable_fn = fn
+
+        if not asyncio.iscoroutinefunction(fn):
+
+            async def _awaitable(*args, **kwargs):
+                return fn(*args, **kwargs)
+
+            _awaitable.__name__ = fn.__name__
+            awaitable_fn = _awaitable
+
+        aw = awaitable_fn(**kwargs)
         if self.timer:
             aw = self._make_time_logger(aw)
         return aw
 
     async def _execute_sequential(self, results, ts):
         for name in ts.static_order():
             if name not in self._registry:
```

### Comparing `asyncinject-0.5/asyncinject/vendored_graphlib.py` & `asyncinject-0.6/asyncinject/vendored_graphlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
 
         if self._ready_nodes is None:
             raise ValueError("prepare() must be called first")
 
         n2i = self._node2info
 
         for node in nodes:
-
             # Check if we know about this node (it was added previously using add()
             nodeinfo = n2i.get(node)
             if nodeinfo is None:
                 raise ValueError(f"node {node!r} was not added using add()")
 
             # If the node has not being returned (marked as ready) previously, inform the user.
             stat = nodeinfo.npredecessors
```

### Comparing `asyncinject-0.5/asyncinject.egg-info/PKG-INFO` & `asyncinject-0.6/asyncinject.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: asyncinject
-Version: 0.5
+Version: 0.6
 Summary: Run async workflows using pytest-fixtures-style dependency injection
 Home-page: https://github.com/simonw/asyncinject
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/asyncinject/issues
 Project-URL: CI, https://github.com/simonw/asyncinject/actions
 Project-URL: Changelog, https://github.com/simonw/asyncinject/releases
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # asyncinject
 
@@ -56,20 +55,55 @@
 async def both(example, simonwillison):
     return example + "\n\n" + simonwillison
 
 registry = Registry(example, simonwillison, both)
 combined = await registry.resolve(both)
 print(combined)
 ```
-If you run this in `ipython` (which supports top-level await) you will see output that combines HTML from both of those pages.
+If you run this in `ipython` or `python -m asyncio` (to enable top-level await in the console) you will see output that combines HTML from both of those pages.
 
 The HTTP requests to `www.example.com` and `simonwillison.net` will be performed in parallel.
 
 The library notices that `both()` takes two arguments which are the names of other registered `async def` functions, and will construct an execution plan that executes those two functions in parallel, then passes their results to the `both()` method.
 
+### Registry.from_dict()
+
+Passing a list of functions to the `Registry` constructor will register each function under their introspected function name, using `fn.__name__`.
+
+You can set explicit names instead using a dictionary:
+
+```python
+registry = Registry.from_dict({
+    "example": example,
+    "simonwillison": simonwillison,
+    "both": both
+})
+```
+Those string names will be used to match parameters, so each function will need to accept parameters named after the keys used in that dictionary.
+
+### Registering additional functions
+
+Functions that are registered can be regular functions or `async def` functions.
+
+In addition to registering functions by passing them to the constructor, you can also add them to a registry using the `.register()` method:
+
+```python
+async def another():
+    return "another"
+
+registry.register(another)
+```
+To register them with a name other than the name of the function, pass the `name=` argument:
+```python
+async def another():
+    return "another 2"
+
+registry.register(another, name="another_2")
+```
+
 ### Resolving an unregistered function
 
 You don't need to register the final function that you pass to `.resolve()` - if you pass an unregistered function, the library will introspect the function's parameters and resolve them directly.
 
 This works with both regular and async functions:
 
 ```python
@@ -170,9 +204,7 @@
 Now install the dependencies and test dependencies:
 
     pip install -e '.[test]'
 
 To run the tests:
 
     pytest
-
-
```

### Comparing `asyncinject-0.5/setup.py` & `asyncinject-0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.5"
+VERSION = "0.6"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

