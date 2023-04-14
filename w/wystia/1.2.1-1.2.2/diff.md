# Comparing `tmp/wystia-1.2.1.tar.gz` & `tmp/wystia-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wystia-1.2.1.tar", last modified: Fri Apr 14 19:23:42 2023, max compression
+gzip compressed data, was "wystia-1.2.2.tar", last modified: Fri Apr 14 19:43:55 2023, max compression
```

## Comparing `wystia-1.2.1.tar` & `wystia-1.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.438271 wystia-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 19:23:37.000000 wystia-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-14 19:23:37.000000 wystia-1.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 19:23:37.000000 wystia-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-14 19:23:37.000000 wystia-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-04-14 19:23:42.438271 wystia-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-14 19:23:37.000000 wystia-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.rst
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.utils.parse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 19:23:37.000000 wystia-1.2.1/docs/wystia.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 19:23:42.438271 wystia-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-14 19:23:37.000000 wystia-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/testdata/sample-captions.srt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/testdata/upload_response.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/test_wystia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/tests/unit/utils/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/parse/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 19:23:37.000000 wystia-1.2.1/tests/unit/utils/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/api_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/requests_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/requests_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/metaclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia/utils/parse/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/srt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/parse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 19:23:37.000000 wystia-1.2.1/wystia/utils/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:42.434271 wystia-1.2.1/wystia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 19:23:42.000000 wystia-1.2.1/wystia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.638334 wystia-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 19:43:49.000000 wystia-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-14 19:43:49.000000 wystia-1.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 19:43:49.000000 wystia-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-14 19:43:49.000000 wystia-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-04-14 19:43:55.638334 wystia-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-14 19:43:49.000000 wystia-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.630334 wystia-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/wystia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/wystia.utils.parse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 19:43:49.000000 wystia-1.2.2/docs/wystia.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 19:43:55.638334 wystia-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 19:43:49.000000 wystia-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.630334 wystia-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.630334 wystia-1.2.2/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/testdata/sample-captions.srt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/testdata/upload_response.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.630334 wystia-1.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/test_wystia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.634334 wystia-1.2.2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.634334 wystia-1.2.2/tests/unit/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/parse/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/parse/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/parse/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 19:43:49.000000 wystia-1.2.2/tests/unit/utils/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.638334 wystia-1.2.2/wystia/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/api_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/api_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/requests_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.638334 wystia-1.2.2/wystia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/metaclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.638334 wystia-1.2.2/wystia/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/parse/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/parse/srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/parse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 19:43:49.000000 wystia-1.2.2/wystia/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:43:55.638334 wystia-1.2.2/wystia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 19:43:55.000000 wystia-1.2.2/wystia.egg-info/top_level.txt
```

### Comparing `wystia-1.2.1/CONTRIBUTING.rst` & `wystia-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/HISTORY.rst` & `wystia-1.2.2/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+1.2.2 (2023-04-14)
+------------------
+
+**Features and Improvements**
+
+* Update ``keywords`` for the package.
+* Add `Python 3.11` to the list of supported versions.
+
 1.2.1 (2023-04-14)
 ------------------
 
 **Bugfixes**
 
 * The ``Media`` class did not have the ``archived`` (``bool``) field, which
   was resulting in errors when ``list_project()`` was called.
@@ -26,14 +34,16 @@
 * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
 
 .. _@KaneDM: https://github.com/KaneDM
 
 1.1.0 (2022-01-27)
 ------------------
 
+**Features and Improvements**
+
 * Refactor any model classes that would be returned in *list* API
   calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
   simply so that ``Container`` objects will be returned by default.
 
 * Refactor to import ``Container`` from the ``dataclass-wizard`` library
   instead. For backwards compatibility reasons, the ``models`` module
   still exports the *Container* namespace.
```

### Comparing `wystia-1.2.1/LICENSE` & `wystia-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/PKG-INFO` & `wystia-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wystia
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Description: ==========================
         Wystia - Wistia API Helper
@@ -298,14 +298,22 @@
         .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
         
         
         =======
         History
         =======
         
+        1.2.2 (2023-04-14)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Update ``keywords`` for the package.
+        * Add `Python 3.11` to the list of supported versions.
+        
         1.2.1 (2023-04-14)
         ------------------
         
         **Bugfixes**
         
         * The ``Media`` class did not have the ``archived`` (``bool``) field, which
           was resulting in errors when ``list_project()`` was called.
@@ -326,14 +334,16 @@
         * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
         
         .. _@KaneDM: https://github.com/KaneDM
         
         1.1.0 (2022-01-27)
         ------------------
         
+        **Features and Improvements**
+        
         * Refactor any model classes that would be returned in *list* API
           calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
           simply so that ``Container`` objects will be returned by default.
         
         * Refactor to import ``Container`` from the ``dataclass-wizard`` library
           instead. For backwards compatibility reasons, the ``models`` module
           still exports the *Container* namespace.
@@ -408,22 +418,23 @@
         * Update docs with better examples
         
         0.1.0 (2021-06-12)
         ------------------
         
         * First release on PyPI.
         
-Keywords: wistia,wistia api,wystia,wistia data api,wistia upload api
+Keywords: wistia,api,wrapper,data api,upload api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
```

### Comparing `wystia-1.2.1/README.rst` & `wystia-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/Makefile` & `wystia-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/conf.py` & `wystia-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/installation.rst` & `wystia-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/make.bat` & `wystia-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/usage.rst` & `wystia-1.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/wystia.rst` & `wystia-1.2.2/docs/wystia.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/wystia.utils.parse.rst` & `wystia-1.2.2/docs/wystia.utils.parse.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/docs/wystia.utils.rst` & `wystia-1.2.2/docs/wystia.utils.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/setup.py` & `wystia-1.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,60 +7,64 @@
 here = pathlib.Path(__file__).parent
 
 package_name = 'wystia'
 
 packages = [
     package_name,
     f'{package_name}.utils',
-    f'{package_name}.utils.parse'
+    f'{package_name}.utils.parse',
 ]
 
 requires = [
     'requests',
     'requests-toolbelt',
     'urllib3',  # should already be installed via requests
     'dataclass-wizard>=0.21.0,<1.0',
-    'cached-property~=1.5.2; python_version == "3.7"'
+    'cached-property~=1.5.2; python_version == "3.7"',
 ]
 
 test_requirements = [
     'pytest>=6',
-    'pytest-mock~=3.6.1'
+    'pytest-mock~=3.6.1',
 ]
 
 readme = (here / 'README.rst').read_text()
 history = (here / 'HISTORY.rst').read_text()
 
 setup(
     name='wystia',
-    version='1.2.1',
+    version='1.2.2',
     description='A Python wrapper library for the Wistia API',
     long_description=readme + '\n\n' + history,
     author='Ritvik Nag',
     author_email='rv.kvetch@gmail.com',
     url='https://github.com/rnag/wystia',
     packages=packages,
     include_package_data=True,
     python_requires='>=3.7',
     install_requires=requires,
     license='MIT',
-    keywords=['wistia', 'wistia api', 'wystia',
-              'wistia data api', 'wistia upload api'],
+    keywords=['wistia',
+              'api',
+              'wrapper',
+              'data api',
+              'upload api'],
     classifiers=[
         # Ref: https://pypi.org/classifiers/
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python'
     ],
     test_suite='tests',
     tests_require=test_requirements,
     zip_safe=False
 )
```

### Comparing `wystia-1.2.1/tests/conftest.py` & `wystia-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/tests/unit/conftest.py` & `wystia-1.2.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/tests/unit/test_wystia.py` & `wystia-1.2.2/tests/unit/test_wystia.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/tests/unit/utils/parse/test_srt.py` & `wystia-1.2.2/tests/unit/utils/parse/test_srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/tests/unit/utils/parse/test_types.py` & `wystia-1.2.2/tests/unit/utils/parse/test_types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/__init__.py` & `wystia-1.2.2/wystia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 
 # A handy alias in case it comes in useful to anyone :-)
 WistiaApi = WistiaDataApi
 
 
 __author__ = 'Ritvik Nag'
 __email__ = 'rv.kvetch@gmail.com'
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 #   https://docs.python.org/3.8/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger('wystia').addHandler(logging.NullHandler())
```

### Comparing `wystia-1.2.1/wystia/api_base.py` & `wystia-1.2.2/wystia/api_base.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/api_data.py` & `wystia-1.2.2/wystia/api_data.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/api_embed.py` & `wystia-1.2.2/wystia/api_embed.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/api_helper.py` & `wystia-1.2.2/wystia/api_helper.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/api_upload.py` & `wystia-1.2.2/wystia/api_upload.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/config.py` & `wystia-1.2.2/wystia/config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/constants.py` & `wystia-1.2.2/wystia/constants.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/errors.py` & `wystia-1.2.2/wystia/errors.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/models.py` & `wystia-1.2.2/wystia/models.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/requests_config.py` & `wystia-1.2.2/wystia/requests_config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/requests_models.py` & `wystia-1.2.2/wystia/requests_models.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/utils/decorators.py` & `wystia-1.2.2/wystia/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/utils/parse/file.py` & `wystia-1.2.2/wystia/utils/parse/file.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/utils/parse/srt.py` & `wystia-1.2.2/wystia/utils/parse/srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia/utils/parse/types.py` & `wystia-1.2.2/wystia/utils/parse/types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.2.1/wystia.egg-info/PKG-INFO` & `wystia-1.2.2/wystia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wystia
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Description: ==========================
         Wystia - Wistia API Helper
@@ -298,14 +298,22 @@
         .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
         
         
         =======
         History
         =======
         
+        1.2.2 (2023-04-14)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Update ``keywords`` for the package.
+        * Add `Python 3.11` to the list of supported versions.
+        
         1.2.1 (2023-04-14)
         ------------------
         
         **Bugfixes**
         
         * The ``Media`` class did not have the ``archived`` (``bool``) field, which
           was resulting in errors when ``list_project()`` was called.
@@ -326,14 +334,16 @@
         * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
         
         .. _@KaneDM: https://github.com/KaneDM
         
         1.1.0 (2022-01-27)
         ------------------
         
+        **Features and Improvements**
+        
         * Refactor any model classes that would be returned in *list* API
           calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
           simply so that ``Container`` objects will be returned by default.
         
         * Refactor to import ``Container`` from the ``dataclass-wizard`` library
           instead. For backwards compatibility reasons, the ``models`` module
           still exports the *Container* namespace.
@@ -408,22 +418,23 @@
         * Update docs with better examples
         
         0.1.0 (2021-06-12)
         ------------------
         
         * First release on PyPI.
         
-Keywords: wistia,wistia api,wystia,wistia data api,wistia upload api
+Keywords: wistia,api,wrapper,data api,upload api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
```

### Comparing `wystia-1.2.1/wystia.egg-info/SOURCES.txt` & `wystia-1.2.2/wystia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

