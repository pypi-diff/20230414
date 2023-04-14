# Comparing `tmp/cacholote-0.2.2.tar.gz` & `tmp/cacholote-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.2.2.tar", last modified: Mon Feb 27 10:31:47 2023, max compression
+gzip compressed data, was "cacholote-0.3.0.tar", last modified: Fri Apr 14 07:36:44 2023, max compression
```

## Comparing `cacholote-0.2.2.tar` & `cacholote-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.851345 cacholote-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-27 10:31:28.000000 cacholote-0.2.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.827345 cacholote-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.835345 cacholote-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-02-27 10:31:28.000000 cacholote-0.2.2/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-02-27 10:31:28.000000 cacholote-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-27 10:31:28.000000 cacholote-0.2.2/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-27 10:31:28.000000 cacholote-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-27 10:31:28.000000 cacholote-0.2.2/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-27 10:31:28.000000 cacholote-0.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-02-27 10:31:28.000000 cacholote-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-27 10:31:28.000000 cacholote-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-27 10:31:28.000000 cacholote-0.2.2/OBJECT-STORAGE-DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-02-27 10:31:47.851345 cacholote-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-02-27 10:31:28.000000 cacholote-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.839345 cacholote-0.2.2/cacholote/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-02-27 10:31:28.000000 cacholote-0.2.2/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.843345 cacholote-0.2.2/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-27 10:31:47.000000 cacholote-0.2.2/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.843345 cacholote-0.2.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-27 10:31:28.000000 cacholote-0.2.2/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-27 10:31:28.000000 cacholote-0.2.2/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.847345 cacholote-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.847345 cacholote-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.847345 cacholote-0.2.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-27 10:31:28.000000 cacholote-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-27 10:31:28.000000 cacholote-0.2.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-27 10:31:28.000000 cacholote-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 10:31:47.851345 cacholote-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:31:47.851345 cacholote-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-02-27 10:31:28.000000 cacholote-0.2.2/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.774470 cacholote-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 07:36:30.000000 cacholote-0.3.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.766470 cacholote-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-14 07:36:30.000000 cacholote-0.3.0/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-14 07:36:30.000000 cacholote-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 07:36:30.000000 cacholote-0.3.0/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 07:36:30.000000 cacholote-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-14 07:36:30.000000 cacholote-0.3.0/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 07:36:30.000000 cacholote-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-14 07:36:30.000000 cacholote-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 07:36:30.000000 cacholote-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 07:36:30.000000 cacholote-0.3.0/OBJECT-STORAGE-DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-04-14 07:36:44.774470 cacholote-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-14 07:36:30.000000 cacholote-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-14 07:36:30.000000 cacholote-0.3.0/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-14 07:36:30.000000 cacholote-0.3.0/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 07:36:30.000000 cacholote-0.3.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 07:36:30.000000 cacholote-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:36:44.774470 cacholote-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_60_clean.py
```

### Comparing `cacholote-0.2.2/.cruft.json` & `cacholote-0.3.0/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'23164e60b3e44472716d3d46bcd3ef47bbf2e79a'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "1b0360c571d754905484199eca2d203a3d0aada2",
+    "commit": "23164e60b3e44472716d3d46bcd3ef47bbf2e79a",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "B-Open Solutions srl",
             "copyright_year": "2019",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cacholote-0.2.2/.github/workflows/on-push.yml` & `cacholote-0.3.0/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/.gitignore` & `cacholote-0.3.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -289,14 +289,24 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+### Python Patch ###
+# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
+poetry.toml
+
+# ruff
+.ruff_cache/
+
+# LSP config files
+pyrightconfig.json
+
 ### Vim ###
 # Swap
 [._]*.s[a-v][a-z]
 !*.svg  # comment out if you don't need vector files
 [._]*.sw[a-p]
 [._]s[a-rt-v][a-z]
 [._]ss[a-gi-z]
@@ -330,14 +340,11 @@
 *.vsix
 
 ### VisualStudioCode Patch ###
 # Ignore all local history of files
 .history
 .ionide
 
-# Support for Project snippet scope
-.vscode/*.code-snippets
-
 # Ignore code-workspaces
 *.code-workspace
 
 # End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
```

### Comparing `cacholote-0.2.2/.pre-commit-config.yaml` & `cacholote-0.3.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -7,31 +7,31 @@
   - id: check-json
   - id: check-yaml
   - id: check-toml
   - id: check-added-large-files
   - id: debug-statements
   - id: mixed-line-ending
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.252
+  rev: v0.0.260
   hooks:
   - id: ruff
     args: [--fix]
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.16
   hooks:
   - id: mdformat
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.7.0
+  rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
```

### Comparing `cacholote-0.2.2/DESIGN.rst` & `cacholote-0.3.0/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/LICENSE` & `cacholote-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/Makefile` & `cacholote-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.3.0/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/PKG-INFO` & `cacholote-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.2.2
+Version: 0.3.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.2.2/README.md` & `cacholote-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/cacholote/__init__.py` & `cacholote-0.3.0/cacholote/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import config, database, extra_encoders, utils
 from .cache import cacheable
-from .clean import clean_cache_files
+from .clean import clean_cache_files, delete
 from .decode import loads
 from .encode import dumps
 
 try:
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
     from .version import __version__
@@ -33,12 +33,13 @@
 
 __all__ = [
     "__version__",
     "cacheable",
     "clean_cache_files",
     "config",
     "database",
+    "delete",
     "dumps",
     "extra_encoders",
     "loads",
     "utils",
 ]
```

### Comparing `cacholote-0.2.2/cacholote/cache.py` & `cacholote-0.3.0/cacholote/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import functools
 import json
 import warnings
-from typing import Any, Callable, TypeVar, Union, cast
+from typing import Any, Callable, TypeVar, cast
 
 import sqlalchemy
 import sqlalchemy.orm
 
-from . import clean, config, database, decode, encode, utils
+from . import clean, config, database, decode, encode
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def _decode_and_update(
     session: sqlalchemy.orm.Session,
     cache_entry: Any,
@@ -41,44 +41,26 @@
     database._commit_or_rollback(session)
     if settings.return_cache_entry:
         session.refresh(cache_entry)
         return cache_entry
     return result
 
 
-def _delete_cache_entry(
-    session: sqlalchemy.orm.Session, cache_entry: database.CacheEntry
-) -> None:
-    # First, delete database entry
-    session.delete(cache_entry)
-    database._commit_or_rollback(session)
-    # Then, delete files
-    json.loads(cache_entry._result_as_string, object_hook=clean._delete_cache_file)
-
-
-def _hexdigestify_python_call(
-    func_to_hex: Union[str, Callable[..., Any]],
-    *args: Any,
-    **kwargs: Any,
-) -> str:
-    return utils.hexdigestify(encode.dumps_python_call(func_to_hex, *args, **kwargs))
-
-
 def cacheable(func: F) -> F:
     """Make a function cacheable."""
 
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         settings = config.get()
 
         if not settings.use_cache:
             return func(*args, **kwargs)
 
         try:
-            hexdigest = _hexdigestify_python_call(func, *args, **kwargs)
+            hexdigest = encode._hexdigestify_python_call(func, *args, **kwargs)
         except encode.EncodeError as ex:
             if settings.return_cache_entry:
                 raise ex
             warnings.warn(f"can NOT encode python call: {ex!r}", UserWarning)
             return func(*args, **kwargs)
 
         filters = [
@@ -95,15 +77,15 @@
                 .filter(*filters)
                 .order_by(database.CacheEntry.timestamp.desc())
             ):
                 try:
                     return _decode_and_update(session, cache_entry, settings)
                 except decode.DecodeError as ex:
                     warnings.warn(str(ex), UserWarning)
-                    _delete_cache_entry(session, cache_entry)
+                    clean._delete_cache_entry(session, cache_entry)
 
         result = func(*args, **kwargs)
         cache_entry = database.CacheEntry(
             key=hexdigest,
             expiration=settings.expiration,
             tag=settings.tag,
         )
```

### Comparing `cacholote-0.2.2/cacholote/clean.py` & `cacholote-0.3.0/cacholote/clean.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import collections
 import datetime
 import functools
 import json
 import posixpath
-from typing import Any, Dict, Literal, Optional, Sequence, Set
+from typing import Any, Callable, Dict, Literal, Optional, Sequence, Set, Union
 
 import sqlalchemy
 import sqlalchemy.orm
 import structlog
 
-from . import config, database, extra_encoders, utils
+from . import config, database, encode, extra_encoders, utils
 
 LOGGER = structlog.get_logger()
 
 
 def _delete_cache_file(
     obj: Dict[str, Any],
     session: Optional[sqlalchemy.orm.Session] = None,
@@ -56,40 +57,84 @@
                 logger.info("Delete cache entry", cache_entry=cache_entry)
                 session.delete(cache_entry)
                 database._commit_or_rollback(session)
             if not dry_run:
                 with utils._Locker(fs, urlpath) as file_exists:
                     if file_exists:
                         logger.info("Delete cache file", urlpath=urlpath)
-                        fs.rm(urlpath, recursive=True)
+                        fs.rm(
+                            urlpath,
+                            recursive=obj["args"][0]["type"] == "application/vnd+zarr",
+                        )
 
     return obj
 
 
+def _delete_cache_entry(
+    session: sqlalchemy.orm.Session, cache_entry: database.CacheEntry
+) -> None:
+    # First, delete database entry
+    session.delete(cache_entry)
+    database._commit_or_rollback(session)
+    # Then, delete files
+    json.loads(cache_entry._result_as_string, object_hook=_delete_cache_file)
+
+
+def delete(
+    func_to_del: Union[str, Callable[..., Any]], *args: Any, **kwargs: Any
+) -> None:
+    """Delete function previously cached.
+
+    Parameters
+    ----------
+    func_to_del: callable, str
+        Function to delete from cache
+    *args: Any
+        Argument of functions to delete from cache
+    **kwargs: Any
+        Keyword arguments of functions to delete from cache
+    """
+    hexdigest = encode._hexdigestify_python_call(func_to_del, *args, **kwargs)
+    with config.get().sessionmaker() as session:
+        for cache_entry in session.query(database.CacheEntry).filter(
+            database.CacheEntry.key == hexdigest
+        ):
+            _delete_cache_entry(session, cache_entry)
+
+
 class _Cleaner:
     def __init__(self, logger: structlog.stdlib.BoundLogger) -> None:
-        self.logger = logger
-
         fs, dirname = utils.get_cache_files_fs_dirname()
-        sizes = {fs.unstrip_protocol(path): fs.du(path) for path in fs.ls(dirname)}
+        urldir = fs.unstrip_protocol(dirname)
+
+        logger.info("Get disk usage of cache files")
+        sizes: Dict[str, int] = collections.defaultdict(lambda: 0)
+        for path, size in fs.du(dirname, total=False).items():
+            # Group dirs
+            urlpath = fs.unstrip_protocol(path)
+            basename, *_ = urlpath.replace(urldir, "", 1).strip("/").split("/")
+            if basename:
+                sizes[posixpath.join(urldir, basename)] += size
 
+        self.logger = logger
         self.fs = fs
         self.dirname = dirname
         self.sizes = sizes
 
     @property
     def size(self) -> int:
-        return sum(self.sizes.values())
+        sum_sizes = sum(self.sizes.values())
+        self.logger.info("Check cache files total size", size=sum_sizes)
+        return sum_sizes
 
     def stop_cleaning(self, maxsize: int) -> bool:
-        size = self.size
-        self.logger.info("Check cache files size", size=self.size)
-        return size <= maxsize
+        return self.size <= maxsize
 
     def get_unknown_files(self, lock_validity_period: Optional[float]) -> Set[str]:
+        self.logger.info("Get unknown files")
         now = datetime.datetime.now()
         files_to_skip = []
         for urlpath in self.sizes:
             if urlpath.endswith(".lock"):
                 delta = now - self.fs.modified(urlpath)
                 if lock_validity_period is None or delta < datetime.timedelta(
                     seconds=lock_validity_period
@@ -108,24 +153,25 @@
                             sizes=unknown_sizes,
                             dry_run=True,
                             logger=self.logger,
                         ),
                     )
         return set(unknown_sizes)
 
-    def delete_unknown_files(self, lock_validity_period: Optional[float]) -> None:
+    def delete_unknown_files(
+        self, lock_validity_period: Optional[float], recursive: bool
+    ) -> None:
         for urlpath in self.get_unknown_files(lock_validity_period):
             self.sizes.pop(urlpath)
-            if not self.fs.exists(urlpath):
-                continue
-
             with utils._Locker(self.fs, urlpath, lock_validity_period) as file_exists:
                 if file_exists:
-                    self.logger.info("Delete unkown file", urlpath=urlpath)
-                    self.fs.rm(urlpath)
+                    self.logger.info(
+                        "Delete unknown", urlpath=urlpath, recursive=recursive
+                    )
+                    self.fs.rm(urlpath, recursive=recursive)
 
     @staticmethod
     def check_tags(*args: Any) -> None:
         if None not in args:
             raise ValueError("tags_to_clean/keep are mutually exclusive.")
         for tags in args:
             if tags is not None and (
@@ -200,14 +246,15 @@
         )
 
 
 def clean_cache_files(
     maxsize: int,
     method: Literal["LRU", "LFU"] = "LRU",
     delete_unknown_files: bool = False,
+    recursive: bool = False,
     lock_validity_period: Optional[float] = None,
     tags_to_clean: Optional[Sequence[Optional[str]]] = None,
     tags_to_keep: Optional[Sequence[Optional[str]]] = None,
     logger: Optional[structlog.stdlib.BoundLogger] = None,
 ) -> None:
     """Clean cache files.
 
@@ -216,27 +263,29 @@
     maxsize: int
         Maximum total size of cache files (bytes).
     method: str, default: "LRU"
         * LRU: Last Recently Used
         * LFU: Least Frequently Used
     delete_unknown_files: bool, default: False
         Delete all files that are not registered in the cache database.
+    recursive: bool, default: False
+        Whether to delete unknown directories or not
     lock_validity_period: float, optional, default: None
         Validity period of lock files in seconds. Expired locks will be deleted.
     tags_to_clean, tags_to_keep: sequence of strings/None, optional, default: None
         Tags to clean/keep. If None, delete all cache entries.
         To delete/keep untagged entries, add None in the sequence (e.g., [None, 'tag1', ...]).
         tags_to_clean and tags_to_keep are mutually exclusive.
     logger: optional
         Python object use to produce logs.
     """
     cleaner = _Cleaner(logger=logger or LOGGER)
 
     if delete_unknown_files:
-        cleaner.delete_unknown_files(lock_validity_period)
+        cleaner.delete_unknown_files(lock_validity_period, recursive)
 
     cleaner.delete_cache_files(
         maxsize=maxsize,
         method=method,
         tags_to_clean=tags_to_clean,
         tags_to_keep=tags_to_keep,
     )
```

### Comparing `cacholote-0.2.2/cacholote/config.py` & `cacholote-0.3.0/cacholote/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,24 @@
     ] = "application/netcdf"
     io_delete_original: bool = False
     raise_all_encoding_errors: bool = False
     expiration: Optional[datetime.datetime] = None
     tag: Optional[str] = None
     return_cache_entry: bool = False
 
-    @pydantic.validator("return_cache_entry")
+    @pydantic.validator("create_engine_kwargs", allow_reuse=True)
+    def validate_create_engine_kwargs(
+        cls: pydantic.BaseSettings, create_engine_kwargs: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        poolclass = create_engine_kwargs.get("poolclass")
+        if isinstance(poolclass, str):
+            create_engine_kwargs["poolclass"] = getattr(sqlalchemy.pool, poolclass)
+        return create_engine_kwargs
+
+    @pydantic.validator("return_cache_entry", allow_reuse=True)
     def validate_return_cache_entry(
         cls: pydantic.BaseSettings, return_cache_entry: bool, values: Dict[str, Any]
     ) -> bool:
         if return_cache_entry is True and values["use_cache"] is False:
             raise ValueError(
                 "`use_cache` must be True when `return_cache_entry` is True"
             )
@@ -171,15 +180,15 @@
 
     Parameters
     ----------
     env_file: str, tuple[str], default=None
         Dot env file(s).
     """
     global _SETTINGS
-    _SETTINGS = Settings(_env_file=env_file)
+    _SETTINGS = Settings(_env_file=env_file)  # type: ignore[call-arg]
     set()
 
 
 def get() -> Settings:
     """Get cacholote settings."""
     if _SETTINGS is None:
         raise ValueError(_CONFIG_NOT_SET_MSG)
```

### Comparing `cacholote-0.2.2/cacholote/database.py` & `cacholote-0.3.0/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/cacholote/decode.py` & `cacholote-0.3.0/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/cacholote/encode.py` & `cacholote-0.3.0/cacholote/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,27 @@
 import datetime
 import inspect
 import json
 import pickle
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from . import config, decode
+from . import config, decode, utils
 
 _JSON_DUMPS_KWARGS: Dict[str, Any] = {"separators": (",", ":"), "skipkeys": False}
 
 
+def _hexdigestify_python_call(
+    func_to_hex: Union[str, Callable[..., Any]],
+    *args: Any,
+    **kwargs: Any,
+) -> str:
+    return utils.hexdigestify(dumps_python_call(func_to_hex, *args, **kwargs))
+
+
 def inspect_fully_qualified_name(obj: Callable[..., Any]) -> str:
     """Return the fully qualified name of a python object."""
     module = inspect.getmodule(obj)
     if module is None:
         raise ValueError(f"can't getmodule for {obj!r}")
     return f"{module.__name__}:{obj.__qualname__}"
```

### Comparing `cacholote-0.2.2/cacholote/extra_encoders.py` & `cacholote-0.3.0/cacholote/extra_encoders.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/cacholote/utils.py` & `cacholote-0.3.0/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/cacholote.egg-info/PKG-INFO` & `cacholote-0.3.0/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.2.2
+Version: 0.3.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.2.2/cacholote.egg-info/SOURCES.txt` & `cacholote-0.3.0/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/docs/Makefile` & `cacholote-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/docs/conf.py` & `cacholote-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/docs/make.bat` & `cacholote-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/pyproject.toml` & `cacholote-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/conftest.py` & `cacholote-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_01_settings.py` & `cacholote-0.3.0/tests/test_01_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pathlib
-from typing import Any, Dict
+from typing import Any, Dict, Union
 
 import pytest
+import sqlalchemy
 
 from cacholote import config
 
 
 def test_change_cache_db_urlpath(tmpdir: pathlib.Path) -> None:
     old_db = config.get().cache_db_urlpath
     new_db = "sqlite:///" + str(tmpdir / "dummy.db")
@@ -77,7 +78,15 @@
         assert config.get().cache_db_urlpath == "sqlite://"
         assert str(config.get().engine.url) == "sqlite://"
         assert config.get().io_delete_original is True
         assert str(config.get().engine.url) == "sqlite://"
     finally:
         os.environ.clear()
         os.environ.update(old_environ)
+
+
+@pytest.mark.parametrize("poolclass", ("NullPool", sqlalchemy.pool.NullPool))
+def test_set_poolclass(poolclass: Union[str, sqlalchemy.pool.Pool]) -> None:
+    config.set(create_engine_kwargs={"poolclass": poolclass})
+    settings = config.get()
+    assert settings.create_engine_kwargs["poolclass"] == sqlalchemy.pool.NullPool
+    assert isinstance(settings.engine.pool, sqlalchemy.pool.NullPool)
```

### Comparing `cacholote-0.2.2/tests/test_02_utils.py` & `cacholote-0.3.0/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_10_decode.py` & `cacholote-0.3.0/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_20_encode.py` & `cacholote-0.3.0/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_30_cache.py` & `cacholote-0.3.0/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_40_xarray_encoder.py` & `cacholote-0.3.0/tests/test_40_xarray_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_50_io_encoder.py` & `cacholote-0.3.0/tests/test_50_io_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.2.2/tests/test_60_clean.py` & `cacholote-0.3.0/tests/test_60_clean.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import contextlib
 import pathlib
 from typing import Any, Literal, Optional, Sequence
 
 import fsspec
 import pytest
 
 from cacholote import cache, clean, config, utils
 
+does_not_raise = contextlib.nullcontext
+
 
 @cache.cacheable
 def open_url(url: pathlib.Path) -> fsspec.spec.AbstractBufferedFile:
     with fsspec.open(url) as f:
         return f
 
 
@@ -72,14 +75,32 @@
     if delete_unknown_files:
         file_hash = f"{fs.checksum(tmpfile):x}"
         assert fs.ls(dirname) == [f"{dirname}/{file_hash}.txt"]
     else:
         assert fs.ls(dirname) == [f"{dirname}/unknown.txt"]
 
 
+@pytest.mark.parametrize(
+    "recursive,raises,final_size",
+    [
+        (True, does_not_raise(), 0),
+        (False, pytest.raises((PermissionError, IsADirectoryError)), 1),
+    ],
+)
+def test_delete_unknown_dirs(
+    recursive: bool, raises: contextlib.nullcontext, final_size: int  # type: ignore[type-arg]
+) -> None:
+    fs, dirname = utils.get_cache_files_fs_dirname()
+    fs.mkdir(f"{dirname}/unknown")
+    fs.touch(f"{dirname}/unknown/unknown.txt")
+    with raises:
+        clean.clean_cache_files(0, delete_unknown_files=True, recursive=recursive)
+    assert len(fs.ls(dirname)) == final_size
+
+
 @pytest.mark.parametrize("lock_validity_period", [None, 0])
 def test_clean_locked_files(
     tmpdir: pathlib.Path, lock_validity_period: Optional[float]
 ) -> None:
     fs, dirname = utils.get_cache_files_fs_dirname()
 
     # Create file
@@ -143,17 +164,38 @@
         match="tags_to_clean/keep are mutually exclusive.",
     ):
         clean.clean_cache_files(1, tags_to_keep=[], tags_to_clean=[])
 
 
 @pytest.mark.parametrize("wrong_type", ["1", [1]])
 def test_clean_tagged_files_wrong_types(wrong_type: Any) -> None:
-    with pytest.raises(
+    raises = pytest.raises(
         TypeError,
         match="tags_to_clean/keep must be None or a sequence of str/None.",
-    ):
+    )
+    with raises:
         clean.clean_cache_files(1, tags_to_keep=wrong_type)
-    with pytest.raises(
-        TypeError,
-        match="tags_to_clean/keep must be None or a sequence of str/None.",
-    ):
+    with raises:
         clean.clean_cache_files(1, tags_to_clean=wrong_type)
+
+
+def test_delete_cache_entry_and_files(tmpdir: pathlib.Path) -> None:
+    fs, dirname = utils.get_cache_files_fs_dirname()
+
+    # Create file
+    tmpfile = tmpdir / "test.txt"
+    fsspec.filesystem("file").pipe_file(tmpfile, b"old")
+
+    # Copy to cache
+    open_url(tmpfile)
+
+    # Change tmp file
+    fsspec.filesystem("file").pipe_file(tmpfile, b"new")
+    assert open_url(tmpfile).read() == b"old"
+
+    # Delete cache entry
+    clean.delete(open_url, tmpfile)
+    assert fs.ls(dirname) == []
+
+    # Cache again
+    assert open_url(tmpfile).read() == b"new"
+    assert len(fs.ls(dirname)) == 1
```

