# Comparing `tmp/xpip-python-0.2.tar.gz` & `tmp/xpip-python-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpip-python-0.2.tar", last modified: Thu Apr 13 18:36:07 2023, max compression
+gzip compressed data, was "dist/xpip-python-0.3.tar", last modified: Fri Apr 14 15:30:31 2023, max compression
```

## Comparing `xpip-python-0.2.tar` & `xpip-python-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 18:36:07.000000 xpip-python-0.2/
--rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-13 18:36:07.000000 xpip-python-0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 14:48:57.000000 xpip-python-0.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)     1072 2023-04-13 18:36:07.000000 xpip-python-0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      103 2023-04-13 14:48:57.000000 xpip-python-0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 18:36:07.000000 xpip-python-0.2/xpip/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 18:36:07.000000 xpip-python-0.2/xpip/config/
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-04-13 18:14:18.000000 xpip-python-0.2/xpip/config/mirrors.toml
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 14:48:57.000000 xpip-python-0.2/xpip/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      921 2023-04-13 14:48:57.000000 xpip-python-0.2/xpip/xpip_command.py
--rwxrwxrwx   0 root         (0) root         (0)      362 2023-04-13 17:14:24.000000 xpip-python-0.2/xpip/xpip_config.py
--rwxrwxrwx   0 root         (0) root         (0)     3183 2023-04-13 18:31:12.000000 xpip-python-0.2/xpip/xpip_mirror.py
--rwxrwxrwx   0 root         (0) root         (0)      744 2023-04-13 18:27:59.000000 xpip-python-0.2/xpip/xpip_util.py
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 18:31:53.000000 xpip-python-0.2/xpip/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 18:36:07.000000 xpip-python-0.2/xpip_python.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 18:36:06.000000 xpip-python-0.2/xpip_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       85 2023-04-13 18:36:06.000000 xpip-python-0.2/xpip_python.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-13 18:36:06.000000 xpip-python-0.2/xpip_python.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 18:36:06.000000 xpip-python-0.2/xpip_python.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      415 2023-04-13 18:36:07.000000 xpip-python-0.2/xpip_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-13 18:36:06.000000 xpip-python-0.2/xpip_python.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 14:56:57.000000 xpip-python-0.2/xpip_python.egg-info/zip-safe
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 15:30:31.000000 xpip-python-0.3/
+-rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-14 15:30:31.000000 xpip-python-0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 14:48:57.000000 xpip-python-0.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1072 2023-04-14 15:30:31.000000 xpip-python-0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      103 2023-04-13 14:48:57.000000 xpip-python-0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 15:30:31.000000 xpip-python-0.3/xpip/config/
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-04-14 14:36:11.000000 xpip-python-0.3/xpip/config/mirrors.toml
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 14:48:57.000000 xpip-python-0.3/xpip/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      921 2023-04-13 14:48:57.000000 xpip-python-0.3/xpip/xpip_command.py
+-rwxrwxrwx   0 root         (0) root         (0)      362 2023-04-13 17:14:24.000000 xpip-python-0.3/xpip/xpip_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     4804 2023-04-14 15:27:56.000000 xpip-python-0.3/xpip/xpip_mirror.py
+-rwxrwxrwx   0 root         (0) root         (0)      757 2023-04-13 18:49:34.000000 xpip-python-0.3/xpip/xpip_util.py
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-14 15:30:04.000000 xpip-python-0.3/xpip/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 15:30:31.000000 xpip-python-0.3/xpip_python.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       85 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)      415 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-14 15:30:30.000000 xpip-python-0.3/xpip_python.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 14:56:57.000000 xpip-python-0.3/xpip_python.egg-info/zip-safe
```

### Comparing `xpip-python-0.2/PKG-INFO` & `xpip-python-0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpip-python
-Version: 0.2
+Version: 0.3
 Summary: Python package. Build. Install.
 Home-page: https://github.com/zoumingzhe/xpip-python
 Author: mingzhe
 Author-email: zoumingzhe@qq.com
 License: MIT
 Project-URL: Source Code, https://github.com/zoumingzhe/xpip-python
 Project-URL: Bug Tracker, https://github.com/zoumingzhe/xpip-python/issues
```

### Comparing `xpip-python-0.2/setup.cfg` & `xpip-python-0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `xpip-python-0.2/xpip/xpip_command.py` & `xpip-python-0.3/xpip/xpip_command.py`

 * *Files identical despite different names*

### Comparing `xpip-python-0.2/xpip/xpip_util.py` & `xpip-python-0.3/xpip/xpip_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,11 @@
         return end_time - start_time if result == 0 else None
 
 
 def get_domain_location(domain: str) -> str:
     try:
         ip = socket.gethostbyname(domain)
         obj = IPWhois(ip, timeout=1)
-        results = obj.lookup_rdap()
+        results = obj.lookup_rdap(retry_count=0)
         return results['asn_country_code']
     except Exception:
         return 'UNKOWN'
```

### Comparing `xpip-python-0.2/xpip_python.egg-info/PKG-INFO` & `xpip-python-0.3/xpip_python.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpip-python
-Version: 0.2
+Version: 0.3
 Summary: Python package. Build. Install.
 Home-page: https://github.com/zoumingzhe/xpip-python
 Author: mingzhe
 Author-email: zoumingzhe@qq.com
 License: MIT
 Project-URL: Source Code, https://github.com/zoumingzhe/xpip-python
 Project-URL: Bug Tracker, https://github.com/zoumingzhe/xpip-python/issues
```

