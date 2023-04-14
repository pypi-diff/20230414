# Comparing `tmp/orbax-checkpoint-0.2.0.tar.gz` & `tmp/orbax-checkpoint-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-checkpoint-0.2.0.tar", last modified: Tue Apr 11 01:58:27 2023, max compression
+gzip compressed data, was "orbax-checkpoint-0.2.1.tar", last modified: Fri Apr 14 17:20:24 2023, max compression
```

## Comparing `orbax-checkpoint-0.2.0.tar` & `orbax-checkpoint-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/LICENSE
--rw-r--r--   0        0        0      696 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/README.md
--rw-r--r--   0        0        0     2564 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4742 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    33132 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7146 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0    44930 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    21582 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     9406 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13488 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    21621 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    19878 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7444 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/LICENSE
+-rw-r--r--   0        0        0      696 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/README.md
+-rw-r--r--   0        0        0     2564 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4742 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    33132 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7146 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0    44930 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    21752 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5234 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0     9406 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    13488 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    21621 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    19878 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7444 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.1/PKG-INFO
```

### Comparing `orbax-checkpoint-0.2.0/LICENSE` & `orbax-checkpoint-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/README.md` & `orbax-checkpoint-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/__init__.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/abstract_checkpointer.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/aggregate_handlers.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/array_checkpoint_handler.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpoint_handler.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpointer.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_handler.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_manager.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils_test.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpointer.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/conftest.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/future.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/lazy_utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/msgpack_utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax-checkpoint-0.2.1/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,20 +503,24 @@
     param_infos = _get_param_infos_from_structure(directory, structure)
 
     if transform_fn is not None and transforms is not None:
       raise ValueError('Cannot provide both `transforms` and `transform_fn`.')
     if transform_fn is not None:
       structure, param_infos = transform_fn(item, structure, param_infos)
 
-    concurrent_bytes = self._concurrent_gb * 10**9
-    # Construction must take place here so that it is within the same async
-    # method, to prevent errors resulting from different event loops, and
-    # cannot be created below this level because there must be a single object
-    # for the entire restore call.
-    byte_limiter = serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
+    async def _create_byte_limiter():
+      # Wrap creation in async function to avoid issues on python<=3.9.
+      concurrent_bytes = self._concurrent_gb * 10**9
+      # Construction must take place here so that it is within the same async
+      # method, to prevent errors resulting from different event loops, and
+      # cannot be created below this level because there must be a single object
+      # for the entire restore call.
+      return serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
+
+    byte_limiter = asyncio.run(_create_byte_limiter())
     param_infos = jax.tree_util.tree_map(
         functools.partial(dataclasses.replace, byte_limiter=byte_limiter),
         param_infos,
     )
     lazy_restored_item = jax.tree_util.tree_map(
         self._maybe_deserialize,
         param_infos,
```

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/test_utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils_test.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/type_handlers.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/type_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/utils.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/orbax/checkpoint/utils_test.py` & `orbax-checkpoint-0.2.1/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/pyproject.toml` & `orbax-checkpoint-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.0/PKG-INFO` & `orbax-checkpoint-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.0
+Version: 0.2.1
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

