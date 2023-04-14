# Comparing `tmp/funding-service-design-utils-1.0.8.tar.gz` & `tmp/funding-service-design-utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-1.0.8.tar", last modified: Tue Nov  1 13:47:54 2022, max compression
+gzip compressed data, was "funding-service-design-utils-1.0.9.tar", last modified: Thu Nov  3 16:17:40 2022, max compression
```

## Comparing `funding-service-design-utils-1.0.8.tar` & `funding-service-design-utils-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10093 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7757 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7084 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11916 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-01 13:47:54.000000 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-01 13:47:54.000000 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 13:47:54.000000 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-01 13:47:54.000000 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-01 13:47:54.000000 funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:54.171417 funding-service-design-utils-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-01 13:47:44.000000 funding-service-design-utils-1.0.8/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10093 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9814 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7757 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7084 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11916 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-1.0.8/LICENSE` & `funding-service-design-utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/PKG-INFO` & `funding-service-design-utils-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-1.0.8/README.md` & `funding-service-design-utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/__init__.py` & `funding-service-design-utils-1.0.9/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-1.0.9/fsd_utils/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/config/configclass.py` & `funding-service-design-utils-1.0.9/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-1.0.9/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-1.0.9/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-1.0.9/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-1.0.9/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-1.0.9/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/logging/logging.py` & `funding-service-design-utils-1.0.9/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-1.0.9/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-1.0.8/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/pyproject.toml` & `funding-service-design-utils-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-1.0.8/tests/conftest.py` & `funding-service-design-utils-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/tests/test_checkers.py` & `funding-service-design-utils-1.0.9/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/tests/test_get_lang.py` & `funding-service-design-utils-1.0.9/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/tests/test_healthcheck.py` & `funding-service-design-utils-1.0.9/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.8/tests/test_set_lang.py` & `funding-service-design-utils-1.0.9/tests/test_set_lang.py`

 * *Files identical despite different names*

