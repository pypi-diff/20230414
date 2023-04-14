# Comparing `tmp/wystia-1.2.0.tar.gz` & `tmp/wystia-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wystia-1.2.0.tar", last modified: Fri Apr  7 21:44:52 2023, max compression
+gzip compressed data, was "wystia-1.2.1.tar", last modified: Fri Apr 14 19:23:42 2023, max compression
```

## Comparing `wystia-1.2.0.tar` & `wystia-1.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-07 21:44:47.000000 wystia-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-07 21:44:47.000000 wystia-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 21:44:47.000000 wystia-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-07 21:44:47.000000 wystia-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-07 21:44:52.429243 wystia-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-07 21:44:47.000000 wystia-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.rst
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.utils.parse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 21:44:52.429243 wystia-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-07 21:44:47.000000 wystia-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/testdata/sample-captions.srt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/testdata/upload_response.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/test_wystia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/utils/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/wystia/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/requests_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/requests_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/wystia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/metaclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/wystia/utils/parse/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/srt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/wystia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.438271 wystia-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 19:23:37.000000 wystia-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-14 19:23:37.000000 wystia-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 19:23:37.000000 wystia-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-14 19:23:37.000000 wystia-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-04-14 19:23:42.438271 wystia-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-14 19:23:37.000000 wystia-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.utils.parse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 19:23:42.438271 wystia-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-14 19:23:37.000000 wystia-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/testdata/sample-captions.srt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/testdata/upload_response.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/test_wystia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/requests_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/metaclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/top_level.txt
```

### Comparing `wystia-1.2.0/CONTRIBUTING.rst` & `wystia-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/HISTORY.rst` & `wystia-1.2.1/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,36 @@
 =======
 History
 =======
 
+1.2.1 (2023-04-14)
+------------------
+
+**Bugfixes**
+
+* The ``Media`` class did not have the ``archived`` (``bool``) field, which
+  was resulting in errors when ``list_project()`` was called.
+
+  Therefore, moved over this field from ``Video`` to ``Media`` instead (which is the
+  super-class) so that this issue can be resolved.
+
 1.2.0 (2023-04-07)
 ------------------
 
-* Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
-* Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+**Features and Improvements**
+
+* Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default -- credits to `@KaneDM`_.
 * Upgrade dependencies in ``requirements-dev.txt``.
 
+**Bugfixes**
+
+* Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+
+.. _@KaneDM: https://github.com/KaneDM
+
 1.1.0 (2022-01-27)
 ------------------
 
 * Refactor any model classes that would be returned in *list* API
   calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
   simply so that ``Container`` objects will be returned by default.
```

### Comparing `wystia-1.2.0/LICENSE` & `wystia-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/PKG-INFO` & `wystia-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wystia
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Description: ==========================
         Wystia - Wistia API Helper
@@ -298,21 +298,39 @@
         .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
         
         
         =======
         History
         =======
         
+        1.2.1 (2023-04-14)
+        ------------------
+        
+        **Bugfixes**
+        
+        * The ``Media`` class did not have the ``archived`` (``bool``) field, which
+          was resulting in errors when ``list_project()`` was called.
+        
+          Therefore, moved over this field from ``Video`` to ``Media`` instead (which is the
+          super-class) so that this issue can be resolved.
+        
         1.2.0 (2023-04-07)
         ------------------
         
-        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
-        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        **Features and Improvements**
+        
+        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default -- credits to `@KaneDM`_.
         * Upgrade dependencies in ``requirements-dev.txt``.
         
+        **Bugfixes**
+        
+        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        
+        .. _@KaneDM: https://github.com/KaneDM
+        
         1.1.0 (2022-01-27)
         ------------------
         
         * Refactor any model classes that would be returned in *list* API
           calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
           simply so that ``Container`` objects will be returned by default.
```

### Comparing `wystia-1.2.0/README.rst` & `wystia-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/Makefile` & `wystia-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/conf.py` & `wystia-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/installation.rst` & `wystia-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/make.bat` & `wystia-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/usage.rst` & `wystia-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/wystia.rst` & `wystia-1.2.1/docs/wystia.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/wystia.utils.parse.rst` & `wystia-1.2.1/docs/wystia.utils.parse.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/docs/wystia.utils.rst` & `wystia-1.2.1/docs/wystia.utils.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/setup.py` & `wystia-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 
 readme = (here / 'README.rst').read_text()
 history = (here / 'HISTORY.rst').read_text()
 
 setup(
     name='wystia',
-    version='1.2.0',
+    version='1.2.1',
     description='A Python wrapper library for the Wistia API',
     long_description=readme + '\n\n' + history,
     author='Ritvik Nag',
     author_email='rv.kvetch@gmail.com',
     url='https://github.com/rnag/wystia',
     packages=packages,
     include_package_data=True,
```

### Comparing `wystia-1.2.0/tests/conftest.py` & `wystia-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/tests/unit/conftest.py` & `wystia-1.2.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/tests/unit/test_wystia.py` & `wystia-1.2.1/tests/unit/test_wystia.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/tests/unit/utils/parse/test_srt.py` & `wystia-1.2.1/tests/unit/utils/parse/test_srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/tests/unit/utils/parse/test_types.py` & `wystia-1.2.1/tests/unit/utils/parse/test_types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/__init__.py` & `wystia-1.2.1/wystia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 
 # A handy alias in case it comes in useful to anyone :-)
 WistiaApi = WistiaDataApi
 
 
 __author__ = 'Ritvik Nag'
 __email__ = 'rv.kvetch@gmail.com'
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 #   https://docs.python.org/3.8/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger('wystia').addHandler(logging.NullHandler())
```

### Comparing `wystia-1.2.0/wystia/api_base.py` & `wystia-1.2.1/wystia/api_base.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/api_data.py` & `wystia-1.2.1/wystia/api_data.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/api_embed.py` & `wystia-1.2.1/wystia/api_embed.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/api_helper.py` & `wystia-1.2.1/wystia/api_helper.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/api_upload.py` & `wystia-1.2.1/wystia/api_upload.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/config.py` & `wystia-1.2.1/wystia/config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/constants.py` & `wystia-1.2.1/wystia/constants.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/errors.py` & `wystia-1.2.1/wystia/errors.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/models.py` & `wystia-1.2.1/wystia/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 
     hashed_id: str
     id: int
     name: str
     type: MediaType
     created: datetime
     updated: datetime
+    archived: bool | None = None
     # Note: only videos have this attribute set; thumbnails and other
     # medias don't.
     duration: float | None = None
     status: MediaStatus = MediaStatus.NOT_FOUND
     description: str = ''
     progress: float = 0.0
     thumbnail: Thumbnail = None
@@ -234,15 +235,14 @@
     class _(JSONWizard.Meta):
         raise_on_unknown_json_key = RAISE_ON_UNKNOWN_KEY
         skip_defaults = True
 
     # Override the type annotations as needed.
     duration: float = 0.0
     project: ProjectInfo = None
-    archived: bool | None = None
 
     # Not included in GET '/v1/medias' response, but technically
     # still part of video metadata.
     has_audio_description: bool | None = None
     captions_enabled: bool | None = None
     overlay_text: str | None = None
     caption_duration: float | None = None
```

### Comparing `wystia-1.2.0/wystia/requests_config.py` & `wystia-1.2.1/wystia/requests_config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/requests_models.py` & `wystia-1.2.1/wystia/requests_models.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/utils/decorators.py` & `wystia-1.2.1/wystia/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/utils/parse/file.py` & `wystia-1.2.1/wystia/utils/parse/file.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/utils/parse/srt.py` & `wystia-1.2.1/wystia/utils/parse/srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia/utils/parse/types.py` & `wystia-1.2.1/wystia/utils/parse/types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.0/wystia.egg-info/PKG-INFO` & `wystia-1.2.1/wystia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wystia
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Description: ==========================
         Wystia - Wistia API Helper
@@ -298,21 +298,39 @@
         .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
         
         
         =======
         History
         =======
         
+        1.2.1 (2023-04-14)
+        ------------------
+        
+        **Bugfixes**
+        
+        * The ``Media`` class did not have the ``archived`` (``bool``) field, which
+          was resulting in errors when ``list_project()`` was called.
+        
+          Therefore, moved over this field from ``Video`` to ``Media`` instead (which is the
+          super-class) so that this issue can be resolved.
+        
         1.2.0 (2023-04-07)
         ------------------
         
-        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
-        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        **Features and Improvements**
+        
+        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default -- credits to `@KaneDM`_.
         * Upgrade dependencies in ``requirements-dev.txt``.
         
+        **Bugfixes**
+        
+        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        
+        .. _@KaneDM: https://github.com/KaneDM
+        
         1.1.0 (2022-01-27)
         ------------------
         
         * Refactor any model classes that would be returned in *list* API
           calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
           simply so that ``Container`` objects will be returned by default.
```

### Comparing `wystia-1.2.0/wystia.egg-info/SOURCES.txt` & `wystia-1.2.1/wystia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

