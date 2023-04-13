# Comparing `tmp/python-project-structure-0.8.9b0.tar.gz` & `tmp/python-project-structure-0.8.9b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.9b0.tar", last modified: Wed Apr 12 16:22:09 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.9b7.tar", last modified: Wed Apr 12 21:15:07 2023, max compression
```

## Comparing `python-project-structure-0.8.9b0.tar` & `python-project-structure-0.8.9b7.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4519 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58045 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5312 2023-04-12 16:21:49.000000 python-project-structure-0.8.9b0/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/gitlab-runner/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/gitlab-runner/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/gitlab-runner/config/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-12 16:21:50.000000 python-project-structure-0.8.9b0/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.557545 python-project-structure-0.8.9b7/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1461 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1461 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4519 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58199 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      152 2023-04-12 21:06:40.000000 python-project-structure-0.8.9b7/NEWS-VERSION.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     6456 2023-04-12 21:06:42.000000 python-project-structure-0.8.9b7/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 21:15:07.557545 python-project-structure-0.8.9b7/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/gitlab-runner/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/gitlab-runner/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/gitlab-runner/config/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2658 2023-04-12 21:06:43.000000 python-project-structure-0.8.9b7/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 21:06:57.000000 python-project-structure-0.8.9b7/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-12 21:15:07.557545 python-project-structure-0.8.9b7/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1846 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.553544 python-project-structure-0.8.9b7/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 21:15:07.557545 python-project-structure-0.8.9b7/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-12 21:15:07.000000 python-project-structure-0.8.9b7/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-12 21:05:26.000000 python-project-structure-0.8.9b7/tox.ini
```

### Comparing `python-project-structure-0.8.9b0/.dir-locals.el.in` & `python-project-structure-0.8.9b7/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/.dockerignore` & `python-project-structure-0.8.9b7/.dockerignore`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,13 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
 /README.md
-/NEWS-release.rst
 
 # Explicit ignores for the Docker build context.
 .local
 **/.local
 .gnupg
 **/.gnupg
```

### Comparing `python-project-structure-0.8.9b0/.env.in` & `python-project-structure-0.8.9b7/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/.github/workflows/build-test.yml` & `python-project-structure-0.8.9b7/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/.gitignore` & `python-project-structure-0.8.9b7/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,13 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
 /README.md
-/NEWS-release.rst
 
 # Explicit ignores for the Docker build context.
 .local
 **/.local
 .gnupg
 **/.gnupg
```

### Comparing `python-project-structure-0.8.9b0/.gitlab-ci.yml` & `python-project-structure-0.8.9b7/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -43,24 +43,27 @@
   GH_TOKEN: "$PROJECT_GITHUB_PAT"
   # Uncomment to get more debugging output:
   # DEBUG: "true"
 
 stages:
   - "build-test"
   - "release"
-  - "release-tag"
+  - "release-bump"
   - "scheduled"
 
 build-test:
   stage: "build-test"
   rules:
     - if: >-
-        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
+        (
+          $CI_COMMIT_BRANCH !~ /^(develop|master)$/
+          || $CI_COMMIT_MESSAGE =~ /(?ims).*\[ci release\].*/
+        )
+        && ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
         && $CI_PIPELINE_SOURCE != "schedule"
-        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   interruptible: true
   parallel:
     matrix:
       - PYTHON_MINORS:
           - "3.11"
           - "3.10"
           - "3.9"
@@ -98,43 +101,41 @@
   # Avoid unnecessary artifact downloads:
   # https://docs.gitlab.com/ee/ci/yaml/#dependencies
   dependencies: []
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
-        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
+        (
+          $CI_COMMIT_BRANCH =~ /^(develop|master)$/
+          && $CI_COMMIT_MESSAGE =~ /(?ims).*\[ci release\].*/
+        )
         && $CI_PROJECT_NAMESPACE == "rpatterson"
-        && $CI_COMMIT_BRANCH != null
-        && $CI_COMMIT_BRANCH =~ /^(develop|master)$/
         && $CI_PIPELINE_SOURCE != "schedule"
-        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   script:
     - >-
       entrypoint make -e release-python test-clean
   artifacts:
     paths:
-      - "./NEWS-release.rst"
       - "./dist/python?project?structure-*"
 
-
-release-tag:
-  stage: "release-tag"
+release-bump:
+  stage: "release-bump"
   needs: []
   dependencies: []
+  variables:
+    DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
-        $CI_COMMIT_TAG != null && $CI_COMMIT_TAG =~ /^v*\.*\.*$/
-  inherit:
-    default: false
-  # Version tags are only created and pushed if the pipeline that generated the
-  # release succeeded:
+        $CI_COMMIT_MESSAGE !~ /(?ims).*\[ci release\].*/
+        && $CI_COMMIT_BRANCH =~ /^(develop|master)$/
+        && $CI_PIPELINE_SOURCE != "schedule"
   script:
     - >-
-      true
+      entrypoint make -e release-bump
 
 # TEMPLATE: Optionally add a scheduled pipeline with the following variables to
 # periodically upgrade all requirements and run CI:
 # - `DOCKER_BUILD_PULL=true`
 # - `SCHEDULED_TARGETS=devel-upgrade-branch`
 # - `TEMPLATE_IGNORE_EXISTING=true`
 # WARNING: Running this even just daily can easily exhaust the gitlab.org free quotas.
```

### Comparing `python-project-structure-0.8.9b0/.pre-commit-config.yaml` & `python-project-structure-0.8.9b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/.prospector.yaml` & `python-project-structure-0.8.9b7/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/CONTRIBUTING.rst` & `python-project-structure-0.8.9b7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/Dockerfile` & `python-project-structure-0.8.9b7/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/Dockerfile.devel` & `python-project-structure-0.8.9b7/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/LICENSE` & `python-project-structure-0.8.9b7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/Makefile` & `python-project-structure-0.8.9b7/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -423,28 +423,28 @@
 
 .PHONY: $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 ### Print the list of image tags for the current registry and variant.
 $(DOCKER_REGISTRIES:%=build-docker-tags-%): \
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/tox/build/build.log
 	docker_image=$(DOCKER_IMAGE_$(@:build-docker-tags-%=%))
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
+ifeq ($(VCS_BRANCH),master)
+# Only update tags end users may depend on to be stable from the `master` branch
 	VERSION=$$(./.tox/build/bin/cz version --project)
 	major_version=$$(echo $${VERSION} | sed -nE 's|([0-9]+).*|\1|p')
 	minor_version=$$(
 	    echo $${VERSION} | sed -nE 's|([0-9]+\.[0-9]+).*|\1|p'
 	)
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
-ifeq ($(VCS_BRANCH),master)
-# Only update tags end users may depend on to be stable from the `master` branch
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${major_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)
 endif
 # This variant is the default used for tags such as `latest`
-ifeq ($(PYTHON_ENV),$(PYTHON_LATEST_ENV))
+ifeq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(DOCKER_BRANCH_TAG)
 ifeq ($(VCS_BRANCH),master)
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${major_version}
 ifeq ($(DOCKER_VARIANT),)
 	echo $${docker_image}:latest
 else
@@ -613,72 +613,34 @@
 ### Publish installable Python packages and container images as required by commits.
 release: release-python release-docker
 
 .PHONY: release-python
 ### Publish installable Python packages to PyPI.
 release-python: ./var/log/tox/build/build.log $(VCS_RELEASE_FETCH_TARGETS) \
 		~/.pypirc ./.env build-docker-volumes-$(PYTHON_ENV)
-ifeq ($(VCS_BRANCH),master)
-	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
-	    ./.tox/build/bin/cz version --project
-	)
-	then
-# There's no pre-release for which to publish a final release:
-	    exit
-	fi
-else
-# Only release if required by conventional commits:
-	exit_code=0
-	./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
-	if (( $$exit_code == 3 || $$exit_code == 21 ))
-	then
-# No commits require a release:
-	    exit
-	elif (( $$exit_code != 0 ))
-	then
-	    exit $$exit_code
-	fi
-endif
 # Only release from the `master` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
-	$(MAKE) -e release-bump build-pkgs
+	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
 	./.tox/build/bin/twine check ./dist/python?project?structure-*
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
-ifeq ($(VCS_BRANCH),master)
-# Merge the bumped version back into `develop`:
-	bump_rev="$$(git rev-parse HEAD)"
-	git checkout --track "$(VCS_COMPARE_REMOTE)/develop" --
-	git merge --ff --gpg-sign \
-	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
-	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
-	git checkout "$${bump_rev}" --
-endif
-ifneq ($(GITHUB_ACTIONS),true)
-ifneq ($(PROJECT_GITHUB_PAT),)
-# Ensure the tag is available for creating the GitHub release below but push *before* to
-# GitLab to avoid a race with repository mirrorying:
-	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
-endif
-endif
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
 	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
 	    ./dist/python?project?structure-*
 	export VERSION=$$(./.tox/build/bin/cz version --project)
 # Create a GitLab release
 	./.tox/build/bin/twine upload -s -r "gitlab" \
 	    ./dist/python?project?structure-*
-	release_cli_args="--description ./NEWS-release.rst"
+	release_cli_args="--description ./NEWS-VERSION.rst"
 	release_cli_args+=" --tag-name v$${VERSION}"
 	release_cli_args+=" --assets-link {\
 	\"name\":\"PyPI\",\
 	\"url\":\"https://$(PYPI_HOSTNAME)/project/$(CI_PROJECT_NAME)/$${VERSION}/\",\
 	\"link_type\":\"package\"\
 	}"
 	release_cli_args+=" --assets-link {\
@@ -693,29 +655,29 @@
 	}"
 	docker compose pull gitlab-release-cli
 	docker compose run --rm gitlab-release-cli release-cli \
 	    --server-url "$(CI_SERVER_URL)" --project-id "$(CI_PROJECT_ID)" \
 	    create $${release_cli_args}
 # Create a GitHub release
 	gh release create "v$${VERSION}" $(GITHUB_RELEASE_ARGS) \
-	    --notes-file "./NEWS-release.rst" ./dist/python?project?structure-*
+	    --notes-file "./NEWS-VERSION.rst" ./dist/python?project?structure-*
 endif
 
 .PHONY: release-docker
 ### Publish all container images to all container registries.
 release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
 ### Publish the container images for one Python version to all container registry.
 $(PYTHON_MINORS:%=release-docker-%): $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	export PYTHON_ENV="py$(subst .,,$(@:release-docker-%=%))"
 	$(MAKE) -e -j $(DOCKER_REGISTRIES:%=release-docker-registry-%)
-ifeq ($${PYTHON_ENV},$(PYTHON_LATEST_ENV))
+ifeq ($${PYTHON_ENV},$(PYTHON_HOST_ENV))
 	$(MAKE) -e "./var/log/docker-login-DOCKER.log"
 	docker compose pull pandoc docker-pushrm
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
 endif
 
 .PHONY: $(DOCKER_REGISTRIES:%=release-docker-registry-%)
 ### Publish all container images to one container registry.
@@ -745,14 +707,35 @@
 		./.env build-docker-volumes-$(PYTHON_ENV)
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
+ifeq ($(VCS_BRANCH),master)
+	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
+	    ./.tox/build/bin/cz version --project
+	)
+	then
+# There's no pre-release for which to publish a final release:
+	    exit
+	fi
+else
+# Only release if required by conventional commits:
+	exit_code=0
+	./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
+	if (( $$exit_code == 3 || $$exit_code == 21 ))
+	then
+# No commits require a release:
+	    exit
+	elif (( $$exit_code != 0 ))
+	then
+	    exit $$exit_code
+	fi
+endif
 # Collect the versions involved in this release according to conventional commits:
 	cz_bump_args="--check-consistency --no-verify"
 ifneq ($(VCS_BRANCH),master)
 	cz_bump_args+=" --prerelease beta"
 endif
 ifeq ($(RELEASE_PUBLISH),true)
 	cz_bump_args+=" --gpg-sign"
@@ -762,33 +745,56 @@
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args} --yes --dry-run |
 	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p'
 	) || true
-	docker compose run --rm python-project-structure-devel $(TOX_EXEC_ARGS) \
-	    towncrier build --version "$${next_version}" --draft --yes \
-	        >"./NEWS-release.rst"
 # Build and stage the release notes to be commited by `$ cz bump`
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
+	    tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" -qq -- \
+	    towncrier build --version "$${next_version}" --draft --yes \
+	    >"./NEWS-VERSION.rst"
+	git add -- "./NEWS-VERSION.rst"
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
 	    $(TOX_EXEC_ARGS) towncrier build --version "$${next_version}" --yes
 # Increment the version in VCS
 	$(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
 ifneq ($(CI),true)
 # If running under CI/CD then the image will be updated in the next pipeline stage.
 # For testing locally, however, ensure the image is up-to-date for subsequent recipes.
 	$(MAKE) -e "./var/docker/$(PYTHON_ENV)/log/build-user.log"
 endif
+ifeq ($(VCS_BRANCH),master)
+# Merge the bumped version back into `develop`:
+	bump_rev="$$(git rev-parse HEAD)"
+	git checkout --track "$(VCS_COMPARE_REMOTE)/develop" --
+	git merge --ff --gpg-sign \
+	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
+ifeq ($(CI),true)
+	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
+endif
+	git checkout "$(VCS_BRANCH)" --
+endif
+ifneq ($(GITHUB_ACTIONS),true)
+ifneq ($(PROJECT_GITHUB_PAT),)
+# Ensure the tag is available for creating the GitHub release below but push *before* to
+# GitLab to avoid a race with repository mirrorying:
+	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
+endif
+endif
+ifeq ($(CI),true)
+	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
+endif
 
 
 ## Development Targets:
 #
 # Recipes used by developers to make changes to the code.
 
 .PHONY: devel-format
@@ -1220,14 +1226,15 @@
 # Ensure minimal VCS configuration, mostly useful in automation such as CI.
 ~/.gitconfig:
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
 ifeq ($(RELEASE_PUBLISH),true)
+	mkdir -pv "$(dir $(@))"
 	set +x
 ifneq ($(VCS_REMOTE_PUSH_URL),)
 	if ! git remote get-url --push --all "origin" |
 	    grep -q -F "$(VCS_REMOTE_PUSH_URL)"
 	then
 	    git remote set-url --push --add "origin" "$(VCS_REMOTE_PUSH_URL)" |
 	        tee -a "$(@)"
```

### Comparing `python-project-structure-0.8.9b0/NEWS.rst` & `python-project-structure-0.8.9b7/NEWS.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,70 @@
+python-project-structure 0.8.9b7 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b6 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b5 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b4 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b3 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b2 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.9b1 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Wed Apr 12 06:44:42 PM UTC 2023. (upgrade-requirements)
+
+
 python-project-structure 0.8.9b0 (2023-04-12)
 =============================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `python-project-structure-0.8.9b0/PKG-INFO` & `python-project-structure-0.8.9b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.9b0
+Version: 0.8.9b7
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.9b0/README.rst` & `python-project-structure-0.8.9b7/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/TODO.rst` & `python-project-structure-0.8.9b7/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/bin/cz-check-bump` & `python-project-structure-0.8.9b7/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/bin/entrypoint` & `python-project-structure-0.8.9b7/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/bin/get-base-version` & `python-project-structure-0.8.9b7/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/build-host/Dockerfile` & `python-project-structure-0.8.9b7/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/build-host/Makefile` & `python-project-structure-0.8.9b7/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/build-host/README.rst` & `python-project-structure-0.8.9b7/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/build-host/bin/entrypoint` & `python-project-structure-0.8.9b7/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/build-host/requirements-py310.txt` & `python-project-structure-0.8.9b7/build-host/requirements-py37.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+importlib-metadata==6.3.0
+    # via
+    #   pluggy
+    #   tox
+    #   virtualenv
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
@@ -30,9 +35,16 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.11
     # via -r build-host/requirements.txt.in
+typing-extensions==4.5.0
+    # via
+    #   importlib-metadata
+    #   platformdirs
+    #   tox
 virtualenv==20.21.0
     # via tox
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `python-project-structure-0.8.9b0/build-host/requirements-py311.txt` & `python-project-structure-0.8.9b7/build-host/requirements-py311.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
```

### Comparing `python-project-structure-0.8.9b0/build-host/requirements-py37.txt` & `python-project-structure-0.8.9b7/build-host/requirements-py39.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.3.0
-    # via
-    #   pluggy
-    #   tox
-    #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
@@ -35,16 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.11
     # via -r build-host/requirements.txt.in
-typing-extensions==4.5.0
-    # via
-    #   importlib-metadata
-    #   platformdirs
-    #   tox
 virtualenv==20.21.0
     # via tox
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `python-project-structure-0.8.9b0/build-host/requirements-py38.txt` & `python-project-structure-0.8.9b7/build-host/requirements-py310.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py38.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
```

### Comparing `python-project-structure-0.8.9b0/build-host/requirements-py39.txt` & `python-project-structure-0.8.9b7/build-host/requirements-py38.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py38.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
```

### Comparing `python-project-structure-0.8.9b0/docker-compose.override.yml` & `python-project-structure-0.8.9b7/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/docker-compose.yml` & `python-project-structure-0.8.9b7/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/gitlab-runner/config/config.toml.in` & `python-project-structure-0.8.9b7/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/pyproject.toml` & `python-project-structure-0.8.9b7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.9b0"
+version = "0.8.9b7"
 tag_format = "v$version"
 annotated_tag = true
+gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
+[ci release]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "pythonprojectstructure"
 package_dir = "src"
 name = "python-project-structure"
```

### Comparing `python-project-structure-0.8.9b0/requirements/build.txt.in` & `python-project-structure-0.8.9b7/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/requirements/py310/build.txt` & `python-project-structure-0.8.9b7/requirements/py310/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `python-project-structure-0.8.9b0/requirements/py310/devel.txt` & `python-project-structure-0.8.9b7/requirements/py310/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `python-project-structure-0.8.9b0/requirements/py311/build.txt` & `python-project-structure-0.8.9b7/requirements/py311/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `python-project-structure-0.8.9b0/requirements/py311/devel.txt` & `python-project-structure-0.8.9b7/requirements/py311/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `python-project-structure-0.8.9b0/requirements/py37/build.txt` & `python-project-structure-0.8.9b7/requirements/py38/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -32,21 +32,18 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.2.0
+importlib-metadata==6.3.0
     # via
-    #   argcomplete
     #   keyring
-    #   pre-commit
     #   twine
-    #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -61,21 +58,21 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.0
     # via
@@ -93,32 +90,29 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
-    #   importlib-metadata
-    #   markdown-it-py
-    #   platformdirs
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `python-project-structure-0.8.9b0/requirements/py37/devel.txt` & `python-project-structure-0.8.9b7/requirements/py37/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `python-project-structure-0.8.9b0/requirements/py38/build.txt` & `python-project-structure-0.8.9b7/requirements/py37/build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -32,18 +32,21 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.3.0
+importlib-metadata==5.2.0
     # via
+    #   argcomplete
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -58,21 +61,21 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.0
     # via
@@ -90,29 +93,32 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `python-project-structure-0.8.9b0/requirements/py38/devel.txt` & `python-project-structure-0.8.9b7/requirements/py38/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `python-project-structure-0.8.9b0/requirements/py39/build.txt` & `python-project-structure-0.8.9b7/requirements/py39/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `python-project-structure-0.8.9b0/requirements/py39/devel.txt` & `python-project-structure-0.8.9b7/requirements/py39/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `python-project-structure-0.8.9b0/setup.cfg` & `python-project-structure-0.8.9b7/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.9b7/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.9b0
+Version: 0.8.9b7
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.9b0/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.9b7/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 .pre-commit-config.yaml
 .prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
 Dockerfile.devel
 LICENSE
 Makefile
+NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
 docker-compose.override.yml
 docker-compose.yml
 pyproject.toml
 setup.cfg
```

### Comparing `python-project-structure-0.8.9b0/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.9b7/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.9b7/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.9b0/tox.ini` & `python-project-structure-0.8.9b7/tox.ini`

 * *Files identical despite different names*

