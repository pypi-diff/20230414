# Comparing `tmp/bsb-hdf5-0.7.2.tar.gz` & `tmp/bsb-hdf5-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb-hdf5-0.7.2.tar", last modified: Mon Feb 27 09:13:12 2023, max compression
+gzip compressed data, was "bsb-hdf5-0.7.3.tar", last modified: Fri Apr 14 13:54:42 2023, max compression
```

## Comparing `bsb-hdf5-0.7.2.tar` & `bsb-hdf5-0.7.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-02-27 09:13:12.457303 bsb-hdf5-0.7.2/
--rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.2/LICENSE
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-02-27 09:13:12.455705 bsb-hdf5-0.7.2/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.2/README.md
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-02-27 09:13:12.333303 bsb-hdf5-0.7.2/bsb_hdf5/
--rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-02-27 09:01:40.000000 bsb-hdf5-0.7.2/bsb_hdf5/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.2/bsb_hdf5/chunks.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    20846 2023-01-27 13:40:35.000000 bsb-hdf5-0.7.2/bsb_hdf5/connectivity_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4734 2023-01-27 13:41:06.000000 bsb-hdf5-0.7.2/bsb_hdf5/file_store.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     7412 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.2/bsb_hdf5/morphology_repository.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    15175 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.2/bsb_hdf5/placement_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4996 2023-01-19 16:34:25.000000 bsb-hdf5-0.7.2/bsb_hdf5/resource.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-02-27 09:13:12.392627 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/SOURCES.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/dependency_links.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/entry_points.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/requires.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-02-27 09:13:12.000000 bsb-hdf5-0.7.2/bsb_hdf5.egg-info/top_level.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.2/pyproject.toml
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-02-27 09:13:12.457303 bsb-hdf5-0.7.2/setup.cfg
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-02-03 09:58:50.000000 bsb-hdf5-0.7.2/setup.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-02-27 09:13:12.432303 bsb-hdf5-0.7.2/test/
--rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.7.2/test/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.7.2/test/test_cs.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.2/test/test_interface.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     5780 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.2/test/test_mr.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-02-27 09:13:12.443305 bsb-hdf5-0.7.2/test/test_setup/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.2/test/test_setup/__init__.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 13:54:42.213310 bsb-hdf5-0.7.3/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.3/LICENSE
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-04-14 13:54:42.211310 bsb-hdf5-0.7.3/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.3/README.md
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 13:54:42.032283 bsb-hdf5-0.7.3/bsb_hdf5/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-04-14 13:48:25.000000 bsb-hdf5-0.7.3/bsb_hdf5/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.3/bsb_hdf5/chunks.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    20846 2023-01-27 13:40:35.000000 bsb-hdf5-0.7.3/bsb_hdf5/connectivity_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4818 2023-04-14 13:25:49.000000 bsb-hdf5-0.7.3/bsb_hdf5/file_store.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     7412 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.3/bsb_hdf5/morphology_repository.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    15580 2023-04-14 13:45:55.000000 bsb-hdf5-0.7.3/bsb_hdf5/placement_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4996 2023-01-19 16:34:25.000000 bsb-hdf5-0.7.3/bsb_hdf5/resource.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 13:54:42.088251 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/SOURCES.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/dependency_links.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/entry_points.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/requires.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-04-14 13:54:41.000000 bsb-hdf5-0.7.3/bsb_hdf5.egg-info/top_level.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.3/pyproject.toml
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-04-14 13:54:42.213310 bsb-hdf5-0.7.3/setup.cfg
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-02-03 09:58:50.000000 bsb-hdf5-0.7.3/setup.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 13:54:42.185691 bsb-hdf5-0.7.3/test/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.7.3/test/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.7.3/test/test_cs.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.3/test/test_interface.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     5780 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.3/test/test_mr.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 13:54:42.200308 bsb-hdf5-0.7.3/test/test_setup/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.3/test/test_setup/__init__.py
```

### Comparing `bsb-hdf5-0.7.2/LICENSE` & `bsb-hdf5-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/PKG-INFO` & `bsb-hdf5-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.7.2
+Version: 0.7.3
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/__init__.py` & `bsb-hdf5-0.7.3/bsb_hdf5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 import json
 import h5py
 import os
 import shutil
 import shortuuid
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 __all__ = [
     "PlacementSet",
     "ConnectivitySet",
     "FileStore",
     "MorphologyRepository",
     "HDF5Engine",
     "StorageNode",
```

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/chunks.py` & `bsb-hdf5-0.7.3/bsb_hdf5/chunks.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/connectivity_set.py` & `bsb-hdf5-0.7.3/bsb_hdf5/connectivity_set.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/file_store.py` & `bsb-hdf5-0.7.3/bsb_hdf5/file_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,26 @@
     def __bool__(self):
         return True
 
     def all(self):
         with self._engine._read():
             with self._engine._handle("r") as root:
                 store = root[self._path]
-                return {id: json.loads(f.attrs["meta"]) for id, f in store.items()}
+                return {
+                    id: json.loads(f.attrs.get("meta", "{}")) for id, f in store.items()
+                }
 
     def load(self, id):
         with self._engine._read():
             with self._engine._handle("r") as root:
                 ds = root[f"{self._path}/{id}"]
                 data = ds[()]
-                if encoding := ds.attrs.get("encoding"):
+                if encoding := ds.attrs.get("encoding", None):
                     data = data.decode(encoding)
-                return data, json.loads(ds.attrs["meta"])
+                return data, json.loads(ds.attrs.get("meta", "{}"))
 
     def remove(self, id):
         with self._engine._write():
             with self._engine._handle("a") as root:
                 del root[f"{self._path}/{id}"]
 
     def store(self, content, meta=None, id=None, encoding=None, overwrite=False):
@@ -120,13 +122,13 @@
         with self._engine._read():
             with self._engine._handle("r") as root:
                 return root[self._path][id].attrs["mtime"]
 
     def get_encoding(self, id):
         with self._engine._read():
             with self._engine._handle("r") as root:
-                return root[self._path][id].attrs["encoding"]
+                return root[self._path][id].attrs.get("encoding", None)
 
     def get_meta(self, id):
         with self._engine._read():
             with self._engine._handle("r") as root:
-                return json.loads(root[self._path][id].attrs["meta"])
+                return json.loads(root[self._path][id].attrs.get("meta", "{}"))
```

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/morphology_repository.py` & `bsb-hdf5-0.7.3/bsb_hdf5/morphology_repository.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/placement_set.py` & `bsb-hdf5-0.7.3/bsb_hdf5/placement_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,47 +155,60 @@
     @handles_handles("r")
     def load_morphologies(self, handle=HANDLED, allow_empty=False):
         """
         Load the cell morphologies.
 
         :raises: DatasetNotFoundError when the morphology data is not found.
         """
-        data = self._morphology_chunks.load(handle=handle)
+        reader = self._morphology_chunks.get_chunk_reader(handle, True)
         loaders = self._get_morphology_loaders(handle=handle)
+        data = []
+        for chunk in self.get_loaded_chunks():
+            path = self.get_chunk_path(chunk)
+            try:
+                _map = handle[path].attrs["morphology_loaders"]
+            except KeyError:
+                continue
+            block = np.vectorize(list(loaders.keys()).index)(_map[reader(chunk)])
+            if len(block):
+                data.append(block)
         if not allow_empty and (len(data) == 0 and (len(self) != 0 or len(loaders) == 0)):
             raise DatasetNotFoundError("No morphology data available.")
+        data = np.concatenate(data)
         if self._labels:
             mask = self.get_label_mask(self._labels, handle=handle)
             data = data[mask]
         return MorphologySet(
-            loaders,
+            list(loaders.values()),
             data,
             labels=self._morphology_labels,
         )
 
     @handles_handles("r")
     def load_additional(self, key=None, handle=HANDLED):
         if key is None:
             return self._additional_chunks.load_all()
         else:
             return self._additional_chunks.load(key)
 
     @handles_handles("r")
     def _get_morphology_loaders(self, handle=HANDLED):
-        loaded_names = set()
-        stor_mor = []
+        stor_mor = {}
         for chunk in self.get_loaded_chunks():
             path = self.get_chunk_path(chunk)
             try:
                 _map = handle[path].attrs["morphology_loaders"]
             except KeyError:
                 continue
-            cmlist = self._engine.morphologies.select(_MapSelector(ps=self, names=_map))
-            stor_mor.extend(m for m in cmlist if m.name not in loaded_names)
-            loaded_names.update(m.name for m in cmlist)
+            stor_mor.update(
+                (m.name, m)
+                for m in self._engine.morphologies.select(
+                    _MapSelector(ps=self, names=_map)
+                )
+            )
         return stor_mor
 
     @handles_handles("a")
     def _set_morphology_loaders(self, map, handle=HANDLED):
         for chunk in self.get_loaded_chunks():
             path = self.get_chunk_path(chunk)
             handle[path].attrs["morphology_loaders"] = map
```

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5/resource.py` & `bsb-hdf5-0.7.3/bsb_hdf5/resource.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/bsb_hdf5.egg-info/PKG-INFO` & `bsb-hdf5-0.7.3/bsb_hdf5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.7.2
+Version: 0.7.3
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.7.2/setup.py` & `bsb-hdf5-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/test/test_cs.py` & `bsb-hdf5-0.7.3/test/test_cs.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/test/test_interface.py` & `bsb-hdf5-0.7.3/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/test/test_mr.py` & `bsb-hdf5-0.7.3/test/test_mr.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.2/test/test_setup/__init__.py` & `bsb-hdf5-0.7.3/test/test_setup/__init__.py`

 * *Files identical despite different names*

