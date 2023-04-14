# Comparing `tmp/yourtools-0.4.6.tar.gz` & `tmp/yourtools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.4.6.tar", last modified: Fri Apr 14 09:32:26 2023, max compression
+gzip compressed data, was "dist/yourtools-0.4.7.tar", last modified: Fri Apr 14 09:34:13 2023, max compression
```

## Comparing `yourtools-0.4.6.tar` & `yourtools-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:32:26.000000 yourtools-0.4.6/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.4.6/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.4.6/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.4.6/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.4.6/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.4.6/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      649 2023-04-13 09:13:14.000000 yourtools-0.4.6/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3954 2023-04-14 09:31:12.000000 yourtools-0.4.6/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.4.6/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 09:32:26.000000 yourtools-0.4.6/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.4.6/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.4.6/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.4.6/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 09:32:26.000000 yourtools-0.4.6/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 09:32:26.000000 yourtools-0.4.6/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:34:13.000000 yourtools-0.4.7/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.4.7/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.4.7/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.4.7/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.4.7/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.4.7/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      649 2023-04-13 09:13:14.000000 yourtools-0.4.7/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     4059 2023-04-14 09:33:58.000000 yourtools-0.4.7/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.4.7/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 09:34:13.000000 yourtools-0.4.7/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.4.7/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.4.7/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.4.7/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 09:34:13.000000 yourtools-0.4.7/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 09:34:13.000000 yourtools-0.4.7/setup.cfg
```

### Comparing `yourtools-0.4.6/yourtools/db/dbutils.py` & `yourtools-0.4.7/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/yourtools/db/hive.py` & `yourtools-0.4.7/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/yourtools/db/mysql.py` & `yourtools-0.4.7/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/yourtools/Azkaban.py` & `yourtools-0.4.7/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/yourtools/Time.py` & `yourtools-0.4.7/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/yourtools/WeChat.py` & `yourtools-0.4.7/yourtools/WeChat.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,17 @@
             m = MultipartEncoder(
                 fields={filename: (filename, open(filepath + filename, 'rb'), 'text/plain')},
             )
             response = requests.post(url=post_file_url, data=m, headers={'Content-Type': m.content_type})
             if response.status_code == 200:
                 result = json.loads(response.text)
                 return result['media_id']
+            else:
+                print("HTTP Error:", response.status_code)
+                return None
         except Exception as err:
             raise Exception("upload media error", err)
 
     def get_media(self, media_id):
         """
         获取临时素材
         :param media_id:
```

### Comparing `yourtools-0.4.6/yourtools.egg-info/PKG-INFO` & `yourtools-0.4.7/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.4.6/README.md` & `yourtools-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/setup.py` & `yourtools-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.6/PKG-INFO` & `yourtools-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

