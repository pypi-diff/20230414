# Comparing `tmp/swarmpal-0.1.0.tar.gz` & `tmp/swarmpal-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmpal-0.1.0.tar", last modified: Thu Apr 13 22:32:34 2023, max compression
+gzip compressed data, was "swarmpal-0.1.0a4.tar", last modified: Thu Apr  6 20:13:39 2023, max compression
```

## Comparing `swarmpal-0.1.0.tar` & `swarmpal-0.1.0a4.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0      156 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.flake8
--rw-r--r--   0        0        0      316 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2511 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2091 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.gitignore
--rw-r--r--   0        0        0     2218 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      500 2023-04-13 22:26:16.773093 swarmpal-0.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     1092 2023-04-13 22:26:16.777093 swarmpal-0.1.0/CITATION.cff
--rw-r--r--   0        0        0     5495 2023-04-13 22:26:16.777093 swarmpal-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2518 2023-04-13 22:26:16.777093 swarmpal-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1067 2023-04-13 22:26:16.777093 swarmpal-0.1.0/LICENSE
--rw-r--r--   0        0        0     2162 2023-04-13 22:26:16.777093 swarmpal-0.1.0/README.md
--rw-r--r--   0        0        0      633 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1432 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/acknowledgements.md
--rw-r--r--   0        0        0      683 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/api/dsecs.rst
--rw-r--r--   0        0        0      244 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/api/fac.rst
--rw-r--r--   0        0        0      134 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/api/io.rst
--rw-r--r--   0        0        0      434 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/api/tfa.rst
--rw-r--r--   0        0        0      189 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0     3396 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      655 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/contributing.md
--rw-r--r--   0        0        0     6899 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/dsecs/intro_dsecs.ipynb
--rw-r--r--   0        0        0     4380 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/fac/intro_fac.ipynb
--rw-r--r--   0        0        0    10651 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/quickstart.ipynb
--rw-r--r--   0        0        0    11537 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/shared/paldata.ipynb
--rw-r--r--   0        0        0    11882 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/intro_tfa.ipynb
--rw-r--r--   0        0        0     4593 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_AUX_OBS.ipynb
--rw-r--r--   0        0        0     4282 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_Cluster.ipynb
--rw-r--r--   0        0        0     4269 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_EFIx_TCT.ipynb
--rw-r--r--   0        0        0     5044 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_MAGx_HR.ipynb
--rw-r--r--   0        0        0     6810 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_MAGx_LR.ipynb
--rw-r--r--   0        0        0     6484 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/guides/tfa/tfa_background.ipynb
--rw-r--r--   0        0        0      689 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/index.md
--rw-r--r--   0        0        0     2110 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/installation.md
--rw-r--r--   0        0        0      759 2023-04-13 22:26:16.777093 swarmpal-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      678 2023-04-13 22:26:16.777093 swarmpal-0.1.0/environment.yml
--rw-r--r--   0        0        0     1353 2023-04-13 22:26:16.777093 swarmpal-0.1.0/noxfile.py
--rw-r--r--   0        0        0     2579 2023-04-13 22:27:01.002640 swarmpal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/__init__.py
--rw-r--r--   0        0        0      216 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/io/__init__.py
--rw-r--r--   0        0        0     8280 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/io/_datafetchers.py
--rw-r--r--   0        0        0    16014 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/io/_paldata.py
--rw-r--r--   0        0        0        0 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/io/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/__init__.py
--rw-r--r--   0        0        0      149 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/__init__.py
--rw-r--r--   0        0        0    17840 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/aux_tools.py
--rw-r--r--   0        0        0    79676 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/dsecs_algorithms.py
--rw-r--r--   0        0        0     5558 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/processes.py
--rw-r--r--   0        0        0       71 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/fac/__init__.py
--rw-r--r--   0        0        0     4052 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/fac/fac_algorithms.py
--rw-r--r--   0        0        0     3789 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/fac/processes.py
--rw-r--r--   0        0        0      125 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/__init__.py
--rw-r--r--   0        0        0    10483 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/plotting.py
--rw-r--r--   0        0        0    18459 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/processes.py
--rw-r--r--   0        0        0    24364 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/tfalib.py
--rw-r--r--   0        0        0        0 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/utils/__init__.py
--rw-r--r--   0        0        0       35 2023-04-13 22:26:16.781093 swarmpal-0.1.0/src/swarmpal/utils/exceptions.py
--rw-r--r--   0        0        0     1536 2023-04-13 22:26:16.781093 swarmpal-0.1.0/tests/io/test_datafetchers.py
--rw-r--r--   0        0        0     5979 2023-04-13 22:26:16.781093 swarmpal-0.1.0/tests/io/test_paldata.py
--rw-r--r--   0        0        0     1943 2023-04-13 22:26:16.781093 swarmpal-0.1.0/tests/io/test_palprocess.py
--rw-r--r--   0        0        0      478 2023-04-13 22:26:16.785094 swarmpal-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 swarmpal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/.flake8
+-rw-r--r--   0        0        0      316 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2511 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2091 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0     2218 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      500 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/.readthedocs.yml
+-rw-r--r--   0        0        0     1041 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/CITATION.cff
+-rw-r--r--   0        0        0     5495 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2518 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1067 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     1674 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/README.md
+-rw-r--r--   0        0        0      633 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/docs/Makefile
+-rw-r--r--   0        0        0     1466 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/acknowledgements.md
+-rw-r--r--   0        0        0      683 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/api/dsecs.rst
+-rw-r--r--   0        0        0      244 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/api/fac.rst
+-rw-r--r--   0        0        0      134 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/api/io.rst
+-rw-r--r--   0        0        0      644 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/api/tfa.rst
+-rw-r--r--   0        0        0      176 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/changelog.md
+-rw-r--r--   0        0        0     3091 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/conf.py
+-rw-r--r--   0        0        0      531 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/contributing.md
+-rw-r--r--   0        0        0     6899 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/guides/dsecs/intro_dsecs.ipynb
+-rw-r--r--   0        0        0     4380 2023-04-06 20:09:46.668853 swarmpal-0.1.0a4/docs/guides/fac/intro_fac.ipynb
+-rw-r--r--   0        0        0    10651 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0     8508 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/shared/data_io.ipynb
+-rw-r--r--   0        0        0    11537 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/shared/paldata.ipynb
+-rw-r--r--   0        0        0    16216 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/intro_tfa.ipynb
+-rw-r--r--   0        0        0     7928 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/using_tfa.ipynb
+-rw-r--r--   0        0        0     7620 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_1.ipynb
+-rw-r--r--   0        0        0     5348 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_2.ipynb
+-rw-r--r--   0        0        0     5520 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_3.ipynb
+-rw-r--r--   0        0        0     6535 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_4.ipynb
+-rw-r--r--   0        0        0      693 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/index.md
+-rw-r--r--   0        0        0     1622 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/docs/installation.md
+-rw-r--r--   0        0        0      759 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/docs/make.bat
+-rw-r--r--   0        0        0      678 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/environment.yml
+-rw-r--r--   0        0        0     1353 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/noxfile.py
+-rw-r--r--   0        0        0     2601 2023-04-06 20:13:34.128772 swarmpal-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-04-06 20:11:24.084245 swarmpal-0.1.0a4/src/swarmpal/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/io/__init__.py
+-rw-r--r--   0        0        0    12281 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/io/_data_container.py
+-rw-r--r--   0        0        0     8280 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/io/_datafetchers.py
+-rw-r--r--   0        0        0    17318 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/io/_paldata.py
+-rw-r--r--   0        0        0        0 2023-04-06 20:09:38.876582 swarmpal-0.1.0a4/src/swarmpal/io/py.typed
+-rw-r--r--   0        0        0        0 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/__init__.py
+-rw-r--r--   0        0        0      149 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/__init__.py
+-rw-r--r--   0        0        0    17840 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/aux_tools.py
+-rw-r--r--   0        0        0    79676 2023-04-06 20:09:46.672854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/dsecs_algorithms.py
+-rw-r--r--   0        0        0     5558 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/processes.py
+-rw-r--r--   0        0        0       71 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/fac/__init__.py
+-rw-r--r--   0        0        0     4052 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/fac/fac_algorithms.py
+-rw-r--r--   0        0        0     3789 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/fac/processes.py
+-rw-r--r--   0        0        0      161 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/__init__.py
+-rw-r--r--   0        0        0    10429 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/plotting.py
+-rw-r--r--   0        0        0    18459 2023-04-06 20:11:24.088245 swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/processes.py
+-rw-r--r--   0        0        0    31496 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/tfa_processor.py
+-rw-r--r--   0        0        0    24364 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/tfalib.py
+-rw-r--r--   0        0        0        0 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/utils/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/src/swarmpal/utils/exceptions.py
+-rw-r--r--   0        0        0     1536 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/tests/io/test_datafetchers.py
+-rw-r--r--   0        0        0     5979 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/tests/io/test_paldata.py
+-rw-r--r--   0        0        0     1943 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/tests/io/test_palprocess.py
+-rw-r--r--   0        0        0     2676 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/tests/test_io_deprecated.py
+-rw-r--r--   0        0        0      478 2023-04-06 20:09:46.676854 swarmpal-0.1.0a4/tests/test_package.py
+-rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 swarmpal-0.1.0a4/PKG-INFO
```

### Comparing `swarmpal-0.1.0/.github/workflows/ci.yml` & `swarmpal-0.1.0a4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/.gitignore` & `swarmpal-0.1.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/.pre-commit-config.yaml` & `swarmpal-0.1.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/CITATION.cff` & `swarmpal-0.1.0a4/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     email: ashley.smith@ed.ac.uk
     orcid: 'https://orcid.org/0000-0001-5198-9574'
   - given-names: Sebastian
     family-names: Käki
     orcid: 'https://orcid.org/0000-0001-7212-5791'
   - given-names: Theresa
     family-names: Hoppe
-    orcid: 'https://orcid.org/0009-0000-7108-5468'
   - given-names: Heikki
     family-names: Vanhamäki
     orcid: 'https://orcid.org/0000-0002-3454-0350'
   - given-names: Constantinos
     family-names: Papadimitriou
     orcid: 'https://orcid.org/0000-0002-5191-0149'
   - given-names: Georgios
```

### Comparing `swarmpal-0.1.0/CODE_OF_CONDUCT.md` & `swarmpal-0.1.0a4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/CONTRIBUTING.md` & `swarmpal-0.1.0a4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/LICENSE` & `swarmpal-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/README.md` & `swarmpal-0.1.0a4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # SwarmPAL
 
 ---
-[![Swarm-VRE](https://img.shields.io/badge/%F0%9F%9A%80%20launch-Swarm--VRE-blue)](https://vre.vires.services/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fsmithara%2Fswarmpal-demo&urlpath=lab%2Ftree%2Fswarmpal-demo%2FREADME.ipynb&branch=main)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/smithara/swarmpal-demo/HEAD)
-
-[![PyPI](https://img.shields.io/pypi/v/swarmpal)]( https://pypi.org/project/swarmpal/)
 [![Documentation](https://img.shields.io/badge/docs-online-success)][rtd-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
-
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 ---
 
 [actions-badge]:            https://github.com/Swarm-DISC/SwarmPAL/workflows/CI/badge.svg
@@ -26,11 +21,8 @@
 [github-discussions-link]:  https://github.com/Swarm-DISC/SwarmPAL/discussions
 [pypi-link]:                https://pypi.org/project/swarmpal/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/swarmpal
 [pypi-version]:             https://badge.fury.io/py/swarmpal.svg
 [rtd-badge]:                https://img.shields.io/badge/docs-online-success
 [rtd-link]:                 https://swarmpal.readthedocs.io/
 
-![SwarmPAL diagram](https://swarmpal-benchmarks.netlify.app/swarmpal-diagram.png)
-
-For more information see:
-- <https://swarmdisc.org/lab/>
+See the [SwarmPAL development guide on HackMD](https://hackmd.io/@swarm/dev/%2Ff6YIHfqxT9yL0giWJzhr_Q)
```

### Comparing `swarmpal-0.1.0/docs/Makefile` & `swarmpal-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/acknowledgements.md` & `swarmpal-0.1.0a4/docs/acknowledgements.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Acknowledgements
 
 If you make use of this package in a publication, please cite the following:
 
 ```raw
-[Pending Zenodo link - for now, just reference the GitHub repo]
+[Pending Zenodo link and update of https://github.com/Swarm-DISC/SwarmPAL/blob/main/CITATION.cff]
 ```
 
 ## Funding
 
 This project is funded by ESA through [Swarm DISC (Data, Innovation, and Science Cluster)](https://earth.esa.int/eogateway/activities/swarm-disc) as well as through other [Swarm mission](https://earth.esa.int/eogateway/missions/swarm) funding. In particular, the following Swarm projects have contributed to this work:
 - Time-Frequency Analysis (TFA) toolbox
 - [Dipolar Spherical Elementary Current Systems (DSECS) toolbox](https://earth.esa.int/eogateway/activities/dsecs)
```

### Comparing `swarmpal-0.1.0/docs/api/dsecs.rst` & `swarmpal-0.1.0a4/docs/api/dsecs.rst`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/conf.py` & `swarmpal-0.1.0a4/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -159,55 +159,36 @@
 000009e0: 414c 222c 0a20 2020 2022 7573 655f 7265  AL",.    "use_re
 000009f0: 706f 7369 746f 7279 5f62 7574 746f 6e22  pository_button"
 00000a00: 3a20 5472 7565 2c0a 2020 2020 2275 7365  : True,.    "use
 00000a10: 5f69 7373 7565 735f 6275 7474 6f6e 223a  _issues_button":
 00000a20: 2054 7275 652c 0a20 2020 2022 7573 655f   True,.    "use_
 00000a30: 6564 6974 5f70 6167 655f 6275 7474 6f6e  edit_page_button
 00000a40: 223a 2054 7275 652c 0a20 2020 2022 616e  ": True,.    "an
-00000a50: 6e6f 756e 6365 6d65 6e74 223a 2028 0a20  nouncement": (. 
-00000a60: 2020 2020 2020 2022 5741 524e 494e 4721         "WARNING!
-00000a70: 2054 4849 5320 5041 434b 4147 4520 4953   THIS PACKAGE IS
-00000a80: 2049 4e20 4143 5449 5645 2044 4556 454c   IN ACTIVE DEVEL
-00000a90: 4f50 4d45 4e54 2041 4e44 2049 5320 4e4f  OPMENT AND IS NO
-00000aa0: 5420 5945 5420 5354 4142 4c45 213c 6272  T YET STABLE!<br
-00000ab0: 3e22 0a20 2020 2020 2020 2022 3c62 7574  >".        "<but
-00000ac0: 746f 6e3e 3c61 2068 7265 663d 2768 7474  ton><a href='htt
-00000ad0: 7073 3a2f 2f76 7265 2e76 6972 6573 2e73  ps://vre.vires.s
-00000ae0: 6572 7669 6365 732f 6875 622f 7573 6572  ervices/hub/user
-00000af0: 2d72 6564 6972 6563 742f 6769 742d 7075  -redirect/git-pu
-00000b00: 6c6c 3f72 6570 6f3d 6874 7470 7325 3341  ll?repo=https%3A
-00000b10: 2532 4625 3246 6769 7468 7562 2e63 6f6d  %2F%2Fgithub.com
-00000b20: 2532 4673 6d69 7468 6172 6125 3246 7377  %2Fsmithara%2Fsw
-00000b30: 6172 6d70 616c 2d64 656d 6f26 616d 703b  armpal-demo&amp;
-00000b40: 7572 6c70 6174 683d 6c61 6225 3246 7472  urlpath=lab%2Ftr
-00000b50: 6565 2532 4673 7761 726d 7061 6c2d 6465  ee%2Fswarmpal-de
-00000b60: 6d6f 2532 4652 4541 444d 452e 6970 796e  mo%2FREADME.ipyn
-00000b70: 6226 616d 703b 6272 616e 6368 3d6d 6169  b&amp;branch=mai
-00000b80: 6e27 3e43 6c69 636b 2068 6572 6520 746f  n'>Click here to
-00000b90: 2074 7279 2053 7761 726d 5041 4c20 696e   try SwarmPAL in
-00000ba0: 2074 6865 2056 6972 7475 616c 2052 6573   the Virtual Res
-00000bb0: 6561 7263 6820 456e 7669 726f 6e6d 656e  earch Environmen
-00000bc0: 743c 2f61 3e3c 2f62 7574 746f 6e3e 220a  t</a></button>".
-00000bd0: 2020 2020 292c 0a7d 0a0a 2320 4164 6420      ),.}..# Add 
-00000be0: 616e 7920 7061 7468 7320 7468 6174 2063  any paths that c
-00000bf0: 6f6e 7461 696e 2063 7573 746f 6d20 7374  ontain custom st
-00000c00: 6174 6963 2066 696c 6573 2028 7375 6368  atic files (such
-00000c10: 2061 7320 7374 796c 6520 7368 6565 7473   as style sheets
-00000c20: 2920 6865 7265 2c0a 2320 7265 6c61 7469  ) here,.# relati
-00000c30: 7665 2074 6f20 7468 6973 2064 6972 6563  ve to this direc
-00000c40: 746f 7279 2e20 5468 6579 2061 7265 2063  tory. They are c
-00000c50: 6f70 6965 6420 6166 7465 7220 7468 6520  opied after the 
-00000c60: 6275 696c 7469 6e20 7374 6174 6963 2066  builtin static f
-00000c70: 696c 6573 2c0a 2320 736f 2061 2066 696c  iles,.# so a fil
-00000c80: 6520 6e61 6d65 6420 2264 6566 6175 6c74  e named "default
-00000c90: 2e63 7373 2220 7769 6c6c 206f 7665 7277  .css" will overw
-00000ca0: 7269 7465 2074 6865 2062 7569 6c74 696e  rite the builtin
-00000cb0: 2022 6465 6661 756c 742e 6373 7322 2e0a   "default.css"..
-00000cc0: 6874 6d6c 5f73 7461 7469 635f 7061 7468  html_static_path
-00000cd0: 3a20 6c69 7374 5b73 7472 5d20 3d20 5b5d  : list[str] = []
-00000ce0: 0a0a 2320 4669 7820 6874 7470 733a 2f2f  ..# Fix https://
-00000cf0: 6769 7468 7562 2e63 6f6d 2f65 7865 6375  github.com/execu
-00000d00: 7461 626c 6562 6f6f 6b73 2f73 7068 696e  tablebooks/sphin
-00000d10: 782d 626f 6f6b 2d74 6865 6d65 2f69 7373  x-book-theme/iss
-00000d20: 7565 732f 3130 350a 6874 6d6c 5f73 6f75  ues/105.html_sou
-00000d30: 7263 656c 696e 6b5f 7375 6666 6978 203d  rcelink_suffix =
-00000d40: 2022 220a                                 "".
+00000a50: 6e6f 756e 6365 6d65 6e74 223a 2022 5741  nouncement": "WA
+00000a60: 524e 494e 4721 2054 4849 5320 5041 434b  RNING! THIS PACK
+00000a70: 4147 4520 4953 2049 4e20 4143 5449 5645  AGE IS IN ACTIVE
+00000a80: 2044 4556 454c 4f50 4d45 4e54 2041 4e44   DEVELOPMENT AND
+00000a90: 2049 5320 4e4f 5420 5945 5420 5354 4142   IS NOT YET STAB
+00000aa0: 4c45 2122 2c0a 7d0a 0a23 2041 6464 2061  LE!",.}..# Add a
+00000ab0: 6e79 2070 6174 6873 2074 6861 7420 636f  ny paths that co
+00000ac0: 6e74 6169 6e20 6375 7374 6f6d 2073 7461  ntain custom sta
+00000ad0: 7469 6320 6669 6c65 7320 2873 7563 6820  tic files (such 
+00000ae0: 6173 2073 7479 6c65 2073 6865 6574 7329  as style sheets)
+00000af0: 2068 6572 652c 0a23 2072 656c 6174 6976   here,.# relativ
+00000b00: 6520 746f 2074 6869 7320 6469 7265 6374  e to this direct
+00000b10: 6f72 792e 2054 6865 7920 6172 6520 636f  ory. They are co
+00000b20: 7069 6564 2061 6674 6572 2074 6865 2062  pied after the b
+00000b30: 7569 6c74 696e 2073 7461 7469 6320 6669  uiltin static fi
+00000b40: 6c65 732c 0a23 2073 6f20 6120 6669 6c65  les,.# so a file
+00000b50: 206e 616d 6564 2022 6465 6661 756c 742e   named "default.
+00000b60: 6373 7322 2077 696c 6c20 6f76 6572 7772  css" will overwr
+00000b70: 6974 6520 7468 6520 6275 696c 7469 6e20  ite the builtin 
+00000b80: 2264 6566 6175 6c74 2e63 7373 222e 0a68  "default.css"..h
+00000b90: 746d 6c5f 7374 6174 6963 5f70 6174 683a  tml_static_path:
+00000ba0: 206c 6973 745b 7374 725d 203d 205b 5d0a   list[str] = [].
+00000bb0: 0a23 2046 6978 2068 7474 7073 3a2f 2f67  .# Fix https://g
+00000bc0: 6974 6875 622e 636f 6d2f 6578 6563 7574  ithub.com/execut
+00000bd0: 6162 6c65 626f 6f6b 732f 7370 6869 6e78  ablebooks/sphinx
+00000be0: 2d62 6f6f 6b2d 7468 656d 652f 6973 7375  -book-theme/issu
+00000bf0: 6573 2f31 3035 0a68 746d 6c5f 736f 7572  es/105.html_sour
+00000c00: 6365 6c69 6e6b 5f73 7566 6669 7820 3d20  celink_suffix = 
+00000c10: 2222 0a                                  "".
```

### Comparing `swarmpal-0.1.0/docs/contributing.md` & `swarmpal-0.1.0a4/docs/contributing.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ## Ideas and more!
 
 1. Read the code of conduct below
 1. Join the mailing list at <https://groups.io/g/swarm-dev>
 1. Join a meeting at <https://hackmd.io/@swarm/meetings>
 1. Found something to improve? [Open an Issue on GitHub](https://github.com/Swarm-DISC/SwarmPAL/issues) or get in touch otherwise
-1. Have other ideas / requests for help? [Start a Discussion on GitHub](https://github.com/Swarm-DISC/SwarmPAL/discussions)
 
 ## Development
 
 1. Read the development guide at [https://hackmd.io/@swarm/dev](https://hackmd.io/@swarm/dev/%2FVFOe2P1ETYmup0K0YSxKEQ?view)
 1. Open an Issue/PR ☺️
 
 ---
```

### Comparing `swarmpal-0.1.0/docs/guides/dsecs/intro_dsecs.ipynb` & `swarmpal-0.1.0a4/docs/guides/dsecs/intro_dsecs.ipynb`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/guides/fac/intro_fac.ipynb` & `swarmpal-0.1.0a4/docs/guides/fac/intro_fac.ipynb`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/guides/quickstart.ipynb` & `swarmpal-0.1.0a4/docs/guides/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/guides/shared/paldata.ipynb` & `swarmpal-0.1.0a4/docs/guides/shared/paldata.ipynb`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/docs/guides/tfa/tfa_AUX_OBS.ipynb` & `swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_3.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7418504901960784%*

 * *Differences: {"'cells'": "{0: {'source': ['# Analysis of Swarm Electric Field data'], delete: ['id']}, 1: "*

 * *            "{'source': ['   Imports:'], delete: ['id']}, 2: {'source': {insert: [(1, 'import "*

 * *            "swarmpal.toolboxes.tfa.tfa_processor as tfa')], delete: [3, 2, 1]}, delete: ['id']}, "*

 * *            "7: {'source': ['Note: This is a dataset that is not yet supported officially by "*

 * *            'SwarmPAL. The TFA bypasses that, by calling the ViresClient directly, behind the '*

 * *            'scenes, in order  […]*

```diff
@@ -1,161 +1,187 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "783bd806-a4e6-434f-9494-cdd98cce9b47",
             "metadata": {},
             "source": [
-                "# Analysis of Ground Observatory data"
+                "# Analysis of Swarm Electric Field data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2c621f95-3850-4250-afb7-c54b0f4dfe63",
             "metadata": {},
             "source": [
-                "VirES also has ground observatory data from INTERMAGNET (via the \"AUX_OBS\" collections). We can apply the same TFA tools to this data.\n",
-                "\n",
-                "For more details, see the [viresclient documentation](https://viresclient.readthedocs.io/en/latest/available_parameters.html) and the [AUX_OBS demo notebook](https://notebooks.vires.services/notebooks/04c2_geomag-ground-data-vires)"
+                "   Imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9adecf37-9d3d-4219-84cb-5b7110ec9fcc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import datetime as dt\n",
-                "\n",
-                "from swarmpal.io import create_paldata, PalDataItem\n",
-                "from swarmpal.toolboxes import tfa"
+                "import swarmpal.toolboxes.tfa.tfa_processor as tfa"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c4492e83-0c1c-47a4-b92d-13c174d057e5",
             "metadata": {},
             "source": [
-                "## Fetching data"
+                "Provide values for the parameters of the analysis.  The `dataset` can be chosen from one of the compatible magnetic data collections, and the `var` is a VirES-compatible variable string (see [viresclient](https://viresclient.readthedocs.io/en/latest/available_parameters.html) for more information). The \"start\" and \"end\" times must be given as a datetime object. If the data are required as they are, set the `remove_chaos_model` parameter to False. Otherwise, if the inputs are magnetic field data and the analysis requires subtraction of the model field, set the parameter to True. \n",
+                "For the electric field, the `SW_EXPT_EFIA_TCT02` has to be used, which includes electric field measurements from the VxB product, in two directions, \"horizonta\" or \"vertical\", both in the instrument XYZ cartesian coordinate frame. Each of these can be selected with the `Eh_XYV` or `Ev_XYZ` variables."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dataset = \"SW_EXPT_EFIA_TCT02\"\n",
+                "series_dt = \"PT1S\"\n",
+                "var = \"Eh_XYZ\"\n",
+                "remove_chaos_model = False\n",
+                "time_start = dt.datetime(2015, 3, 14, 12, 5, 0)\n",
+                "time_end = dt.datetime(2015, 3, 14, 12, 30, 0)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e975d53f-3576-4249-baed-c76d23040351",
             "metadata": {},
             "source": [
-                "Here we access the 1-minute data (the \"M\" in `OBSM2_`) from Hornsund (`HRN`). The three-letter code is an INTERMAGNET observatory code (see <https://intermagnet.github.io/metadata/#/imos>).\n",
-                "\n",
-                "Since this is only 1-minute time resolution, only the very low frequency bands can be found (i.e. Pc5)."
+                "Now run the TfaInput to retrieve the selected data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1cf70e30-1fcb-4fd8-930b-c5ee16fa80d8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_params = dict(\n",
-                "    collection=\"SW_OPER_AUX_OBSM2_:HRN\",\n",
-                "    measurements=[\"B_NEC\"],\n",
-                "    models=[\"Model='CHAOS-Core'+'CHAOS-Static'\"],\n",
-                "    auxiliaries=[\"MLT\"],\n",
-                "    start_time=dt.datetime(2015, 3, 14, 0, 0, 0),\n",
-                "    end_time=dt.datetime(2015, 3, 14, 23, 59, 59),\n",
-                "    pad_times=(dt.timedelta(hours=3), dt.timedelta(hours=3)),\n",
-                "    server_url=\"https://vires.services/ows\",\n",
-                "    options=dict(asynchronous=False, show_progress=False),\n",
-                ")\n",
-                "data = create_paldata(PalDataItem.from_vires(**data_params))"
+                "inputs = tfa.TfaInput(\n",
+                "    collection=dataset,\n",
+                "    start_time=time_start,\n",
+                "    end_time=time_end,\n",
+                "    initialise=True,\n",
+                "    varname=var,\n",
+                "    sampling_time=series_dt,\n",
+                "    remove_chaos=remove_chaos_model,\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Note: This is a dataset that is not yet supported officially by SwarmPAL. The TFA bypasses that, by calling the ViresClient directly, behind the scenes, in order to get the data and then formats them so that they become of similar type with the other commonly used products. This will be updated soon, to be correctly supported through the normal channels."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "56aa6b9d-8ece-4aa4-8738-a62ffe9eb478",
             "metadata": {},
             "source": [
-                "## Processing"
+                "Now that the input instance is ready, we can proceed to for Wavelet processing by initiating the `TfaProcessor` object and specifying the name of the variable and the component of choice, 0 for X, 1 for Y and 2 for the Z one."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "70394c05-7dcb-4bc7-933c-7256a7a7b10a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p1 = tfa.processes.Preprocess()\n",
-                "p1.set_config(\n",
-                "    dataset=\"SW_OPER_AUX_OBSM2_:HRN\",\n",
-                "    active_variable=\"B_NEC_res_Model\",\n",
-                "    active_component=0,\n",
-                "    sampling_rate=1 / 60,\n",
-                "    remove_model=True,\n",
-                ")\n",
-                "p2 = tfa.processes.Clean()\n",
-                "p2.set_config(\n",
-                "    window_size=10,\n",
-                "    method=\"iqr\",\n",
-                "    multiplier=1,\n",
-                ")\n",
-                "p3 = tfa.processes.Filter()\n",
-                "p3.set_config(\n",
-                "    cutoff_frequency=0.001,\n",
-                ")\n",
-                "p4 = tfa.processes.Wavelet()\n",
-                "p4.set_config(\n",
-                "    min_scale=1000 / 8,\n",
-                "    max_scale=1000 / 1,\n",
-                "    dj=0.1,\n",
-                ")\n",
-                "\n",
-                "p1(data)\n",
-                "p2(data)\n",
-                "p3(data)\n",
-                "p4(data);"
+                "processor = tfa.TfaProcessor(\n",
+                "    inputs, active_variable={\"varname\": \"Eh_XYZ\", \"component\": 0}\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "528eef47-568e-4ab5-88fd-88d798b0bd38",
             "metadata": {},
             "source": [
-                "## Plotting"
+                "To perform cleaning on the data, we initialize a `Cleaning` object with the parameters of our choice and then apply it on the data with the `TfaProcessor` `apply()` function.\n",
+                "The active variable series can be plotted by means of the `plotX()` function."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "c = tfa.Cleaning({\"Window_Size\": 300, \"Method\": \"iqr\", \"Multiplier\": 1})\n",
+                "processor.apply(c)\n",
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "14e758c8-0280-4b9c-8154-94f8e3dc7a16",
             "metadata": {},
             "source": [
-                "Note that since the ground station data are provided in a 1-minute sampling time, the frequency range to be studied must be very low, i.e. Pc5 (2 - 7 mHz). Frequencies higher than 8 mHz cannot really be captured with these data, since the Nyquist frequency for a sampling time dt of 60 seconds is 1/(2*60) = 8.33 mHz!"
+                "Similarly, the filtering can be performed by first initializing a `Filtering` object with the parameters of our choosing and the applying in on the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b90715b6-eac3-4712-b61d-71b8cbe834b6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tfa.plotting.quicklook(data, extra_x=(\"MLT\",));"
+                "f = tfa.Filtering({\"Cutoff_Frequency\": 10 / 1000})\n",
+                "processor.apply(f)\n",
+                "processor.plotX()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In the same way, the wavelet transform is applied. The result of the wavelet can be visualized by means of the image() function"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "w = tfa.Wavelet(\n",
+                "    {\n",
+                "        \"Min_Frequency\": 20 / 1000,\n",
+                "        \"Max_Frequency\": 200 / 1000,\n",
+                "        \"dj\": 0.1,\n",
+                "    }\n",
+                ")\n",
+                "processor.apply(w)\n",
+                "processor.image(cbar_lims=[-2, 2])"
             ]
         }
     ],
     "metadata": {
+        "interpreter": {
+            "hash": "87d67a24c2c5892c025cb327df6d3922c0a9d4e9219e4fcf3b6836bad3fb9136"
+        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `swarmpal-0.1.0/docs/guides/tfa/tfa_Cluster.ipynb` & `swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_2.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7344907407407407%*

 * *Differences: {"'cells'": "{0: {'source': ['# Analysis of Swarm HR data (50 Hz sampling rate)'], delete: "*

 * *            "['id']}, 1: {'source': ['   Imports:'], delete: ['id']}, 2: {'source': {insert: [(1, "*

 * *            "'import swarmpal.toolboxes.tfa.tfa_processor as tfa')], delete: [3, 2, 1]}, delete: "*

 * *            "['id']}, 9: {'source': ['Now that the model field has been removed and the "*

 * *            'transformation has been performed, we can proceed to for Wavelet processing by '*

 * *            "initiating the `TfaProc […]*

```diff
@@ -1,155 +1,196 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "d5b95cd8-6f5e-4332-b70a-6716d13b7c9f",
             "metadata": {},
             "source": [
-                "# Analysis of Cluster data"
+                "# Analysis of Swarm HR data (50 Hz sampling rate)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f041987c-0abc-4ce0-94b2-5986254bd3ad",
             "metadata": {},
             "source": [
-                "In this example we will access Cluster data via a HAPI server (not from VirES)\n",
-                "\n",
-                "For more information about HAPI, see <http://hapi-server.org/>"
+                "   Imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "350edcfb-60c8-4bff-9685-5846774ea760",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import datetime as dt\n",
-                "\n",
-                "from swarmpal.io import create_paldata, PalDataItem\n",
-                "from swarmpal.toolboxes import tfa"
+                "import swarmpal.toolboxes.tfa.tfa_processor as tfa"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "200bc103-f5bb-4d1e-8cdc-0a6b598dae14",
             "metadata": {},
             "source": [
-                "## Fetching data"
+                "Provide values for the parameters of the analysis.  The `dataset` can be chosen from one of the compatible magnetic data collections, and the `var` is a VirES-compatible variable string (see [viresclient](https://viresclient.readthedocs.io/en/latest/available_parameters.html) for more information). The \"start\" and \"end\" times must be given as a datetime object. If the data are required as they are, set the `remove_chaos_model` parameter to False. Otherwise, if the inputs are magnetic field data and the analysis requires subtraction of the model field, set the parameter to True. \n",
+                "For the HR product, remember to set the sampling_time to 0.02 seconds, i.e. 50 Hz rate."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dataset = \"SW_OPER_MAGB_HR_1B\"\n",
+                "series_dt = \"PT0.02S\"\n",
+                "var = \"B_NEC\"\n",
+                "remove_chaos_model = True\n",
+                "time_start = dt.datetime(2015, 3, 14, 12, 5, 0)\n",
+                "time_end = dt.datetime(2015, 3, 14, 12, 30, 0)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "01b00f2d-092c-45c9-8183-25fff1de2993",
             "metadata": {},
             "source": [
-                "We can access HAPI data in an almost identical way as from VirES, instead using `PalDataItem.from_hapi`.\n",
-                "\n",
-                "Here we will use the AMDA service to get the data. This might change in the future.\n",
-                "\n",
-                "Available HAPI data can be browsed at <http://hapi-server.org/servers>, to quickly look at the data or to generate code snippets using the Python `hapiclient` package - the inputs to hapiclient can be used in `PalDataItem.from_hapi` (hapiclient is used underneath within SwarmPAL). For example:\n",
-                "- <http://hapi-server.org/servers/#server=AMDA&dataset=clust3-fgm-prp&parameters=c3_b_gse&start=2015-03-29T17:00:00&stop=2015-03-29T19:00:00&return=script&format=python>\n",
-                "- <http://hapi-server.org/servers/#server=CDAWeb&dataset=C3_CP_FGM_SPIN&parameters=B_vec_xyz_gse__C3_CP_FGM_SPIN&start=2015-03-29T17:00:00&stop=2015-03-29T19:00:00&return=script&format=python>"
+                "Now run the TfaInput to retrieve the selected data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0384448e-da8c-4b41-8ed1-dd43b611c2b9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_params = dict(\n",
-                "    server=\"http://amda.irap.omp.eu/service/hapi\",\n",
-                "    dataset=\"clust3-fgm-prp\",\n",
-                "    parameters=\"c3_b_gse\",\n",
-                "    start=\"2015-03-29T17:00:00\",\n",
-                "    stop=\"2015-03-29T19:00:00\",\n",
-                "    pad_times=(dt.timedelta(hours=3), dt.timedelta(hours=3)),\n",
-                ")\n",
-                "data = create_paldata(PalDataItem.from_hapi(**data_params))\n",
-                "print(data)"
+                "inputs = tfa.TfaInput(\n",
+                "    collection=dataset,\n",
+                "    start_time=time_start,\n",
+                "    end_time=time_end,\n",
+                "    initialise=True,\n",
+                "    varname=var,\n",
+                "    sampling_time=series_dt,\n",
+                "    remove_chaos=remove_chaos_model,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "28fbf535-d448-46cd-bde3-e4e4467cef1d",
             "metadata": {},
             "source": [
-                "## Processing"
+                "We can now use the full arsenal of functions to perform pre-processing of the data. If the selected variable is in vector form, we can convert it to its magnitude using the `calculate_magnitude()` function. This will generate a new variable named simply `B `. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0174f15b-742f-4510-9630-b602a67131cf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p1 = tfa.processes.Preprocess()\n",
-                "p1.set_config(\n",
-                "    dataset=\"clust3-fgm-prp\",\n",
-                "    timevar=\"Time\",\n",
-                "    active_variable=\"c3_b_gse\",\n",
-                "    active_component=2,\n",
-                "    sampling_rate=1 / 4,\n",
-                ")\n",
-                "p2 = tfa.processes.Clean()\n",
-                "p2.set_config(\n",
-                "    window_size=300,\n",
-                "    method=\"iqr\",\n",
-                "    multiplier=1,\n",
-                ")\n",
-                "p3 = tfa.processes.Filter()\n",
-                "p3.set_config(\n",
-                "    cutoff_frequency=0.1,\n",
-                ")\n",
-                "p4 = tfa.processes.Wavelet()\n",
-                "p4.set_config(\n",
-                "    min_frequency=1,\n",
-                "    max_frequency=25,\n",
-                "    dj=0.1,\n",
-                ")\n",
-                "\n",
-                "p1(data)\n",
-                "p2(data)\n",
-                "p3(data)\n",
-                "p4(data);"
+                "inputs.flag_cleaning()\n",
+                "inputs.subtract_chaos()\n",
+                "inputs.calculate_magnitude()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "871ad53a-f00b-466f-aa84-ee3ed320f11a",
             "metadata": {},
             "source": [
-                "## Plotting"
+                "Now that the model field has been removed and the transformation has been performed, we can proceed to for Wavelet processing by initiating the `TfaProcessor` object and specifying the name of the variable."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "70598c47-4a29-4c39-b0aa-e6ce34188956",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tfa.plotting.quicklook(data, extra_x=None);"
+                "processor = tfa.TfaProcessor(inputs, active_variable={\"varname\": \"B\"})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "processor.plotX()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To perform cleaning on the data, we initialize a `Cleaning` object with the parameters of our choice and then apply it on the data with the `TfaProcessor` `apply()` function.\n",
+                "The active variable series can be plotted by means of the `plotX()` function."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "c = tfa.Cleaning({\"Window_Size\": 300, \"Method\": \"iqr\", \"Multiplier\": 1})\n",
+                "processor.apply(c)\n",
+                "processor.plotX()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Similarly, the filtering can be performed by first initializing a `Filtering` object with the parameters of our choosing and the applying in on the data."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "f = tfa.Filtering({\"Cutoff_Frequency\": 0.1})\n",
+                "processor.apply(f)\n",
+                "processor.plotX()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In the same way, the wavelet transform is applied. The result of the wavelet can be visualized by means of the image() function"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "w = tfa.Wavelet(\n",
+                "    {\n",
+                "        \"Min_Frequency\": 1,\n",
+                "        \"Max_Frequency\": 25,\n",
+                "        \"dj\": 0.1,\n",
+                "    }\n",
+                ")\n",
+                "processor.apply(w)\n",
+                "processor.image(cbar_lims=[-6, -3])"
             ]
         }
     ],
     "metadata": {
+        "interpreter": {
+            "hash": "87d67a24c2c5892c025cb327df6d3922c0a9d4e9219e4fcf3b6836bad3fb9136"
+        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `swarmpal-0.1.0/docs/guides/tfa/tfa_MAGx_LR.ipynb` & `swarmpal-0.1.0a4/docs/guides/tfa/using_tfa_1.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7464776976495726%*

 * *Differences: {"'cells'": "{1: {'source': ['   Imports:'], delete: ['id']}, 2: {'source': {insert: [(1, 'import "*

 * *            "swarmpal.toolboxes.tfa.tfa_processor as tfa')], delete: [4, 3, 2, 1]}, delete: "*

 * *            "['id']}, 3: {'source': ['Provide values for the parameters of the analysis.  The "*

 * *            '`dataset` can be chosen from one of the compatible magnetic data collections, and the '*

 * *            '`var` is a VirES-compatible variable string (see '*

 * *            '[viresclient](https://viresclient.readthedoc […]*

```diff
@@ -1,235 +1,280 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "68c253c7-1b1c-48d3-82eb-cedf959c7a6d",
             "metadata": {},
             "source": [
-                "# Analysis of Swarm MAG LR data (1Hz)\n",
-                "\n",
-                "For more information about the data and other ways to access it, see:\n",
-                "\n",
-                "- [Data handbook](https://swarmhandbook.earth.esa.int/catalogue/SW_MAGx_LR_1B)\n",
-                "- [viresclient documentation](https://viresclient.readthedocs.io/en/latest/available_parameters.html)\n",
-                "- [MAGx_LR demo notebook](https://notebooks.vires.services/notebooks/03a1_demo-magx_lr_1b)"
+                "# Using the TFA toolbox"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "   Imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "92f4673e-491d-4c59-b376-e86a254d2fd9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import datetime as dt\n",
-                "import matplotlib.pyplot as plt\n",
-                "\n",
-                "from swarmpal.io import create_paldata, PalDataItem\n",
-                "from swarmpal.toolboxes import tfa"
+                "import swarmpal.toolboxes.tfa.tfa_processor as tfa"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a90ecd00-48ed-4dbd-9b23-931ba654fc27",
             "metadata": {},
             "source": [
-                "## Fetching data"
+                "Provide values for the parameters of the analysis.  The `dataset` can be chosen from one of the compatible magnetic data collections, and the `var` is a VirES-compatible variable string (see [viresclient](https://viresclient.readthedocs.io/en/latest/available_parameters.html) for more information). The \"start\" and \"end\" times must be given as a datetime object. If the data are required as they are, set the `remove_chaos_model` parameter to False. Otherwise, if the inputs are magnetic field data and the analysis requires subtraction of the model field, set the parameter to True. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dataset = \"SW_OPER_MAGA_LR_1B\"\n",
+                "var = \"B_NEC\"\n",
+                "remove_chaos_model = True\n",
+                "time_start = dt.datetime(2015, 3, 14)\n",
+                "time_end = dt.datetime(2015, 3, 14, 3, 59, 59)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f8b55f7c-06e3-43be-86b2-c61d5c4ea6e6",
             "metadata": {},
             "source": [
-                "As in the introduction example, we will fetch the MAG LR data."
+                "Now run the TfaInput to retrieve the selected data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "44ea9d02-db7f-4a54-b22c-16fd708ef70a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = create_paldata(\n",
-                "    PalDataItem.from_vires(\n",
-                "        collection=\"SW_OPER_MAGA_LR_1B\",\n",
-                "        measurements=[\"B_NEC\"],\n",
-                "        models=[\"Model=CHAOS\"],\n",
-                "        auxiliaries=[\"QDLat\", \"MLT\"],\n",
-                "        start_time=dt.datetime(2015, 3, 14),\n",
-                "        end_time=dt.datetime(2015, 3, 14, 3, 59, 59),\n",
-                "        pad_times=(dt.timedelta(hours=3), dt.timedelta(hours=3)),\n",
-                "        server_url=\"https://vires.services/ows\",\n",
-                "        options=dict(asynchronous=False, show_progress=False),\n",
-                "    )\n",
-                ")\n",
-                "print(data)"
+                "inputs = tfa.TfaInput(\n",
+                "    collection=dataset,\n",
+                "    start_time=time_start,\n",
+                "    end_time=time_end,\n",
+                "    initialise=True,\n",
+                "    varname=var,\n",
+                "    sampling_time=\"PT1S\",\n",
+                "    remove_chaos=remove_chaos_model,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bece3525-5191-4c2f-afa4-78cb9bcac85d",
             "metadata": {},
             "source": [
-                "## Processing"
+                "We can now use the full arsenal of functions to perform pre-processing of the data."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "inputs.flag_cleaning()\n",
+                "inputs.subtract_chaos()\n",
+                "inputs.convert_to_mfa()\n",
+                "# inputs.calculate_magnitude()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6295e255-87e9-4914-98e0-3b9067ea1db9",
             "metadata": {},
             "source": [
-                "This time we will use the `convert_to_mfa` option to rotate the B_NEC vector to the mean-field aligned (MFA) frame. When the MFA frame is used, the `active_component` must be set to one of (0, 1, 2): 0 is the poloidal component, 1 the toroidal and 2 the compressional. Similarly for B_NEC, the numbers correspond to the North (0), East (1) or Center (2) components."
+                "Now that the model field has been removed and the transformation to Mean Field Aligned coordinate system has been performed, we can select one of the components for Wavelet processing, e.g. the compressional, by initiating the `TfaProcessor` object and specifying the name of the variable and the component number (0, 1, or 2). For MFA, 0 is the poloidal component, 1 the toroidal and 2 the compressional. Similarly for B_NEC, the numbers correspond to the North (0), East (1) or Center (2) components."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e74fe86b-ab51-4160-860a-fff44fd17f6e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p1 = tfa.processes.Preprocess()\n",
-                "p1.set_config(\n",
-                "    dataset=\"SW_OPER_MAGA_LR_1B\",\n",
-                "    active_variable=\"B_MFA\",\n",
-                "    active_component=2,\n",
-                "    sampling_rate=1,\n",
-                "    remove_model=True,\n",
-                "    convert_to_mfa=True,\n",
-                ")\n",
-                "p1(data);"
+                "processor = tfa.TfaProcessor(\n",
+                "    inputs, active_variable={\"varname\": \"B_MFA\", \"component\": 2}\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "89c48259-d5b4-425e-8614-939da0622dfb",
             "metadata": {},
             "source": [
-                "Even though `B_MFA` isn't available in the original data, this variable becomes available when we select `convert_to_mfa=True`. For more information on the other options, refer to the documentation:"
+                "To perform cleaning on the data, we initialize a `Cleaning` object with the parameters of our choice and then apply it on the data with the `TfaProcessor` `apply()` function.\n",
+                "The active variable series can be plotted by means of the `plotX()` function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8d65aa75-d058-419c-94bf-0b017b72b219",
             "metadata": {},
             "outputs": [],
             "source": [
-                "help(tfa.processes.Preprocess.set_config)"
+                "c = tfa.Cleaning({\"Window_Size\": 300, \"Method\": \"iqr\", \"Multiplier\": 1})\n",
+                "processor.apply(c)\n",
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f0e2d565-ab59-4618-a88e-64938a65e6b0",
             "metadata": {},
             "source": [
-                "We can inspect the data directly to get an idea about what has happened using `Preprocess`.\n",
-                "\n",
-                "In the figure below, the input `B_NEC` (first row) and `B_NEC_Model` have been taken to produce `B_NEC_res_Model` (second row), and then that has been rotated to the MFA frame (third row). Component \"2\" is identified from B_MFA and used as the TFA variable (`active_component=2` in the above config)."
+                "Similarly, the filtering can be performed by first initializing a `Filtering` object with the parameters of our choosing and then applying in on the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c383e483-2ff0-438a-b485-4403b6f12639",
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig, axes = plt.subplots(3, 1, sharex=True)\n",
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"B_NEC\"].plot.line(x=\"Timestamp\", ax=axes[0])\n",
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"B_NEC_res_Model\"].plot.line(x=\"Timestamp\", ax=axes[1])\n",
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"B_MFA\"].plot.line(x=\"Timestamp\", ax=axes[2])\n",
-                "axes[1].set_ylim(-200, 200)\n",
-                "axes[2].set_ylim(-200, 200);"
+                "f = tfa.Filtering({\"Cutoff_Frequency\": 20 / 1000})\n",
+                "processor.apply(f)\n",
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0944c3d2-d8f5-4cc5-9c35-e9cc1abe5185",
             "metadata": {},
             "source": [
-                "Let's prepare the other processes..."
+                "In the same way, the wavelet transform is applied. The result of the wavelet can be visualized by means of the image() function"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5c1e2a51-a17d-48e6-a988-519b9d9a70d4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p2 = tfa.processes.Clean()\n",
-                "p2.set_config(\n",
-                "    window_size=300,\n",
-                "    method=\"iqr\",\n",
-                "    multiplier=1,\n",
-                ")\n",
-                "p3 = tfa.processes.Filter()\n",
-                "p3.set_config(\n",
-                "    cutoff_frequency=20 / 1000,\n",
+                "w = tfa.Wavelet(\n",
+                "    {\n",
+                "        \"Min_Frequency\": 20 / 1000,\n",
+                "        \"Max_Frequency\": 100 / 1000,\n",
+                "        \"dj\": 0.1,\n",
+                "    }\n",
                 ")\n",
-                "p4 = tfa.processes.Wavelet()\n",
-                "p4.set_config(\n",
-                "    min_frequency=20 / 1000,\n",
-                "    max_frequency=100 / 1000,\n",
-                "    dj=0.1,\n",
-                ")"
+                "processor.apply(w)\n",
+                "processor.image()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "This is not very useful for large time intervals e.g. an entire day, so the signal can be cut-down into segments, based on the magnetic latitude of the satellite. By default the segments correspond to tracks (half-orbits) from -75 to +75 degrees in Mag. Lat."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "processor.create_segment_index()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "949003be-c283-4cfe-9701-3b0f1e04b551",
             "metadata": {},
             "source": [
-                "In practice, you might want to prepare and apply each process in turn to make sure things work right. Here however, we will just apply them all together. Make sure you apply them in the right order!"
+                "All the plotting functions can now be used to visualize a specific segment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c518412-513f-4fab-a065-b77347a65609",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p2(data)\n",
-                "p3(data)\n",
-                "p4(data);"
+                "processor.image(segment=4)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "768468ae-2beb-4fe1-aec2-25b3190372f7",
             "metadata": {},
             "source": [
-                "## Plotting"
+                "Additional positional information (Magnetic Latitude and MLT) can also be plotted (again either for the entire series or for a specific segment)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0fde2ec2-4366-43de-b8ad-7514754434b5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tfa.plotting.quicklook(data);"
+                "processor.plotAUX(segment=4)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "A simple for loop can be written to produce plots for all segments and save them locally."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# import matplotlib as mpl\n",
+                "# import matplotlib.pyplot as plt\n",
+                "\n",
+                "# mpl.rcParams[\n",
+                "#     \"figure.max_open_warning\"\n",
+                "# ] = 100  # stops the warning when many plots are being produced\n",
+                "\n",
+                "# for i in range(int(processor.Max_Segment) + 1):\n",
+                "#     fig, ax = plt.subplots(3, 1, gridspec_kw={\"height_ratios\": [1, 1.5, 1]})\n",
+                "#     plt.subplot(3, 1, 1)\n",
+                "#     processor.plotX(segment=i)\n",
+                "#     plt.subplot(3, 1, 2)\n",
+                "#     processor.image(segment=i, cbar_lims=[-3, 3])\n",
+                "#     plt.subplot(3, 1, 3)\n",
+                "#     processor.plotAUX(segment=i)\n",
+                "\n",
+                "#     plt.savefig(\"segment_%02d.png\" % i)\n",
+                "#     plt.close(fig)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "75048f8b19dc2376e8ce021c430fd300fc261773814cb02da2fef53030a6379a"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `swarmpal-0.1.0/docs/guides/tfa/tfa_background.ipynb` & `swarmpal-0.1.0a4/docs/guides/tfa/using_tfa.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7471022391047062%*

 * *Differences: {"'cells'": "{0: {'source': ['# Intro to the TFA tool and the Wavelet Transform'], delete: "*

 * *            "['id']}, 1: {'source': ['   Imports:'], delete: ['id']}, 2: {'source': {insert: [(1, "*

 * *            "'\\n'), (5, 'import swarmpal.toolboxes.tfa.tfa_processor as tfa')], delete: [5, 4]}, "*

 * *            "delete: ['id']}, 5: {'source': ['Now run the TfaInput to retrieve the selected "*

 * *            "data.'], delete: ['id']}, 6: {'source': {insert: [(0, 'inputs = tfa.TfaInput(\\n'), "*

 * *            "(1, '    coll […]*

```diff
@@ -1,251 +1,307 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "87f0aae4-34e4-475e-be72-2b6bb63877f2",
             "metadata": {},
             "source": [
-                "# TFA and the Wavelet Transform"
+                "# Intro to the TFA tool and the Wavelet Transform"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "02a9b938-2d3a-4d75-ae7c-5834512048e3",
             "metadata": {},
             "source": [
-                "Here we delve a little into the background of the TFA toolbox.\n",
-                "\n",
-                "First we will fetch some data to setup the framework of a typical TFA application, but then we will replace the data with dummy data to demonstrate what the TFA toolbox does."
+                "   Imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0a174a3b-babf-4386-ad46-7bcc361a4e81",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import datetime as dt\n",
+                "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
-                "from swarmpal.io import create_paldata, PalDataItem\n",
-                "from swarmpal.toolboxes import tfa"
+                "import swarmpal.toolboxes.tfa.tfa_processor as tfa"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Provide values for the parameters of the analysis.  The `dataset` can be chosen from one of the compatible magnetic data collections, and the `var` is a VirES-compatible variable string (see [viresclient](https://viresclient.readthedocs.io/en/latest/available_parameters.html) for more information). The \"start\" and \"end\" times must be given as a datetime object. If the data are required as they are, set the `remove_chaos_model` parameter to False. Otherwise, if the inputs are magnetic field data and the analysis requires subtraction of the model field, set the parameter to True. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dataset = \"SW_OPER_MAGA_LR_1B\"\n",
+                "var = \"F\"\n",
+                "remove_chaos_model = False\n",
+                "time_start = dt.datetime(2015, 3, 18)\n",
+                "time_end = dt.datetime(2015, 3, 18, 0, 15, 0)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "66a7fe5b-7589-4ead-b72a-3b28c4fd4fb2",
             "metadata": {},
             "source": [
-                "Get some data and apply the preprocessing."
+                "Now run the TfaInput to retrieve the selected data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "145c4054-3285-47dd-b858-83f5d5b1d8ce",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = create_paldata(\n",
-                "    PalDataItem.from_vires(\n",
-                "        collection=\"SW_OPER_MAGA_LR_1B\",\n",
-                "        measurements=[\"F\"],\n",
-                "        start_time=dt.datetime(2015, 3, 18),\n",
-                "        end_time=dt.datetime(2015, 3, 18, 0, 15, 0),\n",
-                "        server_url=\"https://vires.services/ows\",\n",
-                "        options=dict(asynchronous=False, show_progress=False),\n",
-                "    )\n",
+                "inputs = tfa.TfaInput(\n",
+                "    collection=dataset,\n",
+                "    start_time=time_start,\n",
+                "    end_time=time_end,\n",
+                "    initialise=True,\n",
+                "    varname=var,\n",
+                "    sampling_time=\"PT1S\",\n",
+                "    remove_chaos=remove_chaos_model,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a2a8ccce-d99c-4ea8-9212-8cec709c0923",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p1 = tfa.processes.Preprocess()\n",
-                "p1.set_config(\n",
-                "    dataset=\"SW_OPER_MAGA_LR_1B\",\n",
-                "    active_variable=\"F\",\n",
-                "    sampling_rate=1,\n",
-                ")\n",
-                "p1(data);"
+                "# inputs.to_file('using_tfa.nc')\n",
+                "# inputs.initialise('using_tfa.nc')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f702d99f-a102-4ef2-b50f-7874295228e7",
             "metadata": {},
             "source": [
-                "The `TFA_Variable` has been set with the content of `F` (the scalar magnetic data)."
+                "The data now contains everything we need to start the processing. This data is contained in the `.xarray` attribute:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9b4b9baf-2e38-430a-9db8-e86b00efa8e8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"TFA_Variable\"].plot.line(x=\"TFA_Time\");"
+                "inputs.xarray"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "89e457c7-bb2e-4e15-9fb1-b90149d45be4",
             "metadata": {},
             "source": [
-                "Let's test the analysis with an artificial series, so we'll replace the `TFA_Variable` with a time series of our choice, with a specific frequency of 40 mHz (i.e. 25 sec) and amplitude of 4 nT.\n",
+                "Let's first test the analysis with an artificial series, so we'll replace the `F` variable with a time series of our choice, with a specific frequency of 40 mHz (i.e. 25 sec) and amplitude of 4 nT. \n",
                 "\n",
-                "To test the cleaning we'll add some random spikes as well."
+                "To test the cleaning we'll add some random spikes as well"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "480c693b-41f4-4658-8fc4-885334596419",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Get a test wave with the same length as the data, sampled at 1Hz\n",
-                "N = data[\"SW_OPER_MAGA_LR_1B\"][\"TFA_Variable\"].shape[0]\n",
+                "N = inputs.xarray[\"F\"].shape[0]  # get the length of the data\n",
                 "test_wave = 4 * np.sin(2 * np.pi * np.arange(N) / 50)\n",
-                "# Create ten spikes at ten random locations\n",
-                "np.random.seed(0)\n",
-                "spike_locations = np.random.randint(\n",
-                "    0,\n",
-                "    N,\n",
-                "    10,\n",
-                ")\n",
+                "# test_wave = np.ones(N)\n",
+                "\n",
+                "# create ten spikes at ten random locations\n",
+                "spike_locations = np.random.randint(0, 1000, 10) + int(N / 2) - 500\n",
                 "test_wave[spike_locations] = test_wave[spike_locations] + 4\n",
-                "# Overwrite the data with the test data\n",
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"TFA_Variable\"].data = test_wave"
+                "inputs.xarray[\"F\"].data = test_wave"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To use the processing capabilities of TFA we create a `TfaProcessor` object, that contains the variable of choice."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "processor = tfa.TfaProcessor(inputs, active_variable={\"varname\": var})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5332d5c3-f13c-43c3-97d1-ad255c398da9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"TFA_Variable\"].plot.line(x=\"TFA_Time\");"
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "103811c5-72dd-4c49-9319-238356a64940",
             "metadata": {},
             "source": [
-                "Let's see the effect of the cleaning routine..."
+                "To perform cleaning on the data, we initialize a `Cleaning` object with the parameters of our choice and then apply it on the data with the `TfaProcessor` `apply()` function.\n",
+                "The active variable series can be plotted by means of the `plotX()` function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1424d095-c5c7-409d-aebc-7dc6c6f931ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p2 = tfa.processes.Clean()\n",
-                "p2.set_config(\n",
-                "    window_size=10,\n",
-                "    method=\"iqr\",\n",
-                "    multiplier=0.5,\n",
-                ")\n",
-                "p2(data)\n",
-                "data[\"SW_OPER_MAGA_LR_1B\"][\"TFA_Variable\"].plot.line(x=\"TFA_Time\");"
+                "c = tfa.Cleaning()\n",
+                "processor.apply(c)\n",
+                "processor.plotX()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1b0e36d6-b25f-4536-802f-320c3b524efa",
             "metadata": {},
             "source": [
-                "... and the filtering..."
+                "Similarly, the filtering can be performed by first initializing a `Filtering` object with the parameters of our choosing and the applying in on the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3aadd612-7864-4d5e-a83e-819ec676ae15",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p3 = tfa.processes.Filter()\n",
-                "p3.set_config(\n",
-                "    cutoff_frequency=10 / 1000,\n",
-                ")\n",
-                "p3(data)\n",
-                "tfa.plotting.time_series(data);"
+                "f = tfa.Filtering()\n",
+                "processor.apply(f)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "793e5ef9-577b-47f8-b6ef-2fba29f24710",
             "metadata": {},
             "source": [
-                "Next the wavelet transform is applied..."
+                "In the same way, the wavelet transform is applied"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4321c622-ea6c-4b48-992c-5c3de8a05004",
             "metadata": {},
             "outputs": [],
             "source": [
-                "p4 = tfa.processes.Wavelet()\n",
-                "p4.set_config(\n",
-                "    min_frequency=10 / 1000,\n",
-                "    max_frequency=100 / 1000,\n",
-                "    dj=0.1,\n",
-                ")\n",
-                "p4(data);"
+                "w = tfa.Wavelet()\n",
+                "processor.apply(w)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The result of the wavelet can be visualized by means of the `image()` function. Set the `log` parameter to True to plot the log-10 of the results or False to plot them as they are. The optional parameter `cbar_lims` can be set to specify the limits of the colorbar for the spectral plot."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a5e09b36-2486-4a1a-b212-d477858ea2f6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tfa.plotting.spectrum(data, levels=np.linspace(0, 4, 20), log=False, extra_x=None);"
+                "processor.image(log=False, cbar_lims=[0, 4])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "93f1af27-1d18-43fa-ac54-e81134b9391d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "plt.plot(\n",
-                "    1 / data[\"SW_OPER_MAGA_LR_1B\"][\"scale\"].data,\n",
-                "    data[\"SW_OPER_MAGA_LR_1B\"][\"wavelet_power\"][:, int(N / 2)],\n",
+                "    1 / processor.input_data.xarray[\"scale\"].data,\n",
+                "    processor.input_data.xarray[\"wavelet_power\"][:, int(N / 2)],\n",
                 "    \"-x\",\n",
-                ");"
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fft_freq = np.arange(1, 2190) / N\n",
+                "F = np.abs(np.fft.fft(processor.input_data.xarray[\"X\"].data)[1:2190]) / (N / 2)\n",
+                "plt.plot(fft_freq, F)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "(\n",
+                "    np.sum(processor.input_data.xarray[\"wavelet_power\"].data[:, int(N / 2)]),\n",
+                "    np.sum(F**2),\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The same result holds even if one changes the frequency resolution."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "w = tfa.Wavelet(\n",
+                "    {\n",
+                "        \"Min_Scale\": 1000 / 50,\n",
+                "        \"Max_Scale\": 1000 / 5,\n",
+                "        \"dj\": 0.01,\n",
+                "    }\n",
+                ")\n",
+                "processor.apply(w)\n",
+                "plt.subplot(1, 2, 1)\n",
+                "plt.plot(\n",
+                "    1 / processor.input_data.xarray[\"scale\"].data,\n",
+                "    processor.input_data.xarray[\"wavelet_power\"][:, int(N / 2)],\n",
+                "    \"-x\",\n",
+                ")\n",
+                "plt.subplot(1, 2, 2)\n",
+                "processor.image(log=False, cbar_lims=[0, 0.2])\n",
+                "np.sum(processor.input_data.xarray[\"wavelet_power\"].data[:, int(N / 2)])"
             ]
         }
     ],
     "metadata": {
+        "interpreter": {
+            "hash": "87d67a24c2c5892c025cb327df6d3922c0a9d4e9219e4fcf3b6836bad3fb9136"
+        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `swarmpal-0.1.0/docs/index.md` & `swarmpal-0.1.0a4/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 000000f0: 6465 732f 6661 632f 696e 7472 6f5f 6661  des/fac/intro_fa
 00000100: 630a 6775 6964 6573 2f64 7365 6373 2f69  c.guides/dsecs/i
 00000110: 6e74 726f 5f64 7365 6373 0a67 7569 6465  ntro_dsecs.guide
 00000120: 732f 7466 612f 696e 7472 6f5f 7466 610a  s/tfa/intro_tfa.
 00000130: 6060 600a 0a60 6060 7b74 6f63 7472 6565  ```..```{toctree
 00000140: 7d0a 3a68 6964 6465 6e3a 0a3a 6d61 7864  }.:hidden:.:maxd
 00000150: 6570 7468 3a20 320a 3a63 6170 7469 6f6e  epth: 2.:caption
-00000160: 3a20 5446 4120 546f 6f6c 626f 780a 0a67  : TFA Toolbox..g
-00000170: 7569 6465 732f 7466 612f 7466 615f 6261  uides/tfa/tfa_ba
-00000180: 636b 6772 6f75 6e64 0a67 7569 6465 732f  ckground.guides/
-00000190: 7466 612f 7466 615f 4d41 4778 5f4c 520a  tfa/tfa_MAGx_LR.
-000001a0: 6775 6964 6573 2f74 6661 2f74 6661 5f4d  guides/tfa/tfa_M
-000001b0: 4147 785f 4852 0a67 7569 6465 732f 7466  AGx_HR.guides/tf
-000001c0: 612f 7466 615f 4546 4978 5f54 4354 0a67  a/tfa_EFIx_TCT.g
-000001d0: 7569 6465 732f 7466 612f 7466 615f 4155  uides/tfa/tfa_AU
-000001e0: 585f 4f42 530a 6775 6964 6573 2f74 6661  X_OBS.guides/tfa
-000001f0: 2f74 6661 5f43 6c75 7374 6572 0a60 6060  /tfa_Cluster.```
-00000200: 0a0a 6060 607b 746f 6374 7265 657d 0a3a  ..```{toctree}.:
-00000210: 6869 6464 656e 3a0a 3a6d 6178 6465 7074  hidden:.:maxdept
-00000220: 683a 2032 0a3a 6361 7074 696f 6e3a 2046  h: 2.:caption: F
-00000230: 6f72 2064 6576 656c 6f70 6572 730a 0a67  or developers..g
-00000240: 7569 6465 732f 7368 6172 6564 2f70 616c  uides/shared/pal
-00000250: 6461 7461 0a60 6060 0a0a 6060 607b 746f  data.```..```{to
-00000260: 6374 7265 657d 0a3a 6869 6464 656e 3a0a  ctree}.:hidden:.
-00000270: 3a6d 6178 6465 7074 683a 2032 0a3a 6361  :maxdepth: 2.:ca
-00000280: 7074 696f 6e3a 2041 5049 0a0a 6170 692f  ption: API..api/
-00000290: 696f 0a61 7069 2f66 6163 0a61 7069 2f64  io.api/fac.api/d
-000002a0: 7365 6373 0a61 7069 2f74 6661 0a60 6060  secs.api/tfa.```
-000002b0: 0a                                       .
+00000160: 3a20 5446 4120 546f 6f6c 626f 7820 286f  : TFA Toolbox (o
+00000170: 6c64 2066 6f72 6d29 0a0a 6775 6964 6573  ld form)..guides
+00000180: 2f74 6661 2f75 7369 6e67 5f74 6661 0a67  /tfa/using_tfa.g
+00000190: 7569 6465 732f 7466 612f 7573 696e 675f  uides/tfa/using_
+000001a0: 7466 615f 310a 6775 6964 6573 2f74 6661  tfa_1.guides/tfa
+000001b0: 2f75 7369 6e67 5f74 6661 5f32 0a67 7569  /using_tfa_2.gui
+000001c0: 6465 732f 7466 612f 7573 696e 675f 7466  des/tfa/using_tf
+000001d0: 615f 330a 6775 6964 6573 2f74 6661 2f75  a_3.guides/tfa/u
+000001e0: 7369 6e67 5f74 6661 5f34 0a60 6060 0a0a  sing_tfa_4.```..
+000001f0: 6060 607b 746f 6374 7265 657d 0a3a 6869  ```{toctree}.:hi
+00000200: 6464 656e 3a0a 3a6d 6178 6465 7074 683a  dden:.:maxdepth:
+00000210: 2032 0a3a 6361 7074 696f 6e3a 2046 6f72   2.:caption: For
+00000220: 2064 6576 656c 6f70 6572 730a 0a67 7569   developers..gui
+00000230: 6465 732f 7368 6172 6564 2f70 616c 6461  des/shared/palda
+00000240: 7461 0a67 7569 6465 732f 7368 6172 6564  ta.guides/shared
+00000250: 2f64 6174 615f 696f 0a60 6060 0a0a 6060  /data_io.```..``
+00000260: 607b 746f 6374 7265 657d 0a3a 6869 6464  `{toctree}.:hidd
+00000270: 656e 3a0a 3a6d 6178 6465 7074 683a 2032  en:.:maxdepth: 2
+00000280: 0a3a 6361 7074 696f 6e3a 2041 5049 0a0a  .:caption: API..
+00000290: 6170 692f 696f 0a61 7069 2f66 6163 0a61  api/io.api/fac.a
+000002a0: 7069 2f64 7365 6373 0a61 7069 2f74 6661  pi/dsecs.api/tfa
+000002b0: 0a60 6060 0a                             .```.
```

### Comparing `swarmpal-0.1.0/docs/installation.md` & `swarmpal-0.1.0a4/docs/installation.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Installation
 
-## Swarm Virtual Research Environment
+## ESA Virtual Research Environment
 
-The easiest way to use SwarmPAL is in the Swarm Virtual Research Environment (read more [here](https://notebooks.vires.services/)). To get started with the SwarmPAL demo tool (which includes the examples given on these pages, as interactive notebooks), follow this link: [![Swarm-VRE](https://img.shields.io/badge/%F0%9F%9A%80%20launch-Swarm--VRE-blue)](https://vre.vires.services/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fsmithara%2Fswarmpal-demo&urlpath=lab%2Ftree%2Fswarmpal-demo%2FREADME.ipynb&branch=main)
+> To be updated
 
 ## Install latest release
 
-The package is available from PyPI:
+> To be updated
+
+<!-- The package is available from PyPI:
 
 ```bash
 pip install swarmpal
-```
+``` -->
 
 :::{admonition} New to Python?
 :class: note
 
 To setup Python on your system, check guidance on the [viresclient installation notes](https://viresclient.readthedocs.io/en/latest/installation.html#recommended-setup-if-starting-without-python-already)
 :::
```

### Comparing `swarmpal-0.1.0/docs/make.bat` & `swarmpal-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/environment.yml` & `swarmpal-0.1.0a4/environment.yml`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/noxfile.py` & `swarmpal-0.1.0a4/noxfile.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/pyproject.toml` & `swarmpal-0.1.0a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "swarmpal"
 authors = [
-    { name = "Ashley Smith", email = "ashley.smith@ed.ac.uk" },
+    { name = "Ashley Smith", email = "ashley.smith@magneticearth.org" },
 ]
 maintainers = [
-    { name = "Ashley Smith", email = "ashley.smith@ed.ac.uk" },
+    { name = "Ashley Smith", email = "ashley.smith@magneticearth.org" },
 ]
 license = { file = "LICENSE" }
 
 description = "Toolbox for ESA's Swarm mission"
 readme = "README.md"
 
 requires-python = ">=3.8"
@@ -26,22 +26,22 @@
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 1 - Planning",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
     "hapiclient >= 0.2.3",
-    "numpy >= 1.21",
+    "numpy >= 1.22",
     "matplotlib >= 3.5",
     "scipy >= 1.8",
     "viresclient >= 0.11",
     "xarray >= 0.21",
     "xarray-datatree >= 0.0.11",
 ]
```

### Comparing `swarmpal-0.1.0/src/swarmpal/io/_datafetchers.py` & `swarmpal-0.1.0a4/src/swarmpal/io/_datafetchers.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/io/_paldata.py` & `swarmpal-0.1.0a4/src/swarmpal/io/_paldata.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,51 +187,28 @@
         params = PalDataItem._update_start_end_times(params, *times_to_fetch)
         return (params, analysis_window)
 
     @staticmethod
     def from_vires(**params) -> PalDataItem:
         """Create PalDataItem from VirES source
 
-        Parameters
-        ----------
-        collection : str
-        measurements : list[str]
-        start_time : str | datetime
-        end_time : str | datetime
-        models : list[str]
-        auxiliaries : list[str]
-        sampling_step : str
-        filters : list[str]
-        options : dict
-        server_url : str
-            defaults to "https://vires.services/ows"
-        pad_times : tuple[timedelta]
-            This is handled specially by SwarmPAL and not passed to viresclient
+        TODO: Detail params given by swarmpal.io.datafetchers.ViresParameters
         """
         params, analysis_window = PalDataItem._pad_times(params)
         fetcher = get_fetcher("vires")(**params)
         pdi = PalDataItem(fetcher)
         pdi.analysis_window = analysis_window
         pdi.dataset_name = params.get("collection")
         return pdi
 
     @staticmethod
     def from_hapi(**params) -> PalDataItem:
         """Create PalDataItem from HAPI source
 
-        Parameters
-        ----------
-        server : str
-        dataset : str
-        parameters : str
-        start : str
-        stop : str
-        options : dict
-        pad_times : tuple[timedelta]
-            This is handled specially by SwarmPAL and not passed to hapiclient
+        TODO: Detail params given by swarmpal.io.datafetchers.HapiParameters
         """
         params, analysis_window = PalDataItem._pad_times(params)
         fetcher = get_fetcher("hapi")(**params)
         pdi = PalDataItem(fetcher)
         pdi.analysis_window = analysis_window
         pdi.dataset_name = params.get("dataset")
         return pdi
@@ -275,14 +252,68 @@
         """
         if xarray_dataset:
             params["xarray_dataset"] = xarray_dataset
         fetcher = get_fetcher("manual")(**params)
         return PalDataItem(fetcher)
 
 
+class PalData:
+    """Holds an Xarray DataTree of PAL inputs and outputs
+
+    - PalData can be created from PalDataItem objects passed to .set_inputs.
+    - PalData can be created from existing datatree (e.g. stored on disk)
+        See https://xarray-datatree.readthedocs.io/en/latest/io.html
+    - The data is stored within the .datatree property.
+
+    Parameters
+    ----------
+    name: str
+        Provide a name to label the datatree
+    datatree: DataTree
+        Provide an existing DataTree directly instead
+
+    Examples
+    --------
+    >>> from swarmpal.io import PalData, PalDataItem
+    >>>
+    >>> params = dict(
+    >>>     collection="SW_OPER_MAGA_LR_1B",
+    >>>     measurements=["F", "B_NEC"],
+    >>>     start_time="2016-01-01T00:00:00",
+    >>>     end_time="2016-01-02T00:00:00",
+    >>>     server_url="https://vires.services/ows",
+    >>> )
+    >>> my_pal = PalData(name="trial")
+    >>> my_pal.set_inputs(
+    >>>     SwarmAlpha=PalDataItem.from_vires(**params)
+    >>> )
+    >>> # Access data directly through the datatree
+    >>> my_pal.datatree["inputs/SwarmAlpha"]
+    """
+
+    def __init__(self, name: str | None = None, datatree: DataTree | None = None):
+        self.datatree = datatree if datatree else DataTree(name=name)
+
+    def set_inputs(self, **paldataitems: PalDataItem):
+        """Supply named input datasets through PalDataItem
+
+        Parameters
+        ----------
+        **paldataitems_kw: PalDataItem
+            Provide instances of PalDataItem as keyword arguments
+        """
+        if self.datatree:
+            logger.warn(" Resetting contents of PalData")
+            self.datatree = DataTree(name=self.datatree.name)
+        for name, item in paldataitems.items():
+            # Use paldataitems to populate the DataTree; triggers download
+            self.datatree[f"inputs/{name}"] = DataTree(item.xarray)
+            # TODO: Validate and extract PAL meta as a property
+
+
 class PalMeta:
     @staticmethod
     def serialise(meta: dict) -> str:
         def _format_handler(x):
             if isinstance(x, datetime):
                 return x.isoformat()
             raise TypeError("Unknown type")
```

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/aux_tools.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/aux_tools.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/dsecs_algorithms.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/dsecs_algorithms.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/dsecs/processes.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/dsecs/processes.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/fac/fac_algorithms.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/fac/fac_algorithms.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/fac/processes.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/fac/processes.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/plotting.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,15 @@
         ax_new.set_xticks(ax.get_xticks())
         ax_new.set_xticklabels(x, rotation=30, horizontalalignment="left")
         return ax_new
 
     # Place the first secondary x-axis
     ax_new = add_xaxis(varname=varnames[0], yposition=1.02)
     # Find the height of the placed labels, in figure coordinates
-    bbox = ax_new.get_xticklabels()[0].get_window_extent(
-        renderer=ax.figure.canvas.get_renderer()
-    )
+    bbox = ax_new.get_xticklabels()[0].get_window_extent()
     bbox = bbox.transformed(ax.figure.dpi_scale_trans.inverted())
     label_height = bbox.height
     # Recalculate that height as a fraction of main axes height
     bbox_ax = ax.get_window_extent()
     bbox_ax = bbox_ax.transformed(ax.figure.dpi_scale_trans.inverted())
     label_height = label_height / bbox_ax.height
     # Increase it to account for the extra height taken by label rotation(?)
```

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/processes.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/processes.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/src/swarmpal/toolboxes/tfa/tfalib.py` & `swarmpal-0.1.0a4/src/swarmpal/toolboxes/tfa/tfalib.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/tests/io/test_datafetchers.py` & `swarmpal-0.1.0a4/tests/io/test_datafetchers.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/tests/io/test_paldata.py` & `swarmpal-0.1.0a4/tests/io/test_paldata.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/tests/io/test_palprocess.py` & `swarmpal-0.1.0a4/tests/io/test_palprocess.py`

 * *Files identical despite different names*

### Comparing `swarmpal-0.1.0/PKG-INFO` & `swarmpal-0.1.0a4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: swarmpal
-Version: 0.1.0
+Version: 0.1.0a4
 Summary: Toolbox for ESA's Swarm mission
-Author-email: Ashley Smith <ashley.smith@ed.ac.uk>
-Maintainer-email: Ashley Smith <ashley.smith@ed.ac.uk>
+Author-email: Ashley Smith <ashley.smith@magneticearth.org>
+Maintainer-email: Ashley Smith <ashley.smith@magneticearth.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Requires-Dist: hapiclient >= 0.2.3
-Requires-Dist: numpy >= 1.21
+Requires-Dist: numpy >= 1.22
 Requires-Dist: matplotlib >= 3.5
 Requires-Dist: scipy >= 1.8
 Requires-Dist: viresclient >= 0.11
 Requires-Dist: xarray >= 0.21
 Requires-Dist: xarray-datatree >= 0.0.11
 Requires-Dist: pytest >=6 ; extra == "dev"
 Requires-Dist: nox >=2022 ; extra == "dev"
@@ -42,21 +42,16 @@
 Provides-Extra: docs
 Provides-Extra: dsecs
 Provides-Extra: test
 
 # SwarmPAL
 
 ---
-[![Swarm-VRE](https://img.shields.io/badge/%F0%9F%9A%80%20launch-Swarm--VRE-blue)](https://vre.vires.services/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fsmithara%2Fswarmpal-demo&urlpath=lab%2Ftree%2Fswarmpal-demo%2FREADME.ipynb&branch=main)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/smithara/swarmpal-demo/HEAD)
-
-[![PyPI](https://img.shields.io/pypi/v/swarmpal)]( https://pypi.org/project/swarmpal/)
 [![Documentation](https://img.shields.io/badge/docs-online-success)][rtd-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
-
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 ---
 
 [actions-badge]:            https://github.com/Swarm-DISC/SwarmPAL/workflows/CI/badge.svg
@@ -71,12 +66,9 @@
 [github-discussions-link]:  https://github.com/Swarm-DISC/SwarmPAL/discussions
 [pypi-link]:                https://pypi.org/project/swarmpal/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/swarmpal
 [pypi-version]:             https://badge.fury.io/py/swarmpal.svg
 [rtd-badge]:                https://img.shields.io/badge/docs-online-success
 [rtd-link]:                 https://swarmpal.readthedocs.io/
 
-![SwarmPAL diagram](https://swarmpal-benchmarks.netlify.app/swarmpal-diagram.png)
-
-For more information see:
-- <https://swarmdisc.org/lab/>
+See the [SwarmPAL development guide on HackMD](https://hackmd.io/@swarm/dev/%2Ff6YIHfqxT9yL0giWJzhr_Q)
```

