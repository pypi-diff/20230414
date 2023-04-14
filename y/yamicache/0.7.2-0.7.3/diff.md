# Comparing `tmp/yamicache-0.7.2.tar.gz` & `tmp/yamicache-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamicache-0.7.2.tar", max compression
+gzip compressed data, was "yamicache-0.7.3.tar", max compression
```

## Comparing `yamicache-0.7.2.tar` & `yamicache-0.7.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1087 2023-04-14 15:02:27.481066 yamicache-0.7.2/LICENSE
--rw-r--r--   0        0        0     1346 2023-04-14 15:02:27.481066 yamicache-0.7.2/README.rst
--rw-r--r--   0        0        0     1004 2023-04-14 17:39:00.325549 yamicache-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      194 2023-04-14 17:39:00.325549 yamicache-0.7.2/yamicache/__init__.py
--rw-r--r--   0        0        0       96 2023-04-14 17:46:05.790228 yamicache-0.7.2/yamicache/__init__.pyi
--rw-r--r--   0        0        0        0 2023-04-14 17:46:05.790228 yamicache-0.7.2/yamicache/py.typed
--rw-r--r--   0        0        0    15500 2023-04-14 16:35:34.602013 yamicache-0.7.2/yamicache/yamicache.py
--rw-r--r--   0        0        0     1353 2023-04-14 17:46:05.790228 yamicache-0.7.2/yamicache/yamicache.pyi
--rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 yamicache-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-04-14 15:02:27.481066 yamicache-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1346 2023-04-14 15:02:27.481066 yamicache-0.7.3/README.rst
+-rw-r--r--   0        0        0     1004 2023-04-14 18:08:56.435087 yamicache-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-04-14 18:08:56.435087 yamicache-0.7.3/yamicache/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-14 18:10:03.883430 yamicache-0.7.3/yamicache/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 18:10:03.883430 yamicache-0.7.3/yamicache/py.typed
+-rw-r--r--   0        0        0    15420 2023-04-14 18:06:07.435097 yamicache-0.7.3/yamicache/yamicache.py
+-rw-r--r--   0        0        0     1353 2023-04-14 18:10:03.883430 yamicache-0.7.3/yamicache/yamicache.pyi
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 yamicache-0.7.3/PKG-INFO
```

### Comparing `yamicache-0.7.2/LICENSE` & `yamicache-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yamicache-0.7.2/README.rst` & `yamicache-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `yamicache-0.7.2/pyproject.toml` & `yamicache-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamicache"
-version = "0.7.2"
+version = "0.7.3"
 description = "Yet another in-memory caching package"
 authors = ["Timothy McFadden <mtik00@users.noreply.github.com>"]
 license = "MIT"
 classifiers=[
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yamicache-0.7.2/yamicache/yamicache.py` & `yamicache-0.7.3/yamicache/yamicache.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,14 @@
 
     def _is_key_initialized(self, key: str) -> bool:
         with self._gc_lock:
             return self._data_store.get(key) is INIT_CACHE_VALUE
 
     def _from_timestamp(self, timestamp: str) -> float:
         """Convert a timestamp string to an epoch value"""
-        print("_from_timestamp:", timestamp)
-        # Fri Apr 14 09:50:20 2023
         return time.mktime(time.strptime(timestamp))
 
     def _to_timestamp(self, epoch: Optional[float] = None) -> str:
         """Convert an epoch value to a timestamp string"""
         if epoch:
             return time.asctime(time.localtime(epoch))
```

### Comparing `yamicache-0.7.2/yamicache/yamicache.pyi` & `yamicache-0.7.3/yamicache/yamicache.pyi`

 * *Files identical despite different names*

### Comparing `yamicache-0.7.2/PKG-INFO` & `yamicache-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamicache
-Version: 0.7.2
+Version: 0.7.3
 Summary: Yet another in-memory caching package
 Home-page: https://github.com/mtik00/yamicache
 License: MIT
 Author: Timothy McFadden
 Author-email: mtik00@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

