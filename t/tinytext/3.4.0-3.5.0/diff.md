# Comparing `tmp/tinytext-3.4.0.tar.gz` & `tmp/tinytext-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Fri Apr 14 11:07:39 2023, max compression
```

## Comparing `tinytext-3.4.0.tar` & `tinytext-3.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinytext-3.4.0/.coveragerc
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinytext-3.4.0/.flake8
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinytext-3.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 tinytext-3.4.0/.zenodo.json
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tinytext-3.4.0/RELEASING.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinytext-3.4.0/codecov.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tinytext-3.4.0/requirements.txt
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tinytext-3.4.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/labels.yml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/renovate.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 tinytext-3.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 tinytext-3.4.0/src/tinytext/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tinytext-3.4.0/src/tinytext/__main__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tinytext-3.4.0/src/tinytext/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinytext-3.4.0/tests/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tinytext-3.4.0/tests/test_tinytext.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tinytext-3.4.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tinytext-3.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 tinytext-3.4.0/README.md
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tinytext-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 tinytext-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0      329 2023-04-14 11:07:39.000000 tinytext-3.5.0/.coveragerc
+-rw-r--r--   0        0        0       30 2023-04-14 11:07:39.000000 tinytext-3.5.0/.flake8
+-rw-r--r--   0        0        0     1671 2023-04-14 11:07:39.000000 tinytext-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      505 2023-04-14 11:07:39.000000 tinytext-3.5.0/.zenodo.json
+-rw-r--r--   0        0        0      821 2023-04-14 11:07:39.000000 tinytext-3.5.0/RELEASING.md
+-rw-r--r--   0        0        0       34 2023-04-14 11:07:39.000000 tinytext-3.5.0/codecov.yml
+-rw-r--r--   0        0        0       77 2023-04-14 11:07:39.000000 tinytext-3.5.0/requirements.txt
+-rw-r--r--   0        0        0      502 2023-04-14 11:07:39.000000 tinytext-3.5.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      443 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1148 2023-04-14 11:07:39.000000 tinytext-3.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2045 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/__main__.py
+-rw-r--r--   0        0        0      494 2023-04-14 11:07:39.000000 tinytext-3.5.0/src/tinytext/cli.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:07:39.000000 tinytext-3.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-14 11:07:39.000000 tinytext-3.5.0/tests/test_tinytext.py
+-rw-r--r--   0        0        0     3077 2023-04-14 11:07:39.000000 tinytext-3.5.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-04-14 11:07:39.000000 tinytext-3.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1475 2023-04-14 11:07:39.000000 tinytext-3.5.0/README.md
+-rw-r--r--   0        0        0     1668 2023-04-14 11:07:39.000000 tinytext-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-04-14 11:07:39.000000 tinytext-3.5.0/PKG-INFO
```

### Comparing `tinytext-3.4.0/.pre-commit-config.yaml` & `tinytext-3.5.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
@@ -28,43 +28,44 @@
     hooks:
       - id: python-check-blanket-noqa
       - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
       - id: mypy
         args: [--strict, --pretty, --show-error-codes]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.6.0
+    rev: 0.9.2
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.6.1
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `tinytext-3.4.0/RELEASING.md` & `tinytext-3.5.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/.github/labels.yml` & `tinytext-3.5.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/.github/release-drafter.yml` & `tinytext-3.5.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/.github/workflows/release-drafter.yml` & `tinytext-3.5.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/.github/workflows/test.yml` & `tinytext-3.5.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.8", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
         os: [macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `tinytext-3.4.0/src/tinytext/__init__.py` & `tinytext-3.5.0/src/tinytext/__init__.py`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/.gitignore` & `tinytext-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/LICENSE.txt` & `tinytext-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/README.md` & `tinytext-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tinytext-3.4.0/pyproject.toml` & `tinytext-3.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -44,24 +44,21 @@
   'importlib-metadata; python_version < "3.8"',
 ]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
-
 [project.urls]
 Changelog = "https://github.com/hugovk/tinytext/releases"
 Homepage = "https://github.com/hugovk/tinytext"
 Source = "https://github.com/hugovk/tinytext"
-
 [project.scripts]
 tinytext = "tinytext.cli:main"
 
-
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
```

### Comparing `tinytext-3.4.0/PKG-INFO` & `tinytext-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinytext
-Version: 3.4.0
+Version: 3.5.0
 Summary: A helpful converter to change any normal text into cuter tinier text
 Project-URL: Changelog, https://github.com/hugovk/tinytext/releases
 Project-URL: Homepage, https://github.com/hugovk/tinytext
 Project-URL: Source, https://github.com/hugovk/tinytext
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
```

