# Comparing `tmp/dask_awkward-2023.4.0.tar.gz` & `tmp/dask_awkward-2023.4.1.tar.gz`

## Comparing `dask_awkward-2023.4.0.tar` & `dask_awkward-2023.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61123 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    28744 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61222 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    28745 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.1/PKG-INFO
```

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.4.1/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/typing.py` & `dask_awkward-2023.4.1/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/utils.py` & `dask_awkward-2023.4.1/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.4.1/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/core.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,14 +976,16 @@
         If there are no __dunder__ parameters in the function call then the function
         is wrapped in map_partitions automatically.
         """
         if hasattr(self._meta, method_name):
             themethod = getattr(self._meta, method_name)
             thesig = inspect.signature(themethod)
             if "_dask_array_" in thesig.parameters:
+                if "_dask_array_" not in kwargs:
+                    kwargs["_dask_array_"] = self
                 return themethod(*args, **kwargs)
             return self.map_partitions(
                 _BehaviorMethodFn(method_name, **kwargs),
                 *args,
                 label=hyphenize(method_name),
             )
```

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -888,15 +888,15 @@
         self.where = where
         self.highlevel = highlevel
         self.behavior = behavior
 
     def __call__(self, base: ak.Array, what: ak.Array) -> ak.Array:
         # TODO: remove backend handling when touch is handled automatically
         if ak.backend(what) == "typetracer":
-            what.layout._touch_data(recursive=True)
+            what.layout._touch_data(recursive=False)
         return ak.with_field(
             base,
             what,
             where=self.where,
             highlevel=self.highlevel,
             behavior=self.behavior,
         )
```

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.4.1/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/.gitignore` & `dask_awkward-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/LICENSE` & `dask_awkward-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/README.md` & `dask_awkward-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.0/pyproject.toml` & `dask_awkward-2023.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "awkward >=2.1.2",
+  "awkward >=2.1.3",
   "dask >=2022.02.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
```

### Comparing `dask_awkward-2023.4.0/PKG-INFO` & `dask_awkward-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.1.2
+Requires-Dist: awkward>=2.1.3
 Requires-Dist: dask>=2022.02.1
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
```

