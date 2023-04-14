# Comparing `tmp/boto_session_manager-1.4.2.tar.gz` & `tmp/boto_session_manager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto_session_manager-1.4.2.tar", last modified: Fri Mar 24 15:05:07 2023, max compression
+gzip compressed data, was "boto_session_manager-1.4.3.tar", last modified: Fri Apr 14 06:58:44 2023, max compression
```

## Comparing `boto_session_manager-1.4.2.tar` & `boto_session_manager-1.4.3.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-24 15:05:07.541946 boto_session_manager-1.4.2/
--rw-r--r--   0 sanhehu    (505) staff       (20)      607 2023-03-24 14:27:36.000000 boto_session_manager-1.4.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      389 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      947 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/LICENSE
--rw-r--r--   0 sanhehu    (505) staff       (20)      318 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)       88 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/NOTICE
--rw-r--r--   0 sanhehu    (505) staff       (20)     8040 2023-03-24 15:05:07.541806 boto_session_manager-1.4.2/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     6824 2023-03-24 14:12:52.000000 boto_session_manager-1.4.2/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-24 15:05:07.539884 boto_session_manager-1.4.2/boto_session_manager/
--rw-r--r--   0 sanhehu    (505) staff       (20)      733 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/boto_session_manager/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-03-24 15:03:54.000000 boto_session_manager-1.4.2/boto_session_manager/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)   113267 2023-03-24 15:02:29.000000 boto_session_manager-1.4.2/boto_session_manager/clients.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-24 15:05:07.540724 boto_session_manager-1.4.2/boto_session_manager/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/boto_session_manager/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    12275 2023-03-24 03:08:16.000000 boto_session_manager-1.4.2/boto_session_manager/manager.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    11542 2023-03-24 15:02:29.000000 boto_session_manager-1.4.2/boto_session_manager/services.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-24 15:05:07.540568 boto_session_manager-1.4.2/boto_session_manager.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     8040 2023-03-24 15:05:07.000000 boto_session_manager-1.4.2/boto_session_manager.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      659 2023-03-24 15:05:07.000000 boto_session_manager-1.4.2/boto_session_manager.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-03-24 15:05:07.000000 boto_session_manager-1.4.2/boto_session_manager.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      184 2023-03-24 15:05:07.000000 boto_session_manager-1.4.2/boto_session_manager.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       21 2023-03-24 15:05:07.000000 boto_session_manager-1.4.2/boto_session_manager.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     3622 2023-03-24 15:04:34.000000 boto_session_manager-1.4.2/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      338 2023-03-24 13:06:34.000000 boto_session_manager-1.4.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      196 2023-03-24 14:00:50.000000 boto_session_manager-1.4.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        0 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-03-24 15:05:07.541994 boto_session_manager-1.4.2/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     5435 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/setup.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-24 15:05:07.541281 boto_session_manager-1.4.2/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      309 2023-03-21 20:18:02.000000 boto_session_manager-1.4.2/tests/test_import.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5265 2023-03-24 14:12:09.000000 boto_session_manager-1.4.2/tests/test_manager.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.342922 boto_session_manager-1.4.3/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      607 2023-03-24 14:27:36.000000 boto_session_manager-1.4.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      389 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11387 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/LICENSE
+-rw-r--r--   0 sanhehu    (505) staff       (20)      318 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (505) staff       (20)       88 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/NOTICE
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8123 2023-04-14 06:58:44.342780 boto_session_manager-1.4.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)     6824 2023-03-24 14:12:52.000000 boto_session_manager-1.4.3/README.rst
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.340792 boto_session_manager-1.4.3/boto_session_manager/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      804 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/boto_session_manager/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/boto_session_manager/_version.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)   113267 2023-03-24 15:02:29.000000 boto_session_manager-1.4.3/boto_session_manager/clients.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.341881 boto_session_manager-1.4.3/boto_session_manager/docs/
+-rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/boto_session_manager/docs/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       79 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/exc.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    15107 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/manager.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2435 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/boto_session_manager/sentinel.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11542 2023-03-24 15:02:29.000000 boto_session_manager-1.4.3/boto_session_manager/services.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.341740 boto_session_manager-1.4.3/boto_session_manager.egg-info/
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8123 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)      720 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      190 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       21 2023-04-14 06:58:44.000000 boto_session_manager-1.4.3/boto_session_manager.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)     4206 2023-04-14 06:58:28.000000 boto_session_manager-1.4.3/release-history.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      338 2023-03-24 13:06:34.000000 boto_session_manager-1.4.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      196 2023-03-24 14:00:50.000000 boto_session_manager-1.4.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)        6 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/requirements.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-04-14 06:58:44.342967 boto_session_manager-1.4.3/setup.cfg
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5447 2023-04-14 04:41:12.000000 boto_session_manager-1.4.3/setup.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-14 06:58:44.342301 boto_session_manager-1.4.3/tests/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      309 2023-03-21 20:18:02.000000 boto_session_manager-1.4.3/tests/test_import.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5265 2023-03-24 14:12:09.000000 boto_session_manager-1.4.3/tests/test_manager.py
```

### Comparing `boto_session_manager-1.4.2/AUTHORS.rst` & `boto_session_manager-1.4.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/CONTRIBUTING.rst` & `boto_session_manager-1.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/PKG-INFO` & `boto_session_manager-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: boto_session_manager
-Version: 1.4.2
-Summary: Python AWS SDK boto3 library enhancement
+Version: 1.4.3
+Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto-session-manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
-License: MIT
+License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `boto_session_manager-1.4.2/README.rst` & `boto_session_manager-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/boto_session_manager/__init__.py` & `boto_session_manager-1.4.3/boto_session_manager/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     from .manager import BotoSesManager
     from .services import AwsServiceEnum
 except ImportError:  # pragma: no cover
     pass
 except:  # pragma: no cover
     raise
 
-__short_description__ = "Python AWS SDK boto3 library enhancement"
-__license__ = "MIT"
+__short_description__ = "Provides an alternative, or maybe a more user friendly way to use the native boto3 API."
+__license__ = "Apache License, Version 2.0"
 __author__ = "Sanhe Hu"
 __author_email__ = "husanhe@gmail.com"
 __maintainer__ = "Sanhe Hu"
 __maintainer_email__ = "sanhehu@amazon.com"
 __github_username__ = "aws-samples"
```

### Comparing `boto_session_manager-1.4.2/boto_session_manager/clients.py` & `boto_session_manager-1.4.3/boto_session_manager/clients.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/boto_session_manager/manager.py` & `boto_session_manager-1.4.3/boto_session_manager/manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,20 +13,30 @@
 try:
     import boto3
     import boto3.session
     import botocore.session
 except ImportError as e:  # pragma: no cover
     print("You probably need to install 'boto3' first.")
 
+try:
+    from botocore.credentials import (
+        AssumeRoleCredentialFetcher,
+        DeferredRefreshableCredentials,
+    )
+except ImportError as e: # pragma: no cover
+    print("The auto refreshable assume role session would not work.")
+
 if T.TYPE_CHECKING:  # pragma: no cover
     from botocore.client import BaseClient
     from boto3.resources.base import ServiceResource
 
 from .services import AwsServiceEnum
 from .clients import ClientMixin
+from .sentinel import NOTHING, resolve_kwargs
+from .exc import NoBotocoreCredentialError
 
 
 class BotoSesManager(ClientMixin):
     """
     Boto3 session and client manager that use cache to create low level client.
 
     .. note::
@@ -41,101 +51,103 @@
 
         add ``default_client_kwargs`` arguments that set default keyword
         arguments for ``boto3.session.Session.client`` method.
     """
 
     def __init__(
         self,
-        aws_access_key_id: str = None,
-        aws_secret_access_key: str = None,
-        aws_session_token: str = None,
-        region_name: str = None,
-        botocore_session: T.Optional["botocore.session.Session"] = None,
-        profile_name: str = None,
-        default_client_kwargs: dict = None,
-        expiration_time: datetime = None,
+        aws_access_key_id: T.Optional[str] = NOTHING,
+        aws_secret_access_key: T.Optional[str] = NOTHING,
+        aws_session_token: T.Optional[str] = NOTHING,
+        region_name: T.Optional[str] = NOTHING,
+        botocore_session: T.Optional["botocore.session.Session"] = NOTHING,
+        profile_name: str = NOTHING,
+        default_client_kwargs: dict = NOTHING,
+        expiration_time: datetime = NOTHING,
     ):
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.region_name = region_name
-        if botocore_session is not None:  # pragma: no cover
+        if botocore_session is not NOTHING:  # pragma: no cover
             if not isinstance(botocore_session, botocore.session.Session):
                 raise TypeError
-        self.botocore_session: "botocore.session.Session" = botocore_session
+        self.botocore_session: T.Optional["botocore.session.Session"] = botocore_session
         self.profile_name = profile_name
         self.expiration_time: datetime
-        if expiration_time is None:
+        if expiration_time is NOTHING:
             self.expiration_time = datetime.utcnow().replace(
                 tzinfo=timezone.utc
             ) + timedelta(days=365)
         else:
             self.expiration_time = expiration_time
-        if default_client_kwargs is None:
+        if default_client_kwargs is NOTHING:
             default_client_kwargs = dict()
         self.default_client_kwargs = default_client_kwargs
 
-        self._boto_ses_cache: T.Optional["boto3.session.Session"] = None
+        self._boto_ses_cache: T.Optional["boto3.session.Session"] = NOTHING
         self._client_cache: T.Dict[str, "BaseClient"] = dict()
         self._resource_cache: T.Dict[str, "ServiceResource"] = dict()
-        self._aws_account_id_cache: T.Optional[str] = None
-        self._aws_region_cache: T.Optional[str] = None
+        self._aws_account_id_cache: T.Optional[str] = NOTHING
+        self._aws_region_cache: T.Optional[str] = NOTHING
 
     @property
     def boto_ses(self) -> "boto3.session.Session":
         """
         Get boto3 session from metadata.
 
         .. versionadded:: 1.0.2
         """
-        if self._boto_ses_cache is None:
+        if self._boto_ses_cache is NOTHING:
             self._boto_ses_cache = boto3.session.Session(
-                aws_access_key_id=self.aws_access_key_id,
-                aws_secret_access_key=self.aws_secret_access_key,
-                aws_session_token=self.aws_session_token,
-                region_name=self.region_name,
-                botocore_session=self.botocore_session,
-                profile_name=self.profile_name,
+                **resolve_kwargs(
+                    aws_access_key_id=self.aws_access_key_id,
+                    aws_secret_access_key=self.aws_secret_access_key,
+                    aws_session_token=self.aws_session_token,
+                    region_name=self.region_name,
+                    botocore_session=self.botocore_session,
+                    profile_name=self.profile_name,
+                )
             )
         return self._boto_ses_cache
 
     @property
     def aws_account_id(self) -> str:
         """
-        Get current aws account id of the boto session
+        Get current aws account id of the boto session.
 
         .. versionadded:: 1.0.1
         """
-        if self._aws_account_id_cache is None:
+        if self._aws_account_id_cache is NOTHING:
             sts_client = self.get_client(AwsServiceEnum.STS)
             self._aws_account_id_cache = sts_client.get_caller_identity()["Account"]
         return self._aws_account_id_cache
 
     @property
     def aws_region(self) -> str:
         """
-        Get current aws region of the boto session
+        Get current aws region of the boto session.
 
         .. versionadded:: 0.0.1
         """
-        if self._aws_region_cache is None:
+        if self._aws_region_cache is NOTHING:
             self._aws_region_cache = self.boto_ses.region_name
         return self._aws_region_cache
 
     def get_client(
         self,
         service_name: str,
-        region_name: str = None,
-        api_version: str = None,
+        region_name: str = NOTHING,
+        api_version: str = NOTHING,
         use_ssl: bool = True,
-        verify: T.Union[bool, str] = None,
-        endpoint_url: str = None,
-        aws_access_key_id: str = None,
-        aws_secret_access_key: str = None,
-        aws_session_token: str = None,
+        verify: T.Union[bool, str] = NOTHING,
+        endpoint_url: str = NOTHING,
+        aws_access_key_id: str = NOTHING,
+        aws_secret_access_key: str = NOTHING,
+        aws_session_token: str = NOTHING,
         config=None,
     ) -> "BaseClient":
         """
         Get aws boto client using cache.
 
         .. versionadded:: 0.0.1
 
@@ -143,124 +155,167 @@
 
             add additional keyword arguments pass to
             ``boto3.session.Session.client()`` method.
         """
         try:
             return self._client_cache[service_name]
         except KeyError:
-            client_kwargs = dict(
+            client_kwargs = resolve_kwargs(
                 region_name=region_name,
                 api_version=api_version,
                 use_ssl=use_ssl,
                 verify=verify,
                 endpoint_url=endpoint_url,
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 config=config,
             )
-            client_kwargs = {k: v for k, v in client_kwargs.items() if v is not None}
             kwargs = dict(self.default_client_kwargs)
             if self.default_client_kwargs:  # pragma: no cover
                 kwargs.update(client_kwargs)
             client = self.boto_ses.client(service_name, **kwargs)
             self._client_cache[service_name] = client
             return client
 
     def get_resource(
         self,
         service_name: str,
-        region_name: str = None,
-        api_version: str = None,
+        region_name: str = NOTHING,
+        api_version: str = NOTHING,
         use_ssl: bool = True,
-        verify: T.Union[bool, str] = None,
-        endpoint_url: str = None,
-        aws_access_key_id: str = None,
-        aws_secret_access_key: str = None,
-        aws_session_token: str = None,
-        config=None,
+        verify: T.Union[bool, str] = NOTHING,
+        endpoint_url: str = NOTHING,
+        aws_access_key_id: str = NOTHING,
+        aws_secret_access_key: str = NOTHING,
+        aws_session_token: str = NOTHING,
+        config=NOTHING,
     ) -> "ServiceResource":
         """
         Get aws boto service resource using cache
 
         .. versionadded:: 0.0.2
 
         .. versionchanged:: 0.0.3
 
             add additional keyword arguments pass to
             ``boto3.session.Session.resource()`` method.
         """
         try:
             return self._resource_cache[service_name]
         except KeyError:
-            resource_kwargs = dict(
+            resource_kwargs = resolve_kwargs(
                 region_name=region_name,
                 api_version=api_version,
                 use_ssl=use_ssl,
                 verify=verify,
                 endpoint_url=endpoint_url,
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 config=config,
             )
-            resource_kwargs = {
-                k: v for k, v in resource_kwargs.items() if v is not None
-            }
             kwargs = dict(self.default_client_kwargs)
             if self.default_client_kwargs:
                 kwargs.update(resource_kwargs)
             resource = self.boto_ses.resource(service_name, **kwargs)
             self._resource_cache[service_name] = resource
             return resource
 
     def assume_role(
         self,
         role_arn: str,
-        role_session_name: str = None,
+        role_session_name: str = NOTHING,
         duration_seconds: int = 3600,
-        tags: list = None,
-        transitive_tag_keys: list = None,
-        external_id: str = None,
-        mfa_serial_number: str = None,
-        mfa_token: str = None,
-        source_identity: str = None,
+        tags: T.Optional[T.List[T.Dict[str, str]]] = NOTHING,
+        transitive_tag_keys: T.Optional[T.List[str]] = NOTHING,
+        external_id: str = NOTHING,
+        mfa_serial_number: str = NOTHING,
+        mfa_token: str = NOTHING,
+        source_identity: str = NOTHING,
+        auto_refresh: bool = False,
     ) -> "BotoSesManager":
         """
         Assume an IAM role, create another :class`BotoSessionManager` and return.
 
+        :param auto_refresh: if True, the assumed role will be refreshed automatically.
+
         .. versionadded:: 0.0.1
+
+        .. versionchanged:: 1.5.1
+
+            add ``auto_refresh`` argument. note that it is using
+            ``AssumeRoleCredentialFetcher`` and ``DeferredRefreshableCredentials``
+            from botocore, which is not public API officially supported by botocore.
         """
-        if role_session_name is None:
+        if role_session_name is NOTHING:
             role_session_name = uuid.uuid4().hex
-        kwargs = {
-            k: v
-            for k, v in dict(
+
+        # this branch cannot be tested regularly
+        # it is tested in a separate integration test environment.
+        if auto_refresh: # pragma: no cover
+            botocore_session = self.boto_ses._session
+            credentials = botocore_session.get_credentials()
+            # the get_credentials() method can return None
+            # raise error explicitly
+            if not credentials:
+                raise NoBotocoreCredentialError
+
+            credential_fetcher = AssumeRoleCredentialFetcher(
+                client_creator=botocore_session.create_client,
+                source_credentials=credentials,
+                role_arn=role_arn,
+                extra_args=resolve_kwargs(
+                    RoleSessionName=role_session_name,
+                    DurationSeconds=duration_seconds,
+                    Tags=tags,
+                    TransitiveTagKeys=transitive_tag_keys,
+                    external_id=external_id,
+                    SerialNumber=mfa_serial_number,
+                    TokenCode=mfa_token,
+                    SourceIdentity=source_identity,
+                ),
+            )
+
+            assumed_role_credentials = DeferredRefreshableCredentials(
+                refresh_using=credential_fetcher.fetch_credentials,
+                method="assume-role",
+            )
+            assumed_role_botocore_session: "botocore.session.Session" = botocore.session.get_session()
+            assumed_role_botocore_session._credentials = assumed_role_credentials
+            return BotoSesManager(
+                botocore_session=assumed_role_botocore_session,
+                # ensure that the new boto session manager with assumed role
+                # is using the same AWS region as this one
+                region_name=self.aws_region,
+                expiration_time=datetime(2099, 12, 31, 23, 59, 59, tzinfo=timezone.utc),
+                default_client_kwargs=self.default_client_kwargs,
+            )
+        else:
+            assume_role_kwargs = resolve_kwargs(
                 RoleArn=role_arn,
                 RoleSessionName=role_session_name,
                 DurationSeconds=duration_seconds,
                 Tags=tags,
                 TransitiveTagKeys=transitive_tag_keys,
                 external_id=external_id,
                 SerialNumber=mfa_serial_number,
                 TokenCode=mfa_token,
                 SourceIdentity=source_identity,
-            ).items()
-            if v is not None
-        }
-        sts_client = self.get_client(AwsServiceEnum.STS)
-        res = sts_client.assume_role(**kwargs)
-        expiration_time = res["Credentials"]["Expiration"]
-        bsm = self.__class__(
-            aws_access_key_id=res["Credentials"]["AccessKeyId"],
-            aws_secret_access_key=res["Credentials"]["SecretAccessKey"],
-            aws_session_token=res["Credentials"]["SessionToken"],
-            expiration_time=expiration_time,
-            default_client_kwargs=self.default_client_kwargs,
-        )
+            )
+            sts_client = self.get_client(AwsServiceEnum.STS)
+            res = sts_client.assume_role(**assume_role_kwargs)
+            expiration_time = res["Credentials"]["Expiration"]
+            bsm = self.__class__(
+                aws_access_key_id=res["Credentials"]["AccessKeyId"],
+                aws_secret_access_key=res["Credentials"]["SecretAccessKey"],
+                aws_session_token=res["Credentials"]["SessionToken"],
+                expiration_time=expiration_time,
+                default_client_kwargs=self.default_client_kwargs,
+            )
         return bsm
 
     def is_expired(self, delta: int = 0) -> bool:
         """
         Check if this boto session is expired.
 
         .. versionadded:: 0.0.1
@@ -269,16 +324,16 @@
             datetime.utcnow().replace(tzinfo=timezone.utc) + timedelta(seconds=delta)
         ) >= self.expiration_time
 
     @contextlib.contextmanager
     def awscli(
         self,
         duration_seconds: int = 900,
-        serial_number: T.Optional[str] = None,
-        token_code: T.Optional[str] = None,
+        serial_number: T.Optional[str] = NOTHING,
+        token_code: T.Optional[str] = NOTHING,
     ) -> "BotoSesManager":
         """
         Temporarily set up environment variable to pass the boto session
         credential to AWS CLI.
 
         Example::
 
@@ -308,29 +363,29 @@
             if env_name in os.environ:  # pragma: no cover
                 env_var[env_name] = os.environ[env_name]
             else:
                 env_var[env_name] = None
 
         # set environment variable for aws cli
         if (
-            (self.aws_access_key_id is not None)
-            and (self.aws_secret_access_key is not None)
-            and (self.aws_access_key_id is not None)
+            (self.aws_access_key_id is not NOTHING)
+            and (self.aws_secret_access_key is not NOTHING)
+            and (self.aws_access_key_id is not NOTHING)
         ):
             os.environ["AWS_ACCESS_KEY_ID"] = self.aws_access_key_id
             os.environ["AWS_SECRET_ACCESS_KEY"] = self.aws_secret_access_key
             os.environ["AWS_SESSION_TOKEN"] = self.aws_session_token
             os.environ["AWS_REGION"] = self.aws_region
         else:
             kwargs = dict(
                 DurationSeconds=duration_seconds,
             )
-            if serial_number is not None:  # pragma: no cover
+            if serial_number is not NOTHING:  # pragma: no cover
                 kwargs["SerialNumber"] = serial_number
-            if token_code is not None:  # pragma: no cover
+            if token_code is not NOTHING:  # pragma: no cover
                 kwargs["TokenCode"] = token_code
             response = self.sts_client.get_session_token(**kwargs)
             os.environ["AWS_ACCESS_KEY_ID"] = response["Credentials"]["AccessKeyId"]
             os.environ["AWS_SECRET_ACCESS_KEY"] = response["Credentials"][
                 "SecretAccessKey"
             ]
             os.environ["AWS_SESSION_TOKEN"] = response["Credentials"]["SessionToken"]
@@ -346,12 +401,12 @@
                 else:
                     os.environ[env_name] = env_value
 
     def clear_cache(self):
         """
         Clear all the boto session and boto client cache.
         """
-        self._boto_ses_cache = None
+        self._boto_ses_cache = NOTHING
         self._client_cache.clear()
         self._resource_cache.clear()
-        self._aws_account_id_cache = None
-        self._aws_region_cache = None
+        self._aws_account_id_cache = NOTHING
+        self._aws_region_cache = NOTHING
```

### Comparing `boto_session_manager-1.4.2/boto_session_manager/services.py` & `boto_session_manager-1.4.3/boto_session_manager/services.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/boto_session_manager.egg-info/PKG-INFO` & `boto_session_manager-1.4.3/boto_session_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: boto-session-manager
-Version: 1.4.2
-Summary: Python AWS SDK boto3 library enhancement
+Version: 1.4.3
+Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto-session-manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.4.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
-License: MIT
+License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `boto_session_manager-1.4.2/boto_session_manager.egg-info/SOURCES.txt` & `boto_session_manager-1.4.3/boto_session_manager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 boto_session_manager/__init__.py
 boto_session_manager/_version.py
 boto_session_manager/clients.py
+boto_session_manager/exc.py
 boto_session_manager/manager.py
+boto_session_manager/sentinel.py
 boto_session_manager/services.py
 boto_session_manager.egg-info/PKG-INFO
 boto_session_manager.egg-info/SOURCES.txt
 boto_session_manager.egg-info/dependency_links.txt
 boto_session_manager.egg-info/requires.txt
 boto_session_manager.egg-info/top_level.txt
 boto_session_manager/docs/__init__.py
```

### Comparing `boto_session_manager-1.4.2/release-history.rst` & `boto_session_manager-1.4.3/release-history.rst`

 * *Files 26% similar despite different names*

```diff
@@ -4,112 +4,123 @@
 ==============================================================================
 
 
 Backlog
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- add auto refreshable session support
-
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+1.5.1 (2023-04-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Add auto refreshable session support (beta). Note that it is using ``AssumeRoleCredentialFetcher`` and ``DeferredRefreshableCredentials`` from botocore, which is not public API officially supported by botocore.
+
+**Minor Improvements**
+
+- Use Sentinel ``NOTHING`` instead of ``None`` to remove the ambiguity of ``None`` value.
+
+
+1.4.3 (2023-04-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- Add ``boto3`` as explicit dependency.
+- Change license from MIT to Apache 2.0
+
+
 1.4.2 (2023-03-24)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
-- fix a bug that the client object cannot locate the right boto3 stubs.
+- Fix a bug that the client object cannot locate the right boto3 stubs.
 
 
 1.4.1 (2023-03-24)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- now all the client and it's methods support auto complete and type hint. You have to do ``pip install "boto3-stubs[all]"`` to enable "Client method auto complete" and "Arguments type hint" features.
+- Now all the client and it's methods support auto complete and type hint. You have to do ``pip install "boto3-stubs[all]"`` to enable "Client method auto complete" and "Arguments type hint" features.
 
 **Bugfixes**
 
-- fix a bug that :meth:`~boto_session_manager.manager.BotoSesManager.awscli()`` context manager doesn't work properly.
+- Fix a bug that :meth:`~boto_session_manager.manager.BotoSesManager.awscli()`` context manager doesn't work properly.
 
 
 1.3.2 (2023-01-31)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- add boto3 documentation link in doc string
+- Add boto3 documentation link in doc string
 
 
 1.3.1 (2022-12-10)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- allow to call :meth:`~boto_session_manager.manager.BotoSesManager.clear_cache()` to clear all cached boto session and client.
-- add ton's of property method to access the cached boto client.
-- update the list of AWS service to the latest (as of 2022-12-10), which are 333 services.
+- Allow to call :meth:`~boto_session_manager.manager.BotoSesManager.clear_cache()` to clear all cached boto session and client.
+- Add ton's of property method to access the cached boto client.
+- Update the list of AWS service to the latest (as of 2022-12-10), which are 333 services.
 
 
 1.2.2 (2022-12-10)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
-- now ``boto_session_manager`` doesn't force to install ``boto3`` when installing itself. You have to manage your ``boto3`` installation separately.
+- Now ``boto_session_manager`` doesn't force to install ``boto3`` when installing itself. You have to manage your ``boto3`` installation separately.
 
 
 1.2.1 (2022-11-20)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- add :meth:`~boto_session_manager.manager.BotoSesManager.awscli` context manager to pass boto session credential to AWS CLI.
+- Add :meth:`~boto_session_manager.manager.BotoSesManager.awscli` context manager to pass boto session credential to AWS CLI.
 
 
 1.1.1 (2022-11-20)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- the first API stable version
+- The first API stable version
 
 **Minor Improvements**
 
-- add ``delta`` arguments for :meth:`~boto_session_manager.manager.BotoSesManager.is_expired` method. allow to check if the session will expire in X seconds.
+- Add ``delta`` arguments for :meth:`~boto_session_manager.manager.BotoSesManager.is_expired` method. allow to check if the session will expire in X seconds.
 
 
 0.0.4 (2022-05-20)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- add ``default_client_kwargs`` argument for :class:`boto_session_manager.manager.BotoSesManager`.
+- Add ``default_client_kwargs`` argument for :class:`boto_session_manager.manager.BotoSesManager`.
 
 **Miscellaneous**
 
-- use `localstack <https://localstack.cloud/>`_ for unit test.
+- Use `localstack <https://localstack.cloud/>`_ for unit test.
 
 
 0.0.3 (2022-05-16)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- add additional keyword arguments for :meth:`boto_session_manager.manager.BotoSesManager.get_client` method
-
-**Minor Improvements**
-
-**Bugfixes**
-
-**Miscellaneous**
+- Add additional keyword arguments for :meth:`boto_session_manager.manager.BotoSesManager.get_client` method
 
 
 0.0.2 (2022-04-30)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-- now :class:`boto_session_manager.manager.BotoSesManager`
-- add :meth:`boto_session_manager.manager.BotoSesManager.get_resource` method
+- Now the public API becomes :class:`boto_session_manager.manager.BotoSesManager`
+- Add :meth:`boto_session_manager.manager.BotoSesManager.get_resource` method
 
 
 0.0.1 (2022-04-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - First release
```

### Comparing `boto_session_manager-1.4.2/requirements-doc.txt` & `boto_session_manager-1.4.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.4.2/setup.py` & `boto_session_manager-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         "MacOS",
         "Unix",
     ]
 
     CLASSIFIERS = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
```

### Comparing `boto_session_manager-1.4.2/tests/test_manager.py` & `boto_session_manager-1.4.3/tests/test_manager.py`

 * *Files identical despite different names*

