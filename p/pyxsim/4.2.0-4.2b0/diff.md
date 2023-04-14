# Comparing `tmp/pyxsim-4.2.0.tar.gz` & `tmp/pyxsim-4.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxsim-4.2.0.tar", last modified: Fri Apr 14 17:21:46 2023, max compression
+gzip compressed data, was "pyxsim-4.2b0.tar", last modified: Fri Jan 20 16:20:25 2023, max compression
```

## Comparing `pyxsim-4.2.0.tar` & `pyxsim-4.2b0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.598724 pyxsim-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 17:21:32.000000 pyxsim-4.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.582724 pyxsim-4.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.586724 pyxsim-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-14 17:21:32.000000 pyxsim-4.2.0/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-14 17:21:32.000000 pyxsim-4.2.0/.github/workflows/wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 17:21:32.000000 pyxsim-4.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 17:21:32.000000 pyxsim-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-14 17:21:32.000000 pyxsim-4.2.0/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:32.000000 pyxsim-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 17:21:46.598724 pyxsim-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-14 17:21:32.000000 pyxsim-4.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       14 2023-04-14 17:21:32.000000 pyxsim-4.2.0/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.586724 pyxsim-4.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.586724 pyxsim-4.2.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.590724 pyxsim-4.2.0/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   415373 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/allsky.png
--rw-r--r--   0 runner    (1001) docker     (123)   724590 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/art_xrbs.png
--rw-r--r--   0 runner    (1001) docker     (123)   278049 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/cluster_merger_events.png
--rw-r--r--   0 runner    (1001) docker     (123)   379332 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/enzo_xrbs.png
--rw-r--r--   0 runner    (1001) docker     (123)   293296 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/gizmo_xrbs.png
--rw-r--r--   0 runner    (1001) docker     (123)   384954 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/light_cone.png
--rw-r--r--   0 runner    (1001) docker     (123)    90172 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/projected_emiss.png
--rw-r--r--   0 runner    (1001) docker     (123)   326571 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/projected_intensity.png
--rw-r--r--   0 runner    (1001) docker     (123)   289700 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/_images/schematic.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.590724 pyxsim-4.2.0/doc/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/api/event_list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/api/photon_list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/api/source_generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/api/source_models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23937 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.590724 pyxsim-4.2.0/doc/source/cookbook/
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/Advanced_Thermal_Emission.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/Line_Emission.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/More_Advanced_Thermal_Emission.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/Power_Law.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/Thermal_Emission.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/cookbook/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/getting_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/parallel.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/doc/source/photon_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/allsky.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/event_lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/generation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/instruments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/light_cone.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/photon_lists/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/doc/source/source_models/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/source_models/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/source_models/line_sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/source_models/powerlaw_sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/source_models/thermal_sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/spectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/v3_to_v4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-14 17:21:32.000000 pyxsim-4.2.0/doc/source/xray_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/pyxsim/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/event_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/pyxsim/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/lib/interpolate.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/lib/sky_functions.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/lib/spectra.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/light_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)    40682 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/photon_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/pyxsim/source_models/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/source_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/source_models/line_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/source_models/power_law_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/source_models/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    38949 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/source_models/thermal_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/spectral_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.598724 pyxsim-4.2.0/pyxsim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_beta_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_light_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_line_emission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_pixel_to_cel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_power_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_sloshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-04-14 17:21:32.000000 pyxsim-4.2.0/pyxsim/xray_binaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.594724 pyxsim-4.2.0/pyxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 17:21:46.000000 pyxsim-4.2.0/pyxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-14 17:21:46.000000 pyxsim-4.2.0/pyxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:21:46.000000 pyxsim-4.2.0/pyxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 17:21:46.000000 pyxsim-4.2.0/pyxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 17:21:46.000000 pyxsim-4.2.0/pyxsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-14 17:21:46.598724 pyxsim-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-14 17:21:32.000000 pyxsim-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:21:46.598724 pyxsim-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 17:21:32.000000 pyxsim-4.2.0/tests/ci_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.108452 pyxsim-4.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-20 16:20:11.000000 pyxsim-4.2b0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.088452 pyxsim-4.2b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.096452 pyxsim-4.2b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-20 16:20:11.000000 pyxsim-4.2b0/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-20 16:20:11.000000 pyxsim-4.2b0/.github/workflows/wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-20 16:20:11.000000 pyxsim-4.2b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-20 16:20:11.000000 pyxsim-4.2b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-20 16:20:11.000000 pyxsim-4.2b0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:11.000000 pyxsim-4.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-20 16:20:25.108452 pyxsim-4.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-01-20 16:20:11.000000 pyxsim-4.2b0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       14 2023-01-20 16:20:11.000000 pyxsim-4.2b0/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.096452 pyxsim-4.2b0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.096452 pyxsim-4.2b0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.100452 pyxsim-4.2b0/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   415373 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/allsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)   724590 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/art_xrbs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278049 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/cluster_merger_events.png
+-rw-r--r--   0 runner    (1001) docker     (123)   379332 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/enzo_xrbs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   293296 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/gizmo_xrbs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   384954 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/light_cone.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90172 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/projected_emiss.png
+-rw-r--r--   0 runner    (1001) docker     (123)   326571 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/projected_intensity.png
+-rw-r--r--   0 runner    (1001) docker     (123)   289700 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/_images/schematic.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/doc/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/api/event_list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/api/photon_list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/api/source_generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/api/source_models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/doc/source/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/Advanced_Thermal_Emission.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/Line_Emission.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/More_Advanced_Thermal_Emission.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/Power_Law.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/Thermal_Emission.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/cookbook/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/getting_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/parallel.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/doc/source/photon_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/allsky.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/event_lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/instruments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/light_cone.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/photon_lists/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/doc/source/source_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/source_models/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/source_models/line_sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/source_models/powerlaw_sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/source_models/thermal_sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/spectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/v3_to_v4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-01-20 16:20:11.000000 pyxsim-4.2b0/doc/source/xray_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/pyxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/event_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/pyxsim/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/lib/interpolate.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/lib/sky_functions.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/lib/spectra.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/light_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40093 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/photon_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.108452 pyxsim-4.2b0/pyxsim/source_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/source_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/source_models/line_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/source_models/power_law_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/source_models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38955 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/source_models/thermal_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22002 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/spectral_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.108452 pyxsim-4.2b0/pyxsim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_beta_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_light_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_line_emission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_pixel_to_cel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_power_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_sloshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-01-20 16:20:11.000000 pyxsim-4.2b0/pyxsim/xray_binaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.104452 pyxsim-4.2b0/pyxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-20 16:20:24.000000 pyxsim-4.2b0/pyxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-20 16:20:25.000000 pyxsim-4.2b0/pyxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 16:20:24.000000 pyxsim-4.2b0/pyxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-20 16:20:24.000000 pyxsim-4.2b0/pyxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-20 16:20:24.000000 pyxsim-4.2b0/pyxsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-20 16:20:25.108452 pyxsim-4.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-01-20 16:20:11.000000 pyxsim-4.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:20:25.108452 pyxsim-4.2b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-20 16:20:11.000000 pyxsim-4.2b0/tests/ci_install.sh
```

### Comparing `pyxsim-4.2.0/.github/workflows/build-test.yml` & `pyxsim-4.2b0/.github/workflows/build-test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -46,8 +46,8 @@
                   python-version: ${{matrix.python-version}}
             - name: Install dependencies and pyxsim
               shell: bash
               env:
                   mode: testing
               run: source ./tests/ci_install.sh
             - name: Run Tests
-              run: py.test -vv pyxsim/tests
+              run: py.test -vv pyxsim/tests --answer_dir=$PWD/$ANSWER_VER
```

### Comparing `pyxsim-4.2.0/.github/workflows/wheels.yaml` & `pyxsim-4.2b0/.github/workflows/wheels.yaml`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/.pre-commit-config.yaml` & `pyxsim-4.2b0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
 -   repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 22.12.0
     hooks:
     - id: black-jupyter
 
 -   repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.11.4
     hooks:
     - id: isort
       name: isort (python)
     - id: isort
       name: isort (cython)
       types: [cython]
 -   repo: https://github.com/PyCQA/flake8
```

### Comparing `pyxsim-4.2.0/COPYING.txt` & `pyxsim-4.2b0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/README.md` & `pyxsim-4.2b0/README.md`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/Makefile` & `pyxsim-4.2b0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/make.bat` & `pyxsim-4.2b0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/allsky.png` & `pyxsim-4.2b0/doc/source/_images/allsky.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/art_xrbs.png` & `pyxsim-4.2b0/doc/source/_images/art_xrbs.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/cluster_merger_events.png` & `pyxsim-4.2b0/doc/source/_images/cluster_merger_events.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/enzo_xrbs.png` & `pyxsim-4.2b0/doc/source/_images/enzo_xrbs.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/gizmo_xrbs.png` & `pyxsim-4.2b0/doc/source/_images/gizmo_xrbs.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/light_cone.png` & `pyxsim-4.2b0/doc/source/_images/light_cone.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/projected_emiss.png` & `pyxsim-4.2b0/doc/source/_images/projected_emiss.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/projected_intensity.png` & `pyxsim-4.2b0/doc/source/_images/projected_intensity.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/_images/schematic.png` & `pyxsim-4.2b0/doc/source/_images/schematic.png`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/api/source_models.rst` & `pyxsim-4.2b0/doc/source/api/source_models.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/basic_concepts.rst` & `pyxsim-4.2b0/doc/source/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/changelog.rst` & `pyxsim-4.2b0/doc/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,12 @@
 .. _changelog:
 
 ChangeLog
 =========
 
-Version 4.2.0
--------------
-
-This version of pyXSIM contains one new feature and a critical bugfix.
-
-* A bug introduced upstream in SOXS 4.4.0 caused normalization of emission and
-  spectra in the :class:`~pyxsim.source_models.thermal_sources.IGMSourceModel`
-  to be incorrect. This is fixed in SOXS 4.5.1 and this version requires that
-  version of SOXS to work correctly.
-* The function :func:`~pyxsim.photon_list.make_photons` now has a ``fields_to_keep``
-  option that allows one to store fields other than the positions, velocities, and
-  sizes of cells or particles to the photon list HDF5 file. See :ref:`generate_new`
-  for more details.
-
 Version 4.1.1
 -------------
 
 This version of pyXSIM fixes a bug in the
 :class:`~pyxsim.source_models.thermal_sources.IGMSourceModel` where low density,
 low temperature, and low metallicity plasmas would sometimes result in spectra with
 negative values.
```

### Comparing `pyxsim-4.2.0/doc/source/conf.py` & `pyxsim-4.2b0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,17 +76,17 @@
 author = "John ZuHone"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "4.2.0"
+version = "4.1.1"
 # The full version, including alpha/beta/rc tags.
-release = "4.2.0"
+release = "4.1.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `pyxsim-4.2.0/doc/source/cookbook/Advanced_Thermal_Emission.ipynb` & `pyxsim-4.2b0/doc/source/cookbook/Advanced_Thermal_Emission.ipynb`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/cookbook/Line_Emission.ipynb` & `pyxsim-4.2b0/doc/source/cookbook/Line_Emission.ipynb`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/cookbook/More_Advanced_Thermal_Emission.ipynb` & `pyxsim-4.2b0/doc/source/cookbook/More_Advanced_Thermal_Emission.ipynb`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/cookbook/Power_Law.ipynb` & `pyxsim-4.2b0/doc/source/cookbook/Power_Law.ipynb`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/cookbook/Thermal_Emission.ipynb` & `pyxsim-4.2b0/doc/source/cookbook/Thermal_Emission.ipynb`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/getting_help.rst` & `pyxsim-4.2b0/doc/source/getting_help.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/index.rst` & `pyxsim-4.2b0/doc/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 pyXSIM is released under a
 `BSD 3-clause license <https://opensource.org/licenses/BSD-3-Clause>`_.
 
 Current Version
 ---------------
 
-The current stable version is 4.2.0. See the :ref:`changelog` for details on
+The current stable version is 4.1.1. See the :ref:`changelog` for details on
 changes from previous versions.
 
 Table of Contents
 -----------------
 
 .. toctree::
    :maxdepth: 2
```

#### html2text {}

```diff
@@ -14,13 +14,13 @@
 FLASH, Enzo, and Athena, to particle-based codes such as Gadget and AREPO, and
 even from datasets that have been created "by hand", such as from NumPy arrays.
 pyXSIM also provides facilities for manipulating the synthetic observations it
 produces in various ways, as well as ways to export the simulated X-ray events
 to other software packages to simulate the end products of specific X-ray
 observatories. License ------- pyXSIM is released under a `BSD 3-clause license
 opensource.org/licenses/BSD-3-Clause>`_. Current Version --------------- The
-current stable version is 4.2.0. See the :ref:`changelog` for details on
+current stable version is 4.1.1. See the :ref:`changelog` for details on
 changes from previous versions. Table of Contents ----------------- ..
 toctree:: :maxdepth: 2 installing v3_to_v4 basic_concepts source_models/index
 xray_fields spectra photon_lists/index parallel getting_help cookbook/index
 api/index Indices and tables ================== * :ref:`genindex` * :ref:
 `modindex` * :ref:`search`
```

### Comparing `pyxsim-4.2.0/doc/source/installing.rst` & `pyxsim-4.2b0/doc/source/installing.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/parallel.rst` & `pyxsim-4.2b0/doc/source/parallel.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/allsky.rst` & `pyxsim-4.2b0/doc/source/photon_lists/allsky.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/event_lists.rst` & `pyxsim-4.2b0/doc/source/photon_lists/event_lists.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/generation.rst` & `pyxsim-4.2b0/doc/source/photon_lists/generation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 =======================
 
 A photon list in pyXSIM is a three-dimensional HDF5 dataset that contains a
 distribution of cell or particle positions, velocities, and photon energies
 within each cell or particle. Once created, it be used to generated simulated
 X-ray events from a particular line of sight.
 
-.. _generate_new:
-
 Generating a New Photon List from a Data Source
 -----------------------------------------------
 
 A photon list is generated from a data source, by which we mean any spatially
 extended object in three dimensions represented in yt. For example, we may have
 a dataset of a galaxy cluster simulation, and wish to generate photons from the
 thermal emission of the hot cluster plasma. We can load up the dataset in yt and
@@ -73,17 +71,14 @@
   velocity frame of reference. If not a :class:`~yt.units.yt_array.YTArray`,
   it is assumed to have units of km/s. Default: [0.0, 0.0, 0.0] km/s.
 * ``observer`` (optional): Whether the observer is "external", and the flat-sky
   approximation can be assumed for the purposes of projecting photons onto the
   sky, or the observer is "internal" and a spherical projection is assumed.
   Default is "external". For more details on the "internal" observing mode see
   :ref:`allsky`.
-* ``fields_to_keep`` (optional): A list of fields to add to the HDF5 photon
-  list in addition to the cell or particle positions, velocities, and sizes.
-  Default: None
 
 As an example, we'll assume we have created a ``source_model`` representing the
 thermal emission from the plasma (see :ref:`source-models` for more details on
 how to create one):
 
 .. code-block:: python
 
@@ -131,35 +126,20 @@
 ``"velocity_y"``, and ``"velocity_z"`` for grid/cell-based datasets and
 ``"particle_velocity_x"``, ``"particle_velocity_y"``, and
 ``"particle_velocity_z"`` for particle-based datasets. If you need to use other
 fields, you can specify them using the ``velocity_fields`` keyword argument:
 
 .. code-block:: python
 
-    vfields = [("flash", "velx"), ("flash", "vely"), ("flash", "velz")]
+    vfields = ["velx", "vely", "velz"]
     n_photons, n_cells = pyxsim.make_photons("my_photons", sp, redshift, area,
                                              exp_time, source_model,
                                              center=center, dist=(4., "kpc"),
                                              velocity_fields=vfields)
 
-We can also add other fields to the file using the ``fields_to_keep`` option,
-which will not be used for photon projection in later steps but can be used for
-diagnostic and/or analysis purposes. These represent the fields at the positions
-where photons have been generated from. For example, to add density and
-temperature fields to the file:
-
-.. code-block:: python
-
-    fields_to_keep = [("gas", "density"), ("gas", "temperature")]
-    n_photons, n_cells = pyxsim.make_photons("my_photons", sp, redshift, area,
-                                             exp_time, source_model,
-                                             center=center, dist=(4., "kpc"),
-                                             fields_to_keep=fields_to_keep)
-
-
 Merging Photon Lists
 --------------------
 
 Photon lists which have been written to files can be merged together, using the
 :func:`~pyxsim.utils.merge_files` function. This may be useful if you generate photons from
 different sources or source types that are co-spatial.
```

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/instruments.rst` & `pyxsim-4.2b0/doc/source/photon_lists/instruments.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/light_cone.rst` & `pyxsim-4.2b0/doc/source/photon_lists/light_cone.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/photon_lists/overview.rst` & `pyxsim-4.2b0/doc/source/photon_lists/overview.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/source_models/index.rst` & `pyxsim-4.2b0/doc/source/source_models/index.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/source_models/line_sources.rst` & `pyxsim-4.2b0/doc/source/source_models/line_sources.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/source_models/powerlaw_sources.rst` & `pyxsim-4.2b0/doc/source/source_models/powerlaw_sources.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/source_models/thermal_sources.rst` & `pyxsim-4.2b0/doc/source/source_models/thermal_sources.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/spectra.rst` & `pyxsim-4.2b0/doc/source/spectra.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/v3_to_v4.rst` & `pyxsim-4.2b0/doc/source/v3_to_v4.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/doc/source/xray_fields.rst` & `pyxsim-4.2b0/doc/source/xray_fields.rst`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyproject.toml` & `pyxsim-4.2b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/__init__.py` & `pyxsim-4.2b0/pyxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/event_list.py` & `pyxsim-4.2b0/pyxsim/event_list.py`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/lib/interpolate.pyx` & `pyxsim-4.2b0/pyxsim/lib/interpolate.pyx`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/lib/sky_functions.pyx` & `pyxsim-4.2b0/pyxsim/lib/sky_functions.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             k += 1
 
 
 @cython.cdivision(True)
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def scatter_events(normal, prng, kernel, data_type,
-                   np.int64_t num_det,
+                   int num_det,
                    np.ndarray[np.uint8_t, cast=True] det,
                    np.ndarray[np.int64_t, ndim=1] n_ph,
                    np.ndarray[np.float64_t, ndim=1] x,
                    np.ndarray[np.float64_t, ndim=1] y,
                    np.ndarray[np.float64_t, ndim=1] z,
                    np.ndarray[np.float64_t, ndim=1] dx,
                    np.ndarray[np.float64_t, ndim=1] x_hat,
@@ -178,15 +178,15 @@
         xsky[i] *= 180.0/PI
         ysky[i] *= 180.0/PI
 
 
 @cython.cdivision(True)
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def scatter_events_allsky(data_type, kernel, prng, np.int64_t num_det,
+def scatter_events_allsky(data_type, kernel, prng, int num_det,
                           np.ndarray[np.uint8_t, cast=True] det,
                           np.ndarray[np.int64_t, ndim=1] n_ph,
                           np.ndarray[np.float64_t, ndim=1] x,
                           np.ndarray[np.float64_t, ndim=1] y,
                           np.ndarray[np.float64_t, ndim=1] z,
                           np.ndarray[np.float64_t, ndim=1] dx,
                           np.ndarray[np.float64_t, ndim=1] x_hat,
```

### Comparing `pyxsim-4.2.0/pyxsim/lib/spectra.pyx` & `pyxsim-4.2b0/pyxsim/lib/spectra.pyx`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/light_cone.py` & `pyxsim-4.2b0/pyxsim/light_cone.py`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/photon_list.py` & `pyxsim-4.2b0/pyxsim/photon_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,40 +168,29 @@
         following will be assumed:
         ['velocity_x', 'velocity_y', 'velocity_z'] for grid datasets
         ['particle_velocity_x', 'particle_velocity_y', 'particle_velocity_z'] for particle datasets
     bulk_velocity : array-like, optional
         A 3-element array or list specifying the local velocity frame of
         reference. If not a :class:`~yt.units.yt_array.YTArray`, it is assumed
         to have units of km/s. Default: [0.0, 0.0, 0.0] km/s.
-    observer : string, optional
-        Controls whether the source is at a large distance, in which case
-        the observer sits far outside the source ("external"), or if the
-        observer is inside the X-ray-emitting source ("internal"), such as a
-        galaxy. Default: "external"
-    fields_to_keep : list of tuples
-        A list of fields to add to the HDF5 photon list in addition to the cell
-        or particle positions, velocities, and sizes. Default: None
 
     Returns
     -------
     A tuple of two integers, the number of photons and the number of cells with
     photons
 
     Examples
     --------
-    >>> thermal_model = pyxsim.CIESourceModel("apec", 0.1, 10.0, 1000, 0.3)
+    >>> thermal_model = pyxsim.CIESourceModel(0.1, 10.0, 1000, 0.3)
     >>> redshift = 0.05
     >>> area = 6000.0 # assumed here in cm**2
-    >>> exp_time = 2.0e5 # assumed here in seconds
+    >>> time = 2.0e5 # assumed here in seconds
     >>> sp = ds.sphere("c", (500., "kpc"))
-    >>> fields_to_keep = [("gas", "density"), ("gas", "temperature")]
-    >>> n_photons, n_cells = pyxsim.make_photons(
-    ...     sp, redshift, area, exp_time, thermal_model,
-    ...     fields_to_keep=fields_to_keep
-    ... )
+    >>> n_photons, n_cells = pyxsim.make_photons(sp, redshift, area,
+    ...                                          time, thermal_model)
     """
     ds = data_source.ds
 
     if photon_prefix.endswith(".h5"):
         photon_prefix = photon_prefix[:-3]
 
     if comm.size > 1:
@@ -387,17 +376,19 @@
             dtype=dtype,
             chunks=True,
         )
 
     f.flush()
 
     for chunk in parallel_objects(data_source.chunks([], "io")):
+
         chunk_data = source_model.process_data("photons", chunk, spectral_norm)
 
         if chunk_data is not None:
+
             chunk_nc, number_of_photons, idxs, energies = chunk_data
 
             chunk_nph = np.sum(number_of_photons)
 
             if chunk_nph == 0:
                 continue
 
@@ -481,14 +472,15 @@
     north_vector=None,
     flat_sky=False,
     sigma_pos=None,
     kernel="top_hat",
     save_los=False,
     prng=None,
 ):
+
     from yt.funcs import ensure_numpy_array
 
     prng = parse_prng(prng)
 
     if photon_prefix.endswith(".h5"):
         photon_prefix = photon_prefix[:-3]
 
@@ -570,18 +562,20 @@
         )
 
     d = f["data"]
 
     D_A = p["fid_d_a"][()] * 1.0e3
 
     if d["energy"].size == 0:
+
         mylog.warning("No photons are in file %s, so I am done.", photon_file)
         n_events = 0
 
     else:
+
         fe = h5py.File(event_file, "w")
 
         ie = fe.create_group("info")
         ie.attrs["pyxsim_version"] = pyxsim_version
         ie.attrs["yt_version"] = yt_version
         ie.attrs["soxs_version"] = soxs_version
         ie.attrs["photon_file"] = photon_file
@@ -627,14 +621,15 @@
         n_cells = d["num_photons"].size
 
         pbar = tqdm(
             leave=True, total=n_cells, desc="Projecting photons from cells/particles "
         )
 
         for start_c in range(0, n_cells, cell_chunk):
+
             end_c = min(start_c + cell_chunk, n_cells)
 
             n_ph = d["num_photons"][start_c:end_c]
             x = d["x"][start_c:end_c]
             y = d["y"][start_c:end_c]
             z = d["z"][start_c:end_c]
             dx = d["dx"][start_c:end_c]
@@ -670,21 +665,23 @@
                     + d["vy"][start_c:end_c] * d["vy"][start_c:end_c]
                     + d["vz"][start_c:end_c] * d["vz"][start_c:end_c]
                 )
                 doppler_shift(vn * scale_shift, v2 * scale_shift2, n_ph, eobs)
 
             if absorb_model is None:
                 det = np.ones(eobs.size, dtype="bool")
-                num_det = np.int64(eobs.size)
+                num_det = eobs.size
             else:
                 det = absorb_model.absorb_photons(eobs, prng=prng)
-                num_det = np.int64(det.sum())
+                num_det = det.sum()
 
             if num_det > 0:
+
                 if observer == "external":
+
                     if data_type == "particles":
                         dx *= 0.5
 
                     xsky, ysky, los = scatter_events(
                         norm,
                         prng,
                         kernel,
@@ -712,14 +709,15 @@
                     if flat_sky:
                         xsky = sky_center[0] - np.rad2deg(xsky)
                         ysky = sky_center[1] + np.rad2deg(ysky)
                     else:
                         pixel_to_cel(xsky, ysky, sky_center)
 
                 elif observer == "internal":
+
                     xsky, ysky, los = scatter_events_allsky(
                         data_type,
                         kernel,
                         prng,
                         num_det,
                         det,
                         n_ph,
```

### Comparing `pyxsim-4.2.0/pyxsim/source_models/line_sources.py` & `pyxsim-4.2b0/pyxsim/source_models/line_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,19 +150,21 @@
             data_source.ds, ebins, spec, redshift, dist, cosmology
         )
 
     def make_fluxf(self, emin, emax, energy=False):
         return {"emin": emin, "emax": emax}
 
     def process_data(self, mode, chunk, spectral_norm, fluxf=None, ebins=None):
+
         num_cells = len(chunk[self.emission_field])
 
         norm_field = chunk[self.emission_field]
 
         if mode == "photons":
+
             F = norm_field * spectral_norm * self.scale_factor
             if self.observer == "internal":
                 pos = np.array(
                     [
                         np.ravel(chunk[self.p_fields[i]].to_value("kpc"))
                         for i in range(3)
                     ]
@@ -203,14 +205,15 @@
 
             active_cells = number_of_photons > 0
             ncells = active_cells.sum()
 
             return ncells, number_of_photons[active_cells], active_cells, energies
 
         elif mode in ["photon_field", "energy_field"]:
+
             xlo = fluxf["emin"].v - self.e0.value
             xhi = fluxf["emax"].v - self.e0.value
             if self.sigma is None:
                 if (xlo < 0) & (xhi > 0.0):
                     fac = 1.0
                 else:
                     fac = 0.0
@@ -230,14 +233,15 @@
                         sigma
                         * (np.exp(-0.5 * xhis**2) - np.exp(-0.5 * xlos**2))
                         / np.sqrt(2.0 * np.pi)
                     )
             return fac * norm_field
 
         elif mode == "spectrum":
+
             inv_sf = 1.0 / self.scale_factor
             ee = ebins * inv_sf - self.e0.value
             de = np.diff(ebins * inv_sf)
 
             if isinstance(self.sigma, unyt_quantity):
                 xtmp = ee / self.sigma.value
                 ret = np.interp(xtmp, gx, gcdf)
```

### Comparing `pyxsim-4.2.0/pyxsim/source_models/power_law_sources.py` & `pyxsim-4.2b0/pyxsim/source_models/power_law_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyxsim.lib.spectra import power_law_spectrum
 from pyxsim.source_models.sources import SourceModel
 from pyxsim.utils import mylog, parse_value
 
 
 class PowerLawSourceModel(SourceModel):
-    """
+    r"""
     Initialize a source model from a power-law spectrum.
 
     Parameters
     ----------
     e0 : float, (value, unit) tuple, :class:`~yt.units.yt_array.YTQuantity`, or :class:`~astropy.units.Quantity`
         The reference energy of the power law, in the rest frame of the source.
         If units are not given, they are assumed to be in keV.
@@ -134,14 +134,15 @@
             data_source.ds, ebins, spec, redshift, dist, cosmology
         )
 
     def make_fluxf(self, emin, emax, energy=False):
         return {"emin": emin, "emax": emax}
 
     def process_data(self, mode, chunk, spectral_norm, fluxf=None, ebins=None):
+
         num_cells = len(chunk[self.emission_field])
 
         if isinstance(self.alpha, float):
             alpha = self.alpha * np.ones(num_cells)
         else:
             alpha = chunk[self.alpha].d
 
@@ -149,22 +150,24 @@
             ei = self.emin.v
             ef = self.emax.v
         else:
             ei = fluxf["emin"].v
             ef = fluxf["emax"].v
 
         if mode in ["photons", "photon_field"]:
+
             norm_fac = ef ** (1.0 - alpha) - ei ** (1.0 - alpha)
             norm_fac[alpha == 1] = np.log(ef / ei)
             norm_fac *= self.e0.v**alpha
             norm = norm_fac * chunk[self.emission_field].d
             if np.any(alpha != 1):
                 norm[alpha != 1] /= 1.0 - alpha[alpha != 1]
 
             if mode == "photons":
+
                 norm *= spectral_norm * self.scale_factor
 
                 if self.observer == "internal":
                     pos = np.array(
                         [
                             np.ravel(chunk[self.p_fields[i]].to_value("kpc"))
                             for i in range(3)
@@ -198,23 +201,26 @@
                     ncells,
                     number_of_photons[active_cells],
                     active_cells,
                     energies[:end_e].copy(),
                 )
 
             elif mode == "photon_field":
+
                 return norm
 
         elif mode == "energy_field":
+
             norm_fac = ef ** (2.0 - alpha) - ei ** (2.0 - alpha)
             norm_fac *= self.e0.v**alpha / (2.0 - alpha)
 
             return norm_fac * chunk[self.emission_field].d
 
         elif mode == "spectrum":
+
             inv_sf = 1.0 / self.scale_factor
             emid = 0.5 * (ebins[1:] + ebins[:-1]) * inv_sf / self.e0.v
 
             spec = power_law_spectrum(
                 num_cells, emid, alpha, chunk[self.emission_field].d, self.pbar
             )
```

### Comparing `pyxsim-4.2.0/pyxsim/source_models/sources.py` & `pyxsim-4.2b0/pyxsim/source_models/sources.py`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/pyxsim/source_models/thermal_sources.py` & `pyxsim-4.2b0/pyxsim/source_models/thermal_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
             data_source.ds, ebins, spec, redshift, dist, cosmology
         )
 
     def make_fluxf(self, emin, emax, energy=False):
         return self.spectral_model.make_fluxf(emin, emax, energy=energy)
 
     def process_data(self, mode, chunk, spectral_norm, fluxf=None):
+
         spec = np.zeros(self.nbins)
 
         orig_shape = chunk[self.temperature_field].shape
         if len(orig_shape) == 0:
             orig_ncells = 0
         else:
             orig_ncells = np.prod(orig_shape)
@@ -350,23 +351,25 @@
 
         start_e = 0
         end_e = 0
 
         idxs = np.where(cut)[0]
 
         for ck in chunked(range(num_cells), 100):
+
             ibegin = ck[0]
             iend = ck[-1] + 1
             nck = iend - ibegin
 
             cnm = cell_nrm[ibegin:iend]
 
             kTi = kT[ibegin:iend]
 
             if mode in ["photons", "spectrum"]:
+
                 if self._density_dependence:
                     nHi = nH[ibegin:iend]
                     cspec, mspec, vspec = self.spectral_model.get_spectrum(kTi, nHi)
                 else:
                     cspec, mspec, vspec = self.spectral_model.get_spectrum(kTi)
 
                 tot_spec = cspec
@@ -374,14 +377,15 @@
                 if self.num_var_elem > 0:
                     tot_spec += np.sum(
                         elemZ[:, ibegin:iend, np.newaxis] * vspec, axis=0
                     )
                 np.clip(tot_spec, 0.0, None, out=tot_spec)
 
                 if mode == "photons":
+
                     spec_sum = tot_spec.sum(axis=-1)
                     cell_norm = spec_sum * cnm
 
                     cell_n = np.atleast_1d(self.prng.poisson(lam=cell_norm))
 
                     number_of_photons[ibegin:iend] = cell_n
                     end_e += int(cell_n.sum())
@@ -406,19 +410,21 @@
                         if num_photons_max > energies.size:
                             energies.resize(num_photons_max, refcheck=False)
                         energies[ei : ei + cn] = cell_e
                         ei += cn
                     start_e = end_e
 
                 elif mode == "spectrum":
+
                     spec += np.sum(tot_spec * cnm[:, np.newaxis], axis=0)
 
                 self.pbar.update(nck)
 
             else:
+
                 if self._density_dependence:
                     nHi = nH[ibegin:iend]
                     cflux, mflux, vflux = fluxf(kTi, nHi)
                 else:
                     cflux, mflux, vflux = fluxf(kTi)
 
                 tot_flux = cflux
```

### Comparing `pyxsim-4.2.0/pyxsim/spectral_models.py` & `pyxsim-4.2b0/pyxsim/spectral_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,24 +275,18 @@
         self.de = self.sgen.de
         self.binscale = self.sgen.binscale
         self.Tvals = self.sgen.Tvals
 
     def prepare_spectrum(self, zobs):
         eidxs, ne, ebins, emid, de = self.sgen._get_energies(zobs)
         cosmic_spec, metal_spec, var_spec = self.sgen._get_table(ne, eidxs, zobs)
-        self.cosmic_spec = 1.0e-14 * regrid_spectrum(
-            self.ebins, ebins, cosmic_spec, clip_neg=False
-        )
-        self.metal_spec = 1.0e-14 * regrid_spectrum(
-            self.ebins, ebins, metal_spec, clip_neg=False
-        )
+        self.cosmic_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, cosmic_spec)
+        self.metal_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, metal_spec)
         if var_spec is not None:
-            var_spec = 1.0e-14 * regrid_spectrum(
-                self.ebins, ebins, var_spec, clip_neg=False
-            )
+            var_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, var_spec)
         self.var_spec = var_spec
         self.si = SpectralInterpolator1D(
             self.Tvals, self.cosmic_spec, self.metal_spec, self.var_spec
         )
 
 
 class MekalSpectralModel(Atable1DSpectralModel):
@@ -420,24 +414,18 @@
 
     def prepare_spectrum(self, zobs):
         """
         Prepare the thermal model for execution given a redshift *zobs* for the spectrum.
         """
         eidxs, ne, ebins, emid, de = self.igen._get_energies(zobs)
         cosmic_spec, metal_spec, var_spec = self.igen._get_table(ne, eidxs, zobs)
-        self.cosmic_spec = 1.0e-14 * regrid_spectrum(
-            self.ebins, ebins, cosmic_spec, clip_neg=False
-        )
-        self.metal_spec = 1.0e-14 * regrid_spectrum(
-            self.ebins, ebins, metal_spec, clip_neg=False
-        )
+        self.cosmic_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, cosmic_spec)
+        self.metal_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, metal_spec)
         if var_spec is not None:
-            var_spec = 1.0e-14 * regrid_spectrum(
-                self.ebins, ebins, var_spec, clip_neg=False
-            )
+            var_spec = 1.0e-14 * regrid_spectrum(self.ebins, ebins, var_spec)
         self.var_spec = var_spec
         self.cie_model.prepare_spectrum(zobs)
         self.si = SpectralInterpolator2D(
             self.Tvals, self.Dvals, self.cosmic_spec, self.metal_spec, self.var_spec
         )
 
     def get_spectrum(self, kT, nH):
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/conftest.py` & `pyxsim-4.2b0/pyxsim/tests/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import os
 
 import pytest
 
 
 def pytest_addoption(parser):
+    parser.addoption("--answer_dir", help="Directory where answers are stored.")
     parser.addoption("--check_dir", help="Directory where spectrum checks are stored.")
     parser.addoption(
         "--answer_store",
         action="store_true",
         help="Generate new answers, but don't test.",
     )
 
 
 @pytest.fixture()
 def answer_store(request):
     return request.config.getoption("--answer_store")
 
 
 @pytest.fixture()
+def answer_dir(request):
+    ad = request.config.getoption("--answer_dir")
+    if ad is None:
+        pytest.skip("No answer directory")
+    ad = os.path.abspath(ad)
+    if not os.path.exists(ad):
+        os.makedirs(ad)
+    return ad
+
+
+@pytest.fixture()
 def check_dir(request):
     cd = request.config.getoption("--check_dir")
     if cd is not None:
         cd = os.path.abspath(cd)
         if not os.path.exists(cd):
             os.makedirs(cd)
         cd = os.path.join(cd, f"{request.node.name}.dat")
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_beta_model.py` & `pyxsim-4.2b0/pyxsim/tests/test_beta_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 def test_particle_beta_model_offaxis(check_dir):
     bms = ParticleBetaModelSource()
     do_beta_model(bms, check_dir, prng=67, axis=[1.0, -2.0, 5.0])
 
 
 def do_beta_model(source, check_dir, axis="z", prng=None):
+
     tmpdir = tempfile.mkdtemp()
     curdir = os.getcwd()
     os.chdir(tmpdir)
 
     if prng is None:
         prng = source.prng
 
@@ -120,14 +121,15 @@
     assert pvalue > 0.05
 
     os.chdir(curdir)
     shutil.rmtree(tmpdir)
 
 
 def test_vapec_beta_model(check_dir):
+
     bms = BetaModelSource()
 
     tmpdir = tempfile.mkdtemp()
     curdir = os.getcwd()
     os.chdir(tmpdir)
 
     prng = 50
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_light_cone.py` & `pyxsim-4.2b0/pyxsim/tests/test_light_cone.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pyxsim import CIESourceModel
 from pyxsim.tests.utils import hdf5_answer_testing
 
 
 @importorskip("yt_astro_analysis")
 def test_light_cone(answer_store, answer_dir):
+
     from pyxsim.light_cone import XrayLightCone
 
     prng = RandomState(0x4D3D3D3)
 
     A = 20000.0
     exp_time = 1.0e6
     fov = (0.5, "deg")
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_line_emission.py` & `pyxsim-4.2b0/pyxsim/tests/test_line_emission.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pyxsim.tests.utils import BetaModelSource
 
 cross_section = YTQuantity(500.0e-22, "cm**3/s")
 m_chi = YTQuantity(10.0, "GeV").to_equivalent("g", "mass_energy")
 
 
 def test_line_emission():
+
     tmpdir = tempfile.mkdtemp()
     curdir = os.getcwd()
     os.chdir(tmpdir)
 
     cosmo = Cosmology()
 
     bms = BetaModelSource()
@@ -80,14 +81,15 @@
     assert np.abs(n_E - n_E_pred) < 1.645 * np.sqrt(n_E)
 
     os.chdir(curdir)
     shutil.rmtree(tmpdir)
 
 
 def test_line_emission_fields():
+
     bms = BetaModelSource()
     ds = bms.ds
 
     def _dm_emission(field, data):
         return (
             (data["gas", "dark_matter_density"] / m_chi) ** 2
             * data["cell_volume"]
@@ -135,14 +137,15 @@
     )
     assert_allclose(
         (sphere[line_fields4[-1]] * sphere["cell_volume"]).sum(), 0.5 * dm_E
     )
 
 
 def test_line_emission_spectra():
+
     cosmo = Cosmology()
 
     bms = BetaModelSource()
     ds = bms.ds
 
     def _dm_emission(field, data):
         return data["index", "ones"] * data.ds.quan(1.0e40, "1/s")
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_pixel_to_cel.py` & `pyxsim-4.2b0/pyxsim/tests/test_pixel_to_cel.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from numpy.testing import assert_allclose
 from yt import YTArray, YTQuantity
 
 from pyxsim.lib.sky_functions import pixel_to_cel
 
 
 def test_pixel_to_cel():
+
     prng = RandomState(24)
 
     n_evt = 100000
 
     sky_center = YTArray([30.0, 45.0], "deg")
 
     rr = YTQuantity(100.0, "kpc") * prng.uniform(size=n_evt)
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_power_law.py` & `pyxsim-4.2b0/pyxsim/tests/test_power_law.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 def test_power_law(check_dir):
     plaw_fit(1.1, check_dir, prng=33)
     plaw_fit(0.8, check_dir, prng=28)
     plaw_fit(1.0, check_dir, prng=23)
 
 
 def plaw_fit(alpha_sim, check_dir, prng=None):
+
     tmpdir = tempfile.mkdtemp()
     curdir = os.getcwd()
     os.chdir(tmpdir)
 
     bms = BetaModelSource()
     ds = bms.ds
 
@@ -139,14 +140,15 @@
 
     elum2 = norm * (7.0 - 0.5)
     elum3 = sphere[src_fields2[1]].sum().to_value("keV/s")
     assert_allclose(elum2, elum3)
 
 
 def test_power_law_spectrum():
+
     cosmo = Cosmology()
 
     bms = BetaModelSource()
     ds = bms.ds
 
     def _hard_emission(field, data):
         return (
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_sloshing.py` & `pyxsim-4.2b0/pyxsim/tests/test_sloshing.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     project_photons,
 )
 from pyxsim.tests.utils import hdf5_answer_testing
 
 gslr = "GasSloshingLowRes/sloshing_low_res_hdf5_plt_cnt_0300"
 
 
-def test_sloshing(answer_store):
+def test_sloshing(answer_store, answer_dir):
+
     prng = RandomState(0x4D3D3D3)
 
     ds = yt.load(gslr, default_species_fields="ionized")
     A = 2000.0
     exp_time = 1.0e4
     redshift = 0.1
 
@@ -36,36 +37,36 @@
     thermal_model = CIESourceModel(
         "apec", 0.1, 11.0, 10000, 0.3, thermal_broad=False, prng=prng
     )
     n_photons1, n_cells1 = make_photons(
         "photons1", sphere, redshift, A, exp_time, thermal_model
     )
 
-    hdf5_answer_testing("photons1.h5", answer_store)
+    hdf5_answer_testing("photons1.h5", answer_store, answer_dir)
 
     n_events1 = project_photons(
         "photons1",
         "events1",
         [1.0, -0.5, 0.2],
         [30.0, 45.0],
         absorb_model="tbabs",
         nH=0.1,
         prng=prng,
     )
 
-    hdf5_answer_testing("events1.h5", answer_store)
+    hdf5_answer_testing("events1.h5", answer_store, answer_dir)
 
     events1 = EventList("events1.h5")
 
     events1.write_fits_file("test_events.fits", (20.0, "arcmin"), 1024, overwrite=True)
     events1.write_spectrum("test_spec.fits", 0.2, 10.0, 2000, overwrite=True)
     events1.write_fits_image("test_img.fits", (20.0, "arcmin"), 1024, overwrite=True)
 
-    file_answer_testing("EVENTS", "test_events.fits", answer_store)
-    file_answer_testing("SPECTRUM", "test_spec.fits", answer_store)
+    file_answer_testing("EVENTS", "test_events.fits", answer_store, answer_dir)
+    file_answer_testing("SPECTRUM", "test_spec.fits", answer_store, answer_dir)
 
     n_photons2, n_cells2 = make_photons(
         "photons2", sphere, redshift, A, exp_time, thermal_model
     )
     n_events2 = project_photons(
         "photons2",
         "events2",
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/test_spectra.py` & `pyxsim-4.2b0/pyxsim/tests/test_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import soxs
 from numpy.testing import assert_allclose
 
 from pyxsim.spectral_models import IGMSpectralModel, TableCIEModel
 
 
 def test_apec():
+
     amod = TableCIEModel("apec", 0.1, 10.0, 10000, 1.0, 10.0, thermal_broad=True)
     amod.prepare_spectrum(0.2)
 
     acspec, amspec, _ = amod.get_spectrum(6.0)
     spec = acspec + 0.3 * amspec
 
     agen = soxs.ApecGenerator(0.1, 10.0, 10000, broadening=True)
@@ -29,14 +30,15 @@
     assert_allclose(c + 0.3 * m, (spec2.flux * spec2.de)[eidxs].value.sum())
     assert_allclose(
         ec + 0.3 * em, (spec2.emid * spec2.flux * spec2.de)[eidxs].value.sum()
     )
 
 
 def test_igm():
+
     imod = IGMSpectralModel(0.2, 3.0, 1000)
     imod.prepare_spectrum(0.05)
 
     icspec, imspec, _ = imod.get_spectrum(1.0, 0.01)
     spec = icspec + 0.3 * imspec
 
     igen = soxs.IGMGenerator(0.2, 3.0, 1000)
```

### Comparing `pyxsim-4.2.0/pyxsim/tests/utils.py` & `pyxsim-4.2b0/pyxsim/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from numbers import Real
 
 import numpy as np
 from numpy.random import RandomState
-from soxs.utils import soxs_cfg
 from yt.loaders import load_particles, load_uniform_grid
 from yt.utilities.physical_ratios import K_per_keV, cm_per_mpc, mass_hydrogen_grams
 
-answer_dir = soxs_cfg.get("soxs", "soxs_answer_dir")
-
 # Gas parameters
 R = 1.0  # Mpc
 r_c = 0.05  # Mpc
 rho_c = 0.04 * mass_hydrogen_grams  # g/cm**3
 beta = 2.0 / 3.0
 kT = 6.0  # keV
 v_shift = 4.0e7  # cm/s
@@ -23,14 +20,15 @@
 # Dark matter parameters
 r_s = 0.350  # Mpc
 rho_s = 9.0e-26  # g/cm**3
 
 
 class BetaModelSource:
     def __init__(self):
+
         self.prng = RandomState(32)
         self.kT = kT
         self.Z = Z
         self.O = O
         self.Ca = Ca
 
         nx = 128
@@ -71,14 +69,15 @@
             bbox=bbox,
             default_species_fields="ionized",
         )
 
 
 class ParticleBetaModelSource:
     def __init__(self):
+
         self.prng = RandomState(35)
         self.kT = kT
         self.Z = Z
 
         num_particles = 1000000
 
         rr = np.linspace(0.0, R, 10000)
@@ -125,15 +124,15 @@
             data,
             length_unit=(2 * R, "Mpc"),
             bbox=bbox,
             default_species_fields="ionized",
         )
 
 
-def hdf5_answer_testing(filename, answer_store):
+def hdf5_answer_testing(filename, answer_store, answer_dir):
     import os
     import shutil
 
     import h5py
     from numpy.testing import assert_almost_equal, assert_equal
 
     oldf = os.path.join(answer_dir, filename)
```

### Comparing `pyxsim-4.2.0/pyxsim/utils.py` & `pyxsim-4.2b0/pyxsim/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,36 +84,33 @@
                 raise RuntimeError(
                     f"The values for the parameter '{k1}' in the two inputs"
                     f" are not identical ({v1} vs. {v2})!"
                 )
 
 
 def merge_files(input_files, output_file, overwrite=False, add_exposure_times=False):
-    """
+    r"""
     Helper function for merging PhotonList or EventList HDF5 files.
-
     Parameters
     ----------
     input_files : list of strings
         List of filenames that will be merged together.
     output_file : string
         Name of the merged file to be outputted.
     overwrite : boolean, default False
-        If the output file already exists, set this to True to
+        If a the output file already exists, set this to True to
         overwrite it.
     add_exposure_times : boolean, default False
         If set to True, exposure times will be added together. Otherwise,
         the exposure times of all of the files must be the same.
-
     Examples
     --------
     >>> from pyxsim import merge_files
     >>> merge_files(["events_0.h5","events_1.h5","events_3.h5"], "events.h5",
     ...             overwrite=True, add_exposure_times=True)
-
     Notes
     -----
     Currently, to merge files it is mandated that all of the parameters have the
     same values, with the exception of the exposure time parameter "exp_time". If
     add_exposure_times=False, the maximum exposure time will be used.
     """
     from collections import defaultdict
```

### Comparing `pyxsim-4.2.0/pyxsim/xray_binaries.py` & `pyxsim-4.2b0/pyxsim/xray_binaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
     vyp = []
     vzp = []
     lp = []
     rp = []
     ap = []
 
     if N_l > 0.0:
+
         F_l = np.zeros(nbins + 1)
         for i in range(1, nbins + 1):
             F_l[i] = lmxb_cdf(Lbins[i])
         F_l /= F_l[-1]
         invcdf_l = InterpolatedUnivariateSpline(F_l, logLbins)
 
         n_l = prng.poisson(lam=N_l * m / mtot)
@@ -276,14 +277,15 @@
                 vyp.append(vy)
                 vzp.append(vz)
                 lp.append(l)
                 rp.append(r)
                 ap.append(np.array([alpha_lmxb] * n))
 
     if N_h > 0.0:
+
         F_h = np.zeros(nbins + 1)
         for i in range(1, nbins + 1):
             F_h[i] = hmxb_cdf(Lbins[i])
         F_h /= F_h[-1]
         invcdf_h = InterpolatedUnivariateSpline(F_h, logLbins)
 
         n_h = prng.poisson(lam=N_h * m / mtot)
```

### Comparing `pyxsim-4.2.0/pyxsim.egg-info/SOURCES.txt` & `pyxsim-4.2b0/pyxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxsim-4.2.0/setup.py` & `pyxsim-4.2b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     install_requires=[
         "numpy",
         "astropy>=4.0",
         "h5py>=3.0",
         "scipy",
         "yt>=4.1.3",
         "unyt>=2.9.3",
-        "soxs>=4.5.1",
+        "soxs>=4.2.1",
         "tqdm",
     ],
     include_package_data=True,
     ext_modules=cython_extensions,
     classifiers=[
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
```

### Comparing `pyxsim-4.2.0/tests/ci_install.sh` & `pyxsim-4.2b0/tests/ci_install.sh`

 * *Files 16% similar despite different names*

```diff
@@ -17,22 +17,14 @@
     tar -zxf ${ANSWER_VER}.tar.gz
 
     # Set location of yt test data
     mkdir -p $HOME/.config/yt
     echo "[yt]" > $HOME/.config/yt/yt.toml
     echo "test_data_dir = \"${PWD}\"" >> $HOME/.config/yt/yt.toml
     cat $HOME/.config/yt/yt.toml
-
-    # Set location of SOXS data
-    mkdir -p $HOME/.config/soxs
-    echo "[soxs]" > $HOME/.config/soxs/soxs.cfg
-    echo "soxs_data_dir = ${GITHUB_WORKSPACE}/soxs_data" >> $HOME/.config/soxs/soxs.cfg
-    echo "soxs_answer_dir = ${GITHUB_WORKSPACE}/${ANSWER_VER}" >> $HOME/.config/soxs/soxs.cfg
-    cat $HOME/.config/soxs/soxs.cfg
-
 fi
 
 # Install dependencies using conda
 
 PYVER=`python --version`
 
 conda install --yes numpy pytest pip h5py astropy nose cython scipy yt
```

