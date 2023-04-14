# Comparing `tmp/yamicache-0.6.0.tar.gz` & `tmp/yamicache-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yamicache-0.6.0.tar", last modified: Sun Nov 22 20:03:38 2020, max compression
+gzip compressed data, was "yamicache-0.7.0.tar", max compression
```

## Comparing `yamicache-0.6.0.tar` & `yamicache-0.7.0.tar`

### file list

```diff
@@ -1,40 +1,6 @@
-drwxr-xr-x   0 timcfadd  (1000) timcfadd  (1000)        0 2020-11-22 20:03:38.320469 yamicache-0.6.0/
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     3141 2020-11-22 18:56:43.000000 yamicache-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      846 2020-11-22 19:12:44.000000 yamicache-0.6.0/HISTORY.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1087 2020-11-22 18:56:43.000000 yamicache-0.6.0/LICENSE
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      252 2020-11-22 18:56:43.000000 yamicache-0.6.0/MANIFEST.in
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     3580 2020-11-22 20:03:38.320469 yamicache-0.6.0/PKG-INFO
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1346 2020-11-22 19:48:50.000000 yamicache-0.6.0/README.rst
-drwxr-xr-x   0 timcfadd  (1000) timcfadd  (1000)        0 2020-11-22 20:03:38.320469 yamicache-0.6.0/docs/
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     6951 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/Makefile
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     8526 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/conf.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)       33 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/contributing.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)       28 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/history.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      284 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/index.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1123 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/installation.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     6707 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/make.bat
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)       27 2020-11-22 18:56:43.000000 yamicache-0.6.0/docs/readme.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     4844 2020-11-22 18:57:06.000000 yamicache-0.6.0/docs/usage.rst
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      117 2020-11-22 20:03:38.320469 yamicache-0.6.0/setup.cfg
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1167 2020-11-22 19:12:07.000000 yamicache-0.6.0/setup.py
-drwxr-xr-x   0 timcfadd  (1000) timcfadd  (1000)        0 2020-11-22 20:03:38.320469 yamicache-0.6.0/tests/
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)       67 2020-11-22 18:56:43.000000 yamicache-0.6.0/tests/__init__.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     4025 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_class.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      584 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_clear_deco.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      962 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_collide.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      638 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_default_args.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      286 2020-11-22 18:56:43.000000 yamicache-0.6.0/tests/test_exceptions.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     2342 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_gc.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      932 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_init.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1369 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_noclass.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     1504 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_serialization.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     3753 2020-11-22 19:13:27.000000 yamicache-0.6.0/tests/test_threading.py
-drwxr-xr-x   0 timcfadd  (1000) timcfadd  (1000)        0 2020-11-22 20:03:38.320469 yamicache-0.6.0/yamicache/
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      194 2020-11-22 19:13:31.000000 yamicache-0.6.0/yamicache/__init__.py
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)    15095 2020-11-22 19:13:31.000000 yamicache-0.6.0/yamicache/yamicache.py
-drwxr-xr-x   0 timcfadd  (1000) timcfadd  (1000)        0 2020-11-22 20:03:38.320469 yamicache-0.6.0/yamicache.egg-info/
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)     3580 2020-11-22 20:03:38.000000 yamicache-0.6.0/yamicache.egg-info/PKG-INFO
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)      678 2020-11-22 20:03:38.000000 yamicache-0.6.0/yamicache.egg-info/SOURCES.txt
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)        1 2020-11-22 20:03:38.000000 yamicache-0.6.0/yamicache.egg-info/dependency_links.txt
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)       10 2020-11-22 20:03:38.000000 yamicache-0.6.0/yamicache.egg-info/top_level.txt
--rw-r--r--   0 timcfadd  (1000) timcfadd  (1000)        1 2020-11-22 19:02:15.000000 yamicache-0.6.0/yamicache.egg-info/zip-safe
+-rw-r--r--   0        0        0     1087 2023-04-14 15:02:27.481066 yamicache-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1346 2023-04-14 15:02:27.481066 yamicache-0.7.0/README.rst
+-rw-r--r--   0        0        0     1004 2023-04-14 16:39:25.220538 yamicache-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-04-14 16:39:25.220538 yamicache-0.7.0/yamicache/__init__.py
+-rw-r--r--   0        0        0    15500 2023-04-14 16:35:34.602013 yamicache-0.7.0/yamicache/yamicache.py
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 yamicache-0.7.0/PKG-INFO
```

### Comparing `yamicache-0.6.0/LICENSE` & `yamicache-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yamicache-0.6.0/README.rst` & `yamicache-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `yamicache-0.6.0/yamicache/yamicache.py` & `yamicache-0.7.0/yamicache/yamicache.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,77 +4,31 @@
 yamicache : Yet another in-memory cache module ('yami' sounds better to me than
 'yaim')
 
 This module provides a simple in-memory interface for caching results from
 function calls.
 """
 
+import collections
+import contextlib
+import inspect
+
 # Imports #####################################################################
-from __future__ import print_function
 import json
+import pickle
 import time
-import inspect
-import contextlib
-import collections
-from hashlib import sha224
 from functools import wraps
+from hashlib import sha224
 from threading import Lock, Thread
-
-try:
-    import cPickle as pickle
-except ImportError:
-    import pickle
-
+from typing import Any, ItemsView, KeysView, Optional, ValuesView
 
 # Globals #####################################################################
 __all__ = ["Cache", "nocache", "override_timeout"]
 
 
-@contextlib.contextmanager
-def override_timeout(cache_obj, timeout):
-    cache_obj._override_timeout = timeout
-
-    try:
-        yield
-    finally:
-        # The value of ``None`` disable the override timeout mechanism
-        cache_obj._override_timeout = None
-
-
-@contextlib.contextmanager
-def nocache(cache_obj):
-    """
-    Use this context manager to temporarily disable all caching for an
-    object.
-
-    Example:
-
-        >>> from yamicache import Cache, nocache
-        >>> c = Cache()
-        >>> @c.cached
-        ... def test():
-        ...     return 4
-        ...
-        >>> with nocache(c):
-        ...     test()
-        ...
-        4
-        >>> print c.data_store
-        {}
-        >>>
-
-    """
-    cache_obj._cache = False
-
-    try:
-        yield
-    finally:
-        cache_obj._cache = True
-
-
 CachedItem = collections.namedtuple("CachedItem", "value timeout time_added")
 INIT_CACHE_VALUE = CachedItem("<value not cached yet>", None, None)
 
 
 class Cache(collections.abc.MutableMapping):
     """
     A class for caching and retreiving returns from function calls.
@@ -98,183 +52,183 @@
         *garbage collection*.  The default, ``None``, will disable the garbage
         collection thread.  This parameter is only valid if ``default_timeout``
         is > 0 (``ValueError`` is raised otherwise).
     """
 
     def __init__(
         self,
-        hashing=True,
-        key_join="|",
-        debug=False,
-        prefix=None,
-        quiet=False,
-        default_timeout=0,
-        gc_thread_wait=None,
+        hashing: bool = True,
+        key_join: str = "|",
+        debug: bool = False,
+        prefix: Optional[str] = None,
+        quiet: bool = False,
+        default_timeout: int = 0,
+        gc_thread_wait: bool = False,
     ):
         self._prefix = prefix or ""
         self._hashing = hashing
         self._key_join = key_join
         self._debug = debug
         self._quiet = quiet
         self._cache = True  # Allow for ``nocache``
-        self._data_store = {}
+        self._data_store: dict[Any, Any] = {}
         self._default_timeout = default_timeout
         self._gc_thread_wait = gc_thread_wait
         self._gc_thread = None
         self._do_gc_thread = False
         self._gc_lock = Lock()
-        self.counters = {}  # Only enabled with ``debug``
+        self.counters: dict[Any, int] = {}  # Only enabled with ``debug``
 
         # Force all calls to use this value instead of default, or what was
         # used during decorator creation.
-        self._override_timeout = None
+        self._override_timeout: Optional[int] = None
 
         if default_timeout and not isinstance(default_timeout, int):
             raise ValueError("Default timeout can only be `int`")
 
         if self._gc_thread_wait:
             self._do_gc_thread = True
             self._gc_thread = Thread(target=self._gc)
             self._gc_thread.daemon = True
             self._gc_thread.start()
 
     # Default stuff to override MutableMapping ABC ############################
-    def __len__(self):
+    def __len__(self) -> int:
         return len([x for x, y in self.items() if y is not INIT_CACHE_VALUE])
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any) -> Any:
         """Only return the item if it's not the INIT value"""
         with self._gc_lock:
             if (key not in self._data_store) or (
                 self._data_store[key] is INIT_CACHE_VALUE
             ):
                 raise KeyError(key)
             return self._data_store[key]
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: Any, value: Any) -> None:
         with self._gc_lock:
             self._data_store[key] = value
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: Any) -> None:
         with self._gc_lock:
             del self._data_store[key]
 
-    def __iter__(self):
+    def __iter__(self) -> Any:
         """
         Override ``iter()``.  This can make things slow, but it's the only
         way to prevent the underlying object from changing during iteration.
         """
         with self._gc_lock:
             for x in self._data_store.keys():
                 yield x
 
     # Override some of the *normal* methods to include the lock ###############
-    def clear(self):
+    def clear(self) -> None:
         """Clear the cache"""
         with self._gc_lock:
             self._data_store.clear()
             self.counters.clear()
 
-    def keys(self):
+    def keys(self) -> KeysView:
         """Return a list of keys in the cache"""
         with self._gc_lock:
             return self._data_store.keys()
 
-    def items(self):
+    def items(self) -> ItemsView:
         """Return all items in the cache as a list of ``tuple(key, value)``"""
         with self._gc_lock:
             return self._data_store.items()
 
-    def values(self):
+    def values(self) -> ValuesView:
         """Return a list of cached values"""
         with self._gc_lock:
             return self._data_store.values()
 
-    def pop(self, key):
+    def pop(self, key: Any, /) -> Any:  # type: ignore
         """Remove the cached value specified by ``key``"""
         with self._gc_lock:
             return self._data_store.pop(key)
 
-    def popitem(self):
+    def popitem(self) -> Any:
         """Remove a random item from the cache (only useful during testing)"""
         with self._gc_lock:
             return self._data_store.popitem()
 
     ###########################################################################
 
-    def _is_key_initialized(self, key):
+    def _is_key_initialized(self, key: str) -> bool:
         with self._gc_lock:
             return self._data_store.get(key) is INIT_CACHE_VALUE
 
-    def _from_timestamp(self, timestamp):
+    def _from_timestamp(self, timestamp: str) -> float:
         """Convert a timestamp string to an epoch value"""
+        print("_from_timestamp:", timestamp)
+        # Fri Apr 14 09:50:20 2023
         return time.mktime(time.strptime(timestamp))
 
-    def _to_timestamp(self, epoch=None):
+    def _to_timestamp(self, epoch: Optional[float] = None) -> str:
         """Convert an epoch value to a timestamp string"""
         if epoch:
             return time.asctime(time.localtime(epoch))
 
         return time.asctime()
 
-    def _debug_print(self, *args):
+    def _debug_print(self, *args) -> None:
         if self._debug:
             print(*args)
 
-    def dump(self):
+    def dump(self) -> str:
         """Dump the entire cache as a JSON string"""
         return json.dumps(self._data_store, indent=4, separators=(",", ": "))
 
-    def _calculate_key(self, func, cached_key=None, *args, **kwargs):
+    def _calculate_key(self, func, cached_key: str = "", *args, **kwargs) -> str:
         """
         Calculates the cache key based on the function, inputs, and object
         settings.
 
         :param code func: The function being cached
         :param str cached_key: The `keyed_cache`, if any
         :param *args: Any ``*args`` used to call the function
         :param *kwargs: Any ``*kwargs`` used to call the function
         """
         if cached_key:
             return cached_key
 
-        key = cached_key
-        if not key:
-            key = {}
-            # We need to grab the default arguments.  `inspect.getargspec()`
-            # returns the function argument names, and any defaults.  The
-            # defaults are always the last args.  For example:
-            # `args=['arg1', 'arg2'], defaults=(4,)` means that `arg2` has a
-            # default of 4.
-            spec = inspect.getfullargspec(func)
-
-            # Load the defaults first, since they may not be in the calling
-            # spec.
-            if spec.defaults:
-                key = dict(zip(spec.args[-len(spec.defaults) :], spec.defaults))
-
-            # Now load in the arguments.
-            key.update(kwargs)
-            key.update(dict(zip(func.__code__.co_varnames, args)))
-
-            # This next issue is that Python may re-order the keys when we go
-            # to repr them.  This will cause invalid cache misses.  We can fix
-            # this by recreating a dictionary with a 'known' algorithm.
-            key = repr(dict(sorted(key.items())))
+        # We need to grab the default arguments.  `inspect.getargspec()`
+        # returns the function argument names, and any defaults.  The
+        # defaults are always the last args.  For example:
+        # `args=['arg1', 'arg2'], defaults=(4,)` means that `arg2` has a
+        # default of 4.
+        spec = inspect.getfullargspec(func)
+
+        # Load the defaults first, since they may not be in the calling
+        # spec.
+        key: dict = {}
+        if spec.defaults:
+            key = dict(zip(spec.args[-len(spec.defaults) :], spec.defaults))
+
+        # Now load in the arguments.
+        key.update(kwargs)
+        key.update(dict(zip(func.__code__.co_varnames, args)))
+
+        # This next issue is that Python may re-order the keys when we go
+        # to repr them.  This will cause invalid cache misses.  We can fix
+        # this by recreating a dictionary with a 'known' algorithm.
+        repr_key = repr(dict(sorted(key.items())))
 
         return "{prefix}{name}{join}{formatted_key}".format(
             join=self._key_join,
             prefix=(self._prefix + self._key_join) if self._prefix else "",
             name=func.__name__,
-            formatted_key=sha224(str(key).encode("utf-8")).hexdigest()
+            formatted_key=sha224(repr_key.encode("utf-8")).hexdigest()
             if self._hashing
-            else str(key),
+            else repr_key,
         )
 
-    def _update_counter(self, key):
+    def _update_counter(self, key: str) -> None:
         """Keeps track of cache hits"""
         if not self._debug:
             return
 
         with self._gc_lock:
             if key in self.counters:
                 self.counters[key] += 1
@@ -290,15 +244,15 @@
         while self._do_gc_thread:
             if time.time() > tnext:
                 self.collect()
                 tnext = time.time() + self._gc_thread_wait
 
             time.sleep(1)
 
-    def collect(self, since=None):
+    def collect(self, since: Optional[float] = None) -> None:
         """
         Clear any item from the cache that has timed out.
         """
         remove_keys = []
         for key, item in self.items():
             if (
                 item.timeout and (time.time() > self._from_timestamp(item.timeout))
@@ -327,31 +281,31 @@
                 self.clear()
                 return function(*args, **kwargs)
 
             return wrapper
 
         return real_decorator
 
-    def cached(self, key=None, timeout=None):
+    def cached(self, key: str = "", timeout: Optional[int] = 0):
         """
         A decorator used to memoize the return of a function call.
         """
         if timeout and not isinstance(timeout, int):
             raise ValueError("timeout can only be `int`")
-        elif (key in self) or self._is_key_initialized(key):
+        elif key and (key in self) or self._is_key_initialized(key):
             # `key in self` will return False if the key either doesn't exist,
             # or it's set to the INIT value.  Therefore, we need to call
             # `_is_key_initialized()` to check that condition.
             raise ValueError("cache key '%s' already exists" % key)
         elif key:
             # Set the default value so we can check for collisions when the
             # next decorator is called.
             self[key] = INIT_CACHE_VALUE
 
-        def real_decorator(function, timeout=timeout):
+        def real_decorator(function, timeout: Optional[int] = timeout):
             function.__cached_timeout__ = timeout or self._default_timeout
 
             @wraps(function)
             def wrapper(*args, **kwargs):
                 # Check the timeout here, since this is the call and not the
                 # instantiation.
 
@@ -408,22 +362,64 @@
                 self[cache_key] = result
                 return result.value
 
             return wrapper
 
         return real_decorator
 
-    def serialize(self, filename):
+    def serialize(self, filename: str) -> None:
         """
         Serialize the cache to a filename.  This process uses ``pickle``; Do
         not use this function if you are caching something that is not
         picklable!
         """
         with open(filename, "wb") as fh:
             pickle.dump(self._data_store, fh, -1)
 
-    def deserialize(self, filename):
+    def deserialize(self, filename: str) -> None:
         """
         Read the serialized cache data from a file.
         """
         with open(filename, "rb") as fh:
             self._data_store = pickle.load(fh)
+
+
+@contextlib.contextmanager
+def override_timeout(cache_obj: Cache, timeout: int):
+    cache_obj._override_timeout = timeout
+
+    try:
+        yield
+    finally:
+        # The value of ``None`` disable the override timeout mechanism
+        cache_obj._override_timeout = None
+
+
+@contextlib.contextmanager
+def nocache(cache_obj: Cache):
+    """
+    Use this context manager to temporarily disable all caching for an
+    object.
+
+    Example:
+
+        >>> from yamicache import Cache, nocache
+        >>> c = Cache()
+        >>> @c.cached
+        ... def test():
+        ...     return 4
+        ...
+        >>> with nocache(c):
+        ...     test()
+        ...
+        4
+        >>> print c.data_store
+        {}
+        >>>
+
+    """
+    cache_obj._cache = False
+
+    try:
+        yield
+    finally:
+        cache_obj._cache = True
```

