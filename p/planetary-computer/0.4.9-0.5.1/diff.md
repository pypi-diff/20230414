# Comparing `tmp/planetary-computer-0.4.9.tar.gz` & `tmp/planetary-computer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetary-computer-0.4.9.tar", last modified: Fri Nov  4 01:30:45 2022, max compression
+gzip compressed data, was "planetary-computer-0.5.1.tar", last modified: Fri Apr 14 19:27:57 2023, max compression
```

## Comparing `planetary-computer-0.4.9.tar` & `planetary-computer-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5113 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/planetary_computer/
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/_adlfs.py
--rw-r--r--   0 runner    (1001) docker     (121)    15062 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/planetary_computer/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/planetary_computer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/planetary_computer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-04 01:30:45.000000 planetary-computer-0.4.9/planetary_computer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:45.643691 planetary-computer-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/tests/test_adlfs.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    13179 2022-11-04 01:30:37.000000 planetary-computer-0.4.9/tests/test_signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/_adlfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_adlfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_signing.py
```

### Comparing `planetary-computer-0.4.9/LICENSE` & `planetary-computer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/PKG-INFO` & `planetary-computer-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: planetary-computer
-Version: 0.4.9
+Version: 0.5.1
 Summary: Planetary Computer SDK for Python
 Author: microsoft
 Author-email: planetarycomputer@microsoft.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: adlfs
 Provides-Extra: azure
+Provides-Extra: dev
 License-File: LICENSE
 
 # Planetary Computer SDK for Python
 
 Python library for interacting with the Microsoft Planetary Computer.
 
 For general questions or discussions about the Planetary Computer, use the [microsoft/PlanetaryComputer](http://github.com/microsoft/PlanetaryComputer) repository.
@@ -93,15 +94,15 @@
 
 ### Convenience methods
 
 You'll occasionally need to interact with the Blob Storage container directly, rather than
 using STAC items. We include two convenience methods for this:
 
 * `planetary_computer.get_container_client`: Get an [`azure.storage.blob.ContainerClient`](https://learn.microsoft.com/en-us/python/api/azure-storage-blob/azure.storage.blob.containerclient?view=azure-python)
-* `planetary_computer.get_adlfs_fliesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
+* `planetary_computer.get_adlfs_filesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
 
 ## Development
 
 The following steps may be followed in order to develop locally:
 
 ```bash
 ## Create and activate venv
```

### Comparing `planetary-computer-0.4.9/README.md` & `planetary-computer-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 ### Convenience methods
 
 You'll occasionally need to interact with the Blob Storage container directly, rather than
 using STAC items. We include two convenience methods for this:
 
 * `planetary_computer.get_container_client`: Get an [`azure.storage.blob.ContainerClient`](https://learn.microsoft.com/en-us/python/api/azure-storage-blob/azure.storage.blob.containerclient?view=azure-python)
-* `planetary_computer.get_adlfs_fliesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
+* `planetary_computer.get_adlfs_filesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
 
 ## Development
 
 The following steps may be followed in order to develop locally:
 
 ```bash
 ## Create and activate venv
```

### Comparing `planetary-computer-0.4.9/planetary_computer/__init__.py` & `planetary-computer-0.5.1/planetary_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/planetary_computer/_adlfs.py` & `planetary-computer-0.5.1/planetary_computer/_adlfs.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/planetary_computer/sas.py` & `planetary-computer-0.5.1/planetary_computer/sas.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 
     token: str
     """The Shared Access (SAS) Token that can be used to access the data
     in, for example, Azure's Python SDK"""
 
     def sign(self, href: str) -> SignedLink:
         """Signs an href with this token"""
-        return SignedLink(href=f"{href}?{self.token}", expiry=self.expiry)
+        return SignedLink(
+            href=f"{href}?{self.token}", expiry=self.expiry  # type: ignore [call-arg]
+        )
 
     def ttl(self) -> float:
         """Number of seconds the token is still valid for"""
         return (self.expiry - datetime.now(timezone.utc)).total_seconds()
 
 
 # Cache of signing requests so we can reuse them
@@ -260,15 +262,14 @@
         href = asset["href"]
 
     if is_fsspec_asset(extra_d):
         key: Optional[str]
 
         storage_options = None
         for key in ["table:storage_options", "xarray:storage_options"]:
-
             if key in extra_d:
                 storage_options = extra_d[key]
                 break
         if storage_options is None:
             storage_options = extra_d.get("xarray:open_kwargs", {}).get(
                 "storage_options", None
             )
@@ -440,14 +441,15 @@
     # Refresh the token if there's less than a minute remaining,
     # in order to give a small amount of buffer
     if not token or token.ttl() < 60:
         session = requests.Session()
         retry = urllib3.util.retry.Retry(
             total=retry_total,
             backoff_factor=retry_backoff_factor,
+            status_forcelist=[429, 500, 502, 503, 504],
         )
         adapter = requests.adapters.HTTPAdapter(max_retries=retry)
         session.mount("http://", adapter)
         session.mount("https://", adapter)
         response = session.get(
             token_request_url,
             headers=(
```

### Comparing `planetary-computer-0.4.9/planetary_computer/scripts/cli.py` & `planetary-computer-0.5.1/planetary_computer/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/planetary_computer/settings.py` & `planetary-computer-0.5.1/planetary_computer/settings.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/planetary_computer/utils.py` & `planetary-computer-0.5.1/planetary_computer/utils.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/planetary_computer.egg-info/PKG-INFO` & `planetary-computer-0.5.1/planetary_computer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: planetary-computer
-Version: 0.4.9
+Version: 0.5.1
 Summary: Planetary Computer SDK for Python
 Author: microsoft
 Author-email: planetarycomputer@microsoft.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: adlfs
 Provides-Extra: azure
+Provides-Extra: dev
 License-File: LICENSE
 
 # Planetary Computer SDK for Python
 
 Python library for interacting with the Microsoft Planetary Computer.
 
 For general questions or discussions about the Planetary Computer, use the [microsoft/PlanetaryComputer](http://github.com/microsoft/PlanetaryComputer) repository.
@@ -93,15 +94,15 @@
 
 ### Convenience methods
 
 You'll occasionally need to interact with the Blob Storage container directly, rather than
 using STAC items. We include two convenience methods for this:
 
 * `planetary_computer.get_container_client`: Get an [`azure.storage.blob.ContainerClient`](https://learn.microsoft.com/en-us/python/api/azure-storage-blob/azure.storage.blob.containerclient?view=azure-python)
-* `planetary_computer.get_adlfs_fliesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
+* `planetary_computer.get_adlfs_filesystem`: Get an [`adlfs.AzureBlobFilesystem`](https://github.com/fsspec/adlfs)
 
 ## Development
 
 The following steps may be followed in order to develop locally:
 
 ```bash
 ## Create and activate venv
```

### Comparing `planetary-computer-0.4.9/planetary_computer.egg-info/SOURCES.txt` & `planetary-computer-0.5.1/planetary_computer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/setup.cfg` & `planetary-computer-0.5.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = planetary-computer
-version = 0.4.9
+version = 0.5.1
 license_file = LICENSE
 author = microsoft
 author_email = planetarycomputer@microsoft.com
 long_description = file:README.md
 long_description_content_type = text/markdown
 description = Planetary Computer SDK for Python
 
@@ -18,14 +18,22 @@
 	pystac-client>=0.2.0
 	pytz>=2020.5
 	requests>=2.25.1
 
 [options.extras_require]
 adlfs = adlfs
 azure = azure-storage-blob
+dev = 
+	black
+	flake8
+	mypy
+	types-requests
+	setuptools
+	pytest
+	responses
 
 [options.entry_points]
 console_scripts = 
 	planetarycomputer = planetary_computer.scripts.cli:app
 
 [egg_info]
 tag_build =
```

### Comparing `planetary-computer-0.4.9/tests/test_adlfs.py` & `planetary-computer-0.5.1/tests/test_adlfs.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/tests/test_settings.py` & `planetary-computer-0.5.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.4.9/tests/test_signing.py` & `planetary-computer-0.5.1/tests/test_signing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import json
 import unittest
 from urllib.parse import parse_qs, urlparse
 from pathlib import Path
 import warnings
 import pystac
+import pytest
+from requests.exceptions import RetryError
 
+import responses
 import requests
 
 import planetary_computer as pc
 from planetary_computer.utils import parse_blob_url, is_fsspec_asset, parse_adlfs_url
 from planetary_computer.sas import get_token, TOKEN_CACHE
 from pystac import Asset, Item, ItemCollection
 from pystac_client import ItemSearch
@@ -363,7 +366,23 @@
             "adlfs://my-container/my/path.ext",
             extra_fields={"xarray:storage_options": {}},
         )
         self.assertFalse(is_fsspec_asset(asset))
 
         asset = Asset("adlfs://my-container/my/path.ext")
         self.assertFalse(is_fsspec_asset(asset))
+
+
+@responses.activate
+def test_retry() -> None:
+    TOKEN_CACHE.clear()
+    rsp1 = responses.Response(
+        method="GET",
+        url="https://planetarycomputer.microsoft.com/api/sas/v1/token/naipeuwest/naip",
+        status=503,
+    )
+    responses.add(rsp1)
+
+    with pytest.raises(RetryError):
+        get_token("naipeuwest", "naip")
+
+    assert rsp1.call_count == 11
```

