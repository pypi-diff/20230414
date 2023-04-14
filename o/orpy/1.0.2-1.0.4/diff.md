# Comparing `tmp/orpy-1.0.2.tar.gz` & `tmp/orpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orpy-1.0.2.tar", last modified: Tue Nov 30 14:52:09 2021, max compression
+gzip compressed data, was "orpy-1.0.4.tar", last modified: Fri Apr 14 07:16:45 2023, max compression
```

## Comparing `orpy-1.0.2.tar` & `orpy-1.0.4.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.908538 orpy-1.0.2/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      102 2019-06-07 14:20:32.000000 orpy-1.0.2/.coveragerc
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.888538 orpy-1.0.2/.github/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      308 2019-06-07 14:20:32.000000 orpy-1.0.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1384 2019-06-07 14:20:32.000000 orpy-1.0.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.888538 orpy-1.0.2/.github/workflows/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      864 2021-11-29 22:24:22.000000 orpy-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       89 2019-06-07 14:20:32.000000 orpy-1.0.2/.mailmap
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      319 2019-06-07 14:20:32.000000 orpy-1.0.2/.testr.conf
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       85 2021-11-30 14:52:08.000000 orpy-1.0.2/AUTHORS
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3231 2019-06-07 14:20:32.000000 orpy-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    14141 2019-06-07 14:20:32.000000 orpy-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2217 2021-11-30 14:52:08.000000 orpy-1.0.2/ChangeLog
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    10143 2019-06-07 14:20:32.000000 orpy-1.0.2/LICENSE
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       94 2019-06-07 14:20:32.000000 orpy-1.0.2/MANIFEST.in
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     6246 2021-11-30 14:52:09.908538 orpy-1.0.2/PKG-INFO
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     4351 2021-01-27 17:05:30.000000 orpy-1.0.2/README.md
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.888538 orpy-1.0.2/doc/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      207 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/requirements.txt
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.892538 orpy-1.0.2/doc/source/
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.892538 orpy-1.0.2/doc/source/_static/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     9342 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/_static/logo.png
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.896538 orpy-1.0.2/doc/source/_templates/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      282 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/_templates/sidebarfooter.html
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1990 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/api.rst
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3231 2019-06-07 14:20:32.000000 orpy-1.0.2/doc/source/code_of_conduct.md
--rwxr-xr-x   0 alvaro    (1000) alvaro    (1000)     7069 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/conf.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    14141 2019-06-07 14:20:32.000000 orpy-1.0.2/doc/source/contributing.md
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1198 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/index.rst
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      200 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/installation.rst
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.896538 orpy-1.0.2/doc/source/releasenotes/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      113 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/releasenotes/index.rst
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.896538 orpy-1.0.2/doc/source/user/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1375 2021-01-27 17:05:30.000000 orpy-1.0.2/doc/source/user/shell.rst
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.896538 orpy-1.0.2/orpy/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      660 2019-06-07 14:20:32.000000 orpy-1.0.2/orpy/__init__.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.904538 orpy-1.0.2/orpy/client/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        0 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/client/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3415 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/client/base.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    12467 2021-11-30 14:48:21.000000 orpy-1.0.2/orpy/client/client.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1420 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/client/config.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     4278 2021-11-30 14:48:46.000000 orpy-1.0.2/orpy/client/deployments.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1378 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/client/info.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1701 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/client/resources.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.904538 orpy-1.0.2/orpy/cmd/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        0 2019-06-07 14:20:32.000000 orpy-1.0.2/orpy/cmd/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1150 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/cmd/config.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     9061 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/cmd/deployments.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1161 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/cmd/info.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2363 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/cmd/resources.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     5727 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/exceptions.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2484 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/oidc.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     6501 2021-01-27 21:21:20.000000 orpy-1.0.2/orpy/shell.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.904538 orpy-1.0.2/orpy/tests/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        0 2019-06-07 14:20:32.000000 orpy-1.0.2/orpy/tests/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1927 2019-06-07 14:20:32.000000 orpy-1.0.2/orpy/tests/base.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      756 2019-06-07 14:20:32.000000 orpy-1.0.2/orpy/tests/test_orpy.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2182 2021-11-29 22:24:22.000000 orpy-1.0.2/orpy/utils.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      898 2021-01-27 17:05:30.000000 orpy-1.0.2/orpy/version.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.900538 orpy-1.0.2/orpy.egg-info/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     6246 2021-11-30 14:52:08.000000 orpy-1.0.2/orpy.egg-info/PKG-INFO
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1532 2021-11-30 14:52:09.000000 orpy-1.0.2/orpy.egg-info/SOURCES.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        1 2021-11-30 14:52:08.000000 orpy-1.0.2/orpy.egg-info/dependency_links.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      910 2021-11-30 14:52:08.000000 orpy-1.0.2/orpy.egg-info/entry_points.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        1 2019-06-07 14:22:21.000000 orpy-1.0.2/orpy.egg-info/not-zip-safe
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       47 2021-01-27 21:17:33.000000 orpy-1.0.2/orpy.egg-info/pbr.json
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       70 2021-11-30 14:52:08.000000 orpy-1.0.2/orpy.egg-info/requires.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        5 2021-11-30 14:52:08.000000 orpy-1.0.2/orpy.egg-info/top_level.txt
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.876538 orpy-1.0.2/releasenotes/
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2021-11-30 14:52:09.908538 orpy-1.0.2/releasenotes/notes/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      263 2021-01-27 17:05:30.000000 orpy-1.0.2/releasenotes/notes/initial-version-with-full-functionality-c63da317250d228d.yaml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      143 2021-11-29 22:24:22.000000 orpy-1.0.2/releasenotes/notes/new-command-configuration-show-645affdd13bfd015.yaml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      169 2021-11-29 22:24:22.000000 orpy-1.0.2/releasenotes/notes/new-long-output-ddcb9d95d1431e47.yaml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      135 2021-01-27 17:05:30.000000 orpy-1.0.2/releasenotes/notes/use-objects-bf546c89548f424c.yaml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      131 2021-01-27 17:05:30.000000 orpy-1.0.2/releasenotes/notes/use-oidc-agent-bdfbb4d37788a455.yaml
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      188 2021-01-27 17:05:30.000000 orpy-1.0.2/requirements.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2183 2021-11-30 14:52:09.912538 orpy-1.0.2/setup.cfg
--rwxr-xr-x   0 alvaro    (1000) alvaro    (1000)      781 2019-06-07 15:57:40.000000 orpy-1.0.2/setup.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      450 2021-01-27 17:05:30.000000 orpy-1.0.2/test-requirements.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2653 2021-01-27 17:05:30.000000 orpy-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 07:16:31.000000 orpy-1.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 07:16:31.000000 orpy-1.0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-14 07:16:31.000000 orpy-1.0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 07:16:31.000000 orpy-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-14 07:16:31.000000 orpy-1.0.4/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 07:16:31.000000 orpy-1.0.4/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 07:16:31.000000 orpy-1.0.4/.testr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 07:16:44.000000 orpy-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-14 07:16:31.000000 orpy-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-04-14 07:16:31.000000 orpy-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 07:16:44.000000 orpy-1.0.4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-14 07:16:31.000000 orpy-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 07:16:31.000000 orpy-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-14 07:16:45.018660 orpy-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-14 07:16:31.000000 orpy-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/_templates/sidebarfooter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/code_of_conduct.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7069 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/source/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/releasenotes/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/doc/source/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 07:16:31.000000 orpy-1.0.4/doc/source/user/shell.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/orpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/orpy/_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/_cmd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/_cmd/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/_cmd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/_cmd/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/orpy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/client/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/orpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/tests/test_orpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-14 07:16:31.000000 orpy-1.0.4/orpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/orpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 07:16:44.000000 orpy-1.0.4/orpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.014660 orpy-1.0.4/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:16:45.018660 orpy-1.0.4/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 07:16:31.000000 orpy-1.0.4/releasenotes/notes/initial-version-with-full-functionality-c63da317250d228d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-14 07:16:31.000000 orpy-1.0.4/releasenotes/notes/new-command-configuration-show-645affdd13bfd015.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 07:16:31.000000 orpy-1.0.4/releasenotes/notes/new-long-output-ddcb9d95d1431e47.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 07:16:31.000000 orpy-1.0.4/releasenotes/notes/use-objects-bf546c89548f424c.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 07:16:31.000000 orpy-1.0.4/releasenotes/notes/use-oidc-agent-bdfbb4d37788a455.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 07:16:31.000000 orpy-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 07:16:45.018660 orpy-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-04-14 07:16:31.000000 orpy-1.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-14 07:16:31.000000 orpy-1.0.4/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-14 07:16:31.000000 orpy-1.0.4/tox.ini
```

### Comparing `orpy-1.0.2/.github/PULL_REQUEST_TEMPLATE.md` & `orpy-1.0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/.github/workflows/python-publish.yml` & `orpy-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/CODE_OF_CONDUCT.md` & `orpy-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/CONTRIBUTING.md` & `orpy-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/LICENSE` & `orpy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/PKG-INFO` & `orpy-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,17 @@
 Metadata-Version: 2.1
 Name: orpy
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python library and CLI for the INDIGO PaaS Orchestrator.
 Home-page: https://github.com/indigo-dc/orpy
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/indigo-dc/orpy/issues
 Project-URL: Documentation, https://orpy.readthedocs.io/
-Description: # orpy
-        
-        Python library and CLI for the INDIGO PaaS Orchestrator.
-        
-        <img src="https://marketplace.deep-hybrid-datacloud.eu/images/logo-deep.png" width=200 alt="DEEP-Hybrid-DataCloud logo"/>
-        
-        * Free software: Apache License 2.0
-        * Source: https://github.com/indigo-dc/orpy
-        * Documentation: https://orpy.readthedocs.io/
-        * Bugs: https://github.com/indigo-dc/orpy/issues
-        
-        ## Installation.
-        
-        You can install it directly from PyPI:
-        
-            pip install orpy
-        
-        ## Usage as CLI
-        
-        Before using the orchestrator with orpy you need to export your IAM access
-        token. As long as the access token is valid orchent can tell the orchestrator
-        what to do.
-        
-            export ORCHESTRATOR_TOKEN=<your access token here>
-        
-        Please check the [documentation](https://docs.deep-hybrid-datacloud.eu/projects/orpy/en/stable/user/shell.html)
-        for more details on how to set the credentials.
-        
-        Then, the usage is as follows:
-        
-            usage: orpy [--version] [-v | -q] [--log-file LOG_FILE] [-h] [--debug]
-                       [--url <orchestrator-url>]
-        
-            Command line client for the INDIGO PaaS Orchestrator.
-        
-                Please, before using this command put your a valid OpenID Connnect access
-                token into the ORCHESTRATOR_TOKEN environment variable, so that we can use
-                this token for authentication.
-        
-        
-            optional arguments:
-              --version             show program's version number and exit
-              -v, --verbose         Increase verbosity of output. Can be repeated.
-              -q, --quiet           Suppress output except warnings and errors.
-              --log-file LOG_FILE   Specify a file to log output. Disabled by default.
-              -h, --help            Show help message and exit.
-              --debug               Show tracebacks on errors.
-              --url <orchestrator-url>
-                                    The base url of the orchestrator rest interface.
-                                    Alternative the environment variable ORCHESTRATOR_URL
-                                    can be used.
-        
-            Commands:
-              complete       print bash completion command (cliff)
-              dep create     Create a deployment.
-              dep delete     Show details about an existing deployment.
-              dep list       List existing deployments at orchestrator.
-              dep show       Show details about an existing deployment.
-              dep template   Get template used for a given deployment.
-              dep update     Update an existing deployment.
-              deployment create  Create a deployment.
-              deployment delete  Show details about an existing deployment.
-              deployment list  List existing deployments at orchestrator.
-              deployment show  Show details about an existing deployment.
-              deployment template  Get template used for a given deployment.
-              deployment update  Update an existing deployment.
-              help           print detailed help for another command (cliff)
-              resources list  List Resources for a given deployment.
-              resources show  Show details about a resource for a given deployment.
-              test           Test if the given URL is pointing to an orchestrator.
-        
-        ## Usage as API
-        
-        Besides being a CLI application, `orpy` can be used as a library:
-        
-            >>> from orpy.client import client
-            >>> orpy = client.OrpyClient(
-            ...     url=ORCHESTRATOR_URL,
-            ...     token=ORCHESTRATOR_TOKEN)
-            >>> deployments = orpy.deployments.list()
-            >>> deployments[0]
-            <Deployment cloudProviderName=provider-BARI, createdBy={u'subject': u'de28e179-ec86-4915-a748-7a37f8d80311', u'issuer': u'https://iam.deep-hybrid-datacloud.eu/'}, creationTime=2019-05-27T11:31+0000, links=[{u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005', u'rel': u'self'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/resources', u'rel': u'resources'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/template', u'rel': u'template'}], outputs={}, physicalId=11e98073-06f3-6797-9258-0242ac140005, status=CREATE_FAILED, statusReason=Error while checking the deployment status; nested exception is feign.RetryableException: mesos.ui.sav.sk executing GET https://mesos.ui.sav.sk/marathon/v2/groups/11e98073-06f3-6797-9258-0242ac140005, task=NONE, updateTime=2019-05-29T02:05+0000, uuid=11e98073-06f3-6797-9258-0242ac140005>
-            >>> deployments[0].status
-            CREATE_FAILED
-            >>>
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -109,7 +21,95 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# orpy
+
+Python library and CLI for the INDIGO PaaS Orchestrator.
+
+<img src="https://marketplace.deep-hybrid-datacloud.eu/images/logo-deep.png" width=200 alt="DEEP-Hybrid-DataCloud logo"/>
+
+* Free software: Apache License 2.0
+* Source: https://github.com/indigo-dc/orpy
+* Documentation: https://orpy.readthedocs.io/
+* Bugs: https://github.com/indigo-dc/orpy/issues
+
+## Installation.
+
+You can install it directly from PyPI:
+
+    pip install orpy
+
+## Usage as CLI
+
+Before using the orchestrator with orpy you need to export your IAM access
+token. As long as the access token is valid orchent can tell the orchestrator
+what to do.
+
+    export ORCHESTRATOR_TOKEN=<your access token here>
+
+Please check the [documentation](https://docs.deep-hybrid-datacloud.eu/projects/orpy/en/stable/user/shell.html)
+for more details on how to set the credentials.
+
+Then, the usage is as follows:
+
+    usage: orpy [--version] [-v | -q] [--log-file LOG_FILE] [-h] [--debug]
+               [--url <orchestrator-url>]
+
+    Command line client for the INDIGO PaaS Orchestrator.
+
+        Please, before using this command put your a valid OpenID Connnect access
+        token into the ORCHESTRATOR_TOKEN environment variable, so that we can use
+        this token for authentication.
+
+
+    optional arguments:
+      --version             show program's version number and exit
+      -v, --verbose         Increase verbosity of output. Can be repeated.
+      -q, --quiet           Suppress output except warnings and errors.
+      --log-file LOG_FILE   Specify a file to log output. Disabled by default.
+      -h, --help            Show help message and exit.
+      --debug               Show tracebacks on errors.
+      --url <orchestrator-url>
+                            The base url of the orchestrator rest interface.
+                            Alternative the environment variable ORCHESTRATOR_URL
+                            can be used.
+
+    Commands:
+      complete       print bash completion command (cliff)
+      dep create     Create a deployment.
+      dep delete     Show details about an existing deployment.
+      dep list       List existing deployments at orchestrator.
+      dep show       Show details about an existing deployment.
+      dep template   Get template used for a given deployment.
+      dep update     Update an existing deployment.
+      deployment create  Create a deployment.
+      deployment delete  Show details about an existing deployment.
+      deployment list  List existing deployments at orchestrator.
+      deployment show  Show details about an existing deployment.
+      deployment template  Get template used for a given deployment.
+      deployment update  Update an existing deployment.
+      help           print detailed help for another command (cliff)
+      resources list  List Resources for a given deployment.
+      resources show  Show details about a resource for a given deployment.
+      test           Test if the given URL is pointing to an orchestrator.
+
+## Usage as API
+
+Besides being a CLI application, `orpy` can be used as a library:
+
+    >>> from orpy.client import client
+    >>> orpy = client.OrpyClient(
+    ...     url=ORCHESTRATOR_URL,
+    ...     token=ORCHESTRATOR_TOKEN)
+    >>> deployments = orpy.deployments.list()
+    >>> deployments[0]
+    <Deployment cloudProviderName=provider-BARI, createdBy={u'subject': u'de28e179-ec86-4915-a748-7a37f8d80311', u'issuer': u'https://iam.deep-hybrid-datacloud.eu/'}, creationTime=2019-05-27T11:31+0000, links=[{u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005', u'rel': u'self'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/resources', u'rel': u'resources'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/template', u'rel': u'template'}], outputs={}, physicalId=11e98073-06f3-6797-9258-0242ac140005, status=CREATE_FAILED, statusReason=Error while checking the deployment status; nested exception is feign.RetryableException: mesos.ui.sav.sk executing GET https://mesos.ui.sav.sk/marathon/v2/groups/11e98073-06f3-6797-9258-0242ac140005, task=NONE, updateTime=2019-05-29T02:05+0000, uuid=11e98073-06f3-6797-9258-0242ac140005>
+    >>> deployments[0].status
+    CREATE_FAILED
+    >>>
+
```

### Comparing `orpy-1.0.2/README.md` & `orpy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/_static/logo.png` & `orpy-1.0.4/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/api.rst` & `orpy-1.0.4/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/code_of_conduct.md` & `orpy-1.0.4/doc/source/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/conf.py` & `orpy-1.0.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/contributing.md` & `orpy-1.0.4/doc/source/contributing.md`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/index.rst` & `orpy-1.0.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/doc/source/user/shell.rst` & `orpy-1.0.4/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `orpy-1.0.2/orpy/__init__.py` & `orpy-1.0.4/orpy/tests/test_orpy.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,12 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import pbr.version
+"""Tests for `orpy` module."""
 
+from orpy.tests import base
 
-__version__ = pbr.version.VersionInfo(
-    'orpy').version_string()
+
+class TestOrpy(base.TestCase):
+    """Base test class."""
+
+    def test_something(self):
+        """Test something please."""
+        pass
```

### Comparing `orpy-1.0.2/orpy/client/base.py` & `orpy-1.0.4/orpy/client/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,63 +10,67 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Module defining base object for all orchestrator resources."""
+
 import copy
 
 
 class BaseObject(object):
     """Base class for all objects that represents orchestrator resoruces."""
 
     def __init__(self, info):
-        """Initalize the object.
+        """Init the object.
 
         :param dict info: A dictionary object containing the object's
                           information
         """
         self._info = {}
         self._add_details(info)
         self.uuid = info.get("uuid", None)
 
     def __repr__(self):
-        reprkeys = sorted(k
-                          for k in self.__dict__.keys()
-                          if k[0] != '_')
+        """Return representation of object."""
+        reprkeys = sorted(k for k in self.__dict__.keys() if k[0] != "_")
         info = ", ".join("%s=%s" % (k, getattr(self, k)) for k in reprkeys)
         return "<%s %s>" % (self.__class__.__name__, info)
 
     def _add_details(self, info):
         for (k, v) in info.items():
             try:
                 setattr(self, k, v)
                 self._info[k] = v
             except AttributeError:
                 # In this case we already defined the attribute on the class
                 pass
 
     def __getattr__(self, k):
+        """Get an attribute from the object."""
         if k not in self.__dict__:
             raise AttributeError(k)
         else:
             return self.__dict__[k]
 
     def __eq__(self, other):
+        """Return of this object equals to another."""
         if not isinstance(other, BaseObject):
             return NotImplemented
         # two resources of different types are not equal
         if not isinstance(other, self.__class__):
             return False
-        if hasattr(self, 'id') and hasattr(other, 'id'):
+        if hasattr(self, "id") and hasattr(other, "id"):
             return self.id == other.id
         return self._info == other._info
 
     def __ne__(self, other):
+        """Return if this object is different from another one."""
         # Using not of '==' implementation because the not of
         # __eq__, when it returns NotImplemented, is returning False.
         return not self == other
 
     def set_info(self, key, value):
         """Set an objects information with key, value.
 
@@ -80,36 +84,42 @@
 
         :return: A dictionary contaning the object representation
         :rtype: dict
         """
         return copy.deepcopy(self._info)
 
     def get(self, k, default=None):
+        """Get an attribute from the resource."""
         try:
             return self.__getattr__(k)
         except AttributeError:
             return default
 
 
 class Deployment(BaseObject):
     """Object that represents a deployment."""
+
     pass
 
 
 class Resource(BaseObject):
     """Object that represents a Resource."""
+
     pass
 
 
 class TOSCATemplate(BaseObject):
     """Object that repesents a TOSCA template."""
+
     pass
 
 
 class OrchestratorInfo(BaseObject):
     """Object that represents the Orchestrtor information."""
+
     pass
 
 
 class OrchestratorConfiguration(BaseObject):
     """Object that represents the Orchestrtor information."""
+
     pass
```

### Comparing `orpy-1.0.2/orpy/client/client.py` & `orpy-1.0.4/orpy/client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""INDIGO-DataCloud PaaS orchestrator client module."""
+
 import copy
 import datetime
 import hashlib
 import json
 import logging
 import uuid
 import warnings
@@ -31,63 +33,80 @@
 from orpy.client import info
 from orpy.client import resources
 from orpy import exceptions
 from orpy import version
 
 
 class _JSONEncoder(json.JSONEncoder):
-
     def default(self, o):
         if isinstance(o, datetime.datetime):
             return o.isoformat()
         if isinstance(o, uuid.UUID):
             return six.text_type(o)
 
         return super(_JSONEncoder, self).default(o)
 
 
 class OrpyClient(object):
-    """An INDIGO-DataCloud PaaS orchestrator client class."""
+    """An INDIGO-DataCloud PaaS orchestrator client class.
+
+    If you want an authenticated client, when creating the object you MUST pass either:
+        - An orpy.oidc.OpenIDConnectAgent object (oidc_agent parameter)
+        - An orpy.oidc.OpenIDConnectSession object (oidc_session parameter)
+        - An access token for authentication (token parameter)
+
+    The first method is the preferred, you can create an object this way (assuming that
+    the oidc-agent account is named "oidc-agent-account":
+
+        from orpy import oidc
+        from orpy.client import client
+        oidc_agent = oidc.OpenIDConnectAgent("oidc-agent-account")
+
+        cli = client.OrpyClient(url, oidc_agent=oidc_agent)
+
+    The second method is only useful when you are programming a library and have access
+    to a requests.Request like object session, like the ones used by Flask Dance:
 
-    def __init__(self, url, oidc_agent=None, token=None, debug=False):
-        """Initialization of OrpyClient object.
+        from orpy import oidc
+        from orpy.client import client
+        oidc_session = oidc.OpenIDConnectSession(flask_blueprint.session)
 
-        You MUST pass either a valid orpy.oidc.OpenIDConnectAgent object into
-        the oidc_agent parameter or a valid access token for authentication.
-        The former method is the preferred, you can create an object this way
-        (assuming that the oidc-agent account is named "oidc-agent-account":
+        cli = client.OrpyClient(url oidc_session=oidc_session)
 
-            from orpy import oidc
-            from orpy.client import client
-            oidc_agent = oidc.OpenIDConnectAgent("oidc-agent-account")
+    Note that passing more than one of the above methods will result in a warning, not
+    an error. In that case, the preference is the following (note also that if one
+    method fails we will not continue to the next one, so the rest of the methods are
+    actually ignored):
 
-            cli = client.OrpyClient(url, oidc_agent=oidc_agent)
+        - oidc_agent
+        - oidc_session
+        - token
 
-        Note that passing both will result in a warning, with the access token
-        passed in the token paramter ignored.
+    If you do not pass any of these when creating the client, but you want
+    to setup them afterwards, you can do so with the set_authentication method.
+    """
+
+    def __init__(
+        self, url, oidc_agent=None, token=None, oidc_session=None, debug=False
+    ):
+        """Initialize of OrpyClient object.
 
         :param str url: Orchestrator URL
         :param orpy.oidc.OpenIDConnectAgent oidc_agent: OpenID Connect agent
                                                         object to use for
-                                                        fetching access tokens
+                                                        fetching access tokens.
+        :param orpy.oidc.OpenIDConnectSession oidc_session: OpenID Connect
+                                                            session to use for
+                                                            fetching the token.
         :param str token: OpenID Connect access token to use for auth.
         :param bool debug: whether to enable debug logging
         """
-
         self.url = url + "/"
-        self._token = token
-        self.oidc_agent = oidc_agent
 
-        if not any([oidc_agent, token]):
-            raise exceptions.InvalidUsage("Must pass either an oidc-agent "
-                                          "object or an access token.")
-        if all([oidc_agent, token]):
-            msg = ("Using both oidc-agent and access token means that the "
-                   "user provider token will be ignored.")
-            warnings.warn(msg, RuntimeWarning)
+        self.set_authentication(token=token, agent=oidc_agent, session=oidc_session)
 
         self.http_debug = debug
 
         self._deployments = deployments.Deployments(self)
         self._resources = resources.Resources(self)
         self._info = info.Info(self)
         self._config = config.Config(self)
@@ -95,30 +114,72 @@
         self._logger = logging.getLogger(__name__)
 
         if self.http_debug:
             # Logging level is already set on the root logger
             ch = logging.StreamHandler()
             self._logger.addHandler(ch)
             self._logger.propagate = False
-            if hasattr(requests, 'logging'):
+            if hasattr(requests, "logging"):
                 rql = requests.logging.getLogger(requests.__name__)
                 rql.addHandler(ch)
                 # Since we have already setup the root logger on debug, we
                 # have to set it up here on WARNING (its original level)
                 # otherwise we will get all the requests logging messages
                 rql.setLevel(logging.WARNING)
 
         self._json = _JSONEncoder()
         self.session = requests.Session()
 
+    def set_authentication(self, token=None, agent=None, session=None):
+        """Set OIDC authentication options.
+
+        :param orpy.oidc.OpenIDConnectAgent oidc_agent: OpenID Connect agent
+                                                        object to use for
+                                                        fetching access tokens.
+        :param orpy.oidc.OpenIDConnectSession oidc_session: OpenID Connect
+                                                            session to use for
+                                                            fetching the token.
+        :param str token: OpenID Connect access token to use for auth.
+        """
+        self._token = token
+        self.oidc_agent = agent
+        self.oidc_session = session
+
+        if [agent, session, token].count(None) < 2:
+            msg = (
+                "Using more than one of oidc-agent oidc-session and access "
+                "token means that only one of them will be used, check "
+                "documentation. "
+                f"token: -{token}- "
+                f"agent: -{agent}- "
+                f"session: -{session}- "
+            )
+            warnings.warn(msg, RuntimeWarning)
+
+    def _check_auth(self):
+        token = self._token
+        oidc_agent = self.oidc_agent
+        oidc_session = self.oidc_session
+
+        if not any([oidc_agent, oidc_session, token]):
+            raise exceptions.InvalidUsageError(
+                "Authentication is not correctly setup. You must pass either an "
+                "oidc-agent object, an oidc-session object or an access token."
+            )
+
     @property
     def token(self):
+        """Get an access token to interact with the Orchestrator."""
+        self._check_auth()
+
         token = self._token
         if self.oidc_agent is not None:
             token = self.oidc_agent.get_token()["access_token"]
+        elif self.oidc_session is not None:
+            token = self.oidc_session.get_token()["access_token"]
         return token
 
     @property
     def deployments(self):
         """Interface to query for deployments.
 
         :return: Deployments interface.
@@ -149,65 +210,69 @@
         """Interface to query for Orchestrator information.
 
         :return: Information interface.
         :rtype: orpy.info.Info
         """
         return self._info
 
-    def request(self, url, method, json=None, **kwargs):
+    def request(self, url, method, authenticated=True, payload=None, **kwargs):
         """Send an HTTP request with the specified characteristics.
 
         Wrapper around `requests.Session.request` to handle tasks such as
         setting headers, JSON encoding/decoding, and error handling.
 
         Arguments that are not handled are passed through to the requests
         library.
 
         :param str url: Path or fully qualified URL of the HTTP request. If
                         only a path is provided then the URL will be prefixed
                         with the attribute self.url. If a fully qualified URL
                         is provided then self.url will be ignored.
         :param str method: The http method to use. (e.g. 'GET', 'POST')
-        :param json: Some data to be represented as JSON. (optional)
+        :param bool authenticated: Whether the request must be authenticated or not.
+        :param payload: Some data to be represented as JSON. (optional)
         :param kwargs: any other parameter that can be passed to
                        :meth:`requests.Session.request` (such as `headers`).
                        Except:
 
-                       - `data` will be overwritten by the data in the `json`
-                         param.
+                       - `data` will be overwritten by the data in the
+                         `payload` param.
                        - `allow_redirects` is ignored as redirects are handled
                          by the session.
 
         :returns: The response to the request.
         """
-
         method = method.lower()
 
-        kwargs.setdefault('headers', kwargs.get('headers', {}))
+        kwargs.setdefault("headers", kwargs.get("headers", {}))
 
         kwargs["headers"]["User-Agent"] = "orpy-%s" % version.user_agent
         kwargs["headers"]["Accept"] = "application/json"
 
-        if self.token is not None:
+        if authenticated and self.token is not None:
             kwargs["headers"]["Authorization"] = "Bearer" + self.token
 
-        if json is not None:
-            kwargs["headers"].setdefault('Content-Type', 'application/json')
-            kwargs['data'] = self._json.encode(json)
+        if payload is not None:
+            kwargs["headers"].setdefault("Content-Type", "application/json")
+            kwargs["data"] = self._json.encode(payload)
 
         url = parse.urljoin(self.url, url)
 
-        self.http_log_req(method, url, kwargs)
+        self._http_log_req(method, url, kwargs)
 
         resp = self.session.request(method, url, **kwargs)
 
-        self.http_log_resp(resp)
+        self._http_log_resp(resp)
 
         if resp.status_code >= 400:
-            raise exceptions.from_response(resp, resp.json(), url, method)
+            try:
+                body = resp.json()
+            except json.decoder.JSONDecodeError:
+                body = resp.text
+            raise exceptions.from_response(resp, body, url, method)
 
         do_pagination = False
 
         try:
             content = resp.json().get("content", resp.json())
         except Exception:
             do_pagination = True
@@ -215,15 +280,15 @@
 
         while not do_pagination:
             curr, next_, last = self._get_links_from_response(resp)
 
             # If we have curr, next and last this means that we are paginating
             # therefore we need to append to the "contents"
             if all([curr, next_, last]) and curr != last:
-                self.http_log_req(method, next_, kwargs)
+                self._http_log_req(method, next_, kwargs)
                 resp = self.session.request(method, next_, **kwargs)
                 self.http_log_resp(resp)
                 next_content = resp.json().get("content", [])
                 content.extend(next_content)
             else:
                 do_pagination = True
 
@@ -231,57 +296,63 @@
 
     def _get_links_from_response(self, response):
         d = {}
         for link in response.json().get("links", []):
             d[link["rel"]] = link["href"]
         return d.get("self"), d.get("next"), d.get("last")
 
-    def http_log_req(self, method, url, kwargs):
+    def _http_log_req(self, method, url, kwargs):
+        """Log a HTTP request."""
         if not self.http_debug:
             return
 
-        string_parts = ['curl -g -i']
+        string_parts = ["curl -g -i"]
 
-        if not kwargs.get('verify', True):
-            string_parts.append(' --insecure')
+        if not kwargs.get("verify", True):
+            string_parts.append(" --insecure")
 
         string_parts.append(" '%s'" % url)
-        string_parts.append(' -X %s' % method)
+        string_parts.append(" -X %s" % method)
 
-        headers = copy.deepcopy(kwargs['headers'])
-        self._redact(headers, ['Authorization'])
+        headers = copy.deepcopy(kwargs["headers"])
+        self._redact(headers, ["Authorization"])
         # because dict ordering changes from 2 to 3
         keys = sorted(headers.keys())
         for name in keys:
             value = headers[name]
             header = ' -H "%s: %s"' % (name, value)
             string_parts.append(header)
 
-        if 'data' in kwargs:
-            data = json.loads(kwargs['data'])
+        if "data" in kwargs:
+            data = json.loads(kwargs["data"])
             string_parts.append(" -d '%s'" % json.dumps(data))
         self._logger.debug("REQ: %s" % "".join(string_parts))
 
-    def http_log_resp(self, resp):
+    def _http_log_resp(self, resp):
+        """Log a HTTP response."""
         if not self.http_debug:
             return
 
         if resp.text and resp.status_code != 400:
             try:
                 body = json.loads(resp.text)
-                self._redact(body, ['access', 'token', 'id'])
+                self._redact(body, ["access", "token", "id"])
             except ValueError:
                 body = None
         else:
             body = None
 
-        self._logger.debug("RESP: [%(status)s] %(headers)s\nRESP BODY: "
-                           "%(text)s\n", {'status': resp.status_code,
-                                          'headers': resp.headers,
-                                          'text': json.dumps(body)})
+        self._logger.debug(
+            "RESP: [%(status)s] %(headers)s\nRESP BODY: " "%(text)s\n",
+            {
+                "status": resp.status_code,
+                "headers": resp.headers,
+                "text": json.dumps(body),
+            },
+        )
 
     def _redact(self, target, path, text=None):
         """Replace the value of a key in `target`.
 
         The key can be at the top level by specifying a list with a single
         key as the path. Nested dictionaries are also supported by passing a
         list of keys to be navigated to find the one that should be replaced.
@@ -292,67 +363,66 @@
         :param list path: a list representing the nested structure in `target`
                           that should be redacted; modified in place
         :param string text: optional text to use as a replacement for the
                             redacted key. if text is not specified, the
                             default text will be sha1 hash of the value being
                             redacted
         """
-
         key = path.pop()
 
         # move to the most nested dict
         for p in path:
             try:
                 target = target[p]
             except KeyError:
                 return
 
         if key in target:
             if text:
                 target[key] = text
             elif target[key] is not None:
                 # because in python3 byte string handling is ... ug
-                value = target[key].encode('utf-8')
+                value = target[key].encode("utf-8")
                 sha1sum = hashlib.sha1(value)  # nosec
                 target[key] = "{SHA1}%s" % sha1sum.hexdigest()
 
     def head(self, url, **kwargs):
         """Perform a HEAD request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``HEAD``.
         """
-        return self.request(url, 'HEAD', **kwargs)
+        return self.request(url, "HEAD", **kwargs)
 
     def get(self, url, **kwargs):
         """Perform a GET request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``GET``.
         """
-        return self.request(url, 'GET', **kwargs)
+        return self.request(url, "GET", **kwargs)
 
     def post(self, url, **kwargs):
         """Perform a POST request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``POST``.
         """
-        return self.request(url, 'POST', **kwargs)
+        return self.request(url, "POST", **kwargs)
 
     def put(self, url, **kwargs):
         """Perform a PUT request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``PUT``.
         """
-        return self.request(url, 'PUT', **kwargs)
+        return self.request(url, "PUT", **kwargs)
 
     def delete(self, url, **kwargs):
         """Perform a DELETE request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``DELETE``.
         """
-        return self.request(url, 'DELETE', **kwargs)
+        return self.request(url, "DELETE", **kwargs)
 
     def patch(self, url, **kwargs):
         """Perform a PATCH request.
 
         This calls :py:meth:`.request()` with ``method`` set to ``PATCH``.
         """
-        return self.request(url, 'PATCH', **kwargs)
+        return self.request(url, "PATCH", **kwargs)
```

### Comparing `orpy-1.0.2/orpy/client/config.py` & `orpy-1.0.4/orpy/client/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,33 +10,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""This module contains the client dealing with PaaS Orchestrator configuration."""
+
 from orpy.client import base
 from orpy import exceptions
 
 
 class Config(object):
     """Get configured endpoints for the Orchestrator."""
 
     def __init__(self, client):
+        """Initialize client.
+
+        :params client: An instance of OrpyClient.
+        """
         self.client = client
 
-    def get(self):
+    def get(self, **kwargs):
         """Get Configurted endpoints for the orchestrator.
 
+        :param kwargs: Other arguments passed to the request client.
+
         :return: Configured endpoints for the orchestrator.
         :rtype: orpy.client.base.OrchestratorConfiguration
         """
         try:
-            resp, body = self.client.get("./configuration")
-        except exceptions.ClientException:
-            raise exceptions.InvalidUrl(url=self.client.url)
+            resp, body = self.client.get("./configuration", **kwargs)
+        except exceptions.ClientError:
+            raise exceptions.InvalidUrlError(url=self.client.url)
 
         if resp.status_code == 200:
             body["url"] = self.client.url
             return base.OrchestratorInfo(body)
         else:
-            raise exceptions.InvalidUrl(url=self.client.url)
+            raise exceptions.InvalidUrlError(url=self.client.url)
```

### Comparing `orpy-1.0.2/orpy/client/deployments.py` & `orpy-1.0.4/orpy/client/deployments.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,115 +10,139 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""This module contains the client dealing with PaaS Orchestrator deployments."""
+
 from orpy.client import base
 
 
 class Deployments(object):
     """Manage Orchestrator deployments."""
 
     def __init__(self, client):
+        """Initialize client.
+
+        :params client: An instance of OrpyClient.
+        """
         self.client = client
 
-    def list(self):
+    def list(self, **kwargs):
         """List existing deployments.
 
+        :param kwargs: Other arguments passed to the request client.
+
         :return: List of orpy.client.base.Deployment
         :rtype: list
         """
-        resp, results = self.client.get("./deployments")
+        resp, results = self.client.get("./deployments", **kwargs)
         return [base.Deployment(data) for data in results]
 
-    def show(self, uuid):
+    def show(self, uuid, **kwargs):
         """Show details about a deployment.
 
         :param str uuid: The UUID of the deployment to show.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: The deployment requested
         :rtype: orpy.client.base.Deployment
         """
-        resp, result = self.client.get("./deployments/%s" % uuid)
+        resp, result = self.client.get("./deployments/%s" % uuid, **kwargs)
         return base.Deployment(result)
 
-    def delete(self, uuid):
+    def delete(self, uuid, **kwargs):
         """Delete a deployment.
 
         :param str uuid: The UUID of the deployment to delete.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: None
         :rtype: None
         """
-        resp, body = self.client.delete("./deployments/%s" % uuid)
+        resp, body = self.client.delete("./deployments/%s" % uuid, **kwargs)
         return
 
-    def get_template(self, uuid):
+    def get_template(self, uuid, **kwargs):
         """Get the TOSCA template of a deployment.
 
         :param str uuid: The UUID of the deployment.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: The TOSCA template for the deployment
         :rtype: orpy.client.base.TOSCATemplate
         """
-        resp, result = self.client.get("./deployments/%s/template/" % uuid)
-        info = {"template": result,
-                "uuid": uuid}
+        resp, result = self.client.get("./deployments/%s/template/" % uuid, **kwargs)
+        info = {"template": result}
         return base.TOSCATemplate(info)
 
-    def create(self, template, callback_url=None, max_providers_retry=None,
-               keep_last_attemp=True, parameters={}):
+    def create(
+        self,
+        template,
+        callback_url=None,
+        max_providers_retry=None,
+        keep_last_attemp=True,
+        parameters=None,
+        **kwargs,
+    ):
         """Create a deployment.
 
         :param str template: The TOSCA template to use.
         :param str callback_url: The orchestrator callback url.
         :param int max_providers_retry: Maximum number of providers to retry.
         :param bool keep_last_attemp: Whether to keep the allocated resources
                                       in case of failure.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: The created deployment
         :rtype: orpy.client.base.Deployment
         """
         json = {
             "template": template,
             "keepLastAttemp": keep_last_attemp,
-            "parameters": parameters,
+            "parameters": parameters or {},
         }
         if callback_url:
             json["callback"] = callback_url
         if max_providers_retry:
             json["maxProvidersRetry"] = max_providers_retry
 
-        resp, result = self.client.post("./deployments/",
-                                        json=json)
+        resp, result = self.client.post("./deployments/", json=json, **kwargs)
         return base.Deployment(result)
 
-    def update(self, uuid, template, callback_url=None,
-               max_providers_retry=None, keep_last_attemp=True,
-               parameters={}):
+    def update(
+        self,
+        uuid,
+        template,
+        callback_url=None,
+        max_providers_retry=None,
+        keep_last_attemp=True,
+        parameters=None,
+        **kwargs,
+    ):
         """Update a deployment.
 
         :param str uuid: The UUID of the deployment.
         :param str template: The TOSCA template to use.
         :param str callback_url: The orchestrator callback url.
         :param int max_providers_retry: Maximum number of providers to retry.
         :param bool keep_last_attemp: Whether to keep the allocated resources
                                       in case of failure.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: The updated deployment
         :rtype: orpy.client.base.Deployment
         """
         json = {
             "template": template,
             "keepLastAttemp": keep_last_attemp,
-            "parameters": parameters,
+            "parameters": parameters or {},
         }
         if callback_url:
             json["callback"] = callback_url
         if max_providers_retry:
             json["maxProvidersRetry"] = max_providers_retry
 
-        resp, result = self.client.put("./deployments/%s" % uuid,
-                                       json=json)
+        resp, result = self.client.put("./deployments/%s" % uuid, json=json, **kwargs)
         return base.Deployment(result)
```

### Comparing `orpy-1.0.2/orpy/client/info.py` & `orpy-1.0.4/orpy/_cmd/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,33 +10,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from orpy.client import base
-from orpy import exceptions
 
+from cliff import show
 
-class Info(object):
-    """Get information about the Orchestrator."""
+from orpy import utils
 
-    def __init__(self, client):
-        self.client = client
-
-    def get(self):
-        """Get information about the Orchestrator.
-
-        :return: Information about the orchestrator.
-        :rtype: orpy.client.base.OrchestratorInfo
-        """
-        try:
-            resp, body = self.client.get("./info")
-        except exceptions.ClientException:
-            raise exceptions.InvalidUrl(url=self.client.url)
-
-        if resp.status_code == 200:
-            body["url"] = self.client.url
-            return base.OrchestratorInfo(body)
-        else:
-            raise exceptions.InvalidUrl(url=self.client.url)
+
+class OrchestratorEndpointInfo(show.ShowOne):
+    """Test if the given URL is pointing to an orchestrator.
+
+    Use this command to check if the URL provided is actually from an INDIGO
+    PaaS Orchestrator.
+    """
+
+    auth_required = False
+
+    def take_action(self, parsed_args):
+        """Execute command."""
+        d = self.app.client.info.get(authenticated=self.auth_required).to_dict()
+        for k, v in d.items():
+            if isinstance(v, dict):
+                d[k] = utils.format_dict(v)
+        return self.dict2columns(d)
```

### Comparing `orpy-1.0.2/orpy/client/resources.py` & `orpy-1.0.4/orpy/client/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,39 +10,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""This module contains the client dealing with PaaS Orchestrator resources."""
+
 from orpy.client import base
 
 
 class Resources(object):
     """Manage Orchestrator deployment resources."""
 
     def __init__(self, client):
+        """Initialize client.
+
+        :params client: An instance of OrpyClient.
+        """
         self.client = client
 
-    def list(self, uuid):
+    def list(self, uuid, **kwargs):
         """List resources for a deployment.
 
         :param str uuid: The UUID of the deployment get the resources.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: A list of orpy.client.base.Resource
         :rtype: list
         """
-        resp, results = self.client.get("./deployments/%s/resources/" % uuid)
+        resp, results = self.client.get("./deployments/%s/resources/" % uuid, **kwargs)
         return [base.Resource(result) for result in results]
 
-    def show(self, deployment_uuid, resource_uuid):
+    def show(self, deployment_uuid, resource_uuid, **kwargs):
         """Show details about a resource on a deployment.
 
         :param str resource_uuid: The UUID of the deployment get the resource.
         :param str deployment_uuid: The UUID of the resource.
+        :param kwargs: Other arguments passed to the request client.
 
         :return: The resource requested
         :rtype: orpy.client.base.Resource
         """
-        resp, result = self.client.get("./deployments/%s/resources/%s" %
-                                       (deployment_uuid, resource_uuid))
+        resp, result = self.client.get(
+            "./deployments/%s/resources/%s" % (deployment_uuid, resource_uuid), **kwargs
+        )
         return base.Resource(result)
```

### Comparing `orpy-1.0.2/orpy/cmd/config.py` & `orpy-1.0.4/orpy/_cmd/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 class OrchestratorConfigShow(show.ShowOne):
     """Show current orchestrator endpoints configured.
 
     Use this command to get the list of endpoints that the current orchrestator
     is using.
     """
 
-    auth_required = False
+    auth_required = True
 
     def take_action(self, parsed_args):
-        d = self.app.client.config.get().to_dict()
+        """Execute command."""
+        d = self.app.client.config.get(authenticated=self.auth_required).to_dict()
         for k, v in d.items():
             if isinstance(v, dict):
                 d[k] = utils.format_dict(v)
         return self.dict2columns(d)
-
```

### Comparing `orpy-1.0.2/orpy/cmd/deployments.py` & `orpy-1.0.4/orpy/_cmd/deployments.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,67 +26,75 @@
 class KeyValueAction(argparse.Action):
     """A custom action to parse arguments as key=value pairs.
 
     Ensures that ``dest`` is a dict.
     """
 
     def __call__(self, parser, namespace, values, option_string=None):
+        """Call the action."""
         # Make sure we have an empty dict rather than None
         if getattr(namespace, self.dest, None) is None:
             setattr(namespace, self.dest, {})
 
         for v in values:
-            v = v.split('=', 1)
+            v = v.split("=", 1)
             # NOTE(qtang): Prevent null key setting in property
-            if '' == v[0]:
+            if "" == v[0]:
                 msg = "Property key must be specified: %s"
                 raise argparse.ArgumentTypeError(msg % str(values))
             else:
                 getattr(namespace, self.dest, {}).update([v])
 
 
 class DeploymentList(lister.Lister):
     """List existing deployments at orchestrator."""
 
     # TODO(aloga): implement filters
 
     def take_action(self, parsed_args):
+        """Execute command."""
         ret = self.app.client.deployments.list()
 
         columns = (
-            'uuid',
-            'status',
-            'task',
-            'creationTime',
-            'createdBy',
-            'cloudProviderName'
+            "uuid",
+            "status",
+            "task",
+            "creationTime",
+            "createdBy",
+            "cloudProviderName",
         )
 
-        values = [utils.get_item_properties(s, columns,
-                                            mixed_case_fields=columns)
-                  for s in ret]
+        values = [
+            utils.get_item_properties(s, columns, mixed_case_fields=columns)
+            for s in ret
+        ]
 
         return columns, values
 
 
 class DeploymentShow(show.ShowOne):
     """Show details about an existing deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(DeploymentShow, self).get_parser(prog_name)
-        parser.add_argument('uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID to show.")
-        parser.add_argument('-l', '--long',
-                            action="store_true",
-                            default=False,
-                            help="Show additional fields in output.")
+        parser.add_argument(
+            "uuid", metavar="<deployment uuid>", help="Deployment UUID to show."
+        )
+        parser.add_argument(
+            "-l",
+            "--long",
+            action="store_true",
+            default=False,
+            help="Show additional fields in output.",
+        )
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         d = self.app.client.deployments.show(parsed_args.uuid).to_dict()
 
         is_table = parsed_args.formatter == "table"
 
         if not parsed_args.long:
             rm = [
                 "links",
@@ -99,146 +107,164 @@
 
         if is_table:
             links = {}
             for i in d["links"]:
                 links[i["rel"]] = i["href"]
 
             d["links"] = utils.format_dict(links)
-            d["cloudProviderEndpoint"] = utils.format_dict(
-                d["cloudProviderEndpoint"]
-            )
+            d["cloudProviderEndpoint"] = utils.format_dict(d["cloudProviderEndpoint"])
             d["createdBy"] = utils.format_dict(d["createdBy"])
 
         return self.dict2columns({k: v for k, v in d.items() if k not in rm})
 
 
 class DeploymentDelete(command.Command):
     """Show details about an existing deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(DeploymentDelete, self).get_parser(prog_name)
-        parser.add_argument('uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID to delete.")
+        parser.add_argument(
+            "uuid", metavar="<deployment uuid>", help="Deployment UUID to delete."
+        )
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         self.app.client.deployments.delete(parsed_args.uuid)
 
 
 class DeploymentGetTemplate(show.ShowOne):
     """Get template used for a given deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(DeploymentGetTemplate, self).get_parser(prog_name)
-        parser.add_argument('uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID to get template for.")
+        parser.add_argument(
+            "uuid",
+            metavar="<deployment uuid>",
+            help="Deployment UUID to get template for.",
+        )
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         d = self.app.client.deployments.get_template(parsed_args.uuid)
         return self.dict2columns(d.to_dict())
 
 
 class DeploymentCreate(show.ShowOne):
     """Create a deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(DeploymentCreate, self).get_parser(prog_name)
 
-        parser.add_argument("--callback-url",
-                            dest="callback",
-                            default=None,
-                            help="The callback url.")
-        parser.add_argument("--max-providers-retry",
-                            dest="max_retries",
-                            default=None,
-                            type=int,
-                            help="Maximum number of cloud providers to be "
-                                 "used in case of failure (Default is to "
-                                 "be unbounded).")
-        parser.add_argument("--keep-last-attempt",
-                            dest="keep_last",
-                            default=True,
-                            type=bool,
-                            help="In case of failure, keep the resources "
-                                 "allocated in the last try (Default: True, "
-                                 "accepts boolean values).")
-
-        parser.add_argument('filename',
-                            metavar="<template file>",
-                            help="TOSCA template file.")
-
-        parser.add_argument('parameters',
-                            metavar="<parameter>=<value>",
-                            nargs="*",
-                            action=KeyValueAction,
-                            help="Input parameter for the deployment in the "
-                                 "form <parameter>=<value>. Can be specified "
-                                 "several times.")
+        parser.add_argument(
+            "--callback-url", dest="callback", default=None, help="The callback url."
+        )
+        parser.add_argument(
+            "--max-providers-retry",
+            dest="max_retries",
+            default=None,
+            type=int,
+            help="Maximum number of cloud providers to be "
+            "used in case of failure (Default is to "
+            "be unbounded).",
+        )
+        parser.add_argument(
+            "--keep-last-attempt",
+            dest="keep_last",
+            default=True,
+            type=bool,
+            help="In case of failure, keep the resources "
+            "allocated in the last try (Default: True, "
+            "accepts boolean values).",
+        )
+
+        parser.add_argument(
+            "filename", metavar="<template file>", help="TOSCA template file."
+        )
+
+        parser.add_argument(
+            "parameters",
+            metavar="<parameter>=<value>",
+            nargs="*",
+            action=KeyValueAction,
+            help="Input parameter for the deployment in the "
+            "form <parameter>=<value>. Can be specified "
+            "several times.",
+        )
 
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         with open(parsed_args.filename, "r") as f:
             d = self.app.client.deployments.create(
                 template=f.read(),
                 callback_url=parsed_args.callback,
                 max_providers_retry=parsed_args.max_retries,
                 keep_last_attemp=parsed_args.keep_last,
-                parameters=parsed_args.parameters
+                parameters=parsed_args.parameters,
             )
         return self.dict2columns(d.to_dict())
 
 
 class DeploymentUpdate(show.ShowOne):
     """Update an existing deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(DeploymentUpdate, self).get_parser(prog_name)
 
-        parser.add_argument("--callback-url",
-                            dest="callback",
-                            default=None,
-                            help="The callback url.")
-        parser.add_argument("--max-providers-retry",
-                            dest="max_retries",
-                            default=None,
-                            type=int,
-                            help="Maximum number of cloud providers to be "
-                                 "used in case of failure (Default is to "
-                                 "be unbounded).")
-        parser.add_argument("--keep-last-attempt",
-                            dest="keep_last",
-                            default=True,
-                            type=bool,
-                            help="In case of failure, keep the resources "
-                                 "allocated in the last try (Default: True, "
-                                 "accepts boolean values).")
-
-        parser.add_argument('uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID to update.")
-        parser.add_argument('filename',
-                            metavar="<template file>",
-                            help="TOSCA template file.")
-        parser.add_argument('parameters',
-                            metavar="<parameter>=<value>",
-                            nargs="*",
-                            action=KeyValueAction,
-                            help="Input parameter for the deployment in the "
-                                 "form <parameter>=<value>. Can be specified "
-                                 "several times.")
+        parser.add_argument(
+            "--callback-url", dest="callback", default=None, help="The callback url."
+        )
+        parser.add_argument(
+            "--max-providers-retry",
+            dest="max_retries",
+            default=None,
+            type=int,
+            help="Maximum number of cloud providers to be "
+            "used in case of failure (Default is to "
+            "be unbounded).",
+        )
+        parser.add_argument(
+            "--keep-last-attempt",
+            dest="keep_last",
+            default=True,
+            type=bool,
+            help="In case of failure, keep the resources "
+            "allocated in the last try (Default: True, "
+            "accepts boolean values).",
+        )
+
+        parser.add_argument(
+            "uuid", metavar="<deployment uuid>", help="Deployment UUID to update."
+        )
+        parser.add_argument(
+            "filename", metavar="<template file>", help="TOSCA template file."
+        )
+        parser.add_argument(
+            "parameters",
+            metavar="<parameter>=<value>",
+            nargs="*",
+            action=KeyValueAction,
+            help="Input parameter for the deployment in the "
+            "form <parameter>=<value>. Can be specified "
+            "several times.",
+        )
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         with open(parsed_args.filename, "r") as f:
             d = self.app.client.deployments.update(
                 uuid=parsed_args.uuid,
                 template=f.read(),
                 callback_url=parsed_args.callback,
                 max_providers_retry=parsed_args.max_retries,
                 keep_last_attemp=parsed_args.keep_last,
-                parameters=parsed_args.parameters
+                parameters=parsed_args.parameters,
             )
         return self.dict2columns(d.to_dict())
```

### Comparing `orpy-1.0.2/orpy/cmd/resources.py` & `orpy-1.0.4/orpy/_cmd/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,51 +20,59 @@
 from orpy import utils
 
 
 class ResourcesList(lister.Lister):
     """List Resources for a given deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(ResourcesList, self).get_parser(prog_name)
-        parser.add_argument('uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID to show.")
+        parser.add_argument(
+            "uuid", metavar="<deployment uuid>", help="Deployment UUID to show."
+        )
         return parser
 
     def take_action(self, parsed_args):
+        """Execute command."""
         ret = self.app.client.resources.list(parsed_args.uuid)
 
         columns = (
-            'uuid',
-            'state',
-            'toscaNodeType',
-            'toscaNodeName',
-            'creationTime',
-            'requiredBy',
+            "uuid",
+            "state",
+            "toscaNodeType",
+            "toscaNodeName",
+            "creationTime",
+            "requiredBy",
         )
 
-        values = [utils.get_item_properties(s, columns,
-                                            mixed_case_fields=columns)
-                  for s in ret]
+        values = [
+            utils.get_item_properties(s, columns, mixed_case_fields=columns)
+            for s in ret
+        ]
 
         return columns, values
 
 
 class ResourcesShow(show.ShowOne):
     """Show details about a resource for a given deployment."""
 
     def get_parser(self, prog_name):
+        """Return parser for the command."""
         parser = super(ResourcesShow, self).get_parser(prog_name)
-        parser.add_argument('deployment_uuid',
-                            metavar="<deployment uuid>",
-                            help="Deployment UUID for the resource.")
-
-        parser.add_argument('resource_uuid',
-                            metavar="<resource uuid>",
-                            help="Resource UUID to show.")
+        parser.add_argument(
+            "deployment_uuid",
+            metavar="<deployment uuid>",
+            help="Deployment UUID for the resource.",
+        )
+
+        parser.add_argument(
+            "resource_uuid", metavar="<resource uuid>", help="Resource UUID to show."
+        )
         return parser
 
     def take_action(self, parsed_args):
-        d = self.app.client.resources.show(parsed_args.deployment_uuid,
-                                           parsed_args.resource_uuid).to_dict()
+        """Execute command."""
+        d = self.app.client.resources.show(
+            parsed_args.deployment_uuid, parsed_args.resource_uuid
+        ).to_dict()
         d.pop("links")
         return self.dict2columns(d)
```

### Comparing `orpy-1.0.2/orpy/exceptions.py` & `orpy-1.0.4/orpy/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,192 +10,228 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""This module contains all the orpy exceptions."""
+
 import sys
 
 import six
 
 
-class ClientException(Exception):
+class ClientError(Exception):
+    """Generic CLient errror."""
+
     message = "An unknown exception occurred."
 
     def __init__(self, message=None, **kwargs):
+        """Initialize the Client exception with a messsage, formatted with kwargs."""
         self.kwargs = kwargs
 
         if not message:
             try:
                 message = self.message % kwargs
             except Exception:
                 exc_info = sys.exc_info()
                 # kwargs doesn't match a variable in the message
                 # log the issue and the kwargs
-                print('Exception in string format operation')
+                print("Exception in string format operation")
                 for name, value in kwargs.iteritems():
                     print("%s: %s" % (name, value))
                 six.reraise(exc_info[0], exc_info[1], exc_info[2])
 
         message = "ERROR: " + message
-        super(ClientException, self).__init__(message)
+        super(ClientError, self).__init__(message)
+
+
+class AuthError(ClientError):
+    """Error when obtaining a token."""
 
+    message = (
+        "An exception has happened while obtaining an access token" " (err: %(err)s)"
+    )
 
-class AuthException(ClientException):
-    message = ("An exception has happened while obtaining an access token"
-               " (err: %(err)s)")
 
+class InvalidUsageError(ClientError):
+    """Invalid client usage."""
 
-class InvalidUsage(ClientException):
-    message = "Invalid client usage"
+    message = "Invalid client usage."
 
 
-class InvalidUrl(ClientException):
-    message = "URL provided is not a valid orchestrator (%(url)s)"
+class InvalidUrlError(ClientError):
+    """Invalid orchestrator URL."""
 
+    message = "URL provided is not a valid orchestrator (%(url)s)."
+
+
+class RetryAfterExceptionError(ClientError):
+    """Base class for ClientErrors that use Retry-After header."""
 
-class RetryAfterException(ClientException):
-    """Base class for ClientExceptions that use Retry-After header."""
     def __init__(self, *args, **kwargs):
+        """Initialize error, and setup retry_after attribute."""
         try:
-            self.retry_after = int(kwargs.pop('retry_after'))
+            self.retry_after = int(kwargs.pop("retry_after"))
         except (KeyError, ValueError):
             self.retry_after = 0
 
-        super(RetryAfterException, self).__init__(*args, **kwargs)
+        super(RetryAfterExceptionError, self).__init__(*args, **kwargs)
 
 
-class BadRequest(ClientException):
+class BadRequestError(ClientError):
     """HTTP 400 - Bad request.
 
     You sent some malformed data.
     """
+
     http_status = 400
     message = "Bad request"
 
 
-class Unauthorized(ClientException):
-    """HTTP 401 - Unauthorized.
+class UnauthorizedError(ClientError):
+    """HTTP 401 - UnauthorizedError.
 
     Bad credentials.
     """
+
     http_status = 401
-    message = "Unauthorized"
+    message = "UnauthorizedError"
 
 
-class Forbidden(ClientException):
-    """HTTP 403 - Forbidden.
+class ForbiddenError(ClientError):
+    """HTTP 403 - ForbiddenError.
 
     Your credentials don't give you access to this resource.
     """
+
     http_status = 403
-    message = "Forbidden"
+    message = "ForbiddenError"
 
 
-class NotFound(ClientException):
+class NotFoundError(ClientError):
     """HTTP 404 - Not found."""
+
     http_status = 404
     message = "Not found"
 
 
-class MethodNotAllowed(ClientException):
+class MethodNotAllowedError(ClientError):
     """HTTP 405 - Method Not Allowed."""
+
     http_status = 405
     message = "Method Not Allowed"
 
 
-class NotAcceptable(ClientException):
+class NotAcceptableError(ClientError):
     """HTTP 406 - Not Acceptable."""
+
     http_status = 406
     message = "Not Acceptable"
 
 
-class Conflict(ClientException):
-    """HTTP 409 - Conflict."""
+class ConflictError(ClientError):
+    """HTTP 409 - ConflictError."""
+
     http_status = 409
-    message = "Conflict"
+    message = "ConflictError"
 
 
-class OverLimit(RetryAfterException):
+class OverLimitError(RetryAfterExceptionError):
     """HTTP 413 - Over limit.
 
     You're over the API limits for this time period.
     """
+
     http_status = 413
     message = "Over limit"
 
 
-class RateLimit(RetryAfterException):
-    """HTTP 429 - Rate limit
+class RateLimitError(RetryAfterExceptionError):
+    """HTTP 429 - Rate limit.
 
     You've sent too many requests for this time period.
     """
+
     http_status = 429
     message = "Rate limit"
 
 
 # NotImplemented is a python keyword.
-class HTTPNotImplemented(ClientException):
+class HTTPNotImplementedErrorError(ClientError):
     """HTTP 501 - Not Implemented.
 
     The server does not support this operation.
     """
+
     http_status = 501
     message = "Not Implemented"
 
 
 # In Python 2.4 Exception is old-style and thus doesn't have a __subclasses__()
 # so we can do this:
 #     _code_map = dict((c.http_status, c)
-#                      for c in ClientException.__subclasses__())
+#                      for c in ClientError.__subclasses__())
 #
 # Instead, we have to hardcode it:
-_error_classes = [BadRequest, Unauthorized, Forbidden, NotFound,
-                  MethodNotAllowed, NotAcceptable, Conflict, OverLimit,
-                  RateLimit, HTTPNotImplemented]
+_error_classes = [
+    BadRequestError,
+    UnauthorizedError,
+    ForbiddenError,
+    NotFoundError,
+    MethodNotAllowedError,
+    NotAcceptableError,
+    ConflictError,
+    OverLimitError,
+    RateLimitError,
+    HTTPNotImplementedErrorError,
+]
 _code_map = dict((c.http_status, c) for c in _error_classes)
 
 
 def from_response(response, body, url, method=None):
-    """Return an instance of ClientException or subclass based on a response.
+    """Return an instance of ClientError or subclass based on a response.
 
     Usage::
 
         resp, body = requests.request(...)
         if resp.status_code != 200:
             raise exception_from_response(resp, rest.text)
     """
-    cls = _code_map.get(response.status_code, ClientException)
+    cls = _code_map.get(response.status_code, ClientError)
 
     kwargs = {
-        'code': response.status_code,
-        'method': method,
-        'url': url,
-        'request_id': None,
+        "code": response.status_code,
+        "method": method,
+        "url": url,
+        "request_id": None,
     }
 
     if body:
         message = "n/a"
         details = "n/a"
 
-        if hasattr(body, 'keys'):
+        if hasattr(body, "keys"):
             # NOTE(mriedem): WebOb<1.6.0 will return a nested dict structure
             # where the error keys to the message/details/code. WebOb>=1.6.0
             # returns just a response body as a single dict, not nested,
             # so we have to handle both cases (since we can't trust what we're
             # given with content_type: application/json either way.
-            if 'message' in body:
+            if "message" in body:
                 # WebOb 1.6.0 case
-                message = body.get('message')
-                details = body.get('details')
+                message = body.get("message")
+                details = body.get("details")
+            elif "title" in body:
+                message = body.get("title")
+                details = body.get("details")
             else:
                 # WebOb<1.6.0 where we assume there is a single error message
                 # key to the body that has the message and details.
                 error = body[list(body)[0]]
-                message = error.get('message')
-                details = error.get('details')
+                message = error.get("message")
+                details = error.get("details")
 
-        kwargs['message'] = message
-        kwargs['details'] = details
+        kwargs["message"] = message
+        kwargs["details"] = details
 
     return cls(**kwargs)
```

### Comparing `orpy-1.0.2/orpy/oidc.py` & `orpy-1.0.4/orpy/oidc.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""A module to interact with an OIDC agent."""
+
 import json
 import socket
 
 from orpy import exceptions
 from orpy import utils
 
 
@@ -60,16 +62,50 @@
             while True:
                 recv = self._sock.recv(16).decode()
                 if recv:
                     data += recv
                 else:
                     break
         except socket.error as err:
-            raise exceptions.AuthExceptiob(err="Cannot communicate with the "
-                                               "oidc-agent: %s" % err)
+            raise exceptions.AuthExceptiob(
+                err="Cannot communicate with the " "oidc-agent: %s" % err
+            )
         finally:
             self._sock.close()
 
         token = json.loads(data)
         if token.get("status") == "failure":
-            raise exceptions.AuthException(err=token.get("error"))
+            raise exceptions.AuthError(err=token.get("error"))
+        return token
+
+
+class OpenIDConnectSession(object):
+    """Get the token from an object session.
+
+    This class will try to obtain the token from an object derived from the
+    requests.Session class. Namely we will get the object from the "token"
+    attribute of the session object.
+
+    This follows the approach implemented in Flask Dance Session objects, as
+    explained here [1].
+
+    [1]: https://flask-dance.readthedocs.io/en/latest/api.html#sessions
+    """
+
+    def __init__(self, session):
+        """Initialize the OpenID Connect Session.
+
+        :param session: A request.Session subclass object, containing a "token"
+                        attribute where we will obtain the access token.
+        """
+        if not (getattr(session, "token", None) and isinstance(session.token, dict)):
+            raise exceptions.InvalidUsageError("Session object is not valid")
+        self._session = session
+
+    def get_token(self):
+        """Communicate with the oidc agent and get an access token.
+
+        :returns: A dictionary containing the access token
+        :rtype: dict
+        """
+        token = self._session.token
         return token
```

### Comparing `orpy-1.0.2/orpy/shell.py` & `orpy-1.0.4/orpy/shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Module that implements the CLI."""
+
 import argparse
 import sys
 
 from cliff import app
 from cliff import command
 from cliff import commandmanager
 from cliff import complete
@@ -33,79 +35,87 @@
 class OrpyApp(app.App):
     """Command line client for the INDIGO PaaS Orchestrator.
 
     Please, before using this command put your a valid OpenID Connnect access
     token into the ORCHESTRATOR_TOKEN environment variable, so that we can use
     this token for authentication.
     """
+
     commands = []
 
     def __init__(self):
-
+        """Initialize the OrpyApp and setup the CLI."""
         self.client = None
         self.token = None
         self.oidc_agent = None
 
         # Patch command.Command to add a default auth_required = True
         command.Command.auth_required = True
 
         # Some commands do not need authentication
         help.HelpCommand.auth_required = False
         complete.CompleteCommand.auth_required = False
 
-        cm = commandmanager.CommandManager('orpy.cli')
+        cm = commandmanager.CommandManager("orpy.cli")
         super(OrpyApp, self).__init__(
             description="Command line client for the INDIGO PaaS Orchestrator",
             version=version.__version__,
             command_manager=cm,
             deferred_help=True,
         )
 
     def initialize_app(self, argv):
+        """Initialize the Cliff application."""
         for cmd in self.commands:
             self.command_manager.add_command(cmd.__name__.lower(), cmd)
 
     def prepare_to_run_command(self, cmd):
+        """Do preliminary stuff to run the command."""
         if isinstance(cmd, help.HelpCommand):
             return
 
         if not self.options.orchestrator_url:
-            self.parser.error("No URL for the orchestrator has been suplied "
-                              "use --url or set the ORCHESTRATOR_URL "
-                              "environment variable.")
-
-        if not cmd.auth_required:
-            return
-
-        if (not all([self.options.oidc_agent_sock,
-                     self.options.oidc_agent_account])) and not self.token:
-
-            self.parser.error("No oidc-agent has been set up or no access "
-                              "token has been provided, please set the "
-                              "ORCHESTRATOR_TOKEN environment variable or "
-                              "set up an oidc-agent "
-                              "(see '%s help' for more details on how "
-                              "to set up authentication)" %
-                              self.parser.prog)
-
-        self.token = utils.env("ORCHESTRATOR_TOKEN")
-
-        if self.options.oidc_agent_sock and self.options.oidc_agent_account:
-            self.oidc_agent = oidc.OpenIDConnectAgent(
-                self.options.oidc_agent_account,
-                socket_path=self.options.oidc_agent_sock
+            self.parser.error(
+                "No URL for the orchestrator has been suplied "
+                "use --url or set the ORCHESTRATOR_URL "
+                "environment variable."
             )
 
+        if cmd.auth_required:
+            if (
+                not all([self.options.oidc_agent_sock, self.options.oidc_agent_account])
+            ) and not self.token:
+
+                self.parser.error(
+                    "No oidc-agent has been set up or no access "
+                    "token has been provided, please set the "
+                    "ORCHESTRATOR_TOKEN environment variable or "
+                    "set up an oidc-agent "
+                    "(see '%s help' for more details on how "
+                    "to set up authentication)" % self.parser.prog
+                )
+
+            self.token = utils.env("ORCHESTRATOR_TOKEN", default=None)
+
+            if self.options.oidc_agent_sock and self.options.oidc_agent_account:
+                self.oidc_agent = oidc.OpenIDConnectAgent(
+                    self.options.oidc_agent_account,
+                    socket_path=self.options.oidc_agent_sock,
+                )
+
         if self.client is None:
-            self.client = client.OrpyClient(self.options.orchestrator_url,
-                                            oidc_agent=self.oidc_agent,
-                                            token=self.token,
-                                            debug=self.options.debug)
+            self.client = client.OrpyClient(
+                self.options.orchestrator_url,
+                oidc_agent=self.oidc_agent,
+                token=self.token,
+                debug=self.options.debug,
+            )
 
     def build_option_parser(self, description, version):
+        """Generate and populate the option parser."""
         auth_help = """Authentication:
 
     In order to interact with the INDIGO PaaS Orchestrator we need to use an
     OpenID Connect access token from a trusted OpenID Connect provider at the
     orchestrator.
 
     Please either store your access token in 'ORCHESTRATOR_TOKEN' or set the
@@ -127,51 +137,53 @@
 """
         parser = super(OrpyApp, self).build_option_parser(
             self.__doc__,
             version,
             argparse_kwargs={
                 "formatter_class": argparse.RawDescriptionHelpFormatter,
                 "epilog": auth_help,
-            })
+            },
+        )
 
         parser.add_argument(
-            '--oidc-agent-sock',
-            metavar='<oidc-agent-socket>',
-            dest='oidc_agent_sock',
-            default=utils.env('OIDC_SOCK'),
-            help='The path for the oidc-agent socket to use to get and renew '
-                 'access tokens from the OpenID Connect provider. This '
-                 'defaults to the OIDC_SOCK environment variable, that should '
-                 'be automatically set up if you are using oidc-agent. '
-                 'In order to use the oidc-agent you must also pass the '
-                 '--oidc-agent-account parameter, or set the OIDC_ACCOUNT '
-                 'environment variable.'
+            "--oidc-agent-sock",
+            metavar="<oidc-agent-socket>",
+            dest="oidc_agent_sock",
+            default=utils.env("OIDC_SOCK"),
+            help="The path for the oidc-agent socket to use to get and renew "
+            "access tokens from the OpenID Connect provider. This "
+            "defaults to the OIDC_SOCK environment variable, that should "
+            "be automatically set up if you are using oidc-agent. "
+            "In order to use the oidc-agent you must also pass the "
+            "--oidc-agent-account parameter, or set the OIDC_ACCOUNT "
+            "environment variable.",
         )
         parser.add_argument(
-            '--oidc-agent-account',
-            metavar='<oidc-agent-account>',
-            dest='oidc_agent_account',
-            default=utils.env('OIDC_ACCOUNT'),
-            help='The oidc-agent account that we will use to get tokens from. '
-                 'In order to use the oidc-agent you must pass thos parameter '
-                 'or set the OIDC_ACCOUNT environment variable.'
+            "--oidc-agent-account",
+            metavar="<oidc-agent-account>",
+            dest="oidc_agent_account",
+            default=utils.env("OIDC_ACCOUNT"),
+            help="The oidc-agent account that we will use to get tokens from. "
+            "In order to use the oidc-agent you must pass thos parameter "
+            "or set the OIDC_ACCOUNT environment variable.",
         )
         parser.add_argument(
-            '--url',
-            metavar='<orchestrator-url>',
-            dest='orchestrator_url',
-            default=utils.env('ORCHESTRATOR_URL'),
-            help='The base url of the orchestrator rest interface. '
-                 'Alternative the environment variable ORCHESTRATOR_URL '
-                 'can be used.'
+            "--url",
+            metavar="<orchestrator-url>",
+            dest="orchestrator_url",
+            default=utils.env("ORCHESTRATOR_URL"),
+            help="The base url of the orchestrator rest interface. "
+            "Alternative the environment variable ORCHESTRATOR_URL "
+            "can be used.",
         )
 
         return parser
 
 
 def main(argv=sys.argv[1:]):
+    """Execute the main program."""
     orpy = OrpyApp()
     return orpy.run(argv)
 
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv[1:]))
```

### Comparing `orpy-1.0.2/orpy/tests/base.py` & `orpy-1.0.4/orpy/tests/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Base classes for all tests."""
+
 import os
 
 import fixtures
 import testtools
 
-_TRUE_VALUES = ('True', 'true', '1', 'yes')
+_TRUE_VALUES = ("True", "true", "1", "yes")
 
 
 class TestCase(testtools.TestCase):
-
     """Test case base class for all unit tests."""
 
     def setUp(self):
         """Run before each test method to initialize test environment."""
-
         super(TestCase, self).setUp()
-        test_timeout = os.environ.get('OS_TEST_TIMEOUT', 0)
+        test_timeout = os.environ.get("OS_TEST_TIMEOUT", 0)
         try:
             test_timeout = int(test_timeout)
         except ValueError:
             # If timeout value is invalid do not set a timeout.
             test_timeout = 0
         if test_timeout > 0:
             self.useFixture(fixtures.Timeout(test_timeout, gentle=True))
 
         self.useFixture(fixtures.NestedTempfile())
         self.useFixture(fixtures.TempHomeDir())
 
-        if os.environ.get('OS_STDOUT_CAPTURE') in _TRUE_VALUES:
-            stdout = self.useFixture(fixtures.StringStream('stdout')).stream
-            self.useFixture(fixtures.MonkeyPatch('sys.stdout', stdout))
-        if os.environ.get('OS_STDERR_CAPTURE') in _TRUE_VALUES:
-            stderr = self.useFixture(fixtures.StringStream('stderr')).stream
-            self.useFixture(fixtures.MonkeyPatch('sys.stderr', stderr))
+        if os.environ.get("OS_STDOUT_CAPTURE") in _TRUE_VALUES:
+            stdout = self.useFixture(fixtures.StringStream("stdout")).stream
+            self.useFixture(fixtures.MonkeyPatch("sys.stdout", stdout))
+        if os.environ.get("OS_STDERR_CAPTURE") in _TRUE_VALUES:
+            stderr = self.useFixture(fixtures.StringStream("stderr")).stream
+            self.useFixture(fixtures.MonkeyPatch("sys.stderr", stderr))
 
         self.log_fixture = self.useFixture(fixtures.FakeLogger())
```

### Comparing `orpy-1.0.2/orpy/tests/test_orpy.py` & `orpy-1.0.4/orpy/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,21 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-"""
-test_orpy
-----------------------------------
-
-Tests for `orpy` module.
-"""
-
-from orpy.tests import base
-
-
-class TestOrpy(base.TestCase):
-
-    def test_something(self):
-        pass
+"""orpy is an INDIGO-PaaS orchestrator client."""
```

### Comparing `orpy-1.0.2/orpy/utils.py` & `orpy-1.0.4/orpy/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Miscelaneous utilities."""
+
 import os
 
 import six
 
 
 def env(*vars, **kwargs):
-    """Search for the first defined of possibly many env vars
+    """Search for the first defined of possibly many env vars.
 
     Returns the first environment variable defined in vars, or
     returns the default defined in kwargs.
     """
     for v in vars:
         value = os.environ.get(v, None)
         if value:
             return value
-    return kwargs.get('default', '')
+    return kwargs.get("default", "")
 
 
 def get_item_properties(item, fields, mixed_case_fields=None):
     """Return a tuple containing the item properties.
 
     :param item: a single item resource (e.g. Server, Project, etc)
     :param fields: tuple of strings with the desired field names
@@ -42,37 +44,40 @@
     if mixed_case_fields is None:
         mixed_case_fields = []
 
     row = []
 
     for field in fields:
         if field in mixed_case_fields:
-            field_name = field.replace(' ', '')
+            field_name = field.replace(" ", "")
         else:
-            field_name = field.lower().replace(' ', '')
+            field_name = field.lower().replace(" ", "")
 
-        data = getattr(item, field_name, '')
+        data = getattr(item, field_name, "")
         if isinstance(data, dict):
             data = format_dict(data)
 
         row.append(data)
     return tuple(row)
 
 
 def format_list_of_dicts(data, sep="\n"):
+    """Format a list of dicts into a string.
+
+    :param sep: Separator to join the different dicts on.
+    """
     return sep.join([format_dict(d) for d in data])
 
 
 def format_dict(data):
-    """Return a formatted string of key value pairs
+    """Return a formatted string of key value pairs.
 
     :param data: a dict
     :rtype: a string formatted to key='value'
     """
-
     if data is None:
         return None
 
     output = ""
     for s in sorted(data):
         output = output + s + ": " + six.text_type(data[s]) + "\n"
     return output[:-2]
```

### Comparing `orpy-1.0.2/orpy/version.py` & `orpy-1.0.4/orpy/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import pbr
+"""Module that deals with versions."""
 
-version_info = pbr.version.VersionInfo('orpy')
+import pbr.version
+
+version_info = pbr.version.VersionInfo("orpy")
 try:
     __version__ = version_info.version_string()
     __release__ = version_info.release_string()
 except AttributeError:
     __version__ = None
     __release__ = None
```

### Comparing `orpy-1.0.2/orpy.egg-info/PKG-INFO` & `orpy-1.0.4/orpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,17 @@
 Metadata-Version: 2.1
 Name: orpy
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python library and CLI for the INDIGO PaaS Orchestrator.
 Home-page: https://github.com/indigo-dc/orpy
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/indigo-dc/orpy/issues
 Project-URL: Documentation, https://orpy.readthedocs.io/
-Description: # orpy
-        
-        Python library and CLI for the INDIGO PaaS Orchestrator.
-        
-        <img src="https://marketplace.deep-hybrid-datacloud.eu/images/logo-deep.png" width=200 alt="DEEP-Hybrid-DataCloud logo"/>
-        
-        * Free software: Apache License 2.0
-        * Source: https://github.com/indigo-dc/orpy
-        * Documentation: https://orpy.readthedocs.io/
-        * Bugs: https://github.com/indigo-dc/orpy/issues
-        
-        ## Installation.
-        
-        You can install it directly from PyPI:
-        
-            pip install orpy
-        
-        ## Usage as CLI
-        
-        Before using the orchestrator with orpy you need to export your IAM access
-        token. As long as the access token is valid orchent can tell the orchestrator
-        what to do.
-        
-            export ORCHESTRATOR_TOKEN=<your access token here>
-        
-        Please check the [documentation](https://docs.deep-hybrid-datacloud.eu/projects/orpy/en/stable/user/shell.html)
-        for more details on how to set the credentials.
-        
-        Then, the usage is as follows:
-        
-            usage: orpy [--version] [-v | -q] [--log-file LOG_FILE] [-h] [--debug]
-                       [--url <orchestrator-url>]
-        
-            Command line client for the INDIGO PaaS Orchestrator.
-        
-                Please, before using this command put your a valid OpenID Connnect access
-                token into the ORCHESTRATOR_TOKEN environment variable, so that we can use
-                this token for authentication.
-        
-        
-            optional arguments:
-              --version             show program's version number and exit
-              -v, --verbose         Increase verbosity of output. Can be repeated.
-              -q, --quiet           Suppress output except warnings and errors.
-              --log-file LOG_FILE   Specify a file to log output. Disabled by default.
-              -h, --help            Show help message and exit.
-              --debug               Show tracebacks on errors.
-              --url <orchestrator-url>
-                                    The base url of the orchestrator rest interface.
-                                    Alternative the environment variable ORCHESTRATOR_URL
-                                    can be used.
-        
-            Commands:
-              complete       print bash completion command (cliff)
-              dep create     Create a deployment.
-              dep delete     Show details about an existing deployment.
-              dep list       List existing deployments at orchestrator.
-              dep show       Show details about an existing deployment.
-              dep template   Get template used for a given deployment.
-              dep update     Update an existing deployment.
-              deployment create  Create a deployment.
-              deployment delete  Show details about an existing deployment.
-              deployment list  List existing deployments at orchestrator.
-              deployment show  Show details about an existing deployment.
-              deployment template  Get template used for a given deployment.
-              deployment update  Update an existing deployment.
-              help           print detailed help for another command (cliff)
-              resources list  List Resources for a given deployment.
-              resources show  Show details about a resource for a given deployment.
-              test           Test if the given URL is pointing to an orchestrator.
-        
-        ## Usage as API
-        
-        Besides being a CLI application, `orpy` can be used as a library:
-        
-            >>> from orpy.client import client
-            >>> orpy = client.OrpyClient(
-            ...     url=ORCHESTRATOR_URL,
-            ...     token=ORCHESTRATOR_TOKEN)
-            >>> deployments = orpy.deployments.list()
-            >>> deployments[0]
-            <Deployment cloudProviderName=provider-BARI, createdBy={u'subject': u'de28e179-ec86-4915-a748-7a37f8d80311', u'issuer': u'https://iam.deep-hybrid-datacloud.eu/'}, creationTime=2019-05-27T11:31+0000, links=[{u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005', u'rel': u'self'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/resources', u'rel': u'resources'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/template', u'rel': u'template'}], outputs={}, physicalId=11e98073-06f3-6797-9258-0242ac140005, status=CREATE_FAILED, statusReason=Error while checking the deployment status; nested exception is feign.RetryableException: mesos.ui.sav.sk executing GET https://mesos.ui.sav.sk/marathon/v2/groups/11e98073-06f3-6797-9258-0242ac140005, task=NONE, updateTime=2019-05-29T02:05+0000, uuid=11e98073-06f3-6797-9258-0242ac140005>
-            >>> deployments[0].status
-            CREATE_FAILED
-            >>>
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -109,7 +21,95 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# orpy
+
+Python library and CLI for the INDIGO PaaS Orchestrator.
+
+<img src="https://marketplace.deep-hybrid-datacloud.eu/images/logo-deep.png" width=200 alt="DEEP-Hybrid-DataCloud logo"/>
+
+* Free software: Apache License 2.0
+* Source: https://github.com/indigo-dc/orpy
+* Documentation: https://orpy.readthedocs.io/
+* Bugs: https://github.com/indigo-dc/orpy/issues
+
+## Installation.
+
+You can install it directly from PyPI:
+
+    pip install orpy
+
+## Usage as CLI
+
+Before using the orchestrator with orpy you need to export your IAM access
+token. As long as the access token is valid orchent can tell the orchestrator
+what to do.
+
+    export ORCHESTRATOR_TOKEN=<your access token here>
+
+Please check the [documentation](https://docs.deep-hybrid-datacloud.eu/projects/orpy/en/stable/user/shell.html)
+for more details on how to set the credentials.
+
+Then, the usage is as follows:
+
+    usage: orpy [--version] [-v | -q] [--log-file LOG_FILE] [-h] [--debug]
+               [--url <orchestrator-url>]
+
+    Command line client for the INDIGO PaaS Orchestrator.
+
+        Please, before using this command put your a valid OpenID Connnect access
+        token into the ORCHESTRATOR_TOKEN environment variable, so that we can use
+        this token for authentication.
+
+
+    optional arguments:
+      --version             show program's version number and exit
+      -v, --verbose         Increase verbosity of output. Can be repeated.
+      -q, --quiet           Suppress output except warnings and errors.
+      --log-file LOG_FILE   Specify a file to log output. Disabled by default.
+      -h, --help            Show help message and exit.
+      --debug               Show tracebacks on errors.
+      --url <orchestrator-url>
+                            The base url of the orchestrator rest interface.
+                            Alternative the environment variable ORCHESTRATOR_URL
+                            can be used.
+
+    Commands:
+      complete       print bash completion command (cliff)
+      dep create     Create a deployment.
+      dep delete     Show details about an existing deployment.
+      dep list       List existing deployments at orchestrator.
+      dep show       Show details about an existing deployment.
+      dep template   Get template used for a given deployment.
+      dep update     Update an existing deployment.
+      deployment create  Create a deployment.
+      deployment delete  Show details about an existing deployment.
+      deployment list  List existing deployments at orchestrator.
+      deployment show  Show details about an existing deployment.
+      deployment template  Get template used for a given deployment.
+      deployment update  Update an existing deployment.
+      help           print detailed help for another command (cliff)
+      resources list  List Resources for a given deployment.
+      resources show  Show details about a resource for a given deployment.
+      test           Test if the given URL is pointing to an orchestrator.
+
+## Usage as API
+
+Besides being a CLI application, `orpy` can be used as a library:
+
+    >>> from orpy.client import client
+    >>> orpy = client.OrpyClient(
+    ...     url=ORCHESTRATOR_URL,
+    ...     token=ORCHESTRATOR_TOKEN)
+    >>> deployments = orpy.deployments.list()
+    >>> deployments[0]
+    <Deployment cloudProviderName=provider-BARI, createdBy={u'subject': u'de28e179-ec86-4915-a748-7a37f8d80311', u'issuer': u'https://iam.deep-hybrid-datacloud.eu/'}, creationTime=2019-05-27T11:31+0000, links=[{u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005', u'rel': u'self'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/resources', u'rel': u'resources'}, {u'href': u'https://paas.cloud.cnaf.infn.it/orchestrator/deployments/11e98073-06f3-6797-9258-0242ac140005/template', u'rel': u'template'}], outputs={}, physicalId=11e98073-06f3-6797-9258-0242ac140005, status=CREATE_FAILED, statusReason=Error while checking the deployment status; nested exception is feign.RetryableException: mesos.ui.sav.sk executing GET https://mesos.ui.sav.sk/marathon/v2/groups/11e98073-06f3-6797-9258-0242ac140005, task=NONE, updateTime=2019-05-29T02:05+0000, uuid=11e98073-06f3-6797-9258-0242ac140005>
+    >>> deployments[0].status
+    CREATE_FAILED
+    >>>
+
```

### Comparing `orpy-1.0.2/orpy.egg-info/SOURCES.txt` & `orpy-1.0.4/orpy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/python-publish.yml
+.github/workflows/python-test.yml
 doc/requirements.txt
 doc/source/api.rst
 doc/source/code_of_conduct.md
 doc/source/conf.py
 doc/source/contributing.md
 doc/source/index.rst
 doc/source/installation.rst
@@ -37,26 +38,26 @@
 orpy.egg-info/SOURCES.txt
 orpy.egg-info/dependency_links.txt
 orpy.egg-info/entry_points.txt
 orpy.egg-info/not-zip-safe
 orpy.egg-info/pbr.json
 orpy.egg-info/requires.txt
 orpy.egg-info/top_level.txt
+orpy/_cmd/__init__.py
+orpy/_cmd/config.py
+orpy/_cmd/deployments.py
+orpy/_cmd/info.py
+orpy/_cmd/resources.py
 orpy/client/__init__.py
 orpy/client/base.py
 orpy/client/client.py
 orpy/client/config.py
 orpy/client/deployments.py
 orpy/client/info.py
 orpy/client/resources.py
-orpy/cmd/__init__.py
-orpy/cmd/config.py
-orpy/cmd/deployments.py
-orpy/cmd/info.py
-orpy/cmd/resources.py
 orpy/tests/__init__.py
 orpy/tests/base.py
 orpy/tests/test_orpy.py
 releasenotes/notes/initial-version-with-full-functionality-c63da317250d228d.yaml
 releasenotes/notes/new-command-configuration-show-645affdd13bfd015.yaml
 releasenotes/notes/new-long-output-ddcb9d95d1431e47.yaml
 releasenotes/notes/use-objects-bf546c89548f424c.yaml
```

### Comparing `orpy-1.0.2/orpy.egg-info/entry_points.txt` & `orpy-1.0.4/orpy.egg-info/entry_points.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [console_scripts]
 orpy = orpy.shell:main
 
 [orpy.cli]
-configuration_show = orpy.cmd.config:OrchestratorConfigShow
-dep_create = orpy.cmd.deployments:DeploymentCreate
-dep_delete = orpy.cmd.deployments:DeploymentDelete
-dep_list = orpy.cmd.deployments:DeploymentList
-dep_show = orpy.cmd.deployments:DeploymentShow
-dep_template = orpy.cmd.deployments:DeploymentGetTemplate
-dep_update = orpy.cmd.deployments:DeploymentUpdate
-deployment_create = orpy.cmd.deployments:DeploymentCreate
-deployment_delete = orpy.cmd.deployments:DeploymentDelete
-deployment_list = orpy.cmd.deployments:DeploymentList
-deployment_show = orpy.cmd.deployments:DeploymentShow
-deployment_template = orpy.cmd.deployments:DeploymentGetTemplate
-deployment_update = orpy.cmd.deployments:DeploymentUpdate
-info = orpy.cmd.info:OrchestratorEndpointInfo
-resource_list = orpy.cmd.resources:ResourcesList
-resource_show = orpy.cmd.resources:ResourcesShow
-
+configuration_show = orpy._cmd.config:OrchestratorConfigShow
+dep_create = orpy._cmd.deployments:DeploymentCreate
+dep_delete = orpy._cmd.deployments:DeploymentDelete
+dep_list = orpy._cmd.deployments:DeploymentList
+dep_show = orpy._cmd.deployments:DeploymentShow
+dep_template = orpy._cmd.deployments:DeploymentGetTemplate
+dep_update = orpy._cmd.deployments:DeploymentUpdate
+deployment_create = orpy._cmd.deployments:DeploymentCreate
+deployment_delete = orpy._cmd.deployments:DeploymentDelete
+deployment_list = orpy._cmd.deployments:DeploymentList
+deployment_show = orpy._cmd.deployments:DeploymentShow
+deployment_template = orpy._cmd.deployments:DeploymentGetTemplate
+deployment_update = orpy._cmd.deployments:DeploymentUpdate
+info = orpy._cmd.info:OrchestratorEndpointInfo
+resource_list = orpy._cmd.resources:ResourcesList
+resource_show = orpy._cmd.resources:ResourcesShow
```

### Comparing `orpy-1.0.2/setup.cfg` & `orpy-1.0.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -33,31 +33,31 @@
 packages = 
 	orpy
 
 [entry_points]
 console_scripts = 
 	orpy = orpy.shell:main
 orpy.cli = 
-	info = orpy.cmd.info:OrchestratorEndpointInfo
-	configuration_show = orpy.cmd.config:OrchestratorConfigShow
-	deployment_list = orpy.cmd.deployments:DeploymentList
-	dep_list = orpy.cmd.deployments:DeploymentList
-	deployment_show = orpy.cmd.deployments:DeploymentShow
-	dep_show = orpy.cmd.deployments:DeploymentShow
-	deployment_template = orpy.cmd.deployments:DeploymentGetTemplate
-	dep_template = orpy.cmd.deployments:DeploymentGetTemplate
-	deployment_create = orpy.cmd.deployments:DeploymentCreate
-	dep_create = orpy.cmd.deployments:DeploymentCreate
-	deployment_delete = orpy.cmd.deployments:DeploymentDelete
-	dep_delete = orpy.cmd.deployments:DeploymentDelete
-	deployment_update = orpy.cmd.deployments:DeploymentUpdate
-	dep_update = orpy.cmd.deployments:DeploymentUpdate
+	info                = orpy._cmd.info:OrchestratorEndpointInfo
+	configuration_show  = orpy._cmd.config:OrchestratorConfigShow
+	deployment_list     = orpy._cmd.deployments:DeploymentList
+	dep_list            = orpy._cmd.deployments:DeploymentList
+	deployment_show     = orpy._cmd.deployments:DeploymentShow
+	dep_show            = orpy._cmd.deployments:DeploymentShow
+	deployment_template = orpy._cmd.deployments:DeploymentGetTemplate
+	dep_template        = orpy._cmd.deployments:DeploymentGetTemplate
+	deployment_create   = orpy._cmd.deployments:DeploymentCreate
+	dep_create          = orpy._cmd.deployments:DeploymentCreate
+	deployment_delete   = orpy._cmd.deployments:DeploymentDelete
+	dep_delete          = orpy._cmd.deployments:DeploymentDelete
+	deployment_update   = orpy._cmd.deployments:DeploymentUpdate
+	dep_update          = orpy._cmd.deployments:DeploymentUpdate
 	
-	resource_list = orpy.cmd.resources:ResourcesList
-	resource_show = orpy.cmd.resources:ResourcesShow
+	resource_list       = orpy._cmd.resources:ResourcesList
+	resource_show       = orpy._cmd.resources:ResourcesShow
 
 [build_sphinx]
 source-dir = doc/source
 build-dir = doc/build
 all_files = 1
 
 [upload_sphinx]
```

### Comparing `orpy-1.0.2/setup.py` & `orpy-1.0.4/setup.py`

 * *Files identical despite different names*

