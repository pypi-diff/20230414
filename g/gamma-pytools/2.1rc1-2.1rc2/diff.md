# Comparing `tmp/gamma-pytools-2.1rc1.tar.gz` & `tmp/gamma-pytools-2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma-pytools-2.1rc1.tar", last modified: Wed Oct 26 17:51:52 2022, max compression
+gzip compressed data, was "gamma-pytools-2.1rc2.tar", last modified: Fri Apr 14 14:29:38 2023, max compression
```

## Comparing `gamma-pytools-2.1rc1.tar` & `gamma-pytools-2.1rc2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0      666 2022-10-26 17:50:42.603389 gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      689 2022-10-26 17:50:42.603389 gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4728 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/.gitignore
--rw-r--r--   0        0        0     1065 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/LICENSE
--rw-r--r--   0        0        0     4077 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/README.rst
--rw-r--r--   0        0        0    13743 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    25508 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/azure-pipelines.yml
--rw-r--r--   0        0        0     1600 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/config/spelling.dic
--rwxr-xr-x   0        0        0       95 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/dev-setup.sh
--rw-r--r--   0        0        0      799 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/environment.yml
--rwxr-xr-x   0        0        0    20668 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/make.py
--rw-r--r--   0        0        0      757 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/mypy.ini
--rw-r--r--   0        0        0     1749 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/pypi_description.rst
--rw-r--r--   0        0        0     3001 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/pyproject.toml
--rw-r--r--   0        0        0       60 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/.gitignore
--rw-r--r--   0        0        0     1430 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/css/gamma.css
--rw-r--r--   0        0        0    28396 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/gamma_logo.png
--rw-r--r--   0        0        0     1867 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/js/gamma.js
--rw-r--r--   0        0        0      851 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1464 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/custom-module-template.rst
--rw-r--r--   0        0        0       64 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/getting-started-header.rst
--rw-r--r--   0        0        0     2783 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/bootstrap.py
--rw-r--r--   0        0        0     8061 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/conf_base.py
--rwxr-xr-x   0        0        0    17644 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/make_base.py
--rw-r--r--   0        0        0     1212 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/make_util.py
--rwxr-xr-x   0        0        0      285 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/make.py
--rw-r--r--   0        0        0    16224 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/_images/gamma_pytools_logo.png
--rw-r--r--   0        0        0       89 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      449 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/conf.py
--rw-r--r--   0        0        0    16543 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     1157 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      270 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/index.rst
--rw-r--r--   0        0        0      118 2022-10-26 17:50:43.675397 gamma-pytools-2.1rc1/src/pytools/__init__.py
--rw-r--r--   0        0        0      209 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/__init__.py
--rw-r--r--   0        0        0    12196 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_alltracker.py
--rw-r--r--   0        0        0    16056 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_api.py
--rw-r--r--   0        0        0     4872 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_decorators.py
--rw-r--r--   0        0        0     8591 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_doc_validator.py
--rw-r--r--   0        0        0      104 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/doc/__init__.py
--rw-r--r--   0        0        0    10806 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/doc/_doc.py
--rw-r--r--   0        0        0      142 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/__init__.py
--rw-r--r--   0        0        0     9732 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_linkage.py
--rw-r--r--   0        0        0    14286 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_matrix.py
--rw-r--r--   0        0        0     8423 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_simulation.py
--rw-r--r--   0        0        0       71 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/linkage/__init__.py
--rw-r--r--   0        0        0     4040 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/linkage/_linkage.py
--rw-r--r--   0        0        0     2941 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/__init__.py
--rw-r--r--   0        0        0    19468 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/_expression.py
--rw-r--r--   0        0        0      136 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/atomic/__init__.py
--rw-r--r--   0        0        0     3794 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/atomic/_atomic.py
--rw-r--r--   0        0        0      113 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/base/__init__.py
--rw-r--r--   0        0        0    11032 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/base/_base.py
--rw-r--r--   0        0        0      521 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/__init__.py
--rw-r--r--   0        0        0     9060 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/_composite.py
--rw-r--r--   0        0        0      143 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/base/__init__.py
--rw-r--r--   0        0        0     3761 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/composite/base/_base.py
--rw-r--r--   0        0        0      125 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/formatter/__init__.py
--rw-r--r--   0        0        0    22319 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/formatter/_python.py
--rw-r--r--   0        0        0       64 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/operator/__init__.py
--rw-r--r--   0        0        0     7817 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/operator/_operator.py
--rw-r--r--   0        0        0      107 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/fit/__init__.py
--rw-r--r--   0        0        0     4059 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/fit/_fit.py
--rw-r--r--   0        0        0       51 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/meta/__init__.py
--rw-r--r--   0        0        0     2162 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/meta/_meta.py
--rw-r--r--   0        0        0      101 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/parallelization/__init__.py
--rw-r--r--   0        0        0    12349 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/parallelization/_parallelization.py
--rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/py.typed
--rw-r--r--   0        0        0      111 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/__init__.py
--rw-r--r--   0        0        0    12755 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/_sphinx.py
--rw-r--r--   0        0        0      109 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/util/__init__.py
--rw-r--r--   0        0        0    42554 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/util/_util.py
--rw-r--r--   0        0        0      101 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/__init__.py
--rw-r--r--   0        0        0      823 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/_strings.py
--rw-r--r--   0        0        0     7466 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/_text.py
--rw-r--r--   0        0        0      198 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/__init__.py
--rw-r--r--   0        0        0    11047 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_matplot.py
--rw-r--r--   0        0        0     2095 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_text.py
--rw-r--r--   0        0        0    11284 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_viz.py
--rw-r--r--   0        0        0       69 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/__init__.py
--rw-r--r--   0        0        0    12466 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/_color.py
--rw-r--r--   0        0        0     6475 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/_rgb.py
--rw-r--r--   0        0        0      119 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/__init__.py
--rw-r--r--   0        0        0     4948 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_draw.py
--rw-r--r--   0        0        0    16230 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_style.py
--rw-r--r--   0        0        0       76 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/__init__.py
--rw-r--r--   0        0        0     5042 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/_style.py
--rw-r--r--   0        0        0       97 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/__init__.py
--rw-r--r--   0        0        0     8204 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/_distribution.py
--rw-r--r--   0        0        0       68 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/__init__.py
--rw-r--r--   0        0        0     2392 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/_base.py
--rw-r--r--   0        0        0       86 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/__init__.py
--rw-r--r--   0        0        0    17783 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/_matrix.py
--rw-r--r--   0        0        0       62 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/__init__.py
--rw-r--r--   0        0        0     2255 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/_base.py
--rw-r--r--   0        0        0       79 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/util/__init__.py
--rw-r--r--   0        0        0     4912 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/util/_matplot.py
--rw-r--r--   0        0        0       28 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/__init__.py
--rw-r--r--   0        0        0      696 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/conftest.py
--rw-r--r--   0        0        0      109 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/paths.py
--rw-r--r--   0        0        0       28 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/__init__.py
--rw-r--r--   0        0        0     7710 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_api.py
--rw-r--r--   0        0        0     6420 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_data.py
--rw-r--r--   0        0        0     7100 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_expression.py
--rw-r--r--   0        0        0     2590 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_jobs.py
--rw-r--r--   0        0        0     3052 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_sphinx.py
--rw-r--r--   0        0        0      861 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_text.py
--rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/__init__.py
--rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/__init__.py
--rw-r--r--   0        0        0     3890 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/test_dendrogram.py
--rw-r--r--   0        0        0     4837 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/test_color.py
--rw-r--r--   0        0        0      504 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/test_import.py
--rw-r--r--   0        0        0      175 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/test_docs.py
--rw-r--r--   0        0        0     2251 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/tox.ini
--rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 gamma-pytools-2.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      689 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     4728 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/.gitignore
+-rw-r--r--   0        0        0     1065 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/LICENSE
+-rw-r--r--   0        0        0     4077 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/README.rst
+-rw-r--r--   0        0        0    14648 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0    26107 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/azure-pipelines.yml
+-rw-r--r--   0        0        0     1600 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/condabuild/meta.yaml
+-rw-r--r--   0        0        0        0 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/config/spelling.dic
+-rwxr-xr-x   0        0        0       95 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/dev-setup.sh
+-rw-r--r--   0        0        0      839 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/environment.yml
+-rwxr-xr-x   0        0        0    20668 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/make.py
+-rw-r--r--   0        0        0      757 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/mypy.ini
+-rw-r--r--   0        0        0     1749 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/pypi_description.rst
+-rw-r--r--   0        0        0     2959 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/sphinx/.gitignore
+-rw-r--r--   0        0        0     1430 2023-04-14 14:28:12.513831 gamma-pytools-2.1rc2/sphinx/base/_static/css/gamma.css
+-rw-r--r--   0        0        0    28396 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/_static/gamma_logo.png
+-rw-r--r--   0        0        0     1867 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/_static/js/gamma.js
+-rw-r--r--   0        0        0      851 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1464 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0       64 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/_templates/getting-started-header.rst
+-rw-r--r--   0        0        0     2783 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/bootstrap.py
+-rw-r--r--   0        0        0     8061 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/conf_base.py
+-rwxr-xr-x   0        0        0    17644 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/make_base.py
+-rw-r--r--   0        0        0     1212 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/base/make_util.py
+-rwxr-xr-x   0        0        0      285 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/make.py
+-rw-r--r--   0        0        0    16224 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/_images/gamma_pytools_logo.png
+-rw-r--r--   0        0        0       89 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/api_landing.rst
+-rw-r--r--   0        0        0      449 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/conf.py
+-rw-r--r--   0        0        0    16543 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/contribution_guide.rst
+-rw-r--r--   0        0        0     1157 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/faqs.rst
+-rw-r--r--   0        0        0      270 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/sphinx/source/index.rst
+-rw-r--r--   0        0        0      118 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/__init__.py
+-rw-r--r--   0        0        0    12196 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/_alltracker.py
+-rw-r--r--   0        0        0    16056 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/_api.py
+-rw-r--r--   0        0        0     4872 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/_decorators.py
+-rw-r--r--   0        0        0     8591 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/_doc_validator.py
+-rw-r--r--   0        0        0      104 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/doc/__init__.py
+-rw-r--r--   0        0        0    10806 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/api/doc/_doc.py
+-rw-r--r--   0        0        0      142 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/__init__.py
+-rw-r--r--   0        0        0     9732 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/_linkage.py
+-rw-r--r--   0        0        0    14288 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/_matrix.py
+-rw-r--r--   0        0        0     8423 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/_simulation.py
+-rw-r--r--   0        0        0       71 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/linkage/__init__.py
+-rw-r--r--   0        0        0     4040 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/data/linkage/_linkage.py
+-rw-r--r--   0        0        0     2941 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/__init__.py
+-rw-r--r--   0        0        0    19980 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/_expression.py
+-rw-r--r--   0        0        0      136 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/atomic/__init__.py
+-rw-r--r--   0        0        0     3794 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/atomic/_atomic.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/base/__init__.py
+-rw-r--r--   0        0        0    11032 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/base/_base.py
+-rw-r--r--   0        0        0      521 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/composite/__init__.py
+-rw-r--r--   0        0        0     9060 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/composite/_composite.py
+-rw-r--r--   0        0        0      143 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/composite/base/__init__.py
+-rw-r--r--   0        0        0     3761 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/composite/base/_base.py
+-rw-r--r--   0        0        0      125 2023-04-14 14:28:12.517832 gamma-pytools-2.1rc2/src/pytools/expression/formatter/__init__.py
+-rw-r--r--   0        0        0    22319 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/expression/formatter/_python.py
+-rw-r--r--   0        0        0       64 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/expression/operator/__init__.py
+-rw-r--r--   0        0        0     7817 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/expression/operator/_operator.py
+-rw-r--r--   0        0        0      107 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/fit/__init__.py
+-rw-r--r--   0        0        0     4059 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/fit/_fit.py
+-rw-r--r--   0        0        0       51 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/meta/__init__.py
+-rw-r--r--   0        0        0     2162 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/meta/_meta.py
+-rw-r--r--   0        0        0      101 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/parallelization/__init__.py
+-rw-r--r--   0        0        0    12349 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/parallelization/_parallelization.py
+-rw-r--r--   0        0        0        0 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/py.typed
+-rw-r--r--   0        0        0      111 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/sphinx/__init__.py
+-rw-r--r--   0        0        0    12755 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/sphinx/_sphinx.py
+-rw-r--r--   0        0        0      109 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/sphinx/util/__init__.py
+-rw-r--r--   0        0        0    42570 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/sphinx/util/_util.py
+-rw-r--r--   0        0        0      101 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/text/_strings.py
+-rw-r--r--   0        0        0     7466 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/text/_text.py
+-rw-r--r--   0        0        0      198 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/__init__.py
+-rw-r--r--   0        0        0    11047 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/_matplot.py
+-rw-r--r--   0        0        0     2095 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/_text.py
+-rw-r--r--   0        0        0    11284 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/_viz.py
+-rw-r--r--   0        0        0       69 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/color/__init__.py
+-rw-r--r--   0        0        0    12466 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/color/_color.py
+-rw-r--r--   0        0        0     6475 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/color/_rgb.py
+-rw-r--r--   0        0        0      119 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/__init__.py
+-rw-r--r--   0        0        0     4948 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/_draw.py
+-rw-r--r--   0        0        0    16230 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/_style.py
+-rw-r--r--   0        0        0       76 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/base/__init__.py
+-rw-r--r--   0        0        0     5042 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/base/_style.py
+-rw-r--r--   0        0        0       97 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/distribution/__init__.py
+-rw-r--r--   0        0        0     8204 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/distribution/_distribution.py
+-rw-r--r--   0        0        0       68 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/distribution/base/__init__.py
+-rw-r--r--   0        0        0     2392 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/distribution/base/_base.py
+-rw-r--r--   0        0        0       86 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/matrix/__init__.py
+-rw-r--r--   0        0        0    17783 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/matrix/_matrix.py
+-rw-r--r--   0        0        0       62 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/matrix/base/__init__.py
+-rw-r--r--   0        0        0     2255 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/matrix/base/_base.py
+-rw-r--r--   0        0        0       79 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/util/__init__.py
+-rw-r--r--   0        0        0     4912 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/src/pytools/viz/util/_matplot.py
+-rw-r--r--   0        0        0       28 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/conftest.py
+-rw-r--r--   0        0        0      109 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/paths.py
+-rw-r--r--   0        0        0       28 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/__init__.py
+-rw-r--r--   0        0        0     7710 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_api.py
+-rw-r--r--   0        0        0     6420 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_data.py
+-rw-r--r--   0        0        0     8018 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_expression.py
+-rw-r--r--   0        0        0     2590 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_jobs.py
+-rw-r--r--   0        0        0     3052 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_sphinx.py
+-rw-r--r--   0        0        0      861 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/test_text.py
+-rw-r--r--   0        0        0        0 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/viz/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/viz/dendrogram/__init__.py
+-rw-r--r--   0        0        0     3890 2023-04-14 14:28:12.521832 gamma-pytools-2.1rc2/test/test/pytools/viz/dendrogram/test_dendrogram.py
+-rw-r--r--   0        0        0     4837 2023-04-14 14:28:12.525832 gamma-pytools-2.1rc2/test/test/pytools/viz/test_color.py
+-rw-r--r--   0        0        0      504 2023-04-14 14:28:12.525832 gamma-pytools-2.1rc2/test/test/pytools/viz/test_import.py
+-rw-r--r--   0        0        0      175 2023-04-14 14:28:12.525832 gamma-pytools-2.1rc2/test/test/test_docs.py
+-rw-r--r--   0        0        0     2251 2023-04-14 14:28:12.525832 gamma-pytools-2.1rc2/tox.ini
+-rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 gamma-pytools-2.1rc2/PKG-INFO
```

### Comparing `gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `gamma-pytools-2.1rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `gamma-pytools-2.1rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/.gitignore` & `gamma-pytools-2.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/.pre-commit-config.yaml` & `gamma-pytools-2.1rc2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 repos:
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
       - id: black
         language: python_venv
         language_version: python39
 
-  - repo: https://gitlab.com/pycqa/flake8
+  - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         name: flake8
         entry: flake8 --config tox.ini
         language: python_venv
         language_version: python39
@@ -30,15 +30,15 @@
       - id: check-json
       - id: check-xml
       - id: check-yaml
         language: python_venv
         exclude: condabuild/meta.yaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.981
+    rev: v1.2.0
     hooks:
       - id: mypy
         files: src|sphinx|test
         language: python_venv
         language_version: python39
         additional_dependencies:
-          - numpy~=1.22
+          - numpy~=1.24
```

### Comparing `gamma-pytools-2.1rc1/LICENSE` & `gamma-pytools-2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/README.rst` & `gamma-pytools-2.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/RELEASE_NOTES.rst` & `gamma-pytools-2.1rc2/RELEASE_NOTES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,51 @@
   class being processed by *autodoc*.
 - API: new Sphinx callback :class:`.RenamePrivateArguments` to rename private
   “positional-only” arguments in a function's signature (with two leading underscores)
   back to their original names in the source code, so that *autodoc* can pick them up
   correctly.
 
 
+*pytools* 2.1
+-------------
+
+2.1.0
+~~~~~
+
+- API: new decorator :obj:`.fitted_only` to mark methods that may only be
+  called after their associated object has been fitted using :meth:`.FittableMixin.fit`.
+- API: remove method ``ensure_fitted`` from :class:`.FittableMixin`, which is no longer
+  needed due to the new decorator :obj:`.fitted_only`.
+- API: new Sphinx callback :class:`.TrackCurrentClass` to keep track of the current
+  class being processed by *autodoc*.
+- API: new Sphinx callback :class:`.RenamePrivateArguments` to rename private
+  “positional-only” arguments in a function's signature (with two leading underscores)
+  back to their original names in the source code, so that *autodoc* can pick them up
+  correctly.
+- API: :class:`.Expression` objects support plain text and HTML output in Jupyter
+  notebooks
+
+
 *pytools* 2.0
 -------------
 
-*pytools* 2.0 features enhanced visualisations together with additional API improvements,
+*pytools* 2 introduces enhanced visualisations along with additional API improvements,
 and is now subject to static type checking with |mypy|.
 
+
+2.0.6
+~~~~~
+
+- BUILD: add support for :mod:`pandas` |nbsp| 2.0 and above
+
+
 2.0.5
 ~~~~~
 
-- API: de-dent docstrings before processing them with the :obj:``.subsdoc`` decorator
+- API: de-dent docstrings before processing them with the :obj:`.subsdoc` decorator
 - FIX: in method :meth:`.AllTracker.resolve_forward_references`, unwrap functions before
   accessing their ``__globals__`` attribute
 
 
 2.0.4
 ~~~~~
```

### Comparing `gamma-pytools-2.1rc1/azure-pipelines.yml` & `gamma-pytools-2.1rc2/azure-pipelines.yml`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         displayName: 'isort'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install isort~=5.10
+              python -m pip install isort~=5.12
               python -m isort --check --diff .
             displayName: 'Run isort'
       - job:
         displayName: 'black'
         steps:
           - task: UsePythonVersion@0
             inputs:
@@ -83,39 +83,42 @@
         displayName: 'mypy'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install mypy~=0.981 numpy~=1.22
+              python -m pip install mypy~=1.2.0 numpy~=1.24
               python -m mypy src
             displayName: 'Run mypy'
 
   # detect whether the build config (pyproject.toml) was changed -> then we must run a build test
   - stage: detect_build_config_changes
     displayName: 'Pyproject.toml build config'
 
     jobs:
 
       - job: checkout_and_diff
         displayName: 'detect changes'
         steps:
           - checkout: self
+            fetchDepth: 2
 
           - task: Bash@3
             name: diff
             inputs:
               targetType: 'inline'
               script: |
+                set -eux
+
                 echo Repo: $(Build.DefinitionName)
                 cd $(System.DefaultWorkingDirectory)
-                files_changed=$(git diff $(Build.SourceVersion)^! --name-only)
+                files_changed=$(git diff $(Build.SourceVersion)^ --name-only)
                 echo "Files changed since last commit: ${files_changed}"
-                n_files_changed=$(git diff $(Build.SourceVersion)^! --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
+                n_files_changed=$(git diff $(Build.SourceVersion)^ --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
                 if [ ${n_files_changed} -gt 0 ]
                 then
                 build_changed=1
                 echo "build config has been changed"
                 else
                 build_changed=0
                 echo "build config is unchanged";
@@ -137,30 +140,35 @@
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
 
-                conda env create
-                conda activate $(project_name)-develop
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
 
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 pytest \
                    --cov $(project_name) \
                    --cov-config "tox.ini" \
@@ -405,16 +413,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             env:
               BRANCH_NAME: $(branchName)
@@ -470,16 +478,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             inputs:
               targetType: inline
@@ -597,36 +605,35 @@
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - task: InstallSSHKey@0
             inputs:
               knownHostsEntry: $(knownHostsEntry)
               sshPublicKey: $(sshPublicKey)
               sshKeySecureFile: 'deploy_docs_$(project_name)'
             displayName: 'Install the deploy SSH key'
 
-          - checkout: pytools
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
                 echo "Checking out github-pages"
                 git checkout --track origin/github-pages
 
                 # make sure we have a docs directory
                 mkdir -p docs/docs-version
 
                 echo "Current documentation contents:"
@@ -638,49 +645,54 @@
             displayName: 'Retrieve current documentation versions from github-pages'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
                 echo "Checking out $(branchName)"
                 git checkout $(branchName)
 
-                conda env create
-                conda activate $(project_name)-develop
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
 
-                export PYTHONPATH=$(System.DefaultWorkingDirectory)/$(project_root)/src/
+                export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
 
                 python sphinx/make.py html
 
             displayName: 'Build latest documentation'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
 
                 # install the tree utility
                 sudo apt-get install tree
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
 
                 echo "Restoring previous documentation to the docs directory"
                 mkdir -p docs
                 mv $(Build.ArtifactStagingDirectory)/docs-version.bak docs/docs-version
                 ls docs/docs-version
 
-                mkdir -p $(System.DefaultWorkingDirectory)/$(project_root)/sphinx/build/
+                mkdir -p $(System.DefaultWorkingDirectory)/sphinx/build/
 
-                conda activate $(project_name)-develop
+                micromamba activate $(project_name)-develop
                 python sphinx/make.py prepare_docs_deployment
 
                 echo "Current docs contents:"
                 tree docs
                 mv docs $(Build.ArtifactStagingDirectory)/docs
             displayName: 'Merge previous and latest docs'
 
@@ -704,15 +716,15 @@
 
           - task: Bash@3
             condition: eq(variables['source_is_release_branch'], 'True')
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
 
                 echo "Adjusting git credentials"
                 git config --global user.name "Azure Pipelines"
                 git config --global user.email "azuredevops@microsoft.com"
                 git config --global url.ssh://git@github.com/.insteadOf https://github.com/
                 git checkout github-pages
```

### Comparing `gamma-pytools-2.1rc1/condabuild/meta.yaml` & `gamma-pytools-2.1rc2/condabuild/meta.yaml`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/environment.yml` & `gamma-pytools-2.1rc2/environment.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 name: pytools-develop
 channels:
   - conda-forge
   - bcg_gamma
 dependencies:
   # run
-  - joblib ~= 1.1
-  - matplotlib ~= 3.5
-  - numpy ~= 1.22
-  - pandas ~= 1.4
+  - joblib ~= 1.2
+  - matplotlib ~= 3.6
+  - numpy ~= 1.23
+  - pandas ~= 2.0
   - python ~= 3.9
-  - scipy ~= 1.8
+  - scipy ~= 1.10
   - typing_extensions ~= 4.3
   - typing_inspect ~= 0.7
   # build/test
-  - conda-build ~= 3.21
-  - conda-verify ~= 3.1
-  - docutils ~= 0.17
-  - flit ~= 3.0
-  - jinja2 ~= 2.11
+  - conda-build ~= 3.23.3
+  - conda-verify ~= 3.1.1
+  - docutils ~= 0.17.1
+  - flit ~= 3.8.0
+  - jinja2 ~= 2.11.3
   - markupsafe ~= 2.0.1  # markupsafe 2.1 breaks support for jinja2
-  - m2r ~= 0.2
-  - pluggy ~= 0.13
-  - pre-commit ~= 2.20
-  - pytest ~= 7.1
-  - pytest-cov ~= 2.12
-  - pyyaml ~= 5.4
-  - toml ~= 0.10
-  - tox ~= 3.24
-  - yaml ~= 0.2
+  - m2r ~= 0.3.1
+  - pluggy ~= 0.13.1
+  - pre-commit ~= 2.21.0
+  - pytest ~= 7.2.1
+  - pytest-cov ~= 2.12.1
+  - pyyaml ~= 5.4.1
+  - toml ~= 0.10.2
+  - tox ~= 3.27.1
+  - yaml ~= 0.2.5
   # sphinx
-  - sphinx ~= 4.5
-  - sphinx-autodoc-typehints ~= 1.19
   - nbsphinx ~= 0.8.9
+  - sphinx ~= 4.5.0
+  - sphinx-autodoc-typehints ~= 1.19.2
   - pydata-sphinx-theme ~= 0.8.1
   # notebooks
-  - jupyterlab ~= 3.2
-  - openpyxl ~= 3.0
-  - seaborn ~= 0.11
+  - jupyterlab ~= 3.5.2
+  - openpyxl ~= 3.0.10
+  - seaborn ~= 0.12.2
```

### Comparing `gamma-pytools-2.1rc1/make.py` & `gamma-pytools-2.1rc2/make.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/mypy.ini` & `gamma-pytools-2.1rc2/mypy.ini`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/pypi_description.rst` & `gamma-pytools-2.1rc2/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/pyproject.toml` & `gamma-pytools-2.1rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 description-file = "pypi_description.rst"
 dist-name = "gamma-pytools"
 license = "Apache Software License v2.0"
 
 requires = [
     "joblib            >=0.14,<2a",
     "matplotlib        ~=3.0",
-    "numpy             >=1.21,<2a",
-    "pandas            >=0.24,<2a",
+    "numpy             >=1.21,<2a",  # cannot use ~= due to conda bug
+    "pandas            >=1",
     "scipy             ~=1.2",
     "typing_inspect    ~=0.4",
     "typing_extensions ~=4.0",
 ]
 
 requires-python = ">=3.7,<4a"
 
@@ -40,18 +40,15 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.flit.metadata.requires-extra]
 testing = [
     "pytest ~= 7.1",
-    "pytest-cov ~= 2.8",
-    "flake8 ~= 3.8",
-    "flake8-comprehensions ~= 3.2",
-    "isort ~= 5.5",
+    "pytest-cov ~= 2.12",
 ]
 docs = [
     "sphinx ~= 4.5",
     "sphinx-autodoc-typehints ~= 1.19",
     "pydata-sphinx-theme ~= 0.8.1",
     "jinja2 ~= 2.11",
     "nbsphinx ~= 0.8.9",
@@ -70,26 +67,26 @@
 no-binary.min = ["matplotlib"]
 
 [build.matrix.min]
 # minimum requirements of gamma-pytools
 joblib            = "~=0.14.0"
 matplotlib        = "~=3.0.3"
 numpy             = "==1.21.6"  # cannot use ~= due to conda bug
-pandas            = "~=0.24.2"
-python            = "==3.7.12"  # cannot use ~= due to conda bug
+pandas            = "~=1.0.5"
+python            = ">=3.7.12,<3.8a"    # cannot use ~= due to conda bug
 scipy             = "~=1.2.1"
 typing_inspect    = "~=0.4.0"
 typing_extensions = "~=4.0.0"
 
 [build.matrix.max]
 # maximum requirements of gamma-pytools
 joblib            = "~=1.1"
 matplotlib        = "~=3.5"
-numpy             = ">=1.23,<2a"  # cannot use ~= due to conda bug
-pandas            = "~=1.4"
+numpy             = ">=1.24,<2a"  # cannot use ~= due to conda bug
+pandas            = "~=2.0"
 python            = ">=3.9,<4a"   # cannot use ~= due to conda bug
 scipy             = "~=1.8"
 typing_inspect    = "~=0.7"
 typing_extensions = "~=4.3"
 
 [tool.black]
 # quiet = "True"
```

### Comparing `gamma-pytools-2.1rc1/sphinx/base/_static/css/gamma.css` & `gamma-pytools-2.1rc2/sphinx/base/_static/css/gamma.css`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/_static/gamma_logo.png` & `gamma-pytools-2.1rc2/sphinx/base/_static/gamma_logo.png`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/_static/js/gamma.js` & `gamma-pytools-2.1rc2/sphinx/base/_static/js/gamma.js`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/_templates/custom-class-template.rst` & `gamma-pytools-2.1rc2/sphinx/base/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/_templates/custom-module-template.rst` & `gamma-pytools-2.1rc2/sphinx/base/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/bootstrap.py` & `gamma-pytools-2.1rc2/sphinx/base/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/conf_base.py` & `gamma-pytools-2.1rc2/sphinx/base/conf_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/make_base.py` & `gamma-pytools-2.1rc2/sphinx/base/make_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/base/make_util.py` & `gamma-pytools-2.1rc2/sphinx/base/make_util.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/source/_images/gamma_pytools_logo.png` & `gamma-pytools-2.1rc2/sphinx/source/_images/gamma_pytools_logo.png`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/source/contribution_guide.rst` & `gamma-pytools-2.1rc2/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/sphinx/source/faqs.rst` & `gamma-pytools-2.1rc2/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/api/_alltracker.py` & `gamma-pytools-2.1rc2/src/pytools/api/_alltracker.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/api/_api.py` & `gamma-pytools-2.1rc2/src/pytools/api/_api.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/api/_decorators.py` & `gamma-pytools-2.1rc2/src/pytools/api/_decorators.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/api/_doc_validator.py` & `gamma-pytools-2.1rc2/src/pytools/api/_doc_validator.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/api/doc/_doc.py` & `gamma-pytools-2.1rc2/src/pytools/api/doc/_doc.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/data/_linkage.py` & `gamma-pytools-2.1rc2/src/pytools/data/_linkage.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/data/_matrix.py` & `gamma-pytools-2.1rc2/src/pytools/data/_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         def _arg_to_array(
             axis: int, axis_arg: Optional[Iterable[Any]], arg_name_: str
         ) -> Optional[npt.NDArray[Any]]:
             if axis_arg is None:
                 return None
             else:
-                arr = np.array(axis_arg)
+                arr = np.asarray(axis_arg)
                 if arr.ndim != 1:
                     raise ValueError(
                         f"arg {arg_name_}[{axis}] must be a 1d array, but has "
                         f"shape {arr.shape}"
                     )
                 if arr.shape != (values.shape[axis],):
                     raise ValueError(
```

### Comparing `gamma-pytools-2.1rc1/src/pytools/data/_simulation.py` & `gamma-pytools-2.1rc2/src/pytools/data/_simulation.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/data/linkage/_linkage.py` & `gamma-pytools-2.1rc2/src/pytools/data/linkage/_linkage.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/__init__.py` & `gamma-pytools-2.1rc2/src/pytools/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/_expression.py` & `gamma-pytools-2.1rc2/src/pytools/expression/_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Implementation of :mod:`pytools.expression` and subpackages.
 """
 from __future__ import annotations
 
 import logging
 from abc import ABCMeta, abstractmethod
-from typing import Any, Optional, Tuple, TypeVar
+from typing import Any, Dict, Optional, Tuple, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
 from ..api import AllTracker, inheritdoc, to_list
 from .operator import BinaryOperator, UnaryOperator
 
@@ -103,14 +103,27 @@
         return repr(self.to_expression())
 
     def __str__(self) -> str:
         # get the expression representing this object, and use the default formatter
         # to convert the expression to a formatted string
         return str(self.to_expression())
 
+    def _repr_html_(self) -> str:
+        # get the expression representing this object, and use the default formatter
+        # to convert the expression to HTML for Jupyter notebooks
+        return f"<pre>{self}\n</pre>\n"
+
+    def _repr_mimebundle_(self, **kwargs: Any) -> Dict[str, Any]:
+        # get plain text and HTML representations of this object
+        # for use in Jupyter notebooks
+        return {
+            "text/plain": str(self),
+            "text/html": self._repr_html_(),
+        }
+
 
 @inheritdoc(match="[see superclass]")
 class Expression(HasExpressionRepr, metaclass=ABCMeta):
     """
     A representation of an expression.
     """
```

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/atomic/_atomic.py` & `gamma-pytools-2.1rc2/src/pytools/expression/atomic/_atomic.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/base/_base.py` & `gamma-pytools-2.1rc2/src/pytools/expression/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/composite/__init__.py` & `gamma-pytools-2.1rc2/src/pytools/expression/composite/__init__.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/composite/_composite.py` & `gamma-pytools-2.1rc2/src/pytools/expression/composite/_composite.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/composite/base/_base.py` & `gamma-pytools-2.1rc2/src/pytools/expression/composite/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/formatter/_python.py` & `gamma-pytools-2.1rc2/src/pytools/expression/formatter/_python.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/expression/operator/_operator.py` & `gamma-pytools-2.1rc2/src/pytools/expression/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/fit/_fit.py` & `gamma-pytools-2.1rc2/src/pytools/fit/_fit.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/meta/_meta.py` & `gamma-pytools-2.1rc2/src/pytools/meta/_meta.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/parallelization/_parallelization.py` & `gamma-pytools-2.1rc2/src/pytools/parallelization/_parallelization.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/sphinx/_sphinx.py` & `gamma-pytools-2.1rc2/src/pytools/sphinx/_sphinx.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/sphinx/util/_util.py` & `gamma-pytools-2.1rc2/src/pytools/sphinx/util/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     # noinspection PyMissingOrEmptyDocstring,SpellCheckingInspection
     class _Text(_Element):
 
         rawsource: str
 
         # noinspection SpellCheckingInspection
-        def astext(self) -> str:
+        def astext(self) -> str:  # type: ignore
             ...
 
     Sphinx = type("Sphinx", (object,), {})
     Element = _Element
     Text = _Text
 
 
@@ -103,19 +103,19 @@
     "Replace3rdPartyDoc",
     "ResolveTypeVariables",
     "SkipIndirectImports",
     "TrackCurrentClass",
 ]
 
 #
-# Type aliases
+# Type variables
 #
 
-method_descriptor = type(str.__dict__["startswith"])
-wrapper_descriptor = type(str.__dict__["__add__"])
+method_descriptor: Type[Any] = type(str.startswith)
+wrapper_descriptor: Type[Any] = type(str.__add__)
 
 
 #
 # Constants
 #
 
 METHOD_TYPE_DYNAMIC = 0
```

### Comparing `gamma-pytools-2.1rc1/src/pytools/text/_strings.py` & `gamma-pytools-2.1rc2/src/pytools/text/_strings.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/text/_text.py` & `gamma-pytools-2.1rc2/src/pytools/text/_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/_matplot.py` & `gamma-pytools-2.1rc2/src/pytools/viz/_matplot.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/_text.py` & `gamma-pytools-2.1rc2/src/pytools/viz/_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/_viz.py` & `gamma-pytools-2.1rc2/src/pytools/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/color/_color.py` & `gamma-pytools-2.1rc2/src/pytools/viz/color/_color.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/color/_rgb.py` & `gamma-pytools-2.1rc2/src/pytools/viz/color/_rgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 __all__ = [
     "RgbColor",
     "RgbaColor",
 ]
 
 
 #
-# Type Aliases
+# Type aliases
 #
 TupleRgb: TypeAlias = Tuple[float, float, float]
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
```

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_draw.py` & `gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/_draw.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_style.py` & `gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/_style.py` & `gamma-pytools-2.1rc2/src/pytools/viz/dendrogram/base/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/distribution/_distribution.py` & `gamma-pytools-2.1rc2/src/pytools/viz/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/_base.py` & `gamma-pytools-2.1rc2/src/pytools/viz/distribution/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/matrix/_matrix.py` & `gamma-pytools-2.1rc2/src/pytools/viz/matrix/_matrix.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/_base.py` & `gamma-pytools-2.1rc2/src/pytools/viz/matrix/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/src/pytools/viz/util/_matplot.py` & `gamma-pytools-2.1rc2/src/pytools/viz/util/_matplot.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/conftest.py` & `gamma-pytools-2.1rc2/test/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_api.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_api.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_data.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_data.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_expression.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,42 @@
     expr_5 = Lambda(Id.x, body=e)(Lit(5))
     assert repr(expr_5) == "(lambda x: f((1 | 2) >> 'x' % x, abc=-5))(5)"
 
     expr_6 = Lambda(Id.x, Id.y, body=e)(Lit(5), 6)
     assert repr(expr_6) == "(lambda x, y: f((1 | 2) >> 'x' % x, abc=-5))(5, 6)"
 
 
+def test_expression_repr_html() -> None:
+
+    # create an expression
+    e = Call(Id.f, (1 | Lit(2)) >> Lit("x") % Id.x, abc=-Lit(5))
+    expr = e * (e + e + e - e * e)
+
+    # create the expected representations
+    expected_formatted_expression = """(
+    f((1 | 2) >> 'x' % x, abc=-5)
+    * (
+        f((1 | 2) >> 'x' % x, abc=-5)
+        + f((1 | 2) >> 'x' % x, abc=-5)
+        + f((1 | 2) >> 'x' % x, abc=-5)
+        - f((1 | 2) >> 'x' % x, abc=-5) * f((1 | 2) >> 'x' % x, abc=-5)
+    )
+)"""
+    expected_html_expression = f"<pre>{expected_formatted_expression}\n</pre>\n"
+
+    # test if the html representation is generated as expected
+    assert expr._repr_html_() == expected_html_expression
+
+    # test if the mimebundle representation is generated as expected
+    assert expr._repr_mimebundle_() == {
+        "text/html": expected_html_expression,
+        "text/plain": expected_formatted_expression,
+    }
+
+
 def test_expression() -> None:
     lit_5 = Lit(5)
     lit_abc = Lit("abc")
     expressions: List[Tuple[Expression, str]] = [
         (lit_5, "5"),
         (lit_abc, "'abc'"),
         (Id.xx, "xx"),
```

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_jobs.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_jobs.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_sphinx.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/test_text.py` & `gamma-pytools-2.1rc2/test/test/pytools/test_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/test_dendrogram.py` & `gamma-pytools-2.1rc2/test/test/pytools/viz/dendrogram/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/test/test/pytools/viz/test_color.py` & `gamma-pytools-2.1rc2/test/test/pytools/viz/test_color.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/tox.ini` & `gamma-pytools-2.1rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc1/PKG-INFO` & `gamma-pytools-2.1rc2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamma-pytools
-Version: 2.1rc1
+Version: 2.1rc2
 Summary: A collection of Python extensions and tools used in BCG GAMMA's open-source libraries.
 Home-page: https://github.com/BCG-Gamma/pytools
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,32 +19,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: joblib            >=0.14,<2a
 Requires-Dist: matplotlib        ~=3.0
 Requires-Dist: numpy             >=1.21,<2a
-Requires-Dist: pandas            >=0.24,<2a
+Requires-Dist: pandas            >=1
 Requires-Dist: scipy             ~=1.2
 Requires-Dist: typing_inspect    ~=0.4
 Requires-Dist: typing_extensions ~=4.0
 Requires-Dist: sphinx ~= 4.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ~= 1.19 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme ~= 0.8.1 ; extra == "docs"
 Requires-Dist: jinja2 ~= 2.11 ; extra == "docs"
 Requires-Dist: nbsphinx ~= 0.8.9 ; extra == "docs"
 Requires-Dist: jupyter == 1 ; extra == "docs"
 Requires-Dist: docutils ~= 0.17 ; extra == "docs"
 Requires-Dist: xlrd ~= 1.2 ; extra == "docs"
 Requires-Dist: m2r ~= 0.2 ; extra == "docs"
 Requires-Dist: pytest ~= 7.1 ; extra == "testing"
-Requires-Dist: pytest-cov ~= 2.8 ; extra == "testing"
-Requires-Dist: flake8 ~= 3.8 ; extra == "testing"
-Requires-Dist: flake8-comprehensions ~= 3.2 ; extra == "testing"
-Requires-Dist: isort ~= 5.5 ; extra == "testing"
+Requires-Dist: pytest-cov ~= 2.12 ; extra == "testing"
 Project-URL: Documentation, https://bcg-gamma.github.io/pytools/
 Project-URL: Repository, https://github.com/BCG-Gamma/pytools
 Provides-Extra: docs
 Provides-Extra: testing
 
 *pytools* is an open source library containing general machine learning and visualisation
 utilities for reuse, including:
```

