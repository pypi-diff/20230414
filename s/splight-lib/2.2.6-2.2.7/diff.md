# Comparing `tmp/splight-lib-2.2.6.tar.gz` & `tmp/splight-lib-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.2.6.tar", last modified: Wed Apr 12 17:58:11 2023, max compression
+gzip compressed data, was "splight-lib-2.2.7.tar", last modified: Fri Apr 14 17:15:49 2023, max compression
```

## Comparing `splight-lib-2.2.6.tar` & `splight-lib-2.2.7.tar`

### file list

```diff
@@ -1,141 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.143168 splight-lib-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:10.000000 splight-lib-2.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 17:58:11.143168 splight-lib-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 17:58:10.000000 splight-lib-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 17:58:10.000000 splight-lib-2.2.6/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:58:11.143168 splight-lib-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 17:58:10.000000 splight-lib-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.127167 splight-lib-2.2.6/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.131168 splight-lib-2.2.6/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.135168 splight-lib-2.2.6/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.135168 splight-lib-2.2.6/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.135168 splight-lib-2.2.6/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.135168 splight-lib-2.2.6/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.139168 splight-lib-2.2.6/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.139168 splight-lib-2.2.6/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.139168 splight-lib-2.2.6/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/restclient/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.135168 splight-lib-2.2.6/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 17:58:11.000000 splight-lib-2.2.6/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.143168 splight-lib-2.2.6/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:11.143168 splight-lib-2.2.6/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-12 17:58:10.000000 splight-lib-2.2.6/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:48.000000 splight-lib-2.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 17:15:49.161148 splight-lib-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 17:15:48.000000 splight-lib-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 17:15:48.000000 splight-lib-2.2.7/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:15:49.161148 splight-lib-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 17:15:48.000000 splight-lib-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.153148 splight-lib-2.2.7/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.157148 splight-lib-2.2.7/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 17:15:49.000000 splight-lib-2.2.7/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:15:49.161148 splight-lib-2.2.7/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 17:15:48.000000 splight-lib-2.2.7/splight_models/webhook.py
```

### Comparing `splight-lib-2.2.6/PKG-INFO` & `splight-lib-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.6
+Version: 2.2.7
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.6/remote_splight_lib/communication/client.py` & `splight-lib-2.2.7/remote_splight_lib/communication/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/remote_splight_lib/database/classmap.py` & `splight-lib-2.2.7/remote_splight_lib/database/classmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from splight_models import (
     Alert,
     AlertCondition,
     Asset,
     Attribute,
     File,
-    Edge,
-    Graph,
     Component,
     Notification,
     Query,
-    Node,
     BlockchainContract,
     HubComponent,
     ComponentObject,
     ComponentCommand,
     Secret,
     SetPoint,
 )
@@ -31,29 +28,20 @@
     },
     Asset: {
         "path": "v2/engine/assets"
     },
     Attribute: {
         "path": "v2/engine/attributes"
     },
-    Edge: {
-        "path": "v2/engine/graph/edges"
-    },
     File: {
         "path": "v2/engine/files"
     },
-    Graph: {
-        "path": "v2/engine/graph/graphs"
-    },
     Notification: {
         "path": "v2/account/notifications"
     },
-    Node: {
-        "path": "v2/engine/graph/nodes"
-    },
     BlockchainContract: {
         "path": "v2/backoffice/blockchain/contracts"
     },
     ComponentObject: {
         "path": "v2/engine/component/objects"
     },
     ComponentCommand: {
```

### Comparing `splight-lib-2.2.6/remote_splight_lib/database/client.py` & `splight-lib-2.2.7/remote_splight_lib/database/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/remote_splight_lib/datalake/client.py` & `splight-lib-2.2.7/remote_splight_lib/datalake/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/remote_splight_lib/hub/client.py` & `splight-lib-2.2.7/remote_splight_lib/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/remote_splight_lib/settings.py` & `splight-lib-2.2.7/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/setup.py` & `splight-lib-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 dependency_links = [
     # External repoitories different from pypi
 ]
 
 setup(
     name='splight-lib',
-    version='2.2.6',
+    version='2.2.7',
     author='Splight',
     author_email='factory@splight-ae.com',
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.2.6/splight_abstract/auth/abstract.py` & `splight-lib-2.2.7/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/auth/exceptions.py` & `splight-lib-2.2.7/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/cache/abstract.py` & `splight-lib-2.2.7/splight_abstract/cache/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/client/abstract.py` & `splight-lib-2.2.7/splight_abstract/client/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/client/filter.py` & `splight-lib-2.2.7/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/client/hooks.py` & `splight-lib-2.2.7/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/communication/abstract.py` & `splight-lib-2.2.7/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/database/abstract.py` & `splight-lib-2.2.7/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/datalake/abstract.py` & `splight-lib-2.2.7/splight_abstract/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/deployment/abstract.py` & `splight-lib-2.2.7/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/endpoints/__init__.py` & `splight-lib-2.2.7/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/hub/abstract.py` & `splight-lib-2.2.7/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_abstract/storage/abstract.py` & `splight-lib-2.2.7/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/auth/mac_auth.py` & `splight-lib-2.2.7/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/database/classmap.py` & `splight-lib-2.2.7/splight_lib/client/database/classmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from splight_models import (
     Alert,
     AlertCondition,
     Asset,
     Attribute,
     File,
-    Edge,
-    Graph,
     Component,
     Notification,
     Query,
-    Node,
     BlockchainContract,
     HubComponent,
     ComponentObject,
     ComponentCommand,
     Secret,
     SetPoint,
 )
@@ -31,29 +28,20 @@
     },
     Asset: {
         "path": "v2/engine/assets"
     },
     Attribute: {
         "path": "v2/engine/attributes"
     },
-    Edge: {
-        "path": "v2/engine/graph/edges"
-    },
     File: {
         "path": "v2/engine/files"
     },
-    Graph: {
-        "path": "v2/engine/graph/graphs"
-    },
     Notification: {
         "path": "v2/account/notifications"
     },
-    Node: {
-        "path": "v2/engine/graph/nodes"
-    },
     BlockchainContract: {
         "path": "v2/backoffice/blockchain/contracts"
     },
     ComponentObject: {
         "path": "v2/engine/component/objects"
     },
     ComponentCommand: {
```

### Comparing `splight-lib-2.2.6/splight_lib/client/database/local_client.py` & `splight-lib-2.2.7/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/database/remote_client.py` & `splight-lib-2.2.7/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/datalake/local_client.py` & `splight-lib-2.2.7/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.2.7/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/exceptions.py` & `splight-lib-2.2.7/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/file_handler.py` & `splight-lib-2.2.7/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/filter.py` & `splight-lib-2.2.7/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/client/settings.py` & `splight-lib-2.2.7/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/component/abstract.py` & `splight-lib-2.2.7/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/encryption.py` & `splight-lib-2.2.7/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/execution.py` & `splight-lib-2.2.7/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/logging.py` & `splight-lib-2.2.7/splight_lib/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/restclient/client.py` & `splight-lib-2.2.7/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/restclient/exceptions.py` & `splight-lib-2.2.7/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/restclient/types.py` & `splight-lib-2.2.7/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/settings.py` & `splight-lib-2.2.7/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib/webhook.py` & `splight-lib-2.2.7/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.2.7/splight_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.6
+Version: 2.2.7
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.6/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.2.7/splight_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 splight_models/component.py
 splight_models/constants.py
 splight_models/credential.py
 splight_models/datalake.py
 splight_models/deployment.py
 splight_models/exception.py
 splight_models/file.py
-splight_models/graph.py
 splight_models/hub.py
 splight_models/namespace.py
 splight_models/notification.py
 splight_models/query.py
 splight_models/secret.py
 splight_models/setpoint.py
 splight_models/severity.py
```

### Comparing `splight-lib-2.2.6/splight_models/__init__.py` & `splight-lib-2.2.7/splight_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from splight_models.blockchain import *
 from splight_models.communication import *
 from splight_models.channel import *
 from splight_models.credential import *
 from splight_models.datalake import *
 from splight_models.deployment import *
 from splight_models.file import *
-from splight_models.graph import *
 from splight_models.hub import *
 from splight_models.namespace import *
 from splight_models.notification import *
 from splight_models.query import *
 from splight_models.component import *
 from splight_models.user import *
 from splight_models.variable import *
```

### Comparing `splight-lib-2.2.6/splight_models/alert.py` & `splight-lib-2.2.7/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/blockchain.py` & `splight-lib-2.2.7/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/communication/context.py` & `splight-lib-2.2.7/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/communication/events.py` & `splight-lib-2.2.7/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/component.py` & `splight-lib-2.2.7/splight_models/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     ComponentType
 )
 from splight_models.asset import Asset
 from splight_models.attribute import Attribute
 from splight_models.base import SplightBaseModel
 from splight_models.file import File
 from splight_models.datalake import DatalakeModel
-from splight_models.graph import Graph
 from splight_models.query import Query
 from splight_models import EventActions, EventNames, CommunicationEvent
 from datetime import datetime
 from enum import Enum, auto
 from typing import Type, List, Dict, Tuple, Optional, Any, Union
 from pydantic import BaseModel, create_model, Field, AnyUrl, ValidationError, validator
 from copy import copy
@@ -219,15 +218,14 @@
 }
 
 DATABASE_TYPES = {
     "Component": Component,
     "Asset": Asset,
     "Attribute": Attribute,
     "File": File,
-    "Graph": Graph,
     "Query": Query,
 }
 
 
 SIMPLE_TYPES = list(NATIVE_TYPES.keys()) + list(DATABASE_TYPES.keys())
 
 
@@ -308,15 +306,15 @@
             multiple = getattr(field, "multiple", False)
             required = getattr(field, "required", True)
 
             if choices:
                 validators.update({
                     "choices_validator": validator(
                         field.name, pre=True, allow_reuse=True
-                     )(choices_validator)
+                    )(choices_validator)
                 })
 
             if multiple:
                 type = List[type]
 
             value = ...
             if not required:
```

### Comparing `splight-lib-2.2.6/splight_models/constants.py` & `splight-lib-2.2.7/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/datalake.py` & `splight-lib-2.2.7/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/deployment.py` & `splight-lib-2.2.7/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/file.py` & `splight-lib-2.2.7/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/hub.py` & `splight-lib-2.2.7/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/notification.py` & `splight-lib-2.2.7/splight_models/notification.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 class TargetType(str, Enum):
     component = 'Component'
     dashboard = 'Dashboard'
     asset = 'Asset'
     attribute = 'Attribute'
     file_ = 'File'
-    graph = 'Graph'
     query = 'Query'
 
 
 class Notification(SplightBaseModel):
     id: Optional[str]
     message: str
     seen: bool = False
```

### Comparing `splight-lib-2.2.6/splight_models/query.py` & `splight-lib-2.2.7/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/setpoint.py` & `splight-lib-2.2.7/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/user.py` & `splight-lib-2.2.7/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/variable.py` & `splight-lib-2.2.7/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.6/splight_models/webhook.py` & `splight-lib-2.2.7/splight_models/webhook.py`

 * *Files identical despite different names*

