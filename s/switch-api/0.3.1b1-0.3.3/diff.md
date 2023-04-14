# Comparing `tmp/switch_api-0.3.1b1.tar.gz` & `tmp/switch_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.3.1b1.tar", last modified: Thu Mar 23 01:12:23 2023, max compression
+gzip compressed data, was "switch_api-0.3.3.tar", last modified: Fri Apr 14 07:05:02 2023, max compression
```

## Comparing `switch_api-0.3.1b1.tar` & `switch_api-0.3.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.343237 switch_api-0.3.1b1/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)    22810 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    24086 2023-03-23 01:12:23.343237 switch_api-0.3.1b1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-03-23 01:12:23.343237 switch_api-0.3.1b1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1352 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (122)     1364 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3595 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15497 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)     1030 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7258 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)     1545 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26221 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    80188 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.343237 switch_api-0.3.1b1/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.343237 switch_api-0.3.1b1/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-03-23 01:12:09.000000 switch_api-0.3.1b1/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-23 01:12:23.339237 switch_api-0.3.1b1/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    24086 2023-03-23 01:12:23.000000 switch_api-0.3.1b1/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-03-23 01:12:23.000000 switch_api-0.3.1b1/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-23 01:12:23.000000 switch_api-0.3.1b1/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-03-23 01:12:23.000000 switch_api-0.3.1b1/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-03-23 01:12:23.000000 switch_api-0.3.1b1/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-04-14 07:04:48.000000 switch_api-0.3.3/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    25085 2023-04-14 07:04:48.000000 switch_api-0.3.3/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-04-14 07:04:48.000000 switch_api-0.3.3/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-04-14 07:04:48.000000 switch_api-0.3.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    26359 2023-04-14 07:05:02.709312 switch_api-0.3.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-04-14 07:04:48.000000 switch_api-0.3.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-04-14 07:04:48.000000 switch_api-0.3.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-14 07:05:02.713312 switch_api-0.3.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-04-14 07:04:48.000000 switch_api-0.3.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1358 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15497 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7627 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3051 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    89587 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    26359 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.3.1b1/HISTORY.md` & `switch_api-0.3.3/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,88 @@
 # History
 
-## 0.3.1-beta1
+## 0.3.3
 
 ### Added
-- Switch Python Extensions support
-  - This stil work in progress, documentation on usage will be updated in a future release.
+- New `upsert_device_sensors_ext` method to the `integration` module.
+  - Compared to existing `upsert_device_sensors` following are supported:
+    - Installation Code or Installation Id may be provided
+      - BUT cannot provide mix of the two, all must have either code or id and not both.
+    - DriverClassName
+    - DriverDeviceType
+    - PropertyName
+### Added Feature - Switch Python Extensions
+- Extensions may be used in Task Insights and Switch Guides for code reuse
+- Extensions maybe located in any directory structure within the repo where the usage scripts are located
+- May need to adjust your environment to detect the files if you're not running a project environment
+  - Tested on VSCode and PyCharm - contact Switch Support for issues.
+
+#### Extensions Usage
+```python
+import switch_api as sw
+
+# Single import line per extension
+from extensions.my_extension import MyExtension
+
+@sw.extensions.provide(field="some_extension")
+class MyTask:
+    some_extension: MyExtension
+
+if __name__ == "__main__":
+    task = MyTask()
+    task.some_extension.do_something()
+```
+
+#### Extensions Registration
+```python
+import uuid
+import switch_api as sw
+
+class SimpleExtension(sw.extensions.ExtensionTask):
+    @property
+    def id(self) -> uuid.UUID:
+        # Unique ID for the extension.
+        # Generate in CLI using:
+        #   python -c 'import uuid; print(uuid.uuid4())'
+        return '46759cfe-68fa-440c-baa9-c859264368db'
+    
+    @property
+    def description(self) -> str:
+        return 'Extension with a simple get_name function.'
+    
+    @property
+    def author(self) -> str:
+        return 'Amruth Akoju'
+    
+    @property
+    def version(self) -> str:
+        return '1.0.1'
+
+    def get_name(self):
+        return "Simple Extension"
+
+# Scaffold code for registration. This will not be persisted in the extension.
+if __name__ == '__main__':
+    task = SimpleExtension()
+
+    api_inputs = sw.initialize(api_project_id='<portfolio-id>')
+
+    # Usage test
+    print(task.get_name())
+
+    # =================================================================
+    # REGISTER TASK & DATAFEED ========================================
+    # =================================================================
+    register = sw.pipeline.Automation.register_task(api_inputs, task)
+    print(register)
+
+```
+
+### Updated
+- get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
```

### Comparing `switch_api-0.3.1b1/LICENCE` & `switch_api-0.3.3/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/PKG-INFO` & `switch_api-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_api
-Version: 0.3.1b1
+Version: 0.3.3
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,19 +34,93 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
-## 0.3.1-beta1
+## 0.3.3
 
 ### Added
-- Switch Python Extensions support
-  - This stil work in progress, documentation on usage will be updated in a future release.
+- New `upsert_device_sensors_ext` method to the `integration` module.
+  - Compared to existing `upsert_device_sensors` following are supported:
+    - Installation Code or Installation Id may be provided
+      - BUT cannot provide mix of the two, all must have either code or id and not both.
+    - DriverClassName
+    - DriverDeviceType
+    - PropertyName
+### Added Feature - Switch Python Extensions
+- Extensions may be used in Task Insights and Switch Guides for code reuse
+- Extensions maybe located in any directory structure within the repo where the usage scripts are located
+- May need to adjust your environment to detect the files if you're not running a project environment
+  - Tested on VSCode and PyCharm - contact Switch Support for issues.
+
+#### Extensions Usage
+```python
+import switch_api as sw
+
+# Single import line per extension
+from extensions.my_extension import MyExtension
+
+@sw.extensions.provide(field="some_extension")
+class MyTask:
+    some_extension: MyExtension
+
+if __name__ == "__main__":
+    task = MyTask()
+    task.some_extension.do_something()
+```
+
+#### Extensions Registration
+```python
+import uuid
+import switch_api as sw
+
+class SimpleExtension(sw.extensions.ExtensionTask):
+    @property
+    def id(self) -> uuid.UUID:
+        # Unique ID for the extension.
+        # Generate in CLI using:
+        #   python -c 'import uuid; print(uuid.uuid4())'
+        return '46759cfe-68fa-440c-baa9-c859264368db'
+    
+    @property
+    def description(self) -> str:
+        return 'Extension with a simple get_name function.'
+    
+    @property
+    def author(self) -> str:
+        return 'Amruth Akoju'
+    
+    @property
+    def version(self) -> str:
+        return '1.0.1'
+
+    def get_name(self):
+        return "Simple Extension"
+
+# Scaffold code for registration. This will not be persisted in the extension.
+if __name__ == '__main__':
+    task = SimpleExtension()
+
+    api_inputs = sw.initialize(api_project_id='<portfolio-id>')
+
+    # Usage test
+    print(task.get_name())
+
+    # =================================================================
+    # REGISTER TASK & DATAFEED ========================================
+    # =================================================================
+    register = sw.pipeline.Automation.register_task(api_inputs, task)
+    print(register)
+
+```
+
+### Updated
+- get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
```

### Comparing `switch_api-0.3.1b1/README.md` & `switch_api-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/setup.py` & `switch_api-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.3.1-beta1",
+    version="0.3.3",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus', 'msal>=1.11.0'],
     python_requires=">=3.8.*",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Other Audience',
```

### Comparing `switch_api-0.3.1b1/switch_api/__init__.py` & `switch_api-0.3.3/switch_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.3.1-beta1"
+__version__ = "0.3.3"
```

### Comparing `switch_api-0.3.1b1/switch_api/_authentication/_authentication.py` & `switch_api-0.3.3/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.3.3/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.3.3/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/_utils/_constants.py` & `switch_api-0.3.3/switch_api/_utils/_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 ACCOUNT = Literal['SwitchStorage', 'SwitchContainer', 'Argus', 'DataIngestion', 'GatewayMqttStorage']
 
 DATA_INGESTION_CONTAINER = Literal['data-ingestion-adx', 'data-ingestion-timeseries-adx']
 
 QUERY_LANGUAGE = Literal['sql', 'kql']
 
+RESPONSE_TYPE = Literal['dataframe', 'json', 'string']
+
 ERROR_TYPE = Literal['DateTime', 'MissingDevices', 'NonNumeric', 'MissingRequiredField(s)', 'MissingSite(s)',
                      'DuplicateRecords', 'MissingSensors', 'UnableToReadFile', 'InvalidFileType', 'InvalidInputSettings']
 
 PROCESS_STATUS = Literal['ActionRequired', 'Failed']
 
 MAPPING_ENTITIES = Literal['Installations', 'Devices/Sensors', 'Readings', 'Work Orders']
```

### Comparing `switch_api-0.3.1b1/switch_api/_utils/_platform.py` & `switch_api-0.3.3/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/_utils/_utils.py` & `switch_api-0.3.3/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/analytics/__init__.py` & `switch_api-0.3.3/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/analytics/analytics.py` & `switch_api-0.3.3/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/cache/cache.py` & `switch_api-0.3.3/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/dataset/__init__.py` & `switch_api-0.3.3/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/dataset/dataset.py` & `switch_api-0.3.3/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/error_handlers/__init__.py` & `switch_api-0.3.3/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/error_handlers/error_handlers.py` & `switch_api-0.3.3/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/extensions/__init__.py` & `switch_api-0.3.3/switch_api/extensions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Switch Automation Pty Ltd. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
-A module for providing for extensions to tasks.
+A module for providing support for extensions to tasks.
 Allows sharing of code between tasks.
 """
 
 from .extensions import (provide, get_extension_fields, replace_extension_imports, 
                          replace_extensions_imports, tokenize_extension_imports)
 
 from .field_meta import FieldMeta
```

### Comparing `switch_api-0.3.1b1/switch_api/extensions/extensions.py` & `switch_api-0.3.3/switch_api/extensions/extensions.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,28 +28,35 @@
         The decorator function.
 
     """
 
     def decorator(cls):
         if not cls or not isinstance(cls, type):
             raise TypeError("The provided class must be a valid class")
+        
+        if issubclass(cls, ExtensionTask):
+            raise TypeError(f"""
+                Extensions cannot be provided to other extensions at this time. 
+                Please check for nested extensions in class '{cls.__name__}'.
+                Nested Extensions are extensions which depend on other extensions.
+                """)
 
         # Load the module from the local file system
         type_hints = get_type_hints(cls)
         
         if isinstance(field, str):
             __provide(cls, type_hints, field)
         elif isinstance(field, list):
             field_list = filter(lambda x: x and isinstance(x, str), field)
             for f in field_list:
                 __provide(cls, type_hints, f)
 
         return cls
 
-    def __provide(cls, type_hints, inner_field):
+    def __provide(cls, type_hints: dict[str, any], inner_field: str):
         if inner_field not in type_hints:
             raise TypeError(f"Provided field '{inner_field}' must exist as a field on the class {cls.__name__}")
         
         module_type = type_hints[inner_field]
 
         if not issubclass(module_type, ExtensionTask):
             raise TypeError(f"Provided field '{inner_field}' must have a return type that inherits from ExtensionTask")
```

### Comparing `switch_api-0.3.1b1/switch_api/extensions/field_meta.py` & `switch_api-0.3.3/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/extensions/helpers.py` & `switch_api-0.3.3/switch_api/extensions/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 from typing import List
 
 HasExtensionClsAttributeName = '__has_sw_extension_support__'
+"""The name of the attribute that is added to a class that has extensions."""
 
 def __get_code(cls):
     """
     Get the code used to create the class.
 
     (Code was taken from sw.pipeline.Automation._get_task_code function)
```

### Comparing `switch_api-0.3.1b1/switch_api/extensions/pipeline.py` & `switch_api-0.3.3/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/initialize.py` & `switch_api-0.3.3/switch_api/initialize.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/integration/__init__.py` & `switch_api-0.3.3/switch_api/integration/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 A module for integrating asset creation, asset updates, data ingestion, etc into the Switch Automation Platform.
 """
 
-from .integration import (upsert_data, upsert_sites, upsert_workorders, upsert_device_sensors,
+from .integration import (upsert_data, upsert_sites, upsert_workorders, upsert_device_sensors, upsert_device_sensors_ext,
                           upsert_timeseries_ds, replace_data, append_data, upsert_file_row_count,
                           upsert_discovered_records, upsert_timeseries, upsert_tags, upsert_device_metadata)
 
 from .helpers import (get_sites, get_tag_groups, get_metadata_keys, get_data, get_device_sensors, get_templates,
                       get_units_of_measure, get_states_by_country, get_operation_state, get_equipment_classes,
                       load_data, get_timezones)
 
-__all__ = ['upsert_data', 'upsert_sites', 'upsert_workorders', 'upsert_device_sensors', 'upsert_timeseries_ds',
+__all__ = ['upsert_data', 'upsert_sites', 'upsert_workorders', 'upsert_device_sensors', 'upsert_device_sensors_ext', 'upsert_timeseries_ds',
            'replace_data', 'append_data', 'get_sites', 'get_tag_groups', 'get_metadata_keys', 'get_data',
            'get_device_sensors', 'get_templates', 'get_units_of_measure', 'get_states_by_country',
            'get_operation_state', 'get_equipment_classes', 'load_data', 'upsert_file_row_count',
            'upsert_discovered_records', 'upsert_timeseries', 'upsert_tags', 'upsert_device_metadata', 'get_timezones']
```

### Comparing `switch_api-0.3.1b1/switch_api/integration/_utils.py` & `switch_api-0.3.3/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/integration/helpers.py` & `switch_api-0.3.3/switch_api/integration/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import pandas
 import pandas as pd
 import requests
 import logging
 import uuid
 from typing import Union
 from .._utils._constants import QUERY_LANGUAGE
+from .._utils._constants import RESPONSE_TYPE
 from .._utils._utils import ApiInputs, _column_name_cap
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 consoleHandler = logging.StreamHandler(stream=sys.stdout)
 consoleHandler.setLevel(logging.INFO)
 
@@ -334,15 +335,15 @@
             df_master.rename(columns={"InstallationID": "InstallationId", "ObjectPropertyID": "ObjectPropertyId"},
                              inplace=True)
             return df_master
 
     return df_master
 
 
-def get_data(query_text, api_inputs: ApiInputs, query_language: QUERY_LANGUAGE = "sql"):
+def get_data(query_text, api_inputs: ApiInputs, query_language: QUERY_LANGUAGE = "sql", response_type: RESPONSE_TYPE = 'dataframe'):
     """Retrieve data.
 
     Parameters
     ----------
     query_text : str
         SQL statement used to retrieve data.
     api_inputs : ApiInputs
@@ -380,17 +381,20 @@
         logger.error("API Call was not successful. Response Status: %s. Reason: %s.", response.status_code,
                      response.reason)
         return response_status
     elif len(response.text) == 0:
         logger.error('No data returned for this API call. %s', response.request.url)
         return response_status
 
-    df = pandas.read_json(response.text)
-
-    return df
+    if response_type == 'dataframe':
+        return pandas.read_json(response.text)
+    elif response_type == 'json':
+        return json.loads(response.text)
+    else:
+        return response.text
 
 
 def get_states_by_country(api_inputs: ApiInputs, country: str):
     """Get list of States for selected country.
 
         Parameters
         ----------
```

### Comparing `switch_api-0.3.1b1/switch_api/integration/integration.py` & `switch_api-0.3.3/switch_api/integration/integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -386,14 +386,190 @@
     _upsert_entities_affected_count(api_inputs=api_inputs,
                                     entities_affected_count=upsert_response_df['SensorCount'].sum())
     _adx_support(api_inputs=api_inputs, payload_type='Sensors')
 
     logger.info("Ingestion Complete. ")
     return upsert_response_status_list, upsert_response_df
 
+@_with_func_attrs(df_required_columns=['DriverClassName', 'DriverDeviceType', 'PropertyName', 'DeviceCode', 'DeviceName', 'SensorName', 'SensorTemplate',
+                        'SensorUnitOfMeasure', 'EquipmentClass', 'EquipmentLabel'])
+def upsert_device_sensors_ext(df: pandas.DataFrame, api_inputs: ApiInputs, tag_columns: list = None,
+                          metadata_columns: list = None, save_additional_columns_as_slices: bool = False):
+    """Upsert device(s) and sensor(s)
+
+    Required fields are:
+
+    - InstallationCode or InstallationId
+    - DriverClassName
+    - DriverDeviceType
+    - DeviceCode
+    - DeviceName
+    - PropertyName
+    - SensorName
+    - SensorTemplate
+    - SensorUnitOfMeasure
+    - EquipmentClass
+    - EquipmentLabel
+
+    Parameters
+    ----------
+    df: pandas.DataFrame
+        The asset register created by the driver including the minimum required set of columns.
+    api_inputs : ApiInputs
+        Object returned by initialize() function.
+    tag_columns : list, default = None
+        Columns of dataframe that contain tags (Default value = None).
+    metadata_columns : list, default = None
+        Column(s) of dataframe that contain device-level metadata (Default value = None).
+    save_additional_columns_as_slices : bool, default = False
+        Whether additional columns should be saved as slices (Default value = False).
+
+    Returns
+    -------
+    tuple[list, pandas.DataFrame]
+        (response_status_list, upsert_response_df) - Returns the list of response statuses and the dataframe containing
+        the parsed response text.
+
+    """
+
+    if api_inputs.api_base_url == '' or api_inputs.bearer_token == '':
+        logger.error("You must call initialize() before using API.")
+        return pandas.DataFrame()
+
+    data_frame = df.copy()
+
+    required_columns = ['DriverClassName', 'DriverDeviceType', 'PropertyName', 'DeviceCode', 'DeviceName', 'SensorName', 'SensorTemplate',
+                        'SensorUnitOfMeasure', 'EquipmentClass', 'EquipmentLabel']
+    proposed_columns = data_frame.columns.tolist()
+
+    if not set(required_columns).issubset(data_frame.columns):
+        logger.exception('Missing required column(s): %s', set(required_columns).difference(proposed_columns))
+        return 'Integration.upsert_device_sensors(): data_frame must contain the following columns: ' + ', '.join(
+            required_columns)
+    
+    if 'InstallationCode' not in data_frame.columns and 'InstallationId' not in data_frame.columns:
+        logger.exception('Must contain InstallationCode or InstallationId')
+        return 'Integration.upsert_device_sensors(): data_frame must contain either InstallationCode or InstallationId columns'
+    
+    if tag_columns is not None and not set(tag_columns).issubset(data_frame.columns):
+        logger.exception('Missing expected tag column(s): %s', set(tag_columns).difference(proposed_columns))
+        return 'Integration.upsert_device_sensors(): data_frame expected to contain the following tag column(s): ' + \
+               ', '.join(tag_columns)
+    elif tag_columns is None:
+        tag_columns = []
+
+    if metadata_columns is not None and not set(metadata_columns).issubset(data_frame.columns):
+        logger.exception('Missing expected metadata column(s): %s', set(metadata_columns).difference(proposed_columns))
+        return 'Integration.upsert_device_sensors(): data_frame expected to contain the following metadata ' \
+               'column(s): ' + ', '.join(metadata_columns)
+    elif metadata_columns is None:
+        metadata_columns = []
+
+    required_columns.append('InstallationCode')
+    required_columns.append('InstallationId')
+    slice_columns = set(proposed_columns).difference(set(required_columns)) - set(tag_columns) - set(metadata_columns)
+    slices_data_frame = pandas.DataFrame()
+
+    if len(slice_columns) > 0 or len(tag_columns) > 0 or len(metadata_columns) > 0:
+        def update_values(row, mode):
+            if mode == 'A':
+                j_row = row[slice_columns].to_json()
+                return str(j_row)
+            elif mode == 'B':
+                j_row = row[tag_columns].to_json()
+                return str(j_row)
+            else:
+                j_row = row[metadata_columns].to_json()
+                return str(j_row)
+
+        data_frame['Slices'] = data_frame.apply(update_values, args="A", axis=1)
+        #data_frame['TagsJson'] = data_frame.apply(update_values, args="B", axis=1)
+        #data_frame['MetadataJson'] = data_frame.apply(update_values, args="C", axis=1)
+        data_frame = data_frame.drop(columns=slice_columns)
+        slices_data_frame = data_frame[['DeviceCode', 'Slices']]
+
+    headers = api_inputs.api_headers.integration
+
+    url = f"{api_inputs.api_projects_endpoint}/{api_inputs.api_project_id}/devices/upsert-ingestion"
+    
+    def group_data_frame(df):
+        if 'InstallationCode' in data_frame.columns:
+            return df.groupby(['InstallationCode', 'DeviceCode'])
+        else:
+            return df.groupby(['InstallationId', 'DeviceCode'])
+    
+    data_frame_grpd = group_data_frame(data_frame)
+
+
+    chunk_list = []
+    for name, group in data_frame_grpd:
+        logger.info("Sending request: POST %s", url)
+        logger.info('Upserting data for InstallationCode = %s and DeviceCode = %s', str(name[0]), str(name[1]))
+        # logger.info('Sensor count to upsert: %s', str(group.shape[0]))
+        print(group.to_json(orient='records'))
+        response = requests.post(url, data=group.to_json(orient='records'), headers=headers)
+
+        response_status = '{} {}'.format(response.status_code, response.reason)
+        logger.info("Response status: %s", response_status)
+        if response.status_code != 200:
+            logger.error("API Call was not successful. Response Status: %s. Reason: %s.", response.status_code,
+                         response.reason)
+            chunk_list += [{'Chunk': name, 'DeviceCountToUpsert': 1, 'SensorCountToUpsert': str(group.shape[0]),
+                            'response_status': response_status, 'response_df': pandas.DataFrame(),
+                            'invalid_rows': pandas.DataFrame()}]
+        elif len(response.text) == 0:
+            logger.error('No data returned for this API call. %s', response.request.url)
+            chunk_list += [{'Chunk': name, 'DeviceCountToUpsert': 1, 'SensorCountToUpsert': str(group.shape[0]),
+                            'response_status': response_status, 'response_df': pandas.DataFrame(),
+                            'invalid_rows': pandas.DataFrame()}]
+        elif response.status_code == 200 and len(response.text) > 0:
+            response_data_frame = pandas.read_json(response.text)
+            logger.info('Dataframe response row count = %s', str(response_data_frame.shape[0]))
+            if response_data_frame.shape[1] > 0:
+                response_data_frame = response_data_frame.assign(InstallationCode=str(name[0]),
+                                                                 SensorCount=group.shape[0])
+                invalid_rows = response_data_frame[response_data_frame['status'] != 'Ok']
+                if invalid_rows.shape[0] > 0:
+                    logger.error("The following rows contain invalid data: %s", invalid_rows)
+                    chunk_list += [
+                        {'Chunk': name, 'DeviceCountToUpsert': 1,
+                         'SensorCountToUpsert': str(group.shape[0]),
+                         'response_status': response_status,
+                         'response_df': response_data_frame[response_data_frame['status'] == 'Ok'],
+                         'invalid_rows': invalid_rows}]
+                else:
+                    chunk_list += [{'Chunk': name, 'DeviceCountToUpsert': 1,
+                                    'SensorCountToUpsert': str(group.shape[0]),
+                                    'response_status': response_status, 'response_df': response_data_frame,
+                                    'invalid_rows': invalid_rows}]
+
+    upsert_response_df = pandas.DataFrame()
+    upsert_invalid_rows_df = pandas.DataFrame()
+    upsert_response_status_list = []
+    for i in range(len(chunk_list)):
+        upsert_response_df = upsert_response_df.append(chunk_list[i]['response_df'])
+        upsert_invalid_rows_df = upsert_invalid_rows_df.append(chunk_list[i]['invalid_rows'])
+        upsert_response_status_list += [chunk_list[i]['response_status']]
+
+    if save_additional_columns_as_slices and slices_data_frame.shape[0] > 0:
+        slices_merged = pandas.merge(left=upsert_response_df, right=slices_data_frame, left_on='deviceCode',
+                                     right_on='DeviceCode')
+        slices_data_frame = slices_merged[['deviceId', 'Slices']]
+        slices_data_frame = slices_data_frame.rename(columns={'deviceId': 'DeviceId'})
+        upsert_data(slices_data_frame, api_inputs=api_inputs, key_columns=['DeviceId'], table_name='DeviceSensorSlices',
+                    is_slices_table=True)
+
+    upsert_response_df.columns = _column_name_cap(columns=upsert_response_df.columns)
+    _upsert_entities_affected_count(api_inputs=api_inputs,
+                                    entities_affected_count=upsert_response_df['SensorCount'].sum())
+    _adx_support(api_inputs=api_inputs, payload_type='Sensors')
+
+    logger.info("Ingestion Complete. ")
+    return upsert_response_status_list, upsert_response_df
+
 
 @_with_func_attrs(df_required_columns=['InstallationName', 'InstallationCode', 'Address', 'Country', 'Suburb', 'State',
                                        'StateName', 'FloorAreaM2', 'ZipPostCode'],
                   df_optional_columns=['Latitude', 'Longitude', 'Timezone', 'InstallationId'])
 def upsert_sites(df: pandas.DataFrame, api_inputs: ApiInputs, tag_columns: list = None,
                  save_additional_columns_as_slices: bool = False):
     """Upsert site(s).
```

### Comparing `switch_api-0.3.1b1/switch_api/pipeline/__init__.py` & `switch_api-0.3.3/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/pipeline/automation.py` & `switch_api-0.3.3/switch_api/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/pipeline/definitions.py` & `switch_api-0.3.3/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/pipeline/pipeline.py` & `switch_api-0.3.3/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/platform_insights/__init__.py` & `switch_api-0.3.3/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api/platform_insights/platform_insights.py` & `switch_api-0.3.3/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.1b1/switch_api.egg-info/PKG-INFO` & `switch_api-0.3.3/switch_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-api
-Version: 0.3.1b1
+Version: 0.3.3
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,19 +34,93 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
-## 0.3.1-beta1
+## 0.3.3
 
 ### Added
-- Switch Python Extensions support
-  - This stil work in progress, documentation on usage will be updated in a future release.
+- New `upsert_device_sensors_ext` method to the `integration` module.
+  - Compared to existing `upsert_device_sensors` following are supported:
+    - Installation Code or Installation Id may be provided
+      - BUT cannot provide mix of the two, all must have either code or id and not both.
+    - DriverClassName
+    - DriverDeviceType
+    - PropertyName
+### Added Feature - Switch Python Extensions
+- Extensions may be used in Task Insights and Switch Guides for code reuse
+- Extensions maybe located in any directory structure within the repo where the usage scripts are located
+- May need to adjust your environment to detect the files if you're not running a project environment
+  - Tested on VSCode and PyCharm - contact Switch Support for issues.
+
+#### Extensions Usage
+```python
+import switch_api as sw
+
+# Single import line per extension
+from extensions.my_extension import MyExtension
+
+@sw.extensions.provide(field="some_extension")
+class MyTask:
+    some_extension: MyExtension
+
+if __name__ == "__main__":
+    task = MyTask()
+    task.some_extension.do_something()
+```
+
+#### Extensions Registration
+```python
+import uuid
+import switch_api as sw
+
+class SimpleExtension(sw.extensions.ExtensionTask):
+    @property
+    def id(self) -> uuid.UUID:
+        # Unique ID for the extension.
+        # Generate in CLI using:
+        #   python -c 'import uuid; print(uuid.uuid4())'
+        return '46759cfe-68fa-440c-baa9-c859264368db'
+    
+    @property
+    def description(self) -> str:
+        return 'Extension with a simple get_name function.'
+    
+    @property
+    def author(self) -> str:
+        return 'Amruth Akoju'
+    
+    @property
+    def version(self) -> str:
+        return '1.0.1'
+
+    def get_name(self):
+        return "Simple Extension"
+
+# Scaffold code for registration. This will not be persisted in the extension.
+if __name__ == '__main__':
+    task = SimpleExtension()
+
+    api_inputs = sw.initialize(api_project_id='<portfolio-id>')
+
+    # Usage test
+    print(task.get_name())
+
+    # =================================================================
+    # REGISTER TASK & DATAFEED ========================================
+    # =================================================================
+    register = sw.pipeline.Automation.register_task(api_inputs, task)
+    print(register)
+
+```
+
+### Updated
+- get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
```

### Comparing `switch_api-0.3.1b1/switch_api.egg-info/SOURCES.txt` & `switch_api-0.3.3/switch_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

