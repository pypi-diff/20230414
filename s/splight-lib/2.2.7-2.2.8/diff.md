# Comparing `tmp/splight-lib-2.2.7.tar.gz` & `tmp/splight-lib-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.2.7.tar", last modified: Fri Apr 14 17:15:49 2023, max compression
+gzip compressed data, was "splight-lib-2.2.8.tar", last modified: Fri Apr 14 19:37:50 2023, max compression
```

## Comparing `splight-lib-2.2.7.tar` & `splight-lib-2.2.8.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:48.000000 splight-lib-2.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 17:15:49.161148 splight-lib-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 17:15:48.000000 splight-lib-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:15:49.161148 splight-lib-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 17:15:48.000000 splight-lib-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.319230 splight-lib-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:49.000000 splight-lib-2.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 19:37:50.319230 splight-lib-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 19:37:49.000000 splight-lib-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 19:37:49.000000 splight-lib-2.2.8/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:37:50.319230 splight-lib-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 19:37:49.000000 splight-lib-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.311230 splight-lib-2.2.8/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/restclient/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.315230 splight-lib-2.2.8/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 19:37:50.000000 splight-lib-2.2.8/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.319230 splight-lib-2.2.8/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:37:50.319230 splight-lib-2.2.8/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 19:37:49.000000 splight-lib-2.2.8/splight_models/webhook.py
```

### Comparing `splight-lib-2.2.7/PKG-INFO` & `splight-lib-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.7
+Version: 2.2.8
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.7/remote_splight_lib/communication/client.py` & `splight-lib-2.2.8/remote_splight_lib/communication/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pysher
 import requests
 from furl import furl
 from retry import retry
 from typing import Callable, Dict
-from splight_lib.logging import logging
+from splight_lib.logging import getLogger, LogTags
 from splight_abstract.communication import (
     AbstractCommunicationClient,
     ClientNotReady,
 )
 import logging
 from splight_models.communication import CommunicationClientStatus, CommunicationContext, CommunicationEvent
 
 from remote_splight_lib.auth.auth import SplightAuthToken
 from remote_splight_lib.settings import settings
 from remote_splight_lib.communication.classmap import CLASSMAP
 
 
-logger = logging.getLogger()
+logger = getLogger(dev=True)
 
 
 class CommunicationFactory:
 
     def __init__(self, model):
         self._model = model
 
@@ -60,17 +60,19 @@
             ("pusher:error", self.__on_error),
         ]
         self._daemon = daemon
         try:
             self.__load_context()
             self.__load_client()
             self.__check_readiness()
+            logger.info("Communication client started.", tags=LogTags.COMMUNICATION)
         except Exception as e:
-            logger.exception(e)
-            logger.warning("Failed to start communication client. Moving forward without remote commands.")
+            logger.warning(
+                "Failed to start communication client due to exception %s. Moving forward without remote commands.",
+                e, exc_info=True, tags=LogTags.COMMUNICATION)
             self._status = CommunicationClientStatus.ERROR
 
     @property
     def status(self):
         return self._status
 
     @property
@@ -116,20 +118,20 @@
             self._private_room_channel.bind(event_name, event_handler)
         self._status = CommunicationClientStatus.READY
 
     def __on_connection_failed(self, data):
         self._status = CommunicationClientStatus.FAILED
 
     def __on_error(self, data):
-        logger.error("Error on message", data)
+        logger.error("Error on message %s", data, tags=LogTags.COMMUNICATION)
 
     def bind(self, event_name: str, event_handler: Callable) -> None:
         self._channel_bindings.append((event_name, event_handler))
         if self.status != CommunicationClientStatus.READY:
-            logger.warning("Bind events failed due to comm client is not ready")
+            logger.warning("Bind events failed due to comm client is not ready", tags=LogTags.COMMUNICATION)
             return
         self._channel.bind(event_name, event_handler)
         self._private_room_channel.bind(event_name, event_handler)
 
     def unbind(self, event_name: str, event_handler: Callable) -> None:
         # TODO implement this
         raise NotImplementedError
```

### Comparing `splight-lib-2.2.7/remote_splight_lib/database/classmap.py` & `splight-lib-2.2.8/remote_splight_lib/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/remote_splight_lib/database/client.py` & `splight-lib-2.2.8/splight_lib/client/database/remote_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import json
-from .classmap import CLASSMAP
-from retry import retry
-from splight_abstract.remote import AbstractRemoteClient
-from splight_abstract.database import AbstractDatabaseClient
-from splight_models import File
-from remote_splight_lib.settings import settings
-from remote_splight_lib.exceptions import InvalidModel
-from remote_splight_lib.auth import SplightAuthToken
-from splight_lib.encryption import EncryptionClient
+from tempfile import NamedTemporaryFile
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
 from requests import Session
-from requests.exceptions import (
-    ConnectionError,
-    Timeout
-)
-from tempfile import NamedTemporaryFile
 
+from retry import retry
 
-REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
+from splight_abstract.database import AbstractDatabaseClient
+from splight_abstract.remote import AbstractRemoteClient
+from splight_lib.auth import SplightAuthToken
+from splight_lib.logging import getLogger, LogTags
+from splight_lib.client.database.classmap import CLASSMAP
+from splight_lib.client.exceptions import REQUEST_EXCEPTIONS, InvalidModel
+from splight_lib.client.settings import settings_remote as settings
+from splight_lib.encryption import EncryptionClient
+from splight_models import File
 
+logger = getLogger(dev=True)
 
-class DatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
+
+class RemoteDatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
     Responsible for interacting with database resources using HTTP requests
     to the Splight API.
     """
 
-    def __init__(self, namespace: str = "default"):
-        super(DatabaseClient, self).__init__(namespace=namespace)
+    def __init__(self, namespace: str = "default", *args, **kwargs):
+        super().__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._session = Session()
         self._session.headers.update(token.header)
+        logger.info("Remote database client initialized.", tags=LogTags.DATABASE)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def save(self, instance: BaseModel) -> BaseModel:
         """Creates or updates a new resource depending on the model if
         it contains the id or not.
 
         Parameters
@@ -53,14 +52,16 @@
         -------
         BaseModel with the created or updated resource.
 
         Raises
         ------
         InvalidModel thrown when the model name is not correct.
         """
+        logger.debug("Saving instance %s.", instance.id, tags=LogTags.DATABASE)
+
         constructor = type(instance)
         model_data = self._get_model_data(constructor)
 
         path = model_data["path"]
         if instance.id:
             output = self._update(path, instance.id, instance)
         else:
@@ -79,14 +80,15 @@
         id : str
             The resource's id.
 
         Raises
         ------
         InvalidModel thrown when the model name is not correct.
         """
+        logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         url = self._base_url / f"{path}/{id}/"
         response = self._session.delete(url)
         response.raise_for_status()
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
@@ -98,26 +100,18 @@
         skip_: int = 0,
         page_size: int = -1,
         deleted: bool = False,
         **kwargs,
     ) -> List[BaseModel]:
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
-        response = self._list(
-            path,
-            limit_=limit_,
-            skip_=skip_,
-            deleted=deleted,
-            page_size=page_size,
-            **kwargs,
-        )
-        parsed = [
-            resource_type.parse_obj(resource)
-            for resource in response["results"]
-        ]
+        instances = []
+        for page in self._pages(path, page=1, deleted=deleted, **kwargs):
+            instances.extend(page["results"])
+        parsed = [resource_type.parse_obj(item) for item in instances]
         if first:
             return parsed[0] if parsed else None
         return parsed
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def count(self, resource_type: Type, **kwargs) -> int:
         """Returns the number of resources in the database for a given model
@@ -135,18 +129,21 @@
         ------
         InvalidModel thrown when the model name is not correct.
         """
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         kwargs["page"] = 1  # Always start from the first page
         response = self._list(path, **kwargs)
+        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
         return response["count"]
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def download(self, instance: BaseModel, decrypt: bool = True, **kwargs) -> NamedTemporaryFile:
+    def download(
+        self, instance: BaseModel, decrypt: bool = True, **kwargs
+    ) -> NamedTemporaryFile:
         """Returns the number of resources in the database for a given model
 
         Parameters
         ----------
         instance : BaseModel
             The instance of the model to be downloaded
 
@@ -167,14 +164,15 @@
         response.raise_for_status()
         f = NamedTemporaryFile("wb+")
         f.write(response.content)
         f.seek(0)
         if decrypt and instance.encrypted:
             encryption_manager = EncryptionClient()
             encryption_manager.decrypt_file(path=f.name)
+        logger.debug("Downloaded instance %s.", id, tags=LogTags.DATABASE)
         return f
 
     def _pages(self, path: str, **kwargs):
         next_page = kwargs["page"]
         while next_page:
             response = self._list(path, **kwargs)
             yield response
@@ -199,15 +197,15 @@
             raise InvalidModel(constructor.schema()["title"])
         return model_data
 
     def _create(self, path: str, instance: BaseModel) -> Dict:
         url = self._base_url / f"{path}/"
         data = json.loads(instance.json(exclude_none=True))
         if isinstance(instance, File):
-            with open(instance.file, 'rb') as f:
+            with open(instance.file, "rb") as f:
                 file = {"file": f}
                 response = self._session.post(url, data=data, files=file)
         else:
             response = self._session.post(url, json=data)
 
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.2.7/remote_splight_lib/datalake/client.py` & `splight-lib-2.2.8/remote_splight_lib/datalake/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 
 import pandas as pd
 import json
 from furl import furl
 from pydantic import BaseModel
 
 from remote_splight_lib.auth import SplightAuthToken
+from splight_lib.logging import getLogger, LogTags
 from remote_splight_lib.settings import settings
 from splight_abstract import AbstractRemoteClient, QuerySet
 from splight_abstract.datalake import AbstractDatalakeClient, validate_resource_type, validate_instance_type
 from splight_models import Query, DatalakeModel
 from retry import retry
 
 from splight_lib.restclient import (
     SplightRestClient,
     HTTPError,
     Timeout,
     ConnectError
 )
+
+logger = getLogger(dev=True)
+
 REQUEST_EXCEPTIONS = (HTTPError, Timeout, ConnectError)
 
 
 class DatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
 
     _PREFIX = "v2/engine/datalake"
 
@@ -33,14 +37,16 @@
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
+        logger.info("Datalake client initialized.", tags=LogTags.DATALAKE)
+
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def _raw_save(
         self,
         collection: str,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
@@ -101,22 +107,24 @@
     @validate_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
+        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(self, *args, **kwargs)
 
     def get_output(self, resource_type: DatalakeModel, query: Query) -> List[Dict]:
         # TODO: Add add_fields, project and renaming
+        logger.debug("Retrieving output of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
         return self._raw_get(
             resource_type=resource_type,
             collection=query.source,
             limit_=query.limit,
             skip_=query.skip,
             sort=query.sort,
             group_id=query.group_id,
@@ -131,51 +139,58 @@
         # GET /datalake/dumpdata/?source=collection
         url = self._base_url / f"{self._PREFIX}/dumpdata/"
         collection = resource_type.Meta.collection_name
         kwargs.update({"source": collection})
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
         response.raise_for_status()
+        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
 
         df: pd.DataFrame = pd.DataFrame(pd.read_csv(StringIO(response.text)))
         if df.empty:
             return df
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df.set_index("timestamp", inplace=True)
         return df
 
     def get_dataset(
         self, resource_type: DatalakeModel, queries: List[Dict]
     ) -> pd.DataFrame:
         # TODO this should be
         # def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
+        logger.debug("Retrieving dataset from datalake.", tags=LogTags.DATALAKE)
+
         dfs = [
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
         return pd.DataFrame(dfs)
 
     @validate_instance_type
     def save(
         self,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
         # POST /datalake/save/
+        logger.debug("Saving instances %s.",
+                    [instance.id for instance in instances], tags=LogTags.DATALAKE)
         if not instances:
             return instances
         resource_type = instances[0].__class__
         collection = resource_type.Meta.collection_name
         return self._raw_save(collection=collection, instances=instances)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     @validate_resource_type
     def save_dataframe(self, resource_type: DatalakeModel, dataframe: pd.DataFrame) -> None:
         # POST /datalake/loaddata/
+        logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
+
         url = self._base_url / f"{self._PREFIX}/loaddata/"
 
         tmp_file = NamedTemporaryFile("w")
         with open(tmp_file.name, "wb") as fid:
             dataframe.to_csv(fid)
         collection = resource_type.Meta.collection_name
         response = self._restclient.post(
@@ -183,29 +198,33 @@
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
     @validate_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
+        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+
         collection = resource_type.Meta.collection_name
         return self._raw_delete(collection=collection, **kwargs)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def create_index(self, collection: str, indexes: List[Dict]) -> None:
         # POST /datalake/index/
+        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
         url = self._base_url / f"{self._PREFIX}/index/"
         data = {"source": collection, "index": indexes}
         response = self._restclient.post(url, json=data)
         response.raise_for_status()
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
+        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
         # POST /datalake/aggregate/?source=collection
         url = self._base_url / f"{self._PREFIX}/aggregate/"
         params = {"source": collection}
         data = {"pipeline": pipeline}
         response = self._restclient.post(url, params=params, data=data)
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.2.7/remote_splight_lib/hub/client.py` & `splight-lib-2.2.8/remote_splight_lib/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/remote_splight_lib/settings.py` & `splight-lib-2.2.8/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/setup.py` & `splight-lib-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 dependency_links = [
     # External repoitories different from pypi
 ]
 
 setup(
     name='splight-lib',
-    version='2.2.7',
+    version='2.2.8',
     author='Splight',
     author_email='factory@splight-ae.com',
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.2.7/splight_abstract/auth/abstract.py` & `splight-lib-2.2.8/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/auth/exceptions.py` & `splight-lib-2.2.8/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/cache/abstract.py` & `splight-lib-2.2.8/splight_abstract/cache/abstract.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 from functools import wraps
 from typing import Callable, List
 from abc import abstractmethod
 from splight_abstract.client import AbstractClient
-from splight_lib import logging
+from splight_lib.logging import getLogger, LogTags
 
 
-logger = logging.getLogger()
-
+logger = getLogger(dev=True)
 
 class AbstractCacheClient(AbstractClient):
 
     @abstractmethod
     def get(self, key):
         pass
 
@@ -42,28 +41,28 @@
                 else:
                     for key_arg in cache_key_args:
                         final_cache_key = f'{final_cache_key}:{key_arg}-{str(full_args.get(key_arg))}'
 
             try:
                 cached_data = client.get(final_cache_key)
             except Exception:
-                logger.error(f'Error getting cache for {final_cache_key}')
+                logger.error('Error getting cache for %s', final_cache_key, tags=LogTags.CACHE)
 
             if isinstance(cached_data, bytes):
-                logger.info(f'Cache hit for {final_cache_key}')
+                logger.info('Cache hit for %s', final_cache_key, tags=LogTags.CACHE)
 
                 return json.loads(cached_data.decode('utf-8'))
             else:
                 cached_data = func(*args, **kwargs)
 
                 try:
                     client.set(final_cache_key, json.dumps(cached_data), ex=3600)
-                    logger.info(f'Cache update for {final_cache_key}')
+                    logger.info('Cache update for %s', final_cache_key, tags=LogTags.CACHE)
                 except Exception:
-                    logger.error(f'Error getting cache for {final_cache_key}')
+                    logger.error('Error getting cache for %s', final_cache_key, tags=LogTags.CACHE)
 
                 return cached_data
         return wrapper
     return decorator
 
 
 def flush_cache(client: AbstractCacheClient, cache_key: str, cache_key_args: str or List[str] = None, prefix_match=False) -> Callable:
@@ -80,14 +79,14 @@
                     for key_arg in cache_key_args:
                         final_cache_key += f':{key_arg}-{str(full_args.get(key_arg))}'
 
             try:
                 if prefix_match:
                     final_cache_key += '*'
                 client.delete(final_cache_key)
-                logger.info(f'Cache flush for {final_cache_key}')
+                logger.info('Cache flush for %s', final_cache_key, tags=LogTags.CACHE)
             except Exception:
-                logger.error(f'Error flushing cache for {final_cache_key}')
+                logger.error('Error flushing cache for %s', final_cache_key, tags=LogTags.CACHE)
 
             return func(*args, **kwargs)
         return wrapper
     return decorator
```

### Comparing `splight-lib-2.2.7/splight_abstract/client/abstract.py` & `splight-lib-2.2.8/splight_abstract/client/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from collections import UserList
 from pydantic import BaseModel
 from typing import List, Type, Callable
 from functools import wraps
 from abc import ABC
-from splight_lib import logging
 from .filter import FilterMixin
 from .hooks import HooksMixin
 
 
-logger = logging.getLogger()
-
-
 class empty:
     pass
 
 
 def validate_resource_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, resource_type: Type, *args, **kwargs):
```

### Comparing `splight-lib-2.2.7/splight_abstract/client/filter.py` & `splight-lib-2.2.8/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/client/hooks.py` & `splight-lib-2.2.8/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/communication/abstract.py` & `splight-lib-2.2.8/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/database/abstract.py` & `splight-lib-2.2.8/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/datalake/abstract.py` & `splight-lib-2.2.8/splight_abstract/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/deployment/abstract.py` & `splight-lib-2.2.8/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/endpoints/__init__.py` & `splight-lib-2.2.8/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/hub/abstract.py` & `splight-lib-2.2.8/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_abstract/storage/abstract.py` & `splight-lib-2.2.8/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/auth/mac_auth.py` & `splight-lib-2.2.8/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/client/database/classmap.py` & `splight-lib-2.2.8/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/client/database/local_client.py` & `splight-lib-2.2.8/splight_lib/client/database/local_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,43 +5,49 @@
 from typing import Dict, List, Type, Union
 from uuid import uuid4
 
 from splight_abstract.database import AbstractDatabaseClient
 from splight_lib.client.exceptions import InstanceNotFound
 from splight_lib.client.filter import value_filter_on_tuple
 from splight_models import SplightBaseModel
+from splight_lib.logging import getLogger, LogTags
 
 ResourceType = Type[SplightBaseModel]
 
+logger = getLogger(dev=True)
+
 
 class LocalDatabaseClient(AbstractDatabaseClient):
     """Database Client implementation for a local database that uses a
     JSON file.
     """
 
     def __init__(self, namespace: str, path: str, *args, **kwargs):
         super().__init__(namespace)
         self._db_file = os.path.join(path, "splight-db.json")
 
         if not os.path.exists(self._db_file):
             self._save_db(self._db_file, {})
+        logger.info("Local database client initialized.", tags=LogTags.DATABASE)
 
     def save(self, instance: SplightBaseModel) -> SplightBaseModel:
         """Saves an instance in the local database, if the instance has an id
         will try to update the instance, otherwise it will create a new one.
 
         Parameters
         ----------
         instance : SplightBaseModel
             The instance to be saved in the database.
 
         Returns
         -------
         SplightBaseModel: The instances saved in the database.
         """
+        logger.debug("Saving instance %s.", instance.id, tags=LogTags.DATABASE)
+
         model_class = type(instance)
         model_name = model_class.__name__.lower()
         if instance.id:
             new_instance = self._update(model_name, instance)
         else:
             new_instance = self._create(model_name, instance)
         return new_instance
@@ -56,14 +62,15 @@
         id: str
             The object's id to delete.
 
         Raises
         ------
         InstanceNotFound if the object with the given id is not in the database
         """
+        logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         model_name = resource_type.__name__.lower()
         db = self._load_db_file(self._db_file)
         db_instances = db.get(model_name, {})
 
         if id not in db_instances:
             raise InstanceNotFound(model_name, id)
 
@@ -97,14 +104,15 @@
             return parsed[0] if parsed else None
         return parsed
 
     def count(self, resource_type: ResourceType, **kwargs) -> int:
         db = self._load_db_file(self._db_file)
         model_name = resource_type.__name__.lower()
         db_instances = db.get(model_name, {})
+        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
         return len(db_instances)
 
     def download(
         self, instances: SplightBaseModel, decrtypt: bool = True, **kwargs
     ) -> NamedTemporaryFile:
         raise NotImplementedError()
```

### Comparing `splight-lib-2.2.7/splight_lib/client/database/remote_client.py` & `splight-lib-2.2.8/remote_splight_lib/database/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import json
-from tempfile import NamedTemporaryFile
+from .classmap import CLASSMAP
+from retry import retry
+from splight_abstract.remote import AbstractRemoteClient
+from splight_abstract.database import AbstractDatabaseClient
+from splight_models import File
+from remote_splight_lib.settings import settings
+from remote_splight_lib.exceptions import InvalidModel
+from remote_splight_lib.auth import SplightAuthToken
+from splight_lib.logging import getLogger, LogTags
+from splight_lib.encryption import EncryptionClient
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
 from requests import Session
+from requests.exceptions import (
+    ConnectionError,
+    Timeout
+)
+from tempfile import NamedTemporaryFile
 
-from retry import retry
 
-from splight_abstract.database import AbstractDatabaseClient
-from splight_abstract.remote import AbstractRemoteClient
-from splight_lib.auth import SplightAuthToken
-from splight_lib.client.database.classmap import CLASSMAP
-from splight_lib.client.exceptions import REQUEST_EXCEPTIONS, InvalidModel
-from splight_lib.client.settings import settings_remote as settings
-from splight_lib.encryption import EncryptionClient
-from splight_models import File
+logger = getLogger(dev=True)
 
+REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
 
-class RemoteDatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
+
+class DatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
     Responsible for interacting with database resources using HTTP requests
     to the Splight API.
     """
 
-    def __init__(self, namespace: str = "default", *args, **kwargs):
-        super().__init__(namespace=namespace)
+    def __init__(self, namespace: str = "default"):
+        super(DatabaseClient, self).__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._session = Session()
         self._session.headers.update(token.header)
+        logger.info("Database client initialized.", tags=LogTags.DATABASE)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def save(self, instance: BaseModel) -> BaseModel:
         """Creates or updates a new resource depending on the model if
         it contains the id or not.
 
         Parameters
@@ -48,14 +57,16 @@
         -------
         BaseModel with the created or updated resource.
 
         Raises
         ------
         InvalidModel thrown when the model name is not correct.
         """
+        logger.debug("Saving instance %s.", instance.id, tags=LogTags.DATABASE)
+
         constructor = type(instance)
         model_data = self._get_model_data(constructor)
 
         path = model_data["path"]
         if instance.id:
             output = self._update(path, instance.id, instance)
         else:
@@ -74,14 +85,15 @@
         id : str
             The resource's id.
 
         Raises
         ------
         InvalidModel thrown when the model name is not correct.
         """
+        logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         url = self._base_url / f"{path}/{id}/"
         response = self._session.delete(url)
         response.raise_for_status()
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
@@ -93,18 +105,26 @@
         skip_: int = 0,
         page_size: int = -1,
         deleted: bool = False,
         **kwargs,
     ) -> List[BaseModel]:
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
-        instances = []
-        for page in self._pages(path, page=1, deleted=deleted, **kwargs):
-            instances.extend(page["results"])
-        parsed = [resource_type.parse_obj(item) for item in instances]
+        response = self._list(
+            path,
+            limit_=limit_,
+            skip_=skip_,
+            deleted=deleted,
+            page_size=page_size,
+            **kwargs,
+        )
+        parsed = [
+            resource_type.parse_obj(resource)
+            for resource in response["results"]
+        ]
         if first:
             return parsed[0] if parsed else None
         return parsed
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def count(self, resource_type: Type, **kwargs) -> int:
         """Returns the number of resources in the database for a given model
@@ -118,24 +138,24 @@
         -------
         int
 
         Raises
         ------
         InvalidModel thrown when the model name is not correct.
         """
+
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         kwargs["page"] = 1  # Always start from the first page
         response = self._list(path, **kwargs)
+        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
         return response["count"]
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def download(
-        self, instance: BaseModel, decrypt: bool = True, **kwargs
-    ) -> NamedTemporaryFile:
+    def download(self, instance: BaseModel, decrypt: bool = True, **kwargs) -> NamedTemporaryFile:
         """Returns the number of resources in the database for a given model
 
         Parameters
         ----------
         instance : BaseModel
             The instance of the model to be downloaded
 
@@ -156,14 +176,15 @@
         response.raise_for_status()
         f = NamedTemporaryFile("wb+")
         f.write(response.content)
         f.seek(0)
         if decrypt and instance.encrypted:
             encryption_manager = EncryptionClient()
             encryption_manager.decrypt_file(path=f.name)
+        logger.debug("Downloaded instance %s.", id, tags=LogTags.DATABASE)
         return f
 
     def _pages(self, path: str, **kwargs):
         next_page = kwargs["page"]
         while next_page:
             response = self._list(path, **kwargs)
             yield response
@@ -188,15 +209,15 @@
             raise InvalidModel(constructor.schema()["title"])
         return model_data
 
     def _create(self, path: str, instance: BaseModel) -> Dict:
         url = self._base_url / f"{path}/"
         data = json.loads(instance.json(exclude_none=True))
         if isinstance(instance, File):
-            with open(instance.file, "rb") as f:
+            with open(instance.file, 'rb') as f:
                 file = {"file": f}
                 response = self._session.post(url, data=data, files=file)
         else:
             response = self._session.post(url, json=data)
 
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.2.7/splight_lib/client/datalake/local_client.py` & `splight-lib-2.2.8/splight_lib/client/datalake/local_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,30 +7,34 @@
 import pandas as pd
 
 from splight_abstract.client import QuerySet
 from splight_abstract.datalake import AbstractDatalakeClient
 from splight_lib.client.file_handler import FixedLineNumberFileHandler
 from splight_lib.client.filter import value_filter
 from splight_models import DatalakeModel, Query
+from splight_lib.logging import getLogger, LogTags
 
 DLResource = Type[DatalakeModel]
 
+logger = getLogger(dev=True)
+
 
 class LocalDatalakeClient(AbstractDatalakeClient):
     """Datalake client implementation for a storing locally documents
     in different files.
     """
 
     _DEFAULT = "default"
     _PREFIX = "dl_"
     _TOTAL_DOCS = 10000
 
     def __init__(self, namespace: str, path: str):
         super().__init__(namespace=namespace)
         self._base_path = path
+        logger.info("Local datalake client initialized.", tags=LogTags.DATALAKE)
 
     def _raw_get(
         self,
         resource_type: DLResource,
         limit_: int = -1,
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
@@ -69,14 +73,16 @@
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
         group_id: Union[List, str] = [],
         group_fields: Union[List, str] = [],
         tzinfo: timezone = timezone(timedelta()),
         **kwargs,
     ) -> QuerySet:
+        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(
             self,
             limit_,
@@ -91,58 +97,66 @@
     def get_output(self, query: Query) -> List[Dict]:
         raise NotImplementedError()
 
     def get_dataframe(
         self, resource_type: Type, freq: str = "H", **kwargs
     ) -> pd.DataFrame:
         """Reads documents and returns a dataframe"""
+        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
         documents = self._raw_get(resource_type, **kwargs)
         df = pd.DataFrame([x.dict() for x in documents])
         if not df.empty:
             df.set_index("timestamp", inplace=True, verify_integrity=False)
         return df
 
     def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
         raise NotImplementedError()
 
     def save(self, instances: List[DatalakeModel]) -> List[DatalakeModel]:
         documents = [instance.json() for instance in instances]
         if not instances:
             return instances
 
+        logger.debug("Saving instances %s.",
+                    [instance.id for instance in instances], tags=LogTags.DATALAKE)
+
         collection = instances[0].Meta.collection_name
 
         file_path = os.path.join(
             self._base_path, self._get_file_name(collection)
         )
         handler = FixedLineNumberFileHandler(
             file_path=file_path, total_lines=self._TOTAL_DOCS
         )
         handler.write(documents)
         return instances
 
     def save_dataframe(
         self, resource_type: DLResource, dataframe: pd.DataFrame
     ) -> None:
+        logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
 
         instances = dataframe.apply(
             lambda x: resource_type.parse_obj(x.to_dict()), axis=1
         )
         instances = instances.to_list()
         _ = self.save(instances)
 
     def delete(self, resource_type: DLResource, **kwargs) -> None:
-        pass
+        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        raise NotImplementedError()
 
     def create_index(self, collection: str, index: list) -> None:
-        pass
+        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
+        raise NotImplementedError()
 
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
+        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
         raise NotImplementedError()
 
     def _filter(
         self, instances: List[DLResource], filters: Dict
     ) -> List[DLResource]:
         filtered = instances
         for key, value in filters.items():
```

### Comparing `splight-lib-2.2.7/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.2.8/splight_lib/client/datalake/remote_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,30 +15,34 @@
     AbstractDatalakeClient,
     validate_instance_type,
     validate_resource_type,
 )
 from splight_lib.client.exceptions import SPLIGHT_REQUEST_EXCEPTIONS
 from splight_lib.client.settings import settings_remote as settings
 from splight_lib.restclient import SplightRestClient
+from splight_lib.logging import getLogger, LogTags
 from splight_models import DatalakeModel, Query
 
+logger = getLogger(dev=True)
+
 
 class RemoteDatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
 
     _PREFIX = "v2/engine/datalake"
 
     def __init__(self, namespace: str = "default", *args, **kwargs):
         super().__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
+        logger.info("Remote datalake client initialized.", tags=LogTags.DATALAKE)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def _raw_save(
         self,
         collection: str,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
@@ -99,24 +103,26 @@
     @validate_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
+        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(self, *args, **kwargs)
 
     def get_output(
         self, resource_type: DatalakeModel, query: Query
     ) -> List[Dict]:
         # TODO: Add add_fields, project and renaming
+        logger.debug("Retrieving output of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
         return self._raw_get(
             resource_type=resource_type,
             collection=query.source,
             limit_=query.limit,
             skip_=query.skip,
             sort=query.sort,
             group_id=query.group_id,
@@ -133,50 +139,58 @@
         # GET /datalake/dumpdata/?source=collection
         url = self._base_url / f"{self._PREFIX}/dumpdata/"
         collection = resource_type.Meta.collection_name
         kwargs.update({"source": collection})
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
         response.raise_for_status()
+        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
 
         df: pd.DataFrame = pd.DataFrame(pd.read_csv(StringIO(response.text)))
         if df.empty:
             return df
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df.set_index("timestamp", inplace=True)
         return df
 
     def get_dataset(
         self, resource_type: DatalakeModel, queries: List[Dict]
     ) -> pd.DataFrame:
+        logger.debug("Retrieving dataset from datalake.", tags=LogTags.DATALAKE)
+
         dfs = [
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
         return pd.DataFrame(dfs)
 
     @validate_instance_type
     def save(
         self,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
         # POST /datalake/save/
+        logger.debug("Saving instances %s.",
+                    [instance.id for instance in instances], tags=LogTags.DATALAKE)
+
         if not instances:
             return instances
         resource_type = instances[0].__class__
         collection = resource_type.Meta.collection_name
         return self._raw_save(collection=collection, instances=instances)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     @validate_resource_type
     def save_dataframe(
         self, resource_type: DatalakeModel, dataframe: pd.DataFrame
     ) -> None:
+        logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
+        
         # POST /datalake/loaddata/
         url = self._base_url / f"{self._PREFIX}/loaddata/"
 
         tmp_file = NamedTemporaryFile("w")
         with open(tmp_file.name, "wb") as fid:
             dataframe.to_csv(fid)
         collection = resource_type.Meta.collection_name
@@ -185,29 +199,34 @@
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
     @validate_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
+        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+
         collection = resource_type.Meta.collection_name
         return self._raw_delete(collection=collection, **kwargs)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def create_index(self, collection: str, indexes: List[Dict]) -> None:
         # POST /datalake/index/
+        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
+        
         url = self._base_url / f"{self._PREFIX}/index/"
         data = {"source": collection, "index": indexes}
         response = self._restclient.post(url, json=data)
         response.raise_for_status()
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
+        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
         # POST /datalake/aggregate/?source=collection
         url = self._base_url / f"{self._PREFIX}/aggregate/"
         params = {"source": collection}
         data = {"pipeline": pipeline}
         response = self._restclient.post(url, params=params, data=data)
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.2.7/splight_lib/client/exceptions.py` & `splight-lib-2.2.8/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/client/file_handler.py` & `splight-lib-2.2.8/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/client/filter.py` & `splight-lib-2.2.8/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/client/settings.py` & `splight-lib-2.2.8/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/component/abstract.py` & `splight-lib-2.2.8/splight_lib/component/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tempfile import NamedTemporaryFile
 from typing import Optional, Type, List, Dict, Tuple, Set, Any, Callable, Union
 from mergedeep import merge, Strategy as mergeStrategy
 from collections import defaultdict
 from pydantic import BaseModel, main
 from functools import cached_property
 from splight_lib.execution import ExecutionClient, Thread
-from splight_lib.logging import logging
+from splight_lib.logging import getLogger, LogTags
 from splight_lib.settings import setup as default_setup
 from splight_models import (
     CustomType,
     Deployment,
     DatalakeModel,
     Component,
     Command,
@@ -44,23 +44,24 @@
     SetPointResponseStatus,
     SetPointCreateEvent,
     SetPointUpdateEvent
 )
 import re
 
 
-logger = logging.getLogger()
+logger = getLogger(dev=True)
 
 
 class SecretValueParser:
 
     def __init__(self, utils, *args, **kwargs):
         self.utils = utils
 
     def get_value(self, name: str) -> Any:
+        logger.info("Obtaining secret: %s", name, tags=LogTags.SECRET)
         secret = self.utils.database_client.get(Secret, name=name, first=True)
         return secret.decrypt()
 
 
 class VariableValueMixin:
     _variable_parameter_map_class = {
         'SECRET': SecretValueParser,
@@ -88,23 +89,26 @@
     _STARTUP_FILE_PREFIX = "ready_"
 
     def __init__(self):
         self.health_file = NamedTemporaryFile(prefix=self._HEALTH_FILE_PREFIX)
         self.startup_file = NamedTemporaryFile(
             prefix=self._STARTUP_FILE_PREFIX
         )
+        logger.info("Healthcheck file at: %s", self.health_file.name, tags=LogTags.RUNTIME)
+        logger.info("Startup file at: %s", self.startup_file.name, tags=LogTags.RUNTIME)
+
         self.execution_client.start(Thread(self.healthcheck))
 
     def healthcheck(self) -> None:
         self.terminated = False
         while not self.terminated:
             if not self.execution_client.healthcheck():
-                logger.error("A task has failed")
+                logger.error("Healthcheck task failed.", tags=LogTags.RUNTIME)
                 self.health_file.close()
-                logger.error(f"Healthcheck file removed: {self.health_file}")
+                logger.error("Healthcheck file removed: %s", self.health_file, tags=LogTags.RUNTIME)
                 sys.exit()
             time.sleep(self.healthcheck_interval)
 
     @abstractmethod
     def start(self):
         pass
 
@@ -113,15 +117,15 @@
 
 
 class IndexMixin:
     def _load_client_indexes(self) -> None:
         indexes: List[Tuple[str, int]] = self.__get_indexes()
         collections: List[str] = self.__get_collections()
         for col in collections:
-            logger.debug(f"Adding indexes: {indexes} for collection {col}")
+            logger.info("Adding indexes: %s for collection %s", indexes , col, tags=LogTags.INDEX)
             self.datalake_client.create_index(
                 col,
                 indexes
             )
 
     def __get_collections(self) -> List[str]:
         native_output_types = [Boolean, String, Number]
@@ -150,63 +154,71 @@
             indexes.append((index, 1))
 
         return indexes
 
 
 class HooksMixin:
     def _load_client_hooks(self):
+
+        logger.info("Adding pre-hooks for database and datalake clients.", tags=LogTags.HOOK)
+
         # Datalake
         self.datalake_client.add_pre_hook("save", self.__hook_insert_origin_save)
         self.datalake_client.add_pre_hook("save_dataframe", self.__hook_insert_origin_save_dataframe)
         # Database
         self.database_client.add_pre_hook("save", self.__hook_transform_from_custom_instances)
         self.database_client.add_pre_hook("_get", self.__hook_transform_from_custom_resource_type)
         self.database_client.add_pre_hook("delete", self.__hook_transform_from_custom_resource_type)
         self.database_client.add_pre_hook("count", self.__hook_transform_from_custom_resource_type)
         self.database_client.add_post_hook("_get", self.__hook_transform_to_custom_instances)
         self.database_client.add_post_hook("save", self.__hook_transform_to_custom_instances)
 
     def __hook_insert_origin_save(self, *args, **kwargs):
+        logger.info("Datalake save pre-hook.", tags=LogTags.HOOK)
         instances = kwargs.get("instances", [])
         for instance in instances:
             if not isinstance(instance, DatalakeModel):
                 continue
             instance.instance_id = self.instance_id
             instance.instance_type = self.instance_type.__name__
         return args, kwargs
 
     def __hook_insert_origin_save_dataframe(self, *args, **kwargs):
+        logger.info("Datalake dataframe save pre-hook.", tags=LogTags.HOOK)
         dataframe = kwargs.get("dataframe")
         dataframe["instance_id"] = self.instance_id
         dataframe["instance_type"] = self.instance_type.__name__
         kwargs["dataframe"] = dataframe
         return args, kwargs
 
     def __hook_transform_from_custom_resource_type(self, *args, **kwargs):
+        logger.info("Transform from custom type pre-hook.", tags=LogTags.HOOK)
         resource_type = kwargs["resource_type"]
         if resource_type and hasattr(self.custom_types, resource_type.__name__):
             kwargs["resource_type"] = ComponentObject
             kwargs["component_id"] = self.instance_id
             kwargs["type"] = resource_type.__name__
         return args, kwargs
 
     def __hook_transform_from_custom_instances(self, *args, **kwargs):
+        logger.info("Transform from custom instances pre-hook.", tags=LogTags.HOOK)
         instance = kwargs["instance"]
         if getattr(self.custom_types, type(instance).__name__, None):
             parsed_instance = ComponentObject(
                 component_id=self.instance_id,
                 type=type(instance).__name__,
                 **self.unparse_parameters(instance)
             )
             kwargs["instance"] = parsed_instance
         return args, kwargs
 
     def __hook_transform_to_custom_instances(
         self, result: Union[BaseModel, List[BaseModel]]
     ):
+        logger.info("Transform to custom instances pre-hook.", tags=LogTags.HOOK)
         parsed_result = []
         convert_to_list = not isinstance(result, list)
         result = [result] if convert_to_list else result
         for object in result:
             if isinstance(object, ComponentObject):
                 custom_object_data: List[InputParameter] = object.data
                 custom_object_data.extend([
@@ -231,33 +243,34 @@
         for binding in self.bindings:
             binding_function = getattr(self, binding.name)
             binding_model = getattr(spmodels, binding.object_type, ComponentObject)
             binding_event_name = binding_model.get_event_name(
                 binding.object_type,
                 binding.object_action
             )
-            logger.info(f"Binding event: {binding_event_name}")
+            logger.info("Binding event: %s.", binding_event_name, tags=LogTags.BINDING)
             binding_handler = self.__handle_native_object_trigger
             if binding_model == ComponentObject:
                 binding_handler = self.__handle_component_object_trigger
             if binding_model == SetPoint:
                 binding_handler = self.__handle_setpoint_trigger
 
             self.communication_client.bind(
                 binding_event_name,
                 partial(
                     binding_handler,
                     binding_function,
                     binding.object_type
                 )
             )
-            logger.info(f"Binded event: {binding_event_name}")
+            logger.info("Binded event: %s", binding_event_name, tags=LogTags.BINDING)
 
     def __handle_setpoint_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
         try:
+            logger.debug("Setpoint triggered.", tags=LogTags.SETPOINT)
             object_event = SetPointCreateEvent.parse_raw(data)
             setpoint = object_event.data
             response_status = SetPointResponseStatus(binding_function(setpoint))
             if response_status == SetPointResponseStatus.IGNORE:
                 return
 
             setpoint.responses = [
@@ -265,30 +278,30 @@
                     component=self.instance_id,
                     status=response_status,
                 )
             ]
             setpoint_callback_event = SetPointUpdateEvent(data=setpoint)
             self.communication_client.trigger(setpoint_callback_event)
         except Exception as e:
-            logger.error(f"Error while handling setpoint create: {e}")
-            logger.exception(e)
+            logger.error("Error while handling setpoint create: %s", e, exc_info=True, tags=LogTags.SETPOINT)
 
     def __handle_native_object_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
         assert self.bindings, "Please define .bindings to start."
         try:
+            logger.info("Binding for native object of type %s triggered.", binding_object_type, tags=LogTags.BINDING)
             object_event = CommunicationEvent.parse_raw(data)
             object_model = getattr(spmodels, binding_object_type)
             binding_kwargs = object_model(**object_event.data)
             binding_function(binding_kwargs)
         except Exception as e:
-            logger.error(f"Error while handling native object trigger: {e}")
-            logger.exception(e)
+            logger.error("Error while handling native object trigger: %s", e, exc_info=True, tags=LogTags.BINDING)
 
     def __handle_component_object_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
         assert self.bindings, "Please define .bindings to start."
+        logger.info("Binding for component object of type %s triggered.", binding_object_type, tags=LogTags.BINDING)
         component_object_event = CommunicationEvent.parse_raw(data)
         component_object: ComponentObject = ComponentObject(**component_object_event.data)
         custom_object_data = component_object.data
         custom_object_data.extend([
             InputParameter(name=key, value=getattr(component_object, key))
             for key in CustomType._reserved_names
         ])
@@ -298,34 +311,37 @@
         binding_function(binding_kwargs)
 
     def __handle_component_command_trigger(self, data: str):
         assert self.commands, "Please define .commands to start accepting request."
         component_command_event = ComponentCommandTriggerEvent.parse_raw(data)
         component_command: ComponentCommand = component_command_event.data
         command: Command = component_command.command
+        logger.info("Binding for component command '%s' triggered.", command.name, tags=LogTags.COMMAND)
         try:
             command_function = getattr(self, command.name)
             command_kwargs_model = getattr(self.commands, command.name)
             parsed_command_kwargs = self.parse_parameters(command.dict()["fields"])
             command_kwargs = command_kwargs_model(**parsed_command_kwargs)
             # .dict is not keeping the models of subkeys
             command_kwargs = {
                 str(field): getattr(command_kwargs, str(field)) for field in command_kwargs.__fields__
             }
             component_command.response.return_value = str(command_function(**command_kwargs))
             component_command.status = ComponentCommandStatus.SUCCESS
         except Exception as e:
+            logger.error("Error while handling component command trigger: %s", e, exc_info=True, tags=LogTags.COMMAND)
             component_command.response.error_detail = str(e)
             component_command.status = ComponentCommandStatus.ERROR
         component_command_callback_event = ComponentCommandUpdateEvent(data=component_command)
         self.communication_client.trigger(component_command_callback_event)
 
 
 class ParametersMixin:
     def unparse_parameters(self, instance: Dict) -> List[Dict]:
+        logger.debug("Unparsing parameters for an instance of %s", type(instance).__name__, tags=LogTags.PARAMETER)
         custom_type = getattr(self.custom_types, type(instance).__name__, None)
         if custom_type is None:
             raise NotImplementedError
         reserved_parameters = {k: v for k, v in instance.dict().items() if k in CustomType._reserved_names}
         custom_parameters = {k: v for k, v in instance.dict().items() if k not in CustomType._reserved_names}
         fields = []
         for key, obj in custom_parameters.items():
@@ -348,14 +364,15 @@
                     depends_on=field.depends_on,
                     sensitive=field.sensitive,
                 )
             )
         return {"data": fields, **reserved_parameters}
 
     def parse_parameters(self, parameters: List[Dict]) -> Dict:
+        logger.debug("Parsing parameters %s", parameters, tags=LogTags.PARAMETER)
         parameters = self._fetch_and_reload_component_objects_parameters(parameters)
         object_ids: Dict[str, Dict[str, List]] = self._get_object_ids(parameters)
         objects: Dict[str, BaseModel] = self._fetch_objects(object_ids)
         parameters = self._reload_parameters(parameters, objects=objects)
         transformed_parameters = self._transform_parameters(parameters)
         return transformed_parameters
```

### Comparing `splight-lib-2.2.7/splight_lib/encryption.py` & `splight-lib-2.2.8/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/execution.py` & `splight-lib-2.2.8/splight_lib/execution.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,18 @@
     Thread as DefaultThread,
     Event,
     Lock,
 )
 from subprocess import Popen as DefaultPopen
 from functools import wraps
 from splight_abstract.client.abstract import AbstractClient
-from splight_lib import logging
+from splight_lib.logging import getLogger, LogTags
 
 
-logger = logging.getLogger()
-
+logger = getLogger(dev=True)
 
 class Empty(object):
     pass
 
 
 class Task:
     """A periodic task for the scheduler."""
@@ -273,14 +272,15 @@
 class ExecutionClient(AbstractClient):
     def __init__(self, *args, **kwargs):
         self.processes: List[Thread] = []
         self.threads: List[Popen] = []
 
         self._register_exit_functions()
         super(ExecutionClient, self).__init__(*args, **kwargs)
+        logger.info("Execution client initialized.", tags=LogTags.RUNTIME)
 
     def _register_exit_functions(self) -> None:
         excepthook = sys.excepthook
 
         def wrap_excepthook(type, value, traceback):
             self.terminate_all()
             excepthook(type, value, traceback)
@@ -292,14 +292,16 @@
         self.terminate_all()
 
     def terminate_all(self) -> None:
         for p in self.processes:
             p.terminate()
 
     def start(self, job=Union[Popen, Thread, Task]):
+        logger.info("Executing new job.", tags=LogTags.RUNTIME)
+
         if isinstance(job, Popen):
             return self._start_process(job)
         if isinstance(job, Thread):
             return self._start_thread(job)
         if isinstance(job, Task):
             return self._start_task(job)
 
@@ -308,32 +310,32 @@
             raise NotImplementedError
         if isinstance(job, Thread):
             raise NotImplementedError
         if isinstance(job, Task):
             return self._stop_task(job)
 
     def _start_process(self, job: Popen) -> None:
-        logger.debug(f"Starting process {job}")
+        logger.debug("Starting process %s", job, tags=LogTags.RUNTIME)
         self.processes.append(job)
         return
 
     def _start_thread(self, job: Thread) -> None:
-        logger.debug(f"Starting Thread {job}")
+        logger.debug("Starting Thread %s", job, tags=LogTags.RUNTIME)
         self.threads.append(job)
         job.start()
         return
 
     def _start_task(self, job: Task) -> None:
-        logger.debug(f"Starting Task {job}")
+        logger.debug("Starting Task %s", job, tags=LogTags.RUNTIME)
         if not getattr(self, '_scheduler', None):
             # Instantiate and start Scheduler thread
             self._scheduler = Scheduler()
             self._start_thread(Thread(target=self._scheduler.start))
 
         return self._scheduler.schedule(job)
 
     def _stop_task(self, job: Task) -> None:
-        logger.debug(f"Stopping Task {job}")
+        logger.debug("Stopping Task %s", job, tags=LogTags.RUNTIME)
         return self._scheduler.unschedule(job)
 
     def healthcheck(self):
         return all([p.is_alive() or p.exit_ok() for p in self.processes + self.threads])
```

### Comparing `splight-lib-2.2.7/splight_lib/logging.py` & `splight-lib-2.2.8/splight_lib/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 import logging
 import time
 import os
 import sys
-from typing import Dict, Optional
 from concurrent_log_handler import ConcurrentRotatingFileHandler
+from typing import Dict, Optional
+from enum import auto
+from strenum import UppercaseStrEnum
+
 
+class LogTags(UppercaseStrEnum):
+    RUNTIME = auto()
+    BINDING = auto()
+    COMMUNICATION = auto()
+    INDEX = auto()
+    SECRET = auto()
+    HOOK = auto()
+    SETPOINT = auto()
+    COMMAND = auto()
+    PARAMETER = auto()
+    COMPONENT = auto() # TODO: not used yet.
+    DATABASE = auto()
+    DATALAKE = auto()
+    CACHE = auto()
 
 TAGS_KEY = "tags"
 
 
 class SplightFormatter(logging.Formatter):
     DEFAULT_FMT: str = "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
```

### Comparing `splight-lib-2.2.7/splight_lib/restclient/client.py` & `splight-lib-2.2.8/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/restclient/exceptions.py` & `splight-lib-2.2.8/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/restclient/types.py` & `splight-lib-2.2.8/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/settings.py` & `splight-lib-2.2.8/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib/webhook.py` & `splight-lib-2.2.8/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.2.8/splight_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.7
+Version: 2.2.8
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.7/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.2.8/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/__init__.py` & `splight-lib-2.2.8/splight_models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/alert.py` & `splight-lib-2.2.8/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/blockchain.py` & `splight-lib-2.2.8/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/communication/context.py` & `splight-lib-2.2.8/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/communication/events.py` & `splight-lib-2.2.8/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/component.py` & `splight-lib-2.2.8/splight_models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/constants.py` & `splight-lib-2.2.8/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/datalake.py` & `splight-lib-2.2.8/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/deployment.py` & `splight-lib-2.2.8/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/exception.py` & `splight-lib-2.2.8/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/file.py` & `splight-lib-2.2.8/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/hub.py` & `splight-lib-2.2.8/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/notification.py` & `splight-lib-2.2.8/splight_models/notification.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/query.py` & `splight-lib-2.2.8/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/setpoint.py` & `splight-lib-2.2.8/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/user.py` & `splight-lib-2.2.8/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/variable.py` & `splight-lib-2.2.8/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.7/splight_models/webhook.py` & `splight-lib-2.2.8/splight_models/webhook.py`

 * *Files identical despite different names*

