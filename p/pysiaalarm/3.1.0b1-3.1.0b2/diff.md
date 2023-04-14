# Comparing `tmp/pysiaalarm-3.1.0b1.tar.gz` & `tmp/pysiaalarm-3.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysiaalarm-3.1.0b1.tar", last modified: Tue Dec  6 11:49:59 2022, max compression
+gzip compressed data, was "pysiaalarm-3.1.0b2.tar", last modified: Tue Dec  6 13:15:43 2022, max compression
```

## Comparing `pysiaalarm-3.1.0b1.tar` & `pysiaalarm-3.1.0b2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.386012 pysiaalarm-3.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.362012 pysiaalarm-3.1.0b1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.350012 pysiaalarm-3.1.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.362012 pysiaalarm-3.1.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.366012 pysiaalarm-3.1.0b1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 11:49:59.386012 pysiaalarm-3.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      354 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.370012 pysiaalarm-3.1.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    67606 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    58035 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/SIA Codes.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   133582 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/SIA_code.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.370012 pysiaalarm-3.1.0b1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/codes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/codes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/pytest.old
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2022-12-06 11:49:59.386012 pysiaalarm-3.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.354012 pysiaalarm-3.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.374012 pysiaalarm-3.1.0b1/src/pysiaalarm/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.378012 pysiaalarm-3.1.0b1/src/pysiaalarm/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.378012 pysiaalarm-3.1.0b1/src/pysiaalarm/data/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/data/adm_mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    58799 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/data/sia_codes.json
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/data/xdata.json
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20270 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.382012 pysiaalarm-3.1.0b1/src/pysiaalarm/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/sync/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/sync/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.382012 pysiaalarm-3.1.0b1/src/pysiaalarm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/src/pysiaalarm/utils/regexes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.378012 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 11:49:59.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2022-12-06 11:49:59.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 11:49:59.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 11:49:37.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 11:49:59.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-06 11:49:59.000000 pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 11:49:59.382012 pysiaalarm-3.1.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/encrypted_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/ha.json
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/run_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/run_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/test_alarm_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/test_sia_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/test_sia_package_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tests/unencrypted_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2022-12-06 11:49:21.000000 pysiaalarm-3.1.0b1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.372448 pysiaalarm-3.1.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.384448 pysiaalarm-3.1.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    67606 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    58035 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA Codes.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   133582 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA_code.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.384448 pysiaalarm-3.1.0b2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/codes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/codes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pytest.old
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2022-12-06 13:15:43.400448 pysiaalarm-3.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.372448 pysiaalarm-3.1.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.388448 pysiaalarm-3.1.0b2/src/pysiaalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/adm_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58799 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/sia_codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/xdata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20270 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/regexes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.388448 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:15:26.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/encrypted_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/ha.json
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_alarm_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_sia_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_sia_package_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/unencrypted_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tox.ini
```

### Comparing `pysiaalarm-3.1.0b1/.coveragerc` & `pysiaalarm-3.1.0b2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.devcontainer/Dockerfile` & `pysiaalarm-3.1.0b2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.devcontainer/devcontainer.json` & `pysiaalarm-3.1.0b2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.github/workflows/main.yml` & `pysiaalarm-3.1.0b2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.github/workflows/release.yaml` & `pysiaalarm-3.1.0b2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.gitignore` & `pysiaalarm-3.1.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.vscode/launch.json` & `pysiaalarm-3.1.0b2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/.vscode/settings.json` & `pysiaalarm-3.1.0b2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/LICENSE.txt` & `pysiaalarm-3.1.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/PKG-INFO` & `pysiaalarm-3.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiaalarm
-Version: 3.1.0b1
+Version: 3.1.0b2
 Summary: Python package for creating a client that talks with SIA-based alarm systems.
 Author: E.A. van Valkenburg
 Author-email: github@vanvalkenburg.eu
 License: MIT
 Project-URL: Documentation, https://github.com/eavanvalkenburg/pysiaalarm
 Project-URL: Source, https://github.com/eavanvalkenburg/pysiaalarm
 Platform: any
```

### Comparing `pysiaalarm-3.1.0b1/README.md` & `pysiaalarm-3.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/Makefile` & `pysiaalarm-3.1.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx` & `pysiaalarm-3.1.0b2/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/SIA Codes.xlsx` & `pysiaalarm-3.1.0b2/docs/SIA Codes.xlsx`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/SIA_code.pdf` & `pysiaalarm-3.1.0b2/docs/SIA_code.pdf`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/codes.csv` & `pysiaalarm-3.1.0b2/docs/codes.csv`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/codes.pdf` & `pysiaalarm-3.1.0b2/docs/codes.pdf`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/conf.py` & `pysiaalarm-3.1.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/docs/index.rst` & `pysiaalarm-3.1.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/pytest.ini` & `pysiaalarm-3.1.0b2/pytest.ini`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/pytest.old` & `pysiaalarm-3.1.0b2/pytest.old`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/setup.cfg` & `pysiaalarm-3.1.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/setup.py` & `pysiaalarm-3.1.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/__init__.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/__init__.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/account.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/account.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/aio/client.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/aio/client.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/aio/server.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/aio/server.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/base_client.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/base_client.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/base_server.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/base_server.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/data/adm_mapping.json` & `pysiaalarm-3.1.0b2/src/pysiaalarm/data/adm_mapping.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/data/data.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/data/data.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/data/sia_codes.json` & `pysiaalarm-3.1.0b2/src/pysiaalarm/data/sia_codes.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/data/xdata.json` & `pysiaalarm-3.1.0b2/src/pysiaalarm/data/xdata.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/errors.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/errors.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/event.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/event.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/sync/client.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/client.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/sync/handler.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/handler.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/sync/server.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/server.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/utils/counter.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/counter.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/utils/enums.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm/utils/regexes.py` & `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/regexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,51 +27,57 @@
 (?P<line>L[A-Fa-f0-9]{1,6})
 [#]?(?P<account>[A-Fa-f0-9]{3,16})?
 [\[]
 (?P<rest>.*)
 """
 MAIN_MATCHER = re.compile(main_regex, re.X)
 
-sia_content_regex = r"""
+# Content matcher, with shared pre and post expressions.
+xdata_ts_regex = r"""
+[\]]
+(?:\[(?:(?<=\[)(?P<xdata>.*)(?=\]))\])?
+(?:_(?<=_)(?P<timestamp>[0-9:,-]*)?)?$
+"""
+
+sia_content_regex = (
+    r"""
 [#]?(?P<account>[A-Fa-f0-9]{3,16})?
 [|]?
 [N]?
 (?:ti)?(?:(?<=ti)(?P<ti>\d{2}:\d{2}))?\/?
 (?:id)?(?:(?<=id)(?P<id>\d*))?\/?
 (?:ri)?(?:(?<=ri)(?P<ri>\d*))?\/?
 (?P<code>[a-zA-Z]{2})?
 (?P<message>.[^\[\]]*)?
-[\]]
-(?:\[(?:(?<=\[)(?P<xdata>.*)(?=\]))\])?
-[_]?
-(?P<timestamp>[0-9:,-]*)?$
 """
-SIA_CONTENT_MATCHER = re.compile(sia_content_regex, re.X)
+    + xdata_ts_regex
+)
 
-encr_sia_content_regex = r"""(?:[^\|\[\]]*)[|]?"""
-ENCR_SIA_CONTENT_MATCHER = re.compile(encr_sia_content_regex + sia_content_regex, re.X)
-
-adm_content_regex = r"""
+adm_content_regex = (
+    r"""
 [#]?(?P<account>[A-F0-9]{3,16})?
 [|]?
 (?P<event_qualifier>\d{1})
 (?P<event_type>\d{3})
 \s
 (?P<partition>\d{2})
 \s
 (?P<ri>\d{3})
-[\]]
-(?:\[(?:(?<=\[)(?P<xdata>.[^\[\]]*)(?=\]))\])?
-[_]?
-(?P<timestamp>[0-9:,-]*)?$
 """
-ADM_CONTENT_MATCHER = re.compile(adm_content_regex, re.X)
+    + xdata_ts_regex
+)
 
-encr_adm_content_regex = r"""(?:[^\|\[\]]*)[|]?"""
-ENCR_ADM_CONTENT_MATCHER = re.compile(encr_adm_content_regex + adm_content_regex, re.X)
+encr_content_regex = r"""
+(?:[^\|\[\]]*)[|]?
+"""
+
+SIA_CONTENT_MATCHER = re.compile(sia_content_regex, re.X)
+ADM_CONTENT_MATCHER = re.compile(adm_content_regex, re.X)
+ENCR_SIA_CONTENT_MATCHER = re.compile(encr_content_regex + sia_content_regex, re.X)
+ENCR_ADM_CONTENT_MATCHER = re.compile(encr_content_regex + adm_content_regex, re.X)
 
 
 def _get_matcher(
     message_type: MessageTypes | str, encrypted: bool = False
 ) -> re.Pattern:
     """Extract the content using the different regexes."""
     if message_type == MessageTypes.ADMCID:
```

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/PKG-INFO` & `pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiaalarm
-Version: 3.1.0b1
+Version: 3.1.0b2
 Summary: Python package for creating a client that talks with SIA-based alarm systems.
 Author: E.A. van Valkenburg
 Author-email: github@vanvalkenburg.eu
 License: MIT
 Project-URL: Documentation, https://github.com/eavanvalkenburg/pysiaalarm
 Project-URL: Source, https://github.com/eavanvalkenburg/pysiaalarm
 Platform: any
```

### Comparing `pysiaalarm-3.1.0b1/src/pysiaalarm.egg-info/SOURCES.txt` & `pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/run.py` & `pysiaalarm-3.1.0b2/tests/run.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/run_aio.py` & `pysiaalarm-3.1.0b2/tests/run_aio.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/run_re.py` & `pysiaalarm-3.1.0b2/tests/run_re.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/test_alarm.py` & `pysiaalarm-3.1.0b2/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/test_alarm_aio.py` & `pysiaalarm-3.1.0b2/tests/test_alarm_aio.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/test_sia_package.py` & `pysiaalarm-3.1.0b2/tests/test_sia_package.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/test_sia_package_cases.py` & `pysiaalarm-3.1.0b2/tests/test_sia_package_cases.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tests/test_utils.py` & `pysiaalarm-3.1.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b1/tox.ini` & `pysiaalarm-3.1.0b2/tox.ini`

 * *Files identical despite different names*

