# Comparing `tmp/wg_utilities-3.1.1.tar.gz` & `tmp/wg_utilities-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.1.1.tar", max compression
+gzip compressed data, was "wg_utilities-3.2.0.tar", max compression
```

## Comparing `wg_utilities-3.1.1.tar` & `wg_utilities-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/LICENSE
--rw-r--r--   0        0        0     1520 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/README.md
--rw-r--r--   0        0        0     4855 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-09 17:34:11.155226 wg_utilities-3.1.1/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-09 17:34:11.155226 wg_utilities-3.1.1/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      560 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4962 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10359 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24659 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56685 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7142 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    14065 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    16193 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    24945 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49741 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21403 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6589 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     5993 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36348 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8851 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 23:08:24.073689 wg_utilities-3.2.0/LICENSE
+-rw-r--r--   0        0        0     1520 2023-04-13 23:08:24.073689 wg_utilities-3.2.0/README.md
+-rw-r--r--   0        0        0     4825 2023-04-13 23:08:24.077689 wg_utilities-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      560 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     5081 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10359 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24778 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56600 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7261 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    14184 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    16312 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    25465 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49911 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    21546 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.2.0/PKG-INFO
```

### Comparing `wg_utilities-3.1.1/LICENSE` & `wg_utilities-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/README.md` & `wg_utilities-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/pyproject.toml` & `wg_utilities-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.1.1"
+version = "3.2.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
@@ -137,15 +137,14 @@
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "def __repr__", "def __str__", "@overload"]
 
 [tool.coverage.run]
 relative_files = true
 
 [tool.mypy]
-ignore_missing_imports = true
 exclude = ["_local_sandbox"]
 show_error_codes = true
 plugins = 'pydantic.mypy'
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
```

### Comparing `wg_utilities-3.1.1/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.2.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/__init__.py` & `wg_utilities-3.2.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/_google.py` & `wg_utilities-3.2.0/wg_utilities/clients/_google.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,25 +84,27 @@
         *,
         client_id: str,
         client_secret: str,
         base_url: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         """Initialise the client."""
         super().__init__(
             base_url=base_url,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
             scopes=scopes,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
     def get_items(
         self,
         url: str,
         *,
         list_key: Literal["albums", "drives", "files", "items", "point"] = "items",
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.2.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.2.0/wg_utilities/clients/google_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,22 +598,24 @@
         self,
         client_id: str,
         client_secret: str,
         *,
         scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
             scopes=scopes or self.DEFAULT_SCOPE,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self._primary_calendar: Calendar
 
     def create_event(
         self,
         summary: str,
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/google_drive.py` & `wg_utilities-3.2.0/wg_utilities/clients/google_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,14 @@
         }
 
         instance = cls.parse_obj(value_data)
 
         if not _waive_validation:
             instance._validate()  # pylint: disable=protected-access
 
-        # pylint: disable=isinstance-second-argument-not-valid-type
         if isinstance(instance, File | Directory):
             if parent is not None:
                 parent.add_child(instance)
             elif host_drive is not None and host_drive.id == instance.parents[0]:
                 instance.parent_ = host_drive
                 host_drive.add_child(instance)
 
@@ -288,15 +287,14 @@
         Raises:
             TypeError: if the entity is not hosted on a drive
         """
 
         if isinstance(self, Drive):
             return self
 
-        # pylint: disable=isinstance-second-argument-not-valid-type
         if isinstance(self, File | Directory):
             return self.host_drive_
 
         raise TypeError(f"Cannot get host drive of {self.__class__.__name__}.")
 
     @property
     def path(self) -> str:
@@ -916,15 +914,14 @@
     @property
     def parent(self) -> Directory | Drive:
         """Get the parent directory of this file.
 
         Returns:
             Directory: the parent directory of this file
         """
-        # pylint: disable=isinstance-second-argument-not-valid-type
         if self.parent_ is None and isinstance(self, File | Directory):
             if (parent_id := self.parents[0]) == self.host_drive.id:
                 self.parent_ = self.host_drive
             else:
                 self.parent_ = self.host_drive.get_directory_by_id(parent_id)
 
             self.parent_.add_child(self)
@@ -1475,22 +1472,24 @@
         client_secret: str,
         *,
         scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         # pylint: disable=line-too-long
         item_metadata_retrieval: ItemMetadataRetrieval = ItemMetadataRetrieval.ON_FIRST_REQUEST,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
             scopes=scopes or self.DEFAULT_SCOPE,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self._my_drive: Drive
         self.item_metadata_retrieval = item_metadata_retrieval
 
     @property
     def my_drive(self) -> Drive:
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/google_fit.py` & `wg_utilities-3.2.0/wg_utilities/clients/google_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,22 +197,24 @@
         self,
         client_id: str,
         client_secret: str,
         *,
         scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
             scopes=scopes or self.DEFAULT_SCOPES,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self.data_sources: dict[str, DataSource] = {}
 
     def get_data_source(self, data_source_id: str) -> DataSource:
         """Get a data source based on its UID.
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/google_photos.py` & `wg_utilities-3.2.0/wg_utilities/clients/google_photos.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,22 +353,24 @@
         self,
         client_id: str,
         client_secret: str,
         *,
         scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
             scopes=scopes or self.DEFAULT_SCOPES,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self._albums: list[Album]
         # Only really used to check if all album metadata has been fetched, not
         # available to the user (would still require caching all albums).
         self._album_count: int
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/monzo.py` & `wg_utilities-3.2.0/wg_utilities/clients/monzo.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,23 +431,25 @@
     def __init__(
         self,
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self._current_account: Account
 
     def deposit_into_pot(
         self, pot: Pot, amount_pence: int, dedupe_id: str | None = None
     ) -> None:
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.2.0/wg_utilities/clients/oauth_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from datetime import datetime
 from http import HTTPStatus
 from json import JSONDecodeError, dumps
 from logging import DEBUG, getLogger
+from os import getenv
 from pathlib import Path
 from random import choice
 from string import ascii_letters
 from time import time
 from typing import Any, Generic, Literal, TypeAlias, TypeVar
 from urllib.parse import urlencode
 from webbrowser import open as open_browser
@@ -19,14 +20,15 @@
 from jwt import DecodeError, decode
 from pydantic import BaseModel, Extra, validate_model
 from pydantic.generics import GenericModel
 from requests import Response, get, post
 
 from wg_utilities.api import TempAuthServer
 from wg_utilities.functions import user_data_dir
+from wg_utilities.functions.file_management import force_mkdir
 from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 add_stream_handler(LOGGER)
 
 
@@ -215,15 +217,15 @@
     """Custom client for interacting with OAuth APIs.
 
     Includes all necessary/basic authentication functionality
     """
 
     ACCESS_TOKEN_EXPIRY_THRESHOLD = 150
 
-    DATE_FORMAT = "%Y-%m-%d"
+    DEFAULT_CACHE_DIR = getenv("WG_UTILITIES_CREDS_CACHE_DIR")
 
     DEFAULT_PARAMS: dict[
         StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None
     ] = {}
 
     def __init__(
         self,
@@ -232,22 +234,24 @@
         access_token_endpoint: str,
         auth_link_base: str,
         client_id: str | None = None,
         client_secret: str | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         self._client_id = client_id
         self._client_secret = client_secret
         self.base_url = base_url
         self.access_token_endpoint = access_token_endpoint
         self.auth_link_base = auth_link_base
         self.log_requests = log_requests
         self._creds_cache_path = creds_cache_path
+        self.oauth_login_redirect_host = oauth_login_redirect_host
 
         self.scopes = scopes or []
 
         self._credentials: OAuthCredentials
         self._temp_auth_server: TempAuthServer
 
         if self._creds_cache_path:
@@ -416,30 +420,33 @@
         ]
         | None = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
         timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> GetJsonResponse:
+        res = self._request(
+            method=method,
+            url=url,
+            params=params,
+            header_overrides=header_overrides,
+            timeout=timeout,
+            json=json,
+            data=data,
+        )
+        if res.status_code == HTTPStatus.NO_CONTENT:
+            return {}  # type: ignore[return-value]
+
         try:
-            res = self._request(
-                method=method,
-                url=url,
-                params=params,
-                header_overrides=header_overrides,
-                timeout=timeout,
-                json=json,
-                data=data,
-            )
-            if res.status_code == HTTPStatus.NO_CONTENT:
+            return res.json()  # type: ignore[no-any-return]
+        except JSONDecodeError as exc:
+            if not res.content:
                 return {}  # type: ignore[return-value]
 
-            return res.json()  # type: ignore[no-any-return]
-        except JSONDecodeError:
-            return {}  # type: ignore[return-value]
+            raise ValueError(res.text) from exc
 
     def delete_creds_file(self) -> None:
         """Delete the local creds file."""
         self.creds_cache_path.unlink(missing_ok=True)
 
     def get_json_response(
         self,
@@ -562,15 +569,16 @@
         """
         LOGGER.info("Performing first time login")
 
         state_token = "".join(choice(ascii_letters) for _ in range(32))
 
         self.temp_auth_server.start_server()
 
-        redirect_uri = f"http://localhost:{self.temp_auth_server.port}/get_auth_code"
+        # pylint: disable=line-too-long
+        redirect_uri = f"http://{self.oauth_login_redirect_host}:{self.temp_auth_server.port}/get_auth_code"
 
         auth_link = (
             self.auth_link_base
             + "?"
             + urlencode(
                 {
                     "client_id": self._client_id,
@@ -720,16 +728,21 @@
             not (hasattr(self, "_credentials") and self._credentials)
             and not self._client_id
         ):
             raise ValueError(
                 "Unable to get client ID to generate path for credentials cache file."
             )
 
-        return user_data_dir(
-            file_name=f"oauth_credentials/{type(self).__name__}/{self.client_id}.json"
+        file_path = f"{type(self).__name__}/{self.client_id}.json"
+
+        return force_mkdir(
+            Path(self.DEFAULT_CACHE_DIR) / file_path
+            if self.DEFAULT_CACHE_DIR
+            else user_data_dir() / "oauth_credentials" / file_path,
+            path_is_file=True,
         )
 
     @property
     def request_headers(self) -> dict[str, str]:
         """Header to be used in requests to the API.
 
         Returns:
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/spotify.py` & `wg_utilities-3.2.0/wg_utilities/clients/spotify.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,24 +172,27 @@
     def __init__(
         self,
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        scopes: list[str] | None = None,
+        oauth_login_redirect_host: str = "localhost",
     ):
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
-            scopes=self.ALL_SCOPES,
+            scopes=scopes or self.ALL_SCOPES,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self._current_user: User
 
     def add_tracks_to_playlist(
         self,
         tracks: Iterable[Track],
```

### Comparing `wg_utilities-3.1.1/wg_utilities/clients/truelayer.py` & `wg_utilities-3.2.0/wg_utilities/clients/truelayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from logging import DEBUG, getLogger
 from os.path import sep
 from pathlib import Path
 from typing import Any, ClassVar, Literal, TypeAlias, TypedDict, TypeVar
 
 from pydantic import Field, validator
 from requests import HTTPError
-from strenum import StrEnum
+from strenum import StrEnum  # type: ignore[import]
 
 from wg_utilities.clients.oauth_client import (
     BaseModelWithConfig,
     GenericModelWithConfig,
     OAuthClient,
     StrBytIntFlt,
 )
@@ -536,18 +536,19 @@
     ]
 
     def __init__(
         self,
         *,
         client_id: str,
         client_secret: str,
-        bank: Bank,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
+        oauth_login_redirect_host: str = "localhost",
+        bank: Bank,
     ):
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
             client_secret=client_secret,
@@ -562,14 +563,15 @@
                         type(self).__name__,
                         client_id,
                         f"{bank.name.lower()}.json",
                     ]
                 )
             ),
             scopes=scopes or self.ALL_SCOPES,
+            oauth_login_redirect_host=oauth_login_redirect_host,
         )
 
         self.bank = bank
 
     def _get_entity_by_id(
         self,
         entity_id: str,
```

### Comparing `wg_utilities-3.1.1/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.2.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """A class I found a long time ago for DHT22, I can't remember where :(."""
 from __future__ import annotations
 
 from time import sleep
 
-from pigpio import EITHER_EDGE, INPUT, LOW, PUD_OFF, pi, tickDiff
+from pigpio import (  # type: ignore[import]
+    EITHER_EDGE,
+    INPUT,
+    LOW,
+    PUD_OFF,
+    pi,
+    tickDiff,
+)
 
 
 class DHT22Sensor:
     """Class for DHT22 sensor, I can't remember where I got this from.
 
     Args:
         pi_obj (pi): a PI instance from pigpio
```

### Comparing `wg_utilities-3.1.1/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.2.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.2.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.2.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     DC_PIN = 25
     CS_PIN = 8
     BUSY_PIN = 24
 
     # noinspection PyUnresolvedReferences,PyPackageRequirements
     # pylint: disable=import-outside-toplevel
     def __init__(self) -> None:
-        from RPi import GPIO
-        from spidev import SpiDev
+        from RPi import GPIO  # type: ignore[import]
+        from spidev import SpiDev  # type: ignore[import]
 
         self.gpio = GPIO
 
         # SPI device, bus = 0, device = 0
         self.spi = SpiDev(0, 0)
 
     def digital_write(self, pin: int, value: bool) -> None:  # noqa: D102
```

### Comparing `wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Classes etc. for subscribing to YAS-209 updates."""
 from __future__ import annotations
 
 from asyncio import new_event_loop, run
 from asyncio import sleep as async_sleep
-from collections.abc import Callable, Coroutine, Mapping, Sequence
+from collections.abc import Callable, Coroutine, Mapping, MutableMapping, Sequence
 from datetime import datetime, timedelta
 from enum import Enum
 from functools import wraps
 from logging import DEBUG, getLogger
 from re import compile as re_compile
 from textwrap import dedent
 from threading import Thread
@@ -860,15 +860,15 @@
                 callback(res)
 
             return res
 
         return run(_worker(self))  # type: ignore[no-any-return]
 
     @staticmethod
-    def _parse_xml_dict(xml_dict: dict[str, object]) -> None:
+    def _parse_xml_dict(xml_dict: MutableMapping[str, object]) -> None:
         """Convert XML to JSON within dict in place.
 
         Parse a dictionary where some values are/could be XML strings, and unpack
         the XML into JSON within the dict
 
         Args:
             xml_dict (dict): the dictionary to parse
```

### Comparing `wg_utilities-3.1.1/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.2.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/__init__.py` & `wg_utilities-3.2.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/_functions.py` & `wg_utilities-3.2.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.2.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/file_management.py` & `wg_utilities-3.2.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/json.py` & `wg_utilities-3.2.0/wg_utilities/functions/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Useful functions for working with JSON/dictionaries."""
 from __future__ import annotations
 
-from collections.abc import Callable, Sequence
+from collections.abc import Callable, MutableMapping, Sequence
 from logging import DEBUG, getLogger
 from typing import Any, Protocol, Union
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 
 JSONVal = Union[
     None, object, bool, str, float, int, list["JSONVal"], "JSONObj", dict[str, object]
 ]
-JSONObj = dict[str, JSONVal]
+JSONObj = MutableMapping[str, JSONVal]
 
 
 def set_nested_value(
     *,
     json_obj: dict[Any, Any],
     keys: list[str],
     target_value: Any,
```

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/processes.py` & `wg_utilities-3.2.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.2.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/functions/xml.py` & `wg_utilities-3.2.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/loggers/__init__.py` & `wg_utilities-3.2.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.2.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.1/PKG-INFO` & `wg_utilities-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.1.1
+Version: 3.2.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

