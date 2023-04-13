# Comparing `tmp/deterrers-api-0.1.tar.gz` & `tmp/deterrers-api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-api-0.1.tar", last modified: Thu Apr 13 20:00:53 2023, max compression
+gzip compressed data, was "deterrers-api-0.2.tar", last modified: Thu Apr 13 22:27:39 2023, max compression
```

## Comparing `deterrers-api-0.1.tar` & `deterrers-api-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 20:00:53.365966 deterrers-api-0.1/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrers-api-0.1/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrers-api-0.1/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-13 20:00:53.365966 deterrers-api-0.1/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-04-13 20:00:47.000000 deterrers-api-0.1/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 20:00:53.365966 deterrers-api-0.1/deterrers_api.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-13 20:00:53.000000 deterrers-api-0.1/deterrers_api.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-04-13 20:00:53.000000 deterrers-api-0.1/deterrers_api.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 20:00:53.000000 deterrers-api-0.1/deterrers_api.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 20:00:53.000000 deterrers-api-0.1/deterrers_api.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 20:00:53.000000 deterrers-api-0.1/deterrers_api.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 20:00:53.365966 deterrers-api-0.1/deterrersapi/
--rw-r--r--   0 lars      (1000) lars      (1000)     5271 2023-04-13 16:50:35.000000 deterrers-api-0.1/deterrersapi/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrers-api-0.1/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 20:00:53.365966 deterrers-api-0.1/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      688 2023-04-13 19:59:17.000000 deterrers-api-0.1/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 22:27:39.955280 deterrers-api-0.2/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrers-api-0.2/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrers-api-0.2/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-13 22:27:39.955280 deterrers-api-0.2/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-04-13 20:00:47.000000 deterrers-api-0.2/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 22:27:39.954280 deterrers-api-0.2/deterrers_api.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-13 22:27:39.000000 deterrers-api-0.2/deterrers_api.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-04-13 22:27:39.000000 deterrers-api-0.2/deterrers_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 22:27:39.000000 deterrers-api-0.2/deterrers_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 22:27:39.000000 deterrers-api-0.2/deterrers_api.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 22:27:39.000000 deterrers-api-0.2/deterrers_api.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 22:27:39.954280 deterrers-api-0.2/deterrersapi/
+-rw-r--r--   0 lars      (1000) lars      (1000)     5220 2023-04-13 21:02:35.000000 deterrers-api-0.2/deterrersapi/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrers-api-0.2/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 22:27:39.955280 deterrers-api-0.2/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      688 2023-04-13 22:26:27.000000 deterrers-api-0.2/setup.py
```

### Comparing `deterrers-api-0.1/LICENSE` & `deterrers-api-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.1/PKG-INFO` & `deterrers-api-0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.1
+Version: 0.2
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-api-0.1/README.md` & `deterrers-api-0.2/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.1/deterrers_api.egg-info/PKG-INFO` & `deterrers-api-0.2/deterrers_api.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.1
+Version: 0.2
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-api-0.1/deterrersapi/__init__.py` & `deterrers-api-0.2/deterrersapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 
         :param ipv4: IPv4 address
         :type ipv4: str
         :param admins: List of admins for address
         :type admins: list[str]
         '''
         data = {'ipv4_addr': ipv4,
-                'service_profile': 'Multipurpose',
                 'admin_ids': admins}
         return self.__post('host/', data)
 
     def delete(self, ipv4: str) -> None:
         '''Delete IP from DETERRERS.
 
         :param ipv4: IPv4 address to delete
```

### Comparing `deterrers-api-0.1/setup.py` & `deterrers-api-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-api',
-    version='0.1',
+    version='0.2',
     description='Python API client for DETERRERS',
     url='https://github.com/virtUOS/deterrers-api',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrersapi'],
     license_files=('LICENSE'),
```

