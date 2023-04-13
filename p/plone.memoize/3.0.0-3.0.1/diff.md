# Comparing `tmp/plone.memoize-3.0.0.tar.gz` & `tmp/plone.memoize-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.memoize-3.0.0.tar", last modified: Fri Oct 28 21:02:59 2022, max compression
+gzip compressed data, was "plone.memoize-3.0.1.tar", last modified: Thu Apr 13 23:12:29 2023, max compression
```

## Comparing `plone.memoize-3.0.0.tar` & `plone.memoize-3.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)    18065 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      366 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1519 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/docs/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2171 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone/memoize/
--rw-r--r--   0 maurits    (501) staff       (20)      704 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1354 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/compress.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1777 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/instance.py
--rw-r--r--   0 maurits    (501) staff       (20)      316 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4607 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/instance.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2669 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/request.py
--rw-r--r--   0 maurits    (501) staff       (20)       24 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2645 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/ram.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7560 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/view.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2722 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      642 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/compress.py
--rw-r--r--   0 maurits    (501) staff       (20)     3509 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/request.rst
--rw-r--r--   0 maurits    (501) staff       (20)      565 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/forever.py
--rw-r--r--   0 maurits    (501) staff       (20)     2218 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/volatile.py
--rw-r--r--   0 maurits    (501) staff       (20)     4137 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2213 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1216 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/forever.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7168 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/volatile.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2685 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/plone/memoize/ram.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18065 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      881 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)      165 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/plone.memoize.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      467 2022-10-28 21:02:59.000000 plone.memoize-3.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      595 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8161 2022-10-28 21:02:58.000000 plone.memoize-3.0.0/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.518461 plone.memoize-3.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     8332 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14143 2023-04-13 23:12:29.518716 plone.memoize-3.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      595 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.510250 plone.memoize-3.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1519 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/docs/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      366 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/docs/index.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.510527 plone.memoize-3.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.518235 plone.memoize-3.0.1/plone/memoize/
+-rw-r--r--   0 maurits    (501) staff       (20)     4137 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/compress.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1354 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/compress.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      320 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      541 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/forever.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/forever.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1745 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/instance.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4531 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/instance.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      680 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2540 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/ram.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2645 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/ram.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/request.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3509 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/request.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2189 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2614 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7485 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/view.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2118 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/volatile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7168 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/volatile.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.512593 plone.memoize-3.0.1/plone.memoize.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14143 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      881 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1678 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:12:29.519238 plone.memoize-3.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1990 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.memoize-3.0.0/docs/LICENSE.rst` & `plone.memoize-3.0.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/interfaces.py` & `plone.memoize-3.0.1/plone/memoize/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Interface
 
 
 class ICacheChooser(Interface):
     def __call__(fun_name):
         """Return a cache with a dict interface based on a dotted
         function name `fun_name`.
```

### Comparing `plone.memoize-3.0.0/plone/memoize/compress.rst` & `plone.memoize-3.0.1/plone/memoize/compress.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/instance.py` & `plone.memoize-3.0.1/plone/memoize/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 """Memo decorators for instances.
 
 Stores values in an attribute on the instance. See instance.rst.
 
 This package current subsumes memojito.
 """
 from functools import wraps
 
 
 _marker = object()
 
 
-class Memojito(object):
+class Memojito:
     propname = "_memojito_"
 
     def clear(self, inst):
         if hasattr(inst, self.propname):
             delattr(inst, self.propname)
 
     def clearbefore(self, func):
```

### Comparing `plone.memoize-3.0.0/plone/memoize/instance.rst` & `plone.memoize-3.0.1/plone/memoize/instance.rst`

 * *Files 2% similar despite different names*

```diff
@@ -100,18 +100,15 @@
     J.D.: goodbye cruel world! raise--roofbeams
 
     >>> print(msg.getMsg('Ernest'))
     Ernest: goodbye cruel world!
 
 If we alter the signature, our msg is recalculated, but since mst.txt2 is a memo, only the values passed in change::
 
-    >>> try:
-    ...     from collections import OrderedDict
-    ... except ImportError:
-    ...     OrderedDict = dict
+    >>> from collections import OrderedDict
     >>> ins = OrderedDict([('tale', 'told by idiot'), ('signify', 'nothing')])
     >>> print(msg.getMsg('Bill F.', **ins))
     Bill F.: goodbye cruel world! tale--told by idiot signify--nothing
 
     >>> print(msg.getMsg('J.D.', **{'catcher':'rye'}))
     J.D.: goodbye cruel world! catcher--rye
```

### Comparing `plone.memoize-3.0.0/plone/memoize/request.py` & `plone.memoize-3.0.1/plone/memoize/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-# -*- coding: utf-8 -*-
 """Memoize decorator for methods.
 
 Stores values in an annotation of the request.
 """
 from functools import wraps
+from inspect import getfullargspec
 from plone.memoize import volatile
 from zope.annotation.interfaces import IAnnotations
 
-import inspect
-
-try:
-    getargspec = inspect.getfullargspec
-except AttributeError:
-    # for Python 2
-    getargspec = inspect.getargspec
-
 
 _marker = object()
 
 
-class RequestMemo(object):
-
+class RequestMemo:
     key = "plone.memoize_request"
 
     def __init__(self, arg=0):
         self.arg = arg
 
     def __call__(self, func):
         @wraps(func)
@@ -55,15 +46,15 @@
         return memogetter
 
 
 def store_in_annotation_of(expr):
     def _store_in_annotation(fun, *args, **kwargs):
         # Use expr to find out the name of the request variable
         vars = {}
-        spec = getargspec(fun)
+        spec = getfullargspec(fun)
         num_args = len(args)
         expected_num_args = num_args
 
         # Explicitly check for the correct number of arguments and
         # raise the appropriate TypeError if needed. This is done
         # to avoid the real problem being masked by an IndexError
         # later in this method.
@@ -83,14 +74,13 @@
         request = eval(expr, {}, vars)
         return IAnnotations(request)
 
     return _store_in_annotation
 
 
 def cache(get_key, get_request="request"):
-
     return volatile.cache(get_key, get_cache=store_in_annotation_of(get_request))
 
 
 memoize_diy_request = RequestMemo
 
 __all__ = (memoize_diy_request, store_in_annotation_of, cache)
```

### Comparing `plone.memoize-3.0.0/plone/memoize/ram.rst` & `plone.memoize-3.0.1/plone/memoize/ram.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/view.rst` & `plone.memoize-3.0.1/plone/memoize/view.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,15 @@
     J.D.: goodbye cruel world! raise--roofbeams
 
     >>> print(msg.getMsg('Ernest'))
     Ernest: goodbye cruel world!
 
 If we alter the signature, our msg is recalculated::
 
-    >>> try:
-    ...     from collections import OrderedDict
-    ... except ImportError:
-    ...     OrderedDict = dict
+    >>> from collections import OrderedDict
     >>> ins = OrderedDict([('tale', 'told by idiot'), ('signify', 'nothing')])
     >>> print(msg.getMsg('Bill F.', **ins))
     Bill F.: sound and fury world! tale--told by idiot signify--nothing
 
     >>> print(msg.getMsg('J.D.', **{'catcher':'rye'}))
     J.D.: sound and fury world! catcher--rye
 
@@ -223,15 +220,15 @@
     ...     def context_aware_function(self):
     ...         return self.msg
     ...
     ...     @view.memoize_contextless
     ...     def context_unaware_function(self):
     ...         return self.msg
 
-We now instatiate two objects:
+We now instantiate two objects:
     >>> instance1 = Adapter(Dummy())
     >>> instance2 = Adapter(Dummy())
     >>> instance1.context_aware_function()
     'foo'
     >>> instance1.context_unaware_function()
     'foo'
```

### Comparing `plone.memoize-3.0.0/plone/memoize/view.py` & `plone.memoize-3.0.1/plone/memoize/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-# -*- coding: utf-8 -*-
 """Memoize decorator for views.
 
 Stores values in an annotation of the request. See view.rst.
 """
 from functools import wraps
 from zope.annotation.interfaces import IAnnotations
+from zope.globalrequest import getRequest
 
 
-try:
-    from zope.globalrequest import getRequest
-except ImportError:
-
-    def getRequest():
-        return None
-
-
-class ViewMemo(object):
-
+class ViewMemo:
     key = "plone.memoize"
 
     def memoize(self, func):
         @wraps(func)
         def memogetter(*args, **kwargs):
             instance = args[0]
 
@@ -59,15 +50,14 @@
                 cache[key] = func(*args, **kwargs)
             return cache[key]
 
         return memogetter
 
     def memoize_contextless(self, func):
         def memogetter(*args, **kwargs):
-
             if args:
                 instance = args[0]
             else:
                 instance = None
 
             try:
                 request = instance.request
```

### Comparing `plone.memoize-3.0.0/plone/memoize/request.rst` & `plone.memoize-3.0.1/plone/memoize/request.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/forever.py` & `plone.memoize-3.0.1/plone/memoize/forever.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Memo decorators for globals - memoized values survive for as long as the
 process lives.
 
 Stores values in a module-level variable.
 
 Pay attention that is module is not thread-safe, so use it with care.
 """
```

### Comparing `plone.memoize-3.0.0/plone/memoize/volatile.py` & `plone.memoize-3.0.1/plone/memoize/volatile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """A flexible caching decorator.
 
 This module provides a cache decorator `cache` that you can use to
 cache results of your functions or methods.
 """
 
 from functools import wraps
@@ -14,36 +13,36 @@
     """A dict that automatically cleans up items that haven't been
     accessed in a given timespan on *set*.
     """
 
     cleanup_period = 60 * 60 * 24 * 3  # 3 days
 
     def __init__(self, cleanup_period=None):
-        super(CleanupDict, self).__init__()
+        super().__init__()
         self._last_access = {}
         if cleanup_period is not None:
             self.cleanup_period = cleanup_period
 
     def __getitem__(self, key):
-        value = super(CleanupDict, self).__getitem__(key)
+        value = super().__getitem__(key)
         self._last_access[key] = time.time()
         return value
 
     def __setitem__(self, key, value):
-        super(CleanupDict, self).__setitem__(key, value)
+        super().__setitem__(key, value)
         self._last_access[key] = time.time()
         self._cleanup()
 
     def _cleanup(self):
         now = time.time()
         okay = now - self.cleanup_period
         for key, timestamp in list(self._last_access.items()):
             if timestamp < okay:
                 del self._last_access[key]
-                super(CleanupDict, self).__delitem__(key)
+                super().__delitem__(key)
 
 
 ATTR = "_v_memoize_cache"
 CONTAINER_FACTORY = CleanupDict
 _marker = object()
 
 
@@ -63,15 +62,15 @@
     def decorator(fun):
         @wraps(fun)
         def replacement(*args, **kwargs):
             try:
                 key = get_key(fun, *args, **kwargs)
             except DontCache:
                 return fun(*args, **kwargs)
-            key = "%s.%s:%s" % (fun.__module__, fun.__name__, key)
+            key = f"{fun.__module__}.{fun.__name__}:{key}"
             cache = get_cache(fun, *args, **kwargs)
             cached_value = cache.get(key, _marker)
             if cached_value is _marker:
                 cached_value = cache[key] = fun(*args, **kwargs)
             return cached_value
 
         return replacement
```

### Comparing `plone.memoize-3.0.0/plone/memoize/README.rst` & `plone.memoize-3.0.1/plone/memoize/README.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/tests.py` & `plone.memoize-3.0.1/plone/memoize/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from zope.component.testing import setUp
 from zope.component.testing import tearDown
 from zope.configuration.xmlconfig import XMLConfig
 
 import doctest
 import unittest
```

### Comparing `plone.memoize-3.0.0/plone/memoize/forever.rst` & `plone.memoize-3.0.1/plone/memoize/forever.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/volatile.rst` & `plone.memoize-3.0.1/plone/memoize/volatile.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/plone/memoize/ram.py` & `plone.memoize-3.0.1/plone/memoize/ram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# -*- coding: utf-8 -*-
 """A cache decorator that uses RAMCache by default.
 """
 
 from hashlib import sha1
 from plone.memoize import volatile
 from plone.memoize.interfaces import ICacheChooser
 from zope import component
 from zope import interface
 from zope.ramcache import ram
 from zope.ramcache.interfaces.ram import IRAMCache
 
-import six
-
-
-try:
-    import pickle  # Python 3
-except ImportError:
-    import cPickle as pickle  # Python 2
+import pickle
 
 
 global_cache = ram.RAMCache()
 global_cache.update(maxAge=86400)
 
 DontCache = volatile.DontCache
 MARKER = object()
@@ -36,15 +29,15 @@
 
 class MemcacheAdapter(AbstractDict):
     def __init__(self, client, globalkey=""):
         self.client = client
         self.globalkey = globalkey and "%s:" % globalkey
 
     def _make_key(self, source):
-        if issubclass(type(source), six.text_type):
+        if issubclass(type(source), str):
             source = source.encode("utf-8")
         return sha1(source).hexdigest()
 
     def __getitem__(self, key):
         cached_value = self.client.get(self.globalkey + self._make_key(key))
         if cached_value is None:
             raise KeyError(key)
@@ -58,15 +51,15 @@
 
 class RAMCacheAdapter(AbstractDict):
     def __init__(self, ramcache, globalkey=""):
         self.ramcache = ramcache
         self.globalkey = globalkey
 
     def _make_key(self, source):
-        if issubclass(type(source), six.text_type):
+        if issubclass(type(source), str):
             source = source.encode("utf-8")
         return sha1(source).digest()
 
     def __getitem__(self, key):
         value = self.ramcache.query(
             self.globalkey, dict(key=self._make_key(key)), MARKER
         )
@@ -83,15 +76,15 @@
     return RAMCacheAdapter(component.queryUtility(IRAMCache), globalkey=fun_name)
 
 
 interface.directlyProvides(choose_cache, ICacheChooser)
 
 
 def store_in_cache(fun, *args, **kwargs):
-    key = "%s.%s" % (fun.__module__, fun.__name__)
+    key = f"{fun.__module__}.{fun.__name__}"
     cache_chooser = component.queryUtility(ICacheChooser)
     if cache_chooser is not None:
         return cache_chooser(key)
     else:
         return RAMCacheAdapter(global_cache, globalkey=key)
```

### Comparing `plone.memoize-3.0.0/plone.memoize.egg-info/SOURCES.txt` & `plone.memoize-3.0.1/plone.memoize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/README.rst` & `plone.memoize-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.0/CHANGES.rst` & `plone.memoize-3.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+- Removed more Python 2 compatibility code.
+  [maurits] (#55)
+
+
 3.0.0 (2022-10-28)
 ------------------
 
 Breaking changes:
 
 
 - Drop support for Python 3.5 and 3.6.
```

