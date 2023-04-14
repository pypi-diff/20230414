# Comparing `tmp/tweakwcs-0.8.1.tar.gz` & `tmp/tweakwcs-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweakwcs-0.8.1.tar", last modified: Sat Dec 24 04:01:50 2022, max compression
+gzip compressed data, was "tweakwcs-0.8.2.tar", last modified: Fri Apr 14 04:51:20 2023, max compression
```

## Comparing `tweakwcs-0.8.1.tar` & `tweakwcs-0.8.2.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.668015 tweakwcs-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.656015 tweakwcs-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.660015 tweakwcs-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2022-12-24 04:01:50.668015 tweakwcs-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/azure-templates.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.660015 tweakwcs-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.660015 tweakwcs-0.8.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.660015 tweakwcs-0.8.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/_static/css/custom-tweakwcs.css
--rw-r--r--   0 runner    (1001) docker     (123)    13689 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.660015 tweakwcs-0.8.1/docs/exts/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/exts/numfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/rtd-pip-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.664015 tweakwcs-0.8.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/correctors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/imalign.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/linalg.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/linearfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/matchutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/wcsimage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/docs/source/wcsutils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.664015 tweakwcs-0.8.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/notebooks/align_fits_wcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-24 04:01:50.668015 tweakwcs-0.8.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3678 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.664015 tweakwcs-0.8.1/tweakwcs/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36947 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/correctors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34486 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/imalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    29953 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/linearfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    20438 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/matchutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.664015 tweakwcs-0.8.1/tweakwcs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.668015 tweakwcs-0.8.1/tweakwcs/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/convex_hull_proximity.cat
--rw-r--r--   0 runner    (1001) docker     (123)    84009 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/ref.cat
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/sparse-2dhist.fits
--rw-r--r--   0 runner    (1001) docker     (123)    18006 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis1.cat
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis1.hdr
--rw-r--r--   0 runner    (1001) docker     (123)    18006 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis2.cat
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis2.hdr
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/helper_correctors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_correctors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_imalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_jwst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_linearfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_matchutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_multichip_fitswcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_multichip_jwst.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_wcsimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tests/test_wcsutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/tpwcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.668015 tweakwcs-0.8.1/tweakwcs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/utils/jwst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    66074 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/wcsimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2022-12-24 04:01:40.000000 tweakwcs-0.8.1/tweakwcs/wcsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 04:01:50.664015 tweakwcs-0.8.1/tweakwcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2022-12-24 04:01:50.000000 tweakwcs-0.8.1/tweakwcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-24 04:01:50.000000 tweakwcs-0.8.1/tweakwcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 04:01:50.000000 tweakwcs-0.8.1/tweakwcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-24 04:01:50.000000 tweakwcs-0.8.1/tweakwcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-24 04:01:50.000000 tweakwcs-0.8.1/tweakwcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.898824 tweakwcs-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.898824 tweakwcs-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/azure-templates.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.898824 tweakwcs-0.8.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/_static/css/custom-tweakwcs.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13689 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/docs/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/exts/numfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/rtd-pip-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/correctors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/imalign.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/linalg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/linearfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/matchutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/wcsimage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/docs/source/wcsutils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/notebooks/align_fits_wcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3663 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/tweakwcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37191 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35833 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/imalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/linearfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20438 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/matchutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/tweakwcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/tweakwcs/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/convex_hull_proximity.cat
+-rw-r--r--   0 runner    (1001) docker     (123)    84009 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/ref.cat
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/sparse-2dhist.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis1.cat
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis2.cat
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis2.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/helper_correctors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_correctors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_imalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_jwst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_linearfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_matchutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_multichip_fitswcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_multichip_jwst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_wcsimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tests/test_wcsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/tpwcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.906824 tweakwcs-0.8.2/tweakwcs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/utils/jwst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69136 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/wcsimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 04:51:11.000000 tweakwcs-0.8.2/tweakwcs/wcsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:51:20.902824 tweakwcs-0.8.2/tweakwcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 04:51:20.000000 tweakwcs-0.8.2/tweakwcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-14 04:51:20.000000 tweakwcs-0.8.2/tweakwcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:51:20.000000 tweakwcs-0.8.2/tweakwcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 04:51:20.000000 tweakwcs-0.8.2/tweakwcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 04:51:20.000000 tweakwcs-0.8.2/tweakwcs.egg-info/top_level.txt
```

### Comparing `tweakwcs-0.8.1/.github/workflows/publish-to-pypi.yml` & `tweakwcs-0.8.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/.gitignore` & `tweakwcs-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/CHANGELOG.rst` & `tweakwcs-0.8.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 .. _release_notes:
 
 =============
 Release Notes
 =============
 
-.. 0.8.2 (unreleased)
+.. 0.8.3 (unreleased)
    ==================
 
+0.8.2 (13-April-2023)
+=====================
+
+- Added ``bb_policy`` argument to the ``WCSGroupCatalog`` to control when
+  to switch to an aproximate method of computing of the bounding polygon of
+  a group of images. The default value is set to 50. Also added equivalent
+  ``group_bb_policy`` argument to both ``fit_wcs`` and ``align_wcs``
+  functions. [#176]
+
+
 0.8.1 (23-December-2022)
 ========================
 
 - Fixed a bug in the ``XYXYMatch`` due to which bin size for the 2D histogram
   pre-match alignment did not account for the pixel scale in the tangent plane.
   This required a change in the API of ``XYXYMatch.__call__`` which now
   _must_ have ``tp_pscale`` as input and also inputs catalogs now _must_
```

### Comparing `tweakwcs-0.8.1/CODE_OF_CONDUCT.md` & `tweakwcs-0.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/LICENSE.txt` & `tweakwcs-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/PKG-INFO` & `tweakwcs-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweakwcs
-Version: 0.8.1
+Version: 0.8.2
 Summary: A package for correcting alignment errors in WCS objects
 Home-page: https://github.com/spacetelescope/tweakwcs
 Author: Mihai Cara
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Reports, https://github.com/spacetelescope/tweakwcs/issues/
 Project-URL: Source, https://github.com/spacetelescope/tweakwcs/
```

### Comparing `tweakwcs-0.8.1/README.rst` & `tweakwcs-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/azure-pipelines.yml` & `tweakwcs-0.8.2/azure-pipelines.yml`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - template: azure-templates.yml
   parameters:
     name: Windows
     os: windows
 
 - job: 'PEP8'
   pool:
-    vmImage: 'Ubuntu-18.04'
+    vmImage: 'ubuntu-latest'
 
   steps:
   - task: UsePythonVersion@0
     inputs:
       versionSpec: '3.x'
       architecture: 'x64'
 
@@ -40,15 +40,15 @@
       flake8
     displayName: 'Run check'
 
 
 - job: 'Publish'
   dependsOn: 'Linux'
   pool:
-    vmImage: 'Ubuntu-18.04'
+    vmImage: 'ubuntu-latest'
 
   steps:
   - task: UsePythonVersion@0
     inputs:
       versionSpec: '3.x'
       architecture: 'x64'
```

### Comparing `tweakwcs-0.8.1/azure-templates.yml` & `tweakwcs-0.8.2/azure-templates.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 jobs:
 - job: ${{ format(parameters.name) }}
   pool:
     ${{ if eq(parameters.os, 'windows') }}:
-      vmImage: windows-2019
+      vmImage: windows-latest
     ${{ if eq(parameters.os, 'macos') }}:
-      vmImage: macOS-10.15
+      vmImage: macOS-latest
     ${{ if eq(parameters.os, 'linux') }}:
-      vmImage: ubuntu-18.04
+      vmImage: ubuntu-latest
 
   strategy:
     matrix:
       Python38:
         python.version: '3.8'
       Python39:
         python.version: '3.9'
@@ -45,15 +45,17 @@
       displayName: freeze output
 
     - script: |
         pytest --cov=./ -v --junitxml=junit/test-results.xml
       displayName: run test
 
     - bash: |
-        codecov -t $codecov_token
+        curl -Os https://uploader.codecov.io/latest/linux/codecov
+        chmod +x codecov
+        ./codecov -t $codecov_token
       env:
         codecov_token: $(CODECOV_TOKEN)
       condition: ne( variables['Agent.OS'], 'Windows_NT' )
       displayName: codecov upload on Linux/Darwin
 
     - powershell: |
         codecov -t "$(CODECOV_TOKEN)"
```

### Comparing `tweakwcs-0.8.1/docs/Makefile` & `tweakwcs-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/docs/conf.py` & `tweakwcs-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/docs/exts/numfig.py` & `tweakwcs-0.8.2/docs/exts/numfig.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/docs/index.rst` & `tweakwcs-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/docs/make.bat` & `tweakwcs-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/notebooks/align_fits_wcs.ipynb` & `tweakwcs-0.8.2/notebooks/align_fits_wcs.ipynb`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/setup.cfg` & `tweakwcs-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/setup.py` & `tweakwcs-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     'spherical_geometry>=1.2.20',
     'packaging>=19.0',
 ]
 
 TESTS_REQUIRE = [
     'pytest',
     'pytest-cov',
-    'codecov',
     'scipy'
 ]
 
 DOCS_REQUIRE = [
     'numpydoc',
     'sphinx',
     'sphinx-automodapi',
```

### Comparing `tweakwcs-0.8.1/tweakwcs/__init__.py` & `tweakwcs-0.8.2/tweakwcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/correctors.py` & `tweakwcs-0.8.2/tweakwcs/correctors.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,16 @@
 
         """
         return None
 
 
 class FITSWCSCorrector(WCSCorrector):
     """ A class for holding ``FITS`` ``WCS`` information and for managing
-    tangent-plane corrections.
+    tangent-plane corrections. The units of the tangent plane of this
+    corrector are same as detector coordinates.
 
     .. note::
         Currently only WCS objects that have ``CPDIS``, ``DET2IM``, and ``SIP``
         distortions *before* the application of the ``CD`` or ``PC`` matrix are
         supported.
 
     """
@@ -553,15 +554,17 @@
             return m
 
     return None
 
 
 class JWSTWCSCorrector(WCSCorrector):
     """ A class for holding ``JWST`` ``gWCS`` information and for managing
-    tangent-plane corrections.
+    tangent-plane corrections. The units of the tangent plane of this
+    corrector are ``arcsec`` and the axes are not along parallel to the
+    axes of the detector's coordinate system.
 
     """
     units = 'arcsec'
 
     def __init__(self, wcs, wcsinfo, meta=None):
         """
         Parameters
```

### Comparing `tweakwcs-0.8.1/tweakwcs/imalign.py` & `tweakwcs-0.8.2/tweakwcs/imalign.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 
 @deprecated_renamed_argument('tpwcs', 'corrector', since='0.8.0')
 def fit_wcs(refcat, imcat, corrector, ref_tpwcs=None, fitgeom='general',
-            nclip=3, sigma=(3.0, 'rmse'), clip_accum=False):
+            nclip=3, sigma=(3.0, 'rmse'), clip_accum=False,
+            group_bb_policy='auto'):
     """ "Tweak" **a single** image's ``WCS`` by fitting image catalog to a
     reference catalog. This is a simplified version of `align_wcs` that does
     not perform matching and is limited to the fitting part.
 
     .. note::
         Both reference and image catalogs must have been **matched**
         *prior to* calling ``fit_wcs()``. This means that the lengths of both
@@ -106,14 +107,23 @@
         Indicates whether or not to reset the list of "bad" (clipped out)
         sources after each clipping iteration. When set to `True` the list
         only grows with each iteration as "bad" positions never re-enter
         the pool of available position for the fit. By default the list of
         "bad" source positions is purged at each iteration. This parameter
         is ignored when ``nclip`` is either `None` or 0.
 
+    group_bb_policy: int, {'exact', 'auto'}
+        Describes how to compute the bounding polygon of the group.
+        ``'exact'`` will compute the exact union of bounding boxes of
+        input ``images``. An integer number will *approximate* the bounding
+        box using convex hull if the number of input ``images``
+        is exceeds the value of ``group_bb_policy`` and it will switch to exact
+        computations (using unions) otherwise. ``'auto'`` is the same as
+        setting threshold to 50.
+
     Returns
     -------
     twwcs: WCSCorrector
         "Tweaked" (aligned) ``WCS`` that contains tangent-plane corrections
         so that reference and image catalog sources better align in the tangent
         plane and therefore on the sky as well.
 
@@ -152,15 +162,15 @@
         ``[0.25,0.25,0.25,0.25,0.5,0.5]``.
 
     Upon **successful** completion, this function will set the ``'fit_info'``
     key value of the ``meta`` attribute of the returned ``WCSCorrector``
     object. ``'fit_info'`` is a dictionary with the following items:
 
         * **'shift'**: A ``numpy.ndarray`` with two components of the
-          computed shift.
+          computed shift. Note: shift is in units of the *tangent plane*.
 
         * **'matrix'**: A ``2x2`` ``numpy.ndarray`` with the computed
           generalized rotation matrix.
 
         * **'proper_rot'**: Rotation angle (degree) as if the rotation is
           proper.
 
@@ -246,15 +256,19 @@
         raise ValueError(
             "Unsupported 'fitgeom'. Valid values are: "
             f"{_SUPPORTED_FITGEOM_EN_STR:s}"
         )
 
     wimcat = WCSImageCatalog(imcat, corrector,
                              name=imcat.meta.get('name', 'Unnamed'))
-    wgcat = WCSGroupCatalog(wimcat, name=imcat.meta.get('name', 'Unnamed'))
+    wgcat = WCSGroupCatalog(
+        wimcat,
+        name=imcat.meta.get('name', 'Unnamed'),
+        bb_policy=group_bb_policy
+    )
     wrefcat = RefCatalog(refcat, name=imcat.meta.get('name', 'Unnamed'))
 
     succes = wgcat.align_to_ref(
         refcat=wrefcat,
         ref_tpwcs=ref_tpwcs,
         match=None,
         minobj=None,
@@ -279,15 +293,15 @@
 
     return wgcat[0].corrector
 
 
 def align_wcs(wcscat, refcat=None, ref_tpwcs=None, enforce_user_order=True,
               expand_refcat=False, minobj=None, match=XYXYMatch(),
               fitgeom='general', nclip=3, sigma=(3.0, 'rmse'),
-              clip_accum=False):
+              clip_accum=False, group_bb_policy='auto'):
     r"""
     Align (groups of) image catalogs by adjusting the parameters of their
     WCS based on fits between matched sources in these catalogs and a reference
     catalog which may be automatically created from one of the input ``wcscat``
     catalogs.
 
     .. warning::
@@ -428,14 +442,23 @@
         Indicates whether or not to reset the list of "bad" (clipped out)
         sources after each clipping iteration. When set to `True` the list
         only grows with each iteration as "bad" positions never re-enter
         the pool of available position for the fit. By default the list of
         "bad" source positions is purged at each iteration. This parameter
         is ignored when ``nclip`` is either `None` or 0.
 
+    group_bb_policy: int, {'exact', 'auto'}
+        Describes how to compute the bounding polygon of the group.
+        ``'exact'`` will compute the exact union of bounding boxes of
+        input ``images``. An integer number will *approximate* the bounding
+        box using convex hull if the number of input ``images``
+        is exceeds the value of ``group_bb_policy`` and it will switch to exact
+        computations (using unions) otherwise. ``'auto'`` is the same as
+        setting threshold to 50.
+
     Returns
     -------
     eff_refcat: astropy.table.Table
         Effective reference catalog used for aligning all images. Depending
         on the values of the input parameters ``refcat``,
         ``enforce_user_order``, and ``expand_refcat``, effective
         reference catalog may be one of the input image catalogs, the original
@@ -594,21 +617,26 @@
 
     # create WCSImageCatalog and WCSGroupCatalog:
     wcs_gcat = []
     for group_id, wcatalogs in grouped_images.items():
         if group_id is None:
             for wcat in wcatalogs:
                 wcs_gcat.append(
-                    WCSGroupCatalog(wcat, name='GROUP ID: None')
+                    WCSGroupCatalog(
+                        wcat,
+                        name='GROUP ID: None',
+                        bb_policy=group_bb_policy
+                    )
                 )
 
         else:
             gcat = WCSGroupCatalog(
                 wcatalogs,
-                name='GROUP ID: {}'.format(group_id)
+                name='GROUP ID: {}'.format(group_id),
+                bb_policy=group_bb_policy
             )
             if not len(gcat.catalog):
                 log.warning("Group with ID '{}' will not be aligned: empty "
                             "source catalog".format(group_id))
 
                 for wcat in wcatalogs:
                     wcat.corrector.meta['fit_info'] = {
```

### Comparing `tweakwcs-0.8.1/tweakwcs/linalg.py` & `tweakwcs-0.8.2/tweakwcs/linalg.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/linearfit.py` & `tweakwcs-0.8.2/tweakwcs/linearfit.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/matchutils.py` & `tweakwcs-0.8.2/tweakwcs/matchutils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/conftest.py` & `tweakwcs-0.8.2/tweakwcs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/convex_hull_proximity.cat` & `tweakwcs-0.8.2/tweakwcs/tests/data/convex_hull_proximity.cat`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/ref.cat` & `tweakwcs-0.8.2/tweakwcs/tests/data/ref.cat`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/sparse-2dhist.fits` & `tweakwcs-0.8.2/tweakwcs/tests/data/sparse-2dhist.fits`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis1.cat` & `tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis1.cat`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis1.hdr` & `tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis1.hdr`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis2.cat` & `tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis2.cat`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/data/wfc3_uvis2.hdr` & `tweakwcs-0.8.2/tweakwcs/tests/data/wfc3_uvis2.hdr`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/helper_correctors.py` & `tweakwcs-0.8.2/tweakwcs/tests/helper_correctors.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_correctors.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_correctors.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_imalign.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_imalign.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_jwst_utils.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_jwst_utils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_linalg.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_linearfit.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_linearfit.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_matchutils.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_matchutils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_multichip_fitswcs.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_multichip_fitswcs.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_multichip_jwst.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_multichip_jwst.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_wcsimage.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_wcsimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,31 @@
                                WCSGroupCatalog, _is_int)
 from astropy.utils.data import get_pkg_data_filename
 
 
 _ATOL = 100 * np.finfo(np.array([1.]).dtype).eps
 
 
+def _same_spherical_polygons(p1, p2):
+    p1 = np.array(list(p1.points), dtype=float)
+    p2 = np.array(list(p2.points), dtype=float)
+
+    if p1.shape != p2.shape:
+        return False
+
+    idx = np.argmin(np.linalg.norm(p1[0] - p2, axis=1))
+
+    if idx > 0:
+        p1 = p1[:-1]
+        p2 = p2[:-1]
+        p2 = np.roll(p2, -idx, axis=0)
+
+    return np.allclose(p1, p2, atol=_ATOL, rtol=0)
+
+
 @pytest.fixture
 def rect_cat(scope='function'):
     x = np.array([0.0, 0.0, 10.0, 10.0, 0.0]) - 5
     y = np.array([0.0, 10.0, 10.0, 0.0, 0.0]) - 5
     imcat = Table([x, y], names=('x', 'y'))
     return imcat
 
@@ -288,14 +305,33 @@
 
     # artificially set all catalogs to empty table:
     for im in g:
         im._name = None
     assert not g.create_group_catalog()
 
 
+def test_wcsgroupcat_bb_policy(rect_imcat):
+    w1 = copy.deepcopy(rect_imcat)
+    w2 = copy.deepcopy(rect_imcat)
+    g = WCSGroupCatalog([w1, w2], bb_policy='exact')
+
+    # test approximation to bounding boxes using convex hull:
+    g_approx_bb = WCSGroupCatalog([w1, w2], bb_policy='auto')
+    assert _same_spherical_polygons(g.polygon, g_approx_bb.polygon)
+
+    g_approx_bb = WCSGroupCatalog([w1, w2], bb_policy=0)
+    assert _same_spherical_polygons(g.polygon, g_approx_bb.polygon)
+
+    with pytest.raises(ValueError) as e:
+        WCSGroupCatalog([w1, w2], bb_policy='wrong')
+    assert e.value.args[0].startswith(
+        "'bb_policy' must be either 'auto', 'exact'"
+    )
+
+
 def test_wcsgroupcat_recalc_catalog_radec(mock_fits_wcs, rect_imcat):
     ra, dec = mock_fits_wcs.all_pix2world(rect_imcat.catalog['x'],
                                           rect_imcat.catalog['y'], 0)
     refcat = Table([ra, dec], names=('RA', 'DEC'))
     ref = RefCatalog(refcat)
 
     wim1 = copy.deepcopy(rect_imcat)
```

### Comparing `tweakwcs-0.8.1/tweakwcs/tests/test_wcsutils.py` & `tweakwcs-0.8.2/tweakwcs/tests/test_wcsutils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/tpwcs.py` & `tweakwcs-0.8.2/tweakwcs/tpwcs.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/utils/jwst_utils.py` & `tweakwcs-0.8.2/tweakwcs/utils/jwst_utils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs/wcsimage.py` & `tweakwcs-0.8.2/tweakwcs/wcsimage.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 source catalogs.
 
 :Authors: Mihai Cara
 
 :License: :doc:`LICENSE`
 
 """
-import os
+from copy import deepcopy
 import logging
 import numbers
-from copy import deepcopy
+import os
+import sys
 
 import numpy as np
 from astropy import table
 from astropy.utils.decorators import deprecated, deprecated_renamed_argument
 from spherical_geometry.polygon import SphericalPolygon, MalformedPolygonError
 from gwcs.geometry import CartesianToSpherical, SphericalToCartesian
 
@@ -95,14 +96,21 @@
         self.img_bounding_dec = None
 
         self.meta = dict(meta)
         self._fit_info = {'status': 'SKIPPED'}
 
         self.corrector = corrector
         self.catalog = catalog
+        self._poly_area = None
+
+    @property
+    def poly_area(self):
+        """ Area of the bounding polygon (in srad).
+        """
+        return self._poly_area
 
     @property
     @deprecated("0.8.0", obj_type='property')
     def tpwcs(self):
         """ Get :py:class:`WCSCorrector` WCS. """
         return self._corr
 
@@ -382,51 +390,52 @@
             lx = -0.5
             ly = -0.5
             hx = max(1, int(np.ceil(np.amax(self._catalog['x'])))) - 0.5
             hy = max(1, int(np.ceil(np.amax(self._catalog['y'])))) - 0.5
 
         else:
             ((lx, hx), (ly, hy)) = self.corrector.bounding_box
+            # shrink BB so that we do not get NaNs due to rounding
+            # issues (pixels on the edge could outside the box)
+            lx += 0.5
+            hx -= 0.5
+            ly += 0.5
+            hy -= 0.5
 
         if stepsize is None:
-            nintx = 2
-            ninty = 2
+            nintx = 3
+            ninty = 3
         else:
             nintx = max(2, int(np.ceil((hx - lx) / stepsize)))
             ninty = max(2, int(np.ceil((hy - ly) / stepsize)))
 
-        xs = np.linspace(lx, hx, nintx, dtype=np.double)
-        ys = np.linspace(ly, hy, ninty, dtype=np.double)[1:-1]
+        xs = np.linspace(lx, hx, nintx + 1, dtype=np.double)
+        ys = np.linspace(ly, hy, ninty + 1, dtype=np.double)[1:-1]
         nptx = xs.size
         npty = ys.size
 
-        npts = 2 * (nptx + npty)
-
-        borderx = np.empty((npts + 1,), dtype=np.double)
-        bordery = np.empty((npts + 1,), dtype=np.double)
-
-        # "bottom" points:
-        borderx[:nptx] = xs
-        bordery[:nptx] = ly
-        # "right"
-        sl = np.s_[nptx:nptx + npty]
-        borderx[sl] = hx
-        bordery[sl] = ys
-        # "top"
-        sl = np.s_[nptx + npty:2 * nptx + npty]
-        borderx[sl] = xs[::-1]
-        bordery[sl] = hy
-        # "left"
-        sl = np.s_[2 * nptx + npty:-1]
-        borderx[sl] = lx
-        bordery[sl] = ys[::-1]
-
-        # close polygon:
-        borderx[-1] = borderx[0]
-        bordery[-1] = bordery[0]
+        # bottom
+        borderx = [x for x in xs]
+        bordery = nptx * [ly]
+
+        # right
+        borderx.extend(npty * [hx])
+        bordery.extend(ys)
+
+        # top:
+        borderx.extend(xs[::-1])
+        bordery.extend(nptx * [hy])
+
+        # left:
+        borderx.extend(npty * [lx])
+        bordery.extend(ys[::-1])
+
+        # close:
+        borderx.append(borderx[0])
+        bordery.append(bordery[0])
 
         ra, dec = self.det_to_world(borderx, bordery)
         # TODO: for strange reasons, occasionally ra[0] != ra[-1] and/or
         #       dec[0] != dec[-1] (even though we close the polygon in the
         #       previous two lines). Then SphericalPolygon fails because
         #       points are not closed. Therefore we force it to be closed:
         ra[-1] = ra[0]
@@ -454,15 +463,15 @@
                 "Unexpected error: Contact software developer"
             )
 
         elif len(x) > 2:
             ra, dec = convex_hull(
                 x, y,
                 wcs=self.det_to_world,
-                min_separation=1e-8
+                min_separation=1e-11
             )
             # else, for len(x) in [1, 2], use entire image footprint.
             # TODO: a more robust algorithm should be implemented to deal with
             #       len(x) in [1, 2] cases.
 
             self._bb_radec = (ra, dec)
             self._polygon = SphericalPolygon.from_radec(ra, dec)
@@ -480,41 +489,55 @@
         # create smallest convex spherical polygon bounding all sources:
         if self.catalog:
             self._calc_cat_convex_hull()
 
     @property
     def bb_radec(self):
         """
-        Get a 2xN `numpy.ndarray` of RA and DEC of the vertices of the
+        Get a tuple of `numpy.ndarray` of RA and DEC of the vertices of the
         bounding polygon.
 
         """
         return self._bb_radec
 
 
 class WCSGroupCatalog(object):
     """
     A class that holds together `WCSImageCatalog` image catalog objects
     whose relative positions are fixed and whose source catalogs should be
     fitted together to a reference catalog.
 
     """
 
-    def __init__(self, images, name=None):
+    bb_approx_threshold = 50
+
+    def __init__(self, images, name=None, bb_policy='auto'):
         """
         Parameters
         ----------
         images: list of WCSImageCatalog
             A list of `WCSImageCatalog` image catalogs.
 
         name: str, None, optional
             Name of the group.
 
+        bb_policy: int, {'exact', 'auto'}
+            Describes how to compute the bounding polygon of the group.
+            ``'exact'`` will compute the exact union of bounding boxes of
+            input ``images``. An integer number will *approximate* the bounding
+            box using convex hull if the number of input ``images``
+            is exceeds the value of ``bb_policy`` and it will switch to exact
+            computations (using unions) otherwise. ``'auto'`` is the same as
+            setting threshold to 50.
+
         """
         self._catalog = None
+        self._name = name
+        self._poly_area = None
+        self.bb_policy = bb_policy
 
         if isinstance(images, WCSImageCatalog):
             self._images = [images]
             if images.catalog is None:
                 raise ValueError("Each input WCS image catalog must have a "
                                  "valid catalog.")
 
@@ -533,29 +556,57 @@
                 self._images.append(im)
 
         else:
             raise TypeError("Parameter 'images' must be either a single "
                             "'WCSImageCatalog' object or a list of "
                             "'WCSImageCatalog' objects")
 
-        self._name = name
         self._catalog = self.create_group_catalog()
         self.update_bounding_polygon()
 
     @property
+    def poly_area(self):
+        """ Area of the bounding polygon (in srad).
+        """
+        return self._poly_area
+
+    @property
     def name(self):
         """ Get/set :py:class:`WCSImageCatalog` object's name.
         """
         return self._name
 
     @name.setter
     def name(self, name):
         self._name = name
 
     @property
+    def bb_policy(self):
+        """ Get/set :py:class:`WCSImageCatalog` policy for switching to
+        approximate computation of group's bounding box.
+        """
+        return self._bb_policy
+
+    @bb_policy.setter
+    def bb_policy(self, bb_policy):
+        if bb_policy == 'auto':
+            self._bb_threshold = WCSGroupCatalog.bb_approx_threshold
+        elif bb_policy == 'exact':
+            self._bb_threshold = sys.maxsize
+        elif _is_int(bb_policy) and bb_policy >= 0:
+            self._bb_threshold = bb_policy
+        else:
+            raise ValueError(
+                "'bb_policy' must be either 'auto', 'exact', or "
+                "a non-negative integer number."
+            )
+
+        self._bb_policy = bb_policy
+
+    @property
     def polygon(self):
         """ Get image's (or catalog's) bounding spherical polygon.
         """
         return self._polygon
 
     def intersection(self, wcsim):
         """
@@ -604,18 +655,55 @@
         Calculate the area of the intersection polygon. If some
         intersections fail due to a bug/limitation of ``spherical_geometry``
         then the area of the valid intersections will be returned.
         If images do not intersect or intersection fails, 0 will be returned.
         """
         return sum(im._guarded_intersection_area(wcsim) for im in self._images)
 
+    def _aproximate_bb(self):
+        if not self._images:
+            return
+
+        tanplane_wcs = deepcopy(self._images[0].corrector)
+        tanplane_wcs.wcs.bounding_box = None
+
+        tpx = []
+        tpy = []
+
+        for im in self._images:
+            if im.corrector is None or im.bb_radec is None:
+                return
+
+            r, d = im.bb_radec
+            tx, ty = tanplane_wcs.world_to_tanp(r, d)
+            tpx.extend(tx)
+            tpy.extend(ty)
+
+        ra, dec = convex_hull(
+            tpx,
+            tpy,
+            wcs=tanplane_wcs.tanp_to_world,
+            min_separation=1e-11
+        )
+
+        self.img_bounding_ra = ra
+        self.img_bounding_dec = dec
+        self._bb_radec = (ra, dec)
+        self._polygon = SphericalPolygon.from_radec(ra, dec)
+        self._poly_area = np.fabs(self._polygon.area())
+
     def update_bounding_polygon(self):
         """ Recompute bounding polygons of the member images.
         """
+        if len(self._images) > self._bb_threshold:
+            self._aproximate_bb()
+            return
+
         polygons = [im.polygon for im in self._images]
+
         if polygons:
             try:
                 self._polygon = SphericalPolygon.multi_union(polygons)
             except MalformedPolygonError:
                 log.warning(
                     "MalformedPolygonError in spherical_geometry. Using "
                     "convex hull instead of multi_union. Alignment order "
@@ -623,14 +711,16 @@
                 )
                 refcat = RefCatalog(self._catalog)
                 self._polygon = refcat.polygon
 
         else:
             self._polygon = SphericalPolygon([])
 
+        self._poly_area = np.fabs(self._polygon.area())
+
     def __len__(self):
         return len(self._images)
 
     def __getitem__(self, idx):
         return self._images[idx]
 
     def __iter__(self):
@@ -1102,15 +1192,16 @@
         Upon successful return, this function will also set the following
         fields of the ``fit_info`` attribute of each member
         `WCSImageCatalog` object:
 
             * **'fitgeom'**: the value of the ``fitgeom`` argument
             * **'eff_minobj'**: effective value of the ``minobj`` parameter
             * **'matrix'**: computed rotation matrix
-            * **'shift'**: shift (offset) along X- and Y-axis
+            * **'shift'**: shift (offset) along X- and Y-axis in units of the
+              *tangent plane* coordinates.
             * **'rot'**: A tuple of ``(rotx, roty)`` - the rotation angles with
               regard to the ``X`` and ``Y`` axes.
             * **'<rot>'**: *Arithmetic mean* of the angles of rotation around
               ``X`` and ``Y`` axes.
             * **'proper_rot'**: rotation angle as if rotation is a proper
               rotation.
             * **'proper'**: Indicates whether the rotation is a proper rotation
@@ -1157,14 +1248,20 @@
 
         .. note::
             A ``'SUCCESS'`` status does not indicate a "good" alignment. It
             simply indicates that alignment algortithm has completed without
             errors. Use other fields to evaluate alignment: fit ``RMSE``
             and ``MAE`` values, number of matched sources, etc.
 
+        .. note::
+            Many quantities in ``fit_info`` are in units of the *tangent plane*
+            coordinates, e.g., ``shift``, ``rmse``, ``std``, ``mae``. See
+            specific ``WCSCorrector`` in `~tweakwcs.correctors` for the units
+            of the tangent plane.
+
         Parameters
         ----------
         refcat: RefCatalog
             A `RefCatalog` object that contains a catalog of reference sources.
 
         ref_tpwcs: WCSCorrector
             A `WCSCorrector` object that defines a projection tangent plane to
```

### Comparing `tweakwcs-0.8.1/tweakwcs/wcsutils.py` & `tweakwcs-0.8.2/tweakwcs/wcsutils.py`

 * *Files identical despite different names*

### Comparing `tweakwcs-0.8.1/tweakwcs.egg-info/PKG-INFO` & `tweakwcs-0.8.2/tweakwcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweakwcs
-Version: 0.8.1
+Version: 0.8.2
 Summary: A package for correcting alignment errors in WCS objects
 Home-page: https://github.com/spacetelescope/tweakwcs
 Author: Mihai Cara
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Reports, https://github.com/spacetelescope/tweakwcs/issues/
 Project-URL: Source, https://github.com/spacetelescope/tweakwcs/
```

### Comparing `tweakwcs-0.8.1/tweakwcs.egg-info/SOURCES.txt` & `tweakwcs-0.8.2/tweakwcs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 LICENSE.txt
 README.rst
 azure-pipelines.yml
 azure-templates.yml
 pyproject.toml
 setup.cfg
 setup.py
+.github/CODEOWNERS
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/rtd-pip-requirements.txt
 docs/_static/css/custom-tweakwcs.css
```

