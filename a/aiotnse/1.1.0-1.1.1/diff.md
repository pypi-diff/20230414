# Comparing `tmp/aiotnse-1.1.0.tar.gz` & `tmp/aiotnse-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotnse-1.1.0.tar", last modified: Tue Apr  4 13:23:55 2023, max compression
+gzip compressed data, was "aiotnse-1.1.1.tar", last modified: Fri Apr 14 15:03:55 2023, max compression
```

## Comparing `aiotnse-1.1.0.tar` & `aiotnse-1.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.040726 aiotnse-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-04 13:23:38.000000 aiotnse-1.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 13:23:38.000000 aiotnse-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.032726 aiotnse-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.036726 aiotnse-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-04 13:23:38.000000 aiotnse-1.1.0/.github/workflows/release_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-04 13:23:38.000000 aiotnse-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-04 13:23:38.000000 aiotnse-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 13:23:38.000000 aiotnse-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-04 13:23:55.040726 aiotnse-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-04 13:23:38.000000 aiotnse-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.036726 aiotnse-1.1.0/aiotnse/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 13:23:54.000000 aiotnse-1.1.0/aiotnse/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:38.000000 aiotnse-1.1.0/aiotnse/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.036726 aiotnse-1.1.0/aiotnse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 13:23:55.000000 aiotnse-1.1.0/aiotnse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.036726 aiotnse-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-04 13:23:38.000000 aiotnse-1.1.0/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-04 13:23:38.000000 aiotnse-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 13:23:38.000000 aiotnse-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 13:23:38.000000 aiotnse-1.1.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:23:55.040726 aiotnse-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.036726 aiotnse-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:55.040726 aiotnse-1.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/account_status_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/accounts_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/bill_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/current_payment_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/general_info_response.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/latest_readings_closed.json
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/latest_readings_response_t1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/latest_readings_response_t1_t2.json
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/main_page_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/payments_history_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/readings_history_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/registered_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/send_readings_request.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/fixtures/send_readings_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 13:23:38.000000 aiotnse-1.1.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.712526 aiotnse-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 15:03:32.000000 aiotnse-1.1.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 15:03:32.000000 aiotnse-1.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.700525 aiotnse-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.704525 aiotnse-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-14 15:03:32.000000 aiotnse-1.1.1/.github/workflows/release_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-14 15:03:32.000000 aiotnse-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 15:03:32.000000 aiotnse-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 15:03:32.000000 aiotnse-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 15:03:55.712526 aiotnse-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-14 15:03:32.000000 aiotnse-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.708526 aiotnse-1.1.1/aiotnse/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:32.000000 aiotnse-1.1.1/aiotnse/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.708526 aiotnse-1.1.1/aiotnse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:03:55.000000 aiotnse-1.1.1/aiotnse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.708526 aiotnse-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 15:03:32.000000 aiotnse-1.1.1/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-14 15:03:32.000000 aiotnse-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:03:32.000000 aiotnse-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 15:03:32.000000 aiotnse-1.1.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:03:55.712526 aiotnse-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.708526 aiotnse-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:55.712526 aiotnse-1.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/account_status_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/accounts_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/bill_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/current_payment_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/general_info_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/latest_readings_closed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/latest_readings_response_t1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/latest_readings_response_t1_t2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/main_page_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/payments_history_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/readings_history_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/registered_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/send_readings_request.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/fixtures/send_readings_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-14 15:03:32.000000 aiotnse-1.1.1/tests/test_helpers.py
```

### Comparing `aiotnse-1.1.0/.github/workflows/release_to_pypi.yml` & `aiotnse-1.1.1/.github/workflows/release_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/.gitignore` & `aiotnse-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/LICENSE` & `aiotnse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/PKG-INFO` & `aiotnse-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotnse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous Python API For TNS-Energo
 Author: LizardSystems
 License: MIT License
 Project-URL: Home, https://github.com/lizardsystems/aiotnse
 Project-URL: Repository, https://github.com/lizardsystems/aiotnse
 Project-URL: Documentation, https://github.com/lizardsystems/aiotnse
 Project-URL: Bug Tracker, https://github.com/lizardsystems/aiotnse/issues
```

### Comparing `aiotnse-1.1.0/README.md` & `aiotnse-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/aiotnse/api.py` & `aiotnse-1.1.1/aiotnse/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """TNS-Energo API wrapper."""
 from __future__ import annotations
 
 import uuid
-from datetime import datetime
+from datetime import datetime, date
 from typing import Any, Union, Final
 
 from aiohttp import hdrs, MultipartWriter
 
 from .auth import AbstractTNSEAuth
 from .const import DEFAULT_BASE_URL, DEFAULT_API_VERSION
 from .exceptions import RequiredApiParamNotFound
@@ -80,18 +80,18 @@
 
     async def async_get_payments_history(self, account: str) -> dict[str, Any]:
         """Get payments history for account."""
         region = get_region(account)
         _url = f"region/{region}/action/getPaymentsHistPage/ls/{account}/json/"
         return await self._async_get(_url)
 
-    async def async_get_bill(self, account: str, date: datetime) -> dict[str, Any]:
+    async def async_get_bill(self, account: str, dt: date) -> dict[str, Any]:
         """Get general info about account."""
         region = get_region(account)
-        _url = f"region/{region}/action/getBill/ls/{account}/date/{date:%d.%m.%Y}/json/"
+        _url = f"region/{region}/action/getBill/ls/{account}/date/{dt:%d.%m.%Y}/json/"
         return await self._async_get(_url)
 
     async def async_get_latest_readings(self, account: str) -> dict[str, Any]:
         """Get last readings for account."""
         region = get_region(account)
         _url = f"region/{region}/action/getSendReadingsPage/ls/{account}/json/"
         return await self._async_get(_url)
```

### Comparing `aiotnse-1.1.0/aiotnse/auth.py` & `aiotnse-1.1.1/aiotnse/auth.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/aiotnse/cli.py` & `aiotnse-1.1.1/aiotnse/cli.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/aiotnse/const.py` & `aiotnse-1.1.1/aiotnse/const.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/aiotnse/helpers.py` & `aiotnse-1.1.1/aiotnse/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/aiotnse.egg-info/PKG-INFO` & `aiotnse-1.1.1/aiotnse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotnse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous Python API For TNS-Energo
 Author: LizardSystems
 License: MIT License
 Project-URL: Home, https://github.com/lizardsystems/aiotnse
 Project-URL: Repository, https://github.com/lizardsystems/aiotnse
 Project-URL: Documentation, https://github.com/lizardsystems/aiotnse
 Project-URL: Bug Tracker, https://github.com/lizardsystems/aiotnse/issues
```

### Comparing `aiotnse-1.1.0/aiotnse.egg-info/SOURCES.txt` & `aiotnse-1.1.1/aiotnse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/examples/example.py` & `aiotnse-1.1.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/pyproject.toml` & `aiotnse-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/conftest.py` & `aiotnse-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/accounts_response.json` & `aiotnse-1.1.1/tests/fixtures/accounts_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/current_payment_response.json` & `aiotnse-1.1.1/tests/fixtures/current_payment_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/latest_readings_response_t1.json` & `aiotnse-1.1.1/tests/fixtures/latest_readings_response_t1.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/latest_readings_response_t1_t2.json` & `aiotnse-1.1.1/tests/fixtures/latest_readings_response_t1_t2.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/main_page_response.json` & `aiotnse-1.1.1/tests/fixtures/main_page_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/payments_history_response.json` & `aiotnse-1.1.1/tests/fixtures/payments_history_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/readings_history_response.json` & `aiotnse-1.1.1/tests/fixtures/readings_history_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/fixtures/send_readings_response.json` & `aiotnse-1.1.1/tests/fixtures/send_readings_response.json`

 * *Files identical despite different names*

### Comparing `aiotnse-1.1.0/tests/test_api.py` & `aiotnse-1.1.1/tests/test_api.py`

 * *Files identical despite different names*

