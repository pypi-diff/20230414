# Comparing `tmp/zerobug-2.0.4.tar.gz` & `tmp/zerobug-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerobug-2.0.4.tar", last modified: Fri Jan 13 17:55:44 2023, max compression
+gzip compressed data, was "zerobug-2.0.5.tar", last modified: Fri Apr 14 17:10:53 2023, max compression
```

## Comparing `zerobug-2.0.4.tar` & `zerobug-2.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23939 2022-12-11 06:32:21.000000 zerobug-2.0.4/zerobug/z0testrc
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug/dummy/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/dummy/dummylib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/dummy/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4198 2023-01-13 06:05:00.000000 zerobug-2.0.4/zerobug/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2022-12-11 06:32:21.000000 zerobug-2.0.4/zerobug/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/scripts/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug/_travis/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1828 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/travis_after_tests_success
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    18750 2022-12-14 09:39:07.000000 zerobug-2.0.4/zerobug/_travis/travis_run_pypi_tests
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/coveragerc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24279 2022-12-11 06:32:21.000000 zerobug-2.0.4/zerobug/_travis/travis_install_env
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1308 2022-12-09 08:42:45.000000 zerobug-2.0.4/zerobug/_travis/build_cmd
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/_travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63820 2022-12-14 07:23:54.000000 zerobug-2.0.4/zerobug/z0testlib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      625 2022-12-11 06:32:21.000000 zerobug-2.0.4/zerobug/zerobug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.4/zerobug/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.4/zerobug.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       88 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-01-13 17:55:44.000000 zerobug-2.0.4/zerobug.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-01-13 17:55:44.000000 zerobug-2.0.4/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4198 2023-01-08 15:02:02.000000 zerobug-2.0.4/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-01-13 17:55:44.000000 zerobug-2.0.4/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15384 2023-01-13 17:55:43.000000 zerobug-2.0.4/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2595 2023-04-14 17:10:53.575899 zerobug-2.0.5/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15608 2023-04-14 17:10:52.000000 zerobug-2.0.5/README.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 17:10:53.575899 zerobug-2.0.5/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4102 2023-04-14 14:00:54.000000 zerobug-2.0.5/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.565065 zerobug-2.0.5/zerobug/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/_travis/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.5/zerobug/_travis/build_cmd
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/_travis/cfg/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/coveragerc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.5/zerobug/_travis/travis_after_tests_success
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24300 2023-04-14 17:05:13.000000 zerobug-2.0.5/zerobug/_travis/travis_install_env
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    18750 2023-04-14 17:05:20.000000 zerobug-2.0.5/zerobug/_travis/travis_run_pypi_tests
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/dummy/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/dummy/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/dummy/dummylib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-03-25 14:33:14.000000 zerobug-2.0.5/zerobug/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4102 2023-04-14 17:09:00.000000 zerobug-2.0.5/zerobug/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63946 2023-04-12 10:17:51.000000 zerobug-2.0.5/zerobug/z0testlib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23939 2023-03-25 14:33:10.000000 zerobug-2.0.5/zerobug/z0testrc
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      625 2023-03-25 14:33:05.000000 zerobug-2.0.5/zerobug/zerobug.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2595 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.5/zerobug.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       63 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zerobug-2.0.4/zerobug/z0testrc` & `zerobug-2.0.5/zerobug/z0testrc`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 # WLOGCMD:        oveerride opt_echo; may be None, 'echo', 'echo-1' or 'echo-0'
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 
-__version__=2.0.4
+__version__=2.0.5
 
 export opt_dry_run
 export ctr
 export opt_verbose
 export max_test
 export min_test
 export opt_noctr
```

### Comparing `zerobug-2.0.4/zerobug/scripts/setup.info` & `zerobug-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,37 @@
 from setuptools import find_packages, setup
 
 if sys.version_info >= (3, 0):
     install_requires = (
         [
             'future',
             'coverage',
-            'coveralls',
-            'codecov',
             'pylint-odoo',
             'python-magic',
             'python-plus',
             'os0',
             'z0lib',
         ],
     )
 else:
     install_requires = (
         [
             'future',
             'coverage',
-            'coveralls',
-            'codecov',
             'pylint-odoo<=5.0.0',
             'python-magic',
             'python-plus',
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.4',
+    version='2.0.5',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description="""
 This library can run unit test of target package software.
 Supported languages are python (through z0testlib.py) and bash (through z0testrc)
 
 zerobug supports test automation, aggregation of tests into collections
```

### Comparing `zerobug-2.0.4/zerobug/scripts/main.py` & `zerobug-2.0.5/zerobug/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `zerobug-2.0.4/zerobug/_travis/travis_after_tests_success` & `zerobug-2.0.5/zerobug/_travis/travis_after_tests_success`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import print_function
 
 import os
 import sys
 
 from coverage.cmdline import main as coverage_main
-from coveralls import cli as coveralls_cli
-from codecov import main as codecov_main
+# from coveralls import cli as coveralls_cli
+# from codecov import main as codecov_main
 
 
 def print_flush(msg):
     if sys.version_info[0] == 3:
         print(msg, flush=True)
     else:
         print(msg)
@@ -37,17 +37,17 @@
             if travis_debug_mode > 1:
                 print_flush('DEBUG: coverage report --show-missing')
             coverage_main(["report", "--show-missing"])
         else:
             if travis_debug_mode > 1:
                 print_flush('DEBUG: coverage report')
             coverage_main(["report"])
-        print_flush('DEBUG: sending result to coveralls / codecov')
-        if os.environ['TRAVIS'] == "true":
-            try:
-                coveralls_cli.main(argv=None)
-            except:
-                pass
-            try:
-                codecov_main(argv=None)
-            except:
-                pass
+        # print_flush('DEBUG: sending result to coveralls / codecov')
+        # if os.environ['TRAVIS'] == "true":
+        #     try:
+        #         coveralls_cli.main(argv=None)
+        #     except:
+        #         pass
+        #     try:
+        #         codecov_main(argv=None)
+        #     except:
+        #         pass
```

### Comparing `zerobug-2.0.4/zerobug/_travis/travis_run_pypi_tests` & `zerobug-2.0.5/zerobug/_travis/travis_run_pypi_tests`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.4
+__version__=2.0.5
 
 
 travis_test_bash() {
     echo "======== Testing test_bash   ========"
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
```

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_pr.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_70.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/coveragerc` & `zerobug-2.0.5/zerobug/_travis/cfg/coveragerc`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_flake8.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [flake8]
 # E123,E133,E226,E241,E242 are ignored by default by pep8 and flake8
 # F811 is legal in odoo 8 when we implement 2 interfaces for a method
 # F999 pylint support this case with expected tests
 # W503 changed by W504 and OCA prefers allow both
 # E203: whitespace before ':' (black behaviour and not pep8 compliant)
-ignore = E123,E133,E226,E241,E242,F811,F601,W503,W504,E203
+ignore = E117,E121,E123,E124,E126,E127,E128,E131,E133,E201,E202,E203,E211,E221,E222,E225,E226,E231,E241,E242,E251,E261,E262,E265,E266,E271,E272,W291,W292,W293,E301,E302,E303,E305,W391,F401,E501,E502,W503,W504,F601,E701,E722,F811,F841
 max-line-length = 88
 exclude =
     .svn,
     CVS,
     .bzr,
     .hg,
     .git,
```

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_61.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/cfg/travis_run_pylint_beta.cfg` & `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug/_travis/travis_install_env` & `zerobug-2.0.5/zerobug/_travis/travis_install_env`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.4
+__version__=2.0.5
 
 
 run_traced() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   local xcmd="$1" lm="                    "
@@ -369,14 +369,15 @@
 export MQT_TEST_MODE=$mode
 set_pybin $TRAVIS_PYTHON_VERSION
 install_n_activate_tools
 [[ ${TRAVIS_DEBUG_MODE:-0} -ge 2 ]] && echo "PATH=$PATH" && echo "PYTHONPATH=$PYTHONPATH"
 [[ $PIPVER -gt 18 ]] && PIP_OPTS="$PIP_OPTS --no-warn-conflicts"
 [[ $PIPVER -gt 19 ]] && PIP_OPTS="$PIP_OPTS --use-feature=2020-resolver"
 LISTREQ=$(which list_requirements.py 2>/dev/null)
+chmod -c +x $LISTREQ
 LISA=$(which lisa 2>/dev/null)
 VEM=$(which vem 2>/dev/null)
 if [[ $opt_verbose -gt 1 ]]; then
   echo -e "\e[${PS_TXT_COLOR}m$0.$__version__"
   echo -e "\e[${PS_TXT_COLOR}m\$ alias pip=$PIP.$($PIP --version)"
   echo -e "\e[${PS_TXT_COLOR}m\$ alias vem=$VEM.$($VEM -V)"
   echo -e "\e[${PS_TXT_COLOR}m\$ alias list_requirements.py=$LISTREQ.$($LISTREQ -V 2>&1)"
```

### Comparing `zerobug-2.0.4/zerobug/_travis/build_cmd` & `zerobug-2.0.5/zerobug/_travis/build_cmd`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #! /bin/bash
 # This script replaces or creates a command to test
 # \$1: source file to test
-# \$2: bin command (if not default or it does not exist)
+# \$2: fqn bin command (if not default or it does not exist)
 PYTHON=$(which python)
 PYVER=$(python --version 2>&1 | grep "Python" | grep --color=never -Eo "[0-9]" | head -n1)
 SRCPATH=$(readlink -f "$1")
 CMD="$2"
-BASE=$(basename $1)
+BASE=$(basename "$1")
 [[ -z $CMD ]] && CMD=$(which "$BASE" 2>/dev/null)
 [[ $BASE =~ .py$ ]] && BASE=${BASE:0: -3}
 [[ -z $CMD ]] && CMD=$(which "$BASE" 2>/dev/null)
 [[ -z $CMD ]] && cmd="$SRCPATH" || cmd="$CMD"
 x=$(dirname $SRCPATH)
 FROM="$(basename $x).$BASE"
 PYPATH=""
@@ -24,14 +24,15 @@
 
 if [[ $valid -eq 0 ]]; then
     echo -e "\e[1mNo command $1 found!!\e[0m"
     ln -s $1 $cmd
     chmod +x $cmd
     exit 1
 fi
+[[ $SRCPATH == $CMD ]] && chmod -c +x $SRCPATH
 echo "#!$PYTHON">$cmd
 echo "# -*- coding: utf-8 -*-">>$cmd
 echo "# Created for test use on $(date '+%Y-%m-%d %H:%M:%S')">>$cmd
 echo "import re">>$cmd
 echo "import sys">>$cmd
 echo "sys.path.insert(0, '$PYPATH')">>$cmd
 echo "from $FROM import main">>$cmd
```

### Comparing `zerobug-2.0.4/zerobug/z0testlib.py` & `zerobug-2.0.5/zerobug/z0testlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from subprocess import PIPE, Popen
 
 import magic
 
 from os0 import os0
 from python_plus import _c
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 # return code
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 if os.name == "posix":
     RED = "\033[1;31m"
     GREEN = "\033[1;32m"
@@ -35,19 +35,19 @@
     CLEAR = ''
 fail_msg = RED + "Test FAILED!" + CLEAR
 success_msg = GREEN + "Test successfully terminated" + CLEAR
 # max # of test
 MAX_TEST_NUM = 10
 # Apply for configuration file (True/False)
 APPLY_CONF = False
-# Default configuration file (i.e. myfile.conf or False for default)
+# Default configuration file (i.e. myfile.config or False for default)
 CONF_FN = None
-# Read Odoo configuration file (False or /etc/odoo-server.conf)
+# Read Odoo configuration file (False or /etc/odoo-server.config)
 ODOO_CONF = False
-# Read Odoo configuration file (False or /etc/openerp-server.conf)
+# Read Odoo configuration file (False or /etc/openerp-server.config)
 OE_CONF = False
 # Warning: set all LXs with no values -> LX=(), with 1 value -> LX=(value,)
 # List of string parameters in [options] of config file
 LX_CFG_S = ('opt_debug', 'opt_verbose', 'opt_noctr')
 # List of pure boolean parameters in [options] of config file
 LX_CFG_B = ('opt_debug', 'python2', 'python3')
 # List of string parameters in line command; may be in LX_CFG_S list too
@@ -204,40 +204,37 @@
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Counter", 0, ctx['ctr'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-r)", 0, ctx['min_test'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-z)", 0, ctx['max_test'])
         if sts == TEST_SUCCESS:
-            if os.environ.get("COVERAGE_PROCESS_START", ""):
-                tres = True
-            else:  # pragma: no cover
-                tres = False
-            sts = self.Z.test_result(z0ctx, "Opt -n (-0)", tres, ctx['opt_noctr'])
+            tres = True
+            sts = self.Z.test_result(z0ctx, "Opt -n (-Q)", tres, ctx['opt_noctr'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -B", 0, ctx['opt_debug'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Run on Top", True, ctx['run_on_top'])
         return sts
 
     def test_02(self, z0ctx):
         """Sanity autotest #2"""
-        tlog = "~/dev/z0testlib.log"
+        tlog = "~/devel/z0testlib.log"
         opts = ['-n']
         ctx = self.Z.parseoptest(opts, tlog=tlog)
         sts = self.Z.test_result(z0ctx, "Opt -n", True, ctx['dry_run'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-k)", False, ctx['opt_new'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-l)", tlog, ctx['logfn'])
         return sts
 
     def test_03(self, z0ctx):
         """Sanity autotest #3"""
-        tlog = "~/dev/z0testlib.log"
+        tlog = "~/devel/z0testlib.log"
         opts = ['-n', '-l', tlog]
         ctx = self.Z.parseoptest(opts)
         sts = self.Z.test_result(z0ctx, "Opt -n", True, ctx['dry_run'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-k)", False, ctx['opt_new'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -n (-l)", tlog, ctx['logfn'])
@@ -301,92 +298,77 @@
         sts = self.Z.test_result(z0ctx, "Opt -r 0", 0, ctx['min_test'])
         if sts == TEST_SUCCESS:
             sts = self.Z.test_result(z0ctx, "Opt -r 0 -z 13", 13, ctx['max_test'])
         return sts
 
     def test_08(self, z0ctx):
         """Sanity autotest #8"""
-        opts = []
+        opts = ["-Q"]
         ctx = self.Z.parseoptest(opts)
         ctx['WLOGCMD'] = "wecho-0"
         # sts = self.simulate_main(ctx, '1')
         sts = self.Z.main(ctx, UT=['__test_01'])
         # if os.environ.get("COVERAGE_PROCESS_START", ""):
         #     tres = 0
         # else:                                             # pragma: no cover
         tres = 1
         sts = self.Z.test_result(z0ctx, "UT", tres, ctx['max_test'])
         if sts == TEST_SUCCESS:
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '2')
             sts = self.Z.main(ctx, UT=['__test_02'])
-            # if os.environ.get("COVERAGE_PROCESS_START", ""):
-            #     tres = 0
-            # else:                                         # pragma: no cover
             tres = 2
-            sts = self.Z.test_result(z0ctx, "UT", tres, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT", tres, ctx['max_test'])
         if sts == TEST_SUCCESS:
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
-            # if os.environ.get("COVERAGE_PROCESS_START", ""):
-            #     tres = 0
-            # else:                                         # pragma: no cover
             tres = 3
-            sts = self.Z.test_result(z0ctx, "UT", tres, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT", tres, ctx['max_test'])
         if sts == TEST_SUCCESS:
             opts = ['-0']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
-            sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
             sts = self.Z.test_result(z0ctx, "UT -0", 0, ctx['max_test'])
         if sts == TEST_SUCCESS:
-            opts = ['-n']
+            opts = ['-n', '-Q']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
             tres = 3
-            sts = self.Z.test_result(z0ctx, "UT -n", tres, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT -n", tres, ctx['max_test'])
             tres = 3
-            sts = self.Z.test_result(z0ctx, "UT -n", tres, ctx['ctr'])
+            sts += self.Z.test_result(z0ctx, "UT -n", tres, ctx['ctr'])
         if sts == TEST_SUCCESS:
             opts = ['-n', '-0']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
-            sts = self.Z.test_result(z0ctx, "UT -n -0", 0, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT -n -0", 0, ctx['max_test'])
         if sts == TEST_SUCCESS:
-            opts = ['-z13', '-n']
+            opts = ['-z13', '-n', '-Q']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
             tres = 13
-            sts = self.Z.test_result(z0ctx, "UT -z13", tres, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT -z13", tres, ctx['max_test'])
             tres = 3
             sts = self.Z.test_result(z0ctx, "UT -z13", tres, ctx['ctr'])
         if sts == TEST_SUCCESS:
             opts = ['-z13', '-0']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
-            sts = self.Z.test_result(z0ctx, "UT -z13 -0", 13, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT -z13 -0", 13, ctx['max_test'])
         if sts == TEST_SUCCESS:
             opts = ['-z13', '-0', '-n']
             ctx = self.Z.parseoptest(opts)
             ctx['WLOGCMD'] = "wecho-0"
-            # sts = self.simulate_main(ctx, '3')
             sts = self.Z.main(ctx, UT=['__test_01', '__test_02'])
-            sts = self.Z.test_result(z0ctx, "UT -z13 -0 -n", 13, ctx['max_test'])
+            sts += self.Z.test_result(z0ctx, "UT -z13 -0 -n", 13, ctx['max_test'])
         return sts
 
 
 class Z0test(object):
     """The command line program to execute all tests in professional way."""
 
     def version(self):
@@ -416,27 +398,27 @@
             if os.path.isdir('./tests'):
                 self.testdir = os.path.join(self.this_dir, 'tests')
             else:
                 self.testdir = self.this_dir
             self.rundir = self.this_dir
         # Testing package dir must be the 1.st one in sys.path
         this_pkg_dir = os.path.dirname(self.rundir)
-        PYTHONPATH = os.environ.get('PYTHONPATH', '')
-        if this_pkg_dir not in sys.path:
-            if PYTHONPATH:
-                p = ':%s:' % PYTHONPATH
-                if p.find(':%s:' % this_pkg_dir) < 0:
-                    PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
-            else:
-                PYTHONPATH = this_pkg_dir
-        if this == 'test_zerobug':
-            this_pkg_dir = '%s/%s' % (self.rundir, 'dummy')
-            PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
-        os.putenv('PYTHONPATH', PYTHONPATH)
-        self.PYTHONPATH = PYTHONPATH
+        # PYTHONPATH = os.environ.get('PYTHONPATH', '')
+        # if this_pkg_dir not in sys.path:
+        #     if PYTHONPATH:
+        #         p = ':%s:' % PYTHONPATH
+        #         if p.find(':%s:' % this_pkg_dir) < 0:
+        #             PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
+        #     else:
+        #         PYTHONPATH = this_pkg_dir
+        # if this == 'test_zerobug':
+        #     this_pkg_dir = '%s/%s' % (self.rundir, 'dummy')
+        #     PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
+        # os.putenv('PYTHONPATH', PYTHONPATH)
+        # self.PYTHONPATH = PYTHONPATH
         if this_pkg_dir in sys.path:
             ix = sys.path.index(this_pkg_dir)
             del sys.path[ix]
         sys.path.insert(0, this_pkg_dir)
 
         if not id:
             if this.startswith('test_'):
@@ -460,18 +442,19 @@
             self.pattern = [self.module_id + '_test*', 'test_*']
         else:
             self.pattern = this
         # If auto regression test is executing
         self.def_tlog_fn = os.path.join(self.testdir, self.module_id + "_test.log")
         self.ctr_list = []
         if self.autorun:
-            self.ctx = self.parseoptest(argv, version=version)
+            self.z0ctx = self.parseoptest(argv, version=version)
             sys.exit(self.main())
         self.home_devel = os.environ.get("HOME_DEVEL") or os.path.expanduser("~/devel")
         self.odoo_root = os.path.dirname(self.home_devel)
+        self.z0ctx = {}
 
     def _create_parser(self, version, ctx):
         """Standard test option parser; same funcionality of bash version
         -b --debug      run test in debug mode
         -C --no-coverage run test w/o coverage
         -e --echo        set echo
         -h --help        show help
@@ -494,15 +477,15 @@
         -0 --no-count    no count # unit tests
         -1 --coverage    run test for coverage (obsoslete)
         -2               python2
         -3               python3
         """
         parser = argparse.ArgumentParser(
             description="Regression test on " + self.module_id,
-            epilog="© 2015-2022 by SHS-AV s.r.l."
+            epilog="© 2015-2023 by SHS-AV s.r.l."
             " - http://wiki.zeroincombenze.org/en/Zerobug",
         )
         parser.add_argument(
             "-B",
             "--debug",
             help="trace msgs in zerobug.tracehis",
             action="store_true",
@@ -571,14 +554,22 @@
             "--search-pattern",
             help="test file pattern",
             dest="opt_pattern",
             metavar="file_list",
             default='',
         )
         parser.add_argument(
+            "-Q",
+            "--count",
+            help="count # unit tests",
+            action="store_false",
+            dest="opt_noctr",
+            default=True,
+        )
+        parser.add_argument(
             "-q",
             "--quiet",
             help="run tests without output (quiet mode)",
             action="store_false",
             dest="opt_echo_q",
             default=True,
         )
@@ -630,23 +621,23 @@
             help="display total # tests when execute them",
             dest="max_test",
             metavar="number",
         )
         parser.add_argument(
             "-0",
             "--no-count",
-            help="no count # unit tests",
+            help="no count # unit tests (deprecated)",
             action="store_true",
             dest="opt_noctr",
-            default=False,
+            default=True,
         )
         parser.add_argument(
             "-1",
             "--coverage",
-            help="run tests for coverage (obsolete)",
+            help="run tests for coverage (deprecated)",
             action="store_true",
             dest="run4cover",
             default=True,
         )
         parser.add_argument(
             "-2",
             "--python2",
@@ -968,39 +959,39 @@
             ['sys.executable', '-m', 'doctest', file],
             stdout=FNULL,
             stderr=subprocess.STDOUT,
         )
         return self.test_result(ctx, msg, TEST_SUCCESS, res)
 
     def _exec_tests_4_count(self, test_list, ctx, TestCls=None):
-        if ctx.get('_run_autotest', False):
-            self.dbgmsg(ctx, '>>> exec_tests_4_count(autotest)')
-        else:
-            self.dbgmsg(ctx, '>>> exec_tests_4_count(%s)' % test_list)
+        # if ctx.get('_run_autotest', False):
+        #     self.dbgmsg(ctx, '>>> exec_tests_4_count(autotest)')
+        # else:
+        #     self.dbgmsg(ctx, '>>> exec_tests_4_count(%s)' % test_list)
         opt4childs = ['-n', '-R']
         ctx = self._ready_opts(ctx)
         ctx = self._save_options(ctx)
         testctr = 0
         if TestCls:
             T = TestCls(self)
             if hasattr(TestCls, 'setup'):
                 # getattr(T, 'setup')(ctx)
                 T.setup(ctx)
         for testname in test_list:
-            self.dbgmsg(
-                ctx,
-                '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
-                % (
-                    ctx['min_test'],
-                    ctx['max_test'],
-                    ctx['ctr'],
-                    ctx.get('opt_noctr', False),
-                    ctx.get('run4cover', False),
-                ),
-            )
+            # self.dbgmsg(
+            #     ctx,
+            #     '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
+            #     % (
+            #         ctx['min_test'],
+            #         ctx['max_test'],
+            #         ctx['ctr'],
+            #         ctx.get('opt_noctr', False),
+            #         ctx.get('run4cover', False),
+            #     ),
+            # )
             ctx['dry_run'] = True
             basetn = os.path.basename(testname)
             ctx['ctr'] = 0
             if testname.startswith('__test'):
                 ctx['ctr'] = int(testname[7:9])
             elif testname.startswith('__version'):
                 self.test_version(ctx, testname)
@@ -1017,88 +1008,88 @@
                         test_w_args = ['python3'] + [testname] + opt4childs
                     elif ctx.get('python2', False):
                         test_w_args = ['python2'] + [testname] + opt4childs
                     else:
                         test_w_args = [sys.executable] + [testname] + opt4childs
                 else:
                     test_w_args = [testname] + opt4childs
-                self.dbgmsg(ctx, ">>>  test_w_args=%s" % test_w_args)
+                # self.dbgmsg(ctx, ">>>  test_w_args=%s" % test_w_args)
                 p = Popen(test_w_args, stdin=PIPE, stdout=PIPE, stderr=PIPE)
                 res, err = p.communicate()
                 try:
                     ctx['ctr'] = int(res)
                 except BaseException:  # pragma: no cover
                     ctx['ctr'] = 0
                 self.ctr_list.append(ctx['ctr'])
-            self.dbgmsg(ctx, '- testctr=%d+%d' % (testctr, ctx['ctr']))
+            # self.dbgmsg(ctx, '- testctr=%d+%d' % (testctr, ctx['ctr']))
             testctr += ctx['ctr']
         if TestCls and hasattr(TestCls, 'teardown'):
             T.teardown(ctx)
         ctx = self._restore_options(ctx)
         ctx['ctr'] = testctr
         if ctx.get('max_test', 0) == 0:
             ctx['max_test'] = ctx.get('min_test', 0) + testctr
-        self.dbgmsg(
-            ctx,
-            '- c=%d, min=%d, max=%d' % (ctx['ctr'], ctx['min_test'], ctx['max_test']),
-        )
+        # self.dbgmsg(
+        #     ctx,
+        #     '- c=%d, min=%d, max=%d' % (ctx['ctr'], ctx['min_test'], ctx['max_test']),
+        # )
         ctx['_prior_msg'] = ''
         return TEST_SUCCESS
 
     def _exec_all_tests(self, test_list, ctx, TestCls=None):
-        if ctx.get('_run_autotest', False):
-            self.dbgmsg(ctx, '>>> exec_all_tests(autotest)')
-        else:
-            self.dbgmsg(ctx, '>>> exec_all_tests()')
+        # if ctx.get('_run_autotest', False):
+        #     self.dbgmsg(ctx, '>>> exec_all_tests(autotest)')
+        # else:
+        #     self.dbgmsg(ctx, '>>> exec_all_tests()')
         ctx = self._ready_opts(ctx)
         if (
             not ctx.get('_run_autotest', False)
             and ctx.get('run4cover', False)
             and not os.path.isfile(ctx['COVERAGE_PROCESS_START'])
         ):
             with open(ctx['COVERAGE_PROCESS_START'], 'w') as fd:
                 fd.write(DEFAULT_COVERARC)
         ix = 0
         sts = 0
         ctx['ctr'] = ctx['min_test']
-        self.dbgmsg(ctx, '- c=%d, ctr_list=%s' % (ctx['ctr'], self.ctr_list))
+        # self.dbgmsg(ctx, '- c=%d, ctr_list=%s' % (ctx['ctr'], self.ctr_list))
         if TestCls:
             T = TestCls(self)
         if TestCls and hasattr(TestCls, 'setup'):
             T.setup(ctx)
         for testname in test_list:
-            self.dbgmsg(
-                ctx,
-                '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
-                % (
-                    ctx['min_test'],
-                    ctx['max_test'],
-                    ctx['ctr'],
-                    ctx.get('opt_noctr', False),
-                    ctx.get('run4cover', False),
-                ),
-            )
+            # self.dbgmsg(
+            #     ctx,
+            #     '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
+            #     % (
+            #         ctx['min_test'],
+            #         ctx['max_test'],
+            #         ctx['ctr'],
+            #         ctx.get('opt_noctr', False),
+            #         ctx.get('run4cover', False),
+            #     ),
+            # )
             opt4childs = self._inherit_opts(ctx)
             basetn = os.path.basename(testname)
             if testname.startswith('__test'):
                 sts = self.test_result(ctx, testname, True, True)
             elif testname.startswith('__version'):
                 sts = self.test_version(ctx, testname)
             elif testname.startswith('__doctest'):
                 self.doctest(ctx, testname)
             elif TestCls and hasattr(TestCls, testname):
-                if ctx.get('opt_debug', False):
-                    self.dbgmsg(ctx, ">>> %s()" % testname)
+                # if ctx.get('opt_debug', False):
+                #     self.dbgmsg(ctx, ">>> %s()" % testname)
                 sts = getattr(T, testname)(ctx)
             elif os.path.splitext(basetn)[0] != ctx['this']:
                 mime = magic.Magic(mime=True).from_file(os.path.realpath(testname))
                 if os.path.dirname(testname) == "":
                     testname = os.path.join(self.testdir, testname)
                 if mime == 'text/x-python':
-                    self.dbgmsg(ctx, '- ctr=%d' % ctx['ctr'])
+                    # self.dbgmsg(ctx, '- ctr=%d' % ctx['ctr'])
                     if os.environ.get('TRAVIS_PDB') == 'true':
                         if ctx.get('python3', False):
                             test_w_args = [
                                 'python3',
                                 '-m',
                                 'pdb',
                                 testname,
@@ -1129,21 +1120,21 @@
                     else:
                         if ctx.get('python3', False):
                             test_w_args = ['python3'] + [testname] + opt4childs
                         elif ctx.get('python2', False):
                             test_w_args = ['python2'] + [testname] + opt4childs
                         else:
                             test_w_args = [sys.executable] + [testname] + opt4childs
-                    self.dbgmsg(ctx, ">>> subprocess.call(%s)" % test_w_args)
+                    # self.dbgmsg(ctx, ">>> subprocess.call(%s)" % test_w_args)
                     try:
                         sts = subprocess.call(test_w_args)
                     except OSError:
                         sts = 127
                 else:
-                    self.dbgmsg(ctx, ">>> %s(%s)" % (testname, opt4childs))
+                    # self.dbgmsg(ctx, ">>> %s(%s)" % (testname, opt4childs))
                     test_w_args = [testname] + opt4childs
                     try:
                         sts = subprocess.call(test_w_args)
                     except OSError:
                         sts = 127
                 if not ctx.get('opt_noctr', False):
                     ctx['ctr'] += self.ctr_list[ix]
@@ -1154,60 +1145,64 @@
         ctx['min_test'] = ctx['ctr']
         if TestCls and hasattr(TestCls, 'teardown'):
             T.teardown(ctx)
         return sts
 
     def main_local(self, ctx, Test, UT1=None, UT=None):
         """Default main program for local tests"""
-        self.dbgmsg(ctx, '>>> main_local(%s)' % Test)
-        test_num = 0
-        test_list = []
-        for _i in range(MAX_TEST_NUM):
-            tname = "test_{:02}".format(test_num)
-            if hasattr(Test, tname):
-                test_list.append(tname)
-            test_num += 1
+        # self.dbgmsg(ctx, '>>> main_local(%s)' % Test)
+        test_list = sorted(
+            [meth for meth in dir(Test)
+             if meth.startswith("test_") and callable(getattr(Test, meth))]
+        )
+        # test_num = 0
+        # test_list = []
+        # for _i in range(MAX_TEST_NUM):
+        #     tname = "test_{:02}".format(test_num)
+        #     if hasattr(Test, tname):
+        #         test_list.append(tname)
+        #     test_num += 1
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['max_test'])
             sts = TEST_SUCCESS
         else:
             if not ctx.get('_run_autotest', False):
                 self.set_tlog_file(ctx)
             sts = self._exec_all_tests(test_list, ctx, Test)
         return sts
 
-    def main(self, ctx=None, Test=None, UT1=None, UT=None):
+    def main(self, ctx={}, Test=None, UT1=None, UT=None):
         """Default main program for test execution
         ctx: context
         Test: test class for internal tests;
               if supplied only internal tests are executed
         UT1: protected Unit Test list (w/o log)
         UT: Unit Test list (if None, search for files)
         """
-        ctx = ctx or self.ctx
-        if (
-            ctx.get('opt_debug', False)
-            and ctx.get('run_on_top', False)
-            and not ctx.get('_run_autotest', False)
-        ):
-            self.dbgmsg(ctx, "# Test tree of %s!" % self.module_id)
-        self.dbgmsg(ctx, '>>> main()')
-        self.dbgmsg(
-            ctx,
-            '- min=%s, max=%s, -0=%s, Cover=%s'
-            % (
-                ctx.get('min_test', None),
-                ctx.get('max_test', None),
-                ctx.get('opt_noctr', False),
-                ctx.get('run4cover', False),
-            ),
-        )
+        ctx = self._ready_opts(ctx)
+        # if (
+        #     ctx.get('opt_debug', False)
+        #     and ctx.get('run_on_top', False)
+        #     and not ctx.get('_run_autotest', False)
+        # ):
+        #     self.dbgmsg(ctx, "# Test tree of %s!" % self.module_id)
+        # self.dbgmsg(ctx, '>>> main()')
+        # self.dbgmsg(
+        #     ctx,
+        #     '- min=%s, max=%s, -0=%s, Cover=%s'
+        #     % (
+        #         ctx.get('min_test', None),
+        #         ctx.get('max_test', None),
+        #         ctx.get('opt_noctr', False),
+        #         ctx.get('run4cover', False),
+        #     ),
+        # )
         # Execute sanity check on test library (no if zerobug testing itself)
         if (
             ctx['this'] != 'test_zerobug'
             and ctx.get('run_on_top', False)
             and not ctx.get('_run_autotest', False)
         ):
             if ctx.get('run4cover', False) and not ctx.get('dry_run', False):
@@ -1218,37 +1213,41 @@
                         stderr=open('/dev/null', 'w'),
                     )
                 except OSError:
                     print('Coverage not found!')
                     ctx['run4cover'] = False
         test_list = []
         if isinstance(UT, (list, tuple)):
-            self.dbgmsg(ctx, '>>> test_list=%s' % UT)
+            # self.dbgmsg(ctx, '>>> test_list=%s' % UT)
             test_list = UT
         elif not ctx.get('_run_autotest', False):
             # Discover test files
             test_list = []
             for pattern in (
                 ctx['opt_pattern'] and ctx['opt_pattern'].split(',') or self.pattern
             ):
-                self.dbgmsg(ctx, '- Search for files %s' % pattern)
+                # self.dbgmsg(ctx, '- Search for files %s' % pattern)
                 test_files = os.path.abspath(os.path.join(self.testdir, pattern))
                 for fn in sorted(glob.glob(test_files)):
                     mime = magic.Magic(mime=True).from_file(os.path.realpath(fn))
                     if mime in ('text/x-python', 'text/x-shellscript'):
                         test_list.append(fn)
         if len(test_list) == 0 and Test is not None:
-            self.dbgmsg(ctx, '- len(test_list) == 0 ')
-            test_num = 0
-            for _i in range(MAX_TEST_NUM):
-                tname = "test_{:02}".format(test_num)
-                if hasattr(Test, tname):
-                    test_list.append(tname)
-                test_num += 1
-        self.dbgmsg(ctx, '- test_list=%s' % test_list)
+            # self.dbgmsg(ctx, '- len(test_list) == 0 ')
+            test_list = sorted(
+                [meth for meth in dir(Test)
+                 if meth.startswith("test_") and callable(getattr(Test, meth))]
+            )
+            # test_num = 0
+            # for _i in range(MAX_TEST_NUM):
+            #     tname = "test_{:02}".format(test_num)
+            #     if hasattr(Test, tname):
+            #         test_list.append(tname)
+            #     test_num += 1
+        # self.dbgmsg(ctx, '- test_list=%s' % test_list)
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['ctr'])
             sts = TEST_SUCCESS
         else:
@@ -1256,31 +1255,31 @@
                 self.set_tlog_file(ctx)
             sts = self._exec_all_tests(test_list, ctx, Test)
             if ctx.get('run_on_top', False) and not ctx.get('_run_autotest', False):
                 if sts == TEST_SUCCESS:
                     print(success_msg)
                 else:
                     print(fail_msg)
-            if ctx.get('run4cover', False) and not ctx.get('dry_run', False):
-                try:
-                    subprocess.call(
-                        ['coverage', 'report', '--show-missing'],
-                    )
-                except OSError:
-                    print('Coverage not found!')
-                    ctx['run4cover'] = False
+                if ctx.get('run4cover', False) and not ctx.get('dry_run', False):
+                    try:
+                        subprocess.call(
+                            ['coverage', 'report', '--show-missing'],
+                        )
+                    except OSError:
+                        print('Coverage not found!')
+                        ctx['run4cover'] = False
         return sts
 
-    def dbgmsg(self, ctx, msg, echo=None):
-        if ctx.get('opt_debug', False):
-            fmode = 'w' if msg[0] == "!" else 'a'
-            with open(os.path.join(self.testdir, 'z0bug.tracehis'), fmode) as fd:
-                fd.write("%s> %s\n" % (os.path.basename(ctx['this_fqn']), msg))
-        if echo:
-            print('#DEBUG>>> %s' % msg)
+    # def dbgmsg(self, ctx, msg, echo=None):
+    #     # if ctx.get('opt_debug', False):
+    #     #     fmode = 'w' if msg[0] == "!" else 'a'
+    #     #     with open(os.path.join(self.testdir, 'z0bug.tracehis'), fmode) as fd:
+    #     #         fd.write("%s> %s\n" % (os.path.basename(ctx['this_fqn']), msg))
+    #     if echo:
+    #         print('#DEBUG>>> %s' % msg)
 
     def msg_test(self, ctx, msg):
         # ctx = self.ready_opts(ctx)
         if msg == ctx['_prior_msg']:
             # NEWLN = False
             prfx = "\x1b[A"
         else:
@@ -1302,14 +1301,18 @@
                     txt = "{}Test {}/{}: {}".format(
                         prfx, ctx['ctr'], ctx['max_test'], msg
                     )
                 else:
                     txt = "{}Test {}: {}".format(prfx, ctx['ctr'], msg)
                 os0.wlog(txt)
 
+    # def test_result(self, ctx, msg, test_value, result_value):
+    #     print("Function test_result() deprecated! Please use assertEqual()")
+    #     return assertEqual(test_value, result_value, message=msg)
+
     def test_result(self, ctx, msg, test_value, result_val):
         ctx = self._ready_opts(ctx)
         ctx['ctr'] += 1
         if ctx.get('teststs', TEST_SUCCESS):  # pragma: no cover
             return TEST_FAILED
         self.msg_test(ctx, msg)
         if not ctx.get('dry_run', False):
@@ -1321,15 +1324,15 @@
                 ctx['teststs'] = TEST_FAILED
                 if ctx.get('on_error', '') != 'continue':
                     raise AssertionError
                 else:
                     return TEST_FAILED
         return TEST_SUCCESS
 
-    def _init_test_ctx(self, opt_echo, full=None):
+    def _init_test_ctx(self, opt_echo, full={}):
         """Set context value for autotest"""
         z0ctx = {}
         if full:  # just for tests
             for p in 'min_test', 'max_test', 'opt_debug', 'opt_noctr', 'dry_run':
                 if p in full:
                     z0ctx[p] = full[p]
         if opt_echo == '-e':
@@ -1338,15 +1341,15 @@
             z0ctx['WLOGCMD'] = 'wecho-0'
         z0ctx['this'] = self.module_id
         z0ctx['this_fqn'] = './' + self.module_id
         z0ctx['_run_autotest'] = True
         self.def_tlog_fn = '~/z0bug.log'
         return z0ctx
 
-    def sanity_check(self, opt_echo, full=None):
+    def sanity_check(self, opt_echo, full={}):
         """Internal regression test
         Module z0testlib is needed to run regression tests
         This function run auto validation tests for z0testlib functions
         """
         z0ctx = self._init_test_ctx(opt_echo, full)
         sts = self.main(z0ctx, SanityTest)
         if full:
```

### Comparing `zerobug-2.0.4/zerobug/zerobug.py` & `zerobug-2.0.5/zerobug/zerobug.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
     You can use this file as main all_tests.py too
 """
 import sys
 from . import z0test
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 
 def version():
     return __version__
 
 
 def main(cli_args=None):
```

### Comparing `zerobug-2.0.4/zerobug.egg-info/SOURCES.txt` & `zerobug-2.0.5/zerobug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.4/zerobug.egg-info/PKG-INFO` & `zerobug-2.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zerobug
-Version: 2.0.4
+Version: 2.0.5
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        This library can run unit test of target package software.
-        Supported languages are python (through z0testlib.py) and bash (through z0testrc)
-        
-        zerobug supports test automation, aggregation of tests into collections
-        and independence of the tests from the reporting framework.
-        The zerobug module provides all code that make it easy to support testing
-        both for python programs both for bash scripts.
-        zerobug shows execution test with a message like "n/tot message"
-        where n is current unit test and tot is the total unit test to execute,
-        that is a sort of advancing test progress.
-        
-        You can use z0bug_odoo that is the odoo integration to test Odoo modules.
-        
-        zerobug is built on follow concepts:
-        
-        * test main - it is a main program to executes all test runners
-        * test runner - it is a program to executes one or more test suites
-        * test suite - it is a collection of test cases
-        * test case - it is a smallest unit test
-        
-        The main file is the command zerobug of this package; it searches for test runner files
-        named `[id_]test_` where 'id' is the shor name of testing package.
-        
-        Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
-        executed in sorted order.
-        
-        Every suit can contains one or more test case, the smallest unit test;
-        every unit test terminates with success or with failure.
-        
-        Because zerobug can show total number of unit test to execute, it runs tests
-        in 2 passes. In the first pass it counts the number of test, in second pass executes really
-        it. This behavior can be overridden by -0 switch.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+This library can run unit test of target package software.
+Supported languages are python (through z0testlib.py) and bash (through z0testrc)
+
+zerobug supports test automation, aggregation of tests into collections
+and independence of the tests from the reporting framework.
+The zerobug module provides all code that make it easy to support testing
+both for python programs both for bash scripts.
+zerobug shows execution test with a message like "n/tot message"
+where n is current unit test and tot is the total unit test to execute,
+that is a sort of advancing test progress.
+
+You can use z0bug_odoo that is the odoo integration to test Odoo modules.
+
+zerobug is built on follow concepts:
+
+* test main - it is a main program to executes all test runners
+* test runner - it is a program to executes one or more test suites
+* test suite - it is a collection of test cases
+* test case - it is a smallest unit test
+
+The main file is the command zerobug of this package; it searches for test runner files
+named `[id_]test_` where 'id' is the shor name of testing package.
+
+Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
+executed in sorted order.
+
+Every suit can contains one or more test case, the smallest unit test;
+every unit test terminates with success or with failure.
+
+Because zerobug can show total number of unit test to execute, it runs tests
+in 2 passes. In the first pass it counts the number of test, in second pass executes really
+it. This behavior can be overridden by -0 switch.
+
+
```

### Comparing `zerobug-2.0.4/setup.py` & `zerobug-2.0.5/zerobug/scripts/setup.info`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,37 @@
 from setuptools import find_packages, setup
 
 if sys.version_info >= (3, 0):
     install_requires = (
         [
             'future',
             'coverage',
-            'coveralls',
-            'codecov',
             'pylint-odoo',
             'python-magic',
             'python-plus',
             'os0',
             'z0lib',
         ],
     )
 else:
     install_requires = (
         [
             'future',
             'coverage',
-            'coveralls',
-            'codecov',
             'pylint-odoo<=5.0.0',
             'python-magic',
             'python-plus',
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.4',
+    version='2.0.5',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description="""
 This library can run unit test of target package software.
 Supported languages are python (through z0testlib.py) and bash (through z0testrc)
 
 zerobug supports test automation, aggregation of tests into collections
```

### Comparing `zerobug-2.0.4/PKG-INFO` & `zerobug-2.0.5/zerobug.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zerobug
-Version: 2.0.4
+Version: 2.0.5
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        This library can run unit test of target package software.
-        Supported languages are python (through z0testlib.py) and bash (through z0testrc)
-        
-        zerobug supports test automation, aggregation of tests into collections
-        and independence of the tests from the reporting framework.
-        The zerobug module provides all code that make it easy to support testing
-        both for python programs both for bash scripts.
-        zerobug shows execution test with a message like "n/tot message"
-        where n is current unit test and tot is the total unit test to execute,
-        that is a sort of advancing test progress.
-        
-        You can use z0bug_odoo that is the odoo integration to test Odoo modules.
-        
-        zerobug is built on follow concepts:
-        
-        * test main - it is a main program to executes all test runners
-        * test runner - it is a program to executes one or more test suites
-        * test suite - it is a collection of test cases
-        * test case - it is a smallest unit test
-        
-        The main file is the command zerobug of this package; it searches for test runner files
-        named `[id_]test_` where 'id' is the shor name of testing package.
-        
-        Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
-        executed in sorted order.
-        
-        Every suit can contains one or more test case, the smallest unit test;
-        every unit test terminates with success or with failure.
-        
-        Because zerobug can show total number of unit test to execute, it runs tests
-        in 2 passes. In the first pass it counts the number of test, in second pass executes really
-        it. This behavior can be overridden by -0 switch.
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+This library can run unit test of target package software.
+Supported languages are python (through z0testlib.py) and bash (through z0testrc)
+
+zerobug supports test automation, aggregation of tests into collections
+and independence of the tests from the reporting framework.
+The zerobug module provides all code that make it easy to support testing
+both for python programs both for bash scripts.
+zerobug shows execution test with a message like "n/tot message"
+where n is current unit test and tot is the total unit test to execute,
+that is a sort of advancing test progress.
+
+You can use z0bug_odoo that is the odoo integration to test Odoo modules.
+
+zerobug is built on follow concepts:
+
+* test main - it is a main program to executes all test runners
+* test runner - it is a program to executes one or more test suites
+* test suite - it is a collection of test cases
+* test case - it is a smallest unit test
+
+The main file is the command zerobug of this package; it searches for test runner files
+named `[id_]test_` where 'id' is the shor name of testing package.
+
+Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
+executed in sorted order.
+
+Every suit can contains one or more test case, the smallest unit test;
+every unit test terminates with success or with failure.
+
+Because zerobug can show total number of unit test to execute, it runs tests
+in 2 passes. In the first pass it counts the number of test, in second pass executes really
+it. This behavior can be overridden by -0 switch.
+
+
```

### Comparing `zerobug-2.0.4/README.rst` & `zerobug-2.0.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 =============
-zerobug 2.0.4
+zerobug 2.0.5
 =============
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -362,14 +362,21 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.5 (2023-03-24)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] travis_install_env: ensure list_requirements is executable
+* [IMP] flake8 configuration
+* [IMP] coveralls and codecov are not more dependenciesple  
+
 2.0.4 (2022-12-08)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_pypi_test: best recognition of python version
 * [FIX] build_cmd: best recognition of python version
 * [FIX] travis_install_env: ensure coverage version
 * [IMP] odoo environment to test more precise
@@ -431,21 +438,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-01-13
+Last Update / Ultimo aggiornamento: 2023-04-14
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

