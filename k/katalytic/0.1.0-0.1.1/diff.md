# Comparing `tmp/katalytic-0.1.0.tar.gz` & `tmp/katalytic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-0.1.0.tar", last modified: Sun Apr  9 19:02:27 2023, max compression
+gzip compressed data, was "katalytic-0.1.1.tar", last modified: Fri Apr 14 18:32:44 2023, max compression
```

## Comparing `katalytic-0.1.0.tar` & `katalytic-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 19:02:27.419391 katalytic-0.1.0/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-06 18:07:34.000000 katalytic-0.1.0/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     3841 2023-04-09 19:02:27.419391 katalytic-0.1.0/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)     1579 2023-04-08 14:53:33.000000 katalytic-0.1.0/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)     1363 2023-04-09 18:13:34.000000 katalytic-0.1.0/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 19:02:27.419391 katalytic-0.1.0/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 19:02:27.419391 katalytic-0.1.0/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 19:02:27.419391 katalytic-0.1.0/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)      106 2023-04-09 06:44:10.000000 katalytic-0.1.0/src/katalytic/katalytic.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 19:02:27.419391 katalytic-0.1.0/src/katalytic.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     3841 2023-04-09 19:02:27.000000 katalytic-0.1.0/src/katalytic.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      272 2023-04-09 19:02:27.000000 katalytic-0.1.0/src/katalytic.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 19:02:27.000000 katalytic-0.1.0/src/katalytic.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)      130 2023-04-09 19:02:27.000000 katalytic-0.1.0/src/katalytic.egg-info/requires.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 19:02:27.000000 katalytic-0.1.0/src/katalytic.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 19:02:27.419391 katalytic-0.1.0/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)      875 2023-04-09 07:11:54.000000 katalytic-0.1.0/tests/test_collection.py
+-rw-r--r--   0        0        0      132 2023-04-14 18:31:54.747619 katalytic-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 18:31:54.747619 katalytic-0.1.1/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 18:31:54.747619 katalytic-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 18:31:54.747619 katalytic-0.1.1/.travis.yml
+-rw-r--r--   0        0        0      745 2023-04-14 18:32:40.164900 katalytic-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 18:31:54.747619 katalytic-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2212 2023-04-14 18:31:54.747619 katalytic-0.1.1/README.md
+-rw-r--r--   0        0        0     1779 2023-04-14 18:32:39.709128 katalytic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/pytest.sh
+-rw-r--r--   0        0        0     3107 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/venv.sh
+-rw-r--r--   0        0        0      106 2023-04-14 18:31:54.747619 katalytic-0.1.1/src/katalytic/katalytic.py
+-rw-r--r--   0        0        0      284 2023-04-14 18:31:54.747619 katalytic-0.1.1/tests/test_collection.py
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 katalytic-0.1.1/PKG-INFO
```

### Comparing `katalytic-0.1.0/LICENSE.txt` & `katalytic-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-0.1.0/README.md` & `katalytic-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
+[![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/)
+[![Build Status](https://app.travis-ci.com/katalytic/katalytic.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic)
+[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic)
+[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic?branch=main)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 ## Installation
 ```bash
 # pure
 pip install katalytic
 
 # with 3rd party dependencies
 pip install katalytic[all]
```

