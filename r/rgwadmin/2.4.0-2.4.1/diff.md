# Comparing `tmp/rgwadmin-2.4.0.tar.gz` & `tmp/rgwadmin-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgwadmin-2.4.0.tar", last modified: Mon Mar 13 20:44:02 2023, max compression
+gzip compressed data, was "rgwadmin-2.4.1.tar", last modified: Fri Apr 14 14:23:51 2023, max compression
```

## Comparing `rgwadmin-2.4.0.tar` & `rgwadmin-2.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.603584 rgwadmin-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    26443 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3359 2023-03-13 20:44:02.602584 rgwadmin-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.584583 rgwadmin-2.4.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.587583 rgwadmin-2.4.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.589583 rgwadmin-2.4.0/docs/source/apipages/
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/apipages/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/apipages/rgw.rst
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/apipages/user.rst
--rw-rw-rw-   0 root         (0) root         (0)     5460 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.590583 rgwadmin-2.4.0/docs/source/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/rgwadmin/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)    14356 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/docs/source/rgwadmin/user-guide.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.595584 rgwadmin-2.4.0/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21359 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/rgw.py
--rw-rw-rw-   0 root         (0) root         (0)     9589 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/rgwadmin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.599583 rgwadmin-2.4.0/rgwadmin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3359 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      695 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-13 20:44:02.000000 rgwadmin-2.4.0/rgwadmin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 20:44:02.603584 rgwadmin-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1444 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:44:02.601584 rgwadmin-2.4.0/test/
--rwxrwxrwx   0 root         (0) root         (0)     2683 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/test/test_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     6327 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/test/test_rgw.py
--rwxrwxrwx   0 root         (0) root         (0)     1461 2023-03-13 20:43:54.000000 rgwadmin-2.4.0/test/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.152035 rgwadmin-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    26443 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-04-14 14:23:51.151035 rgwadmin-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.133035 rgwadmin-2.4.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.135034 rgwadmin-2.4.1/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/api.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.138035 rgwadmin-2.4.1/docs/source/apipages/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/rgw.rst
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/user.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.139035 rgwadmin-2.4.1/docs/source/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/rgwadmin/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14356 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/rgwadmin/user-guide.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.144035 rgwadmin-2.4.1/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21420 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/rgw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9589 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.148035 rgwadmin-2.4.1/rgwadmin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 14:23:51.152035 rgwadmin-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.151035 rgwadmin-2.4.1/test/
+-rwxrwxrwx   0 root         (0) root         (0)     2683 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     6327 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_rgw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1461 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_user.py
```

### Comparing `rgwadmin-2.4.0/LICENSE` & `rgwadmin-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/PKG-INFO` & `rgwadmin-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.0/README.md` & `rgwadmin-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/docs/Makefile` & `rgwadmin-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/docs/make.bat` & `rgwadmin-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/docs/source/conf.py` & `rgwadmin-2.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/docs/source/rgwadmin/user-guide.rst` & `rgwadmin-2.4.1/docs/source/rgwadmin/user-guide.rst`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/rgwadmin/exceptions.py` & `rgwadmin-2.4.1/rgwadmin/exceptions.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/rgwadmin/rgw.py` & `rgwadmin-2.4.1/rgwadmin/rgw.py`

 * *Files 4% similar despite different names*

```diff
@@ -476,19 +476,21 @@
                             (self._admin, self._response, parameters))
 
     def unlink_bucket(self, bucket, uid):
         parameters = 'bucket=%s&uid=%s' % (bucket, uid)
         return self.request('post', '/%s/bucket?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
-    def link_bucket(self, bucket, bucket_id, uid):
-        # note that even though the Ceph docs say that bucket-id is optional
-        # the API call will fail (InvalidArgument) if it is omitted.
-        parameters = 'bucket=%s&bucket-id=%s&uid=%s' % \
-            (bucket, bucket_id, uid)
+    def link_bucket(self, bucket, uid, bucket_id=None, new_bucket_name=None):
+        parameters = 'bucket=%s' % bucket
+        parameters += '&uid=%s' % uid
+        if bucket_id is not None:
+            parameters += '&bucket-id=%s' % bucket_id
+        if new_bucket_name is not None:
+            parameters += '&new-bucket-name=%s' % new_bucket_name
         return self.request('put', '/%s/bucket?format=%s&%s' %
                             (self._admin, self._response, parameters))
 
     def remove_object(self, bucket, object_name):
         parameters = 'bucket=%s&object=%s' % (bucket, object_name)
         return self.request('delete', '/%s/bucket?object&format=%s&%s' %
                             (self._admin, self._response, parameters))
```

### Comparing `rgwadmin-2.4.0/rgwadmin/user.py` & `rgwadmin-2.4.1/rgwadmin/user.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/rgwadmin/utils.py` & `rgwadmin-2.4.1/rgwadmin/utils.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/rgwadmin.egg-info/PKG-INFO` & `rgwadmin-2.4.1/rgwadmin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.0/rgwadmin.egg-info/SOURCES.txt` & `rgwadmin-2.4.1/rgwadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/setup.py` & `rgwadmin-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/test/test_metadata.py` & `rgwadmin-2.4.1/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/test/test_rgw.py` & `rgwadmin-2.4.1/test/test_rgw.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.0/test/test_user.py` & `rgwadmin-2.4.1/test/test_user.py`

 * *Files identical despite different names*

