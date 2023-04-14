# Comparing `tmp/yaml2ics-0.1rc3.tar.gz` & `tmp/yaml2ics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml2ics-0.1rc3.tar", last modified: Sun Aug 21 01:07:17 2022, max compression
+gzip compressed data, was "yaml2ics-0.2.tar", last modified: Fri Apr 14 05:57:07 2023, max compression
```

## Comparing `yaml2ics-0.1rc3.tar` & `yaml2ics-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      424 2022-08-20 14:51:08.962846 yaml2ics-0.1rc3/.flake8
--rw-r--r--   0        0        0      817 2022-08-20 14:51:08.962846 yaml2ics-0.1rc3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      847 2022-08-20 14:51:08.963846 yaml2ics-0.1rc3/.github/workflows/test.yml
--rw-r--r--   0        0        0      351 2022-08-20 14:51:08.963846 yaml2ics-0.1rc3/.gitignore
--rw-r--r--   0        0        0     1031 2022-08-20 14:51:08.963846 yaml2ics-0.1rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5090 2022-08-21 01:04:30.372543 yaml2ics-0.1rc3/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2022-08-20 14:51:08.963846 yaml2ics-0.1rc3/LICENSE
--rw-r--r--   0        0        0     2122 2022-08-20 14:51:08.963846 yaml2ics-0.1rc3/README.md
--rw-r--r--   0        0        0     1425 2022-08-20 14:51:08.964846 yaml2ics-0.1rc3/RELEASE.md
--rw-r--r--   0        0        0      180 2022-08-20 14:51:08.964846 yaml2ics-0.1rc3/example/another_calendar.yaml
--rw-r--r--   0        0        0     1565 2022-08-20 14:51:08.964846 yaml2ics-0.1rc3/example/test_calendar.yaml
--rw-r--r--   0        0        0      740 2022-08-21 01:04:56.855639 yaml2ics-0.1rc3/pyproject.toml
--rw-r--r--   0        0        0     5852 2022-08-20 14:51:08.965846 yaml2ics-0.1rc3/yaml2ics.py
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 yaml2ics-0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0      783 2023-04-14 05:32:23.927232 yaml2ics-0.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      817 2022-08-20 14:51:08.962846 yaml2ics-0.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      847 2022-08-20 14:51:08.963846 yaml2ics-0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      351 2022-08-20 14:51:08.963846 yaml2ics-0.2/.gitignore
+-rw-r--r--   0        0        0      939 2023-04-14 05:43:54.815037 yaml2ics-0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7543 2023-04-14 05:49:21.524121 yaml2ics-0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1539 2022-08-20 14:51:08.963846 yaml2ics-0.2/LICENSE
+-rw-r--r--   0        0        0     2352 2023-02-27 22:09:45.305546 yaml2ics-0.2/README.md
+-rw-r--r--   0        0        0     1405 2022-08-29 09:31:52.276291 yaml2ics-0.2/RELEASE.md
+-rw-r--r--   0        0        0      180 2022-08-20 14:51:08.964846 yaml2ics-0.2/example/another_calendar.yaml
+-rw-r--r--   0        0        0     1763 2023-02-01 16:12:40.899039 yaml2ics-0.2/example/test_calendar.yaml
+-rw-r--r--   0        0        0     1105 2023-04-14 05:53:51.208386 yaml2ics-0.2/pyproject.toml
+-rw-r--r--   0        0        0     6478 2023-02-27 22:09:45.306546 yaml2ics-0.2/yaml2ics.py
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 yaml2ics-0.2/PKG-INFO
```

### Comparing `yaml2ics-0.1rc3/.github/workflows/lint.yml` & `yaml2ics-0.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `yaml2ics-0.1rc3/.github/workflows/test.yml` & `yaml2ics-0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `yaml2ics-0.1rc3/.pre-commit-config.yaml` & `yaml2ics-0.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # Install pre-commit hooks via
 # pre-commit install
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
       - id: check-ast
       - id: mixed-line-ending
       - id: check-yaml
         args: [--allow-multiple-documents]
       - id: check-json
       - id: check-toml
       - id: check-added-large-files
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/adamchainz/blacken-docs
+    rev: 1.13.0
     hooks:
-      - id: flake8
-        pass_filenames: true
+      - id: blacken-docs
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    # Ruff version.
+    rev: "v0.0.261"
     hooks:
-      - id: isort
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.37.3
-    hooks:
-      - id: pyupgrade
-        args: [--py38-plus]
+      - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.7.1
     hooks:
       - id: prettier
-        files: \.(html|md|yml|yaml)
+        files: \.(html|md|yml|yaml|toml)
         args: [--prose-wrap=preserve]
```

### Comparing `yaml2ics-0.1rc3/CHANGELOG.md` & `yaml2ics-0.2/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,44 @@
 # Changelog
 
-## [Unreleased](https://github.com/scientific-python/yaml2ics/tree/v0.1rc3) (2022-08-20)
+## [v0.2](https://github.com/scientific-python/yaml2ics/tree/v0.2)
+
+[Full Changelog](https://github.com/scientific-python/yaml2ics/compare/v0.1...v0.2)
+
+**Merged pull requests:**
+
+- Update pre-commit hooks [\#53](https://github.com/scientific-python/yaml2ics/pull/53) ([jarrodmillman](https://github.com/jarrodmillman))
+- Update codecov [\#52](https://github.com/scientific-python/yaml2ics/pull/52) ([jarrodmillman](https://github.com/jarrodmillman))
+- Update pre-commit [\#50](https://github.com/scientific-python/yaml2ics/pull/50) ([jarrodmillman](https://github.com/jarrodmillman))
+- Increase coverage to 100% [\#48](https://github.com/scientific-python/yaml2ics/pull/48) ([stefanv](https://github.com/stefanv))
+- Switch from flake8 to ruff [\#47](https://github.com/scientific-python/yaml2ics/pull/47) ([stefanv](https://github.com/stefanv))
+- Flake8 migrated to GitHub [\#46](https://github.com/scientific-python/yaml2ics/pull/46) ([itrich](https://github.com/itrich))
+- Add possibility to add additional dates to recurring events [\#45](https://github.com/scientific-python/yaml2ics/pull/45) ([itrich](https://github.com/itrich))
+
+## [v0.1](https://github.com/scientific-python/yaml2ics/tree/v0.1)
+
+[Full Changelog](https://github.com/scientific-python/yaml2ics/compare/v0.1rc3...v0.1)
+
+**Closed issues:**
+
+- Release please [\#42](https://github.com/scientific-python/yaml2ics/issues/42)
+
+**Merged pull requests:**
+
+- Announce Python 3.11 support [\#43](https://github.com/scientific-python/yaml2ics/pull/43) ([jarrodmillman](https://github.com/jarrodmillman))
+- Add ability to specify custom ICS [\#41](https://github.com/scientific-python/yaml2ics/pull/41) ([stefanv](https://github.com/stefanv))
+- Fix markdown syntax [\#40](https://github.com/scientific-python/yaml2ics/pull/40) ([jarrodmillman](https://github.com/jarrodmillman))
+- Add test and coverage badges [\#39](https://github.com/scientific-python/yaml2ics/pull/39) ([jarrodmillman](https://github.com/jarrodmillman))
+- Update install and release notes [\#38](https://github.com/scientific-python/yaml2ics/pull/38) ([jarrodmillman](https://github.com/jarrodmillman))
+- Measure test coverage [\#37](https://github.com/scientific-python/yaml2ics/pull/37) ([jarrodmillman](https://github.com/jarrodmillman))
+- Add classifiers [\#36](https://github.com/scientific-python/yaml2ics/pull/36) ([jarrodmillman](https://github.com/jarrodmillman))
+- Lint toml [\#35](https://github.com/scientific-python/yaml2ics/pull/35) ([jarrodmillman](https://github.com/jarrodmillman))
+- Fix linting [\#34](https://github.com/scientific-python/yaml2ics/pull/34) ([jarrodmillman](https://github.com/jarrodmillman))
+
+## [v0.1rc3](https://github.com/scientific-python/yaml2ics/tree/v0.1rc3) (2022-08-21)
 
 [Full Changelog](https://github.com/scientific-python/yaml2ics/compare/v0.1rc2...v0.1rc3)
 
 **Merged pull requests:**
 
 - Use ics pypi pre-release [\#33](https://github.com/scientific-python/yaml2ics/pull/33) ([jarrodmillman](https://github.com/jarrodmillman))
 
@@ -57,14 +91,8 @@
 - Add per-calendar default timezone \(in meta header\) [\#8](https://github.com/scientific-python/yaml2ics/pull/8) ([rkdarst](https://github.com/rkdarst))
 - Don't set end=None for recurring events [\#7](https://github.com/scientific-python/yaml2ics/pull/7) ([rkdarst](https://github.com/rkdarst))
 - Fix rrule creation: use name= and value= for more correct syntax. [\#6](https://github.com/scientific-python/yaml2ics/pull/6) ([rkdarst](https://github.com/rkdarst))
 - Print error messages to stderr, not stdout [\#5](https://github.com/scientific-python/yaml2ics/pull/5) ([rkdarst](https://github.com/rkdarst))
 - Port yaml2ics to ics 0.8.0 [\#4](https://github.com/scientific-python/yaml2ics/pull/4) ([rkdarst](https://github.com/rkdarst))
 - requirements: Add PyYAML [\#2](https://github.com/scientific-python/yaml2ics/pull/2) ([rkdarst](https://github.com/rkdarst))
 
-## [v0.0](https://github.com/scientific-python/yaml2ics/tree/v0.0) (2021-09-21)
-
-[Full Changelog](https://github.com/scientific-python/yaml2ics/compare/930ab55f6f3abe6729afd929cb3d37299581f183...v0.0)
-
-
-
-\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
+\* _This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)_
```

### Comparing `yaml2ics-0.1rc3/LICENSE` & `yaml2ics-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml2ics-0.1rc3/README.md` & `yaml2ics-0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-![PyPI](https://img.shields.io/pypi/v/yaml2ics?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/yaml2ics)](https://pypi.org/project/yaml2ics/)
+[![Test status](https://github.com/scientific-python/yaml2ics/workflows/test/badge.svg?branch=main)](https://github.com/scientific-python/yaml2ics/actions?query=workflow%3A%22test%22)
+[![Test coverage](https://codecov.io/gh/scientific-python/yaml2ics/branch/main/graph/badge.svg)](https://app.codecov.io/gh/scientific-python/yaml2ics/branch/main)
 
 # YAML to iCalendar (ics)
 
 | WARNING: this project is still in beta. Beware of breaking changes! |
 | ------------------------------------------------------------------- |
 
 Convert YAML files to .ics files which can be imported into other
@@ -20,21 +22,14 @@
 
 ## Installation
 
 ```
 pip install yaml2ics
 ```
 
-**Note:** due to a pending release of a dependency (`ics-py`), an additional
-step is required:
-
-```
-pip install -r requirements.txt
-```
-
 ## Usage
 
 To produce a calendar from a list of events:
 
 ```
 python yaml2ics.py example/test_calendar.yaml
 ```
@@ -79,13 +74,16 @@
 
 To test:
 
 ```
 pytest
 ```
 
+Generate a coverage report with:
+
+```
+pytest --cov-report term-missing --cov yaml2ics
+```
+
 [black](https://github.com/psf/black) and other linters are used to auto-format
 files (and enforced by CI). To install the git hooks, use `pre-commit install`.
 To run the tests/auto-formatting manually, use `pre-commit run --all-files`.
-
-Releases are automatically pushed on PyPi by the CI when pushing a tag
-following `*.*`.
```

### Comparing `yaml2ics-0.1rc3/RELEASE.md` & `yaml2ics-0.2/RELEASE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Release process for `yaml2ics`
 
 ## Introduction
 
 Example `version`
 
-- 1.8.dev0 \# development version of 1.8 (release candidate 1)
-- 1.8rc1 \# 1.8 release candidate 1
-- 1.8rc2.dev0 \# development version of 1.8 (release candidate 2)
-- 1.8 \# 1.8 release
-- 1.9.dev0 \# development version of 1.9 (release candidate 1)
+- 1.8.dev0 # development version of 1.8 (release candidate 1)
+- 1.8rc1 # 1.8 release candidate 1
+- 1.8rc2.dev0 # development version of 1.8 release candidate 2
+- 1.8 # 1.8 release
+- 1.9.dev0 # development version of 1.9 (release candidate 1)
 
 ## Process
 
 - Update and review `CHANGELOG.md`:
 
       gem install github_changelog_generator
       github_changelog_generator -u scientific-python -p yaml2ics --since-tag=<last tag>
@@ -20,15 +20,15 @@
 - Update `version` in `pyproject.toml`.
 
 - Commit changes:
 
       git add pyproject.toml CHANGELOG.md
       git commit -m 'Designate <version> release'
 
-- Add the version number (e.g., [v1.2.0]{.title-ref}) as a tag in git:
+- Add the version number (e.g., `1.2.0`) as a tag in git:
 
       git tag -s [-u <key-id>] v<version> -m 'signed <version> tag'
 
   If you do not have a gpg key, use -u instead; it is important for
   Debian packaging that the tags are annotated
 
 - Push the new meta-data to github:
```

### Comparing `yaml2ics-0.1rc3/example/test_calendar.yaml` & `yaml2ics-0.2/example/test_calendar.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -29,28 +29,36 @@
     duration: { minutes: 60 }
     repeat:
       interval:
         # seconds, minutes, hours, days, weeks, months, years
         weeks: 1
       until: 2022-12-31 # required
 
-  - summary: Recurring event with exception
+  - summary: Recurring event with exception and additional date
     begin: 2022-07-01 10:00:00
     duration: { minutes: 60 }
     repeat:
       interval:
         # seconds, minutes, hours, days, weeks, months, years
         hours: 4
       until: 2022-07-31 # required
       except_on:
         - 2022-07-13
         - 2022-07-14 06:00:00
+      also_on:
+        - 2022-12-24 06:00:00
 
   # All-day event
   - summary: Earth Day
     begin: 2021-04-22
     url: https://earthday.org
     repeat:
       interval:
         # seconds, minutes, hours, days, weeks, months, years
         years: 1
       until: 2030-04-22
+
+  # Event with custom RRULE
+  - summary: Another day
+    begin: 2021-04-22
+    ics: |
+      RRULE:FREQ=YEARLY;UNTIL=20280422T000000
```

### Comparing `yaml2ics-0.1rc3/PKG-INFO` & `yaml2ics-0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 Metadata-Version: 2.1
 Name: yaml2ics
-Version: 0.1rc3
+Version: 0.2
 Summary: yaml2ics
 Author: Scientific Python Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ics == 0.8.0.dev0
 Requires-Dist: python-dateutil >= 2.8
 Requires-Dist: pyyaml >= 6
-Requires-Dist: pre-commit >= 2.20 ; extra == "lint"
-Requires-Dist: pytest >= 7 ; extra == "test"
+Requires-Dist: pre-commit >= 3.0 ; extra == "lint"
+Requires-Dist: pytest >= 7.3 ; extra == "test"
+Requires-Dist: pytest-cov >= 4.0 ; extra == "test"
 Project-URL: Home, https://github.com/scientific-python/yaml2ics
 Project-URL: Source, https://github.com/scientific-python/yaml2ics
 Provides-Extra: lint
 Provides-Extra: test
 
-![PyPI](https://img.shields.io/pypi/v/yaml2ics?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/yaml2ics)](https://pypi.org/project/yaml2ics/)
+[![Test status](https://github.com/scientific-python/yaml2ics/workflows/test/badge.svg?branch=main)](https://github.com/scientific-python/yaml2ics/actions?query=workflow%3A%22test%22)
+[![Test coverage](https://codecov.io/gh/scientific-python/yaml2ics/branch/main/graph/badge.svg)](https://app.codecov.io/gh/scientific-python/yaml2ics/branch/main)
 
 # YAML to iCalendar (ics)
 
 | WARNING: this project is still in beta. Beware of breaking changes! |
 | ------------------------------------------------------------------- |
 
 Convert YAML files to .ics files which can be imported into other
@@ -38,21 +47,14 @@
 
 ## Installation
 
 ```
 pip install yaml2ics
 ```
 
-**Note:** due to a pending release of a dependency (`ics-py`), an additional
-step is required:
-
-```
-pip install -r requirements.txt
-```
-
 ## Usage
 
 To produce a calendar from a list of events:
 
 ```
 python yaml2ics.py example/test_calendar.yaml
 ```
@@ -97,14 +99,17 @@
 
 To test:
 
 ```
 pytest
 ```
 
+Generate a coverage report with:
+
+```
+pytest --cov-report term-missing --cov yaml2ics
+```
+
 [black](https://github.com/psf/black) and other linters are used to auto-format
 files (and enforced by CI). To install the git hooks, use `pre-commit install`.
 To run the tests/auto-formatting manually, use `pre-commit run --all-files`.
 
-Releases are automatically pushed on PyPi by the CI when pushing a tag
-following `*.*`.
-
```

