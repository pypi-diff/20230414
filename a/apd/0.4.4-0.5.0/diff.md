# Comparing `tmp/apd-0.4.4.tar.gz` & `tmp/apd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apd-0.4.4.tar", last modified: Thu Jan 19 11:44:42 2023, max compression
+gzip compressed data, was "apd-0.5.0.tar", last modified: Fri Apr 14 13:31:01 2023, max compression
```

## Comparing `apd-0.4.4.tar` & `apd-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.124000 apd-0.4.4/
--rw-r--r--   0 root         (0) root         (0)     2075 2023-01-19 11:44:27.000000 apd-0.4.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1964 2023-01-19 11:44:27.000000 apd-0.4.4/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1066 2023-01-19 11:44:27.000000 apd-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      569 2023-01-19 11:44:27.000000 apd-0.4.4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-01-19 11:44:27.000000 apd-0.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4113 2023-01-19 11:44:42.124000 apd-0.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3695 2023-01-19 11:44:27.000000 apd-0.4.4/README.rst
--rw-r--r--   0 root         (0) root         (0)      572 2023-01-19 11:44:27.000000 apd-0.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1287 2023-01-19 11:44:42.124000 apd-0.4.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.116000 apd-0.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.116000 apd-0.4.4/src/apd/
--rw-r--r--   0 root         (0) root         (0)     1196 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15714 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/analysis_data.py
--rw-r--r--   0 root         (0) root         (0)    11246 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/ap_info.py
--rw-r--r--   0 root         (0) root         (0)     6431 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13521 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/command.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/data_cache.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/eos.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-01-19 11:44:27.000000 apd-0.4.4/src/apd/rich_console.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.120000 apd-0.4.4/src/apd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4113 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      307 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-19 11:44:42.000000 apd-0.4.4/src/apd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.120000 apd-0.4.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.116000 apd-0.4.4/tests/cache-dir/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.120000 apd-0.4.4/tests/cache-dir/b2oc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.120000 apd-0.4.4/tests/cache-dir/b2oc/b02dkpi/
--rw-r--r--   0 root         (0) root         (0)   157583 2023-01-19 11:44:27.000000 apd-0.4.4/tests/cache-dir/b2oc/b02dkpi/tags.json
--rw-r--r--   0 root         (0) root         (0)  2657491 2023-01-19 11:44:27.000000 apd-0.4.4/tests/cache-dir/b2oc/b02dkpi.json
--rw-r--r--   0 root         (0) root         (0)     3197 2023-01-19 11:44:27.000000 apd-0.4.4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:44:42.124000 apd-0.4.4/tests/data/
--rw-r--r--   0 root         (0) root         (0)    22577 2023-01-19 11:44:27.000000 apd-0.4.4/tests/data/rds_ap_info.json
--rw-r--r--   0 root         (0) root         (0)    22577 2023-01-19 11:44:27.000000 apd-0.4.4/tests/data/rds_ap_info_2versions.json
--rw-r--r--   0 root         (0) root         (0)     3719 2023-01-19 11:44:27.000000 apd-0.4.4/tests/test_analysis_data.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-01-19 11:44:27.000000 apd-0.4.4/tests/test_ap_info.py
--rw-r--r--   0 root         (0) root         (0)     9274 2023-01-19 11:44:27.000000 apd-0.4.4/tests/test_b2oc.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-01-19 11:44:27.000000 apd-0.4.4/tests/test_data_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-04-14 13:30:38.000000 apd-0.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-14 13:30:38.000000 apd-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-14 13:30:38.000000 apd-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      596 2023-04-14 13:30:38.000000 apd-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-14 13:30:38.000000 apd-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-04-14 13:31:01.384000 apd-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-04-14 13:30:38.000000 apd-0.5.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-14 13:30:38.000000 apd-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-04-14 13:31:01.384000 apd-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.372000 apd-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/src/apd/
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15871 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/analysis_data.py
+-rw-r--r--   0 root         (0) root         (0)    13854 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/ap_info.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    15411 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/command.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/data_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/eos.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/rich_console.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/snakemake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/src/apd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.372000 apd-0.5.0/tests/cache-dir/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.380000 apd-0.5.0/tests/cache-dir/b2oc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/
+-rw-r--r--   0 root         (0) root         (0)   157583 2023-04-14 13:30:38.000000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/tags.json
+-rw-r--r--   0 root         (0) root         (0)  2657491 2023-04-14 13:30:38.000000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi.json
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-04-14 13:30:38.000000 apd-0.5.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/tests/data/
+-rw-r--r--   0 root         (0) root         (0)    22577 2023-04-14 13:30:38.000000 apd-0.5.0/tests/data/rds_ap_info.json
+-rw-r--r--   0 root         (0) root         (0)    22577 2023-04-14 13:30:38.000000 apd-0.5.0/tests/data/rds_ap_info_2versions.json
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_analysis_data.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_ap_info.py
+-rw-r--r--   0 root         (0) root         (0)     9296 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_b2oc.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_data_cache.py
```

### Comparing `apd-0.4.4/.gitignore` & `apd-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/.gitlab-ci.yml` & `apd-0.5.0/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   - upload_pypi
 
 image: registry.cern.ch/docker.io/library/python:3.9
 
 .setup_environment:
   before_script:
     - pip install .[testing]
+    - pip install snakemake
 
 pre-commit:
   stage: test
   rules:
     - when: always
   before_script:
     - pip install pre-commit
@@ -39,15 +40,15 @@
 
 pylint:
   extends: .setup_environment
   stage: test
   rules:
     - when: always
   script:
-    - pylint -d W1514 src/apd
+    - pylint -d W1514 -d W0719 src/apd
 
 pytest:
   extends: .setup_environment
   stage: test
   rules:
     - when: always
   script:
```

### Comparing `apd-0.4.4/.pre-commit-config.yaml` & `apd-0.5.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 # See https://pre-commit.com/hooks.html for more hooks
 
 default_language_version:
   python: python
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       # - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, main]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-bugbear]
 
   - repo: "https://gitlab.cern.ch/lhcb-core/LbDevTools.git"
-    rev: 2.0.34
+    rev: 2.0.38
     hooks:
       - id: lb-add-copyright
         exclude: |
             (?x)^(
                 tests/data/.*\.json
             )$
```

### Comparing `apd-0.4.4/CONTRIBUTING.md` & `apd-0.5.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Contributing guidelines
 
 ## Creating a development environment
 
 ```bash
 git clone ssh://git@gitlab.cern.ch:7999/lhcb-dpa/analysis-productions/apd.git
 cd apd
-mamba create --name apd-dev requests requests-kerberos beautifulsoup4 click click-log ipython black pre-commit pytest
+mamba create -c conda-forge --name apd-dev requests requests-kerberos beautifulsoup4 click click-log ipython black pre-commit pytest responses
 conda activate apd-dev
-pip install -e .[testing]
+pip install -e ".[testing]"
 pre-commit install
 curl -o lb-check-copyright "https://gitlab.cern.ch/lhcb-core/LbDevTools/raw/master/LbDevTools/SourceTools.py?inline=false"
 chmod +x lb-check-copyright
 ```
 
 ## Running the tests
```

### Comparing `apd-0.4.4/LICENSE` & `apd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/PKG-INFO` & `apd-0.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,22 @@
-Metadata-Version: 2.1
-Name: apd
-Version: 0.4.4
-Summary: Tool to access the Analysis production Data
-License: BSD-3-Clause
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Provides-Extra: testing
-License-File: LICENSE
-
 Analysis Production Data
 ========================
 
-*EXPERIMENTAL* prototype of python module to fulfill:
-
-https://gitlab.cern.ch/lhcb-dpa/project/-/issues/134
+*EXPERIMENTAL* prototype of Python module to fulfill DPA's grand task https://gitlab.cern.ch/lhcb-dpa/project/-/issues/134.
 
-Design
-======
-
-Analysis Production information endpoint
-----------------------------------------
-
-This module allows downloading and using Analysis Production information
-from the endpoint *https://lbap.app.cern.ch/*
-
-Details about the endpoint can be found at:
-
-https://lbap.app.cern.ch/docs#/stable
-
-BEWARE: The endpoint is experimental and can be interrupted at any time.
 
 Usage
 =====
 
-From python
+The `apd` package is available in the ``lb-conda default`` environment.
+
+From Python
 -----------
 
-The python module allows interacting from analysis scripts, doing e.g.
+The Python module allows interacting from analysis scripts, doing e.g.
 
 ::
 
    In [8]: import apd
 
    In [9]: datasets = apd.AnalysisData("SL", "RDs")
 
@@ -78,7 +51,21 @@
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000004_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000005_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000006_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000007_1.bsntuple_mc.root
 
 The *apd-cache* command allows caching the Analysis metadata to a
 specific location.
+
+
+Design
+======
+
+Analysis Production information endpoint
+----------------------------------------
+
+This module allows downloading and using Analysis Productions information
+from the endpoint *https://lbap.app.cern.ch/*
+
+Details about the endpoint can be found at https://lbap.app.cern.ch/docs#/stable.
+
+BEWARE: The endpoint is experimental and can be interrupted at any time.
```

### Comparing `apd-0.4.4/pyproject.toml` & `apd-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/setup.cfg` & `apd-0.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 console_scripts = 
 	apd-login = apd.command:cmd_login
 	apd-logout = apd.command:cmd_logout
 	apd-cache-info = apd.command:cmd_cache_ap_info
 	apd-list-pfns = apd.command:cmd_list_pfns
 	apd-list-samples = apd.command:cmd_list_samples
 	apd-summary = apd.command:cmd_summary
-	apd-cache-pfns = apd.command:cmd_cache_pfns
+	apd-cache-files = apd.command:cmd_cache_ap_files
+	apd-dump-info = apd.command:cmd_dump_info
 
 [flake8]
 max-line-length = 80
-ignore = E501,W503,B950,B008,R0903
+ignore = E501,W503,B950,B008
 extend-ignore = 
 	E203,
 	B017,
 	B905,
 select = C,E,F,W,B,B9
 exclude = 
 	.pyre/
```

### Comparing `apd-0.4.4/src/apd/__init__.py` & `apd-0.5.0/src/apd/__init__.py`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/src/apd/analysis_data.py` & `apd-0.5.0/src/apd/analysis_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
 import copy
 import itertools
 import logging
 import os
-from collections import defaultdict
 
 from apd.ap_info import (
     SampleCollection,
+    check_tag_in_list,
     fetch_ap_info,
     iterable,
     load_ap_info,
     safe_casefold,
 )
 from apd.data_cache import DataCache
 
 logger = logging.getLogger("apd")
 
 APD_METADATA_CACHE_DIR = "APD_METADATA_CACHE_DIR"
 APD_METADATA_LIFETIME = "APD_METADATA_LIFETIME"
 APD_DATA_CACHE_DIR = "APD_DATA_CACHE_DIR"
 
 
-def _validate_tags(tags, default_tags=None):
+def _validate_tags(tags, default_tags=None, available_tags=None):
     """Method that checks the dictionary of tag names, values that should be used
     to filter the data accordingly.
 
      - Special cases are handled: tags "name" and "version" as well as "data" and "mc"
         (which are converted to a "config" value).
      - tag values cannot be None
      - tag values cannot be of type bytes
@@ -50,19 +50,19 @@
                 effective_tags[t] = v
 
     # Final dict that will be returned
     cleaned = {}
 
     # name and version are special tags in our case, we check their validity
     if "name" in effective_tags:
-        raise Exception("name is not supported on AnalysisData objects")
+        raise ValueError("name is not a supported tag in AnalysisData objects")
 
     version = effective_tags.get("version", None)
     if version and iterable(version):
-        raise Exception("version argument doesn't support iterables")
+        raise ValueError("version argument doesn't support iterables")
 
     # Special handling for the data and mc tags to avoid having to
     # use the config tag
     # The config tag is set according to the following table:
     #
     # | mc\data |    True    |    False   |      None      |
     # |:-------:|:----------:|:----------:|:--------------:|
@@ -107,14 +107,16 @@
         # Ignore those as we translated it to config already
         if t in ["data", "mc"]:
             continue
         if v is None:
             raise TypeError(f"{t} value is None")
         if isinstance(v, bytes):
             raise TypeError(f"{t} value is of type {type(v)}")
+        if available_tags is not None:
+            check_tag_in_list(t, available_tags)
         if isinstance(v, int) and not isinstance(v, bool):
             cleaned[t] = str(v)
         else:
             cleaned[t] = v
     return cleaned
 
 
@@ -211,25 +213,22 @@
         analysis,
         metadata_cache=None,
         data_cache=None,
         api_url="https://lbap.app.cern.ch",
         ap_date=None,
         **kwargs,
     ):
-
         """
         Constructor that configures the can either fetch the data from the AP service or load from a local cache.
 
         Analysis Production tags can be specified as keyword arguments
         to specify the data to be analyzed.
         """
         self.working_group = working_group
         self.analysis = analysis
-        # Tags is a list of tags that can be used to restrict the samples that will be used
-        self.default_tags = _validate_tags(kwargs)
 
         #  self.samples is a SampleCollection filled in with the values
         metadata_cache = metadata_cache or os.environ.get(APD_METADATA_CACHE_DIR, "")
         need_clean_fetch = False
         if metadata_cache:
             if isinstance(metadata_cache, SampleCollection):
                 logger.debug("Using SampleCollection passed to constructor")
@@ -253,18 +252,18 @@
             need_clean_fetch = True
 
         if need_clean_fetch:
             self.samples = fetch_ap_info(
                 working_group, analysis, None, api_url, ap_date=ap_date
             )
 
-        self.available_tags = defaultdict(set)
-        for sample in self.samples:
-            for k, v in self.samples._sampleTags(sample).items():
-                self.available_tags[k].add(v)
+        self.available_tags = self.samples.available_tags()
+
+        # Tags is a list of tags that can be used to restrict the samples that will be used
+        self.default_tags = _validate_tags(kwargs, available_tags=self.available_tags)
 
         # Now dealing with data cache
         data_cache = data_cache or os.environ.get(APD_DATA_CACHE_DIR, None)
         if isinstance(data_cache, str):
             self.data_cache = DataCache(data_cache)
         else:
             self.data_cache = data_cache
@@ -272,28 +271,29 @@
     def __call__(
         self,
         *,
         version=None,
         name=None,
         return_pfns=True,
         check_data=True,
+        use_local_cache=True,
         showmax=10,
         **tags,
     ):
         # pylint: disable-msg=too-many-locals
         """Main method that returns the dataset info.
         The normal behaviour is to return the PFNs for the samples but setting
         return_pfns to false returns the SampleCollection"""
 
         # Cannot mix data from 2 versions in the same dataset
         if not version:
             version = self.default_tags.get("version", None)
 
         if iterable(version):
-            raise Exception("version argument doesn't support iterables")
+            raise ValueError("version argument doesn't support iterables")
 
         # Establishing the list of samples to run on
         samples = self.samples
 
         if name:
             if version:
                 # No need to apply other tags, this specifies explicitly a specific dataset
@@ -311,15 +311,17 @@
                 if len(samples) != 1:
                     raise ValueError(
                         f"{len(samples)} matching {name}, should be exactly 1"
                     )
         else:
             # Merge the current tags with the default passed to the constructor
             # and check that they are consistent
-            effective_tags = _validate_tags(tags, self.default_tags)
+            effective_tags = _validate_tags(
+                tags, self.default_tags, self.available_tags
+            )
 
             if version:
                 effective_tags["version"] = version
 
             for tagname, tagvalue in effective_tags.items():
                 logger.debug("Filtering for %s = %s", tagname, tagvalue)
 
@@ -351,15 +353,17 @@
                             error_txt += "".join(
                                 ["\n" + " " * 5 + str(m) for m in match_list]
                             )
                     logger.debug("Error loading data: %s", error_txt)
                     raise ValueError("Error loading data: " + error_txt)
 
         if return_pfns:
-            return self._transform_pfns(samples.PFNs())
+            if use_local_cache:
+                return self._transform_pfns(samples.PFNs())
+            return samples.PFNs()
 
         return samples
 
     def _transform_pfns(self, pfns):
         """Method to return PFNs, useful as it can be overriden in inheriting classes"""
         if not self.data_cache:
             return pfns
```

### Comparing `apd-0.4.4/src/apd/ap_info.py` & `apd-0.5.0/src/apd/ap_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 ###############################################################################
-# (c) Copyright 2021 CERN for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2021-2023 CERN for the benefit of the LHCb Collaboration      #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 #
 # Tool to load and interpret information from the AnalysisProductions data endpoint
 #
 import collections.abc
+import difflib
+import itertools
 import json
 import logging
 import math
 import os
 import secrets
+from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
 
 import requests
 
 from .authentication import get_auth_headers
 from .eos import auth
@@ -38,28 +41,36 @@
 def safe_casefold(a):
     """casefold that can be called on any type, does nothing on non str"""
     if isinstance(a, str):
         return a.casefold()
     return a
 
 
+def check_tag_in_list(tag, tag_list):
+    """Check if the tag exists in the list of whether there is one close enough"""
+    if tag not in tag_list:
+        msg = f"Tag {tag} unknown."
+        closest = difflib.get_close_matches(tag, tag_list, n=1)
+        if closest:
+            msg += f" Did you mean {closest[0]} ?"
+        msg += f"\nAvailable tags: {', '.join(tag_list)}"
+        raise ValueError(msg)
+
+
 class InvalidCacheError(Exception):
     """Exception to signal that the AP info cache is invalid"""
 
 
 class APDataDownloader:
     def __init__(self, api_url="https://lbap.app.cern.ch"):
         self.api_url = api_url
         self.token = None
 
     def _get_kwargs(self):
-        return dict(
-            **get_auth_headers(),
-            timeout=120,
-        )
+        return {"timeout": 120, **get_auth_headers()}
 
     def get_ap_info(self, working_group, analysis, ap_date=None):
         params = {"at_time": ap_date} if ap_date else None
         r = requests.get(
             f"{self.api_url}/stable/v1/{working_group}/{analysis}",
             params=params,
             **self._get_kwargs(),
@@ -214,27 +225,28 @@
     return SampleCollection(data, tags), cacheinfo
 
 
 def load_ap_info_from_single_file(filename):
     """Load the API info from a cache file (ONLY FOR TESTS)"""
     filename = Path(filename)
     if not filename.is_file():
-        raise Exception("Please specify a valid file as metadata cache")
+        raise IOError(
+            f"Please specify a valid file as metadata cache, {filename} does not exist!"
+        )
     data = filename.read_text()
     apinfo = json.loads(data)
     info = apinfo["info"]
     tags = apinfo["tags"]
     return SampleCollection(info, tags)
 
 
 class SampleCollection:
     """Class wrapping the AnalysisProduction metadata."""
 
     def __init__(self, info=None, tags=None):
-
         self.info = info if info else []
         self.tags = tags if tags else {}
 
     def __len__(self):
         return len(self.info)
 
     def _sampleTags(self, sample):
@@ -276,14 +288,16 @@
         if (len(args) != 0) and len(args) != 2:
             raise ValueError(
                 "filter method takes two positional arguments or keyword arguments"
             )
 
         def _compare_tag(sample, ftag, fvalue):
             """Utility method than handles specific tags, but not iterables"""
+            sampleTags = self._sampleTags(sample)
+            check_tag_in_list(ftag, sampleTags.keys())
             return safe_casefold(self._sampleTags(sample).get(ftag)) == safe_casefold(
                 fvalue
             )
 
         def _filter1(samples, ftag, fvalue):
             logger.debug("filtering samples for %s:%s", ftag, fvalue)
             if callable(fvalue):
@@ -335,7 +349,58 @@
             count += len(sample["lfns"].keys())
         return count
 
     def __or__(self, samples):
         info = self.info + samples.info
         tags = {**(self.tags), **(samples.tags)}
         return SampleCollection(info, tags)
+
+    def available_tags(self):
+        """returns a superset of all tags used in the samples of the collection"""
+        available_tags = defaultdict(set)
+        for sample in self.info:
+            for k, v in self._sampleTags(sample).items():
+                available_tags[k].add(v)
+        return dict(available_tags)
+
+    def report(self):
+        """return a report on the samples in the collection"""
+        tags = list(self.available_tags().keys())
+        header = ["id", "total_bytes", "nb_files"] + tags
+        values = [header]
+        for sample in self.info:
+            row = [sample["sample_id"], sample["total_bytes"]]
+            row.append(len(sample["lfns"].keys()))
+            sample_tags = self.tags[str(sample["sample_id"])]
+            for t in tags:
+                row.append(sample_tags.get(t, None))
+            values.append(row)
+        return values
+
+    def groupby(self, tags=None):
+        """Tool that takes the samples and groups them by the tags specified.
+        If no list of tags is specified, then the existing ones are used"""
+
+        report = self.report()
+        header = report[0]
+        data = report[1:]
+        if not tags:
+            tags = list(self.available_tags().keys())
+        else:
+            missing = [t for t in tags if t not in self.available_tags().keys()]
+            if missing:
+                raise ValueError(f"Tag(s): {','.join(missing)} not found!")
+
+        # preparing the function that lists the columns we should group on
+        sort_tags = set(tags) - set(("version", "name"))
+        sort_tag_ids = [i for i in range(len(header)) if header[i] in sort_tags]
+
+        def group_cols(row):
+            return [row[i] for i in sort_tag_ids]
+
+        # Now getting the values themselves (excluding the header) and sort
+        # as this is needed by itertools.groupby
+        data.sort(key=group_cols)
+        return {
+            tuple(key): list(group)
+            for key, group in itertools.groupby(data, group_cols)
+        }
```

### Comparing `apd-0.4.4/src/apd/authentication.py` & `apd-0.5.0/src/apd/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         token_file = _user_token_file()
         try:
             token = json.loads(token_file.read_text())
             _auth_ok(token)
         except Exception:  # pylint: disable=broad-except
             _login_sso(token_file)
             token = json.loads(token_file.read_text())
-    return dict(headers={"Authorization": f"Bearer {token}"})
+    return {"headers": {"Authorization": f"Bearer {token}"}}
 
 
 def logout():
     if "LBAP_TOKENS_FILE" in os.environ:
         tokens_file = Path(os.environ["LBAP_TOKENS_FILE"])
         tokens_file.unlink()
     token_file = _user_token_file()
@@ -146,15 +146,15 @@
         },
         verify=True,
         timeout=30,
     )
 
     if not r.ok:
         stderr(r.text)
-        raise Exception(
+        raise RuntimeError(
             "Authentication request failed: Device authorization response was not successful."
         )
 
     auth_response = r.json()
 
     stderr("CERN SINGLE SIGN-ON\n")
     stderr("On your tablet, phone or computer, go to:")
```

### Comparing `apd-0.4.4/src/apd/command.py` & `apd-0.5.0/src/apd/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 #
 # The command line tools use the click and click-log packages for easier development
 #
+import json
 import logging
 import os
 import sys
 import tempfile
+from pathlib import Path
 
 import click
 import click_log
 import requests
 
 from .analysis_data import (
     APD_DATA_CACHE_DIR,
     APD_METADATA_CACHE_DIR,
     APD_METADATA_LIFETIME,
+    AnalysisData,
     get_analysis_data,
 )
 from .ap_info import InvalidCacheError, cache_ap_info, load_ap_info
 from .authentication import get_auth_headers, logout
 from .data_cache import DataCache
 from .rich_console import console, error_console
 
@@ -35,21 +38,21 @@
 click_log.basic_config(logger)
 
 
 common_help = """
 Variables:
 
 APD_METADATA_CACHE_DIR: Specify the location of the information cache,
-    and reuse the cached information instead of reloading every time.
+and reuse the cached information instead of reloading every time.
 
 APD_METADATA_LIFETIME: Delay after which the cache should be considered
-    as invalid and reloaded.
+as invalid and reloaded.
 
 APD_DATA_CACHE_DIR: Specify the location of the location where a copy
-    of the files will be kept.
+of the files will be kept.
 """
 
 
 def common_docstr(sep="\n"):
     """
     Append the common help to all the functions docstring
     """
@@ -70,15 +73,15 @@
 sys.excepthook = exception_handler
 
 
 def setup_cache(cache_dir, working_group, analysis, ap_date=None):
     """Utility function that checks whether the data for the Analysis
     is cached already and does it if needed."""
     if not cache_dir:
-        cache_dir = "/tmp/apd_cache"
+        cache_dir = Path.home() / ".cache" / "apd"
         logger.debug("Cache directory not set, using %s", cache_dir)
     try:
         lifetime = os.environ.get(APD_METADATA_LIFETIME, None)
         load_ap_info(
             cache_dir,
             working_group,
             analysis,
@@ -154,15 +157,17 @@
 
 @click.command()
 @click.argument("cache_dir")
 @click.argument("working_group")
 @click.argument("analysis")
 @click.option("--date", default=None, help="analysis date in ISO 8601 format")
 @click_log.simple_verbosity_option(logger)
+@common_docstr()
 def cmd_cache_ap_info(cache_dir, working_group, analysis, date):
+    """Cache the metadata for analysis production specified."""
     logger.debug(
         "Caching information for %s/%s to %s for time %s",
         working_group,
         analysis,
         cache_dir,
         date,
     )
@@ -301,14 +306,69 @@
 @click.argument("analysis")
 @click.option(
     "--cache_dir",
     default=os.environ.get(APD_METADATA_CACHE_DIR, None),
     help="Specify location of the cache for the analysis metadata",
 )
 @click.option(
+    "--output",
+    default=None,
+    help="Specify output file for the csv file",
+)
+@click.option(
+    "--groupby",
+    default=None,
+    help="Column list (comma separated) by which the dataset should be grouped (or 'all')",
+)
+@click_log.simple_verbosity_option(logger)
+def cmd_dump_info(working_group, analysis, cache_dir, output, groupby):
+    """Dump the known information about a specific analysis"""
+
+    # Dealing with the cache
+    setup_cache(cache_dir, working_group, analysis)
+
+    # Loading the data first
+    datasets = AnalysisData(working_group, analysis, metadata_cache=cache_dir)
+
+    # Checking whether we need to group the data...
+    if groupby:
+        groupby_tags = [t.strip().lower() for t in groupby.split(",")]
+        # Special case where we use all the tags available except name and version
+        if "all" in groupby_tags:
+            groupby_tags = None
+
+        groups = datasets.samples.groupby(groupby_tags)
+        if output:
+            with open(output, "w") as f:
+                json.dump({str(k): v for k, v in groups.items()}, f)
+        else:
+            for k, v in groups.items():
+                print(",".join(k))
+                for line in v:
+                    print(" " * 8 + str(line))
+    else:
+        report = datasets.samples.report()
+        # gets the report as CSV in this case, not JSON
+        report_str = "\n".join(([",".join([str(e) for e in line]) for line in report]))
+        if output:
+            with open(output, "w") as f:
+                f.write(report_str)
+        else:
+            print(report_str)
+
+
+@click.command()
+@click.argument("working_group")
+@click.argument("analysis")
+@click.option(
+    "--cache_dir",
+    default=os.environ.get(APD_METADATA_CACHE_DIR, None),
+    help="Specify location of the cached analysis data files",
+)
+@click.option(
     "--tag",
     default=None,
     help="Tag for which the values should be listed",
     multiple=True,
 )
 @click.option("--date", default=None, help="analysis date in ISO 8601 format")
 @click_log.simple_verbosity_option(logger)
@@ -338,15 +398,15 @@
 
 
 @click.command()
 @click.argument("working_group")
 @click.argument("analysis")
 @click.option(
     "--cache_dir",
-    default=os.environ.get(APD_METADATA_CACHE_DIR, None),
+    default=os.environ.get("APD_METADATA_CACHE_DIR", None),
     help="Specify location of the cache for the analysis metadata",
 )
 @click.option(
     "--data_cache_dir",
     default=os.environ.get(APD_DATA_CACHE_DIR, None),
     help="Specify location of the cache for the analysis metadata",
 )
@@ -370,60 +430,56 @@
 )
 @click.option(
     "--datatype", default=None, help="datatype to filter the datasets", multiple=True
 )
 @click.option(
     "--polarity", default=None, help="polarity to filter the datasets", multiple=True
 )
+@click.option(
+    "--config", default=None, help="Config to use (e.g. lhcb or mc)", multiple=True
+)
 @click.option("--name", default=None, help="dataset name")
 @click.option("--version", default=None, help="dataset version")
 @click.option("--date", default=None, help="analysis date in ISO 8601 format")
 @click_log.simple_verbosity_option(logger)
 @common_docstr()
-def cmd_cache_pfns(
+def cmd_cache_ap_files(
     working_group,
     analysis,
     cache_dir,
     data_cache_dir,
     dry_run,
     tag,
     value,
     eventtype,
     datatype,
     polarity,
+    config,
     name,
     version,
     date,
 ):
-    """List the PFNs for the analysis, matching the tags specified.
+    """Cache the files for the analysis locally, matching the tags specified.
     This command checks that the arguments are not ambiguous."""
     # pylint: disable-msg=too-many-locals
     cache_dir = setup_cache(cache_dir, working_group, analysis, date)
 
     if not data_cache_dir:
-        raise Exception("Please specify the location of the data cache")
+        raise ValueError("Please specify the location of the data cache")
     data_cache = DataCache(data_cache_dir)
     # Loading the data and filtering/displaying
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
     )
-    filter_tags = {}
-    if name is not None:
-        filter_tags["name"] = name
-    if version is not None:
-        filter_tags["version"] = version
-    if eventtype != ():
-        filter_tags["eventtype"] = eventtype
-    if datatype != ():
-        filter_tags["datatype"] = datatype
-    if polarity != ():
-        filter_tags["polarity"] = polarity
+    filter_tags = filter_tags = _process_common_tags(
+        eventtype, datatype, polarity, config, name, version
+    )
     filter_tags |= dict(zip(tag, value))
 
-    for f in datasets(check_data=False, **filter_tags):
+    for f in datasets(check_data=False, use_local_cache=False, **filter_tags):
         local = data_cache.remote_to_local(f)
         if dry_run:
             print(str(f))
             if local.exists():
                 click.echo(f"Already local for {f}: {str(local)}")
             click.echo(f"Would copy {f} to {data_cache.remote_to_local(f)}")
         else:
```

### Comparing `apd-0.4.4/src/apd/data_cache.py` & `apd-0.5.0/src/apd/data_cache.py`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/src/apd/eos.py` & `apd-0.5.0/src/apd/eos.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,16 +39,23 @@
         msg += f"    * {eos_token['path']}"
         if not eos_token["allow_write"]:
             msg += " (readonly)"
         msg += "\n"
     raise ValueError(msg)
 
 
-def add_token_to_url(url: str, allow_write: bool) -> str:
+def add_token_to_url(url: str, allow_write: bool, ignore_nonroot: bool = True) -> str:
+    original_url = url
     url = urlparse.urlparse(url)
+
+    # skip the files not on root if requested
+    if ignore_nonroot:
+        if not url.scheme or url.scheme == "file":
+            return original_url
+
     token = _find_suitable_token(PurePosixPath(url.path), allow_write)
     token = urlparse.unquote(token)
     url_parts = list(url)
     url_parts[4] = urlparse.urlencode(
         dict(urlparse.parse_qsl(url_parts[4]))
         | {"xrd.wantprot": "unix", "authz": token}
     )
@@ -63,19 +70,19 @@
         r"(&authz=[^&#]+?)((?:%3D){1,3})",
         lambda x: x.groups()[0] + x.groups()[1].lower(),
         url_with_token,
     )
     return url_with_token
 
 
-def auth(url: str) -> str:
+def auth(url: str, ignore_nonroot: bool = True) -> str:
     """Take a PFN and return one with read-only credentials appended"""
     if "LBAP_TOKENS_FILE" in os.environ:
-        return add_token_to_url(url, False)
+        return add_token_to_url(url, False, ignore_nonroot=ignore_nonroot)
     return url
 
 
-def authw(url: str) -> str:
+def authw(url: str, ignore_nonroot: bool = True) -> str:
     """Take a PFN and return one with read-write credentials appended"""
     if "LBAP_TOKENS_FILE" in os.environ:
-        return add_token_to_url(url, True)
+        return add_token_to_url(url, True, ignore_nonroot=ignore_nonroot)
     return url
```

### Comparing `apd-0.4.4/src/apd/rich_console.py` & `apd-0.5.0/src/apd/rich_console.py`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/src/apd.egg-info/PKG-INFO` & `apd-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 Metadata-Version: 2.1
 Name: apd
-Version: 0.4.4
+Version: 0.5.0
 Summary: Tool to access the Analysis production Data
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Provides-Extra: testing
 License-File: LICENSE
 
 Analysis Production Data
 ========================
 
-*EXPERIMENTAL* prototype of python module to fulfill:
+*EXPERIMENTAL* prototype of Python module to fulfill DPA's grand task https://gitlab.cern.ch/lhcb-dpa/project/-/issues/134.
 
-https://gitlab.cern.ch/lhcb-dpa/project/-/issues/134
-
-Design
-======
-
-Analysis Production information endpoint
-----------------------------------------
-
-This module allows downloading and using Analysis Production information
-from the endpoint *https://lbap.app.cern.ch/*
-
-Details about the endpoint can be found at:
-
-https://lbap.app.cern.ch/docs#/stable
-
-BEWARE: The endpoint is experimental and can be interrupted at any time.
 
 Usage
 =====
 
-From python
+The `apd` package is available in the ``lb-conda default`` environment.
+
+From Python
 -----------
 
-The python module allows interacting from analysis scripts, doing e.g.
+The Python module allows interacting from analysis scripts, doing e.g.
 
 ::
 
    In [8]: import apd
 
    In [9]: datasets = apd.AnalysisData("SL", "RDs")
 
@@ -78,7 +64,21 @@
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000004_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000005_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000006_1.bsntuple_mc.root
    root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/MC/2016/BSNTUPLE_MC.ROOT/00110984/0000/00110984_00000007_1.bsntuple_mc.root
 
 The *apd-cache* command allows caching the Analysis metadata to a
 specific location.
+
+
+Design
+======
+
+Analysis Production information endpoint
+----------------------------------------
+
+This module allows downloading and using Analysis Productions information
+from the endpoint *https://lbap.app.cern.ch/*
+
+Details about the endpoint can be found at https://lbap.app.cern.ch/docs#/stable.
+
+BEWARE: The endpoint is experimental and can be interrupted at any time.
```

### Comparing `apd-0.4.4/src/apd.egg-info/SOURCES.txt` & `apd-0.5.0/src/apd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/apd/analysis_data.py
 src/apd/ap_info.py
 src/apd/authentication.py
 src/apd/command.py
 src/apd/data_cache.py
 src/apd/eos.py
 src/apd/rich_console.py
+src/apd/snakemake.py
 src/apd.egg-info/PKG-INFO
 src/apd.egg-info/SOURCES.txt
 src/apd.egg-info/dependency_links.txt
 src/apd.egg-info/entry_points.txt
 src/apd.egg-info/requires.txt
 src/apd.egg-info/top_level.txt
 tests/conftest.py
```

### Comparing `apd-0.4.4/tests/cache-dir/b2oc/b02dkpi/tags.json` & `apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/tags.json`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/tests/cache-dir/b2oc/b02dkpi.json` & `apd-0.5.0/tests/cache-dir/b2oc/b02dkpi.json`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/tests/conftest.py` & `apd-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/tests/data/rds_ap_info.json` & `apd-0.5.0/tests/data/rds_ap_info.json`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/tests/data/rds_ap_info_2versions.json` & `apd-0.5.0/tests/data/rds_ap_info_2versions.json`

 * *Files identical despite different names*

### Comparing `apd-0.4.4/tests/test_analysis_data.py` & `apd-0.5.0/tests/test_analysis_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,7 +83,20 @@
 
 
 def test_summary(apinfo_multipleversions):
     datasets = AnalysisData("SL", "RDs", metadata_cache=apinfo_multipleversions)
     tagname = "datatype"
     dt = set(datasets.summary([tagname])["tags"][tagname])
     assert dt == set(["2011", "2018", "2016", "2017", "2012"])
+
+
+def test_badtag(apinfo_cache):
+    """In case we specify a tag that does not exist an exception should be thrown"""
+    datasets = AnalysisData("SL", "RDs", metadata_cache=apinfo_cache)
+    with pytest.raises(ValueError):
+        datasets(badtag="novalue")
+
+
+def test_badtag_constructor(apinfo_cache):
+    """In case we specify a tag that does not exist an exception should be thrown"""
+    with pytest.raises(ValueError):
+        AnalysisData("SL", "RDs", metadata_cache=apinfo_cache, badtag="novalue")
```

### Comparing `apd-0.4.4/tests/test_ap_info.py` & `apd-0.5.0/tests/test_ap_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,13 @@
 
 def test_filter_samples_tuple(apinfo):
     pi = apinfo.filter(datatype=("2012", "2016"))
     assert len(pi) == 4
 
 
 def test_filter_samples_callable(apinfo):
-
     # from tabulate import tabulate
     # print("\n"+tabulate(pi.list_metadata(with_header=True)))
     assert len(apinfo.PFNs()) == 58
 
     fpi = apinfo.filter("polarity", lambda x: "magdown" in x)
     assert len(fpi.PFNs()) == 25
```

### Comparing `apd-0.4.4/tests/test_b2oc.py` & `apd-0.5.0/tests/test_b2oc.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     pfns = datasets(version="v0r0p2518507", name="2018_15164022_magup")
     assert len(pfns) == 6
 
     pfns = datasets(version="v0r0p2970193", name="2018_15164022_magup")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
-    with pytest.raises(Exception, match="version argument doesn't support iterables"):
+    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
         datasets(version=["v0r0p2518507", "v0r0p2970193"], name="2018_15164022_magup")
 
-    with pytest.raises(Exception, match="version argument doesn't support iterables"):
+    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
         datasets(version={"v0r0p2518507", "v0r0p2970193"}, name="2018_15164022_magup")
 
     pfns = set(
         datasets(
             version="v0r0p2970193",
             name=["2018_15164022_magup", "2018_15164022_magdown"],
         )
@@ -63,29 +63,29 @@
     pfns = datasets(name="2018_15164022_magup")
     assert len(pfns) == 6
 
     datasets = AnalysisData("b2oc", "b02dkpi", version="v0r0p2970193")
     pfns = datasets(name="2018_15164022_magup")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
-    with pytest.raises(Exception, match="version argument doesn't support iterables"):
+    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
         AnalysisData("b2oc", "b02dkpi", version=["v0r0p2518507", "v0r0p2970193"])
-    with pytest.raises(Exception, match="version argument doesn't support iterables"):
+    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
         AnalysisData("b2oc", "b02dkpi", version={"v0r0p2518507", "v0r0p2970193"})
 
 
 def test_defaults_name(apd_cache):
     with pytest.raises(
-        Exception, match="name is not supported on AnalysisData objects"
+        ValueError, match="name is not a supported tag in AnalysisData objects"
     ):
         AnalysisData(
             "b2oc", "b02dkpi", version="v0r0p2518507", name="2018_15164022_magup"
         )
     with pytest.raises(
-        Exception, match="name is not supported on AnalysisData objects"
+        ValueError, match="name is not a supported tag in AnalysisData objects"
     ):
         AnalysisData("b2oc", "b02dkpi", name="2018_15164022_magup")
 
 
 def test_defaults_tag_override(apd_cache):
     datasets = AnalysisData(
         "b2oc", "b02dkpi", datatype=2018, polarity=["magup", "magdown"]
@@ -102,15 +102,15 @@
 
     pfns = datasets(version="v0r0p2970193", eventtype="15164022", polarity="magup")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
     pfns = datasets(version="v0r0p2970193", eventtype=15164022, polarity="MagUp")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
-    with pytest.raises(Exception, match="Error"):  # TODO: This should be more specific
+    with pytest.raises(ValueError, match="Error"):  # TODO: This should be more specific
         datasets(eventtype=15164022, polarity="magup")
 
 
 def test_by_tag_single(apd_cache):
     datasets = AnalysisData("b2oc", "b02dkpi")
 
     pfns = datasets(datatype="2011", eventtype="11164047", polarity="magdown")
@@ -133,15 +133,15 @@
 
     pfns = datasets(
         version="v0r0p2970193", datatype="2018", eventtype=15164022, polarity="MagUp"
     )
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
     with pytest.raises(
-        Exception, match=r"Error loading data: 1 problem\(s\) found"
+        ValueError, match=r"Error loading data: 1 problem\(s\) found"
     ):  # TODO: This should be more specific
         datasets(datatype="2018", eventtype=15164022, polarity="magup")
 
 
 def test_by_tag_multiple(apd_cache):
     datasets = AnalysisData("b2oc", "b02dkpi")
 
@@ -163,20 +163,20 @@
                 "00128212_0000",
             ]
         )
         for x in pfns
     )
 
     with pytest.raises(
-        Exception, match=r"Error loading data: 4 problem\(s\) found"
+        ValueError, match=r"Error loading data: 4 problem\(s\) found"
     ):  # TODO: This should be more specific
         datasets(datatype=["2012", "2011"], polarity=["magup", "magdown"])
 
     with pytest.raises(
-        Exception, match=r"Error loading data: 2 problem\(s\) found"
+        ValueError, match=r"Error loading data: 2 problem\(s\) found"
     ):  # TODO: This should be more specific
         datasets(datatype=["2015", "2016"], polarity=["magoff"])
 
     pfns = datasets(datatype=["2015", "2016"], polarity=["magup", "magdown"], mc=False)
     assert len(pfns) == 519 and all(
         any(
             y in x for y in ["00121802_00", "00121816_00", "00121814_00", "00121794_00"]
```

### Comparing `apd-0.4.4/tests/test_data_cache.py` & `apd-0.5.0/tests/test_data_cache.py`

 * *Files identical despite different names*

