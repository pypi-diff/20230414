# Comparing `tmp/qdyn-22.7.tar.gz` & `tmp/qdyn-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdyn-22.7.tar", last modified: Mon Aug 15 17:22:59 2022, max compression
+gzip compressed data, was "qdyn-23.4.tar", last modified: Fri Apr 14 11:37:37 2023, max compression
```

## Comparing `qdyn-22.7.tar` & `qdyn-23.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      251 2022-08-15 17:21:04.000000 qdyn-22.7/MANIFEST.in
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2174 2022-08-15 17:22:59.859297 qdyn-22.7/PKG-INFO
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     1243 2022-08-15 17:21:04.000000 qdyn-22.7/README.md
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      712 2022-08-15 17:22:59.859297 qdyn-22.7/setup.cfg
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2444 2022-08-15 17:21:04.000000 qdyn-22.7/setup.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.855297 qdyn-22.7/src/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      375 2022-08-15 17:21:04.000000 qdyn-22.7/src/conftest.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/src/qdyn/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      322 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/__init__.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    20867 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/analytical_pulse.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    33196 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/config.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    41865 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/io.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    14609 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/linalg.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     4236 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/memoize.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    38548 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/model.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2223 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/prop_gate.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    64806 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/pulse.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2585 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/shutil.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     6219 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/testing.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    26764 2022-08-15 17:21:04.000000 qdyn-22.7/src/qdyn/units.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/src/qdyn.egg-info/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2174 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/PKG-INFO
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     1188 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/SOURCES.txt
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)        1 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/dependency_links.txt
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)        1 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/not-zip-safe
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      306 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/requires.txt
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)        5 2022-08-15 17:22:59.000000 qdyn-22.7/src/qdyn.egg-info/top_level.txt
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)       13 2022-08-15 17:21:04.000000 qdyn-22.7/tests/matplotlibrc
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     9432 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_analytical_pulse.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    10462 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_config.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/test_io/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     3300 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_io/blocks.dat
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      134 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_io/single_val_matrix.dat
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     5100 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_io/v0.dat
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     8054 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_io.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     4227 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_linalg.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/test_model/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     1042 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      237 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/dissipator.config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2549 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/ensemble.config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     1899 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/ensemble_shared.config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     1092 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/oct.config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      942 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model/target.config
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    13067 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_model.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/test_prop_gate/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     3170 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_prop_gate/U_of_t.dat
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      723 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_prop_gate.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/test_pulse/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     3793 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_pulse/spectral_filter.dat
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     6223 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_pulse.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2038 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_pulse_shapes.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      262 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_qdyn.py
-drwxr-x---   0 gitlab-runner   (999) gitlab-runner   (999)        0 2022-08-15 17:22:59.859297 qdyn-22.7/tests/test_read_ascii_dump/
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)    94470 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_read_ascii_dump/para.asciidump
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)      923 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_read_ascii_dump/state.asciidump
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2060 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_read_ascii_dump.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2609 2022-08-15 17:21:04.000000 qdyn-22.7/tests/test_units.py
--rw-r-----   0 gitlab-runner   (999) gitlab-runner   (999)     2759 2022-08-15 17:21:04.000000 qdyn-22.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.495155 qdyn-23.4/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-14 11:37:03.000000 qdyn-23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-14 11:37:37.495155 qdyn-23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-14 11:37:03.000000 qdyn-23.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      712 2023-04-14 11:37:37.495155 qdyn-23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-04-14 11:37:03.000000 qdyn-23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.483155 qdyn-23.4/src/
+-rw-r--r--   0 root         (0) root         (0)      375 2023-04-14 11:37:03.000000 qdyn-23.4/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.491155 qdyn-23.4/src/qdyn/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/analytical_pulse.py
+-rw-r--r--   0 root         (0) root         (0)    33196 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/config.py
+-rw-r--r--   0 root         (0) root         (0)    41865 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/io.py
+-rw-r--r--   0 root         (0) root         (0)    14609 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/linalg.py
+-rw-r--r--   0 root         (0) root         (0)     4236 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/memoize.py
+-rw-r--r--   0 root         (0) root         (0)    39351 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/model.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/prop_gate.py
+-rw-r--r--   0 root         (0) root         (0)    64806 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/pulse.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/shutil.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/testing.py
+-rw-r--r--   0 root         (0) root         (0)    26795 2023-04-14 11:37:03.000000 qdyn-23.4/src/qdyn/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.491155 qdyn-23.4/src/qdyn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-14 11:37:37.000000 qdyn-23.4/src/qdyn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.491155 qdyn-23.4/tests/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 11:37:03.000000 qdyn-23.4/tests/matplotlibrc
+-rw-r--r--   0 root         (0) root         (0)     9432 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_analytical_pulse.py
+-rw-r--r--   0 root         (0) root         (0)    10462 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.491155 qdyn-23.4/tests/test_io/
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_io/blocks.dat
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_io/single_val_matrix.dat
+-rw-r--r--   0 root         (0) root         (0)     5100 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_io/v0.dat
+-rw-r--r--   0 root         (0) root         (0)     8054 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_linalg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.495155 qdyn-23.4/tests/test_model/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/config
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/custom_config_data.config
+-rw-r--r--   0 root         (0) root         (0)      237 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/dissipator.config
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/ensemble.config
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/ensemble_shared.config
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/oct.config
+-rw-r--r--   0 root         (0) root         (0)      942 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model/target.config
+-rw-r--r--   0 root         (0) root         (0)    14200 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.495155 qdyn-23.4/tests/test_prop_gate/
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_prop_gate/U_of_t.dat
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_prop_gate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.495155 qdyn-23.4/tests/test_pulse/
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_pulse/spectral_filter.dat
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_pulse.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_pulse_shapes.py
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_qdyn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:37:37.495155 qdyn-23.4/tests/test_read_ascii_dump/
+-rw-r--r--   0 root         (0) root         (0)    94470 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_read_ascii_dump/para.asciidump
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_read_ascii_dump/state.asciidump
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_read_ascii_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-04-14 11:37:03.000000 qdyn-23.4/tests/test_units.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-04-14 11:37:03.000000 qdyn-23.4/tox.ini
```

### Comparing `qdyn-22.7/PKG-INFO` & `qdyn-23.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,45 @@
 Metadata-Version: 2.1
 Name: qdyn
-Version: 22.7
+Version: 23.4
 Summary: Python package for interacting with the Fortran QDYN library and tools
 Home-page: https://www.qdyn-library.net
 Author: Michael Goerz
 Author-email: mail@michaelgoerz.net
 License: BSD license
+Description: # QDYN Python Package
+        
+        QDYN-pylib is a Python package `qdyn` for interacting with the [Fortran QDYN library and tools](https://www.qdyn-library.net/). Its purpose is to:
+        
+        - generate config files and input data for QDYN
+        - read data generated by QDYN routines
+        - provide tools for debugging, testing, and documenting QDYN
+        - wrap QDYN's "utility" programs like `qdyn_prop_traj` and `qdyn_optimize`
+        - provide interoperability of QDYN with other optimal control and quantum packages like [`scipy.optimize`](https://docs.scipy.org/doc/scipy/reference/optimize.html), [QuTiP](http://qutip.org) and the [Krotov Python Package](https://qucontrol.github.io/krotov).
+        
+        The package is *not* a direct wrapper around QDYN that would allow to call QDYN Fortran routines from Python.
+        
+        ## Installation
+        
+        To install the latest released version of QDYN-pylib, run this command in your terminal:
+        
+        ```
+        pip install qdyn
+        ```
+        
+        This is the preferred method to install QDYN-pylib, as it will always install the most recent stable release.
+        
+        If you are a QDYN developer, you can install the latest development version of QDYN-pylib with the following command:
+        
+        ```
+        pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@main#egg=qdyn&subdirectory=qdynpylib
+        ```
+        
 Keywords: qdyn
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
@@ -18,35 +47,7 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-
-# QDYN Python Package
-
-QDYN-pylib is a Python package `qdyn` for interacting with the [Fortran QDYN library and tools](https://www.qdyn-library.net/). Its purpose is to:
-
-- generate config files and input data for QDYN
-- read data generated by QDYN routines
-- provide tools for debugging, testing, and documenting QDYN
-- wrap QDYN's "utility" programs like `qdyn_prop_traj` and `qdyn_optimize`
-- provide interoperability of QDYN with other optimal control and quantum packages like [`scipy.optimize`](https://docs.scipy.org/doc/scipy/reference/optimize.html), [QuTiP](http://qutip.org) and the [Krotov Python Package](https://qucontrol.github.io/krotov).
-
-The package is *not* a direct wrapper around QDYN that would allow to call QDYN Fortran routines from Python.
-
-## Installation
-
-To install the latest released version of QDYN-pylib, run this command in your terminal:
-
-```
-pip install qdyn
-```
-
-This is the preferred method to install QDYN-pylib, as it will always install the most recent stable release.
-
-If you are a QDYN developer, you can install the latest development version of QDYN-pylib with the following command:
-
-```
-pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@master#egg=qdyn&subdirectory=qdynpylib
-```
```

### Comparing `qdyn-22.7/README.md` & `qdyn-23.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 ```
 
 This is the preferred method to install QDYN-pylib, as it will always install the most recent stable release.
 
 If you are a QDYN developer, you can install the latest development version of QDYN-pylib with the following command:
 
 ```
-pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@master#egg=qdyn&subdirectory=qdynpylib
+pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@main#egg=qdyn&subdirectory=qdynpylib
 ```
```

### Comparing `qdyn-22.7/setup.cfg` & `qdyn-23.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/setup.py` & `qdyn-23.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 requirements = ['numpy', 'matplotlib', 'scipy', 'sympy', 'click']
 
 # requirements for development (testing, generating docs)
 dev_requirements = [
     'better-apidoc',
     'coverage',
     'coveralls',
-    'doctr-versions-menu',
+    'docs-versions-menu',
     'flake8',
     'gitpython',
     'isort',
     'ipython',
     'pre-commit',
     'pdbpp',
     'pylint',
```

### Comparing `qdyn-22.7/src/qdyn/analytical_pulse.py` & `qdyn-23.4/src/qdyn/analytical_pulse.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/config.py` & `qdyn-23.4/src/qdyn/config.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/io.py` & `qdyn-23.4/src/qdyn/io.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/linalg.py` & `qdyn-23.4/src/qdyn/linalg.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/memoize.py` & `qdyn-23.4/src/qdyn/memoize.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/model.py` & `qdyn-23.4/src/qdyn/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,31 +62,28 @@
     """Model for a system well-described in the energy basis. That is, all
     operators are (sparse) matrices, and all states are simple vectors
 
     Attributes:
         t0 (float or qdyn.units.UnitFloat): Initial time.
         T (float or qdyn.units.UnitFloat): Final time.
         nt (int): Number of points in the time grid.
-        prop_method (str): Propagation method
-        use_mcwf: Propagate using the Monte-Carlo Wave Function (quantum
-            jump) method
         construct_mcwf_ham (bool): When using the MCWF method, the propagation
             must use an "effective" Hamiltonian that includes a non-Hermitian
             decay term. This term is constructed from the Lindblad operators.
             If ``use_mcwf=True`` and ``construct_mcwf_ham=False``, it is the
             user's responsibility to ensure that `ham` is the proper effective
             Hamiltonian. The `construct_mcwf` flag determines the presence of
             `add_to_H_jump` config file parameter for each Lindblad operator
         user_data (collections.OrderedDict): Key-value pairs that should that
             describe user-defined data. These will go in the ``user_strings``,
             ``user_reals``, ``user_logicals``, or ``user_ints`` section of the
             config file, depending on the type of the value
 
-    After instantiation, the attributes `t0`, `T`, `nt`, `prop_method`,
-    `use-mcwf`, and `construct_mcwf_ham` are all set via
+    After instantiation, the attributes `t0`, `T`, `nt`, :attr:`prop_method`,
+    :attr:`use_mcwf`, and `construct_mcwf_ham` are all set via
     :meth:`set_propagation`.  Operators and pulses are added to the system
     through :meth:`add_ham`, :meth:`add_observable`, and
     :meth:`add_lindblad_op`. States are added through :meth:`add_state`.
     Both the general OCT settings (OCT section in the QDYN config file) and
     OCT-related settings for each control pulse are controlled through
     :meth:`set_oct`. After the model has been constructed, a config file
     and all dependent data input files for the operators, pulses, and
@@ -100,22 +97,45 @@
         self._observables = []  # list of (matrix, config_attribs)
         self._dissipator = []  # list of (matrix, config_attribs)
         self._psi = OrderedDict([])  # label => amplitude array
         self._oct = OrderedDict([])  # key => val for OCT section
         self.t0 = UnitFloat(0, 'iu')
         self.T = UnitFloat(0, 'iu')
         self.nt = 0
-        self.prop_method = 'newton'
-        self.use_mcwf = False
-        self.mcwf_order = 2
+        self._prop = OrderedDict(  # key => val of PROP section
+            [
+                ('method', 'newton'),
+                ('use_mcwf', False),
+            ]
+        )
         self.construct_mcwf_ham = False
         self.user_data = OrderedDict([])
         self._pulse_id = defaultdict(int)  # last used pulse_id, per label
         self._pulse_ids = {}  # (id(pulse), label) -> pulse_id
 
+    @property
+    def prop_method(self):
+        """Propagation method (:class:`str`)."""
+        return self._prop['method']
+
+    @prop_method.setter
+    def prop_method(self, val):
+        self._prop['method'] = val
+
+    @property
+    def use_mcwf(self):
+        """Propagate using the Monte-Carlo Wave Function (quantum jump) method
+        (:class:`bool`)
+        """
+        return self._prop['use_mcwf']
+
+    @use_mcwf.setter
+    def use_mcwf(self, val):
+        self._prop['use_mcwf'] = val
+
     @staticmethod
     def _obj_list(obj_list, label=None, with_attribs=False):
         """Common implementation of methods `observables`, 'lindblad_ops`,
         `ham`"""
         if label is None:
             label = ''
         result = []
@@ -304,15 +324,15 @@
             config_attribs['label'] = label
         self._add_matrix(
             self._ham,
             H,
             label=label,
             pulse=pulse,
             check_matrix=False,
-            kwargs=config_attribs
+            kwargs=config_attribs,
         )
 
     def add_observable(
         self,
         O,
         outfile,
         exp_unit,
@@ -491,15 +511,15 @@
                 Hamiltonians may be defined in the same config file if they are
                 differentiated by label. The default label is the empty string.
             pulse: If not None, a pulse for the Dissipator to couple to
 
         All other keyword arguments set options for the dissipator in the
         config file.
         """
-        for (_, config_attribs) in self._lindblad_ops:
+        for _, config_attribs in self._lindblad_ops:
             if config_attribs.get('label', None) == label:
                 raise ValueError(
                     "Cannot set dissipator for a system label for which there "
                     "are already Lindblad operators defined"
                 )
         config_attribs = OrderedDict([])
         for key in sorted(kwargs):
@@ -522,14 +542,15 @@
         t0=0.0,
         prop_method='newton',
         use_mcwf=False,
         mcwf_order=2,
         construct_mcwf_ham=True,
         label=None,
         initial_state=None,
+        **kwargs
     ):
         """Set the time grid and other propagation-specific settings
 
         Args:
             T (float): final time
             nt (int): number of points in the time grid
             time_unit (str): physical unit of `T`, `t0`
@@ -543,14 +564,16 @@
                 Hamiltonian, based on the Lindblad operators. By passing
                 `construct_mcwf_ham=False`, this does not happen. It is the
                 user's responsibility then to ensure the Hamiltonian in the
                 model is the correct "effective" Hamiltonian for a MCWF
                 propagation.
             label (str or None): The label for `initial_state`
             initial_state (numpy.ndarray or None): Initial wave function
+            kwargs: All other keyword arguments set options for the `prop`
+                section in the config file, e.g. ``cheby_prec``
 
         Notes:
             When setting up an MCWF propagation, using the `mcwf_order=2` is
             usually the right thing to do. In some cases of strong dissipation,
             it may be numerically more efficient to use a first-order MCWF
             method, where in each time interval `dt` between two time grids
             there is at most one quantum jump, and the jumps takes place over
@@ -563,22 +586,28 @@
             self.add_state(initial_state, label)
         self.T = UnitFloat(T, time_unit)
         self.nt = nt
         self.t0 = UnitFloat(t0, time_unit)
         self.prop_method = prop_method
         if use_mcwf:
             self.use_mcwf = use_mcwf
-            self.mcwf_order = mcwf_order
+            self._prop['mcwf_order'] = mcwf_order
         if construct_mcwf_ham is None:
             construct_mcwf_ham = use_mcwf
         if use_mcwf:
             self.construct_mcwf_ham = construct_mcwf_ham
         else:
             self.construct_mcwf_ham = False
 
+        if self.use_mcwf:
+            if self._prop['mcwf_order'] not in [1, 2]:
+                raise ValueError('mcwf_order must be in [1,2]')
+        for key in sorted(kwargs):
+            self._prop[key] = kwargs[key]
+
     def set_oct(self, method, J_T_conv, max_ram_mb, **kwargs):
         """Set config file data and pulse properties for optimal control
 
         Args:
             method (str): Optimization method. Allowed values are 'krotovpk',
                 'krotov2', 'krotov2_bwr', and 'lbfgs'
             J_T_conv (float): The value of the final time functional
@@ -704,35 +733,36 @@
         """Add a state (amplitude array) for the given label. Note that there
         can only be one state per label. Thus calling `add_state` with the same
         `label` of an earlier call will replace the `state`"""
         if label is None:
             label = ''
         self._psi[label] = state
 
-    def write_to_runfolder(self, runfolder, config='config'):
+    def write_to_runfolder(
+        self, runfolder, config='config', process_config_data=None
+    ):
         """Write the model to the given runfolder. This will create a config
         file (`config`) in the runfolder, as well as all dependent data file
-        (operators, pulses)"""
+        (operators, pulses)
+
+        A `process_config_data` function may be given to filter/modify the data
+        of the config file before it is written.
+        """
         mkdir(runfolder)
         config_data = OrderedDict([])
 
         # time grid
         if self.nt > 0:
             config_data['tgrid'] = OrderedDict(
                 [('t_start', self.t0), ('t_stop', self.T), ('nt', self.nt)]
             )
 
         # propagation
-        config_data['prop'] = OrderedDict(
-            [('method', self.prop_method), ('use_mcwf', self.use_mcwf)]
-        )
-        if self.use_mcwf:
-            if self.mcwf_order not in [1, 2]:
-                raise ValueError('mcwf_order must be in [1,2]')
-            config_data['prop']['mcwf_order'] = self.mcwf_order
+        if len(self._prop) > 0:
+            config_data['prop'] = self._prop
 
         # pulses
         if len(self._pulses) > 0:
             self._write_pulses(runfolder, config_data)
 
         # Hamiltonian
         if len(self._ham) > 0:
@@ -756,14 +786,16 @@
         if len(self._oct) > 0:
             config_data['oct'] = self._oct
 
         # user-defined data
         for key, val in self.user_data.items():
             set_config_user_value(config_data, key, val)
 
+        if process_config_data is not None:
+            config_data = process_config_data(config_data)
         write_config(config_data, os.path.join(runfolder, config))
 
     def _write_pulses(self, runfolder, config_data):
         """Write numerical pulse files to runfolder, add pulse data to
         config_data,"""
         tgrid = pulse_tgrid(self.T, self.nt, self.t0)
         if 'pulse' not in config_data:
@@ -834,46 +866,42 @@
     def _write_ham(self, runfolder, config_data):
         """Write operators in the Hamiltonian to data files inside `runfolder`,
         and add ham data to `config_data`"""
         if 'ham' not in config_data:
             config_data['ham'] = []
         for op_counter, (op, attribs) in enumerate(self._ham):
             if isinstance(op, str):
-                config_attribs = OrderedDict(
-                    [('type', op)]
-                )
+                config_attribs = OrderedDict([('type', op)])
                 for key, val in attribs.items():
                     config_attribs[key] = val
                 config_data['ham'].append(config_attribs)
             else:
                 self._write_matrices(
                     runfolder,
                     config_data,
                     'ham',
                     [self._ham[op_counter]],
                     outprefix='H',
                     set_op_type=True,
                     counter0=op_counter,
-        )
+                )
 
     def _write_observables(self, runfolder, config_data):
         """Write operators describing all observables to the runfolder,
         and add observables data to `config_data`"""
         if 'observables' not in config_data:
             config_data['observables'] = []
         for op_counter, (op, attribs) in enumerate(self._observables):
             if 'filename' in attribs:
                 filename = attribs['filename']
             else:
                 filename = "O%d.dat" % (op_counter + 1)
             if isinstance(op, str):
                 assert op in ['ham', 'norm', 'pop']
-                config_attribs = OrderedDict(
-                    [('type', op)]
-                )
+                config_attribs = OrderedDict([('type', op)])
             else:  # assume that op is a matrix
                 matrix = op
                 write_indexed_matrix(
                     matrix,
                     filename=os.path.join(runfolder, filename),
                     hermitian=False,
                 )
```

### Comparing `qdyn-22.7/src/qdyn/prop_gate.py` & `qdyn-23.4/src/qdyn/prop_gate.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/pulse.py` & `qdyn-23.4/src/qdyn/pulse.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/shutil.py` & `qdyn-23.4/src/qdyn/shutil.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/testing.py` & `qdyn-23.4/src/qdyn/testing.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/src/qdyn/units.py` & `qdyn-23.4/src/qdyn/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
         ...     print(UnitFloat(1.1, 'GHz')*UnitFloat(1.1, 'GHz'))
         ... except TypeError as e:
         ...     print(e)
         Factor cannot be an instance of UnitFloat
         >>> try:
         ...     print(UnitFloat(1.1, 'GHz')*2.0j)
         ... except TypeError as e:
-        ...     print(e)
+        ...     print("can't convert complex to float")
         can't convert complex to float
         """
         if isinstance(factor, UnitFloat):
             raise TypeError("Factor cannot be an instance of UnitFloat")
         return UnitFloat(val=(float(factor) * self.val), unit=self.unit)
 
     __rmul__ = __mul__
```

### Comparing `qdyn-22.7/src/qdyn.egg-info/PKG-INFO` & `qdyn-23.4/src/qdyn.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,45 @@
 Metadata-Version: 2.1
 Name: qdyn
-Version: 22.7
+Version: 23.4
 Summary: Python package for interacting with the Fortran QDYN library and tools
 Home-page: https://www.qdyn-library.net
 Author: Michael Goerz
 Author-email: mail@michaelgoerz.net
 License: BSD license
+Description: # QDYN Python Package
+        
+        QDYN-pylib is a Python package `qdyn` for interacting with the [Fortran QDYN library and tools](https://www.qdyn-library.net/). Its purpose is to:
+        
+        - generate config files and input data for QDYN
+        - read data generated by QDYN routines
+        - provide tools for debugging, testing, and documenting QDYN
+        - wrap QDYN's "utility" programs like `qdyn_prop_traj` and `qdyn_optimize`
+        - provide interoperability of QDYN with other optimal control and quantum packages like [`scipy.optimize`](https://docs.scipy.org/doc/scipy/reference/optimize.html), [QuTiP](http://qutip.org) and the [Krotov Python Package](https://qucontrol.github.io/krotov).
+        
+        The package is *not* a direct wrapper around QDYN that would allow to call QDYN Fortran routines from Python.
+        
+        ## Installation
+        
+        To install the latest released version of QDYN-pylib, run this command in your terminal:
+        
+        ```
+        pip install qdyn
+        ```
+        
+        This is the preferred method to install QDYN-pylib, as it will always install the most recent stable release.
+        
+        If you are a QDYN developer, you can install the latest development version of QDYN-pylib with the following command:
+        
+        ```
+        pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@main#egg=qdyn&subdirectory=qdynpylib
+        ```
+        
 Keywords: qdyn
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
@@ -18,35 +47,7 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-
-# QDYN Python Package
-
-QDYN-pylib is a Python package `qdyn` for interacting with the [Fortran QDYN library and tools](https://www.qdyn-library.net/). Its purpose is to:
-
-- generate config files and input data for QDYN
-- read data generated by QDYN routines
-- provide tools for debugging, testing, and documenting QDYN
-- wrap QDYN's "utility" programs like `qdyn_prop_traj` and `qdyn_optimize`
-- provide interoperability of QDYN with other optimal control and quantum packages like [`scipy.optimize`](https://docs.scipy.org/doc/scipy/reference/optimize.html), [QuTiP](http://qutip.org) and the [Krotov Python Package](https://qucontrol.github.io/krotov).
-
-The package is *not* a direct wrapper around QDYN that would allow to call QDYN Fortran routines from Python.
-
-## Installation
-
-To install the latest released version of QDYN-pylib, run this command in your terminal:
-
-```
-pip install qdyn
-```
-
-This is the preferred method to install QDYN-pylib, as it will always install the most recent stable release.
-
-If you are a QDYN developer, you can install the latest development version of QDYN-pylib with the following command:
-
-```
-pip install git+git@gitlabph.physik.fu-berlin.de:ag-koch/qdyn.git@master#egg=qdyn&subdirectory=qdynpylib
-```
```

### Comparing `qdyn-22.7/src/qdyn.egg-info/SOURCES.txt` & `qdyn-23.4/src/qdyn.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 tests/test_qdyn.py
 tests/test_read_ascii_dump.py
 tests/test_units.py
 tests/test_io/blocks.dat
 tests/test_io/single_val_matrix.dat
 tests/test_io/v0.dat
 tests/test_model/config
+tests/test_model/custom_config_data.config
 tests/test_model/dissipator.config
 tests/test_model/ensemble.config
 tests/test_model/ensemble_shared.config
 tests/test_model/oct.config
 tests/test_model/target.config
 tests/test_prop_gate/U_of_t.dat
 tests/test_pulse/spectral_filter.dat
```

### Comparing `qdyn-22.7/tests/test_analytical_pulse.py` & `qdyn-23.4/tests/test_analytical_pulse.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_config.py` & `qdyn-23.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_io/blocks.dat` & `qdyn-23.4/tests/test_io/blocks.dat`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_io/v0.dat` & `qdyn-23.4/tests/test_io/v0.dat`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_io.py` & `qdyn-23.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_linalg.py` & `qdyn-23.4/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model/config` & `qdyn-23.4/tests/test_model/config`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model/ensemble.config` & `qdyn-23.4/tests/test_model/ensemble.config`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model/ensemble_shared.config` & `qdyn-23.4/tests/test_model/ensemble_shared.config`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model/oct.config` & `qdyn-23.4/tests/test_model/oct.config`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model/target.config` & `qdyn-23.4/tests/test_model/target.config`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_model.py` & `qdyn-23.4/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -370,14 +370,52 @@
     assert filecmp.cmp(
         os.path.join(test_dir, 'ensemble_shared.config'),
         str(tmpdir.join('model_rf', 'ensemble_shared.config')),
         shallow=False,
     )
 
 
+def test_custom_config_data(tmpdir, request, H0, H1, L1, L2, pop1, pop2):
+    """Test that we tune the config_data of the model"""
+    filename = request.module.__file__
+    test_dir, _ = os.path.splitext(filename)
+
+    psi = np.array([0, 1, 1, 0], dtype=np.complex128) / np.sqrt(2.0)
+    pulse = AnalyticalPulse.from_func(
+        partial(blackman, t_start=0, t_stop=50),
+        ampl_unit='unitless',
+        time_unit='ns',
+    )
+    model = two_level_model(H0, H1, L1, L2, pop1, pop2, pulse, psi)
+    model.set_propagation(
+        initial_state=psi,
+        T=50,
+        nt=1001,
+        time_unit='ns',
+        use_mcwf=True,
+        newton_relerr=1e-8,
+    )
+
+    def process_config_data(config_data):
+        del config_data["prop"]["use_mcwf"]
+        return config_data
+
+    model.write_to_runfolder(
+        str(tmpdir.join('model_rf')),
+        config='custom_config_data.config',
+        process_config_data=process_config_data,
+    )
+
+    assert filecmp.cmp(
+        os.path.join(test_dir, 'custom_config_data.config'),
+        str(tmpdir.join('model_rf', 'custom_config_data.config')),
+        shallow=False,
+    )
+
+
 def complex_pulse_error_data():
     """Generate data for parametrization of test_complex_pulse_error"""
     # real pulse:
     pulse1 = AnalyticalPulse.from_func(partial(blackman, t_start=0, t_stop=50))
     # complex pulse:
     pulse2 = AnalyticalPulse.from_func(lambda t: complex(pulse1.as_func()(t)))
     H1 = np.array(
```

### Comparing `qdyn-22.7/tests/test_prop_gate/U_of_t.dat` & `qdyn-23.4/tests/test_prop_gate/U_of_t.dat`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_prop_gate.py` & `qdyn-23.4/tests/test_prop_gate.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_pulse/spectral_filter.dat` & `qdyn-23.4/tests/test_pulse/spectral_filter.dat`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_pulse.py` & `qdyn-23.4/tests/test_pulse.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_pulse_shapes.py` & `qdyn-23.4/tests/test_pulse_shapes.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_read_ascii_dump/para.asciidump` & `qdyn-23.4/tests/test_read_ascii_dump/para.asciidump`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_read_ascii_dump/state.asciidump` & `qdyn-23.4/tests/test_read_ascii_dump/state.asciidump`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_read_ascii_dump.py` & `qdyn-23.4/tests/test_read_ascii_dump.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tests/test_units.py` & `qdyn-23.4/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `qdyn-22.7/tox.ini` & `qdyn-23.4/tox.ini`

 * *Files identical despite different names*

