# Comparing `tmp/flask-mongorest-mpcontribs-3.2.4.tar.gz` & `tmp/flask-mongorest-mpcontribs-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-mongorest-mpcontribs-3.2.4.tar", last modified: Fri Mar 31 20:49:38 2023, max compression
+gzip compressed data, was "flask-mongorest-mpcontribs-3.3.0.tar", last modified: Fri Apr 14 21:22:18 2023, max compression
```

## Comparing `flask-mongorest-mpcontribs-3.2.4.tar` & `flask-mongorest-mpcontribs-3.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.624733 flask-mongorest-mpcontribs-3.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.616733 flask-mongorest-mpcontribs-3.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.github/workflows/upgrade-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-31 20:49:38.624733 flask-mongorest-mpcontribs-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/example/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/example/documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/example/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47757 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.616733 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.620733 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/templates/mongorest/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/templates/mongorest/debug.html
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21857 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.624733 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 20:49:38.000000 flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:49:38.624733 flask-mongorest-mpcontribs-3.2.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-31 20:49:38.624733 flask-mongorest-mpcontribs-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 20:49:27.000000 flask-mongorest-mpcontribs-3.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.650416 flask-mongorest-mpcontribs-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.642416 flask-mongorest-mpcontribs-3.3.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.638416 flask-mongorest-mpcontribs-3.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.642416 flask-mongorest-mpcontribs-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.github/workflows/upgrade-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 21:22:18.650416 flask-mongorest-mpcontribs-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.646416 flask-mongorest-mpcontribs-3.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.646416 flask-mongorest-mpcontribs-3.3.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/example/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/example/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.646416 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48535 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.642416 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.646416 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/templates/mongorest/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/templates/mongorest/debug.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21857 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.650416 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 21:22:18.000000 flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:22:18.650416 flask-mongorest-mpcontribs-3.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 21:22:18.650416 flask-mongorest-mpcontribs-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 21:22:06.000000 flask-mongorest-mpcontribs-3.3.0/tox.ini
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/.circleci/config.yml` & `flask-mongorest-mpcontribs-3.3.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/.github/workflows/release.yaml` & `flask-mongorest-mpcontribs-3.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/.github/workflows/testing.yml` & `flask-mongorest-mpcontribs-3.3.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/.github/workflows/upgrade-dependencies.yml` & `flask-mongorest-mpcontribs-3.3.0/.github/workflows/upgrade-dependencies.yml`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/.pre-commit-config.yaml` & `flask-mongorest-mpcontribs-3.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/LICENSE` & `flask-mongorest-mpcontribs-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/PKG-INFO` & `flask-mongorest-mpcontribs-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-mongorest-mpcontribs
-Version: 3.2.4
+Version: 3.3.0
 Summary: Flask restful API framework for MongoDB/MongoEngine
 Home-page: http://github.com/tschaume/flask-mongorest
 Author: Close.io
 Author-email: engineering@close.io
 Maintainer: Patrick Huck
 Maintainer-email: phuck@lbl.gov
 License: BSD
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/README.md` & `flask-mongorest-mpcontribs-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/docs/Makefile` & `flask-mongorest-mpcontribs-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/docs/conf.py` & `flask-mongorest-mpcontribs-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/docs/make.bat` & `flask-mongorest-mpcontribs-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/example/app.py` & `flask-mongorest-mpcontribs-3.3.0/example/app.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/example/documents.py` & `flask-mongorest-mpcontribs-3.3.0/example/documents.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/example/schemas.py` & `flask-mongorest-mpcontribs-3.3.0/example/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest/__init__.py` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest/operators.py` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest/operators.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest/resources.py` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import orjson
 from collections import defaultdict
 from math import isnan
-from typing import Pattern
+from re import Pattern
 
 import mongoengine
+from atlasq import AtlasQuerySet
 from bson.dbref import DBRef
 from fastnumbers import fast_int
 from flask import has_request_context, request, url_for
 from flatten_dict import unflatten, flatten
 from boltons.iterutils import remap, default_enter
 from mongoengine.base.datastructures import BaseDict
 
@@ -711,18 +712,30 @@
 
     def get_queryset(self):
         """
         Return a MongoEngine queryset that will later be used to return
         matching documents.
         """
         document_fields = set(self.fields + self.get_optional_fields())
+        term = self.params.pop("_search", None)
+        has_atlas = callable(getattr(self.document, "atlas_filter", None))
 
         if request.method == "PUT":
             # make sure to get full documents for updates
             return self.document.objects.only(*document_fields)
+        elif request.method == "GET" and term and has_atlas:
+            try:
+                fltr = self.document.atlas_filter(term)
+            except Exception as ex:
+                raise ValidationError(ex)
+
+            if not fltr:
+                raise ValidationError(f"Couldn't get filter for {term}")
+
+            return self.document.atlas.filter(fltr)
         else:
             requested_fields = self.get_requested_fields(params=self.params)
             requested_root_fields = {f.split(".", 1)[0] for f in requested_fields}
             root_mask = requested_root_fields & document_fields
             mask = []
 
             for requested_field in requested_fields:
@@ -997,40 +1010,43 @@
         extra = {}
 
         if self.view_method == methods.Download:
             fmt = params.get("format")
             if fmt not in self.download_formats:
                 raise ValueError(f"`format` must be one of {self.download_formats}")
 
-        custom_qs = True
         if qs is None:
-            custom_qs = False
             qs = self.get_queryset()
 
         # Apply filters and ordering, based on the params supplied by the request
-        qs = self.apply_filters(qs, params)
-        qs = self.apply_ordering(qs, params)
+        # apply provided queryset if needed
+        if isinstance(qs, AtlasQuerySet):
+            match = self.apply_filters(self.document.objects, params)
+            if qfilter:
+                match = qfilter(match)
 
-        # If a queryset filter was provided, pass our current queryset in and
-        # get a new one out
-        if qfilter:
-            qs = qfilter(qs)
+            if match._query:
+                qs._aggrs.insert(1, {"$match": match._query})
+        else:
+            qs = self.apply_filters(qs, params)
+            qs = self.apply_ordering(qs, params)  # TODO respect ordering for Atlas Search?
+            if qfilter:
+                qs = qfilter(qs)
 
         # set total count
         extra["total_count"] = qs.count()
 
-        # Apply pagination to the queryset (if no custom queryset provided)
+        # Apply pagination to the queryset
         bulk_methods = {methods.BulkUpdate, methods.BulkDelete}
         limit = None
         if self.view_method in bulk_methods:
             # limit the number of objects that can be bulk-updated at a time
             qs = qs.limit(self.bulk_update_limit)
             limit = self.bulk_update_limit
-        elif not custom_qs:
-            # no need to skip/limit if a custom `qs` was provided
+        else:
             skip, limit = self.get_skip_and_limit(params)
             qs = qs.skip(skip).limit(limit + 1)  # get one extra to determine has_more
             if self.view_method != methods.Download:
                 qs = self.apply_field_pagination(qs, params)
             extra["total_pages"] = int(extra["total_count"] / limit) + bool(
                 extra["total_count"] % limit
             )
@@ -1041,14 +1057,18 @@
 
         # Evaluate the queryset
         # cheapest way to convert a queryset to a list: [i for i in qs]
         # list(queryset) uses a count() query to determine length
         # https://github.com/MongoEngine/mongoengine/blob/96802599045432274481b4ed9fcc4fad4ce5f89b/mongoengine/dereference.py#L39-L40
         objs = [i for i in qs]
 
+        # sort Atlas Search results by score
+        if isinstance(qs, AtlasQuerySet):
+            objs = sorted(objs, key=lambda o: -qs._scores[o.pk])
+
         # Determine the value of has_more
         has_more = False
         if self.paginate:
             has_more = len(objs) > limit
 
         if has_more:
             objs = objs[:-1]
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest/utils.py` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest/utils.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest/views.py` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest/views.py`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/PKG-INFO` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-mongorest-mpcontribs
-Version: 3.2.4
+Version: 3.3.0
 Summary: Flask restful API framework for MongoDB/MongoEngine
 Home-page: http://github.com/tschaume/flask-mongorest
 Author: Close.io
 Author-email: engineering@close.io
 Maintainer: Patrick Huck
 Maintainer-email: phuck@lbl.gov
 License: BSD
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/flask_mongorest_mpcontribs.egg-info/SOURCES.txt` & `flask-mongorest-mpcontribs-3.3.0/flask_mongorest_mpcontribs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.10.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
 dnspython==2.3.0
     # via pymongo
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
@@ -24,14 +30,16 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
+idna==3.4
+    # via requests
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
@@ -44,36 +52,41 @@
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.10_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
-    # via pytest-cov
 dnspython==2.3.0
     # via pymongo
-exceptiongroup==1.1.1
-    # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
-flake8==6.0.0
-    # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
     # via
     #   flask-mongoengine-tschaume
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-iniconfig==2.0.0
-    # via pytest
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
+    # via flask
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
@@ -50,60 +50,47 @@
     # via
     #   jinja2
     #   werkzeug
 marshmallow==3.19.0
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
-mccabe==0.7.0
-    # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
-    # via
-    #   marshmallow
-    #   pytest
-pluggy==1.0.0
-    # via pytest
-pycodestyle==2.10.0
-    # via flake8
-pyflakes==3.0.1
-    # via flake8
+packaging==23.1
+    # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
-    # via
-    #   flask-mongorest-mpcontribs (setup.py)
-    #   pytest-cov
-pytest-cov==4.0.0
-    # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.8.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.10.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
 dnspython==2.3.0
     # via pymongo
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
@@ -24,16 +30,16 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
-    # via flask
+idna==3.4
+    # via requests
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
@@ -46,38 +52,41 @@
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.8_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
+    # via flask-mongorest-mpcontribs (setup.py)
+boto3==1.26.114
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 dnspython==2.3.0
     # via pymongo
 exceptiongroup==1.1.1
     # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
@@ -32,16 +36,16 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
-    # via flask
+idna==3.4
+    # via requests
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -58,56 +62,59 @@
     # via flask-mongorest-mpcontribs (setup.py)
 mccabe==0.7.0
     # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via
     #   marshmallow
     #   pytest
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.9.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.9.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/macos-latest_py3.9.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
 dnspython==2.3.0
     # via pymongo
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
@@ -24,15 +30,17 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
     # via flask
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -46,38 +54,43 @@
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/macos-latest_py3.9_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
+    # via flask-mongorest-mpcontribs (setup.py)
+boto3==1.26.114
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 dnspython==2.3.0
     # via pymongo
 exceptiongroup==1.1.1
     # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
@@ -32,16 +36,16 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
-    # via flask
+idna==3.4
+    # via requests
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -58,56 +62,59 @@
     # via flask-mongorest-mpcontribs (setup.py)
 mccabe==0.7.0
     # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via
     #   marshmallow
     #   pytest
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.10.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
 dnspython==2.3.0
     # via pymongo
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
@@ -24,14 +30,18 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
+    # via flask
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
@@ -44,36 +54,43 @@
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.10_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
+    # via flask-mongorest-mpcontribs (setup.py)
+boto3==1.26.114
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 dnspython==2.3.0
     # via pymongo
 exceptiongroup==1.1.1
     # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
@@ -32,14 +36,18 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
+    # via flask
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -56,54 +64,61 @@
     # via flask-mongorest-mpcontribs (setup.py)
 mccabe==0.7.0
     # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via
     #   marshmallow
     #   pytest
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.8.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.8.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
 dnspython==2.3.0
     # via pymongo
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
@@ -24,15 +30,17 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
     # via flask
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -46,38 +54,43 @@
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.8_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
+    # via flask-mongorest-mpcontribs (setup.py)
+boto3==1.26.114
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 dnspython==2.3.0
     # via pymongo
 exceptiongroup==1.1.1
     # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
@@ -32,15 +36,17 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
     # via flask
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
@@ -58,56 +64,61 @@
     # via flask-mongorest-mpcontribs (setup.py)
 mccabe==0.7.0
     # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via
     #   marshmallow
     #   pytest
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.9.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+boto3==1.26.114
+    # via flask-mongorest-mpcontribs (setup.py)
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
+coverage[toml]==7.2.3
+    # via pytest-cov
 dnspython==2.3.0
     # via pymongo
+exceptiongroup==1.1.1
+    # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
+flake8==6.0.0
+    # via flask-mongorest-mpcontribs (setup.py)
 flask==2.2.3
     # via
     #   flask-mongoengine-tschaume
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
     # via flask
+iniconfig==2.0.0
+    # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
@@ -42,42 +58,67 @@
     # via
     #   jinja2
     #   werkzeug
 marshmallow==3.19.0
     # via marshmallow-mongoengine
 marshmallow-mongoengine==0.31.2
     # via flask-mongorest-mpcontribs (setup.py)
+mccabe==0.7.0
+    # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
-    # via marshmallow
+packaging==23.1
+    # via
+    #   marshmallow
+    #   pytest
+pluggy==1.0.0
+    # via pytest
+pycodestyle==2.10.0
+    # via flake8
+pyflakes==3.0.1
+    # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
+pytest==7.3.1
+    # via
+    #   flask-mongorest-mpcontribs (setup.py)
+    #   pytest-cov
+pytest-cov==4.0.0
+    # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/requirements/ubuntu-latest_py3.9_extras.txt` & `flask-mongorest-mpcontribs-3.3.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
-    # via pytest
-boto3==1.26.104
+atlasq-tschaume==0.11.1.dev2
+    # via flask-mongorest-mpcontribs (setup.py)
+boto3==1.26.114
     # via flask-mongorest-mpcontribs (setup.py)
-botocore==1.29.104
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via flask
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 dnspython==2.3.0
     # via pymongo
 exceptiongroup==1.1.1
     # via pytest
 fastnumbers==5.0.1
     # via flask-mongorest-mpcontribs (setup.py)
@@ -32,15 +36,17 @@
     #   flask-sse
 flask-mongoengine-tschaume==1.1.0
     # via flask-mongorest-mpcontribs (setup.py)
 flask-sse==1.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 flatten-dict==0.4.2
     # via flask-mongorest-mpcontribs (setup.py)
-importlib-metadata==6.1.0
+idna==3.4
+    # via requests
+importlib-metadata==6.3.0
     # via flask
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
@@ -58,56 +64,61 @@
     # via flask-mongorest-mpcontribs (setup.py)
 mccabe==0.7.0
     # via flake8
 mimerender-pr36==0.0.2
     # via flask-mongorest-mpcontribs (setup.py)
 mongoengine==0.27.0
     # via
+    #   atlasq-tschaume
     #   flask-mongoengine-tschaume
     #   marshmallow-mongoengine
-orjson==3.8.9
+orjson==3.8.10
     # via flask-mongorest-mpcontribs (setup.py)
-packaging==23.0
+packaging==23.1
     # via
     #   marshmallow
     #   pytest
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pymongo==4.3.3
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   mongoengine
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   flask-mongorest-mpcontribs (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via flask-mongorest-mpcontribs (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   flask-mongorest-mpcontribs (setup.py)
 python-mimeparse==1.6.0
     # via mimerender-pr36
 redis==4.5.4
     # via flask-sse
+requests==2.28.2
+    # via atlasq-tschaume
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   flask-sse
     #   flatten-dict
     #   python-dateutil
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 urllib3==1.26.15
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 werkzeug==2.2.3
     # via flask
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/setup.py` & `flask-mongorest-mpcontribs-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         "flask-sse>=1.0.0",
         "flatten-dict",
         "marshmallow-mongoengine>=0.31.0",
         "mimerender-pr36>=0.0.2",
         "pymongo>=3.12.0",
         "python-dateutil",
         "orjson",
+        "atlasq-tschaume",
     ],
     extras_require={
         'dev': [
             "flake8",
             "pytest",
             "pytest-cov"
         ]
```

### Comparing `flask-mongorest-mpcontribs-3.2.4/tests.py` & `flask-mongorest-mpcontribs-3.3.0/tests.py`

 * *Files identical despite different names*

