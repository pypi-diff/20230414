# Comparing `tmp/pro-football_reference_web_scraper-0.1.1.tar.gz` & `tmp/pro-football_reference_web_scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pro-football_reference_web_scraper-0.1.1.tar", last modified: Sat Apr  1 04:03:57 2023, max compression
+gzip compressed data, was "pro-football_reference_web_scraper-0.2.0.tar", last modified: Fri Apr 14 21:09:53 2023, max compression
```

## Comparing `pro-football_reference_web_scraper-0.1.1.tar` & `pro-football_reference_web_scraper-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,49 @@
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.399131 pro-football_reference_web_scraper-0.1.1/
--rw-r--r--   0 matthewkim   (501) staff       (20)      323 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/.bumpversion.cfg
--rw-r--r--   0 matthewkim   (501) staff       (20)    11357 2023-02-15 02:53:12.000000 pro-football_reference_web_scraper-0.1.1/LICENSE
--rw-r--r--   0 matthewkim   (501) staff       (20)      622 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/MANIFEST.in
--rw-r--r--   0 matthewkim   (501) staff       (20)     2512 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/Makefile
--rw-r--r--   0 matthewkim   (501) staff       (20)    16276 2023-04-01 04:03:57.398830 pro-football_reference_web_scraper-0.1.1/PKG-INFO
--rw-r--r--   0 matthewkim   (501) staff       (20)     2435 2023-03-31 18:15:23.000000 pro-football_reference_web_scraper-0.1.1/README.md
--rw-r--r--   0 matthewkim   (501) staff       (20)        0 2023-03-02 23:10:23.000000 pro-football_reference_web_scraper-0.1.1/conftest.py
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.396247 pro-football_reference_web_scraper-0.1.1/docs/
--rw-r--r--   0 matthewkim   (501) staff       (20)     1190 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/CONTRIBUTING.md
--rw-r--r--   0 matthewkim   (501) staff       (20)      634 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/Makefile
--rw-r--r--   0 matthewkim   (501) staff       (20)     2367 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/README.md
--rw-r--r--   0 matthewkim   (501) staff       (20)     1993 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/conf.py
--rw-r--r--   0 matthewkim   (501) staff       (20)       50 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/get_player_game_log.md
--rw-r--r--   0 matthewkim   (501) staff       (20)       48 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/get_team_game_log.md
--rw-r--r--   0 matthewkim   (501) staff       (20)     1420 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/index.md
--rw-r--r--   0 matthewkim   (501) staff       (20)      765 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/make.bat
--rw-r--r--   0 matthewkim   (501) staff       (20)       42 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.396560 pro-football_reference_web_scraper-0.1.1/docs/source/
--rw-r--r--   0 matthewkim   (501) staff       (20)      139 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/source/modules.rst
--rw-r--r--   0 matthewkim   (501) staff       (20)      748 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/docs/source/pro_football_reference_web_scraper.rst
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.397253 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/
--rw-r--r--   0 matthewkim   (501) staff       (20)      128 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/__init__.py
--rw-r--r--   0 matthewkim   (501) staff       (20)       22 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/_version.py
--rw-r--r--   0 matthewkim   (501) staff       (20)     9484 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/player_game_log.py
--rw-r--r--   0 matthewkim   (501) staff       (20)    11578 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/team_game_log.py
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.397815 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/
--rw-r--r--   0 matthewkim   (501) staff       (20)    16276 2023-04-01 04:03:57.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matthewkim   (501) staff       (20)      972 2023-04-01 04:03:57.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matthewkim   (501) staff       (20)        1 2023-04-01 04:03:57.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matthewkim   (501) staff       (20)      226 2023-04-01 04:03:57.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/requires.txt
--rw-r--r--   0 matthewkim   (501) staff       (20)       35 2023-04-01 04:03:57.000000 pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/top_level.txt
--rw-r--r--   0 matthewkim   (501) staff       (20)     2320 2023-04-01 04:00:56.000000 pro-football_reference_web_scraper-0.1.1/pyproject.toml
--rw-r--r--   0 matthewkim   (501) staff       (20)       38 2023-04-01 04:03:57.399175 pro-football_reference_web_scraper-0.1.1/setup.cfg
--rw-r--r--   0 matthewkim   (501) staff       (20)       39 2023-03-02 23:10:23.000000 pro-football_reference_web_scraper-0.1.1/setup.py
-drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-01 04:03:57.398478 pro-football_reference_web_scraper-0.1.1/tests/
--rw-r--r--   0 matthewkim   (501) staff       (20)      585 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/tests/test_player_game_log_integration.py
--rw-r--r--   0 matthewkim   (501) staff       (20)     5796 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/tests/test_player_game_log_unit.py
--rw-r--r--   0 matthewkim   (501) staff       (20)      660 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/tests/test_team_game_log_integration.py
--rw-r--r--   0 matthewkim   (501) staff       (20)    36085 2023-03-25 21:28:52.000000 pro-football_reference_web_scraper-0.1.1/tests/test_team_game_log_unit.py
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.197000 pro-football_reference_web_scraper-0.2.0/
+-rw-r--r--   0 matthewkim   (501) staff       (20)      323 2023-04-14 21:03:57.000000 pro-football_reference_web_scraper-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 matthewkim   (501) staff       (20)      125 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 matthewkim   (501) staff       (20)    11357 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/LICENSE
+-rw-r--r--   0 matthewkim   (501) staff       (20)      668 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/MANIFEST.in
+-rw-r--r--   0 matthewkim   (501) staff       (20)     2859 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/Makefile
+-rw-r--r--   0 matthewkim   (501) staff       (20)    16570 2023-04-14 21:09:53.196700 pro-football_reference_web_scraper-0.2.0/PKG-INFO
+-rw-r--r--   0 matthewkim   (501) staff       (20)     2729 2023-04-14 20:33:00.000000 pro-football_reference_web_scraper-0.2.0/README.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)        0 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/conftest.py
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.192602 pro-football_reference_web_scraper-0.2.0/docs/
+-rw-r--r--   0 matthewkim   (501) staff       (20)      125 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/docs/.readthedocs.yaml
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1190 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)      634 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/Makefile
+-rw-r--r--   0 matthewkim   (501) staff       (20)     2367 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/README.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1993 2023-04-14 20:54:39.000000 pro-football_reference_web_scraper-0.2.0/docs/conf.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)    12775 2023-04-14 20:52:23.000000 pro-football_reference_web_scraper-0.2.0/docs/get_player_game_log.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)    10423 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/docs/get_team_game_log.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1375 2023-04-09 21:13:38.000000 pro-football_reference_web_scraper-0.2.0/docs/index.md
+-rw-r--r--   0 matthewkim   (501) staff       (20)      765 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/make.bat
+-rw-r--r--   0 matthewkim   (501) staff       (20)       42 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.193001 pro-football_reference_web_scraper-0.2.0/docs/source/
+-rw-r--r--   0 matthewkim   (501) staff       (20)      139 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/docs/source/modules.rst
+-rw-r--r--   0 matthewkim   (501) staff       (20)      748 2023-04-14 21:00:40.000000 pro-football_reference_web_scraper-0.2.0/docs/source/pro_football_reference_web_scraper.rst
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1672 2023-04-14 20:55:20.000000 pro-football_reference_web_scraper-0.2.0/docs/team_splits.md
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.194411 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/
+-rw-r--r--   0 matthewkim   (501) staff       (20)      201 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/__init__.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)       22 2023-04-14 21:03:57.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/_version.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)    10946 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/player_game_log.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     3259 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/player_splits.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)    11957 2023-04-14 20:33:00.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/team_game_log.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     5107 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/team_splits.py
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.195002 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/
+-rw-r--r--   0 matthewkim   (501) staff       (20)    16570 2023-04-14 21:09:53.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1277 2023-04-14 21:09:53.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewkim   (501) staff       (20)        1 2023-04-14 21:09:53.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewkim   (501) staff       (20)      226 2023-04-14 21:09:53.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/requires.txt
+-rw-r--r--   0 matthewkim   (501) staff       (20)       35 2023-04-14 21:09:53.000000 pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/top_level.txt
+-rw-r--r--   0 matthewkim   (501) staff       (20)     2320 2023-04-14 21:03:57.000000 pro-football_reference_web_scraper-0.2.0/pyproject.toml
+-rw-r--r--   0 matthewkim   (501) staff       (20)       38 2023-04-14 21:09:53.197044 pro-football_reference_web_scraper-0.2.0/setup.cfg
+-rw-r--r--   0 matthewkim   (501) staff       (20)       39 2023-04-14 21:03:05.000000 pro-football_reference_web_scraper-0.2.0/setup.py
+drwxr-xr-x   0 matthewkim   (501) staff       (20)        0 2023-04-14 21:09:53.196433 pro-football_reference_web_scraper-0.2.0/tests/
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1066 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_player_game_log_integration.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     5979 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_player_game_log_unit.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1082 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_player_splits_integration.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     1375 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_player_splits_unit.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)      965 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_team_game_log_integration.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)    36085 2023-04-01 20:08:56.000000 pro-football_reference_web_scraper-0.2.0/tests/test_team_game_log_unit.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)      905 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_team_splits_integration.py
+-rw-r--r--   0 matthewkim   (501) staff       (20)     2840 2023-04-14 21:00:46.000000 pro-football_reference_web_scraper-0.2.0/tests/test_team_splits_unit.py
```

### Comparing `pro-football_reference_web_scraper-0.1.1/LICENSE` & `pro-football_reference_web_scraper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/PKG-INFO` & `pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pro-football_reference_web_scraper
-Version: 0.1.1
+Name: pro-football-reference-web-scraper
+Version: 0.2.0
 Summary: Stats web scraper of Pro Football Reference
 Author-email: Matthew Kim <mjk2244@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # pro-football-reference-web-scraper
 Web scraper to retrieve player and team data from Pro Football Reference.  
 
-[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
+[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/) [![readthedocs](https://img.shields.io/readthedocs/pro-football-reference-web-scraper)](https://pro-football-reference-web-scraper.readthedocs.io/en/latest/) [![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://mjk2244.github.io/pro-football-reference-web-scraper/)
 ## Overview
 pro-football-reference-web-scraper is a Python library that helps developers take advantage of the plethora of free data provided by [Pro Football Reference](https://www.pro-football-reference.com/). It is intended primarily to help fantasy sports players and sports bettors gain an edge in their NFL sports gaming endeavors. However, it can be used for any project that requires team- and player-specific data.
 
 ## Installation
 To install, run the following:
 ```
 pip install pro-football-reference-web-scraper
```

### Comparing `pro-football_reference_web_scraper-0.1.1/README.md` & `pro-football_reference_web_scraper-0.2.0/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pro-football-reference-web-scraper
+# Quick Guide
 Web scraper to retrieve player and team data from Pro Football Reference.  
 
-[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
+[![](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
 ## Overview
 pro-football-reference-web-scraper is a Python library that helps developers take advantage of the plethora of free data provided by [Pro Football Reference](https://www.pro-football-reference.com/). It is intended primarily to help fantasy sports players and sports bettors gain an edge in their NFL sports gaming endeavors. However, it can be used for any project that requires team- and player-specific data.
 
 ## Installation
 To install, run the following:
 ```
 pip install pro-football-reference-web-scraper
```

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/CONTRIBUTING.md` & `pro-football_reference_web_scraper-0.2.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/Makefile` & `pro-football_reference_web_scraper-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/README.md` & `pro-football_reference_web_scraper-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Quick Guide
+# pro-football-reference-web-scraper
 Web scraper to retrieve player and team data from Pro Football Reference.  
 
-[![](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
+[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/) [![readthedocs](https://img.shields.io/readthedocs/pro-football-reference-web-scraper)](https://pro-football-reference-web-scraper.readthedocs.io/en/latest/) [![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://mjk2244.github.io/pro-football-reference-web-scraper/)
 ## Overview
 pro-football-reference-web-scraper is a Python library that helps developers take advantage of the plethora of free data provided by [Pro Football Reference](https://www.pro-football-reference.com/). It is intended primarily to help fantasy sports players and sports bettors gain an edge in their NFL sports gaming endeavors. However, it can be used for any project that requires team- and player-specific data.
 
 ## Installation
 To install, run the following:
 ```
 pip install pro-football-reference-web-scraper
```

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/conf.py` & `pro-football_reference_web_scraper-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/index.md` & `pro-football_reference_web_scraper-0.2.0/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Welcome to pro-football-reference-web-scraper's documentation!
 
-[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
+[![](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
 ## Overview
 pro-football-reference-web-scraper is a Python library that helps developers take advantage of the plethora of free data provided by [Pro Football Reference](https://www.pro-football-reference.com/). It is intended primarily to help fantasy sports players and sports bettors gain an edge in their NFL sports gaming endeavors. However, it can be used for any project that requires team- and player-specific data.
 
 ```eval_rst
 
 .. toctree::
    :maxdepth: 10
```

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/make.bat` & `pro-football_reference_web_scraper-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/docs/source/pro_football_reference_web_scraper.rst` & `pro-football_reference_web_scraper-0.2.0/docs/source/pro_football_reference_web_scraper.rst`

 * *Files identical despite different names*

### Comparing `pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/player_game_log.py` & `pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/player_game_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd  # type: ignore
 from bs4 import BeautifulSoup
 import requests
 
+valid_positions = ['QB', 'RB', 'WR', 'TE']
+
 
 # function that returns a player's game log in a given season
 # player: player's full name (e.g. Tom Brady)
 # position: abbreviation (QB, RB, WR, TE only)
 def get_player_game_log(player: str, position: str, season: int) -> pd.DataFrame:
     """A function to retrieve a player's game log in a given season.
 
@@ -13,17 +15,22 @@
 
     Args:
         player (str): A NFL player's full name, as it appears on Pro Football Reference
         position (str): The position the player plays. Must be 'QB', 'RB', 'WR', or 'TE'
         season (int): The season of the game log you are trying to retrieve
 
     Returns:
-        pandas.DataFrame: Each game is a row
+        pandas.DataFrame: Each game is a row of the DataFrame
 
     """
+
+    # position arg must be formatted properly
+    if position not in valid_positions:
+        raise Exception('Invalid position: "position" arg must be "QB", "RB", "WR", or "TE"')
+
     # make request to find proper href
     r1 = make_request_list(player, position, season)
     player_list = get_soup(r1)
 
     # find href
     href = get_href(player, position, season, player_list)
 
@@ -45,16 +52,16 @@
 # helper function that gets the player's href
 def get_href(player: str, position: str, season: int, player_list: BeautifulSoup) -> str:
     players = player_list.find('div', id='div_players').find_all('p')
     for p in players:
         seasons = p.text.split(' ')
         seasons = seasons[len(seasons) - 1].split('-')
         if season >= int(seasons[0]) and season <= int(seasons[1]) and player in p.text and position in p.text:
-            href = p.find('a').get('href')
-    return href
+            return p.find('a').get('href')
+    raise Exception('Cannot find a ' + position + ' named ' + player + ' from ' + str(season))
 
 
 # helper function that makes a HTTP request over a list of players with a given last initial
 def make_request_list(player: str, position: str, season: int):
     name_split = player.split(' ')
     last_initial = name_split[1][0]
     url = 'https://www.pro-football-reference.com/players/%s/' % (last_initial)
@@ -72,146 +79,170 @@
     return BeautifulSoup(request.text, 'html.parser')
 
 
 # helper function that takes a BeautifulSoup object and converts it into a pandas dataframe containing a QB game log
 def qb_game_log(soup: BeautifulSoup) -> pd.DataFrame:
     # Most relevant QB stats, in my opinion. Could adjust if necessary
     data = {
-        'Date': [],
-        'Week': [],
-        'Team': [],
-        'Game_Location': [],
-        'Opp': [],
-        'Result': [],
-        'Cmp': [],
-        'Att': [],
-        'Pass_Yds': [],
-        'Pass_TD': [],
-        'Int': [],
-        'Rating': [],
-        'Sacked': [],
-        'Rush_Att': [],
-        'Rush_Yds': [],
-        'Rush_TD': [],
+        'date': [],
+        'week': [],
+        'team': [],
+        'game_location': [],
+        'opp': [],
+        'result': [],
+        'team_pts': [],
+        'opp_pts': [],
+        'cmp': [],
+        'att': [],
+        'pass_yds': [],
+        'pass_td': [],
+        'int': [],
+        'rating': [],
+        'sacked': [],
+        'rush_att': [],
+        'rush_yds': [],
+        'rush_td': [],
     }  # type: dict
 
     table_rows = soup.find('tbody').find_all('tr')
 
     # ignore inactive or DNP games
     to_ignore = []
     for i in range(len(table_rows)):
         elements = table_rows[i].find_all('td')
         if elements[len(elements) - 1].text == 'Inactive' or elements[len(elements) - 1].text == 'Did Not Play':
             to_ignore.append(i)
 
     # adding data to data dictionary
     for i in range(len(table_rows)):
         if i not in to_ignore:
-            data['Date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
-            data['Week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
-            data['Team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
-            data['Game_Location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
-            data['Opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
-            data['Result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text)
-            data['Cmp'].append(int(table_rows[i].find('td', {'data-stat': 'pass_cmp'}).text))
-            data['Att'].append(int(table_rows[i].find('td', {'data-stat': 'pass_att'}).text))
-            data['Pass_Yds'].append(int(table_rows[i].find('td', {'data-stat': 'pass_yds'}).text))
-            data['Pass_TD'].append(int(table_rows[i].find('td', {'data-stat': 'pass_td'}).text))
-            data['Int'].append(int(table_rows[i].find('td', {'data-stat': 'pass_int'}).text))
-            data['Rating'].append(float(table_rows[i].find('td', {'data-stat': 'pass_rating'}).text))
-            data['Sacked'].append(int(table_rows[i].find('td', {'data-stat': 'pass_sacked'}).text))
-            data['Rush_Att'].append(int(table_rows[i].find('td', {'data-stat': 'rush_att'}).text))
-            data['Rush_Yds'].append(int(table_rows[i].find('td', {'data-stat': 'rush_yds'}).text))
-            data['Rush_TD'].append(int(table_rows[i].find('td', {'data-stat': 'rush_td'}).text))
+            data['date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
+            data['week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
+            data['team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
+            data['game_location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
+            data['opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
+            data['result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[0])
+            data['team_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[0])
+            )
+            data['opp_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[1])
+            )
+            data['cmp'].append(int(table_rows[i].find('td', {'data-stat': 'pass_cmp'}).text))
+            data['att'].append(int(table_rows[i].find('td', {'data-stat': 'pass_att'}).text))
+            data['pass_yds'].append(int(table_rows[i].find('td', {'data-stat': 'pass_yds'}).text))
+            data['pass_td'].append(int(table_rows[i].find('td', {'data-stat': 'pass_td'}).text))
+            data['int'].append(int(table_rows[i].find('td', {'data-stat': 'pass_int'}).text))
+            data['rating'].append(float(table_rows[i].find('td', {'data-stat': 'pass_rating'}).text))
+            data['sacked'].append(int(table_rows[i].find('td', {'data-stat': 'pass_sacked'}).text))
+            data['rush_att'].append(int(table_rows[i].find('td', {'data-stat': 'rush_att'}).text))
+            data['rush_yds'].append(int(table_rows[i].find('td', {'data-stat': 'rush_yds'}).text))
+            data['rush_td'].append(int(table_rows[i].find('td', {'data-stat': 'rush_td'}).text))
 
     return pd.DataFrame(data=data)
 
 
 # helper function that takes a BeautifulSoup object and converts it into a pandas dataframe containing a WR/TE game log
 def wr_game_log(soup: BeautifulSoup) -> pd.DataFrame:
     # Most relevant WR stats, in my opinion.
     # Could adjust if necessary (maybe figure out how to incorporate rushing stats?)
 
     data = {
-        'Date': [],
-        'Week': [],
-        'Team': [],
-        'Game_Location': [],
-        'Opp': [],
-        'Result': [],
-        'Tgt': [],
-        'Rec': [],
-        'Rec_Yds': [],
-        'Rec_TD': [],
-        'Snap_Pct': [],
+        'date': [],
+        'week': [],
+        'team': [],
+        'game_location': [],
+        'opp': [],
+        'result': [],
+        'team_pts': [],
+        'opp_pts': [],
+        'tgt': [],
+        'rec': [],
+        'rec_yds': [],
+        'rec_td': [],
+        'snap_pct': [],
     }  # type: dict
 
     table_rows = soup.find('tbody').find_all('tr')
 
     # ignore inactive or DNP games
     to_ignore = []
     for i in range(len(table_rows)):
         elements = table_rows[i].find_all('td')
         if elements[len(elements) - 1].text == 'Inactive' or elements[len(elements) - 1].text == 'Did Not Play':
             to_ignore.append(i)
 
     # adding data to data dictionray
     for i in range(len(table_rows)):
         if i not in to_ignore:
-            data['Date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
-            data['Week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
-            data['Team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
-            data['Game_Location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
-            data['Opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
-            data['Result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text)
-            data['Tgt'].append(int(table_rows[i].find('td', {'data-stat': 'targets'}).text))
-            data['Rec'].append(int(table_rows[i].find('td', {'data-stat': 'rec'}).text))
-            data['Rec_Yds'].append(int(table_rows[i].find('td', {'data-stat': 'rec_yds'}).text))
-            data['Rec_TD'].append(int(table_rows[i].find('td', {'data-stat': 'rec_td'}).text))
-            data['Snap_Pct'].append(float(int(table_rows[i].find('td', {'data-stat': 'off_pct'}).text[:-1]) / 100))
+            data['date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
+            data['week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
+            data['team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
+            data['game_location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
+            data['opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
+            data['result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[0])
+            data['team_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[0])
+            )
+            data['opp_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[1])
+            )
+            data['tgt'].append(int(table_rows[i].find('td', {'data-stat': 'targets'}).text))
+            data['rec'].append(int(table_rows[i].find('td', {'data-stat': 'rec'}).text))
+            data['rec_yds'].append(int(table_rows[i].find('td', {'data-stat': 'rec_yds'}).text))
+            data['rec_td'].append(int(table_rows[i].find('td', {'data-stat': 'rec_td'}).text))
+            data['snap_pct'].append(float(int(table_rows[i].find('td', {'data-stat': 'off_pct'}).text[:-1]) / 100))
 
     return pd.DataFrame(data=data)
 
 
 def rb_game_log(soup: BeautifulSoup) -> pd.DataFrame:
     # Most relevant RB stats, in my opinion. Could adjust if necessary
     data = {
-        'Date': [],
-        'Week': [],
-        'Team': [],
-        'Game_Location': [],
-        'Opp': [],
-        'Result': [],
-        'Rush_Att': [],
-        'Rush_Yds': [],
-        'Rush_TD': [],
-        'Tgt': [],
-        'Rec_Yds': [],
-        'Rec_TD': [],
+        'date': [],
+        'week': [],
+        'team': [],
+        'game_location': [],
+        'opp': [],
+        'result': [],
+        'team_pts': [],
+        'opp_pts': [],
+        'rush_att': [],
+        'rush_yds': [],
+        'rush_td': [],
+        'tgt': [],
+        'rec_yds': [],
+        'rec_td': [],
     }  # type: dict
 
     table_rows = soup.find('tbody').find_all('tr')
 
     # ignore inactive or DNP games
     to_ignore = []
     for i in range(len(table_rows)):
         elements = table_rows[i].find_all('td')
         if elements[len(elements) - 1].text == 'Inactive' or elements[len(elements) - 1].text == 'Did Not Play':
             to_ignore.append(i)
 
     # adding data to data dictionary
     for i in range(len(table_rows)):
         if i not in to_ignore:
-            data['Date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
-            data['Week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
-            data['Team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
-            data['Game_Location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
-            data['Opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
-            data['Result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text)
-            data['Rush_Att'].append(int(table_rows[i].find('td', {'data-stat': 'rush_att'}).text))
-            data['Rush_Yds'].append(int(table_rows[i].find('td', {'data-stat': 'rush_yds'}).text))
-            data['Rush_TD'].append(int(table_rows[i].find('td', {'data-stat': 'rush_td'}).text))
-            data['Tgt'].append(int(table_rows[i].find('td', {'data-stat': 'targets'}).text))
-            data['Rec_Yds'].append(int(table_rows[i].find('td', {'data-stat': 'rec_yds'}).text))
-            data['Rec_TD'].append(int(table_rows[i].find('td', {'data-stat': 'rec_td'}).text))
+            data['date'].append(table_rows[i].find('td', {'data-stat': 'game_date'}).text)
+            data['week'].append(int(table_rows[i].find('td', {'data-stat': 'week_num'}).text))
+            data['team'].append(table_rows[i].find('td', {'data-stat': 'team'}).text)
+            data['game_location'].append(table_rows[i].find('td', {'data-stat': 'game_location'}).text)
+            data['opp'].append(table_rows[i].find('td', {'data-stat': 'opp'}).text)
+            data['result'].append(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[0])
+            data['team_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[0])
+            )
+            data['opp_pts'].append(
+                int(table_rows[i].find('td', {'data-stat': 'game_result'}).text.split(' ')[1].split('-')[1])
+            )
+            data['rush_att'].append(int(table_rows[i].find('td', {'data-stat': 'rush_att'}).text))
+            data['rush_yds'].append(int(table_rows[i].find('td', {'data-stat': 'rush_yds'}).text))
+            data['rush_td'].append(int(table_rows[i].find('td', {'data-stat': 'rush_td'}).text))
+            data['tgt'].append(int(table_rows[i].find('td', {'data-stat': 'targets'}).text))
+            data['rec_yds'].append(int(table_rows[i].find('td', {'data-stat': 'rec_yds'}).text))
+            data['rec_td'].append(int(table_rows[i].find('td', {'data-stat': 'rec_td'}).text))
 
     return pd.DataFrame(data=data)
```

### Comparing `pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper/team_game_log.py` & `pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper/team_game_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,21 @@
     'Carolina Panthers': 'car',
     'Jacksonville Jaguars': 'jax',
     'Baltimore Ravens': 'rav',
     'Houston Texans': 'htx',
     'Oakland Raiders': 'rai',
     'San Diego Chargers': 'sdg',
     'St. Louis Rams': 'ram',
+    'Boston Patriots': 'nwe',
 }
 
 months = {"September": 9, "October": 10, "November": 11, "December": 12, "January": 1}
 
 locations = {
+    'Boston': {'latitude': 42.3656, 'longitude': 71.0096, 'airport': 'BOS'},
     'Phoenix': {'latitude': 33.4352, 'longitude': 112.0101, 'airport': 'PHX'},
     'Chicago': {'latitude': 41.9803, 'longitude': 87.9090, 'airport': 'ORD'},
     'Green Bay': {'latitude': 44.4923, 'longitude': 88.1278, 'airport': 'GRB'},
     'New York': {'latitude': 40.6895, 'longitude': 74.1745, 'airport': 'EWR'},
     'Detroit': {'latitude': 42.2162, 'longitude': 83.3554, 'airport': 'DTW'},
     'Washington DC': {'latitude': 38.9531, 'longitude': 77.4565, 'airport': 'IAD'},
     'Philadelphia': {'latitude': 39.9526, 'longitude': 75.1652, 'airport': 'PHL'},
@@ -130,36 +132,43 @@
     'Baltimore Ravens': 'Baltimore',
     'Houston Texans': 'Houston',
     'Oakland Raiders': 'Oakland',
     'San Diego Chargers': 'San Diego',
     'St. Louis Rams': 'St. Louis',
     'Baltimore Colts': 'Baltimore',
     'St. Louis Cardinals': 'St. Louis',
-    # 'Boston Patriots': 'Boston' add Boston to locations dictionary
+    'Boston Patriots': 'Boston',
 }
 
 
 # function that returns a team's game log in a given season
 def get_team_game_log(team: str, season: int) -> pd.DataFrame:
     """A function to retrieve a team's game log in a given season.
 
     Returns a pandas DataFrame of a NFL team's game log in a given season, including relevant team-level statistics.
 
     Args:
         team (str): A NFL team's name, as it appears on Pro Football Reference
         season (int): The season of the game log you are trying to retrieve
 
     Returns:
-        pandas.DataFrame: Each game is a row
+        pandas.DataFrame: Each game is a row of the DataFrame
 
     """
 
+    # raise exception if team name is misspelled
+    if team not in team_hrefs.keys():
+        raise Exception('Invalid team name. Note: spelling is case sensitive')
+
     # make HTTP request and extract HTML
     r = make_request(team, season)
 
+    if r.status_code == 404:
+        raise Exception('404 error. The ' + team + ' may not have existed in ' + str(season))
+
     # parse HTML using BeautifulSoup
     soup = get_soup(r)
 
     # collect data and return data frame
     return collect_data(soup, season, team)
```

### Comparing `pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/PKG-INFO` & `pro-football_reference_web_scraper-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pro-football-reference-web-scraper
-Version: 0.1.1
+Name: pro-football_reference_web_scraper
+Version: 0.2.0
 Summary: Stats web scraper of Pro Football Reference
 Author-email: Matthew Kim <mjk2244@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # pro-football-reference-web-scraper
 Web scraper to retrieve player and team data from Pro Football Reference.  
 
-[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/)
+[![License](https://img.shields.io/github/license/mjk2244/pro-football-reference-web-scraper)](https://opensource.org/licenses/Apache-2.0) ![GitHub issues](https://img.shields.io/github/issues/mjk2244/pro-football-reference-web-scraper) [![codecov](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper/branch/main/graph/badge.svg?token=OTGOR2M0CY)](https://codecov.io/gh/mjk2244/pro-football-reference-web-scraper) [![Package Status](https://img.shields.io/github/actions/workflow/status/mjk2244/pro-football-reference-web-scraper/build.yml)](https://github.com/mjk2244/pro-football-reference-web-scraper/) [![PyPI](https://img.shields.io/pypi/v/pro-football-reference-web-scraper)](https://pypi.org/project/pro-football-reference-web-scraper/) [![readthedocs](https://img.shields.io/readthedocs/pro-football-reference-web-scraper)](https://pro-football-reference-web-scraper.readthedocs.io/en/latest/) [![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://mjk2244.github.io/pro-football-reference-web-scraper/)
 ## Overview
 pro-football-reference-web-scraper is a Python library that helps developers take advantage of the plethora of free data provided by [Pro Football Reference](https://www.pro-football-reference.com/). It is intended primarily to help fantasy sports players and sports bettors gain an edge in their NFL sports gaming endeavors. However, it can be used for any project that requires team- and player-specific data.
 
 ## Installation
 To install, run the following:
 ```
 pip install pro-football-reference-web-scraper
```

### Comparing `pro-football_reference_web_scraper-0.1.1/pro_football_reference_web_scraper.egg-info/SOURCES.txt` & `pro-football_reference_web_scraper-0.2.0/pro_football_reference_web_scraper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 .bumpversion.cfg
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 conftest.py
 pyproject.toml
 setup.py
+docs/.readthedocs.yaml
 docs/CONTRIBUTING.md
 docs/Makefile
 docs/README.md
 docs/conf.py
 docs/get_player_game_log.md
 docs/get_team_game_log.md
 docs/index.md
 docs/make.bat
 docs/requirements.txt
+docs/team_splits.md
 docs/source/modules.rst
 docs/source/pro_football_reference_web_scraper.rst
 pro_football_reference_web_scraper/__init__.py
 pro_football_reference_web_scraper/_version.py
 pro_football_reference_web_scraper/player_game_log.py
+pro_football_reference_web_scraper/player_splits.py
 pro_football_reference_web_scraper/team_game_log.py
+pro_football_reference_web_scraper/team_splits.py
 pro_football_reference_web_scraper.egg-info/PKG-INFO
 pro_football_reference_web_scraper.egg-info/SOURCES.txt
 pro_football_reference_web_scraper.egg-info/dependency_links.txt
 pro_football_reference_web_scraper.egg-info/requires.txt
 pro_football_reference_web_scraper.egg-info/top_level.txt
 tests/test_player_game_log_integration.py
 tests/test_player_game_log_unit.py
+tests/test_player_splits_integration.py
+tests/test_player_splits_unit.py
 tests/test_team_game_log_integration.py
-tests/test_team_game_log_unit.py
+tests/test_team_game_log_unit.py
+tests/test_team_splits_integration.py
+tests/test_team_splits_unit.py
```

### Comparing `pro-football_reference_web_scraper-0.1.1/pyproject.toml` & `pro-football_reference_web_scraper-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pro-football_reference_web_scraper"
 authors = [{name = "Matthew Kim", email = "mjk2244@columbia.edu"}]
 description="Stats web scraper of Pro Football Reference"
 readme = "README.md"
-version = "0.1.1"
+version = "0.2.0"
 requires-python = ">=3.8"
 
 dependencies = ["beautifulsoup4>=4.9.0",
                 "requests>=2.28.2",
                 "pandas>=1.5.3",
                 "haversine>=2.4.0"]
```

### Comparing `pro-football_reference_web_scraper-0.1.1/tests/test_player_game_log_unit.py` & `pro-football_reference_web_scraper-0.2.0/tests/test_player_game_log_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,30 +44,32 @@
         <td data-stat='pass_rating'>87.3</td><td data-stat='pass_sacked'>2</td><td data-stat='rush_att'>1</td>
         <td data-stat='rush_yds'>1</td><td data-stat='rush_td'>1</td></tr></tbody>"""
         soup = BeautifulSoup(fake_html, "html.parser")
 
         # fake dataframe to check with returned dataframe
         fake_df = pd.DataFrame(
             {
-                "Date": ["2022-09-11"],
-                "Week": [1],
-                "Team": ["TAM"],
-                "Game_Location": ["@"],
-                "Opp": ["DAL"],
-                "Result": ["W 19-3"],
-                "Cmp": [18],
-                "Att": [27],
-                "Pass_Yds": [212],
-                "Pass_TD": [1],
-                "Int": [1],
-                "Rating": [87.3],
-                "Sacked": [2],
-                "Rush_Att": [1],
-                "Rush_Yds": [1],
-                "Rush_TD": [1],
+                "date": ["2022-09-11"],
+                "week": [1],
+                "team": ["TAM"],
+                "game_location": ["@"],
+                "opp": ["DAL"],
+                "result": ["W"],
+                "team_pts": [19],
+                "opp_pts": [3],
+                "cmp": [18],
+                "att": [27],
+                "pass_yds": [212],
+                "pass_td": [1],
+                "int": [1],
+                "rating": [87.3],
+                "sacked": [2],
+                "rush_att": [1],
+                "rush_yds": [1],
+                "rush_td": [1],
             }
         )
         # asserting that the returned dataframe is expected
 
         assert p.qb_game_log(soup).equals(fake_df)
 
     def test_rb_game_log(self):
@@ -78,26 +80,28 @@
         <td data-stat='rush_td'>212</td><td data-stat='targets'>1</td><td data-stat='rec_yds'>1</td>
         <td data-stat='rec_td'>1</td></tr></tbody>"""
         soup = BeautifulSoup(fake_html, "html.parser")
 
         # fake dataframe to check with returned dataframe
         fake_df = pd.DataFrame(
             {
-                "Date": ["2022-09-11"],
-                "Week": [1],
-                "Team": ["TAM"],
-                "Game_Location": ["@"],
-                "Opp": ["DAL"],
-                "Result": ["W 19-3"],
-                "Rush_Att": [18],
-                "Rush_Yds": [27],
-                "Rush_TD": [212],
-                "Tgt": [1],
-                "Rec_Yds": [1],
-                "Rec_TD": [1],
+                "date": ["2022-09-11"],
+                "week": [1],
+                "team": ["TAM"],
+                "game_location": ["@"],
+                "opp": ["DAL"],
+                "result": ["W"],
+                "team_pts": [19],
+                "opp_pts": [3],
+                "rush_att": [18],
+                "rush_yds": [27],
+                "rush_td": [212],
+                "tgt": [1],
+                "rec_yds": [1],
+                "rec_td": [1],
             }
         )
 
         # asserting that the returned dataframe is expected
         assert p.rb_game_log(soup).equals(fake_df)
 
     def test_wr_game_log(self):
@@ -108,23 +112,25 @@
         <td data-stat='rec_yds'>212</td><td data-stat='rec_td'>1</td><td data-stat='rec_yds'>1</td>
         <td data-stat='off_pct'>87%</td></tr></tbody>"""
         soup = BeautifulSoup(fake_html, "html.parser")
 
         # fake dataframe to check with returned dataframe
         fake_df = pd.DataFrame(
             {
-                "Date": ["2022-09-11"],
-                "Week": [1],
-                "Team": ["TAM"],
-                "Game_Location": ["@"],
-                "Opp": ["DAL"],
-                "Result": ["W 19-3"],
-                "Tgt": [18],
-                "Rec": [27],
-                "Rec_Yds": [212],
-                "Rec_TD": [1],
-                "Snap_Pct": [0.87],
+                "date": ["2022-09-11"],
+                "week": [1],
+                "team": ["TAM"],
+                "game_location": ["@"],
+                "opp": ["DAL"],
+                "result": ["W"],
+                "team_pts": [19],
+                "opp_pts": [3],
+                "tgt": [18],
+                "rec": [27],
+                "rec_yds": [212],
+                "rec_td": [1],
+                "snap_pct": [0.87],
             }
         )
 
         # asserting that the returned dataframe is expected
         assert p.wr_game_log(soup).equals(fake_df)
```

### Comparing `pro-football_reference_web_scraper-0.1.1/tests/test_team_game_log_integration.py` & `pro-football_reference_web_scraper-0.2.0/tests/test_team_game_log_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from pro_football_reference_web_scraper import team_game_log as t
+import pytest
+import time
 
 
 class TestClass:
     # INTEGRATION TESTS
     def test_get_team_game_log(self):
+        time.sleep(3)
         bills_game_log = t.get_team_game_log('Buffalo Bills', 2022)
 
         # the Bills only played 16 games in 2022 due to the cancellation of their Week 17 game
         assert len(bills_game_log.index) == 16
 
         # the Bills recorded 6361 total yards in 2022
         assert bills_game_log['tot_yds'].sum() == 6361
 
         w = 0
         for index, row in bills_game_log.iterrows():
             if row['result'] == 'W':
                 w += 1
         # the Bills won 13 games in 2022
         assert w == 13
+
+        # misspelled team name
+        with pytest.raises(Exception):
+            t.get_team_game_log('Bufalo Bills', 2022)
+
+        # invalid team-season combo
+        with pytest.raises(Exception):
+            t.get_team_game_log('Houston Texans', 2000)
```

### Comparing `pro-football_reference_web_scraper-0.1.1/tests/test_team_game_log_unit.py` & `pro-football_reference_web_scraper-0.2.0/tests/test_team_game_log_unit.py`

 * *Files identical despite different names*

