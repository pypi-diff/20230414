# Comparing `tmp/shillelagh-1.2.0.tar.gz` & `tmp/shillelagh-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.0.tar", last modified: Fri Feb 17 21:09:08 2023, max compression
+gzip compressed data, was "shillelagh-1.2.1.tar", last modified: Fri Apr 14 21:13:18 2023, max compression
```

## Comparing `shillelagh-1.2.0.tar` & `shillelagh-1.2.1.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.165957 shillelagh-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.149957 shillelagh-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.149957 shillelagh-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.149957 shillelagh-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-17 21:08:47.000000 shillelagh-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-02-17 21:08:47.000000 shillelagh-1.2.0/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-17 21:08:47.000000 shillelagh-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-02-17 21:08:47.000000 shillelagh-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-17 21:08:47.000000 shillelagh-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-02-17 21:08:47.000000 shillelagh-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-17 21:08:47.000000 shillelagh-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-17 21:08:47.000000 shillelagh-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-02-17 21:09:08.165957 shillelagh-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-02-17 21:08:47.000000 shillelagh-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.149957 shillelagh-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.149957 shillelagh-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    31877 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-02-17 21:08:47.000000 shillelagh-1.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-17 21:08:47.000000 shillelagh-1.2.0/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 21:08:47.000000 shillelagh-1.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-17 21:08:47.000000 shillelagh-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-17 21:08:47.000000 shillelagh-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-17 21:08:47.000000 shillelagh-1.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-17 21:08:47.000000 shillelagh-1.2.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-02-17 21:08:47.000000 shillelagh-1.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-17 21:09:08.165957 shillelagh-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-17 21:08:47.000000 shillelagh-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.141957 shillelagh-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-17 21:08:47.000000 shillelagh-1.2.0/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.153957 shillelagh-1.2.0/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-02-17 21:09:08.000000 shillelagh-1.2.0/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-17 21:09:06.000000 shillelagh-1.2.0/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-02-17 21:08:47.000000 shillelagh-1.2.0/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.141957 shillelagh-1.2.0/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-17 21:08:47.000000 shillelagh-1.2.0/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-02-17 21:08:47.000000 shillelagh-1.2.0/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 21:08:47.000000 shillelagh-1.2.0/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-02-17 21:08:47.000000 shillelagh-1.2.0/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.157957 shillelagh-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.161957 shillelagh-1.2.0/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 21:09:08.165957 shillelagh-1.2.0/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-17 21:08:47.000000 shillelagh-1.2.0/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.824736 shillelagh-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-04-14 21:13:06.000000 shillelagh-1.2.1/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 21:13:06.000000 shillelagh-1.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:13:06.000000 shillelagh-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 21:13:06.000000 shillelagh-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-14 21:13:18.824736 shillelagh-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-14 21:13:06.000000 shillelagh-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.804736 shillelagh-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.804736 shillelagh-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.808736 shillelagh-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 21:13:06.000000 shillelagh-1.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 21:13:06.000000 shillelagh-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.808736 shillelagh-1.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-14 21:13:18.824736 shillelagh-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 21:13:06.000000 shillelagh-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.788735 shillelagh-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-04-14 21:13:06.000000 shillelagh-1.2.1/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.792735 shillelagh-1.2.1/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.824736 shillelagh-1.2.1/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/types_test.py
```

### Comparing `shillelagh-1.2.0/.coveragerc` & `shillelagh-1.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/pull_request_template.md` & `shillelagh-1.2.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/workflows/python-integration.yml` & `shillelagh-1.2.1/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.1/.github/workflows/python-package.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Run tests with latest dependencies
+name: Run tests with pinned dependencies
 
 on:
-  schedule:
-    - cron:  '0 6 * * *'
-  workflow_dispatch:
+  push:
+    branches: [ main ]
+  pull_request:
+    branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
@@ -25,14 +26,12 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       env:
         VERSION: 3.38.1
         RELEASE: r1
       run: |
         python -m pip install --upgrade pip setuptools
-        pip install -e '.[testing]'
-        pip install https://github.com/rogerbinns/apsw/releases/download/${VERSION}-${RELEASE}/apsw-${VERSION}-${RELEASE}.zip \
-          --global-option=fetch --global-option=--version --global-option=${VERSION} --global-option=--all \
-          --global-option=build --global-option=--enable-all-extensions
+        pip install -r requirements/test.txt
     - name: Test with pytest
       run: |
+        pre-commit run --all-files
         pytest --cov-fail-under=100 --cov=src/shillelagh -vv tests/ --doctest-modules src/shillelagh --without-integration --without-slow-integration
```

### Comparing `shillelagh-1.2.0/.github/workflows/python-package.yml` & `shillelagh-1.2.1/.github/workflows/python-package-daily.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Run tests with pinned dependencies
+name: Run tests with latest dependencies
 
 on:
-  push:
-    branches: [ main ]
-  pull_request:
-    branches: [ main ]
+  schedule:
+    - cron:  '0 6 * * *'
+  workflow_dispatch:
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       env:
         VERSION: 3.38.1
         RELEASE: r1
       run: |
         python -m pip install --upgrade pip setuptools
-        pip install -r requirements/test.txt
-        pip install https://github.com/rogerbinns/apsw/releases/download/${VERSION}-${RELEASE}/apsw-${VERSION}-${RELEASE}.zip \
-          --global-option=fetch --global-option=--version --global-option=${VERSION} --global-option=--all \
-          --global-option=build --global-option=--enable-all-extensions
+        pip install -e '.[testing]'
     - name: Test with pytest
       run: |
-        pre-commit run --all-files
         pytest --cov-fail-under=100 --cov=src/shillelagh -vv tests/ --doctest-modules src/shillelagh --without-integration --without-slow-integration
```

### Comparing `shillelagh-1.2.0/.github/workflows/python-publish.yml` & `shillelagh-1.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.gitignore` & `shillelagh-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.pre-commit-config.yaml` & `shillelagh-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/.readthedocs.yml` & `shillelagh-1.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/ARCHITECTURE.rst` & `shillelagh-1.2.1/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/CHANGELOG.rst` & `shillelagh-1.2.1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.1 - 2023-04-14
+==========================
+
+- Allow specifying custom request headers when using the generic JSON adapter (#337)
+- Fix for escaping identifiers correctly (#340)
+- Support for S3-compatible storage (#343)
+- Adapters can now know which columns were requested (#345)
+- Python 3.11 officially supported (#334)
+- Fix for error when an adapater can't be loaded (#346)
+- Fix for ``BestIndexObject`` (#350)
+- Fix for empty dataframes (#351)
+
 Version 1.2.0 - 2023-02-17
 ==========================
 
 - Use ``marshal`` instead of ``pickle`` for adapter argument serde (#321)
 - Support SQLAlchemy 2.0 (and 1.4) (#331)
 - ``s3_select`` can now use credentials from the environment or config files
```

### Comparing `shillelagh-1.2.0/CODE_OF_CONDUCT.md` & `shillelagh-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/CONTRIBUTING.rst` & `shillelagh-1.2.1/CONTRIBUTING.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ============
 
 Thanks for wanting to contribute to the project! Here's a quick rundown of how to get it running for development.
 
 Install ``pyenv``
 =================
 
-You don't *need* ``pyenv``, but development will be easier with it. Follow `these instructions <https://github.com/pyenv/pyenv#installation>`_ to install it, and then create a virtual environment. Shillelagh is tested with Python 3.8-3.10, so make sure to install one of those versions.
+You don't *need* ``pyenv``, but development will be easier with it. Follow `these instructions <https://github.com/pyenv/pyenv#installation>`_ to install it, and then create a virtual environment. Shillelagh is tested with Python 3.8-3.11, so make sure to install one of those versions.
 
 .. code-block:: bash
 
     $ pyenv install 3.10.3
     $ pyenv virtualenv 3.10.3 shillelagh
     $ cd /path/to/shillelagh/
     $ pyenv local shillelagh
@@ -21,27 +21,14 @@
 
 You want to install the package in developer mode (``-e``) with all the dependencies needed for testing:
 
 .. code-block:: bash
 
     $ pip install -e ".[testing]"
 
-Install the latest ``apsw``
-===========================
-
-``apsw`` (another Python SQLite wrapper) is the Python library that gives Shillelagh its superpowers. The last command will install a version of ``apsw`` that is not official, since the package is not officially published to PyPI. You should compile and install the latest version from source code by running:
-
-.. code-block:: bash
-
-    $ export VERSION=3.38.1
-    $ export RELEASE=r1
-    $ pip install https://github.com/rogerbinns/apsw/releases/download/${VERSION}-${RELEASE}/apsw-${VERSION}-${RELEASE}.zip \
-    > --global-option=fetch --global-option=--version --global-option=${VERSION} --global-option=--all \
-    > --global-option=build --global-option=--enable-all-extensions
-
 Install pre-commit hooks
 ========================
 
 Shillelagh uses a lot of pre-commit hooks.
 
 .. code-block:: bash
```

### Comparing `shillelagh-1.2.0/LICENSE.txt` & `shillelagh-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/Makefile` & `shillelagh-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/PKG-INFO` & `shillelagh-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.0
+Version: 1.2.1
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
@@ -161,14 +161,15 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: console
```

### Comparing `shillelagh-1.2.0/README.rst` & `shillelagh-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/docs/Makefile` & `shillelagh-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/docs/adapters.rst` & `shillelagh-1.2.1/docs/adapters.rst`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 .. code-block:: python
 
     from shillelagh.backends.apsw.db import connect
 
     connection = connect(
         ":memory:",
         adapter_kwargs={
-            "gsheetaspi": {
+            "gsheetsapi": {
                 # "service_account_file": "/path/to/credentials.json",
                 "service_account_info": {
                     "type": "service_account",
                     ...
                 },
                 "subject": "user@example.com",
             },
@@ -411,7 +411,43 @@
           "popularity": 16,
           "notes": "BEA Account Code: A001RX\n\n"
         }
       ]
     }
 
 In the payload above the data is stored in the ``seriess`` key. In order to have Shillelagh access the data correctly you should pass a `JSONPath <https://goessner.net/articles/JsonPath/>`_ expression as an achor in the URL. For this payload the expression ``$.seriess[*]`` will return all rows inside the ``seriess`` children.
+
+If you need to authenticate you can pass custom request headers via adapter keyword arguments:
+
+.. code-block:: python
+
+    from shillelagh.backends.apsw.db import connect
+
+    connection = connect(
+        ":memory:",
+        adapter_kwargs={
+            "genericjsonapi": {
+                "request_headers": {
+                    "X-Auth-Token": "SECRET",
+                },
+            },
+        },
+    )
+
+Or via SQLAlchemy:
+
+.. code-block:: python
+
+    from sqlalchemy import create_engine
+
+    engine = create_engine(
+        "shilellagh://",
+        connect_args={
+            "adapter_kwargs": {
+                "genericjsonapi": {
+                    "request_headers": {
+                        "X-Auth-Token": "SECRET",
+                    },
+                },
+            },
+        },
+    )
```

### Comparing `shillelagh-1.2.0/docs/conf.py` & `shillelagh-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/docs/development.rst` & `shillelagh-1.2.1/docs/development.rst`

 * *Files 2% similar despite different names*

```diff
@@ -292,14 +292,37 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
 
 Now the adapter can handle ``limit`` and ``offset``, reducing the amount of data that is returned. Note that even if the adapter declares supporting ``LIMIT``, SQLite will still enforce the limit, ie, if for any reason the adapter returns more rows than the limit SQLite will fix the problem. The same is not true for the offset.
 
+Returning only the requested columns
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+By default adapters should return all the columns available, since they have no information on which columns are actually needed. Starting with apsw `apsw 3.41.0.0 <https://github.com/rogerbinns/apsw/releases/tag/3.41.0.0>`_ adapters can optionally receive only the requested columns in their ``get_rows`` and ``get_data`` methods. The adapter must declare support for it by setting the attribute ``supports_requested_columns`` to true:
+
+.. code-block:: python
+
+    class WeatherAPI(Adapter):
+
+        supports_requested_columns = True
+
+Then the ``requested_columns: Optional[Set[str]]`` argument will be passed to ``get_rows`` and ``get_data``:
+
+.. code-block:: python
+
+    def get_rows(
+        self,
+        bounds: Dict[str, Filter],
+        order: List[Tuple[str, RequestedOrder]],
+        requested_columns: Optional[Set[str]] = None,
+        **kwargs: Any,
+    ) -> Iterator[Dict[str, Any]]:
+
 A read-write adapter
 ====================
 
 For a read-write adapter we need to implement at least 2 additional methods:
 
 - ``insert_row(self, row: Dict[str, Any]) -> int``
 - ``delete_row(self, row_id: int) -> None``
@@ -486,15 +509,15 @@
                 100
                 + 1000 * len(filtered_columns)
                 + 10000 * len(order)
             )
 
 In the example above, we have an initial cost of 100. Each filtering operation costs an additional 1000 units, and each sorting costs 10000. This is a simple representation of filtering 1000 points in O(n), and sorting them in O(n log n) (note that the numbers are unitless). These numbers can be improved if you know the size of the data.
 
-If you want to use the model above you can do this in your adapter
+If you want to use the model above you can do this in your adapter:
 
 .. code-block:: python
 
     from shillelagh.lib import SimpleCostModel
 
     class MyAdapter:
```

### Comparing `shillelagh-1.2.0/docs/install.rst` & `shillelagh-1.2.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/docs/usage.rst` & `shillelagh-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/examples/csvfile.py` & `shillelagh-1.2.1/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/examples/dataframe.py` & `shillelagh-1.2.1/examples/dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,7 +21,12 @@
     SQL = "SELECT SUM(a) FROM mydf"
     for row in cursor.execute(SQL):
         print(row)
 
     SQL = "SELECT * FROM mydf LIMIT 2 OFFSET 1"
     for row in cursor.execute(SQL):
         print(row)
+
+    emptydf = pd.DataFrame({"a": []})
+    SQL = "SELECT * from emptydf WHERE a = 'test'"
+    for row in cursor.execute(SQL):
+        print(row)
```

### Comparing `shillelagh-1.2.0/examples/datasette.py` & `shillelagh-1.2.1/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/examples/generic_json.py` & `shillelagh-1.2.1/examples/generic_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,13 +45,15 @@
 from shillelagh.backends.apsw.db import connect
 
 if __name__ == "__main__":
     connection = connect(":memory:")
     cursor = connection.cursor()
 
     SQL = """
-    SELECT * FROM
+    SELECT domain, isDead FROM
     "https://api.domainsdb.info/v1/domains/search?domain=facebook&zone=com#$.domains[*]"
+    WHERE isDead > 2
+    ORDER BY domain DESC
     LIMIT 2
     """
     for row in cursor.execute(SQL):
         print(row)
```

### Comparing `shillelagh-1.2.0/examples/weatherapi.py` & `shillelagh-1.2.1/examples/weatherapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from shillelagh.backends.apsw.db import connect
 
 if __name__ == "__main__":
     three_days_ago = datetime.now() - timedelta(days=3)
 
     # sign up for an API key at https://www.weatherapi.com/my/
-    api_key = sys.argv[1]
+    api_key = sys.argv[1]  # pylint: disable=invalid-name
 
     connection = connect(":memory:")
     cursor = connection.cursor()
 
     SQL = f"""
     SELECT *
     FROM "https://api.weatherapi.com/v1/history.json?key={api_key}&q=94923" AS bodega_bay
```

### Comparing `shillelagh-1.2.0/requirements/base.txt` & `shillelagh-1.2.1/requirements/base.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,22 @@
     # via -r requirements/base.in
 apsw==3.38.5.post1
     # via shillelagh
 certifi==2022.6.15
     # via requests
 charset-normalizer==2.1.0
     # via requests
-greenlet==1.1.2
-    # via sqlalchemy
+greenlet==2.0.2
+    # via
+    #   shillelagh
+    #   sqlalchemy
 idna==3.3
     # via requests
+packaging==23.0
+    # via shillelagh
 python-dateutil==2.8.2
     # via shillelagh
 requests==2.28.1
     # via shillelagh
 six==1.16.0
     # via python-dateutil
 sqlalchemy==1.4.39
```

### Comparing `shillelagh-1.2.0/requirements/test.txt` & `shillelagh-1.2.1/requirements/test.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 -e file:.
     # via -r requirements/test.in
 appdirs==1.4.4
     # via shillelagh
 apsw==3.38.5.post1
     # via shillelagh
-astroid==2.11.7
+astroid==2.14.2
     # via pylint
 attrs==21.4.0
     # via
     #   pytest
     #   requests-cache
 beautifulsoup4==4.11.1
     # via shillelagh
@@ -37,28 +37,32 @@
     # via requests
 click==8.1.3
     # via pip-tools
 codespell==2.1.0
     # via shillelagh
 coverage[toml]==6.4.2
     # via pytest-cov
-dill==0.3.5.1
-    # via pylint
+dill==0.3.6
+    # via
+    #   pylint
+    #   shillelagh
 distlib==0.3.5
     # via virtualenv
 exceptiongroup==1.0.4
     # via pytest
 filelock==3.7.1
     # via virtualenv
 freezegun==1.2.1
     # via shillelagh
 google-auth==2.9.1
     # via shillelagh
-greenlet==1.1.2
-    # via sqlalchemy
+greenlet==2.0.2
+    # via
+    #   shillelagh
+    #   sqlalchemy
 html5lib==1.1
     # via shillelagh
 identify==2.5.2
     # via pre-commit
 idna==3.3
     # via
     #   requests
@@ -85,14 +89,15 @@
     # via pre-commit
 numpy==1.23.1
     # via pandas
 packaging==21.3
     # via
     #   build
     #   pytest
+    #   shillelagh
 pandas==1.4.3
     # via shillelagh
 pep517==0.12.0
     # via build
 pip-tools==6.8.0
     # via shillelagh
 platformdirs==2.5.2
@@ -113,15 +118,15 @@
     #   rsa
 pyasn1-modules==0.2.8
     # via google-auth
 pyfakefs==4.6.3
     # via shillelagh
 pygments==2.12.0
     # via shillelagh
-pylint==2.14.5
+pylint==2.16.2
     # via shillelagh
 pyparsing==3.0.9
     # via packaging
 pytest==7.2.0
     # via
     #   pytest-cov
     #   pytest-mock
```

### Comparing `shillelagh-1.2.0/setup.cfg` & `shillelagh-1.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: SQL
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
@@ -28,15 +29,17 @@
 setup_requires = pyscaffold>=3.2a0
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	apsw>=3.9.2
 	python_dateutil>=2.8.1
 	requests>=2.25.1
 	sqlalchemy>=1.3
+	greenlet>=2.0.2  # needed for Python 3.11 w/o memory leak
 	typing_extensions>=3.7.4.3
+	packaging
 python_requires = >=3.8
 obsoletes = 
 	gsheetsdb
 
 [options.packages.find]
 where = src
 exclude = 
@@ -45,26 +48,27 @@
 [options.extras_require]
 testing = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	beautifulsoup4>=4.11.1
 	boto3>=1.24.28
 	codespell>=2.1.0
+	dill>=0.3.6
 	freezegun>=1.1.0
 	google-auth>=1.23.0
 	html5lib>=1.1
 	jsonpath-python>=1.0.5
 	pandas>=1.2.2
 	pip-tools>=6.4.0
 	pre-commit>=2.13.0
 	prompt_toolkit>=3
 	psutil>=5.8.0
 	pyfakefs>=4.3.3
 	pygments>=2.8
-	pylint>=2.11.1
+	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=7.2.0
 	requests-cache==0.7.1
 	requests-mock>=1.8.0
 	requests>=2.25.1
@@ -83,15 +87,15 @@
 	pandas>=1.2.2
 	pip-tools>=6.4.0
 	pre-commit>=2.13.0
 	prompt_toolkit>=3
 	psutil>=5.8.0
 	pyfakefs>=4.3.3
 	pygments>=2.8
-	pylint>=2.11.1
+	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=6.2.2
 	requests-cache==0.7.1
 	requests-mock>=1.8.0
 	requests>=2.25.1
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/html_table.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,83 @@
 """
-An adapter for fetching JSON data.
+An adapter that scrapes HTML tables.
 """
 
 # pylint: disable=invalid-name
 
-import logging
 import urllib.parse
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
-import requests_cache
-from jsonpath import JSONPath
+import pandas as pd
 
 from shillelagh.adapters.base import Adapter
-from shillelagh.exceptions import ProgrammingError
+from shillelagh.adapters.memory.pandas import get_columns_from_df, get_df_data
 from shillelagh.fields import Field
 from shillelagh.filters import Filter
-from shillelagh.lib import SimpleCostModel, analyze, flatten
-from shillelagh.typing import Maybe, RequestedOrder, Row
+from shillelagh.lib import SimpleCostModel
+from shillelagh.typing import RequestedOrder, Row
 
-_logger = logging.getLogger(__name__)
-
-SUPPORTED_PROTOCOLS = {"http", "https"}
+SUPPORTED_PROTOCOLS = {"http", "https", "ftp", "file"}
 AVERAGE_NUMBER_OF_ROWS = 100
 
 
-def get_session() -> requests_cache.CachedSession:
-    """
-    Return a cached session.
-    """
-    return requests_cache.CachedSession(
-        cache_name="generic_json_cache",
-        backend="sqlite",
-        expire_after=180,
-    )
-
-
-class GenericJSONAPI(Adapter):
+class HTMLTableAPI(Adapter):
 
     """
-    An adapter for fetching JSON data.
+    An adapter for scraping HTML tables.
     """
 
     safe = True
 
-    supports_limit = False
-    supports_offset = False
+    supports_limit = True
+    supports_offset = True
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         parsed = urllib.parse.urlparse(uri)
         if parsed.scheme not in SUPPORTED_PROTOCOLS:
             return False
         if fast:
-            return Maybe
+            return None
 
-        session = get_session()
-        response = session.head(uri)
-        return "application/json" in response.headers.get("content-type", "")
+        # table index can be specified as an anchor; remove
+        uri = urllib.parse.urlunparse(parsed._replace(fragment=""))
+        try:
+            dataframes = pd.read_html(uri, flavor="bs4")
+        except Exception:  # pylint: disable=broad-except
+            return False
+
+        return len(dataframes) > 0
 
     @staticmethod
-    def parse_uri(uri: str) -> Tuple[str, str]:
+    def parse_uri(uri: str) -> Tuple[str, int]:
         parsed = urllib.parse.urlparse(uri)
 
-        path = urllib.parse.unquote(parsed.fragment) or "$[*]"
+        # extract table index from anchor and remove from URI
+        try:
+            index = int(parsed.fragment or "0")
+        except ValueError:
+            index = 0
         uri = urllib.parse.urlunparse(parsed._replace(fragment=""))
 
-        return uri, path
+        return uri, index
 
-    def __init__(self, uri: str, path: str = "$[*]"):
+    def __init__(self, uri: str, index: int = 0):
         super().__init__()
 
-        self.uri = uri
-        self.path = path
-
-        self._session = get_session()
-
-        self._set_columns()
-
-    def _set_columns(self) -> None:
-        rows = list(self.get_data({}, []))
-        column_names = list(rows[0].keys()) if rows else []
-
-        _, order, types = analyze(iter(rows))
-
-        self.columns = {
-            column_name: types[column_name](
-                filters=[],
-                order=order[column_name],
-                exact=False,
-            )
-            for column_name in column_names
-            if column_name != "rowid"
-        }
+        self.df = pd.read_html(uri, flavor="bs4")[index]
+        self.columns = get_columns_from_df(self.df)
 
     def get_columns(self) -> Dict[str, Field]:
         return self.columns
 
     get_cost = SimpleCostModel(AVERAGE_NUMBER_OF_ROWS)
 
-    def get_data(  # pylint: disable=unused-argument
+    def get_data(
         self,
         bounds: Dict[str, Filter],
         order: List[Tuple[str, RequestedOrder]],
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         **kwargs: Any,
     ) -> Iterator[Row]:
-        response = self._session.get(self.uri)
-        payload = response.json()
-        if not response.ok:
-            raise ProgrammingError(f'Error: {payload["message"]}')
-
-        parser = JSONPath(self.path)
-        for i, row in enumerate(parser.parse(payload)):
-            row["rowid"] = i
-            _logger.debug(row)
-            yield flatten(row)
+        yield from get_df_data(self.df, self.columns, bounds, order, limit, offset)
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     @classmethod
     def consume(cls, pattern: str) -> Tuple["Token", str]:
         """
         Consume the pattern, returning the token and the remaining pattern.
         """
         match = re.match(cls.regex, pattern)
         if not match:
+            # pylint: disable=broad-exception-raised
             raise Exception("Token could not find match")
         token = match.group()
         return cls(token), pattern[len(token) :]
 
     def format(self, value: Valid, tokens: List["Token"]) -> str:
         """
         Format the value using the pattern.
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# pylint: disable=invalid-name, fixme
 """
 Parse and format Google Sheet date/time patterns.
 
 https://developers.google.com/sheets/api/guides/formats?hl=en#date_and_time_format_patterns
 """
+
+# pylint: disable=invalid-name, fixme, broad-exception-raised
+
 import calendar
 import re
 from collections import defaultdict
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Parse and format Google Sheet number formats.
 
 https://developers.google.com/sheets/api/guides/formats#number_format_tokens
 """
-# pylint: disable=c-extension-no-member
+# pylint: disable=c-extension-no-member, broad-exception-raised
 import math
 import operator
 import re
 from itertools import zip_longest
 from typing import Any, Dict, Iterator, List, Tuple, Union, cast
 
 from shillelagh.adapters.api.gsheets.parsing.base import (
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/system.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,106 @@
 """
-An adapter that scrapes HTML tables.
-"""
-
-# pylint: disable=invalid-name
+An adapter for retrieving information on running processes and system utilization (CPU,
+memory, disks, network, sensors).
 
+See https://github.com/giampaolo/psutil for more information.
+"""
+import logging
+import time
 import urllib.parse
-from typing import Any, Dict, Iterator, List, Optional, Tuple
+from datetime import datetime, timezone
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
-import pandas as pd
+import psutil
 
 from shillelagh.adapters.base import Adapter
-from shillelagh.adapters.memory.pandas import get_columns_from_df, get_df_data
-from shillelagh.fields import Field
+from shillelagh.exceptions import ProgrammingError
+from shillelagh.fields import DateTime, Field, Float, Order
 from shillelagh.filters import Filter
-from shillelagh.lib import SimpleCostModel
 from shillelagh.typing import RequestedOrder, Row
 
-SUPPORTED_PROTOCOLS = {"http", "https", "ftp", "file"}
+_logger = logging.getLogger(__name__)
+
 AVERAGE_NUMBER_OF_ROWS = 100
 
 
-class HTMLTableAPI(Adapter):
+class SystemAPI(Adapter):
 
     """
-    An adapter for scraping HTML tables.
+    An adapter for retrieving system information.
     """
 
-    safe = True
+    safe = False
 
     supports_limit = True
     supports_offset = True
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         parsed = urllib.parse.urlparse(uri)
-        if parsed.scheme not in SUPPORTED_PROTOCOLS:
-            return False
-        if fast:
-            return None
-
-        # table index can be specified as an anchor; remove
-        uri = urllib.parse.urlunparse(parsed._replace(fragment=""))
-        try:
-            dataframes = pd.read_html(uri, flavor="bs4")
-        except Exception:  # pylint: disable=broad-except
-            return False
-
-        return len(dataframes) > 0
+        return parsed.scheme == "system"
 
     @staticmethod
-    def parse_uri(uri: str) -> Tuple[str, int]:
+    def parse_uri(uri: str) -> Union[Tuple[str], Tuple[str, float]]:
         parsed = urllib.parse.urlparse(uri)
+        resource = parsed.netloc
+        query_string = urllib.parse.parse_qs(parsed.query)
 
-        # extract table index from anchor and remove from URI
-        try:
-            index = int(parsed.fragment or "0")
-        except ValueError:
-            index = 0
-        uri = urllib.parse.urlunparse(parsed._replace(fragment=""))
+        if "interval" in query_string:
+            return (resource, float(query_string["interval"][0]))
+        return (resource,)
 
-        return uri, index
-
-    def __init__(self, uri: str, index: int = 0):
+    def __init__(self, resource: str, interval: float = 1.0):
         super().__init__()
 
-        self.df = pd.read_html(uri, flavor="bs4")[index]
-        self.columns = get_columns_from_df(self.df)
+        self.resource = resource
+        self.interval = interval
+
+        self._set_columns()
+
+    def _set_columns(self) -> None:
+        self.columns: Dict[str, Field] = {
+            "timestamp": DateTime(filters=None, order=Order.ASCENDING, exact=False),
+        }
+
+        if self.resource == "cpu":
+            num_cpus = psutil.cpu_count()
+            for i in range(num_cpus):
+                self.columns[f"cpu{i}"] = Float(
+                    filters=None,
+                    order=Order.NONE,
+                    exact=False,
+                )
+        else:
+            raise ProgrammingError(f"Unknown resource: {self.resource}")
 
     def get_columns(self) -> Dict[str, Field]:
         return self.columns
 
-    get_cost = SimpleCostModel(AVERAGE_NUMBER_OF_ROWS)
-
     def get_data(
         self,
         bounds: Dict[str, Filter],
         order: List[Tuple[str, RequestedOrder]],
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         **kwargs: Any,
     ) -> Iterator[Row]:
-        yield from get_df_data(self.df, self.columns, bounds, order, limit, offset)
+        rowid = 0
+        while limit is None or rowid < limit:
+            if offset is not None:
+                time.sleep(self.interval * offset)
+
+            try:
+                values = psutil.cpu_percent(interval=self.interval, percpu=True)
+            except KeyboardInterrupt:
+                return
+
+            row = {
+                "rowid": rowid,
+                "timestamp": datetime.now(timezone.utc),
+            }
+            for i, value in enumerate(values):
+                row[f"cpu{i}"] = value / 100.0
+
+            _logger.debug(row)
+            yield row
+            rowid += 1
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/s3select.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,15 @@
         self,
         bucket: str,
         key: str,
         input_serialization: InputSerializationType,
         path: str = "$",
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
+        s3_endpoint_url: Optional[str] = None,
         s3_kwargs: Optional[Dict[str, Any]] = None,
     ):
         super().__init__()
 
         self.bucket = bucket
         self.key = key
         self.input_serialization = input_serialization
@@ -251,23 +252,28 @@
 
         # if credentials were passed explicitly, use them
         if aws_access_key_id and aws_secret_access_key:
             self.s3_client = boto3.client(
                 "s3",
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
+                endpoint_url=s3_endpoint_url,
             )
         # if no credentials were passed, check if they're available
         elif boto3.session.Session().get_credentials():
-            self.s3_client = boto3.client("s3")
+            self.s3_client = boto3.client(
+                "s3",
+                endpoint_url=s3_endpoint_url,
+            )
         # if no credentials were found, use an anonymous client to access public buckets
         else:
             self.s3_client = boto3.client(
                 "s3",
                 config=Config(signature_version=UNSIGNED),
+                endpoint_url=s3_endpoint_url,
             )
         self.s3_kwargs = s3_kwargs or {}
 
         self._set_columns()
 
     def _set_columns(self) -> None:
         rows = list(self._run_query(f"SELECT * FROM {self.table_name} LIMIT 1"))
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.1/src/shillelagh/adapters/api/weatherapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     time_range = bounds.get("time", Range())
     time_epoch_range = bounds.get("time_epoch", Range())
 
     if isinstance(time_range, Impossible) or isinstance(time_epoch_range, Impossible):
         raise ImpossibleFilterError()
 
     if not isinstance(time_range, Range) or not isinstance(time_epoch_range, Range):
-        raise Exception("Invalid filter")
+        raise Exception("Invalid filter")  # pylint: disable=broad-exception-raised
 
     # convert time_epoch range to datetime so we can combine it
     # with the time range
     time_epoch_range.start = (
         datetime.fromtimestamp(time_epoch_range.start, tz=timezone.utc)
         if time_epoch_range.start is not None
         else None
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/base.py` & `shillelagh-1.2.1/src/shillelagh/adapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     safe = False
 
     # if true, a corresponding argument will be passed in the kwargs of
     # ``get_rows`` and ``get_data``
     supports_limit = False
     supports_offset = False
 
+    # if true, the requested columns will be passed to ``get_rows`` and ``get_data``
+    supports_requested_columns = False
+
     def __init__(self, *args: Any, **kwargs: Any):  # pylint: disable=unused-argument
         # ensure ``self.close`` gets called before GC
         atexit.register(self.close)
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         """
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.1/src/shillelagh/adapters/file/csvfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Remote files (HTTP/HTTPS) are also supported in read-only mode.
 """
 import csv
 import logging
 import os
 import tempfile
 import urllib.parse
+from datetime import timedelta
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Tuple, cast
 
 import requests
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ProgrammingError
@@ -36,14 +37,16 @@
 
 _logger = logging.getLogger(__name__)
 
 INITIAL_COST = 0
 FILTERING_COST = 1000
 SORTING_COST = 10000
 
+DEFAULT_TIMEOUT = timedelta(minutes=3)
+
 SUPPORTED_PROTOCOLS = {"http", "https"}
 
 
 class RowTracker:
     """An iterator that keeps track of the last yielded row."""
 
     def __init__(self, iterable: Iterator[Row]):
@@ -112,15 +115,15 @@
         if parsed.path.endswith(".csv"):
             return True
 
         # do a head request to get mimetype
         if fast:
             return Maybe
 
-        response = requests.head(uri)
+        response = requests.head(uri, timeout=DEFAULT_TIMEOUT.total_seconds())
         return "text/csv" in response.headers.get("content-type", "")
 
     @staticmethod
     def parse_uri(uri: str) -> Tuple[str]:
         return (uri,)
 
     def __init__(self, path_or_uri: str):
@@ -130,15 +133,18 @@
         if path.suffix == ".csv" and path.exists():
             self.local = True
         else:
             self.local = False
 
             # download CSV file
             with tempfile.NamedTemporaryFile(delete=False) as output:
-                response = requests.get(path_or_uri)
+                response = requests.get(
+                    path_or_uri,
+                    timeout=DEFAULT_TIMEOUT.total_seconds(),
+                )
                 output.write(response.content)
             path = Path(output.name)
 
         self.path = path
         self.modified = False
 
         _logger.info("Opening file CSV file %s to load metadata", self.path)
@@ -180,15 +186,15 @@
     def get_cost(
         self,
         filtered_columns: List[Tuple[str, Operator]],
         order: List[Tuple[str, RequestedOrder]],
     ) -> float:
         cost = INITIAL_COST
 
-        # filtering the data has constant cost, since ``filter_data`` builds a
+        # filtering the data has linear cost, since ``filter_data`` builds a
         # single filter function applied as the data is streamed
         if filtered_columns:
             cost += FILTERING_COST
 
         # sorting, on the other hand, is costy, requiring loading all the data
         # in memory and calling ``.sort()`` for each column that needs to be
         # ordered
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.1/src/shillelagh/adapters/memory/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,28 @@
         context_globals = dict(inspect.getmembers(level[0]))["f_globals"]
         if uri in context_globals and isinstance(context_globals[uri], pd.DataFrame):
             return context_globals[uri]
 
     return None
 
 
-def get_df_data(  # pylint: disable=too-many-arguments
+def get_df_data(  # pylint: disable=too-many-arguments, too-many-branches
     df: pd.DataFrame,
     columns: Dict[str, Field],
     bounds: Dict[str, Filter],
     order: List[Tuple[str, RequestedOrder]],
     limit: Optional[int] = None,
     offset: Optional[int] = None,
 ) -> Iterator[Row]:
     """
     Apply the ``get_data`` method on a Pandas dataframe.
     """
+    if df.empty:
+        return
+
     # ensure column names are strings
     df = df.rename(columns={k: str(k) for k in df.columns})
 
     column_names = list(columns.keys())
     df = df[column_names]
 
     for column_name, filter_ in bounds.items():
```

### Comparing `shillelagh-1.2.0/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.1/src/shillelagh/adapters/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import InterfaceError
 
 _logger = logging.getLogger(__name__)
 
 
+class UnsafeAdaptersError(InterfaceError):
+    """
+    Raised when multiple adapters have the same name.
+    """
+
+
 class AdapterLoader:
     """
     Adapter registry, allowing new adapters to be registered.
     """
 
     def __init__(self):
         self.loaders = defaultdict(list)
@@ -27,15 +33,15 @@
             self.loaders[entry_point.name].append(entry_point.load)
 
     def load(self, name: str, safe: bool = False) -> Type[Adapter]:
         """
         Load a given entry point by its name.
         """
         if safe and len(self.loaders[name]) > 1:
-            raise InterfaceError(f"Multiple adapters found with name {name}")
+            raise UnsafeAdaptersError(f"Multiple adapters found with name {name}")
 
         for load in self.loaders[name]:
             try:
                 return cast(Type[Adapter], load())
             except (ImportError, ModuleNotFoundError) as ex:
                 _logger.warning("Couldn't load adapter %s", name)
                 _logger.debug(ex)
@@ -84,19 +90,25 @@
         adapters: Optional[List[str]] = None,
     ) -> Dict[str, Type[Adapter]]:
         """
         Load all adapters, safe and unsafe.
 
         If no adapters are specified, return all.
         """
-        return {
-            name: self.load(name, safe=False)
-            for name in self.loaders
-            if adapters is None or name in adapters
-        }
+        loaded_adapters = {}
+        for name in self.loaders:
+            if adapters is None:
+                try:
+                    loaded_adapters[name] = self.load(name, safe=False)
+                except InterfaceError:
+                    pass
+            elif name in adapters:
+                loaded_adapters[name] = self.load(name, safe=False)
+
+        return loaded_adapters
 
     def register(self, name: str, modulepath: str, classname: str) -> None:
         """
         Register a new adapter.
         """
 
         def load() -> Type[Adapter]:
```

### Comparing `shillelagh-1.2.0/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.1/src/shillelagh/backends/apsw/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import apsw
+from packaging.version import Version
 
 from shillelagh import functions
 from shillelagh.adapters.base import Adapter
 from shillelagh.adapters.registry import registry
 from shillelagh.backends.apsw.vt import VTModule, type_map
 from shillelagh.exceptions import (  # nopycln: import; pylint: disable=redefined-builtin
     DatabaseError,
@@ -35,15 +36,20 @@
     InternalError,
     NotSupportedError,
     OperationalError,
     ProgrammingError,
     Warning,
 )
 from shillelagh.fields import Blob, Field
-from shillelagh.lib import combine_args_kwargs, escape, find_adapter, serialize
+from shillelagh.lib import (
+    combine_args_kwargs,
+    escape_identifier,
+    find_adapter,
+    serialize,
+)
 from shillelagh.types import (
     BINARY,
     DATETIME,
     NUMBER,
     ROWID,
     STRING,
     Binary,
@@ -286,15 +292,15 @@
             uri = uri[len(prefix) :]
 
         adapter, args, kwargs = find_adapter(uri, self._adapter_kwargs, self._adapters)
         formatted_args = ", ".join(
             f"'{serialize(arg)}'"
             for arg in combine_args_kwargs(adapter, *args, **kwargs)
         )
-        table_name = escape(uri)
+        table_name = escape_identifier(uri)
         self._cursor.execute(
             f'CREATE VIRTUAL TABLE "{table_name}" USING {adapter.__name__}({formatted_args})',
         )
 
     def _get_description(self) -> Description:
         """
         Return the cursor description.
@@ -438,15 +444,22 @@
         apsw_connection_kwargs = apsw_connection_kwargs or {}
         self._connection = apsw.Connection(path, **apsw_connection_kwargs)
         self.isolation_level = isolation_level
         self.schema = schema
 
         # register adapters
         for adapter in adapters:
-            self._connection.createmodule(adapter.__name__, VTModule(adapter))
+            if Version(apsw.apswversion()) >= Version("3.41.0.0"):
+                self._connection.createmodule(
+                    adapter.__name__,
+                    VTModule(adapter),
+                    use_bestindex_object=adapter.supports_requested_columns,
+                )
+            else:
+                self._connection.createmodule(adapter.__name__, VTModule(adapter))
         self._adapters = adapters
         self._adapter_kwargs = adapter_kwargs
 
         # register functions
         available_functions = {
             "sleep": functions.sleep,
             "version": apsw_version,
```

### Comparing `shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 A dialect that only connects to GSheets.
 
 This dialect was implemented to replace the ``gsheetsdb`` library.
 """
 import logging
 import urllib.parse
+from datetime import timedelta
 from operator import itemgetter
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 import requests
 from google.auth.transport.requests import AuthorizedSession
 from sqlalchemy.engine.url import URL
 from sqlalchemy.pool.base import _ConnectionFairy
@@ -18,14 +19,17 @@
 from shillelagh.adapters.api.gsheets.lib import get_credentials
 from shillelagh.backends.apsw.dialects.base import APSWDialect
 from shillelagh.exceptions import ProgrammingError
 
 _logger = logging.getLogger(__name__)
 
 
+DEFAULT_TIMEOUT = timedelta(minutes=3)
+
+
 class QueryType(TypedDict, total=False):
     """
     Types for parameters in the SQLAlchemy URI query.
     """
 
     access_token: str
     service_account_file: str
@@ -115,14 +119,15 @@
 
     def do_ping(self, dbapi_connection: _ConnectionFairy) -> bool:
         """
         Return Google Sheets API status.
         """
         response = requests.get(
             "https://www.google.com/appsstatus/dashboard/incidents.json",
+            timeout=DEFAULT_TIMEOUT.total_seconds(),
         )
         payload = response.json()
 
         updates = [
             update for update in payload if update["service_name"] == "Google Sheets"
         ]
         if not updates:
```

### Comparing `shillelagh-1.2.0/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.1/src/shillelagh/backends/apsw/vt.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Set,
     Tuple,
     Type,
     cast,
 )
 
 import apsw
+from packaging.version import Version
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.fields import (
     Blob,
     FastISODateTime,
     Field,
@@ -47,14 +48,26 @@
     Index,
     RequestedOrder,
     Row,
     SQLiteConstraint,
     SQLiteValidType,
 )
 
+if Version(apsw.apswversion()) >= Version("3.41.0.0"):  # pragma: no cover
+    from apsw.ext import index_info_to_dict
+else:  # pragma: no cover
+    apsw.IndexInfo = Any  # for type annotation
+
+    # pylint: disable=unused-argument
+    def index_info_to_dict(index_info: apsw.IndexInfo) -> None:
+        """
+        Dummy function for testing.
+        """
+
+
 _logger = logging.getLogger(__name__)
 
 
 # map between APSW operators and the ``Operator`` enum
 operator_map = {
     apsw.SQLITE_INDEX_CONSTRAINT_EQ: Operator.EQ,
     apsw.SQLITE_INDEX_CONSTRAINT_GE: Operator.GE,
@@ -165,14 +178,15 @@
 
     all_bounds: DefaultDict[str, Set[Tuple[Operator, Any]]] = defaultdict(set)
     for (column_index, sqlite_index_constraint), constraint in zip(
         indexes,
         constraintargs,
     ):
         if sqlite_index_constraint not in operator_map:
+            # pylint: disable=broad-exception-raised
             raise Exception(f"Invalid constraint passed: {sqlite_index_constraint}")
         if column_index == LIMIT_OFFSET_INDEX:
             continue
         operator = operator_map[sqlite_index_constraint]
         column_name = column_names[column_index]
         column_type = columns[column_name]
 
@@ -195,14 +209,15 @@
     limit = offset = None
 
     for (column_index, sqlite_index_constraint), constraint in zip(
         indexes,
         constraintargs,
     ):
         if sqlite_index_constraint not in operator_map:
+            # pylint: disable=broad-exception-raised
             raise Exception(f"Invalid constraint passed: {sqlite_index_constraint}")
         if column_index != LIMIT_OFFSET_INDEX:
             continue
         operator = operator_map[sqlite_index_constraint]
         if operator == Operator.LIMIT:
             limit = constraint
         elif operator == Operator.OFFSET:
@@ -239,14 +254,15 @@
         column_type = columns[column_name]
         operators = {operation[0] for operation in operations}
         for class_ in column_type.filters:
             if all(operator in class_.operators for operator in operators):
                 bounds[column_name] = class_.build(operations)
                 break
         else:
+            # pylint: disable=broad-exception-raised
             raise Exception("No valid filter found")
 
     return bounds
 
 
 class VTModule:  # pylint: disable=too-few-public-methods
 
@@ -298,14 +314,15 @@
 
     Each row has a unique 64 bit integer rowid with the Cursor routines operating
     on this number, as well as some of the Table routines such as UpdateChangeRow.
     """
 
     def __init__(self, adapter: Adapter):
         self.adapter = adapter
+        self.requested_columns: Optional[Set[str]] = None
 
     def get_create_table(self, tablename: str) -> str:
         """
         Return the table's ``CREATE TABLE`` statement.
         """
         columns = self.adapter.get_columns()
         if not columns:
@@ -338,30 +355,33 @@
 
         indexes: List[Index] = []
         constraints_used: List[Constraint] = []
         filter_index = 0
         filtered_columns: List[Tuple[str, Operator]] = []
         for column_index, sqlite_index_constraint in constraints:
             operator = operator_map.get(sqlite_index_constraint)
-            column_name = column_names[column_index]
-            column_type = column_types[column_index]
-            for class_ in column_type.filters:
-                if operator in class_.operators:
-                    filtered_columns.append((column_name, operator))
-                    constraints_used.append((filter_index, column_type.exact))
-                    filter_index += 1
-                    indexes.append((column_index, sqlite_index_constraint))
-                    break
-            else:
-                if (operator is Operator.LIMIT and self.adapter.supports_limit) or (
-                    operator is Operator.OFFSET and self.adapter.supports_offset
-                ):
-                    constraints_used.append((filter_index, True))
-                    filter_index += 1
-                    indexes.append((LIMIT_OFFSET_INDEX, sqlite_index_constraint))
+
+            # LIMIT/OFFSET
+            if (operator is Operator.LIMIT and self.adapter.supports_limit) or (
+                operator is Operator.OFFSET and self.adapter.supports_offset
+            ):
+                constraints_used.append((filter_index, True))
+                filter_index += 1
+                indexes.append((LIMIT_OFFSET_INDEX, sqlite_index_constraint))
+            # column operator
+            elif column_index >= 0:
+                column_name = column_names[column_index]
+                column_type = column_types[column_index]
+                for class_ in column_type.filters:
+                    if operator in class_.operators:
+                        filtered_columns.append((column_name, operator))
+                        constraints_used.append((filter_index, column_type.exact))
+                        filter_index += 1
+                        indexes.append((column_index, sqlite_index_constraint))
+                        break
                 else:
                     constraints_used.append(None)
 
         # estimate query cost
         order = get_order(orderbys, column_names)
         estimated_cost = self.adapter.get_cost(filtered_columns, order)
 
@@ -385,19 +405,55 @@
             constraints_used,
             index_number,
             index_name,
             orderby_consumed,
             estimated_cost,
         )
 
+    def BestIndexObject(self, index_info: apsw.IndexInfo) -> bool:
+        """
+        Alternative to ``BestIndex`` that allows returning only selected columns.
+        """
+        columns = self.adapter.get_columns()
+        column_names = list(columns.keys())
+        self.requested_columns = {column_names[i] for i in index_info.colUsed}
+
+        index_info_dict = index_info_to_dict(index_info)
+        constraints = [
+            (constraint.get("iColumn", -1), constraint["op"])
+            for constraint in index_info_dict["aConstraint"]
+        ]
+        orderbys = [
+            (orderby["iColumn"], orderby["desc"])
+            for orderby in index_info_dict["aOrderBy"]
+        ]
+        (
+            constraints_used,
+            index_number,
+            index_name,
+            orderby_consumed,
+            estimated_cost,
+        ) = self.BestIndex(constraints, orderbys)
+
+        for i, constraint in enumerate(constraints_used):
+            if isinstance(constraint, tuple):
+                index_info.set_aConstraintUsage_argvIndex(i, constraint[0] + 1)
+                index_info.set_aConstraintUsage_omit(i, constraint[1])
+        index_info.idxNum = index_number
+        index_info.idxStr = index_name
+        index_info.orderByConsumed = orderby_consumed
+        index_info.estimatedCost = estimated_cost
+
+        return True
+
     def Open(self) -> "VTCursor":
         """
         Returns a cursor object.
         """
-        return VTCursor(self.adapter)
+        return VTCursor(self.adapter, self.requested_columns)
 
     def Disconnect(self) -> None:
         """
         The opposite of VTModule.Connect().
 
         This method is called when a reference to a virtual table is no longer used,
         but VTTable.Destroy() will be called when the table is no longer used.
@@ -445,16 +501,17 @@
 
 
 class VTCursor:
     """
     An object for iterating over a table.
     """
 
-    def __init__(self, adapter: Adapter):
+    def __init__(self, adapter: Adapter, requested_columns: Optional[Set[str]] = None):
         self.adapter = adapter
+        self.requested_columns = requested_columns
 
         self.data: Iterator[Tuple[Any, ...]]
         self.current_row: Tuple[Any, ...]
         self.eof = False
 
     def Filter(  # pylint: disable=too-many-locals
         self,
@@ -481,19 +538,21 @@
         limit, offset = get_limit_offset(indexes, constraintargs)
         bounds = get_bounds(columns, all_bounds)
 
         # compute requested order
         order = get_order(orderbys, column_names)
 
         # limit and offset were introduced in 1.1, and not all adapters support it
-        kwargs = {}
+        kwargs: Dict[str, Any] = {}
         if self.adapter.supports_limit:
             kwargs["limit"] = limit
         if self.adapter.supports_offset:
             kwargs["offset"] = offset
+        if self.adapter.supports_requested_columns:
+            kwargs["requested_columns"] = self.requested_columns
 
         rows = self.adapter.get_rows(bounds, order, **kwargs)
         rows = convert_rows_to_sqlite(columns, rows)
 
         # if a given column is not present, replace it with ``None``
         self.data = (
             tuple(row.get(name) for name in ["rowid", *column_names]) for row in rows
```

### Comparing `shillelagh-1.2.0/src/shillelagh/console.py` & `shillelagh-1.2.1/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/exceptions.py` & `shillelagh-1.2.1/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/fields.py` & `shillelagh-1.2.1/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/filters.py` & `shillelagh-1.2.1/src/shillelagh/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     if operator == Operator.GT:
         return Endpoint(value, False, Side.LEFT), Endpoint(None, True, Side.RIGHT)
     if operator == Operator.LE:
         return Endpoint(None, True, Side.LEFT), Endpoint(value, True, Side.RIGHT)
     if operator == Operator.LT:
         return Endpoint(None, True, Side.LEFT), Endpoint(value, False, Side.RIGHT)
 
+    # pylint: disable=broad-exception-raised
     raise Exception(f"Invalid operator: {operator}")
 
 
 class Filter:
     """
     A filter representing a SQL predicate.
     """
```

### Comparing `shillelagh-1.2.0/src/shillelagh/functions.py` & `shillelagh-1.2.1/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/lib.py` & `shillelagh-1.2.1/src/shillelagh/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         3 three
         10 four
 
     """
 
     def __init__(self, ranges: List[range]):
         if not ranges:
+            # pylint: disable=broad-exception-raised
             raise Exception("Argument ``ranges`` cannot be empty")
 
         self.ranges = ranges
 
     def __iter__(self):
         yield from itertools.chain(*self.ranges)
 
@@ -90,14 +91,15 @@
 
     def check_row_id(self, row_id: int) -> None:
         """
         Check if a provided row ID is not being used.
         """
         for range_ in self.ranges:
             if range_.start <= row_id < range_.stop:
+                # pylint: disable=broad-exception-raised
                 raise Exception(f"Row ID {row_id} already present")
 
     def insert(self, row_id: Optional[int] = None) -> int:
         """
         Insert a new row ID.
         """
         if row_id is None:
@@ -128,14 +130,15 @@
                 else:
                     self.ranges[i] = range(range_.start, row_id)
                     self.ranges.insert(i + 1, range(row_id + 1, range_.stop))
                     self.ranges.insert(i + 1, DELETED)
 
                 return
 
+        # pylint: disable=broad-exception-raised
         raise Exception(f"Row ID {row_id} not found")
 
 
 def analyze(  # pylint: disable=too-many-branches
     data: Iterator[Row],
 ) -> Tuple[int, Dict[str, Order], Dict[str, Type[Field]]]:
     """
@@ -217,24 +220,34 @@
             return Order.NONE
     except TypeError:
         return Order.NONE
 
     return current_order
 
 
-def escape(value: str) -> str:
+def escape_string(value: str) -> str:
     """Escape single quotes."""
     return value.replace("'", "''")
 
 
-def unescape(value: str) -> str:
+def unescape_string(value: str) -> str:
     """Unescape single quotes."""
     return value.replace("''", "'")
 
 
+def escape_identifier(value: str) -> str:
+    """Escape double quotes."""
+    return value.replace('"', '""')
+
+
+def unescape_identifier(value: str) -> str:
+    """Unescape double quotes."""
+    return value.replace('""', '"')
+
+
 def serialize(value: Any) -> str:
     """
     Serialize adapter arguments.
 
     This function is used with the SQLite backend, in order to serialize
     the arguments needed to instantiate an adapter via a virtual table.
     """
@@ -243,25 +256,25 @@
     except ValueError as ex:
         raise ProgrammingError(
             f"The argument {value} is not serializable because it has type "
             f"{type(value)}. Make sure only basic types (list, dicts, strings, "
             "numbers) are passed as arguments to adapters.",
         ) from ex
 
-    return escape(base64.b64encode(serialized).decode())
+    return escape_string(base64.b64encode(serialized).decode())
 
 
 def deserialize(value: str) -> Any:
     """
     Deserialize adapter arguments.
 
     This function is used by the SQLite backend, in order to deserialize
     the virtual table definition and instantiate an adapter.
     """
-    return marshal.loads(base64.b64decode(unescape(value).encode()))
+    return marshal.loads(base64.b64decode(unescape_string(value).encode()))
 
 
 def build_sql(  # pylint: disable=too-many-locals, too-many-arguments, too-many-branches
     columns: Dict[str, Field],
     bounds: Dict[str, Filter],
     order: List[Tuple[str, RequestedOrder]],
     table: Optional[str] = None,
```

### Comparing `shillelagh-1.2.0/src/shillelagh/types.py` & `shillelagh-1.2.1/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh/typing.py` & `shillelagh-1.2.1/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.1/src/shillelagh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.0
+Version: 1.2.1
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
@@ -161,14 +161,15 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: console
```

### Comparing `shillelagh-1.2.0/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.1/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.1/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.1/src/shillelagh.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 apsw>=3.9.2
 python_dateutil>=2.8.1
 requests>=2.25.1
 sqlalchemy>=1.3
+greenlet>=2.0.2
 typing_extensions>=3.7.4.3
+packaging
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [all]
 PyYAML>=5.4
 appdirs>=1.4.4
@@ -20,15 +22,15 @@
 pandas>=1.2.2
 pip-tools>=6.4.0
 pre-commit>=2.13.0
 prompt_toolkit>=3
 psutil>=5.8.0
 pyfakefs>=4.3.3
 pygments>=2.8
-pylint>=2.11.1
+pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=6.2.2
 requests-cache==0.7.1
 requests-mock>=1.8.0
 requests>=2.25.1
@@ -77,26 +79,27 @@
 
 [testing]
 PyYAML>=5.4
 appdirs>=1.4.4
 beautifulsoup4>=4.11.1
 boto3>=1.24.28
 codespell>=2.1.0
+dill>=0.3.6
 freezegun>=1.1.0
 google-auth>=1.23.0
 html5lib>=1.1
 jsonpath-python>=1.0.5
 pandas>=1.2.2
 pip-tools>=6.4.0
 pre-commit>=2.13.0
 prompt_toolkit>=3
 psutil>=5.8.0
 pyfakefs>=4.3.3
 pygments>=2.8
-pylint>=2.11.1
+pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=7.2.0
 requests-cache==0.7.1
 requests-mock>=1.8.0
 requests>=2.25.1
```

### Comparing `shillelagh-1.2.0/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.1/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.1/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.1/tests/adapters/api/generic_json_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Test the generic JSON adapter.
 """
 
 import pytest
 from pytest_mock import MockerFixture
-from requests import Session
 from requests_mock.mocker import Mocker
 from yarl import URL
 
 from shillelagh.adapters.api.generic_json import GenericJSONAPI
 from shillelagh.backends.apsw.db import connect
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.typing import Maybe
@@ -16,18 +15,15 @@
 baseurl = URL("https://api.stlouisfed.org/fred/series")
 
 
 def test_generic_json(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query.
     """
-    mocker.patch(
-        "shillelagh.adapters.api.generic_json.requests_cache.CachedSession",
-        return_value=Session(),
-    )
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
 
     # for datassette and other probing adapters
     requests_mock.head(
         "https://api.stlouisfed.org/-/versions.json?"
         "series_id=GNPCA&"
         "api_key=abcdefghijklmnopqrstuvwxyz123456&"
         "file_type=json#$.seriess%5B*%5D",
@@ -68,16 +64,16 @@
         },
     )
 
     connection = connect(":memory:")
     cursor = connection.cursor()
 
     sql = f'SELECT * FROM "{url}"'
-    data = list(cursor.execute(sql))
-    assert data == [
+    rows = list(cursor.execute(sql))
+    assert rows == [
         (
             "GNPCA",
             "2022-11-01",
             "2022-11-01",
             "Real Gross National Product",
             "1929-01-01",
             "2021-01-01",
@@ -98,16 +94,16 @@
         headers={"content-type": "application/json"},
     )
     requests_mock.get(
         "https://example.org/data.json",
         json=[{"a": 1, "b": [10, 20]}, {"a": 2, "b": [11]}],
     )
     sql = 'SELECT a, b FROM "https://example.org/data.json"'
-    data = list(cursor.execute(sql))
-    assert data == [(1, "[10, 20]"), (2, "[11]")]
+    rows = list(cursor.execute(sql))
+    assert rows == [(1, "[10, 20]"), (2, "[11]")]
 
     requests_mock.get(
         "https://example.org/data.json",
         json={"message": "An error occurred"},
         status_code=500,
     )
     with pytest.raises(ProgrammingError) as excinfo:
@@ -118,18 +114,15 @@
 def test_generic_json_complex_type(
     mocker: MockerFixture,
     requests_mock: Mocker,
 ) -> None:
     """
     Test a query where columns are complex.
     """
-    mocker.patch(
-        "shillelagh.adapters.api.generic_json.requests_cache.CachedSession",
-        return_value=Session(),
-    )
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
 
     # for datassette and other probing adapters
     requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
 
     url = URL("https://example.org/")
     requests_mock.head(str(url), headers={"content-type": "application/json"})
     requests_mock.get(
@@ -142,16 +135,16 @@
         ],
     )
 
     connection = connect(":memory:")
     cursor = connection.cursor()
 
     sql = f'SELECT * FROM "{url}"'
-    data = list(cursor.execute(sql))
-    assert data == [("bar", '["one", "two"]')]
+    rows = list(cursor.execute(sql))
+    assert rows == [("bar", '["one", "two"]')]
 
 
 def test_supports(requests_mock: Mocker) -> None:
     """
     Test the ``supports`` method.
     """
     requests_mock.head(
@@ -163,7 +156,52 @@
         headers={"content-type": "application/json"},
     )
 
     assert GenericJSONAPI.supports("/etc/password") is False
     assert GenericJSONAPI.supports("https://example.org/data.html") is Maybe
     assert GenericJSONAPI.supports("https://example.org/data.html", fast=False) is False
     assert GenericJSONAPI.supports("https://example.org/data.json", fast=False) is True
+
+
+def test_request_headers(mocker: MockerFixture, requests_mock: Mocker) -> None:
+    """
+    Test passing requests headers.
+    """
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    supports = requests_mock.head(
+        "https://example.org/data.json",
+        headers={"content-type": "application/json"},
+    )
+
+    # for datassette and other probing adapters
+    requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
+
+    url = URL("https://example.org/")
+    data = requests_mock.head(str(url), headers={"content-type": "application/json"})
+    requests_mock.get(
+        str(url),
+        json=[
+            {
+                "foo": "bar",
+                "baz": ["one", "two"],
+            },
+        ],
+    )
+
+    # test the supports method
+    GenericJSONAPI.supports(
+        "https://example.org/data.json",
+        fast=False,
+        request_headers={"foo": "bar"},
+    )
+    assert supports.last_request.headers["foo"] == "bar"
+
+    connection = connect(
+        ":memory:",
+        adapter_kwargs={"genericjsonapi": {"request_headers": {"foo": "bar"}}},
+    )
+    cursor = connection.cursor()
+
+    sql = f'SELECT * FROM "{url}"'
+    rows = list(cursor.execute(sql))
+    assert rows == [("bar", '["one", "two"]')]
+    assert data.last_request.headers["foo"] == "bar"
```

### Comparing `shillelagh-1.2.0/tests/adapters/api/github_test.py` & `shillelagh-1.2.1/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.1/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.1/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.1/tests/adapters/api/socrata_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,20 +240,20 @@
     """
     Test fetching data from the CDC.
     """
     connection = connect(":memory:", adapter_kwargs=adapter_kwargs)
     cursor = connection.cursor()
 
     sql = """
-        SELECT administered_dose1_recip_4
+        SELECT administered
         FROM "https://data.cdc.gov/resource/unsk-b7fc.json"
         WHERE location = ? AND date = ?
     """
-    cursor.execute(sql, ("US", date(2021, 7, 4)))
-    assert cursor.fetchall() == [(67.1,)]
+    cursor.execute(sql, ("US", date(2023, 3, 1)))
+    assert cursor.fetchall() == [(672076105.0,)]
 
 
 def test_get_cost(mocker: MockerFixture) -> None:
     """
     Test ``get_cost``.
     """
     mocker.patch(
```

### Comparing `shillelagh-1.2.0/tests/adapters/api/system_test.py` & `shillelagh-1.2.1/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.1/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/base_test.py` & `shillelagh-1.2.1/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.1/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.1/tests/adapters/memory/pandas_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -276,7 +276,21 @@
     cursor.execute(sql)
     assert cursor.fetchall() == [
         (10, 15.2, "Diamond_St"),
         (11, 13.1, "Blacktail_Loop"),
         (12, 13.3, "Platinum_St"),
         (13, 12.1, "Kodiak_Trail"),
     ]
+
+
+def test_empty_dataframe() -> None:
+    """
+    Test that empty dataframes work.
+    """
+    emptydf = pd.DataFrame({"a": []})  # noqa: F841  pylint: disable=unused-variable
+
+    connection = connect(":memory:")
+    cursor = connection.cursor()
+
+    sql = "SELECT * FROM emptydf"
+    cursor.execute(sql)
+    assert cursor.fetchall() == []
```

### Comparing `shillelagh-1.2.0/tests/adapters/registry_test.py` & `shillelagh-1.2.1/tests/adapters/registry_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,9 +69,10 @@
         raise ImportError("Error!")
 
     registry.add("valid", FakeAdapter)
     registry.loaders["invalid"].append(load_error)
 
     assert registry.load_all(["valid"]) == {"valid": FakeAdapter}
     with pytest.raises(InterfaceError) as excinfo:
-        registry.load_all()
+        registry.load_all(["valid", "invalid"])
     assert str(excinfo.value) == "Unable to load adapter invalid"
+    assert registry.load_all() == {"valid": FakeAdapter}
```

### Comparing `shillelagh-1.2.0/tests/backends/apsw/db_test.py` & `shillelagh-1.2.1/tests/backends/apsw/db_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Any, List, Tuple
 from unittest import mock
 
 import apsw
 import pytest
 from pytest_mock import MockerFixture
 
-from shillelagh.adapters.registry import AdapterLoader
-from shillelagh.backends.apsw.db import connect, convert_binding
-from shillelagh.exceptions import InterfaceError, NotSupportedError, ProgrammingError
+from shillelagh.adapters.registry import AdapterLoader, UnsafeAdaptersError
+from shillelagh.backends.apsw.db import Connection, connect, convert_binding
+from shillelagh.exceptions import NotSupportedError, ProgrammingError
 from shillelagh.fields import Float, String, StringInteger
 
 from ...fakes import FakeAdapter
 
 
 def test_connect(registry: AdapterLoader) -> None:
     """
@@ -174,15 +174,15 @@
         "main",
     )
 
     # prevent repeated names, in case anyone registers a malicious adapter
     registry.clear()
     registry.add("one", FakeAdapter1)
     registry.add("one", FakeAdapter2)
-    with pytest.raises(InterfaceError) as excinfo:
+    with pytest.raises(UnsafeAdaptersError) as excinfo:
         connect(":memory:", ["one"], safe=True)
     assert str(excinfo.value) == "Multiple adapters found with name one"
 
 
 def test_execute_with_native_parameters(registry: AdapterLoader) -> None:
     """
     Test passing native types to the cursor.
@@ -473,7 +473,34 @@
     drop_table = mocker.patch.object(FakeAdapter, "drop_table")
 
     connection = connect(":memory:", ["dummy"], isolation_level="IMMEDIATE")
     cursor = connection.cursor()
 
     cursor.execute('DROP TABLE "dummy://"')
     drop_table.assert_called()  # type: ignore
+
+
+def test_best_index(mocker: MockerFixture) -> None:
+    """
+    Test that ``use_bestindex_object`` is only passed for apsw >= 3.41.0.0
+    """
+    # pylint: disable=redefined-outer-name, invalid-name
+    apsw = mocker.patch("shillelagh.backends.apsw.db.apsw")
+    VTModule = mocker.patch("shillelagh.backends.apsw.db.VTModule")
+    adapter = mocker.MagicMock()
+    adapter.__name__ = "some_adapter"
+    adapter.supports_requested_columns = True
+
+    apsw.apswversion.return_value = "3.41.0.0"
+    Connection(":memory:", [adapter], {})
+    apsw.Connection().createmodule.assert_called_with(
+        "some_adapter",
+        VTModule(adapter),
+        use_bestindex_object=True,
+    )
+
+    apsw.apswversion.return_value = "3.40.1.0"
+    Connection(":memory:", [adapter], {})
+    apsw.Connection().createmodule.assert_called_with(
+        "some_adapter",
+        VTModule(adapter),
+    )
```

### Comparing `shillelagh-1.2.0/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.1/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.1/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.1/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.1/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.1/tests/backends/apsw/vt_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     table = VTTable(adapter)
     result = table.BestIndex(
         [
             (1, apsw.SQLITE_INDEX_CONSTRAINT_EQ),  # name =
             (2, apsw.SQLITE_INDEX_CONSTRAINT_GT),  # pets >
             (0, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # age <=
             (-1, 73),  # LIMIT
+            (-1, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # INVALID, just for coverage
         ],
         [(1, False)],  # ORDER BY name ASC
     )
     assert result == (
         [(0, True), None, (1, True), (2, True)],
         42,
         (
@@ -107,14 +108,65 @@
             "[[1, false]]]"
         ),
         True,
         666,
     )
 
 
+def test_virtual_best_index_object(mocker: MockerFixture) -> None:
+    """
+    Test ``BestIndexObject``.
+    """
+    index_info = mocker.MagicMock()
+    index_info.colUsed = {0, 2}
+    index_info_to_dict = mocker.patch("shillelagh.backends.apsw.vt.index_info_to_dict")
+    index_info_to_dict.return_value = {
+        "aConstraint": [
+            {"iColumn": 1, "op": apsw.SQLITE_INDEX_CONSTRAINT_EQ},
+            {"iColumn": 2, "op": apsw.SQLITE_INDEX_CONSTRAINT_GT},
+            {"iColumn": 0, "op": apsw.SQLITE_INDEX_CONSTRAINT_LE},
+            {"op": 73},
+        ],
+        "aOrderBy": [{"iColumn": 1, "desc": False}],
+    }
+
+    adapter = FakeAdapter()
+    adapter.supports_limit = True
+
+    table = VTTable(adapter)
+    assert table.requested_columns is None
+
+    result = table.BestIndexObject(index_info)
+    assert result is True
+    assert table.requested_columns == {"age", "pets"}
+
+    index_info.set_aConstraintUsage_argvIndex.assert_has_calls(
+        [
+            mocker.call(0, 1),
+            mocker.call(2, 2),
+            mocker.call(3, 3),
+        ],
+    )
+    index_info.set_aConstraintUsage_omit.assert_has_calls(
+        [
+            mocker.call(0, True),
+            mocker.call(2, True),
+            mocker.call(3, True),
+        ],
+    )
+    assert index_info.idxNum == 42
+    assert index_info.idxStr == (
+        f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}], "
+        f"[0, {apsw.SQLITE_INDEX_CONSTRAINT_LE}], [-1, 73]], "
+        "[[1, false]]]"
+    )
+    assert index_info.orderByConsumed is True
+    assert index_info.estimatedCost == 666
+
+
 def test_virtual_best_index_static_order_not_consumed() -> None:
     """
     Test ``BestIndex`` when the adapter cannot consume the order.
     """
     table = VTTable(FakeAdapterStaticSort())
     result = table.BestIndex(
         [
```

### Comparing `shillelagh-1.2.0/tests/conftest.py` & `shillelagh-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/console_test.py` & `shillelagh-1.2.1/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/__init__.py` & `shillelagh-1.2.1/tests/fakes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Fake objects to simplify testing.
 """
+
 import json
 import os
 import urllib.parse
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.fields import Float, Integer, Order, String
```

### Comparing `shillelagh-1.2.0/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.1/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.1/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.1/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.1/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.1/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.1/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/datasette_results.json` & `shillelagh-1.2.1/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/github_response.json` & `shillelagh-1.2.1/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/github_single_response.json` & `shillelagh-1.2.1/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/incidents.json` & `shillelagh-1.2.1/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.1/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/fields_test.py` & `shillelagh-1.2.1/tests/fields_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for shillelagh.fields.
 """
 import datetime
+import sys
 from typing import Union
 
 import pytest
 
 from shillelagh.adapters.registry import registry
 from shillelagh.backends.apsw.db import connect
 from shillelagh.exceptions import ProgrammingError
@@ -496,14 +497,15 @@
         1,
         1,
         12,
         0,
         0,
     )
 
-    with pytest.raises(ProgrammingError) as excinfo:
-        FastISODateTime().parse("2020-01-01T12:00Z")
-    assert str(excinfo.value) == 'Unable to parse "2020-01-01T12:00Z"'
+    if sys.version_info < (3, 11):
+        with pytest.raises(ProgrammingError) as excinfo:
+            FastISODateTime().parse("2020-01-01T12:00Z")
+        assert str(excinfo.value) == 'Unable to parse "2020-01-01T12:00Z"'
 
     with pytest.raises(ProgrammingError) as excinfo:
         FastISODateTime().parse("invalid")
     assert str(excinfo.value) == 'Unable to parse "invalid"'
```

### Comparing `shillelagh-1.2.0/tests/filters_test.py` & `shillelagh-1.2.1/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/functions_test.py` & `shillelagh-1.2.1/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.0/tests/lib_test.py` & `shillelagh-1.2.1/tests/lib_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,23 @@
     DELETED,
     RowIDManager,
     analyze,
     apply_limit_and_offset,
     build_sql,
     combine_args_kwargs,
     deserialize,
-    escape,
+    escape_identifier,
+    escape_string,
     filter_data,
     find_adapter,
     is_not_null,
     is_null,
     serialize,
-    unescape,
+    unescape_identifier,
+    unescape_string,
     update_order,
 )
 from shillelagh.typing import RequestedOrder
 
 
 def test_row_id_manager_empty_range() -> None:
     """
@@ -268,28 +270,52 @@
     """
     columns: Dict[str, Field] = {"a": String(), "b": Float()}
 
     with pytest.raises(ImpossibleFilterError):
         build_sql(columns, {"a": Impossible()}, [])
 
 
-def test_escape() -> None:
+def test_escape_string() -> None:
     """
-    Test ``escape``.
+    Test ``escape_string``.
     """
-    assert escape("1") == "1"
-    assert escape("O'Malley's") == "O''Malley''s"
+    assert escape_string("1") == "1"
+    assert escape_string("O'Malley's") == "O''Malley''s"
 
 
-def test_unescape() -> None:
+def test_unescape_string() -> None:
     """
-    Test ``unescape``.
+    Test ``unescape_string``.
     """
-    assert unescape("1") == "1"
-    assert unescape("O''Malley''s") == "O'Malley's"
+    assert unescape_string("1") == "1"
+    assert unescape_string("O''Malley''s") == "O'Malley's"
+
+
+def test_escape_identifier() -> None:
+    """
+    Test ``escape_identifier``.
+    """
+    assert escape_identifier("1") == "1"
+    assert escape_identifier("O'Malley's") == "O'Malley's"
+    assert (
+        escape_identifier('a dove called: "Who? who? who?"')
+        == 'a dove called: ""Who? who? who?""'
+    )
+
+
+def test_unescape_identifier() -> None:
+    """
+    Test ``unescape_identifier``.
+    """
+    assert unescape_identifier("1") == "1"
+    assert unescape_identifier("O''Malley''s") == "O''Malley''s"
+    assert (
+        unescape_identifier('a dove called: ""Who? who? who?""')
+        == 'a dove called: "Who? who? who?"'
+    )
 
 
 def test_serialize() -> None:
     """
     Test ``serialize``.
     """
     assert serialize(["O'Malley's"]) == "2wEAAAD6Ck8nTWFsbGV5J3M="
```

### Comparing `shillelagh-1.2.0/tests/types_test.py` & `shillelagh-1.2.1/tests/types_test.py`

 * *Files identical despite different names*

