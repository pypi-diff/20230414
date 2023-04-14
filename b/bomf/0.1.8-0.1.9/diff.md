# Comparing `tmp/bomf-0.1.8.tar.gz` & `tmp/bomf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.1.8.tar", last modified: Tue Apr  4 18:46:56 2023, max compression
+gzip compressed data, was "bomf-0.1.9.tar", last modified: Fri Apr 14 10:33:54 2023, max compression
```

## Comparing `bomf-0.1.8.tar` & `bomf-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.977608 bomf-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-04 18:46:50.000000 bomf-0.1.8/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-04 18:46:50.000000 bomf-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-04 18:46:50.000000 bomf-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-04 18:46:50.000000 bomf-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-04 18:46:56.977608 bomf-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-04 18:46:50.000000 bomf-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-04 18:46:50.000000 bomf-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 18:46:50.000000 bomf-0.1.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-04 18:46:50.000000 bomf-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-04 18:46:56.977608 bomf-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 18:46:50.000000 bomf-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.977608 bomf-0.1.8/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.977608 bomf-0.1.8/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/validation/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-04 18:46:50.000000 bomf-0.1.8/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.973608 bomf-0.1.8/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-04 18:46:56.000000 bomf-0.1.8/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-04 18:46:50.000000 bomf-0.1.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:46:56.977608 bomf-0.1.8/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-04 18:46:50.000000 bomf-0.1.8/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.306327 bomf-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 10:33:44.000000 bomf-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 10:33:44.000000 bomf-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-14 10:33:44.000000 bomf-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-14 10:33:54.310327 bomf-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-14 10:33:44.000000 bomf-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-14 10:33:44.000000 bomf-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 10:33:44.000000 bomf-0.1.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 10:33:44.000000 bomf-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-14 10:33:54.310327 bomf-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 10:33:44.000000 bomf-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.306327 bomf-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 10:33:44.000000 bomf-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_validation.py
```

### Comparing `bomf-0.1.8/.github/dependabot.yml` & `bomf-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/black.yml` & `bomf-0.1.9/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/codeql-analysis.yml` & `bomf-0.1.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/coverage.yml` & `bomf-0.1.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/packaging_test.yml` & `bomf-0.1.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/python-publish.yml` & `bomf-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/pythonlint.yml` & `bomf-0.1.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.github/workflows/unittests.yml` & `bomf-0.1.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.gitignore` & `bomf-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/.pre-commit-config.yaml` & `bomf-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/LICENSE` & `bomf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/PKG-INFO` & `bomf-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.1.8
+Version: 0.1.9
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.1.8/README.md` & `bomf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/pyproject.toml` & `bomf-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/requirements.txt` & `bomf-0.1.9/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 attrs==22.2.0
     # via -r requirements.in
 bidict==0.22.1
     # via -r requirements.in
 bo4e==0.4.7
     # via -r requirements.in
-frozendict==2.3.6
+frozendict==2.3.7
     # via -r requirements.in
 iso3166==2.1.1
     # via bo4e
 pydantic==1.10.7
     # via
     #   -r requirements.in
     #   bo4e
```

### Comparing `bomf-0.1.8/setup.cfg` & `bomf-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/__init__.py` & `bomf-0.1.9/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/filter/__init__.py` & `bomf-0.1.9/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.1.9/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/loader/entityloader.py` & `bomf-0.1.9/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/mapper/__init__.py` & `bomf-0.1.9/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/model/__init__.py` & `bomf-0.1.9/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/provider/__init__.py` & `bomf-0.1.9/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/validation/core.py` & `bomf-0.1.9/src/bomf/validation/core.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/src/bomf/validation/utils.py` & `bomf-0.1.9/src/bomf/validation/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     value.
     """
     current_obj: Any = obj
     for index, attr_name in enumerate(attribute_path):
         try:
             current_obj = getattr(current_obj, attr_name)
         except AttributeError as error:
-            current_path = ".".join(attribute_path[0:index])
-            raise AttributeError(f"{current_path} does not exist") from error
+            current_path = ".".join(attribute_path[0 : index + 1])
+            raise AttributeError(f"'{current_path}' does not exist") from error
     check_type(".".join(attribute_path), current_obj, attribute_type)
     return current_obj
```

### Comparing `bomf-0.1.8/src/bomf.egg-info/PKG-INFO` & `bomf-0.1.9/src/bomf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.1.8
+Version: 0.1.9
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.1.8/src/bomf.egg-info/SOURCES.txt` & `bomf-0.1.9/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/tox.ini` & `bomf-0.1.9/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_bo4e_data_set.py` & `bomf-0.1.9/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_entity_loader.py` & `bomf-0.1.9/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_filter.py` & `bomf-0.1.9/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_mapper.py` & `bomf-0.1.9/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_migration.py` & `bomf-0.1.9/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_source_data_provider.py` & `bomf-0.1.9/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.8/unittests/test_validation.py` & `bomf-0.1.9/unittests/test_validation.py`

 * *Files identical despite different names*

