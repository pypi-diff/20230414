# Comparing `tmp/python-mongodm-0.0.8.tar.gz` & `tmp/python-mongodm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mongodm-0.0.8.tar", last modified: Sun Oct 23 12:13:18 2022, max compression
+gzip compressed data, was "python-mongodm-0.0.9.tar", last modified: Fri Oct 28 21:14:35 2022, max compression
```

## Comparing `python-mongodm-0.0.8.tar` & `python-mongodm-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-23 12:13:18.931881 python-mongodm-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4831 2022-10-23 12:13:18.930881 python-mongodm-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4316 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-23 12:13:18.931881 python-mongodm-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1373 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-23 12:13:18.926880 python-mongodm-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-23 12:13:18.929880 python-mongodm-0.0.8/src/mongodm/
--rw-rw-rw-   0 root         (0) root         (0)     9200 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/src/mongodm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/src/mongodm/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2022-10-23 12:13:16.000000 python-mongodm-0.0.8/src/mongodm/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-23 12:13:18.930881 python-mongodm-0.0.8/src/python_mongodm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4831 2022-10-23 12:13:18.000000 python-mongodm-0.0.8/src/python_mongodm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      302 2022-10-23 12:13:18.000000 python-mongodm-0.0.8/src/python_mongodm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-23 12:13:18.000000 python-mongodm-0.0.8/src/python_mongodm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      221 2022-10-23 12:13:18.000000 python-mongodm-0.0.8/src/python_mongodm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-10-23 12:13:18.000000 python-mongodm-0.0.8/src/python_mongodm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-28 21:14:35.083684 python-mongodm-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4831 2022-10-28 21:14:35.083684 python-mongodm-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-28 21:14:35.083684 python-mongodm-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-28 21:14:35.079684 python-mongodm-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-28 21:14:35.081684 python-mongodm-0.0.9/src/mongodm/
+-rw-rw-rw-   0 root         (0) root         (0)     9188 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/src/mongodm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/src/mongodm/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2022-10-28 21:14:33.000000 python-mongodm-0.0.9/src/mongodm/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-28 21:14:35.083684 python-mongodm-0.0.9/src/python_mongodm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4831 2022-10-28 21:14:35.000000 python-mongodm-0.0.9/src/python_mongodm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      302 2022-10-28 21:14:35.000000 python-mongodm-0.0.9/src/python_mongodm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-28 21:14:35.000000 python-mongodm-0.0.9/src/python_mongodm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2022-10-28 21:14:35.000000 python-mongodm-0.0.9/src/python_mongodm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-10-28 21:14:35.000000 python-mongodm-0.0.9/src/python_mongodm.egg-info/top_level.txt
```

### Comparing `python-mongodm-0.0.8/LICENSE` & `python-mongodm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mongodm-0.0.8/PKG-INFO` & `python-mongodm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mongodm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous Python ODM for MongoDB based on Motor
 Author: Ferréol Jeannot-Lorente
 Project-URL: Homepage, https://github.com/tritons-io/MongODM
 Project-URL: Bug Tracker, https://github.com/tritons-io/MongODM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-mongodm-0.0.8/README.md` & `python-mongodm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python-mongodm-0.0.8/setup.py` & `python-mongodm-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `python-mongodm-0.0.8/src/mongodm/__init__.py` & `python-mongodm-0.0.9/src/mongodm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,22 +197,22 @@
         return self
 
     @classmethod
     async def get_all(
         cls,
         page: int = 1,
         per_page: int = 20,
-        selector_z: dict = None,
+        selector: dict = None,
         **kwargs,
     ) -> list:  # -> List[Self]
-        if selector_z is None:
-            selector_z = kwargs
-        selector_z = cls.replace_str_with_object_id(selector_z)
+        if selector is None:
+            selector = kwargs
+        selector = cls.replace_str_with_object_id(selector)
         items = await config['database_connection'][config['database_name']][cls.__collection_name__]\
-            .find(cls._get_fetch_filter(selector_z))\
+            .find(cls._get_fetch_filter(selector))\
             .skip((page - 1) * per_page)\
             .limit(per_page)\
             .to_list(length=None)
 
         return [cls(**item).after_get_many_hook() for item in items]
 
     def set_attributes(self, **kwargs):
```

### Comparing `python-mongodm-0.0.8/src/mongodm/types.py` & `python-mongodm-0.0.9/src/mongodm/types.py`

 * *Files identical despite different names*

### Comparing `python-mongodm-0.0.8/src/python_mongodm.egg-info/PKG-INFO` & `python-mongodm-0.0.9/src/python_mongodm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mongodm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous Python ODM for MongoDB based on Motor
 Author: Ferréol Jeannot-Lorente
 Project-URL: Homepage, https://github.com/tritons-io/MongODM
 Project-URL: Bug Tracker, https://github.com/tritons-io/MongODM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

