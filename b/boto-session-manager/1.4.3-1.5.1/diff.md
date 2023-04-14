# Comparing `tmp/boto_session_manager-1.4.3.tar.gz` & `tmp/boto_session_manager-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto_session_manager-1.4.3.tar", last modified: Fri Apr 14 06:58:44 2023, max compression
+gzip compressed data, was "boto_session_manager-1.5.1.tar", last modified: Fri Apr 14 07:06:37 2023, max compression
```

## Comparing `boto_session_manager-1.4.3.tar` & `boto_session_manager-1.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.342922 boto_session_manager-1.4.3/
--rw-r--r--   0 sanhehu    (505) staff       (20)      607 2023-03-24 14:27:36.000000 boto_session_manager-1.4.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      389 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/CONTRIBUTING.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)    11387 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/LICENSE
--rw-r--r--   0 sanhehu    (505) staff       (20)      318 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)       88 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/NOTICE
--rw-r--r--   0 sanhehu    (505) staff       (20)     8123 2023-04-14 06:58:44.342780 boto_session_manager-1.4.3/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     6824 2023-03-24 14:12:52.000000 boto_session_manager-1.4.3/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.340792 boto_session_manager-1.4.3/boto_session_manager/
--rw-r--r--   0 sanhehu    (505) staff       (20)      804 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/boto_session_manager/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/boto_session_manager/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)   113267 2023-03-24 15:02:29.000000 boto_session_manager-1.4.3/boto_session_manager/clients.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.341881 boto_session_manager-1.4.3/boto_session_manager/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/boto_session_manager/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       79 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/exc.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    15107 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/manager.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2435 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/sentinel.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    11542 2023-03-24 15:02:29.000000 boto_session_manager-1.4.3/boto_session_manager/services.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.341740 boto_session_manager-1.4.3/boto_session_manager.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     8123 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      720 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      190 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       21 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     4206 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      338 2023-03-24 13:06:34.000000 boto_session_manager-1.4.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      196 2023-03-24 14:00:50.000000 boto_session_manager-1.4.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        6 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-04-14 06:58:44.342967 boto_session_manager-1.4.3/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     5447 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/setup.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.342301 boto_session_manager-1.4.3/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      309 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/tests/test_import.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5265 2023-03-24 14:12:09.000000 boto_session_manager-1.4.3/tests/test_manager.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 07:06:37.089873 boto_session_manager-1.5.1/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      607 2023-03-24 14:27:36.000000 boto_session_manager-1.5.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      389 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11387 2023-04-14 04:41:12.000000 boto_session_manager-1.5.1/LICENSE
+-rw-r--r--   0 sanhehu    (505) staff       (20)      318 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (505) staff       (20)       88 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/NOTICE
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8904 2023-04-14 07:06:37.089638 boto_session_manager-1.5.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)     7605 2023-04-14 07:06:08.000000 boto_session_manager-1.5.1/README.rst
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 07:06:37.084323 boto_session_manager-1.5.1/boto_session_manager/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      804 2023-04-14 04:41:12.000000 boto_session_manager-1.5.1/boto_session_manager/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-04-14 06:59:18.000000 boto_session_manager-1.5.1/boto_session_manager/_version.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)   113267 2023-03-24 15:02:29.000000 boto_session_manager-1.5.1/boto_session_manager/clients.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 07:06:37.088121 boto_session_manager-1.5.1/boto_session_manager/docs/
+-rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/boto_session_manager/docs/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       79 2023-04-14 06:58:28.000000 boto_session_manager-1.5.1/boto_session_manager/exc.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    15107 2023-04-14 06:58:28.000000 boto_session_manager-1.5.1/boto_session_manager/manager.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2435 2023-04-14 06:58:28.000000 boto_session_manager-1.5.1/boto_session_manager/sentinel.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11542 2023-03-24 15:02:29.000000 boto_session_manager-1.5.1/boto_session_manager/services.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 07:06:37.087252 boto_session_manager-1.5.1/boto_session_manager.egg-info/
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8904 2023-04-14 07:06:37.000000 boto_session_manager-1.5.1/boto_session_manager.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)      720 2023-04-14 07:06:37.000000 boto_session_manager-1.5.1/boto_session_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-04-14 07:06:37.000000 boto_session_manager-1.5.1/boto_session_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      190 2023-04-14 07:06:37.000000 boto_session_manager-1.5.1/boto_session_manager.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       21 2023-04-14 07:06:37.000000 boto_session_manager-1.5.1/boto_session_manager.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)     4206 2023-04-14 06:58:28.000000 boto_session_manager-1.5.1/release-history.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      338 2023-03-24 13:06:34.000000 boto_session_manager-1.5.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      196 2023-03-24 14:00:50.000000 boto_session_manager-1.5.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)        6 2023-04-14 04:41:12.000000 boto_session_manager-1.5.1/requirements.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-04-14 07:06:37.089933 boto_session_manager-1.5.1/setup.cfg
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5447 2023-04-14 04:41:12.000000 boto_session_manager-1.5.1/setup.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 07:06:37.089019 boto_session_manager-1.5.1/tests/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      309 2023-03-21 20:18:02.000000 boto_session_manager-1.5.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5265 2023-03-24 14:12:09.000000 boto_session_manager-1.5.1/tests/test_manager.py
```

### Comparing `boto_session_manager-1.4.3/AUTHORS.rst` & `boto_session_manager-1.5.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/CONTRIBUTING.rst` & `boto_session_manager-1.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/LICENSE` & `boto_session_manager-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/PKG-INFO` & `boto_session_manager-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: boto_session_manager
-Version: 1.4.3
+Version: 1.5.1
 Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto-session-manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.3#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
 License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
@@ -134,20 +134,39 @@
 
 **Assume Role**
 
 Create another boto session manager based on an assumed IAM role. Allow you to check if it is expired and maybe renew later.
 
 .. code-block:: python
 
-    bsm_assumed = bsm.assume_role("arn:aws:iam::669508176277:role/sanhe-assume-role-for-iam-test")
+    bsm_assumed = bsm.assume_role("arn:aws:iam::111122223333:role/your-assume-role-name")
     sts_client = bsm_assumed.get_client(AwsServiceEnum.sts)
     print(sts_client.get_caller_identity())
 
     print(bsm_assumed.is_expired())
 
+From ``1.5.1``, it adds support for auto-refreshable assumed role (Beta). Note that it is using ``AssumeRoleCredentialFetcher`` and ``DeferredRefreshableCredentials`` from botocore, which is not public API officially supported by botocore. This API may be unstable.
+
+.. code-block:: python
+
+    bsm_assumed = bsm.assume_role(
+        "arn:aws:iam::111122223333:role/your-assume-role-name",
+        duration_seconds=900,
+        auto_refresh=True,
+    )
+
+    # even though the duration seconds is only 15 minutes,
+    # but it can keep running for 1 hour.
+    tick = 60
+    sleep = 60
+    for i in range(tick):
+        time.sleep(sleep)
+        print("elapsed {} seconds".format((i + 1) * sleep))
+        print("Account id = {}".format(bsm_new.sts_client.get_caller_identity()["Account"]))
+
 **AWS CLI context manager**
 
 You explicitly defined a boto session manager that is not the same as the default one used by your AWS CLI. The ``boto_session_manager.BotoSesManager.awscli()`` context manager can temporarily set your default AWS CLI credential as the same as the one you defined, and automatically revert it back.
 
 .. code-block:: python
 
     # explicitly define a boto session manager
```

### Comparing `boto_session_manager-1.4.3/README.rst` & `boto_session_manager-1.5.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -100,20 +100,39 @@
 
 **Assume Role**
 
 Create another boto session manager based on an assumed IAM role. Allow you to check if it is expired and maybe renew later.
 
 .. code-block:: python
 
-    bsm_assumed = bsm.assume_role("arn:aws:iam::669508176277:role/sanhe-assume-role-for-iam-test")
+    bsm_assumed = bsm.assume_role("arn:aws:iam::111122223333:role/your-assume-role-name")
     sts_client = bsm_assumed.get_client(AwsServiceEnum.sts)
     print(sts_client.get_caller_identity())
 
     print(bsm_assumed.is_expired())
 
+From ``1.5.1``, it adds support for auto-refreshable assumed role (Beta). Note that it is using ``AssumeRoleCredentialFetcher`` and ``DeferredRefreshableCredentials`` from botocore, which is not public API officially supported by botocore. This API may be unstable.
+
+.. code-block:: python
+
+    bsm_assumed = bsm.assume_role(
+        "arn:aws:iam::111122223333:role/your-assume-role-name",
+        duration_seconds=900,
+        auto_refresh=True,
+    )
+
+    # even though the duration seconds is only 15 minutes,
+    # but it can keep running for 1 hour.
+    tick = 60
+    sleep = 60
+    for i in range(tick):
+        time.sleep(sleep)
+        print("elapsed {} seconds".format((i + 1) * sleep))
+        print("Account id = {}".format(bsm_new.sts_client.get_caller_identity()["Account"]))
+
 **AWS CLI context manager**
 
 You explicitly defined a boto session manager that is not the same as the default one used by your AWS CLI. The ``boto_session_manager.BotoSesManager.awscli()`` context manager can temporarily set your default AWS CLI credential as the same as the one you defined, and automatically revert it back.
 
 .. code-block:: python
 
     # explicitly define a boto session manager
```

### Comparing `boto_session_manager-1.4.3/boto_session_manager/__init__.py` & `boto_session_manager-1.5.1/boto_session_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/boto_session_manager/clients.py` & `boto_session_manager-1.5.1/boto_session_manager/clients.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/boto_session_manager/manager.py` & `boto_session_manager-1.5.1/boto_session_manager/manager.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/boto_session_manager/sentinel.py` & `boto_session_manager-1.5.1/boto_session_manager/sentinel.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/boto_session_manager/services.py` & `boto_session_manager-1.5.1/boto_session_manager/services.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/boto_session_manager.egg-info/PKG-INFO` & `boto_session_manager-1.5.1/boto_session_manager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: boto-session-manager
-Version: 1.4.3
+Version: 1.5.1
 Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto-session-manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.3#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
 License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
@@ -134,20 +134,39 @@
 
 **Assume Role**
 
 Create another boto session manager based on an assumed IAM role. Allow you to check if it is expired and maybe renew later.
 
 .. code-block:: python
 
-    bsm_assumed = bsm.assume_role("arn:aws:iam::669508176277:role/sanhe-assume-role-for-iam-test")
+    bsm_assumed = bsm.assume_role("arn:aws:iam::111122223333:role/your-assume-role-name")
     sts_client = bsm_assumed.get_client(AwsServiceEnum.sts)
     print(sts_client.get_caller_identity())
 
     print(bsm_assumed.is_expired())
 
+From ``1.5.1``, it adds support for auto-refreshable assumed role (Beta). Note that it is using ``AssumeRoleCredentialFetcher`` and ``DeferredRefreshableCredentials`` from botocore, which is not public API officially supported by botocore. This API may be unstable.
+
+.. code-block:: python
+
+    bsm_assumed = bsm.assume_role(
+        "arn:aws:iam::111122223333:role/your-assume-role-name",
+        duration_seconds=900,
+        auto_refresh=True,
+    )
+
+    # even though the duration seconds is only 15 minutes,
+    # but it can keep running for 1 hour.
+    tick = 60
+    sleep = 60
+    for i in range(tick):
+        time.sleep(sleep)
+        print("elapsed {} seconds".format((i + 1) * sleep))
+        print("Account id = {}".format(bsm_new.sts_client.get_caller_identity()["Account"]))
+
 **AWS CLI context manager**
 
 You explicitly defined a boto session manager that is not the same as the default one used by your AWS CLI. The ``boto_session_manager.BotoSesManager.awscli()`` context manager can temporarily set your default AWS CLI credential as the same as the one you defined, and automatically revert it back.
 
 .. code-block:: python
 
     # explicitly define a boto session manager
```

### Comparing `boto_session_manager-1.4.3/boto_session_manager.egg-info/SOURCES.txt` & `boto_session_manager-1.5.1/boto_session_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/release-history.rst` & `boto_session_manager-1.5.1/release-history.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/requirements-doc.txt` & `boto_session_manager-1.5.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/setup.py` & `boto_session_manager-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.3/tests/test_manager.py` & `boto_session_manager-1.5.1/tests/test_manager.py`

 * *Files identical despite different names*

