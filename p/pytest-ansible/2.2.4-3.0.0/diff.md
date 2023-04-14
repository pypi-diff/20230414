# Comparing `tmp/pytest-ansible-2.2.4.tar.gz` & `tmp/pytest-ansible-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-2.2.4.tar", last modified: Tue May 25 19:20:52 2021, max compression
+gzip compressed data, was "pytest-ansible-3.0.0.tar", last modified: Fri Apr 14 16:27:42 2023, max compression
```

## Comparing `pytest-ansible-2.2.4.tar` & `pytest-ansible-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,71 @@
-drwxrwxr-x   0 elijah    (1000) elijah    (1000)        0 2021-05-25 19:20:52.270917 pytest-ansible-2.2.4/
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1486 2019-06-20 18:30:25.000000 pytest-ansible-2.2.4/HISTORY.md
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1078 2019-06-20 18:30:25.000000 pytest-ansible-2.2.4/LICENSE
--rw-rw-r--   0 elijah    (1000) elijah    (1000)       86 2019-06-20 18:30:25.000000 pytest-ansible-2.2.4/MANIFEST.in
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      916 2021-05-25 19:20:52.270917 pytest-ansible-2.2.4/PKG-INFO
--rw-rw-r--   0 elijah    (1000) elijah    (1000)    12674 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/README.md
-drwxrwxr-x   0 elijah    (1000) elijah    (1000)        0 2021-05-25 19:20:52.267917 pytest-ansible-2.2.4/pytest_ansible/
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      133 2021-05-25 17:02:51.000000 pytest-ansible-2.2.4/pytest_ansible/__init__.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      678 2019-06-20 18:30:25.000000 pytest-ansible-2.2.4/pytest_ansible/errors.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1267 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/fixtures.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      444 2019-06-20 18:30:25.000000 pytest-ansible-2.2.4/pytest_ansible/has_version.py
-drwxrwxr-x   0 elijah    (1000) elijah    (1000)        0 2021-05-25 19:20:52.269917 pytest-ansible-2.2.4/pytest_ansible/host_manager/
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     4090 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/__init__.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      670 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/v1.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      998 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/v2.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1034 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/v24.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1034 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/v25.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     1034 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/host_manager/v28.py
-drwxrwxr-x   0 elijah    (1000) elijah    (1000)        0 2021-05-25 19:20:52.270917 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     2057 2020-10-26 18:39:00.000000 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/__init__.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     3096 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v1.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     5317 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v2.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     5237 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v24.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     5763 2021-05-25 17:01:27.000000 pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v28.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)    10874 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/plugin.py
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     2740 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/pytest_ansible/results.py
-drwxrwxr-x   0 elijah    (1000) elijah    (1000)        0 2021-05-25 19:20:52.268917 pytest-ansible-2.2.4/pytest_ansible.egg-info/
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      916 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/PKG-INFO
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      902 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/SOURCES.txt
--rw-rw-r--   0 elijah    (1000) elijah    (1000)        1 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/dependency_links.txt
--rw-rw-r--   0 elijah    (1000) elijah    (1000)       51 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/entry_points.txt
--rw-rw-r--   0 elijah    (1000) elijah    (1000)        1 2019-09-13 18:30:25.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/not-zip-safe
--rw-rw-r--   0 elijah    (1000) elijah    (1000)       20 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/requires.txt
--rw-rw-r--   0 elijah    (1000) elijah    (1000)       15 2021-05-25 19:20:52.000000 pytest-ansible-2.2.4/pytest_ansible.egg-info/top_level.txt
--rw-rw-r--   0 elijah    (1000) elijah    (1000)      644 2021-05-25 19:20:52.271917 pytest-ansible-2.2.4/setup.cfg
--rw-rw-r--   0 elijah    (1000) elijah    (1000)     4456 2020-10-26 22:14:57.000000 pytest-ansible-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.765158 pytest-ansible-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.741158 pytest-ansible-3.0.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.741158 pytest-ansible-3.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.745158 pytest-ansible-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.745158 pytest-ansible-3.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-14 16:27:42.761157 pytest-ansible-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:27:42.765158 pytest-ansible-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.737158 pytest-ansible-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.749158 pytest-ansible-3.0.0/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.753157 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.757157 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.753157 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.761157 pytest-ansible-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tox.ini
```

### Comparing `pytest-ansible-2.2.4/HISTORY.md` & `pytest-ansible-3.0.0/HISTORY.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 ## Release History
 
 ### 2.0.1 (2018-08-10)
 
-* Convert AdHocResult.values() to return a list, not a generator (Thanks Alan Rominger)
-* Preliminary support for py3
+- Convert AdHocResult.values() to return a list, not a generator (Thanks Alan Rominger)
+- Preliminary support for py3
 
 ### 2.0.0 (2017-07-27)
 
-* Major changes to allow ansible-style inventory indexing
-* Improved results processing using python objects, rather than dictionaries
+- Major changes to allow ansible-style inventory indexing
+- Improved results processing using python objects, rather than dictionaries
 
 ### 1.4.0 (2016-MM-DD)
 
-* Add parameter --ansible-module-path (thanks David Barroso)
-* Raise DeprecationWarnings for scope=class fixtures
+- Add parameter --ansible-module-path (thanks David Barroso)
+- Raise DeprecationWarnings for scope=class fixtures
 
 ### 1.3.1 (2016-01-22)
 
-* Correctly handle ansible become options
+- Correctly handle ansible become options
 
 ### 1.3.0 (2016-01-20)
 
-* Add support for ansible-2.0
+- Add support for ansible-2.0
 
 ### 1.2.5 (2015-04-20)
 
-* Only validate --ansible-* parameters when using pytest-ansible fixture
-* Include --ansible-user when running module
+- Only validate --ansible-\* parameters when using pytest-ansible fixture
+- Include --ansible-user when running module
 
 ### 1.2.4 (2015-03-18)
 
-* Add ansible-1.9 privilege escalation support
+- Add ansible-1.9 privilege escalation support
 
 ### 1.2.3 (2015-03-03)
 
-* Resolve setuptools import failure by migrating from a module to a package
+- Resolve setuptools import failure by migrating from a module to a package
 
 ### 1.2.2 (2015-03-03)
 
-* Removed py module dependency
-* Add HISTORY.md
+- Removed py module dependency
+- Add HISTORY.md
 
 ### 1.2.1 (2015-03-02)
 
-* Use pandoc to convert existing markdown into pypi friendly rst
+- Use pandoc to convert existing markdown into pypi friendly rst
 
 ### 1.2 (2015-03-02)
 
-* Add `ansible_host` and `ansible_group` parametrized fixture
-* Add cls level fixtures for users needing scope=class fixtures
-* Updated examples to match new fixture return value
-* Alter fixture return data to more closely align with ansible
-* Raise `AnsibleHostUnreachable` whenever hosts are ... unreachable
-* Set contacted and dark hosts in ConnectionError
+- Add `ansible_host` and `ansible_group` parametrized fixture
+- Add cls level fixtures for users needing scope=class fixtures
+- Updated examples to match new fixture return value
+- Alter fixture return data to more closely align with ansible
+- Raise `AnsibleHostUnreachable` whenever hosts are ... unreachable
+- Set contacted and dark hosts in ConnectionError
 
 ### 1.1 (2015-02-16)
 
-* Initial release
+- Initial release
```

### Comparing `pytest-ansible-2.2.4/LICENSE` & `pytest-ansible-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-2.2.4/README.md` & `pytest-ansible-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,107 @@
 # pytest-ansible
 
-[![Build Status](https://github.com/ansible/pytest-ansible/workflows/CI/badge.svg)](https://github.com/ansible/pytest-ansible/actions)
-[![Requirements Status](https://requires.io/github/ansible/pytest-ansible/requirements.svg?branch=master)](https://requires.io/github/ansible/pytest-ansible/requirements/?branch=master)
+[![Build Status](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml)
 [![Version](https://img.shields.io/pypi/v/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![License](https://img.shields.io/pypi/l/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 
-
-This repository contains a plugin for ``py.test`` which adds several fixtures
-for running ``ansible`` modules, or inspecting ``ansible_facts``.  While one
-can simply call out to ``ansible`` using the ``subprocess`` module, having to
+This repository contains a plugin for `py.test` which adds several fixtures
+for running `ansible` modules, or inspecting `ansible_facts`. While one
+can simply call out to `ansible` using the `subprocess` module, having to
 parse stdout to determine the outcome of the operation is unpleasant and prone
-to error.  With ``pytest-ansible``, modules return JSON data which you can
+to error. With `pytest-ansible`, modules return JSON data which you can
 inspect and act on, much like with an ansible
 [playbook](http://docs.ansible.com/playbooks.html).
 
 ## Installation
 
-Install this plugin using ``pip``
+Install this plugin using `pip`
 
 ```bash
 pip install pytest-ansible
 ```
 
 ## Usage
 
-Once installed, the following ``py.test`` command-line parameters are available:
+Once installed, the following `py.test` command-line parameters are available:
 
 ```bash
 py.test \
     [--inventory <path_to_inventory>] \
+    [--extra-inventory <path_to_extra_inventory>] \
     [--host-pattern <host-pattern>] \
     [--connection <plugin>] \
     [--module-path <path_to_modules] \
     [--user <username>] \
     [--become] \
     [--become-user <username>] \
     [--become-method <method>] \
     [--limit <limit>] \
     [--check]
 ```
 
 ## Inventory
 
-Using ansible first starts with defining your inventory.  This can be done
-several ways, but to start, we'll use the ``ansible_adhoc`` fixture.
+Using ansible first starts with defining your inventory. This can be done
+several ways, but to start, we'll use the `ansible_adhoc` fixture.
 
 ```python
 def test_my_inventory(ansible_adhoc):
     hosts = ansible_adhoc()
 ```
 
 In the example above, the `hosts` variable is an instance of the `HostManager`
-class and describes your ansible inventory.  For this to work, you'll need to
-tell `ansible` where to find your inventory.  Inventory can be anything
+class and describes your ansible inventory. For this to work, you'll need to
+tell `ansible` where to find your inventory. Inventory can be anything
 supported by ansible, which includes an [INI
 file](http://docs.ansible.com/ansible/latest/intro_inventory.html) or an
 executable script that returns [properly formatted
 JSON](http://docs.ansible.com/ansible/latest/intro_dynamic_inventory.html).
-For example, 
+For example,
 
 ```bash
 py.test --inventory my_inventory.ini --host-pattern all
 ```
 
-or 
+or
 
 ```bash
 py.test --inventory path/to/my/script.py --host-pattern webservers
 ```
-or 
+
+or
 
 ```bash
 py.test --inventory one.example.com,two.example.com --host-pattern all
 ```
 
 In the above examples, the inventory provided at runtime will be used in all
-tests that use the `ansible_adhoc` fixture.  A more realistic scenario may
+tests that use the `ansible_adhoc` fixture. A more realistic scenario may
 involve using different inventory files (or host patterns) with different
-tests.  To accomplish this, the fixture `ansible_adhoc` allows you to customize
-the inventory parameters.  Read on for more detail on using the `ansible_adhoc`
+tests. To accomplish this, the fixture `ansible_adhoc` allows you to customize
+the inventory parameters. Read on for more detail on using the `ansible_adhoc`
 fixture.
 
-### Fixture ``ansible_adhoc``
+## Extra Inventory
+
+Using ansible first starts with defining your extra inventory. This feature was added in version 2.3.0, and is intended
+to allow the user to work with two different inventories. This can be done in several ways, but to start,
+we'll use the `ansible_adhoc` fixture.
+
+For example,
+
+```bash
+py.test --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
+```
+
+### Fixture `ansible_adhoc`
 
 The `ansible_adhoc` fixture returns a function used to initialize
-a `HostManager` object.  The `ansible_adhoc` fixture will default to parameters
+a `HostManager` object. The `ansible_adhoc` fixture will default to parameters
 supplied to the `py.test` command-line, but also allows one to provide keyword
 arguments used to initialize the inventory.
 
 The example below demonstrates basic usage with options supplied at run-time to
 `py.test`.
 
 ```python
@@ -99,21 +111,21 @@
 
 The following example demonstrates available keyword arguments when creating
 a `HostManager` object.
 
 ```python
 def test_uptime(ansible_adhoc):
     # take down the database
-    ansible_adhoc(inventory='db1.example.com,', user='ec2-user', 
+    ansible_adhoc(inventory='db1.example.com,', user='ec2-user',
         become=True, become_user='root').all.command('reboot')
 ```
 
 The `HostManager` object returned by the `ansible_adhoc()` function provides
 numerous ways of calling ansible modules against some, or all, of the
-inventory.  The following demonstates sample usage.
+inventory. The following demonstates sample usage.
 
 ```python
 def test_host_manager(ansible_adhoc):
     hosts = ansible_adhoc()
 
     # __getitem__
     hosts['all'].ping()
@@ -132,18 +144,18 @@
 
     assert hasattr(hosts, 'two.example.com')
 
     for a_host in hosts:
         a_host.ping()
 ```
 
-### Fixture ``localhost``
+### Fixture `localhost`
 
 The `localhost` fixture is a convenience fixture that surfaces
-a `ModuleDispatcher` instance for ansible host running `pytest`.  This is
+a `ModuleDispatcher` instance for ansible host running `pytest`. This is
 convenient when using ansible modules that typically run on the local machine,
 such as cloud modules (ec2, gce etc...).
 
 ```python
 def test_do_something_cloudy(localhost, ansible_adhoc):
     """Deploy an ec2 instance using multiple fixtures."""
     params = dict(
@@ -160,21 +172,21 @@
     # Deploy an ec2 instance from localhost using the `ansible_adhoc` fixture
     ansible_adhoc(inventory='localhost,', connection='local').localhost.ec2(**params)
 
     # Deploy an ec2 instance from localhost using the `localhost` fixture
     localhost.ec2(**params)
 ```
 
-### Fixture ``ansible_module``
+### Fixture `ansible_module`
 
-The ``ansible_module`` fixture allows tests and fixtures to call [ansible
-modules](http://docs.ansible.com/modules.html).  Unlike the `ansible_adhoc`
+The `ansible_module` fixture allows tests and fixtures to call [ansible
+modules](http://docs.ansible.com/modules.html). Unlike the `ansible_adhoc`
 fixture, this fixture only uses the options supplied to `py.test` at run time.
 
-A very basic example demonstrating the ansible [``ping`` module](http://docs.ansible.com/ping_module.html):
+A very basic example demonstrating the ansible [`ping` module](http://docs.ansible.com/ping_module.html):
 
 ```python
 def test_ping(ansible_module):
     ansible_module.ping()
 ```
 
 A more involved example of updating the sshd configuration, and restarting the
@@ -205,56 +217,56 @@
     for (host, result) in contacted.items():
         assert 'changed' in result and result['changed']
         assert result['name'] == 'sshd'
 
     # do other stuff ...
 ```
 
-### Fixture ``ansible_facts``
+### Fixture `ansible_facts`
 
-The ``ansible_facts`` fixture returns a JSON structure representing the system
-facts for the associated inventory.  Sample fact data is available in the
+The `ansible_facts` fixture returns a JSON structure representing the system
+facts for the associated inventory. Sample fact data is available in the
 [ansible
 documentation](http://docs.ansible.com/playbooks_variables.html#information-discovered-from-systems-facts).
 
 Note, this fixture is provided for convenience and could easily be called using
-``ansible_module.setup()``.
+`ansible_module.setup()`.
 
 A systems facts can be useful when deciding whether to skip a test ...
 
 ```python
 def test_something_with_amazon_ec2(ansible_facts):
     for facts in ansible_facts:
         if 'ec2.internal' != facts['ansible_domain']:
             pytest.skip("This test only applies to ec2 instances")
 
 ```
 
 Additionally, since facts are just ansible modules, you could inspect the
-contents of the ``ec2_facts`` module for greater granularity ...
+contents of the `ec2_facts` module for greater granularity ...
 
 ```python
 
 def test_terminate_us_east_1_instances(ansible_adhoc):
 
     for facts in ansible_adhoc().all.ec2_facts():
         if facts['ansible_ec2_placement_region'].startswith('us-east'):
             '''do some testing'''
 ```
 
-### Parameterizing with ``pytest.mark.ansible``
+### Parameterizing with `pytest.mark.ansible`
 
-Perhaps the ``--ansible-inventory=<inventory>`` includes many systems, but you
-only wish to interact with a subset.  The ``pytest.mark.ansible`` marker can be
-used to modify the ``pytest-ansible`` command-line parameters for a single
-test.  Please note, the fixture `ansible_adhoc` is the prefer mechanism for
+Perhaps the `--ansible-inventory=<inventory>` includes many systems, but you
+only wish to interact with a subset. The `pytest.mark.ansible` marker can be
+used to modify the `pytest-ansible` command-line parameters for a single
+test. Please note, the fixture `ansible_adhoc` is the prefer mechanism for
 interacting with ansible inventory within tests.
 
 For example, to interact with the local system, you would adjust the
-``host_pattern`` and ``connection`` parameters.
+`host_pattern` and `connection` parameters.
 
 ```python
 @pytest.mark.ansible(host_pattern='local,', connection='local')
 def test_copy_local(ansible_module):
 
     # create a file with random data
     contacted = ansible_module.copy(
@@ -273,15 +285,15 @@
     assert 'local' in contacted
 
     # assert the copy module reported changes
     assert 'changed' in contacted['local']
     assert contacted['local']['changed']
 ```
 
-Note, the parameters provided by ``pytest.mark.ansible`` will apply to all
+Note, the parameters provided by `pytest.mark.ansible` will apply to all
 class methods.
 
 ```python
 @pytest.mark.ansible(host_pattern='local,', connection='local')
 class Test_Local(object):
     def test_install(self, ansible_module):
         '''do some testing'''
@@ -290,16 +302,16 @@
     def test_service(self, ansible_module):
         '''do some testing'''
 ```
 
 ### Inspecting results
 
 When using the `ansible_adhoc`, `localhost` or `ansible_module` fixtures, the
-object returned will be an instance of class ``AdHocResult``.  The
-``AdHocResult`` class can be inspected as follows:
+object returned will be an instance of class `AdHocResult`. The
+`AdHocResult` class can be inspected as follows:
 
 ```python
 
 def test_adhoc_result(ansible_adhoc):
     contacted = ansible_adhoc(inventory=my_inventory).command("date")
 
     # As a dictionary
@@ -323,23 +335,23 @@
     # With __getattr__
     assert contacted.localhost.is_successful
 
     # Or __gettem__
     assert contacted['localhost'].is_successful
 ```
 
-Using the ``AdHocResult`` object provides ways to conveniently access results
+Using the `AdHocResult` object provides ways to conveniently access results
 for different hosts involved in the ansible adhoc command. Once the specific
 host result is found, you may inspect the result of the ansible adhoc command
-on that use by way of the ``ModuleResult`` interface.  The ``ModuleResult``
+on that use by way of the `ModuleResult` interface. The `ModuleResult`
 class represents the dictionary returned by the ansible module for a particular
-host.  The contents of the dictionary depend on the module called.
+host. The contents of the dictionary depend on the module called.
 
-The ``ModuleResult`` interface provides some convenient proprerties to
-determine the success of the module call.  Examples are included below.
+The `ModuleResult` interface provides some convenient proprerties to
+determine the success of the module call. Examples are included below.
 
 ```python
 
 def test_module_result(localhost):
     contacted = localhost.command("find /tmp")
 
     assert contacted.localhost.is_successful
@@ -349,32 +361,32 @@
 
     contacted = localhost.shell("exit 1")
     assert contacted.localhost.is_failed
     assert not contacted.localhost.is_successful
 ```
 
 The contents of the JSON returned by an ansible module differs from module to
-module.  For guidance, consult the documentation and examples for the specific
+module. For guidance, consult the documentation and examples for the specific
 [ansible module](http://docs.ansible.com/modules_by_category.html).
 
 ### Exception handling
 
-If ``ansible`` is unable to connect to any inventory, an exception will be raised.
+If `ansible` is unable to connect to any inventory, an exception will be raised.
 
 ```python
 @pytest.mark.ansible(inventory='unreachable.example.com,')
 def test_shutdown(ansible_module):
 
     # attempt to ping a host that is down (or doesn't exist)
     pytest.raises(pytest_ansible.AnsibleHostUnreachable):
         ansible_module.ping()
 ```
 
 Sometimes, only a single host is unreachable, and others will have properly
-returned data.  The following demonstrates how to catch the exception, and
+returned data. The following demonstrates how to catch the exception, and
 inspect the results.
 
 ```python
 @pytest.mark.ansible(inventory='good:bad')
 def test_inventory_unreachable(ansible_module):
     exc_info = pytest.raises(pytest_ansible.AnsibleHostUnreachable, ansible_module.ping)
     (contacted, dark) = exc_info.value.results
@@ -382,8 +394,7 @@
     # inspect the JSON result...
     for (host, result) in contacted.items():
         assert result['ping'] == 'pong'
 
     for (host, result) in dark.items():
         assert result['failed'] == True
 ```
-
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/errors.py` & `pytest-ansible-3.0.0/src/pytest_ansible/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 import ansible.errors
 
 
 class AnsibleNoHostsMatch(ansible.errors.AnsibleError):
 
     """Sub-class AnsibleError when no hosts match."""
 
-    pass
-
 
 class AnsibleConnectionFailure(ansible.errors.AnsibleError):
 
     """Sub-class AnsibleError when connection failures occur."""
 
     def __init__(self, msg, dark=None, contacted=None):
         """Initialize connection error class."""
-        super(AnsibleConnectionFailure, self).__init__(msg)
+        super().__init__(msg)
         self.contacted = contacted
         self.dark = dark
 
 
 class AnsibleModuleError(ansible.errors.AnsibleError):
 
     """Sub-class AnsibleError when module failures occur."""
-
-    pass
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/fixtures.py` & `pytest-ansible-3.0.0/src/pytest_ansible/fixtures.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """PyTest fixtures."""
 
 import pytest
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture()
 def ansible_adhoc(request):
     """Return an inventory initialization method."""
     plugin = request.config.pluginmanager.getplugin("ansible")
 
     def init_host_mgr(**kwargs):
         return plugin.initialize(request.config, request, **kwargs)
+
     return init_host_mgr
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture()
 def ansible_module(ansible_adhoc):
     """Return a subclass of BaseModuleDispatcher."""
     host_mgr = ansible_adhoc()
-    return getattr(host_mgr, host_mgr.options['host_pattern'])
+    return getattr(host_mgr, host_mgr.options["host_pattern"])
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture()
 def ansible_facts(ansible_module):
     """Return ansible_facts dictionary."""
     return ansible_module.setup()
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture()
 def localhost(request):
     """Return a host manager representing localhost."""
     # NOTE: Do not use ansible_adhoc as a dependent fixture since that will assert specific command-line parameters have
     # been supplied.  In the case of localhost, the parameters are provided as kwargs below.
     plugin = request.config.pluginmanager.getplugin("ansible")
-    return plugin.initialize(request.config, request, inventory='localhost,', connection='local',
-                             host_pattern='localhost').localhost
+    return plugin.initialize(
+        request.config,
+        request,
+        inventory="localhost,",
+        connection="local",
+        host_pattern="localhost",
+    ).localhost
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,156 @@
 """Fixme."""
 
 import ansible
-from pytest_ansible.has_version import (
-    has_ansible_v2,
-    has_ansible_v24,
-    has_ansible_v28,
-)
 
+from pytest_ansible.has_version import has_ansible_v2
+from pytest_ansible.has_version import has_ansible_v24
+from pytest_ansible.has_version import has_ansible_v28
+from pytest_ansible.has_version import has_ansible_v29
+from pytest_ansible.has_version import has_ansible_v212
+from pytest_ansible.has_version import has_ansible_v213
 
 
-class BaseHostManager(object):
-
+class BaseHostManager:
     """Fixme."""
 
-    _required_kwargs = ('inventory',)
+    _required_kwargs = ("inventory",)
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
         self.options = kwargs
 
         self.check_required_kwargs(**kwargs)
 
         # Sub-classes should override this value
-        self._dispatcher = None
+        self._dispatcher = self._default_dispatcher
 
         # Initialize ansible inventory manager
         self.initialize_inventory()
 
+    def _default_dispatcher(self, **kwargs):
+        pass
+
+    def get_extra_inventory_hosts(self, host_pattern=None):
+        try:
+            if host_pattern is None:
+                extra_inventory_hosts = [
+                    h.name for h in self.options["extra_inventory_manager"].list_hosts()
+                ]
+            else:
+                extra_inventory_hosts = [
+                    h.name
+                    for h in self.options["extra_inventory_manager"].list_hosts(
+                        host_pattern
+                    )
+                ]
+        except KeyError:
+            extra_inventory_hosts = []
+        return extra_inventory_hosts
+
+    def get_extra_inventory_groups(self):
+        try:
+            extra_inventory_groups = self.options["extra_inventory_manager"].groups
+        except KeyError:
+            extra_inventory_groups = []
+        return extra_inventory_groups
+
     def check_required_kwargs(self, **kwargs):
         """Raise a TypeError if any required kwargs are missing."""
         for kwarg in self._required_kwargs:
             if kwarg not in self.options:
-                raise TypeError("Missing required keyword argument '%s'" % kwarg)
+                raise TypeError(f"Missing required keyword argument '{kwarg}'")
 
     def has_matching_inventory(self, host_pattern):
         """Return whether any matching ansible inventory is found for the provided host_pattern."""
         try:
-            return len(self.options['inventory_manager'].list_hosts(host_pattern)) > 0 or \
-                host_pattern in self.options['inventory_manager'].groups
+            return (
+                len(self.options["inventory_manager"].list_hosts(host_pattern)) > 0
+                or host_pattern in self.options["inventory_manager"].groups
+                or len(self.get_extra_inventory_hosts(host_pattern)) > 0
+                or host_pattern in self.get_extra_inventory_groups()
+            )
         except ansible.errors.AnsibleError:
             return False
 
     def __getitem__(self, item):
         """Return a ModuleDispatcher instance described the provided `item`."""
         # Handle slicing
         if isinstance(item, slice):
             new_item = "all["
             if item.start is not None:
                 new_item += str(item.start)
-            new_item += '-'
+            new_item += "-"
             if item.stop is not None:
                 new_item += str(item.stop)
-            item = new_item + ']'
+            item = new_item + "]"
 
         if item in self.__dict__:
             return self.__dict__[item]
-        else:
-            if not self.has_matching_inventory(item):
-                raise KeyError(item)
-            else:
-                self.options['host_pattern'] = item
-                return self._dispatcher(**self.options)
+        if not self.has_matching_inventory(item):
+            raise KeyError(item)
+        self.options["host_pattern"] = item
+        return self._dispatcher(**self.options)
 
     def __getattr__(self, attr):
         """Return a ModuleDispatcher instance described the provided `attr`."""
         if not self.has_matching_inventory(attr):
-            raise AttributeError("type HostManager has no attribute '%s'" % attr)
-        else:
-            self.options['host_pattern'] = attr
-            return self._dispatcher(**self.options)
+            raise AttributeError(f"type HostManager has no attribute '{attr}'")
+        self.options["host_pattern"] = attr
+        return self._dispatcher(**self.options)
 
     def keys(self):
-        return [h.name for h in self.options['inventory_manager'].list_hosts()]
+        inventory_hosts = [
+            h.name for h in self.options["inventory_manager"].list_hosts()
+        ]
+        extra_inventory_hosts = self.get_extra_inventory_hosts()
+        return inventory_hosts + extra_inventory_hosts
 
     def __iter__(self):
         """Return an iterator for hosts matching the `host_pattern`."""
-        all_hosts = self.options['inventory_manager'].list_hosts(self.options['host_pattern'])
+        extra_hosts = self.get_extra_inventory_hosts(
+            host_pattern=self.options["host_pattern"]
+        )
+        all_hosts = self.options["inventory_manager"].list_hosts(
+            self.options["host_pattern"]
+        )
         # Return only the name (ala .keys()
         # return iter(self.options['inventory_manager'].list_hosts(self.options['host_pattern']))
         # Return a BaseHostManager instance initialized for each host in the inventory
         # return iter([self.__class__(host_pattern=h, **self.options) for h in all_hosts])
         # Return a ModuleDispatcher representing the group
-        return iter([self[h] for h in all_hosts])
+        return iter([self[h] for h in all_hosts + extra_hosts])
 
     def __len__(self):
         """Return the number of inventory hosts."""
-        return len(self.options['inventory_manager'].list_hosts())
+        return len(self.options["inventory_manager"].list_hosts()) + len(
+            self.get_extra_inventory_hosts()
+        )
 
     def __contains__(self, item):
         """Return whether there is inventory matching the provided `item`."""
         return self.has_matching_inventory(item)
 
     def initialize_inventory(self):
         raise NotImplementedError("Must be implemented by sub-class")
 
 
 def get_host_manager(*args, **kwargs):
     """Initialize and return a HostManager instance."""
 
-    if has_ansible_v28:
+    if has_ansible_v213:
+        from pytest_ansible.host_manager.v213 import HostManagerV213 as HostManager
+    elif has_ansible_v212:
+        from pytest_ansible.host_manager.v212 import HostManagerV212 as HostManager
+    elif has_ansible_v29:
+        from pytest_ansible.host_manager.v29 import HostManagerV29 as HostManager
+    elif has_ansible_v28:
         from pytest_ansible.host_manager.v28 import HostManagerV28 as HostManager
     elif has_ansible_v24:
         from pytest_ansible.host_manager.v24 import HostManagerV24 as HostManager
-        # from .v24 import HostManagerV24 as HostManager
     elif has_ansible_v2:
         from pytest_ansible.host_manager.v2 import HostManagerV2 as HostManager
     else:
         from .v1 import HostManagerV1 as HostManager
 
     # TODO - figure out how to surface the parser defaults here too
     return HostManager(*args, **kwargs)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from ansible.inventory import Inventory
+
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v1 import ModuleDispatcherV1
 
 
 class HostManagerV1(BaseHostManager):
 
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
-        super(HostManagerV1, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV1
 
     def keys(self):
-        return [h for h in self.options['inventory_manager'].list_hosts()]
+        return list(self.options["inventory_manager"].list_hosts())
 
     def initialize_inventory(self):
-        self.options['inventory_manager'] = Inventory(self.options['inventory'])
+        self.options["inventory_manager"] = Inventory(self.options["inventory"])
         # self.options['inventory_manager'].subset(self.pattern)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+from ansible.inventory import Inventory
 from ansible.parsing.dataloader import DataLoader
+from ansible.vars import VariableManager
+
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
-from ansible.vars import VariableManager
-from ansible.inventory import Inventory
 
 
 class HostManagerV2(BaseHostManager):
 
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
-        super(HostManagerV2, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV2
 
     def initialize_inventory(self):
-
-        self.options['loader'] = DataLoader()
-        self.options['variable_manager'] = VariableManager()
-        self.options['inventory_manager'] = Inventory(loader=self.options['loader'],
-                                                      variable_manager=self.options['variable_manager'],
-                                                      host_list=self.options['inventory'])
-        self.options['variable_manager'].set_inventory(self.options['inventory_manager'])
+        self.options["loader"] = DataLoader()
+        self.options["variable_manager"] = VariableManager()
+        self.options["inventory_manager"] = Inventory(
+            loader=self.options["loader"],
+            variable_manager=self.options["variable_manager"],
+            host_list=self.options["inventory"],
+        )
+        self.options["variable_manager"].set_inventory(
+            self.options["inventory_manager"]
+        )
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v28.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+from ansible.inventory.manager import InventoryManager
 from ansible.parsing.dataloader import DataLoader
-from pytest_ansible.host_manager import BaseHostManager
-from pytest_ansible.module_dispatcher.v24 import ModuleDispatcherV24
 from ansible.vars.manager import VariableManager
-from ansible.inventory.manager import InventoryManager
+
+from pytest_ansible.host_manager import BaseHostManager
+from pytest_ansible.module_dispatcher.v28 import ModuleDispatcherV28
 
 
-class HostManagerV24(BaseHostManager):
+class HostManagerV28(BaseHostManager):
 
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
-        super(HostManagerV24, self).__init__(*args, **kwargs)
-        self._dispatcher = ModuleDispatcherV24
+        super().__init__(*args, **kwargs)
+        self._dispatcher = ModuleDispatcherV28
 
     def initialize_inventory(self):
-        self.options['loader'] = DataLoader()
-        self.options['inventory_manager'] = InventoryManager(loader=self.options['loader'],
-                                                             sources=self.options['inventory'])
-        self.options['variable_manager'] = VariableManager(loader=self.options['loader'],
-                                                           inventory=self.options['inventory_manager'])
+        self.options["loader"] = DataLoader()
+        self.options["inventory_manager"] = InventoryManager(
+            loader=self.options["loader"], sources=self.options["inventory"]
+        )
+        self.options["variable_manager"] = VariableManager(
+            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+        )
         # self.options['inventory_manager'].clear_caches()
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/v25.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v29.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+from ansible.inventory.manager import InventoryManager
 from ansible.parsing.dataloader import DataLoader
-from pytest_ansible.host_manager import BaseHostManager
-from pytest_ansible.module_dispatcher.v25 import ModuleDispatcherV25
 from ansible.vars.manager import VariableManager
-from ansible.inventory.manager import InventoryManager
 
+from pytest_ansible.host_manager import BaseHostManager
+from pytest_ansible.module_dispatcher.v29 import ModuleDispatcherV29
 
-class HostManagerV25(BaseHostManager):
 
+class HostManagerV29(BaseHostManager):
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
-        super(HostManagerV25, self).__init__(*args, **kwargs)
-        self._dispatcher = ModuleDispatcherV25
+        super().__init__(*args, **kwargs)
+        self._dispatcher = ModuleDispatcherV29
 
     def initialize_inventory(self):
-        self.options['loader'] = DataLoader()
-        self.options['inventory_manager'] = InventoryManager(loader=self.options['loader'],
-                                                             sources=self.options['inventory'])
-        self.options['variable_manager'] = VariableManager(loader=self.options['loader'],
-                                                           inventory=self.options['inventory_manager'])
-        # self.options['inventory_manager'].clear_caches()
+        self.options["loader"] = DataLoader()
+        self.options["inventory_manager"] = InventoryManager(
+            loader=self.options["loader"], sources=self.options["inventory"]
+        )
+        self.options["variable_manager"] = VariableManager(
+            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+        )
+        if "extra_inventory" in self.options:
+            self.options["extra_loader"] = DataLoader()
+            self.options["extra_inventory_manager"] = InventoryManager(
+                loader=self.options["extra_loader"],
+                sources=self.options["extra_inventory"],
+            )
+            self.options["extra_variable_manager"] = VariableManager(
+                loader=self.options["extra_loader"],
+                inventory=self.options["extra_inventory_manager"],
+            )
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v24.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+from ansible.inventory.manager import InventoryManager
 from ansible.parsing.dataloader import DataLoader
-from pytest_ansible.host_manager import BaseHostManager
-from pytest_ansible.module_dispatcher.v28 import ModuleDispatcherV28
 from ansible.vars.manager import VariableManager
-from ansible.inventory.manager import InventoryManager
+
+from pytest_ansible.host_manager import BaseHostManager
+from pytest_ansible.module_dispatcher.v24 import ModuleDispatcherV24
 
 
-class HostManagerV28(BaseHostManager):
+class HostManagerV24(BaseHostManager):
 
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Fixme."""
-        super(HostManagerV28, self).__init__(*args, **kwargs)
-        self._dispatcher = ModuleDispatcherV28
+        super().__init__(*args, **kwargs)
+        self._dispatcher = ModuleDispatcherV24
 
     def initialize_inventory(self):
-        self.options['loader'] = DataLoader()
-        self.options['inventory_manager'] = InventoryManager(loader=self.options['loader'],
-                                                             sources=self.options['inventory'])
-        self.options['variable_manager'] = VariableManager(loader=self.options['loader'],
-                                                           inventory=self.options['inventory_manager'])
+        self.options["loader"] = DataLoader()
+        self.options["inventory_manager"] = InventoryManager(
+            loader=self.options["loader"], sources=self.options["inventory"]
+        )
+        self.options["variable_manager"] = VariableManager(
+            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+        )
         # self.options['inventory_manager'].clear_caches()
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 """Define BaseModuleDispatcher class."""
 
+from typing import Sequence
+
 from pytest_ansible.errors import AnsibleModuleError
 
 
-class BaseModuleDispatcher(object):
+class BaseModuleDispatcher:
 
     """Fixme.."""
 
-    required_kwargs = ('inventory',)
+    required_kwargs: Sequence[str] = ("inventory",)
 
     def __init__(self, **kwargs):
         """Save provided keyword arguments and assert required values have been provided."""
         self.options = kwargs
 
         # Assert the expected kwargs were provided
         self.check_required_kwargs(**kwargs)
 
     def __len__(self):
         """Return the number of hosts that match the `host_pattern`."""
-        return len(self.options['inventory_manager'].list_hosts(self.options['host_pattern']))
+        return len(
+            self.options["inventory_manager"].list_hosts(self.options["host_pattern"])
+        )
 
     def __contains__(self, item):
         """Return the whether the inventory contains a host matching the provided `item`."""
-        return len(self.options['inventory_manager'].list_hosts(item)) > 0
+        return len(self.options["inventory_manager"].list_hosts(item)) > 0
 
     def __getattr__(self, name):
         """Run the ansible module matching the provided `name`.
 
         Raise `AnsibleModuleError` when no such module exists.
         """
         if not self.has_module(name):
             # TODO: should we just raise an AttributeError, or a more
             # raise AttributeError("'{0}' object has no attribute '{1}'".format(self.__class__.__name__, name))
-            raise AnsibleModuleError("The module {0} was not found in configured module paths.".format(name))
-        else:
-            self.options['module_name'] = name
-            return self._run
+            raise AnsibleModuleError(
+                f"The module {name} was not found in configured module paths."
+            )
+        self.options["module_name"] = name
+        return self._run
 
     def check_required_kwargs(self, **kwargs):
         """Raise a TypeError if any required kwargs are missing."""
         for kwarg in self.required_kwargs:
             if kwarg not in self.options:
-                raise TypeError("Missing required keyword argument '%s'" % kwarg)
+                raise TypeError(f"Missing required keyword argument '{kwarg}'")
 
     def has_module(self, name):
         """Return whether ansible provides the requested module."""
         raise RuntimeError("Must be implemented by a sub-class")
 
     def _run(self, *args, **kwargs):
         """Raise a runtime error, unless implemented by sub-classes."""
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 import warnings
+
 import ansible
 import ansible.constants
-import ansible.utils
 import ansible.errors
+import ansible.utils
 
 from ansible.runner import Runner
-from pytest_ansible.module_dispatcher import BaseModuleDispatcher
+
 from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.results import AdHocResult
 from pytest_ansible.has_version import has_ansible_v1
+from pytest_ansible.module_dispatcher import BaseModuleDispatcher
+from pytest_ansible.results import AdHocResult
 
 
 if not has_ansible_v1:
     raise ImportError("Only supported with ansible < 2.0")
 
 
 class ModuleDispatcherV1(BaseModuleDispatcher):
 
     """Pass."""
 
-    required_kwargs = ('inventory', 'inventory_manager', 'host_pattern')
+    required_kwargs = ("inventory", "inventory_manager", "host_pattern")
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
-        if 'module_path' in self.options:
-            paths = self.options['module_path']
+        if "module_path" in self.options:
+            paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
                     ansible.utils.module_finder.add_directory(path)
             else:
                 ansible.utils.module_finder.add_directory(paths)
 
         return ansible.utils.module_finder.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the results in a AdHocResult object."""
         # Assemble module argument string
-        if True:
-            module_args = ' '.join(module_args)
+        if module_args:
+            complex_args.update({"_raw_params": " ".join(module_args)})
         else:
-            if module_args:
-                complex_args.update(dict(_raw_params=' '.join(module_args)))
+            module_args = " ".join(module_args)
 
         # Assert hosts matching the provided pattern exist
-        hosts = self.options['inventory_manager'].list_hosts()
+        hosts = self.options["inventory_manager"].list_hosts()
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
-        self.options['inventory_manager'].subset(self.options.get('subset'))
-        hosts = self.options['inventory_manager'].list_hosts(self.options['host_pattern'])
+        self.options["inventory_manager"].subset(self.options.get("subset"))
+        hosts = self.options["inventory_manager"].list_hosts(
+            self.options["host_pattern"]
+        )
         if len(hosts) == 0 and not no_hosts:
-            raise ansible.errors.AnsibleError("Specified hosts and/or --limit does not match any hosts")
+            raise ansible.errors.AnsibleError(
+                "Specified hosts and/or --limit does not match any hosts"
+            )
 
         # Build module runner object
-        kwargs = dict(
-            inventory=self.options.get('inventory_manager'),
-            pattern=self.options.get('host_pattern'),
-            module_name=self.options.get('module_name'),
-            module_args=module_args,
-            complex_args=complex_args,
-            transport=self.options.get('connection'),
-            remote_user=self.options.get('user'),
-            module_path=self.options.get('module_path'),
-            become=self.options.get('become'),
-            become_method=self.options.get('become_method'),
-            become_user=self.options.get('become_user'),
-        )
+        kwargs = {
+            "inventory": self.options.get("inventory_manager"),
+            "pattern": self.options.get("host_pattern"),
+            "module_name": self.options.get("module_name"),
+            "module_args": module_args,
+            "complex_args": complex_args,
+            "transport": self.options.get("connection"),
+            "remote_user": self.options.get("user"),
+            "module_path": self.options.get("module_path"),
+            "become": self.options.get("become"),
+            "become_method": self.options.get("become_method"),
+            "become_user": self.options.get("become_user"),
+        }
 
         # Run the module
         runner = Runner(**kwargs)
         results = runner.run()
 
-
-        if 'dark' in results and results['dark']:
-            raise AnsibleConnectionFailure("Host unreachable", dark=results['dark'], contacted=results['contacted'])
+        if "dark" in results and results["dark"]:
+            raise AnsibleConnectionFailure(
+                "Host unreachable", dark=results["dark"], contacted=results["contacted"]
+            )
 
         # Success!
-        return AdHocResult(contacted=results['contacted'])
+        return AdHocResult(contacted=results["contacted"])
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,150 +1,169 @@
+from __future__ import annotations
+
 import warnings
+
+from typing import Sequence
+
 import ansible.constants
-import ansible.utils
 import ansible.errors
+import ansible.utils
 
-from ansible.plugins.callback import CallbackBase
-from ansible.executor.task_queue_manager import TaskQueueManager
-from ansible.playbook.play import Play
 # from ansible.plugins.loader import module_loader
 from ansible.cli import CLI
-from pytest_ansible.module_dispatcher import BaseModuleDispatcher
-from pytest_ansible.results import AdHocResult
+from ansible.executor.task_queue_manager import TaskQueueManager
+from ansible.playbook.play import Play
+from ansible.plugins.callback import CallbackBase
+
 from pytest_ansible.errors import AnsibleConnectionFailure
 from pytest_ansible.has_version import has_ansible_v2
+from pytest_ansible.module_dispatcher import BaseModuleDispatcher
+from pytest_ansible.results import AdHocResult
 
 
 if not has_ansible_v2:
     raise ImportError("Only supported with ansible-2.* and newer")
 
 
-
 class ResultAccumulator(CallbackBase):
-
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Initialize object."""
-        super(ResultAccumulator, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         self.contacted[result._host.get_name()] = result._result
 
     v2_runner_on_ok = v2_runner_on_failed
 
     def v2_runner_on_unreachable(self, result):
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
-        return dict(contacted=self.contacted, unreachable=self.unreachable)
+        return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
 class ModuleDispatcherV2(BaseModuleDispatcher):
-
     """Pass."""
 
-    required_kwargs = ('inventory', 'inventory_manager', 'variable_manager', 'host_pattern', 'loader')
+    required_kwargs: Sequence[str] = (
+        "inventory",
+        "inventory_manager",
+        "variable_manager",
+        "host_pattern",
+        "loader",
+    )
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
-        if 'module_path' in self.options:
-            paths = self.options['module_path']
+        if "module_path" in self.options:
+            paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
                     ansible.plugins.module_loader.add_directory(path)
             else:
                 ansible.plugins.module_loader.add_directory(paths)
 
         return ansible.plugins.module_loader.has_plugin(name)
         # return module_loader.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the result in a AdhocResult object."""
         # Assemble module argument string
         if module_args:
-            complex_args.update(dict(_raw_params=' '.join(module_args)))
+            complex_args.update({"_raw_params": " ".join(module_args)})
 
         # Assert hosts matching the provided pattern exist
-        hosts = self.options['inventory_manager'].list_hosts()
+        hosts = self.options["inventory_manager"].list_hosts()
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
-        self.options['inventory_manager'].subset(self.options.get('subset'))
-        hosts = self.options['inventory_manager'].list_hosts(self.options['host_pattern'])
+        self.options["inventory_manager"].subset(self.options.get("subset"))
+        hosts = self.options["inventory_manager"].list_hosts(
+            self.options["host_pattern"]
+        )
         if len(hosts) == 0 and not no_hosts:
-            raise ansible.errors.AnsibleError("Specified hosts and/or --limit does not match any hosts")
-
+            raise ansible.errors.AnsibleError(
+                "Specified hosts and/or --limit does not match any hosts"
+            )
 
         parser = CLI.base_parser(
             runas_opts=True,
             inventory_opts=True,
             async_opts=True,
             output_opts=True,
             connect_opts=True,
             check_opts=True,
             runtask_opts=True,
             vault_opts=True,
             fork_opts=True,
             module_opts=True,
         )
-        (options, args) = parser.parse_args([])
+        (options) = parser.parse_args([])
 
         # Pass along cli options
         options.verbosity = 5
-        options.connection = self.options.get('connection')
-        options.remote_user = self.options.get('user')
-        options.become = self.options.get('become')
-        options.become_method = self.options.get('become_method')
-        options.become_user = self.options.get('become_user')
-        options.module_path = self.options.get('module_path')
+        options.connection = self.options.get("connection")
+        options.remote_user = self.options.get("user")
+        options.become = self.options.get("become")
+        options.become_method = self.options.get("become_method")
+        options.become_user = self.options.get("become_user")
+        options.module_path = self.options.get("module_path")
 
         # Initialize callback to capture module JSON responses
         cb = ResultAccumulator()
 
-        kwargs = dict(
-            inventory=self.options['inventory_manager'],
-            variable_manager=self.options['variable_manager'],
-            loader=self.options['loader'],
-            options=options,
-            stdout_callback=cb,
-            passwords=dict(conn_pass=None, become_pass=None),
-        )
+        kwargs = {
+            "inventory": self.options["inventory_manager"],
+            "variable_manager": self.options["variable_manager"],
+            "loader": self.options["loader"],
+            "options": options,
+            "stdout_callback": cb,
+            "passwords": {"conn_pass": None, "become_pass": None},
+        }
 
         # create a pseudo-play to execute the specified module via a single task
-        play_ds = dict(
-            name="pytest-ansible",
-            hosts=self.options['host_pattern'],
-            gather_facts='no',
-            tasks=[
-                dict(
-                    action=dict(
-                        module=self.options['module_name'], args=complex_args
-                    ),
-                ),
-            ]
+        play_ds = {
+            "name": "pytest-ansible",
+            "hosts": self.options["host_pattern"],
+            "gather_facts": "no",
+            "tasks": [
+                {
+                    "action": {
+                        "module": self.options["module_name"],
+                        "args": complex_args,
+                    }
+                }
+            ],
+        }
+
+        play = Play().load(
+            play_ds,
+            variable_manager=self.options["variable_manager"],
+            loader=self.options["loader"],
         )
-        play = Play().load(play_ds, variable_manager=self.options['variable_manager'], loader=self.options['loader'])
 
         # now create a task queue manager to execute the play
         tqm = None
         try:
             tqm = TaskQueueManager(**kwargs)
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
-
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
         if cb.unreachable:
-            raise AnsibleConnectionFailure("Host unreachable", dark=cb.unreachable, contacted=cb.contacted)
+            raise AnsibleConnectionFailure(
+                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+            )
 
         # Success!
         return AdHocResult(contacted=cb.contacted)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,171 @@
 import warnings
+
 import ansible.constants
-import ansible.utils
 import ansible.errors
+import ansible.utils
 
-from ansible.plugins.callback import CallbackBase
+from ansible.cli import CLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
-from ansible.cli import CLI
+from ansible.plugins.callback import CallbackBase
+from ansible.plugins.loader import module_loader
+
+from pytest_ansible.errors import AnsibleConnectionFailure
+from pytest_ansible.has_version import has_ansible_v24
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
-from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.has_version import (
-    has_ansible_v24,
-)
 
-if not has_ansible_v24:
 
+# pylint: disable=ungrouped-imports, wrong-import-position
+
+if not has_ansible_v24:
     raise ImportError("Only supported with ansible-2.4 and newer")
-else:
-    from ansible.plugins.loader import module_loader
+
+
+# pylint: enable=ungrouped-imports
 
 
 class ResultAccumulator(CallbackBase):
 
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Initialize object."""
-        super(ResultAccumulator, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         self.contacted[result._host.get_name()] = result._result
 
     v2_runner_on_ok = v2_runner_on_failed
 
     def v2_runner_on_unreachable(self, result):
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
-        return dict(contacted=self.contacted, unreachable=self.unreachable)
+        return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
 class ModuleDispatcherV24(ModuleDispatcherV2):
 
     """Pass."""
 
-    required_kwargs = ('inventory', 'inventory_manager', 'variable_manager', 'host_pattern', 'loader')
+    required_kwargs = (
+        "inventory",
+        "inventory_manager",
+        "variable_manager",
+        "host_pattern",
+        "loader",
+    )
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
-        if 'module_path' in self.options:
-            paths = self.options['module_path']
+        if "module_path" in self.options:
+            paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
                     module_loader.add_directory(path)
             else:
                 module_loader.add_directory(paths)
 
         return module_loader.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the result in a AdhocResult object."""
         # Assemble module argument string
         if module_args:
-            complex_args.update(dict(_raw_params=' '.join(module_args)))
+            complex_args.update({"_raw_params": " ".join(module_args)})
 
         # Assert hosts matching the provided pattern exist
-        hosts = self.options['inventory_manager'].list_hosts()
+        hosts = self.options["inventory_manager"].list_hosts()
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
-        self.options['inventory_manager'].subset(self.options.get('subset'))
-        hosts = self.options['inventory_manager'].list_hosts(self.options['host_pattern'])
+        self.options["inventory_manager"].subset(self.options.get("subset"))
+        hosts = self.options["inventory_manager"].list_hosts(
+            self.options["host_pattern"]
+        )
         if len(hosts) == 0 and not no_hosts:
-            raise ansible.errors.AnsibleError("Specified hosts and/or --limit does not match any hosts")
+            raise ansible.errors.AnsibleError(
+                "Specified hosts and/or --limit does not match any hosts"
+            )
 
         parser = CLI.base_parser(
             runas_opts=True,
             inventory_opts=True,
             async_opts=True,
             output_opts=True,
             connect_opts=True,
             check_opts=True,
             runtask_opts=True,
             vault_opts=True,
             fork_opts=True,
             module_opts=True,
         )
-        (options, args) = parser.parse_args([])
+        (options) = parser.parse_args([])
 
         # Pass along cli options
         options.verbosity = 5
-        options.connection = self.options.get('connection')
-        options.remote_user = self.options.get('user')
-        options.become = self.options.get('become')
-        options.become_method = self.options.get('become_method')
-        options.become_user = self.options.get('become_user')
-        options.module_path = self.options.get('module_path')
+        options.connection = self.options.get("connection")
+        options.remote_user = self.options.get("user")
+        options.become = self.options.get("become")
+        options.become_method = self.options.get("become_method")
+        options.become_user = self.options.get("become_user")
+        options.module_path = self.options.get("module_path")
 
         # Initialize callback to capture module JSON responses
         cb = ResultAccumulator()
 
-        kwargs = dict(
-            inventory=self.options['inventory_manager'],
-            variable_manager=self.options['variable_manager'],
-            loader=self.options['loader'],
-            options=options,
-            stdout_callback=cb,
-            passwords=dict(conn_pass=None, become_pass=None),
-        )
+        kwargs = {
+            "inventory": self.options["inventory_manager"],
+            "variable_manager": self.options["variable_manager"],
+            "loader": self.options["loader"],
+            "options": options,
+            "stdout_callback": cb,
+            "passwords": {"conn_pass": None, "become_pass": None},
+        }
 
         # create a pseudo-play to execute the specified module via a single task
-        play_ds = dict(
-            name="pytest-ansible",
-            hosts=self.options['host_pattern'],
-            gather_facts='no',
-            tasks=[
-                dict(
-                    action=dict(
-                        module=self.options['module_name'], args=complex_args
-                    ),
-                ),
-            ]
+        play_ds = {
+            "name": "pytest-ansible",
+            "hosts": self.options["host_pattern"],
+            "gather_facts": "no",
+            "tasks": [
+                {
+                    "action": {
+                        "module": self.options["module_name"],
+                        "args": complex_args,
+                    },
+                },
+            ],
+        }
+
+        play = Play().load(
+            play_ds,
+            variable_manager=self.options["variable_manager"],
+            loader=self.options["loader"],
         )
-        play = Play().load(play_ds, variable_manager=self.options['variable_manager'], loader=self.options['loader'])
 
         # now create a task queue manager to execute the play
         tqm = None
         try:
             tqm = TaskQueueManager(**kwargs)
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
         if cb.unreachable:
-            raise AnsibleConnectionFailure("Host unreachable", dark=cb.unreachable, contacted=cb.contacted)
+            raise AnsibleConnectionFailure(
+                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+            )
 
         # Success!
         return AdHocResult(contacted=cb.contacted)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,187 @@
 import sys
-
 import warnings
+
 import ansible.constants
-import ansible.utils
 import ansible.errors
+import ansible.utils
 
-from ansible.plugins.callback import CallbackBase
+from ansible.cli.adhoc import AdHocCLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
-from ansible.cli.adhoc import AdHocCLI
-from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
-from pytest_ansible.results import AdHocResult
+from ansible.plugins.callback import CallbackBase
+from ansible.plugins.loader import module_loader
+
 from pytest_ansible.errors import AnsibleConnectionFailure
 from pytest_ansible.has_version import has_ansible_v28
+from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
+from pytest_ansible.results import AdHocResult
 
 
+# pylint: disable=ungrouped-imports, wrong-import-position
 if not has_ansible_v28:
     raise ImportError("Only supported with ansible-2.8 and newer")
-else:
-    from ansible.plugins.loader import module_loader
 
 
+# pylint: enable=ungrouped-imports
 
-class ResultAccumulator(CallbackBase):
 
+class ResultAccumulator(CallbackBase):
     """Fixme."""
 
     def __init__(self, *args, **kwargs):
         """Initialize object."""
-        super(ResultAccumulator, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
-        result2 = dict(failed=True)
+        result2 = {"failed": True}
         result2.update(result._result)
         self.contacted[result._host.get_name()] = result2
 
     def v2_runner_on_ok(self, result):
         self.contacted[result._host.get_name()] = result._result
 
     def v2_runner_on_unreachable(self, result):
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
-        return dict(contacted=self.contacted, unreachable=self.unreachable)
+        return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
 class ModuleDispatcherV28(ModuleDispatcherV2):
-
     """Pass."""
 
-    required_kwargs = ('inventory', 'inventory_manager', 'variable_manager', 'host_pattern', 'loader')
+    required_kwargs = (
+        "inventory",
+        "inventory_manager",
+        "variable_manager",
+        "host_pattern",
+        "loader",
+    )
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
-        if 'module_path' in self.options:
-            paths = self.options['module_path']
+        if "module_path" in self.options:
+            paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
                     module_loader.add_directory(path)
             else:
                 module_loader.add_directory(paths)
 
         return module_loader.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the result in a AdhocResult object."""
         # Assemble module argument string
         if module_args:
-            complex_args.update(dict(_raw_params=' '.join(module_args)))
+            complex_args.update({"_raw_params": " ".join(module_args)})
 
         # Assert hosts matching the provided pattern exist
-        hosts = self.options['inventory_manager'].list_hosts()
+        hosts = self.options["inventory_manager"].list_hosts()
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
-        self.options['inventory_manager'].subset(self.options.get('subset'))
-        hosts = self.options['inventory_manager'].list_hosts(self.options['host_pattern'])
+        self.options["inventory_manager"].subset(self.options.get("subset"))
+        hosts = self.options["inventory_manager"].list_hosts(
+            self.options["host_pattern"]
+        )
         if len(hosts) == 0 and not no_hosts:
-            raise ansible.errors.AnsibleError("Specified hosts and/or --limit does not match any hosts")
+            raise ansible.errors.AnsibleError(
+                "Specified hosts and/or --limit does not match any hosts"
+            )
 
         # Pass along cli options
-        args = ['pytest-ansible']
+        args = ["pytest-ansible"]
         verbosity = None
-        for verbosity_syntax in ('-v', '-vv', '-vvv', '-vvvv', '-vvvvv'):
+        for verbosity_syntax in ("-v", "-vv", "-vvv", "-vvvv", "-vvvvv"):
             if verbosity_syntax in sys.argv:
                 verbosity = verbosity_syntax
                 break
         if verbosity is not None:
             args.append(verbosity_syntax)
-        args.extend([self.options['host_pattern']])
-        for argument in ('connection', 'user', 'become', 'become_method', 'become_user', 'module_path'):
+        args.extend([self.options["host_pattern"]])
+        for argument in (
+            "connection",
+            "user",
+            "become",
+            "become_method",
+            "become_user",
+            "module_path",
+        ):
             arg_value = self.options.get(argument)
-            argument = argument.replace('_', '-')
+            argument = argument.replace("_", "-")
 
             if arg_value in (None, False):
                 continue
 
             if arg_value is True:
-                args.append('--{0}'.format(argument))
+                args.append(f"--{argument}")
             else:
-                args.append('--{0}={1}'.format(argument, arg_value))
+                args.append(f"--{argument}={arg_value}")
 
         # Use Ansible's own adhoc cli to parse the fake command line we created and then save it
         # into Ansible's global context
         adhoc = AdHocCLI(args)
         adhoc.parse()
 
         # And now we'll never speak of this again
         del adhoc
 
         # Initialize callback to capture module JSON responses
         cb = ResultAccumulator()
 
-        kwargs = dict(
-            inventory=self.options['inventory_manager'],
-            variable_manager=self.options['variable_manager'],
-            loader=self.options['loader'],
-            stdout_callback=cb,
-            passwords=dict(conn_pass=None, become_pass=None),
-        )
+        kwargs = {
+            "inventory": self.options["inventory_manager"],
+            "variable_manager": self.options["variable_manager"],
+            "loader": self.options["loader"],
+            "stdout_callback": cb,
+            "passwords": {"conn_pass": None, "become_pass": None},
+        }
 
         # create a pseudo-play to execute the specified module via a single task
-        play_ds = dict(
-            name="pytest-ansible",
-            hosts=self.options['host_pattern'],
-            become=self.options.get('become'),
-            become_user=self.options.get('become_user'),
-            gather_facts='no',
-            tasks=[
-                dict(
-                    action=dict(
-                        module=self.options['module_name'], args=complex_args
-                    ),
-                ),
-            ]
+        play_ds = {
+            "name": "pytest-ansible",
+            "hosts": self.options["host_pattern"],
+            "become": self.options.get("become"),
+            "become_user": self.options.get("become_user"),
+            "gather_facts": "no",
+            "tasks": [
+                {
+                    "action": {
+                        "module": self.options["module_name"],
+                        "args": complex_args,
+                    },
+                },
+            ],
+        }
+
+        play = Play().load(
+            play_ds,
+            variable_manager=self.options["variable_manager"],
+            loader=self.options["loader"],
         )
-        play = Play().load(play_ds, variable_manager=self.options['variable_manager'], loader=self.options['loader'])
 
         # now create a task queue manager to execute the play
         tqm = None
         try:
             tqm = TaskQueueManager(**kwargs)
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
-
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
         if cb.unreachable:
-            raise AnsibleConnectionFailure("Host unreachable", dark=cb.unreachable, contacted=cb.contacted)
+            raise AnsibleConnectionFailure(
+                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+            )
 
         # Success!
         return AdHocResult(contacted=cb.contacted)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/plugin.py` & `pytest-ansible-3.0.0/src/pytest_ansible/plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,222 +1,287 @@
 """PyTest Ansible Plugin."""
 
-import pytest
 import ansible
 import ansible.constants
-import ansible.utils
 import ansible.errors
+import ansible.utils
+import pytest
 
-try:
-    from ansible.plugins.loader import become_loader
-except ImportError:
-    become_loader = None
+from ansible.plugins.loader import become_loader
 
-from pytest_ansible.fixtures import (ansible_adhoc, ansible_module, ansible_facts, localhost)
+from pytest_ansible.fixtures import ansible_adhoc
+from pytest_ansible.fixtures import ansible_facts
+from pytest_ansible.fixtures import ansible_module
+from pytest_ansible.fixtures import localhost
 from pytest_ansible.host_manager import get_host_manager
 
 
 # Silence linters for imported fixtures
+# pylint: disable=pointless-statement
 (ansible_adhoc, ansible_module, ansible_facts, localhost)
 
 
 def become_methods():
     """Return string list of become methods available to ansible."""
     if become_loader:
         return [method.name for method in become_loader.all()]
-    else:
-        return ansible.constants.BECOME_METHODS
+    return ansible.constants.BECOME_METHODS
 
 
 def pytest_addoption(parser):
     """Add options to control ansible."""
 
-    group = parser.getgroup('pytest-ansible')
-    group.addoption('--inventory', '--ansible-inventory',
-                    action='store',
-                    dest='ansible_inventory',
-                    default=ansible.constants.DEFAULT_HOST_LIST,
-                    metavar='ANSIBLE_INVENTORY',
-                    help='ansible inventory file URI (default: %(default)s)')
-    group.addoption('--host-pattern', '--ansible-host-pattern',
-                    action='store',
-                    dest='ansible_host_pattern',
-                    default=None,
-                    metavar='ANSIBLE_HOST_PATTERN',
-                    help='ansible host pattern (default: %(default)s)')
-    group.addoption('--limit', '--ansible-limit',
-                    action='store',
-                    dest='ansible_subset',
-                    default=ansible.constants.DEFAULT_SUBSET,
-                    metavar='ANSIBLE_SUBSET',
-                    help='further limit selected hosts to an additional pattern')
-    group.addoption('--connection', '--ansible-connection',
-                    action='store',
-                    dest='ansible_connection',
-                    default=ansible.constants.DEFAULT_TRANSPORT,
-                    help="connection type to use (default: %(default)s)")
-    group.addoption('--user', '--ansible-user',
-                    action='store',
-                    dest='ansible_user',
-                    default=ansible.constants.DEFAULT_REMOTE_USER,
-                    help='connect as this user (default: %(default)s)')
-    group.addoption('--check', '--ansible-check',
-                    action='store_true',
-                    dest='ansible_check',
-                    default=False,
-                    help='don\'t make any changes; instead, try to predict some of the changes that may occur')
-    group.addoption('--module-path', '--ansible-module-path',
-                    action='store',
-                    dest='ansible_module_path',
-                    default=ansible.constants.DEFAULT_MODULE_PATH,
-                    help='specify path(s) to module library (default: %(default)s)')
+    group = parser.getgroup("pytest-ansible")
+    group.addoption(
+        "--inventory",
+        "--ansible-inventory",
+        action="store",
+        dest="ansible_inventory",
+        default=ansible.constants.DEFAULT_HOST_LIST,
+        metavar="ANSIBLE_INVENTORY",
+        help="ansible inventory file URI (default: %(default)s)",
+    )
+    group.addoption(
+        "--extra-inventory",
+        "--ansible-extra-inventory",
+        action="store",
+        dest="ansible_extra_inventory",
+        default=None,
+        metavar="ANSIBLE_EXTRA_INVENTORY",
+        help="ansible extra inventory file URI (default: %(default)s)",
+    )
+    group.addoption(
+        "--host-pattern",
+        "--ansible-host-pattern",
+        action="store",
+        dest="ansible_host_pattern",
+        default=None,
+        metavar="ANSIBLE_HOST_PATTERN",
+        help="ansible host pattern (default: %(default)s)",
+    )
+    group.addoption(
+        "--limit",
+        "--ansible-limit",
+        action="store",
+        dest="ansible_subset",
+        default=ansible.constants.DEFAULT_SUBSET,
+        metavar="ANSIBLE_SUBSET",
+        help="further limit selected hosts to an additional pattern",
+    )
+    group.addoption(
+        "--connection",
+        "--ansible-connection",
+        action="store",
+        dest="ansible_connection",
+        default=ansible.constants.DEFAULT_TRANSPORT,
+        help="connection type to use (default: %(default)s)",
+    )
+    group.addoption(
+        "--user",
+        "--ansible-user",
+        action="store",
+        dest="ansible_user",
+        default=ansible.constants.DEFAULT_REMOTE_USER,
+        help="connect as this user (default: %(default)s)",
+    )
+    group.addoption(
+        "--check",
+        "--ansible-check",
+        action="store_true",
+        dest="ansible_check",
+        default=False,
+        help="don't make any changes; instead, try to predict some of the changes that may occur",
+    )
+    group.addoption(
+        "--module-path",
+        "--ansible-module-path",
+        action="store",
+        dest="ansible_module_path",
+        default=ansible.constants.DEFAULT_MODULE_PATH,
+        help="specify path(s) to module library (default: %(default)s)",
+    )
 
     # become privilege escalation
-    group.addoption('--become', '--ansible-become',
-                    action='store_true',
-                    dest='ansible_become',
-                    default=ansible.constants.DEFAULT_BECOME,
-                    help='run operations with become, nopasswd implied (default: %(default)s)')
-    group.addoption('--become-method', '--ansible-become-method',
-                    action='store',
-                    dest='ansible_become_method',
-                    default=ansible.constants.DEFAULT_BECOME_METHOD,
-                    help="privilege escalation method to use (default: %%(default)s), valid choices: [ %s ]" %
-                    (' | '.join(become_methods())))
-    group.addoption('--become-user', '--ansible-become-user',
-                    action='store',
-                    dest='ansible_become_user',
-                    default=ansible.constants.DEFAULT_BECOME_USER,
-                    help='run operations as this user (default: %(default)s)')
-    group.addoption('--ask-become-pass', '--ansible-ask-become-pass',
-                    action='store',
-                    dest='ansible_ask_become_pass',
-                    default=ansible.constants.DEFAULT_BECOME_ASK_PASS,
-                    help='ask for privilege escalation password (default: %(default)s)')
+    group.addoption(
+        "--become",
+        "--ansible-become",
+        action="store_true",
+        dest="ansible_become",
+        default=ansible.constants.DEFAULT_BECOME,
+        help="run operations with become, nopasswd implied (default: %(default)s)",
+    )
+    group.addoption(
+        "--become-method",
+        "--ansible-become-method",
+        action="store",
+        dest="ansible_become_method",
+        default=ansible.constants.DEFAULT_BECOME_METHOD,
+        help=f"privilege escalation method to use (default: %(default)s), valid choices: [ {' | '.join(become_methods())} ]",
+    )
+
+    group.addoption(
+        "--become-user",
+        "--ansible-become-user",
+        action="store",
+        dest="ansible_become_user",
+        default=ansible.constants.DEFAULT_BECOME_USER,
+        help="run operations as this user (default: %(default)s)",
+    )
+    group.addoption(
+        "--ask-become-pass",
+        "--ansible-ask-become-pass",
+        action="store",
+        dest="ansible_ask_become_pass",
+        default=ansible.constants.DEFAULT_BECOME_ASK_PASS,
+        help="ask for privilege escalation password (default: %(default)s)",
+    )
 
     # Add github marker to --help
     parser.addini("ansible", "Ansible integration", "args")
 
 
 def pytest_configure(config):
     """Validate --ansible-* parameters."""
 
     config.addinivalue_line("markers", "ansible(**kwargs): Ansible integration")
 
     # Enable connection debugging
     if config.option.verbose > 0:
-        if hasattr(ansible.utils, 'VERBOSITY'):
+        if hasattr(ansible.utils, "VERBOSITY"):
             ansible.utils.VERBOSITY = int(config.option.verbose)
         else:
             from ansible.utils.display import Display
+
             display = Display()
             display.verbosity = int(config.option.verbose)
 
     assert config.pluginmanager.register(PyTestAnsiblePlugin(config), "ansible")
 
 
 def pytest_generate_tests(metafunc):
     """Generate tests when specific `ansible_*` fixtures are used by tests."""
 
-    if 'ansible_host' in metafunc.fixturenames:
+    if "ansible_host" in metafunc.fixturenames:
         # assert required --ansible-* parameters were used
         PyTestAnsiblePlugin.assert_required_ansible_parameters(metafunc.config)
         try:
             plugin = metafunc.config.pluginmanager.getplugin("ansible")
-            hosts = plugin.initialize(config=plugin.config, pattern=metafunc.config.getoption('ansible_host_pattern'))
+            hosts = plugin.initialize(
+                config=plugin.config,
+                pattern=metafunc.config.getoption("ansible_host_pattern"),
+            )
         except ansible.errors.AnsibleError as e:
             raise pytest.UsageError(e)
         # Return the host name as a string
         # metafunc.parametrize("ansible_host", hosts.keys())
         # Return a HostManager instance where pattern=host (e.g. ansible_host.all.shell('date'))
         # metafunc.parametrize("ansible_host", iter(plugin.initialize(config=plugin.config, pattern=h) for h in
         #                                           hosts.keys()))
         # Return a ModuleDispatcher instance representing `host` (e.g. ansible_host.shell('date'))
         metafunc.parametrize("ansible_host", iter(hosts[h] for h in hosts.keys()))
 
-    if 'ansible_group' in metafunc.fixturenames:
+    if "ansible_group" in metafunc.fixturenames:
         # assert required --ansible-* parameters were used
         PyTestAnsiblePlugin.assert_required_ansible_parameters(metafunc.config)
         try:
             plugin = metafunc.config.pluginmanager.getplugin("ansible")
-            hosts = plugin.initialize(config=plugin.config, pattern=metafunc.config.getoption('ansible_host_pattern'))
+            hosts = plugin.initialize(
+                config=plugin.config,
+                pattern=metafunc.config.getoption("ansible_host_pattern"),
+            )
         except ansible.errors.AnsibleError as e:
             raise pytest.UsageError(e)
         # FIXME: Eeew, this shouldn't be interfacing with `hosts.options`
-        groups = hosts.options['inventory_manager'].list_groups()
+        groups = hosts.options["inventory_manager"].list_groups()
+        extra_groups = hosts.get_extra_inventory_groups()
         # Return the group name as a string
         # metafunc.parametrize("ansible_group", groups)
         # Return a ModuleDispatcher instance representing the group (e.g. ansible_group.shell('date'))
         metafunc.parametrize("ansible_group", iter(hosts[g] for g in groups))
+        metafunc.parametrize("ansible_group", iter(hosts[g] for g in extra_groups))
 
 
 class PyTestAnsiblePlugin:
 
     """Ansible PyTest Plugin Class."""
 
     def __init__(self, config):
         """Initialize plugin."""
         self.config = config
 
     def pytest_report_header(self, config, startdir):
         """Return the version of ansible."""
-        return 'ansible: %s' % ansible.__version__
+        return f"ansible: {ansible.__version__}"
 
     def pytest_collection_modifyitems(self, session, config, items):
         """Validate --ansible-* parameters."""
 
         uses_ansible_fixtures = False
         for item in items:
-            if not hasattr(item, 'fixturenames'):
+            if not hasattr(item, "fixturenames"):
                 continue
-            if any([fixture.startswith('ansible_') for fixture in item.fixturenames]):
+            if any(fixture.startswith("ansible_") for fixture in item.fixturenames):
                 # TODO - ignore if they are using a marker
                 # marker = item.get_marker('ansible')
                 # if marker and 'inventory' in marker.kwargs:
                 uses_ansible_fixtures = True
                 break
 
         if uses_ansible_fixtures:
             # assert required --ansible-* parameters were used
             self.assert_required_ansible_parameters(config)
 
     def _load_ansible_config(self, config):
         """Load ansible configuration from command-line."""
-        option_names = ['ansible_inventory', 'ansible_host_pattern', 'ansible_connection', 'ansible_user',
-                        'ansible_module_path', 'ansible_become', 'ansible_become_method', 'ansible_become_user',
-                        'ansible_ask_become_pass', 'ansible_subset']
+        option_names = [
+            "ansible_inventory",
+            "ansible_extra_inventory",
+            "ansible_host_pattern",
+            "ansible_connection",
+            "ansible_user",
+            "ansible_module_path",
+            "ansible_become",
+            "ansible_become_method",
+            "ansible_become_user",
+            "ansible_ask_become_pass",
+            "ansible_subset",
+        ]
 
-        kwargs = dict()
+        kwargs = {}
 
         # Load command-line supplied values
         for key in option_names:
             short_key = key[8:]
             kwargs[short_key] = config.getoption(key)
 
         # normalize ansible.ansible_become options
-        kwargs['become'] = kwargs.get('become') or ansible.constants.DEFAULT_BECOME
-        kwargs['become_user'] = kwargs.get('become_user') or ansible.constants.DEFAULT_BECOME_USER
-        kwargs['ask_become_pass'] = kwargs.get('ask_become_pass') or ansible.constants.DEFAULT_BECOME_ASK_PASS
+        kwargs["become"] = kwargs.get("become") or ansible.constants.DEFAULT_BECOME
+        kwargs["become_user"] = (
+            kwargs.get("become_user") or ansible.constants.DEFAULT_BECOME_USER
+        )
+        kwargs["ask_become_pass"] = (
+            kwargs.get("ask_become_pass") or ansible.constants.DEFAULT_BECOME_ASK_PASS
+        )
 
         return kwargs
 
     def _load_request_config(self, request):
         """Load ansible configuration from decorator kwargs."""
-        kwargs = dict()
+        kwargs = {}
 
         # Override options from @pytest.mark.ansible
-        marker = request.node.get_closest_marker('ansible')
+        marker = request.node.get_closest_marker("ansible")
         if marker:
             kwargs = marker.kwargs
 
         return kwargs
 
     def initialize(self, config=None, request=None, **kwargs):
         """Return an initialized Ansible Host Manager instance."""
-        ansible_cfg = dict()
+        ansible_cfg = {}
         # merge command-line configuration options
         if config is not None:
             ansible_cfg.update(self._load_ansible_config(config))
         # merge pytest request configuration options
         if request is not None:
             ansible_cfg.update(self._load_request_config(request))
         # merge in provided kwargs
@@ -225,21 +290,25 @@
 
     @staticmethod
     def assert_required_ansible_parameters(config):
         """Assert whether the required --ansible-* parameters were provided."""
         errors = []
 
         # Verify --ansible-host-pattern was provided
-        ansible_hostname = config.getoption('ansible_host_pattern')
-        if ansible_hostname is None or ansible_hostname == '':
-            errors.append("Missing required parameter --ansible-host-pattern/--host-pattern")
+        ansible_hostname = config.getoption("ansible_host_pattern")
+        if ansible_hostname is None or ansible_hostname == "":
+            errors.append(
+                "Missing required parameter --ansible-host-pattern/--host-pattern"
+            )
 
         # NOTE: I don't think this will ever catch issues since ansible_inventory
         # defaults to '/etc/ansible/hosts'
         # Verify --ansible-inventory was provided
-        ansible_inventory = config.getoption('ansible_inventory')
+        ansible_inventory = config.getoption("ansible_inventory")
         if ansible_inventory is None or ansible_inventory == "":
-            errors.append("Unable to find an inventory file, specify one with the --ansible-inventory/--inventory "
-                          "parameter.")
+            errors.append(
+                "Unable to find an inventory file, specify one with the --ansible-inventory/--inventory "
+                "parameter."
+            )
 
         if errors:
             raise pytest.UsageError(*errors)
```

### Comparing `pytest-ansible-2.2.4/pytest_ansible/results.py` & `pytest-ansible-3.0.0/src/pytest_ansible/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Fixme."""
 
-import ansible.errors  # NOQA
-
 
 class ModuleResult(dict):
 
     """Fixme."""
 
     def _check_key(self, key):
         # if 'results' in self:
@@ -15,61 +13,61 @@
         #             flag |= res.get(key, False)
         #     return flag
         # else:
         return self.get(key, False)
 
     @property
     def is_ok(self):
-        return not (self.is_changed or self.is_unreachable or self.is_skipped or self.is_failed)
+        return not (
+            self.is_changed or self.is_unreachable or self.is_skipped or self.is_failed
+        )
 
     @property
     def is_changed(self):
-        return self._check_key('changed')
+        return self._check_key("changed")
 
     @property
     def is_unreachable(self):
-        return self._check_key('unreachable')
+        return self._check_key("unreachable")
 
     @property
     def is_skipped(self):
-        return self._check_key('skipped')
+        return self._check_key("skipped")
 
     @property
     def is_failed(self):
-        return self._check_key('failed') or self.get('rc', 0) != 0
+        return self._check_key("failed") or self.get("rc", 0) != 0
 
     @property
     def is_successful(self):
         return not (self.is_failed or self.is_unreachable)
 
 
-class AdHocResult(object):
+class AdHocResult:
 
     """Fixme."""
 
     def __init__(self, **kwargs):
         """Fixme."""
-        required_kwargs = ('contacted',)
+        required_kwargs = ("contacted",)
         for kwarg in required_kwargs:
-            assert kwarg in kwargs, "Missing required keyword argument '%s'" % kwarg
+            assert kwarg in kwargs, f"Missing required keyword argument '{kwarg}'"
             setattr(self, kwarg, kwargs.get(kwarg))
 
     def __getitem__(self, item):
         """Return a ModuleResult instance matching the provided `item`."""
         if item in self.contacted:
             return ModuleResult(**self.contacted[item])
-        else:
-            raise KeyError(item)
+        raise KeyError(item)
 
     def __getattr__(self, attr):
         """Return a ModuleResult instance matching the provided `attr`."""
         if attr in self.contacted:
             return ModuleResult(**self.contacted[attr])
-        else:
-            raise AttributeError("type AdHocResult has no attribute '%s'" % attr)
+        raise AttributeError(f"type AdHocResult has no attribute '{attr}'")
 
     def __len__(self):
         """Return the number of contacted hosts."""
         return len(self.contacted)
 
     def __contains__(self, item):
         """Return whether the provided `item` was contacted."""
```

