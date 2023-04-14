# Comparing `tmp/flavio-2.4.0.tar.gz` & `tmp/flavio-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavio-2.4.0.tar", last modified: Tue Jan 24 14:02:19 2023, max compression
+gzip compressed data, was "flavio-2.5.0.tar", last modified: Fri Apr 14 14:39:12 2023, max compression
```

## Comparing `flavio-2.4.0.tar` & `flavio-2.5.0.tar`

### file list

```diff
@@ -1,358 +1,377 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-24 13:57:40.000000 flavio-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 13:57:40.000000 flavio-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-01-24 14:02:19.042204 flavio-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-24 13:57:40.000000 flavio-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.010203 flavio-2.4.0/flavio/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.010203 flavio-2.4.0/flavio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/citations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)   694862 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/measurements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27032 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/parameters_correlated.yml
--rw-r--r--   0 runner    (1001) docker     (123)    82861 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/parameters_metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/parameters_uncorrelated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.010203 flavio-2.4.0/flavio/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/2009.09313_digitized.npz
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/SPheno-2.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/SPheno.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/data/test/wcxf-flavio-example.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.014203 flavio-2.4.0/flavio/io/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/io/instanceio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/io/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.014203 flavio-2.4.0/flavio/math/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/math/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.014203 flavio-2.4.0/flavio/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.018203 flavio-2.4.0/flavio/physics/bdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/angular.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bll.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bpll_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/bvll/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/nonfactorizable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/observables_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/test_bvll.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/test_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/test_qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bxll_qed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_gamma/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/btop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/test_btop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/clnexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/test_btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/hqet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.022203 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/formfactors/test_cln.py
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/lambdablambdagamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/lambdablambdall_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bll.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bvgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/test_wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/bdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.026203 flavio-2.4.0/flavio/physics/betadecays/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/betadecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/betadecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/betadecays/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/betadecays/test_betadecays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.006202 flavio-2.4.0/flavio/physics/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.026203 flavio-2.4.0/flavio/physics/data/arXiv-0810-4077v3/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-0810-4077v3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.026203 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/README
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/
--rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/
--rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/qcdf_interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)   109606 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.030203 flavio-2.4.0/flavio/physics/data/wcsm/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.034204 flavio-2.4.0/flavio/physics/ddecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.034204 flavio-2.4.0/flavio/physics/ddecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/formfactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/formfactors/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/formfactors/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/formfactors/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/rge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/test_dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/ddecays/test_dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.034204 flavio-2.4.0/flavio/physics/edms/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/slcouplings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/test_neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/edms/test_paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/eft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.034204 flavio-2.4.0/flavio/physics/higgs/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/signalstrength.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/test_higgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/higgs/width.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.034204 flavio-2.4.0/flavio/physics/kdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/test_lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/kdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/mdms/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mdms/al.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mdms/test_al.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/mesonmixing/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/test_mesonmixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mesonmixing/wilsoncoefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/mudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/muegamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/test_mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/test_mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/mudecays/test_muegamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/neutrinos/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/neutrinos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/neutrinos/test_trident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/neutrinos/trident.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/running/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/running/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/running/betafunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/running/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/running/running.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/running/test_running.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.038204 flavio-2.4.0/flavio/physics/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/scattering/ee_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/scattering/test_ee_ww.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/flavio/physics/taudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/taudecays/test_tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/test_ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/test_eft.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/flavio/physics/wdecays/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/wdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/wdecays/gammaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/wdecays/mw.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/wdecays/test_mW.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/wdecays/test_wdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/flavio/physics/zdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/afbz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/gammaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/gammazsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/test_smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/physics/zdecays/test_zdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/flavio/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/plots/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/plots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/plots/plotfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/plots/test_plotfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.042204 flavio-2.4.0/flavio/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    79896 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    35892 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/statistics/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/test_parseerrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-01-24 13:57:40.000000 flavio-2.4.0/flavio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:02:19.010203 flavio-2.4.0/flavio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-01-24 14:02:18.000000 flavio-2.4.0/flavio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-01-24 14:02:18.000000 flavio-2.4.0/flavio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 14:02:18.000000 flavio-2.4.0/flavio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-24 14:02:18.000000 flavio-2.4.0/flavio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-24 14:02:18.000000 flavio-2.4.0/flavio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 14:02:19.042204 flavio-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-24 13:57:40.000000 flavio-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.971613 flavio-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-14 14:32:49.000000 flavio-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:32:49.000000 flavio-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-14 14:39:12.967613 flavio-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 14:32:49.000000 flavio-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.923613 flavio-2.5.0/flavio/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.923613 flavio-2.5.0/flavio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/citations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   982184 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/measurements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26756 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/parameters_correlated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    86949 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/parameters_metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/parameters_uncorrelated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.927613 flavio-2.5.0/flavio/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/2009.09313_digitized.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/SPheno-2.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/SPheno.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/data/test/wcxf-flavio-example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.927613 flavio-2.5.0/flavio/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/io/instanceio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/io/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.927613 flavio-2.5.0/flavio/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/math/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.927613 flavio-2.5.0/flavio/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.935613 flavio-2.5.0/flavio/physics/bdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bpll_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.935613 flavio-2.5.0/flavio/physics/bdecays/bvll/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/nonfactorizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/observables_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/test_bvll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/test_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/test_qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bxll_qed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.939613 flavio-2.5.0/flavio/physics/bdecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.939613 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.939613 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/btop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/test_btop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.939613 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/clnexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/test_btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/hqet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.943613 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.943613 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/formfactors/test_cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/lambdablambdagamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/lambdablambdall_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bvgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/test_wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/bdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.943613 flavio-2.5.0/flavio/physics/betadecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/betadecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/betadecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/betadecays/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/betadecays/test_betadecays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.915613 flavio-2.5.0/flavio/physics/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.943613 flavio-2.5.0/flavio/physics/data/arXiv-0810-4077v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-0810-4077v3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.947613 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.947613 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/data/qcdf_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/data/wcsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.951613 flavio-2.5.0/flavio/physics/ddecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.955613 flavio-2.5.0/flavio/physics/ddecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/formfactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/formfactors/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/formfactors/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/formfactors/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/rge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/test_dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/ddecays/test_dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.955613 flavio-2.5.0/flavio/physics/dileptons/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/partondist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/pplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/test_ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/dileptons/test_pplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.955613 flavio-2.5.0/flavio/physics/edms/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/slcouplings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/test_neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/edms/test_paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.955613 flavio-2.5.0/flavio/physics/higgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/signalstrength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/test_higgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/higgs/width.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.959613 flavio-2.5.0/flavio/physics/kdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/test_lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/kdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.959613 flavio-2.5.0/flavio/physics/mdms/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mdms/al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mdms/test_al.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.959613 flavio-2.5.0/flavio/physics/mesonmixing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/test_mesonmixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mesonmixing/wilsoncoefficient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.959613 flavio-2.5.0/flavio/physics/mudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/muegamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/test_mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/test_mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/mudecays/test_muegamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.963613 flavio-2.5.0/flavio/physics/neutrinos/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/neutrinos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/neutrinos/test_trident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/neutrinos/trident.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.963613 flavio-2.5.0/flavio/physics/quarkonium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/Vllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/test_Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/test_Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/test_Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/quarkonium/test_Vllgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.963613 flavio-2.5.0/flavio/physics/running/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/running/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/running/betafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/running/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/running/running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/running/test_running.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.963613 flavio-2.5.0/flavio/physics/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/scattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/scattering/ee_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/scattering/test_ee_ww.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.967613 flavio-2.5.0/flavio/physics/taudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/taudecays/test_tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/test_ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/test_eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.967613 flavio-2.5.0/flavio/physics/wdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/wdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/wdecays/gammaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/wdecays/mw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/wdecays/test_mW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/wdecays/test_wdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.967613 flavio-2.5.0/flavio/physics/zdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/afbz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/gammaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/gammazsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/test_smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/physics/zdecays/test_zdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.967613 flavio-2.5.0/flavio/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/plots/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/plots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/plots/plotfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/plots/test_plotfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.967613 flavio-2.5.0/flavio/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/statistics/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/test_parseerrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-14 14:32:49.000000 flavio-2.5.0/flavio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:39:12.923613 flavio-2.5.0/flavio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-14 14:39:12.000000 flavio-2.5.0/flavio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-14 14:39:12.000000 flavio-2.5.0/flavio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:39:12.000000 flavio-2.5.0/flavio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 14:39:12.000000 flavio-2.5.0/flavio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 14:39:12.000000 flavio-2.5.0/flavio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:39:12.971613 flavio-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 14:32:49.000000 flavio-2.5.0/setup.py
```

### Comparing `flavio-2.4.0/LICENSE.txt` & `flavio-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/PKG-INFO` & `flavio-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.4.0
+Version: 2.5.0
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -68,14 +68,16 @@
 - Christoph Langenbruch
 - Christoph Niehoff
 - Markus Prim
 - Albert Puig
 - Méril Reboud
 - Stefanie Reichert
 - Niladri Sahoo
+- Jakub Šalko
+- Michael Schmidt
 - Aleks Smolkovič
 - Peter Stangl
 - Olcyr Sumensari
 - Felicia Volle
 - Zeren Simon Wang
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.4.0 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.0 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
@@ -21,17 +21,18 @@
 [Github's issue system](https://github.com/flav-io/flavio/issues) rather than
 by E-mail. Thanks! ## Contributors Maintainer: - Peter Stangl (@peterstangl)
 Original author: - David M. Straub (@DavidMStraub) Contributors (in
 alphabetical order): - Jason Aebischer - Jorge Alda Gallo - Frederik Beaujean -
 Adam Falkowski - Tobias Felkl - Ece GÃ¼rler - MatÄj Hudec - Matthew Kirk -
 Jonathan Kriewald - Jacky Kumar - Christoph Langenbruch - Christoph Niehoff -
 Markus Prim - Albert Puig - MÃ©ril Reboud - Stefanie Reichert - Niladri Sahoo -
-Aleks SmolkoviÄ - Peter Stangl - Olcyr Sumensari - Felicia Volle - Zeren Simon
-Wang ## License flavio is released under the MIT license. ## Citation If you
-use flavio in a scientific publication, please cite: > D. Straub, "flavio: a
-Python package for flavour and precision phenomenology in the Standard Model
-and beyond", [arXiv:1810.08132](https://arxiv.org/abs/1810.08132) This paper
-contains many references to results in the literature that went into the code.
-Please also consider citing the relevant original literature, where the real
-work was done. The flavio repository itself is also citable via a DOI provided
-by Zenodo: [![DOI](https://zenodo.org/badge/22356/flav-io/flavio.svg)](https://
-zenodo.org/badge/latestdoi/22356/flav-io/flavio)
+Jakub Å alko - Michael Schmidt - Aleks SmolkoviÄ - Peter Stangl - Olcyr
+Sumensari - Felicia Volle - Zeren Simon Wang ## License flavio is released
+under the MIT license. ## Citation If you use flavio in a scientific
+publication, please cite: > D. Straub, "flavio: a Python package for flavour
+and precision phenomenology in the Standard Model and beyond", [arXiv:
+1810.08132](https://arxiv.org/abs/1810.08132) This paper contains many
+references to results in the literature that went into the code. Please also
+consider citing the relevant original literature, where the real work was done.
+The flavio repository itself is also citable via a DOI provided by Zenodo: [!
+[DOI](https://zenodo.org/badge/22356/flav-io/flavio.svg)](https://zenodo.org/
+badge/latestdoi/22356/flav-io/flavio)
```

### Comparing `flavio-2.4.0/README.md` & `flavio-2.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 - Christoph Langenbruch
 - Christoph Niehoff
 - Markus Prim
 - Albert Puig
 - Méril Reboud
 - Stefanie Reichert
 - Niladri Sahoo
+- Jakub Šalko
+- Michael Schmidt
 - Aleks Smolkovič
 - Peter Stangl
 - Olcyr Sumensari
 - Felicia Volle
 - Zeren Simon Wang
 
 ## License
```

#### html2text {}

```diff
@@ -15,18 +15,18 @@
 questions, bugs and feature request using [Github's issue system](https://
 github.com/flav-io/flavio/issues) rather than by E-mail. Thanks! ##
 Contributors Maintainer: - Peter Stangl (@peterstangl) Original author: - David
 M. Straub (@DavidMStraub) Contributors (in alphabetical order): - Jason
 Aebischer - Jorge Alda Gallo - Frederik Beaujean - Adam Falkowski - Tobias
 Felkl - Ece GÃ¼rler - MatÄj Hudec - Matthew Kirk - Jonathan Kriewald - Jacky
 Kumar - Christoph Langenbruch - Christoph Niehoff - Markus Prim - Albert Puig -
-MÃ©ril Reboud - Stefanie Reichert - Niladri Sahoo - Aleks SmolkoviÄ - Peter
-Stangl - Olcyr Sumensari - Felicia Volle - Zeren Simon Wang ## License flavio
-is released under the MIT license. ## Citation If you use flavio in a
-scientific publication, please cite: > D. Straub, "flavio: a Python package for
-flavour and precision phenomenology in the Standard Model and beyond", [arXiv:
-1810.08132](https://arxiv.org/abs/1810.08132) This paper contains many
-references to results in the literature that went into the code. Please also
-consider citing the relevant original literature, where the real work was done.
-The flavio repository itself is also citable via a DOI provided by Zenodo: [!
-[DOI](https://zenodo.org/badge/22356/flav-io/flavio.svg)](https://zenodo.org/
-badge/latestdoi/22356/flav-io/flavio)
+MÃ©ril Reboud - Stefanie Reichert - Niladri Sahoo - Jakub Å alko - Michael
+Schmidt - Aleks SmolkoviÄ - Peter Stangl - Olcyr Sumensari - Felicia Volle -
+Zeren Simon Wang ## License flavio is released under the MIT license. ##
+Citation If you use flavio in a scientific publication, please cite: > D.
+Straub, "flavio: a Python package for flavour and precision phenomenology in
+the Standard Model and beyond", [arXiv:1810.08132](https://arxiv.org/abs/
+1810.08132) This paper contains many references to results in the literature
+that went into the code. Please also consider citing the relevant original
+literature, where the real work was done. The flavio repository itself is also
+citable via a DOI provided by Zenodo: [![DOI](https://zenodo.org/badge/22356/
+flav-io/flavio.svg)](https://zenodo.org/badge/latestdoi/22356/flav-io/flavio)
```

### Comparing `flavio-2.4.0/flavio/__init__.py` & `flavio-2.5.0/flavio/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/_parse_errors.py` & `flavio-2.5.0/flavio/_parse_errors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/citations.py` & `flavio-2.5.0/flavio/citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/classes.py` & `flavio-2.5.0/flavio/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,14 +502,15 @@
 
         # Read default parameters for B->V form factors
         flavio.physics.bdecays.formfactors.b_v.bsz_parameters.bsz_load('v2', 'LCSR', ('B->omega', 'B->rho'), self)
         flavio.physics.bdecays.formfactors.b_v.bsz_parameters.bsz_load('v2', 'LCSR-Lattice', ('B->K*', 'Bs->phi', 'Bs->K*'), self)
 
         # Read default parameters for B->P form factors
         flavio.physics.bdecays.formfactors.b_p.bsz_parameters.gkvd_load('v1', 'LCSR-Lattice', ('B->K', 'B->pi'), self)
+        flavio.physics.bdecays.formfactors.b_p.bcl_parameters_lmvd.load_parameters('data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml', self)
 
         # Read default parameters for Lambdab->Lambda form factors
         flavio.physics.bdecays.formfactors.lambdab_12.lattice_parameters.lattice_load_ho(self)
 
 
 class WilsonCoefficientPriors(Constraints):
     """
```

### Comparing `flavio-2.4.0/flavio/data/citations.yml` & `flavio-2.5.0/flavio/data/citations.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - Boer:2014kda
 - Bourrely:2008za
 - Brignole:2004ah
 - Brivio:2017vri
 - Brod:2010hi
 - Buras:2006gb
 - Buras:2015yba
+- Calibbi:2022ddo
 - Caprini:1997mu
 - Chobanova:2017rkj
 - Cirigliano:2007ga
 - Descotes-Genon:2015hea
 - Descotes-Genon:2019dbw
 - Falkowski:2019hvp
 - Freitas:2014hra
@@ -30,14 +31,15 @@
 - Gubernari:2018wyi
 - Huber:2015sra
 - Inami:1980fz
 - Kitano:2002mt
 - Kozachuk:2017mdk
 - Kruger:2002gf
 - Kuno:1999jp
+- Leljak:2021vte
 - Meinel:2020owd
 - Melikhov:2004mk
 - Misiak:2006ab
 - Misiak:2015xwa
 - Mott:2011cx
 - Pich:2013lsa
 - Seidel:2004jh
```

### Comparing `flavio-2.4.0/flavio/data/config.yml` & `flavio-2.5.0/flavio/data/config.yml`

 * *Files 15% similar despite different names*

```diff
@@ -64,14 +64,28 @@
 
     # EDMs
     nEDM: 2.  # neutron EDM
 
     # beta decays
     betadecay: 1.
 
+    # quarkonium
+    # renormalization scales are set to the mass of the bb quarkonia and to 2 GeV for the cc quarkonia. The renormalization scale was explicitly specified for J/psi tensor form factor in 2008.02024.
+    J/psi: 2.
+    psi(2S): 2.
+    eta_c(1S): 2.  
+    chi_c0(1P): 2.  
+    
+    Upsilon(1S): 10.
+    Upsilon(2S): 10.
+    Upsilon(3S): 10.
+    eta_b(1S): 10.
+    chi_b0(1P): 10.
+    chi_b0(2P): 10.
+
 # these are the thresholds where quark flavours are decoupled in the RG
 # evolution to low energies.
 RGE thresholds:
   mt: 173.21
   mb: 4.18
   mc: 1.275
 
@@ -88,19 +102,19 @@
   Bs->K* form factor: Bs->K* BSZ3
   Bs->phi form factor: Bs->phi BSZ3
   B->D* form factor: B->D* CLN
 
   # B->P form factors
   B->K form factor: B->K BSZ3
   B->D form factor: B->D CLN
-  B->pi form factor: B->pi BSZ3
+  B->pi form factor: B->pi BCL4-LMVD
 
   # B->gamma form factor
   B->gamma form factor: B->gamma KM
-  
+
   # D->P form factors
   D->K form factor: D->K BSZ3
   D->pi form factor: D->pi BSZ3
 
   # Lambdab form factors
   Lambdab->Lambda form factor: Lambdab->Lambda SSE3
   Lambdab->Lambda(1520) form factor: Lambdab->Lambda(1520) LatticeQCD
@@ -108,14 +122,15 @@
   # Kaon form factors
   K->pi form factor: K->pi dispersive + pole
 
   # B->Vll non-factorizable spectator scattering corrections
   B0->K*0ll spectator scattering: B0->K*0ll QCDF interpolated
   B+->K*+ll spectator scattering: B+->K*+ll QCDF interpolated
   Bs->phill spectator scattering: Bs->phill QCDF interpolated
+  Bs->K*0ll spectator scattering: Bs->K*0ll QCDF interpolated
 
   # B->Vll subleading hadronic effects
   B0->K*0ll subleading effects at low q2: B0->K*0ll deltaC7, 7p polynomial
   B+->K*+ll subleading effects at low q2: B+->K*+ll deltaC7, 7p polynomial
   Bs->phill subleading effects at low q2: Bs->phill deltaC7, 7p polynomial
   B0->K*0ll subleading effects at high q2: B0->K*0ll deltaC9 shift
   B+->K*+ll subleading effects at high q2: B+->K*+ll deltaC9 shift
@@ -126,7 +141,13 @@
   B+->K+ll subleading effects at low q2: B+->K+ll deltaC9 polynomial
   B0->K0ll subleading effects at high q2: B0->K0ll deltaC9 shift
   B+->K+ll subleading effects at high q2: B+->K+ll deltaC9 shift
 
   # Lambdab->Lambdall subleading hadronic effects
   Lambdab->Lambdall subleading effects at low q2: Lambdab->Lambdall deltaC7 polynomial
   Lambdab->Lambdall subleading effects at high q2: Lambdab->Lambdall deltaC9 shift
+
+# set the PDF set used for different processes (at the moment only dileptons)
+PDF set:
+  dileptons:
+    name: NNPDF40_nnlo_as_01180
+    members par: PDFmembers avg=0 replicas=1-100
```

### Comparing `flavio-2.4.0/flavio/data/measurements.yml` & `flavio-2.5.0/flavio/data/measurements.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1043,15 +1043,15 @@
                 [1.00, 0.02, -0.01],
                 [1.00, 0.28],
                 [1.00]]
 
 
 LHCb B+->K*mumu 2020 S 0.1-0.98:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 0.1
       q2max: 0.98
       value: 0.34 +0.10-0.10 ± 0.06
     - name: <S3>(B+->K*mumu)
       q2min: 0.1
@@ -1088,15 +1088,15 @@
                [1.00, 0.19, -0.27, -0.06],
                [1.00, -0.35, 0.22],
                [1.00, -0.08],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 1.1-2.5:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 1.1
       q2max: 2.5
       value: 0.54 +0.21-0.18 ± 0.06
     - name: <S3>(B+->K*mumu)
       q2min: 1.1
@@ -1133,15 +1133,15 @@
                [1.00, 0.20, 0.11, 0.12],
                [1.00, 0.06, 0.16],
                [1.00, 0.22],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 2.5-4:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 2.5
       q2max: 4
       value: 0.17 +0.23-0.32 ± 0.06
     - name: <S3>(B+->K*mumu)
       q2min: 2.5
@@ -1178,15 +1178,15 @@
                [1.00, 0.05, 0.06, -0.16],
                [1.00, 0.26, -0.14],
                [1.00, -0.09],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 4-6:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 4
       q2max: 6
       value: 0.67 +0.12-0.14 ± 0.02
     - name: <S3>(B+->K*mumu)
       q2min: 4
@@ -1223,15 +1223,15 @@
                [1.00, -0.04, -0.03, -0.01],
                [1.00, 0.09, 0.09],
                [1.00, -0.08],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 6-8:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 6
       q2max: 8
       value: 0.39 +0.20-0.21 ± 0.01
     - name: <S3>(B+->K*mumu)
       q2min: 6
@@ -1268,15 +1268,15 @@
                [1.00, -0.05, -0.19, -0.13],
                [1.00, -0.10, -0.06],
                [1.00, 0.04],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 11-12.5:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 11
       q2max: 12.5
       value: 0.39 +0.24-0.17 ± 0.02
     - name: <S3>(B+->K*mumu)
       q2min: 11
@@ -1313,15 +1313,15 @@
                [1.00, 0.10, 0.11, 0.15],
                [1.00, 0.05, -0.07],
                [1.00, -0.07],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 15-17:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 15
       q2max: 17
       value: 0.41 +0.21-0.14 ± 0.02
     - name: <S3>(B+->K*mumu)
       q2min: 15
@@ -1358,15 +1358,15 @@
                [1.00, 0.07, -0.02, 0.16],
                [1.00, 0.23, 0.02],
                [1.00, 0.00],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 17-19:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 17
       q2max: 19
       value: 0.34 +0.12-0.11 ± 0.03
     - name: <S3>(B+->K*mumu)
       q2min: 17
@@ -1403,15 +1403,15 @@
                [1.00, 0.17, 0.01, -0.07],
                [1.00, -0.17, 0.10],
                [1.00, -0.19],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 1.1-6:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 1.1
       q2max: 6
       value: 0.59 +0.09-0.09 ± 0.03
     - name: <S3>(B+->K*mumu)
       q2min: 1.1
@@ -1448,15 +1448,15 @@
                [1.00, -0.05, 0.04, 0.05],
                [1.00, 0.17, -0.02],
                [1.00, -0.01],
                [1.00]]
 
 LHCb B+->K*mumu 2020 S 15-19:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 15
       q2max: 19
       value: 0.40 +0.13-0.11 ± 0.03
     - name: <S3>(B+->K*mumu)
       q2min: 15
@@ -1493,15 +1493,15 @@
                [1.00, -0.10, -0.03, 0.10],
                [1.00, 0.15, -0.01],
                [1.00, -0.09],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 0.1-0.98:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 0.1
       q2max: 0.98
       value: 0.34 +0.10-0.10 ± 0.06
     - name: <P1>(B+->K*mumu)
       q2min: 0.1
@@ -1538,15 +1538,15 @@
                [1.00, -0.22, -0.23, 0.15],
                [1.00, 0.18, -0.18],
                [1.00, -0.25],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 1.1-2.5:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 1.1
       q2max: 2.5
       value: 0.54 +0.18-0.19 ± 0.03
     - name: <P1>(B+->K*mumu)
       q2min: 1.1
@@ -1583,15 +1583,15 @@
                [1.00, 0.03, -0.01, 0.22],
                [1.00, 0.09, -0.08],
                [1.00, -0.01],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 2.5-4:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 2.5
       q2max: 4
       value: 0.17 +0.24-0.14 ± 0.04
     - name: <P1>(B+->K*mumu)
       q2min: 2.5
@@ -1628,15 +1628,15 @@
                [1.00, 0.07, 0.06, 0.08],
                [1.00, -0.02, -0.09],
                [1.00, 0.21],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 4-6:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 4
       q2max: 6
       value: 0.67 +0.11-0.14 ± 0.03
     - name: <P1>(B+->K*mumu)
       q2min: 4
@@ -1673,15 +1673,15 @@
                [1.00, -0.11, -0.01, -0.10],
                [1.00, -0.04, 0.07],
                [1.00, 0.05],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 6-8:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 6
       q2max: 8
       value: 0.39 +0.20-0.21 ± 0.02
     - name: <P1>(B+->K*mumu)
       q2min: 6
@@ -1718,15 +1718,15 @@
                [1.00, 0.25, -0.03, -0.01],
                [1.00, -0.08, -0.06],
                [1.00, -0.05],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 11-12.5:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 11
       q2max: 12.5
       value: 0.39 +0.23-0.16 ± 0.03
     - name: <P1>(B+->K*mumu)
       q2min: 11
@@ -1763,15 +1763,15 @@
                [1.00, 0.04, -0.03, -0.10],
                [1.00, 0.05, -0.01],
                [1.00, 0.06],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 15-17:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 15
       q2max: 17
       value: 0.41 +0.18-0.14 ± 0.02
     - name: <P1>(B+->K*mumu)
       q2min: 15
@@ -1808,15 +1808,15 @@
                [1.00, 0.27, 0.09, 0.05],
                [1.00, 0.09, -0.07],
                [1.00, 0.21],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 17-19:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 17
       q2max: 19
       value: 0.34 +0.11-0.12 ± 0.04
     - name: <P1>(B+->K*mumu)
       q2min: 17
@@ -1853,15 +1853,15 @@
                [1.00, -0.08, -0.03, 0.05],
                [1.00, 0.00, 0.08],
                [1.00, -0.12],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 1.1-6:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 1.1
       q2max: 6
       value: 0.59 +0.10-0.10 ± 0.03
     - name: <P1>(B+->K*mumu)
       q2min: 1.1
@@ -1898,15 +1898,15 @@
                [1.00, -0.03, -0.02, 0.18],
                [1.00, 0.14, 0.04],
                [1.00, 0.17],
                [1.00]]
 
 LHCb B+->K*mumu 2020 P 15-19:
   experiment: LHCb (9 fb-1)
-  inspire:
+  inspire: LHCb:2020gog
   values:
     - name: <FL>(B+->K*mumu)
       q2min: 15
       q2max: 19
       value: 0.40 +0.13-0.11 ± 0.02
     - name: <P1>(B+->K*mumu)
       q2min: 15
@@ -2425,14 +2425,120 @@
       value: 0.37 + 0.06 - 0.05
     - name: <AFB>(B0->K*mumu)
       q2min: 16
       q2max: 19
       value: 0.39 ± 0.04
 
 
+CMS B->K*mumu 2017 1-2:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 1
+      q2max: 2
+      value: 0.12 + 0.46 -0.47 ± 0.10
+    - name: <P5p>(B0->K*mumu)
+      q2min: 1
+      q2max: 2
+      value: 0.10 + 0.32 -0.31 ± 0.07
+  correlation: [[ 1.    ,-0.0526],
+                [-0.0526, 1.    ]]
+
+CMS B->K*mumu 2017 2-4.3:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 2
+      q2max: 4.3
+      value: -0.69 + 0.58 -0.27 ± 0.23
+    - name: <P5p>(B0->K*mumu)
+      q2min: 2
+      q2max: 4.3
+      value: -0.57 + 0.34 -0.31 ± 0.18
+  correlation: [[ 1.    ,-0.0452],
+                [-0.0452, 1.    ]]
+
+CMS B->K*mumu 2017 4.3-6:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 4.3
+      q2max: 6
+      value: 0.53 + 0.24 -0.33 ± 0.19
+    - name: <P5p>(B0->K*mumu)
+      q2min: 4.3
+      q2max: 6
+      value: -0.96 + 0.22 -0.21 ± 0.25
+  correlation: [[ 1.    , 0.4715],
+                [ 0.4715, 1.    ]]
+
+CMS B->K*mumu 2017 6-8.68:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 6
+      q2max: 8.68
+      value: -0.47 + 0.27 -0.23 ± 0.15
+    - name: <P5p>(B0->K*mumu)
+      q2min: 6
+      q2max: 8.68
+      value: -0.64 + 0.15 -0.19 ± 0.13
+  correlation: [[ 1.    , 0.0761],
+                [ 0.0761, 1.    ]]
+
+CMS B->K*mumu 2017 10.09-12.86:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 10.09
+      q2max: 12.86
+      value: -0.53 + 0.20 -0.14 ± 0.15
+    - name: <P5p>(B0->K*mumu)
+      q2min: 10.09
+      q2max: 12.86
+      value: -0.69 + 0.11 -0.14 ± 0.13
+  correlation: [[ 1.    , 0.6077],
+                [ 0.6077, 1.    ]]
+
+CMS B->K*mumu 2017 14.18-16:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 14.18
+      q2max: 16
+      value: -0.33 + 0.24 -0.23 ± 0.20
+    - name: <P5p>(B0->K*mumu)
+      q2min: 14.18
+      q2max: 16
+      value: -0.66 + 0.13 -0.20 ± 0.18
+  correlation: [[ 1.    , 0.4188],
+                [ 0.4188, 1.    ]]
+
+CMS B->K*mumu 2017 16-19:
+  experiment: CMS
+  insipre: CMS:2017rzx
+  values:
+    - name: <P1>(B0->K*mumu)
+      q2min: 16
+      q2max: 19
+      value: -0.53 + 0.19 -0.19 ± 0.16
+    - name: <P5p>(B0->K*mumu)
+      q2min: 16
+      q2max: 19
+      value: -0.56 + 0.12 -0.12 ± 0.07
+  correlation: [[ 1.    , 0.4621],
+                [ 0.4621, 1.    ]]
+
+
 CMS B->K*mumu 2017 P1:
   experiment: CMS
   inspire: CMS:2017ivg
   values:
     - name: <P1>(B0->K*mumu)
       q2min: 1
       q2max: 2
@@ -5109,190 +5215,190 @@
 
 Belle B->hnunu SL 2017:
   experiment: Belle
   inspire: Grygier:2017tzo
   values:
     # Tables I and II
     # counts_total is the square of the statistical error on the signal yield
-    # background_variance is the systematic error on the signal yield
+    # background_std is the systematic error on the signal yield
     BR(B+->Knunu):
       distribution: general_gamma_upper_limit
       limit: 1.9e-5
       confidence_level: 0.9
       counts_total: 83
       counts_signal: 17.7
-      background_variance: 3.4
+      background_std: 3.4
     BR(B0->Knunu):
       distribution: general_gamma_upper_limit
       limit: 2.6e-5
       confidence_level: 0.9
       counts_total: 18
       counts_signal: 0.6
-      background_variance: 1.4
+      background_std: 1.4
     BR(B+->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 6.1e-5
       confidence_level: 0.9
       counts_total: 55
       counts_signal: 16.2
-      background_variance: 1.8
+      background_std: 1.8
     BR(B0->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 1.8e-5
       confidence_level: 0.9
       counts_total: 13
       counts_signal: -2.0
-      background_variance: 1.8
+      background_std: 1.8
     BR(B+->pinunu):
       distribution: general_gamma_upper_limit
       limit: 1.4e-5
       confidence_level: 0.9
       counts_total: 228
       counts_signal: 5.6
-      background_variance: 5.9
+      background_std: 5.9
     BR(B0->pinunu):
       distribution: general_gamma_upper_limit
       limit: 0.9e-5
       confidence_level: 0.9
       counts_total: 31
       counts_signal: 0.2
-      background_variance: 1.6
+      background_std: 1.6
     BR(B+->rhonunu):
       distribution: general_gamma_upper_limit
       limit: 3.0e-5
       confidence_level: 0.9
       counts_total: 151
       counts_signal: 6.2
-      background_variance: 2.4
+      background_std: 2.4
     BR(B0->rhonunu):
       distribution: general_gamma_upper_limit
       limit: 4.0e-5
       confidence_level: 0.9
       counts_total: 81
       counts_signal: 11.9
-      background_variance: 3.6
+      background_std: 3.6
 
 Belle B->hnunu had 2013:
   experiment: Belle
   inspire: Lutz:2013ftz
   values:
     # Table I
-    # background_variance is the systematic error on the # of signal events
+    # background_std is the systematic error on the # of signal events
     BR(B+->Knunu):
       distribution: general_gamma_upper_limit
       limit: 5.5e-5
       confidence_level: 0.9
       counts_total: 43
       counts_signal: 13.3
-      background_variance: 2.3
+      background_std: 2.3
     BR(B0->Knunu):
       distribution: general_gamma_upper_limit
       limit: 19.4e-5
       confidence_level: 0.9
       counts_total: 4
       counts_signal: 1.8
-      background_variance: 1.0
+      background_std: 1.0
     BR(B+->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 4.0e-5
       confidence_level: 0.9
       counts_total: 21
       counts_signal: -1.7
-      background_variance: 1.5
+      background_std: 1.5
     BR(B0->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 5.5e-5
       confidence_level: 0.9
       counts_total: 10
       counts_signal: -2.3
-      background_variance: 0.9
+      background_std: 0.9
     BR(B+->pinunu):
       distribution: general_gamma_upper_limit
       limit: 9.8e-5
       confidence_level: 0.9
       counts_total: 107
       counts_signal: 15.2
-      background_variance: 1.4
+      background_std: 1.4
     BR(B0->pinunu):
       distribution: general_gamma_upper_limit
       limit: 6.9e-5
       confidence_level: 0.9
       counts_total: 6
       counts_signal: 3.5
-      background_variance: 0.6
+      background_std: 0.6
     BR(B+->rhonunu):
       distribution: general_gamma_upper_limit
       limit: 21.3e-5
       confidence_level: 0.9
       counts_total: 90
       counts_signal: 11.3
-      background_variance: 4.1
+      background_std: 4.1
     BR(B0->rhonunu):
       distribution: general_gamma_upper_limit
       limit: 20.8e-5
       confidence_level: 0.9
       counts_total: 31
       counts_signal: 1.6
-      background_variance: 0.4
+      background_std: 0.4
 
 BaBar B->Knunu had 2013:
   experiment: BaBar
   inspire: Lees:2013kla
   values:
     # Tables IV and V
     # For K*, the number and uncertainty of backround events is combined for the
     # two channels K+pi0/K0pi+ or K+pi-/K0pi0, respectively
     BR(B+->Knunu):
       distribution: general_gamma_upper_limit
       limit: 3.7e-5
       confidence_level: 0.9
       counts_total: 6
       counts_background: 2.9
-      background_variance: 0.1
+      background_std: 0.1
     BR(B0->Knunu):
       distribution: general_gamma_upper_limit
       limit: 8.1e-5
       confidence_level: 0.9
       counts_total: 3
       counts_background: 2.9
-      background_variance: 0.2
+      background_std: 0.2
     BR(B+->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 11.6e-5
       confidence_level: 0.9
       counts_total: 6
       counts_background: 4.3
-      background_variance: 0.14
+      background_std: 0.14
     BR(B0->K*nunu):
       distribution: general_gamma_upper_limit
       limit: 9.3e-5
       confidence_level: 0.9
       counts_total: 9
       counts_background: 7.7
-      background_variance: 0.5
+      background_std: 0.5
 
 BaBar B->Knunu SL 2010:
   experiment: BaBar
   inspire: delAmoSanchez:2010bk
   values:
     # Tables II, III and IV
     BR(B+->Knunu):
       distribution: general_gamma_upper_limit
       limit: 1.3e-5
       confidence_level: 0.9
       counts_total: 19.4
       counts_signal: 1.8
-      background_variance: 0.9
+      background_std: 0.9
     BR(B0->Knunu):
       distribution: general_gamma_upper_limit
       limit: 5.6e-5
       confidence_level: 0.9
       counts_total: 6.1
       counts_signal: 2.2
-      background_variance: 0.4
+      background_std: 0.4
 
 LHCb B->tautau 2017:
   experiment: LHCb
   inspire: Aaij:2017xqt
   values:
     BR(Bs->tautau):
       distribution: numerical
@@ -6590,50 +6696,50 @@
   values:
     BR(tau->eee):
         distribution: general_gamma_upper_limit
         limit: 2.7e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.21
-        background_variance: 0.15
+        background_std: 0.15
     BR(tau->mumumu):
         distribution: general_gamma_upper_limit
         limit: 2.1e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.13
-        background_variance: 0.06
+        background_std: 0.06
     BR(tau->emumu):
         distribution: general_gamma_upper_limit
         limit: 2.7e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.10
-        background_variance: 0.04
+        background_std: 0.04
     BR(tau->muee):
         distribution: general_gamma_upper_limit
         limit: 1.8e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.04
-        background_variance: 0.04
+        background_std: 0.04
     BR(tau->muemu):
         distribution: general_gamma_upper_limit
         limit: 1.7e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.02
-        background_variance: 0.02
+        background_std: 0.02
     BR(tau->emue):
         distribution: general_gamma_upper_limit
         limit: 1.5e-8
         confidence_level: 0.9
         counts_total: 0
         counts_background: 0.01
-        background_variance: 0.01
+        background_std: 0.01
 
 PDG 2017 mu LFV:
   experiment: PDG
   inspire: Patrignani:2016xqp
   values:
     BR(mu->egamma): < 4.2e-13 @ 90% CL
     BR(mu->eee):    < 1.0e-12 @ 90% CL
@@ -9773,14 +9879,927 @@
       6.840642771528409e-12, 3.5239813281828545e-12, 1.7834413844648951e-12,
       8.866916854271509e-13, 4.330868391575774e-13, 2.0780973622649082e-13,
       9.795922717795893e-14, 4.5364211203832716e-14, 2.0638110416251535e-14,
       9.225171557120956e-15, 4.319197557578481e-15]
     central_value: [3.0297718212935134e-09, 1.196432308881323e-10]
 
 
+CMS Bs->mumu 2022:
+  experiment: CMS
+  url: http://cds.cern.ch/record/2815334/
+  observables:
+    - BR(Bs->mumu)
+    - BR(B0->mumu)
+  values:
+    distribution: multivariate_numerical
+    xi:
+    - [1.986284262327983e-09, 2.0808933062516934e-09, 2.1755023501754033e-09,
+      2.2701113940991133e-09, 2.3647204380228237e-09, 2.459329481946534e-09,
+      2.553938525870244e-09, 2.648547569793954e-09, 2.7431566137176643e-09,
+      2.8377656576413746e-09, 2.9323747015650846e-09, 3.0269837454887945e-09,
+      3.121592789412505e-09, 3.2162018333362152e-09, 3.310810877259925e-09,
+      3.405419921183635e-09, 3.5000289651073455e-09, 3.594638009031056e-09,
+      3.689247052954766e-09, 3.783856096878476e-09, 3.878465140802186e-09,
+      3.9730741847258965e-09, 4.067683228649606e-09, 4.162292272573316e-09,
+      4.256901316497027e-09, 4.351510360420737e-09, 4.4461194043444475e-09,
+      4.540728448268157e-09, 4.635337492191867e-09, 4.729946536115578e-09,
+      4.824555580039287e-09, 4.919164623962998e-09, 5.013773667886708e-09,
+      5.108382711810418e-09, 5.202991755734129e-09, 5.297600799657838e-09,
+      5.3922098435815486e-09, 5.486818887505259e-09, 5.5814279314289685e-09,
+      5.676036975352679e-09, 5.770646019276389e-09, 5.8652550632000996e-09,
+      5.95986410712381e-09, 6.0544731510475195e-09, 6.14908219497123e-09,
+      6.24369123889494e-09, 6.33830028281865e-09, 6.43290932674236e-09,
+      6.5275183706660704e-09, 6.622127414589781e-09]
+    - [-7.437994531336312e-13, 9.017573627438574e-12, 1.877894670801078e-11,
+      2.8540319788582988e-11, 3.8301692869155195e-11, 4.80630659497274e-11,
+      5.782443903029961e-11, 6.758581211087181e-11, 7.734718519144402e-11,
+      8.710855827201623e-11, 9.686993135258843e-11, 1.0663130443316064e-10,
+      1.1639267751373285e-10, 1.2615405059430505e-10, 1.3591542367487723e-10,
+      1.4567679675544944e-10, 1.5543816983602165e-10, 1.6519954291659386e-10,
+      1.7496091599716607e-10, 1.8472228907773826e-10, 1.9448366215831047e-10,
+      2.0424503523888268e-10, 2.140064083194549e-10, 2.237677814000271e-10,
+      2.335291544805993e-10, 2.432905275611715e-10, 2.5305190064174373e-10,
+      2.628132737223159e-10, 2.725746468028881e-10, 2.823360198834603e-10,
+      2.920973929640325e-10, 3.0185876604460474e-10, 3.1162013912517695e-10,
+      3.2138151220574916e-10, 3.3114288528632137e-10, 3.409042583668936e-10,
+      3.506656314474658e-10, 3.60427004528038e-10, 3.7018837760861016e-10,
+      3.7994975068918237e-10, 3.897111237697546e-10, 3.994724968503268e-10,
+      4.09233869930899e-10, 4.189952430114712e-10, 4.287566160920434e-10,
+      4.3851798917261563e-10, 4.4827936225318784e-10, 4.5804073533376006e-10,
+      4.678021084143323e-10, 4.775634814949044e-10]
+    y:
+    - [6.712618935119312e-07, 7.56209435456342e-07, 8.527719742203528e-07,
+      9.519738821383757e-07, 1.0507740612574722e-06, 1.1454465897561908e-06,
+      1.2319748684434922e-06, 1.3060811132827117e-06, 1.3641282363693222e-06,
+      1.4023782372844687e-06, 1.4188696438272594e-06, 1.4128330591653368e-06,
+      1.3846383550103797e-06, 1.3357663280292383e-06, 1.2689166224097717e-06,
+      1.1880017839357936e-06, 1.0969863501291061e-06, 1.0000279066010901e-06,
+      9.009971725477838e-07, 8.032522726761431e-07, 7.094971338142151e-07,
+      6.216594456862648e-07, 5.408459260004042e-07, 4.676178110074337e-07,
+      4.0186264104572466e-07, 3.431823006529741e-07, 2.909560746881931e-07,
+      2.446536040225052e-07, 2.0382691469741503e-07, 1.6812770755567368e-07,
+      1.3725124056807907e-07, 1.1087332058908058e-07, 8.862412131216861e-08,
+      7.0095071460791e-08, 5.485720631081734e-08, 4.248059208484258e-08,
+      3.255053315207899e-08, 2.4679498033475277e-08, 1.8515063616293636e-08,
+      1.3744367713891782e-08, 1.0095666446954397e-08, 7.337631403478566e-09,
+      5.2770044540218535e-09, 3.755170844658651e-09, 2.6441288250618897e-09,
+      1.8422399313510998e-09, 1.2700489013951518e-09, 8.663739098103903e-10,
+      5.848182014407176e-10, 4.0254564767621736e-10]
+    - [2.7832528641126476e-06, 3.1903470923361034e-06, 3.647776955309146e-06,
+      4.1088464278457475e-06, 4.556670606796639e-06, 4.972908693212869e-06,
+      5.338985932384211e-06, 5.63749497755096e-06, 5.8536679193957505e-06,
+      5.976582198872608e-06, 6.000191844285107e-06, 5.923775759428322e-06,
+      5.751919362002445e-06, 5.494013800061064e-06, 5.163357741707291e-06,
+      4.775975042729766e-06, 4.349248720389379e-06, 3.900653187754457e-06,
+      3.446612369883282e-06, 3.001621649351443e-06, 2.577672020743011e-06,
+      2.1839743609443883e-06, 1.8269158536396355e-06, 1.510361113601504e-06,
+      1.2357970862218588e-06, 1.002797488666941e-06, 8.089976431567823e-07,
+      6.507673095270118e-07, 5.231751185195235e-07, 4.2066664647532384e-07,
+      3.37742315988297e-07, 2.7000249255438576e-07, 2.1424211743366676e-07,
+      1.6839102268218185e-07, 1.309949848572351e-07, 1.0083618040785263e-07,
+      7.680494157196263e-08, 5.78858663792512e-08, 4.316846268310784e-08,
+      3.185453710554065e-08, 2.3258766827261595e-08, 1.6804002667805626e-08,
+      1.2012944466763306e-08, 8.497611419193065e-09, 5.947780552980289e-09,
+      4.119302411634924e-09, 2.8229493519385758e-09, 1.914225807752178e-09,
+      1.2844409082235631e-09, 8.792302169752472e-10]
+    - [1.2353981667575153e-05, 1.418214186612163e-05, 1.6215965059008065e-05,
+      1.823867763955907e-05, 2.01700734497328e-05, 2.1925562701007366e-05,
+      2.3422292528718998e-05, 2.4585976915444528e-05, 2.53573494106871e-05,
+      2.5697413507160863e-05, 2.5590810453114186e-05, 2.5046887205274928e-05,
+      2.409837783474805e-05, 2.2797946152044115e-05, 2.1213113854157505e-05,
+      1.9420271560133244e-05, 1.7498519191558548e-05, 1.552401352427533e-05,
+      1.356534240869335e-05, 1.1680237566663527e-05, 9.913723310545402e-06,
+      8.297612602307047e-06, 6.851130947584221e-06, 5.582363556799065e-06,
+      4.4902047687014536e-06, 3.5665470275193905e-06, 2.7984510177137634e-06,
+      2.170196996317108e-06, 1.6649745336908428e-06, 1.2662045372454942e-06,
+      9.578287116697424e-07, 7.245647199460669e-07, 5.507302322051297e-07,
+      4.210950398325997e-07, 3.226229341165322e-07, 2.461678860696392e-07,
+      1.8622557369725386e-07, 1.3944368409054208e-07, 1.033185568745334e-07,
+      7.574740902979e-08, 5.495002113708205e-08, 3.9443788010494815e-08,
+      2.8015607151359138e-08, 1.968938415106817e-08, 1.3692252409573647e-08,
+      9.421679601626687e-09, 6.41493760770743e-09, 4.321825352521987e-09,
+      2.8811985142473397e-09, 1.960430633054921e-09]
+    - [4.900570354624828e-05, 5.622686128556799e-05, 6.418156411357732e-05,
+      7.198766767972658e-05, 7.931389888030486e-05, 8.582102440746462e-05,
+      9.118810780247034e-05, 9.514022026974849e-05, 9.747305386198838e-05,
+      9.807120412827833e-05, 9.691774718203874e-05, 9.409400347542033e-05,
+      8.976980785924786e-05, 8.418591727007258e-05, 7.763114859140146e-05,
+      7.041730649987512e-05, 6.285490572682436e-05, 5.5232192051643315e-05,
+      4.7799173391986595e-05, 4.0757467806935194e-05, 3.4255926624058696e-05,
+      2.8391321037641105e-05, 2.321295327037849e-05, 1.8729875620405555e-05,
+      1.4919435723842128e-05, 1.1736052520255317e-05, 9.119396395628505e-06,
+      7.001437844726593e-06, 5.312100946226968e-06, 3.98348932109282e-06,
+      2.9527846106993504e-06, 2.16415499085501e-06, 1.5698581753128785e-06,
+      1.1305224018797459e-06, 8.13580063898227e-07, 5.903532809159647e-07,
+      4.334573372953599e-07, 3.2002637592561925e-07, 2.3530807125788326e-07,
+      1.7139297987008453e-07, 1.2353208852529492e-07, 8.809976413036654e-08,
+      6.21699146382001e-08, 4.341066781563041e-08, 2.99932366006902e-08,
+      2.05050517933654e-08, 1.3871041733888532e-08, 9.284701734205056e-09,
+      6.149762456685564e-09, 4.159354250614846e-09]
+    - [0.00017422529723207776, 0.0001995199090481899, 0.00022708908241721987,
+      0.0002537635647852887, 0.0002783479126527175, 0.0002996534458481599,
+      0.0003165948940300722, 0.0003282871510981893, 0.00033412582939997524,
+      0.0003338409082818736, 0.00032751663820825217, 0.0003155758694522485,
+      0.0002987321293685125, 0.00027791709456515207, 0.00025419385795380294,
+      0.00022866723145885786, 0.00020240133371508899, 0.00017635231803114068,
+      0.00015132093002052273, 0.00012792630941788755, 0.000106599618392549,
+      8.759404240540165e-05, 7.100660085599495e-05, 5.6806963319078516e-05,
+      4.4868903512439464e-05, 3.500088935998197e-05, 2.6973358993134794e-05,
+      2.0541269782710744e-05, 1.546139587630493e-05, 1.1504520490059527e-05,
+      8.46310823394701e-06, 6.15527360622705e-06, 4.425932789868864e-06,
+      3.1460164987450315e-06, 2.2105629402236564e-06, 1.536607628766151e-06,
+      1.0608542354684761e-06, 7.349825661809391e-07, 5.173524306200674e-07,
+      3.6964857698261084e-07, 2.641984528619205e-07, 1.8719400714661444e-07,
+      1.3124642573705984e-07, 9.105167654022745e-08, 6.250271978795933e-08,
+      4.2454189634132945e-08, 2.853335670223549e-08, 1.8975614395590505e-08,
+      1.2487360371418546e-08, 8.395131182559053e-09]
+    - [0.0005576322034020957, 0.000636648029132993, 0.0007217831166430796,
+      0.0008029233042709126, 0.0008762705233291614, 0.0009381597230131642,
+      0.000985367482285071, 0.0010154052810620485, 0.001026746923435487,
+      0.0010189599459687567, 0.0009927250656810145, 0.0009497444066180967,
+      0.0008925550984161397, 0.0008242769361005402, 0.0007483292209610754,
+      0.0006681521181442345, 0.0005869626308256166, 0.0005075663208167107,
+      0.00043223534496640516, 0.0003626532661064716, 0.0002999189757633818,
+      0.0002445967743543295, 0.0001967973385336393, 0.00015627456504017386,
+      0.0001225253937908818, 9.488285993104588e-05, 7.259606274886533e-05,
+      5.489390953260124e-05, 4.1032054432559266e-05, 3.0324268322297984e-05,
+      2.2160562464810392e-05, 1.6014860517512054e-05, 1.1445028142754365e-05,
+      8.087789030834909e-06, 5.650620713352523e-06, 3.902242860398717e-06,
+      2.6629059005242005e-06, 1.7955297064439473e-06, 1.1988712109923074e-06,
+      8.01131664665701e-07, 5.45186062412519e-07, 3.786860276581743e-07,
+      2.635595560309618e-07, 1.816842780334186e-07, 1.2391288092215272e-07,
+      8.362232167534661e-08, 5.5839128770677436e-08, 3.689484726097556e-08,
+      2.4122645252790607e-08, 1.6120222939360256e-08]
+    - [0.0016136280149492504, 0.0018348798622982415, 0.00207031557178508,
+      0.0022911031311325055, 0.0024865482356359633, 0.002646647002099181,
+      0.002762948320138556, 0.0028293306987193954, 0.002842557264734017,
+      0.0028025364514102534, 0.0027122600632608013, 0.0025774381281349415,
+      0.002405891982675359, 0.002206795939850335, 0.0019898696032565797,
+      0.0017646173134610126, 0.0015396916763850286, 0.001322430165275811,
+      0.0011185835721947127, 0.0009322280043298813, 0.0007658318578653105,
+      0.0006204373890950878, 0.0004959129048611885, 0.0003912346444218574,
+      0.00030476488082280674, 0.00023450231903583663, 0.00017829055905039227,
+      0.00013397885899298746, 9.953593590063645e-05, 7.312187608618041e-05,
+      5.312557159794991e-05, 3.8175849821987323e-05, 2.7134091970185212e-05,
+      1.907509182124096e-05, 1.326155696830767e-05, 9.11626736529121e-06,
+      6.194647709540155e-06, 4.159466950022846e-06, 2.758596386442988e-06,
+      1.8064594849308384e-06, 1.170291007381419e-06, 7.599371580783092e-07,
+      5.064489430504149e-07, 3.4472182585731215e-07, 2.3369329643795914e-07,
+      1.5669919173563189e-07, 1.039603225731843e-07, 6.824625177964954e-08,
+      4.4332521372503286e-08, 2.9448136503124224e-08]
+    - [0.004238808069334546, 0.004796768273917974, 0.005382565523165356,
+      0.005922406446528393, 0.0063894487012531665, 0.006759392554755133,
+      0.007012604316712259, 0.00713592345867218, 0.007123830414189075,
+      0.0069788275022486315, 0.006711003497815256, 0.006336871100841253,
+      0.005877663479963328, 0.005357334983714582, 0.00480052519771626,
+      0.004230717781395676, 0.0036687667428415924, 0.0031318880332287294,
+      0.002633138889567766, 0.0021813436305021033, 0.001781380225364847,
+      0.0014347193465913545, 0.0011401048611942208, 0.0008942770617803677,
+      0.0006926614573369884, 0.0005299709570187147, 0.000400693273817419,
+      0.0002994554105137666, 0.00022127177819192284, 0.00016169169850820329,
+      0.00011686644976433035, 8.355675341082526e-05, 5.909987809401619e-05,
+      4.1352456826560283e-05, 2.8621528097653483e-05, 1.959281666000426e-05,
+      1.3262214492738462e-05, 8.87396487030033e-06, 5.867215921000117e-06,
+      3.8313363291187075e-06, 2.4695946602551997e-06, 1.5707590384541925e-06,
+      9.899313070572757e-07, 6.327750738006108e-07, 4.1895180730991593e-07,
+      2.7928372938662493e-07, 1.8413319336109185e-07, 1.2009610606169693e-07,
+      7.750986308307893e-08, 5.1177801685668555e-08]
+    - [0.01014784041922637, 0.0114207433432325, 0.012737903713950175,
+      0.01392893206275631, 0.014933457626825752, 0.015698715918475773,
+      0.01618418276302555, 0.01636527724351032, 0.016235458266386484,
+      0.01580646490644017, 0.015106726717900717, 0.014178229652797022,
+      0.013072318756338994, 0.011845020168286213, 0.010552464148182394,
+      0.009246901141919044, 0.007973652915825824, 0.006769165804008308,
+      0.005660166558811356, 0.004663788259193182, 0.003788447822262026,
+      0.0030352200612313233, 0.0023994591688339664, 0.0018724549178519947,
+      0.001442964100861483, 0.0010985154320654184, 0.0008264390196130516,
+      0.0006146139676611817, 0.00045195745319542846, 0.00032869610718281136,
+      0.00023646770076085556, 0.0001683007107232992, 0.00011851407578050471,
+      8.257173454157499e-05, 5.691815534192815e-05, 3.881321581011557e-05,
+      2.6178124400520432e-05, 1.74588497985357e-05, 1.1509717605297748e-05,
+      7.497270991780494e-06, 4.822928702934535e-06, 3.062156972993297e-06,
+      1.9176360343972687e-06, 1.1852714954108855e-06, 7.345942140335223e-07,
+      4.729722016100478e-07, 3.1011945581799963e-07, 2.0105215245798234e-07,
+      1.289209796619674e-07, 8.461308450483226e-08]
+    - [0.02222610337217947, 0.02486432648641659, 0.027551894145622733,
+      0.029932236155267588, 0.03188310739094646, 0.0333016905245138,
+      0.03411360050579352, 0.034279573249595977, 0.03379858740025113,
+      0.03270708668848954, 0.031074540580433824, 0.028996082914865755,
+      0.026583314457730666, 0.023954497694033242, 0.021225308673059638,
+      0.018501079825163205, 0.015871134121360216, 0.013405447703833439,
+      0.011153549799807556, 0.009145320353506403, 0.007393198285087839,
+      0.005895265172199696, 0.004638702627895642, 0.0036032102194278066,
+      0.0027640865010840347, 0.0020947946058386003, 0.001568938693781885,
+      0.001161658780760911, 0.0008505060913316636, 0.000615890961743191,
+      0.00044120517013855544, 0.00031271619021414716, 0.00021931785954758376,
+      0.0001522049869616475, 0.00010452190224941023, 7.101904049778817e-05,
+      4.7738470088912596e-05, 3.173916281664931e-05, 2.0865609731791737e-05,
+      1.3558678051003004e-05, 8.70484976998051e-06, 5.518654783701194e-06,
+      3.4527508353052858e-06, 2.1303522115681507e-06, 1.2959152014443619e-06,
+      7.859906001314649e-07, 4.958791867533392e-07, 3.200257153664732e-07,
+      2.0400071508962077e-07, 1.3308730912486037e-07]
+    - [0.04469922410546479, 0.04968662716575818, 0.05468217618248961,
+      0.05900668629104505, 0.062436358781588444, 0.06479086178666446,
+      0.06594896148138368, 0.06585914114227077, 0.06454314853647862,
+      0.06209219191767511, 0.05865655491994624, 0.05443026597891267,
+      0.04963299585489592, 0.044491503757596675, 0.03922272907134396,
+      0.03402012092529906, 0.029044140250047285, 0.024417192827723585,
+      0.02022266907836341, 0.016507348907428155, 0.013286204948904421,
+      0.010548592848085991, 0.008264913814412973, 0.006393021005438573,
+      0.004883866076843, 0.003686103256321934, 0.0027495568647152584,
+      0.0020275995597708527, 0.0014785796908303687, 0.0010664822011075689,
+      0.0007610181787010629, 0.0005373245172470974, 0.00037542750486125595,
+      0.00025959082615803453, 0.00017763533092785252, 0.00012028859318482485,
+      8.059847991065774e-05, 5.3427046338119385e-05, 3.502860605132634e-05,
+      2.2707887969715408e-05, 1.4549748819681918e-05, 9.209967855568332e-06,
+      5.756366287750558e-06, 3.55020596535216e-06, 2.1590513260475957e-06,
+      1.2941347902710332e-06, 7.730674621041757e-07, 4.82736623843323e-07,
+      3.069904680476629e-07, 1.991492086904351e-07]
+    - [0.08283036353208766, 0.09146195067935844, 0.09995079935328692,
+      0.10711463433244522, 0.11258166858753078, 0.11606667293969623,
+      0.11739526182217788, 0.11651856897100454, 0.1135153000369533,
+      0.10858126444537788, 0.1020082253674561, 0.09415524196835738,
+      0.0854164068539096, 0.07618893839769274, 0.06684504469347331,
+      0.05771000912532304, 0.049047783715373966, 0.041054238043937014,
+      0.03385727345288604, 0.027522377441016647, 0.022061889421215276,
+      0.017446241928914523, 0.013615656664450354, 0.010491122413601745,
+      0.007983876497110503, 0.0060029854534887845, 0.0044609304198621495,
+      0.0032773277597716263, 0.002381054420664796, 0.0017111114974633166,
+      0.0012165662383720988, 0.0008558814355389389, 0.0005958890630763813,
+      0.0004106057250754504, 0.00028003031583795455, 0.00018901476814451107,
+      0.00012625929044618106, 8.345433022585011e-05, 5.457159953328621e-05,
+      3.529417869176334e-05, 2.2569137428690976e-05, 1.4263576026911061e-05,
+      8.905070763115989e-06, 5.489113024453163e-06, 3.33847573648781e-06,
+      2.0020046412200387e-06, 1.1833530203470978e-06, 7.012169224335709e-07,
+      4.3774462880068876e-07, 2.834728859195032e-07]
+    - [0.14191191025589997, 0.1556366234656756, 0.16886664953829092,
+      0.17971329686677104, 0.1876158331698375, 0.1921696908412726,
+      0.19315857770099285, 0.1905687538894407, 0.1845881798147843,
+      0.17558705532452215, 0.16407954780499087, 0.1506735636013218,
+      0.1360175500784201, 0.1207505892643777, 0.10545981710311024,
+      0.0906483586743088, 0.07671552026887446, 0.06394907342062048,
+      0.05252805419481672, 0.04253362335364641, 0.033965174012943425,
+      0.026758960486157186, 0.02080692924455758, 0.015974017548720406,
+      0.012112817293073482, 0.009075081965888158, 0.006720022315012554,
+      0.004919666037030743, 0.003561751267871746, 0.002550703573651686,
+      0.0018072407979895472, 0.0012670898816295956, 0.0008792112250217883,
+      0.0006038297238315537, 0.0004104809862338457, 0.0002762041750112403,
+      0.00018395248610480396, 0.00012124836642190047, 7.908120080205508e-05,
+      5.102752713583164e-05, 3.256489565482437e-05, 2.0547581166007224e-05,
+      1.2813276479598805e-05, 7.89296601285618e-06, 4.800218927696133e-06,
+      2.88037994490276e-06, 1.7041224260800242e-06, 9.947737463438001e-07,
+      5.929859574569688e-07, 3.833134103993229e-07]
+    - [0.22540771091650622, 0.2453012220773916, 0.26389973037165776,
+      0.27854170470710177, 0.28862079307716826, 0.29370965561020285,
+      0.2936088640555784, 0.2883135798158678, 0.2780565604335533,
+      0.2633441252224741, 0.24495462097294987, 0.22387420039149813,
+      0.20115101534287969, 0.17776576528787935, 0.15458040953463456,
+      0.1323144318298899, 0.11152558572383128, 0.092603312139132,
+      0.07577647196302889, 0.06113206366181865, 0.04864074064986538,
+      0.03818518568817889, 0.029588079389055458, 0.022637296124008086,
+      0.017106891024703554, 0.012773272444695276, 0.009426606806340514,
+      0.0068779492187718335, 0.004962843897354, 0.0035422272140969912,
+      0.0025014374212166484, 0.0017480330126096663, 0.0012089841917666926,
+      0.0008276574440654421, 0.000560880400018108, 0.00037626310121649243,
+      0.00024986598740277184, 0.00016424357593173986, 0.00010685257710247666,
+      6.878970933815457e-05, 4.3813308781824554e-05, 2.7600030644192984e-05,
+      1.7190332685299336e-05, 1.0581634866647654e-05, 6.434410276761874e-06,
+      3.8629219408198375e-06, 2.288268033619863e-06, 1.3366012710223599e-06,
+      7.756170558000052e-07, 4.90532280771317e-07]
+    - [0.32933913190831443, 0.35441922767114287, 0.3774560370785067,
+      0.3952093654990806, 0.40687297360476754, 0.4118634564754106,
+      0.40992865571354525, 0.40114873927638534, 0.3859265197295072,
+      0.3649372433728128, 0.33905303612310217, 0.3093263561468987,
+      0.27709138922237386, 0.24391886020274076, 0.21123172306212284,
+      0.1800802824551095, 0.1511991558091353, 0.12507549204510754,
+      0.10197612293146106, 0.08197699483371061, 0.06500032051697181,
+      0.05085454146660288, 0.03927284521559257, 0.0299472446133336,
+      0.022556493132830445, 0.016787213168251446, 0.012348459791613321,
+      0.008980503537754174, 0.006458913971510658, 0.00459511145980512,
+      0.0032344894383415372, 0.00225305345168612, 0.001553326495882037,
+      0.0010600696046697184, 0.0007161857590988885, 0.0004790262438515899,
+      0.0003172051645299993, 0.00020794801764248901, 0.00013494892678088462,
+      8.668220072570776e-05, 5.510108590830631e-05, 3.465461964514777e-05,
+      2.155807414264951e-05, 1.326046544755867e-05, 8.061831064501326e-06,
+      4.8421008428229095e-06, 2.8716412855194323e-06, 1.6806019841319839e-06,
+      9.710597023656047e-07, 5.950602646659381e-07]
+    - [0.4457147128100574, 0.4771174490627085, 0.5055126779806256,
+      0.5266351541479648, 0.5394505130501462, 0.5433212019631711,
+      0.5380527356084189, 0.5239093025017806, 0.5015916311321582,
+      0.4721788335178956, 0.4370384690840826, 0.3977047946001411,
+      0.3557281451749717, 0.3126128859724157, 0.26993065399244376,
+      0.22926656828228809, 0.1917780615341288, 0.15806915637374852,
+      0.1284230328309583, 0.10288284785030825, 0.08130239690375805,
+      0.06339842944018889, 0.04880006023822516, 0.03709175513898698,
+      0.027847975002010743, 0.020658926565140144, 0.015147890691905728,
+      0.010981255412898388, 0.007872708967773612, 0.005583115342959239,
+      0.003917481510618106, 0.002720207299164735, 0.001869547570953581,
+      0.0012719568924782132, 0.0008567569941127509, 0.0005713807042573812,
+      0.0003773059489526156, 0.0002466963709767111, 0.00015970412543059813,
+      0.00010235721453366078, 6.494039378533065e-05, 4.077840686749553e-05,
+      2.5337737248575406e-05, 1.557430477978086e-05, 9.466959934373088e-06,
+      5.68862081184141e-06, 3.377585893517144e-06, 1.9805740412803487e-06,
+      1.1465463971009803e-06, 6.883910197521329e-07]
+    - [0.5713939395801304, 0.6087875367442842, 0.6417458028341284,
+      0.6651621341705654, 0.6778835165984579, 0.6792751139193766,
+      0.6692669957998701, 0.6483599619498447, 0.6175840084952555,
+      0.5784142321926431, 0.5326537310193384, 0.4822964045476961,
+      0.42938348517771624, 0.37587031962011486, 0.32354912593256513,
+      0.2739085557239564, 0.22828978740979194, 0.18750031029128816,
+      0.15181164253977644, 0.1212119323388819, 0.09547121963106753,
+      0.07420529252674286, 0.05693498257425101, 0.043136927322665136,
+      0.032283833455627686, 0.02387385527590814, 0.017449859696526085,
+      0.012610067708855643, 0.009011895171465976, 0.006370849249520892,
+      0.004456167681320272, 0.0030846056128550864, 0.0021134509604995503,
+      0.0014335350401919985, 0.0009627313486710254, 0.0006402161728006757,
+      0.0004216024398454387, 0.00027494768328509733, 0.00017756913155861004,
+      0.00011356353957979119, 7.191686601853395e-05, 4.5091139753747934e-05,
+      2.7986564684221785e-05, 1.7191563951733506e-05, 1.0449065238917266e-05,
+      6.282074699554569e-06, 3.7345419686763073e-06, 2.194330161310231e-06,
+      1.2738672641818595e-06, 7.61459687502082e-07]
+    - [0.6942916119000693, 0.7362391068940458, 0.7721504001658316,
+      0.7962544471333273, 0.8073556995408089, 0.8048983455475841,
+      0.7890058594358642, 0.7604707190191186, 0.7206889107170434,
+      0.6715467582972128, 0.6152728464333374, 0.5542712029756888,
+      0.490953043671189, 0.42758341150592427, 0.36616262091113494,
+      0.3083163906149652, 0.2558062553765015, 0.20936867176716184,
+      0.16894662860998308, 0.1344475367316633, 0.10555169848284567,
+      0.0817767224264035, 0.0625443406320291, 0.047236734442918156,
+      0.035240503492360194, 0.025978136965613362, 0.018928076030825518,
+      0.01363519346375802, 0.009713827877511938, 0.006845497585904213,
+      0.004773192961599521, 0.003293805604276015, 0.0022498763033907596,
+      0.0015214861808805573, 0.0010188085599136972, 0.0006755968646827146,
+      0.000443707109861613, 0.00028863523891607895, 0.00018597880713368617,
+      0.00011869743613329272, 7.503615224446896e-05, 4.698106272959548e-05,
+      2.9130859861620512e-05, 1.7885443563662805e-05, 1.0871305356284666e-05,
+      6.5403346151461375e-06, 3.89345894363195e-06, 2.2927105159181475e-06,
+      1.3350804730493282e-06, 8.006017312105251e-07]
+    - [0.7995441693781381, 0.8438519633099179, 0.8805114714168873,
+      0.9033800123597743, 0.9113160329505325, 0.9039212976344603,
+      0.881566953436832, 0.8453626562355017, 0.7970652782882809,
+      0.738937653584946, 0.6735731672884465, 0.6037050845508967,
+      0.5320200058756371, 0.4609928275602545, 0.39275010831457774,
+      0.3285769373474068, 0.2706236867096729, 0.2206892157165054,
+      0.17748975794459823, 0.14078432345031314, 0.11016969640270988,
+      0.08508147839509228, 0.06486500614176233, 0.048834268657544616,
+      0.03631716436200702, 0.026687244884624338, 0.019383325734816426,
+      0.013919053869769962, 0.009884788697247147, 0.006944088973722936,
+      0.00482682134881244, 0.0033205214317142103, 0.0022612263451193037,
+      0.001524613907064659, 0.0010179591748958141, 0.0006731665132350226,
+      0.0004409538074616576, 0.00028614622668898603, 0.00018396769719299737,
+      0.0001171860059525684, 7.396046087215738e-05, 4.62496589746146e-05,
+      2.8653889949450567e-05, 1.758696124844027e-05, 1.069253101796231e-05,
+      6.438529092570539e-06, 3.839070586252158e-06, 2.266198354565854e-06,
+      1.3240661429086666e-06, 7.971517143277534e-07]
+    - [0.8726549876576977, 0.9166704268559658, 0.9516290878577945,
+      0.9713788792302185, 0.9749283037783799, 0.9620990281187605,
+      0.9335335865920766, 0.8906420460865424, 0.8354866494440489,
+      0.77061757565431, 0.6988780164124241, 0.6231992530825169,
+      0.5464061050883234, 0.4710502477614341, 0.3992691383642107,
+      0.3317262837825194, 0.2709864022141572, 0.22017866346490844,
+      0.17649641047643833, 0.13954153421729734, 0.10884569156916422,
+      0.08379017979611778, 0.06367708918728499, 0.04778757793196911,
+      0.035425905543357276, 0.025949659063399744, 0.01878777580388604,
+      0.013448609432144763, 0.009520491838928051, 0.006667129213933859,
+      0.0046198568850207644, 0.0031683678079000954, 0.0021511034938434025,
+      0.0014461063815950695, 0.0009628080829244647, 0.0006349787906379795,
+      0.0004148868790035194, 0.0002686043645557402, 0.00017233024722220158,
+      0.00010957637410072338, 6.905740847880258e-05, 4.3138098888970356e-05,
+      2.6710154307688982e-05, 1.6392719453322406e-05, 9.971626676178647e-06,
+      6.011579810874654e-06, 3.5914634288307917e-06, 2.1259445436033307e-06,
+      1.2467514861152368e-06, 7.541649919333437e-07]
+    - [0.902711366473401, 0.9437704973955824, 0.9747800210435189,
+      0.9899495356698267, 0.9885134156754539, 0.9705438317028565,
+      0.9369379160681846, 0.8893435291917413, 0.8300253552572405,
+      0.7616864740161501, 0.6872649603371269, 0.6097267315240649,
+      0.5318747136815495, 0.4561905746705044, 0.3845852841685461,
+      0.31644632546586776, 0.25734482762060035, 0.20844862803328545,
+      0.166547759278398, 0.13124969801034853, 0.10204854914391953,
+      0.07830598849824395, 0.05931904688790544, 0.04437476787069108,
+      0.03279081334690493, 0.023942696432411804, 0.017279372251864746,
+      0.01232946566294223, 0.008700553241023446, 0.00607376172398875,
+      0.004195612121352429, 0.0028686263631397943, 0.0019417954804898158,
+      0.001301632749028913, 0.0008642271003121998, 0.0005684790415366235,
+      0.0003705392055097824, 0.00023936776713136599, 0.00015327798580056794,
+      9.730584933402843e-05, 6.124867023967132e-05, 3.822935524881106e-05,
+      2.3663223551023593e-05, 1.4526164067871816e-05, 8.843831926331484e-06,
+      5.340024788206202e-06, 3.1977750624654968e-06, 1.8990232027632275e-06,
+      1.118448604814513e-06, 6.842782757788309e-07]
+    - [0.885034372360477, 0.9209254282809944, 0.9463470259776241,
+      0.9561859269362215, 0.949942564898247, 0.9279304427065218,
+      0.891243904184439, 0.8416679628123735, 0.7815343937435271,
+      0.713540237199466, 0.6405483490655673, 0.5653904109032142,
+      0.4906908482651723, 0.41869100195596504, 0.34995220110055214,
+      0.28514158204262424, 0.23242918946449342, 0.1877105582878339,
+      0.1494912580306317, 0.11742770675970252, 0.09100790030935633,
+      0.06960964846416337, 0.05256192898986493, 0.0391936256469666,
+      0.028869102711538624, 0.021011467936806954, 0.015115273467400395,
+      0.010750844285564191, 0.007562497675125192, 0.0052627347288751345,
+      0.0036241523691912365, 0.0024704306192450468, 0.001667360262562217,
+      0.0011145318490466776, 0.0007380288269603686, 0.0004842603679285115,
+      0.00031492792381276305, 0.00020303288343981264, 0.00012978809832683665,
+      8.22811653112721e-05, 5.174160593464805e-05, 3.2279192089475355e-05,
+      1.9980674294022807e-05, 1.2273131977979295e-05, 7.48174012632301e-06,
+      4.526750969801057e-06, 2.718518843599663e-06, 1.6205207434837847e-06,
+      9.595341240543228e-07, 5.994090789060847e-07]
+    - [0.822356822180574, 0.8516702308690954, 0.8707293000656275,
+      0.8753073465019127, 0.8651692253824129, 0.8408230849994593,
+      0.8034729594299026, 0.7549200819596565, 0.6974189858240273,
+      0.6335043891185291, 0.5658073236694465, 0.4968784160563884,
+      0.4289882968800894, 0.363164619828652, 0.2993296483871571,
+      0.2452648441283822, 0.20016819871345307, 0.16114088721985548,
+      0.12791679300050446, 0.10015679470457686, 0.07737274743280544,
+      0.05898979227479709, 0.044399271809841295, 0.03300014249571816,
+      0.024228648120269484, 0.017577192348481062, 0.01260407761754945,
+      0.008936109379959421, 0.006266084280090729, 0.004346986905697939,
+      0.0029844056096487884, 0.0020283201879893126, 0.0013650680830849219,
+      0.0009099951232767907, 0.0006010574890140196, 0.0003934661782220353,
+      0.0002553477846951204, 0.00016432555354110797, 0.00010489076019130882,
+      6.642546975151292e-05, 4.174441725087284e-05, 2.6038991566059533e-05,
+      1.612507142024698e-05, 9.915492715028388e-06, 6.055344374531108e-06,
+      3.6732026621638517e-06, 2.2135762826818734e-06, 1.3253989588267608e-06,
+      7.916184016523654e-07, 5.028375754096408e-07]
+    - [0.724213610383652, 0.7464911971851631, 0.7593152404258129,
+      0.759425228573551, 0.7468115033606897, 0.7221045005739013,
+      0.6865183961612521, 0.6417522222572686, 0.5898555331438492,
+      0.5330732742066074, 0.4736791524232216, 0.4136872421100274,
+      0.3539559964350399, 0.2957536868945456, 0.2452481313127133,
+      0.20232828249866872, 0.16468961931167084, 0.132153321610565,
+      0.10456875439914354, 0.08161239664545773, 0.06284387584031562,
+      0.047758237909260565, 0.03582953935200254, 0.0265444491643014,
+      0.019425860026571276, 0.014047449519724177, 0.01004069653857304,
+      0.007096092034364205, 0.004960262618857613, 0.003430535142780639,
+      0.0023481885709202743, 0.001591329516605057, 0.0010680341769294492,
+      0.0007101485750064876, 0.0004679424538811296, 0.0003056705284006231,
+      0.0001980019959577157, 0.00012722584417288442, 8.111540210487691e-05,
+      5.133140500428706e-05, 3.225085909220861e-05, 2.0123368691111234e-05,
+      1.2473272734929593e-05, 7.682372138409501e-06, 4.702791435369439e-06,
+      2.8619818949086216e-06, 1.7319243658022942e-06, 1.042717533343047e-06,
+      6.330358688091238e-07, 3.991962859657202e-07]
+    - [0.6044763114395044, 0.6201319899181525, 0.6275774004052289,
+      0.6244759086480277, 0.6109802275135643, 0.5877622612178001,
+      0.5559545584390072, 0.5170583177715398, 0.47282024020745633,
+      0.425047371001792, 0.37523727576973054, 0.3244533783581529,
+      0.2757277883259635, 0.23252673917536937, 0.19416379769815018,
+      0.15984588671415786, 0.12969668942205362, 0.10374170157167578,
+      0.08182518826952148, 0.06365711571964733, 0.048860176530436686,
+      0.037011567391486734, 0.02767735860562716, 0.020438578025898536,
+      0.01490916258656775, 0.010746653212153838, 0.007656925344348925,
+      0.005394400410506089, 0.003759137768318604, 0.002592031769306211,
+      0.0017690978133386374, 0.0011955745615544995, 0.0008003311907149123,
+      0.0005308683741368084, 0.00034904730772598733, 0.00022757186625111425,
+      0.000147179091683199, 9.445457159183196e-05, 6.017339724896075e-05,
+      3.80666932916806e-05, 2.3922025901043834e-05, 1.493875732696822e-05,
+      9.273514493394583e-06, 5.724467331608258e-06, 3.515051176325205e-06,
+      2.1477132435927444e-06, 1.3062247506514e-06, 7.938825550012693e-07,
+      4.890744128685126e-07, 2.9852914425718655e-07]
+    - [0.47817833786307334, 0.48824997174374596, 0.4916001368908028,
+      0.48668465002064915, 0.4737494274307362, 0.4534373586289217,
+      0.42672727676804123, 0.39483480228584356, 0.35905401246630453,
+      0.3207527285914712, 0.2818354370154158, 0.24445563817841026,
+      0.2095595922111511, 0.17715331447781568, 0.1475471746902809,
+      0.12108802026736586, 0.09793957854253722, 0.07809210269337519,
+      0.06139866295393288, 0.047613539563570964, 0.03642873973608892,
+      0.027506009946656754, 0.020502814833839315, 0.015091739091212445,
+      0.01097354607741984, 0.007884658555360455, 0.005600119905578782,
+      0.003933185567033583, 0.0027326368446502444, 0.0018787577278361492,
+      0.001278718907103991, 0.0008619096174579808, 0.0005755726630437766,
+      0.0003809449035489498, 0.0002499894139301063, 0.00016272497364801705,
+      0.00010510835271074075, 6.7398356742742e-05, 4.2921033547981306e-05,
+      2.7156912755590787e-05, 1.7078950016003085e-05, 1.0680559994658132e-05,
+      6.644474216726963e-06, 4.1137934185497955e-06, 2.5358335437969756e-06,
+      1.5569583423082727e-06, 9.53355048105492e-07, 5.896294194272398e-07,
+      3.554731518307508e-07, 2.1151037072154834e-07]
+    - [0.3589694112452352, 0.36487022586042217, 0.36562537249962596,
+      0.3603238759745579, 0.34927152350832524, 0.33304143388805224,
+      0.31241990494638594, 0.2883868898042948, 0.262066704939845,
+      0.23460386461782906, 0.20694442887306208, 0.17981361611711053,
+      0.1538720874540595, 0.12969051945629023, 0.10768333353094334,
+      0.08809893334459035, 0.07103492118632941, 0.056462020798187997,
+      0.0442522277942942, 0.03420783551710521, 0.026088655687701526,
+      0.01963557239296571, 0.014589395512693283, 0.010704707648327766,
+      0.007758962066755261, 0.005557464421125276, 0.003935067260354774,
+      0.0027554543765119666, 0.001908832879252198, 0.0013087264144508062,
+      0.0008884095379076733, 0.0005973684685607565, 0.00039803524197804907,
+      0.0002629300213865154, 0.00017226267414744483, 0.00011198786377919231,
+      7.227351740902779e-05, 4.632534364685307e-05, 2.9504957638436104e-05,
+      1.8681708193420105e-05, 1.1765063388355271e-05, 7.372948813430795e-06,
+      4.600157480825426e-06, 2.858945678894373e-06, 1.770760999504528e-06,
+      1.0938771211061378e-06, 6.79279315496832e-07, 4.1832829467190557e-07,
+      2.418674719580693e-07, 1.4249048472974732e-07]
+    - [0.26007746344207394, 0.2634114872837626, 0.2631174186969177,
+      0.2586469373096039, 0.25022276272741584, 0.23824218957181825,
+      0.22325424704262847, 0.20591982912103196, 0.1869576073302957,
+      0.16709483676521936, 0.1470269427833417, 0.12737892564609826,
+      0.1086747833099847, 0.09131935981360352, 0.07559277826220276,
+      0.06165519224940416, 0.04955954539466698, 0.03926968586058449,
+      0.03068115723375392, 0.023642284097715148, 0.01797368014159423,
+      0.013484912221230895, 0.009987653108963159, 0.007305173466861258,
+      0.005278416388594729, 0.0037691519711156754, 0.0026608343339378105,
+      0.0018578036056329246, 0.0012834214370006003, 0.0008776311901332268,
+      0.000594319110177014, 0.00039873977369796806, 0.00026517009451952617,
+      0.00017487711754990824, 0.0001144269987647396, 7.432413575861823e-05,
+      4.7946932434524616e-05, 3.073618740706038e-05, 1.9589831174756858e-05,
+      1.2420549322202344e-05, 7.838313518339676e-06, 4.926321513573856e-06,
+      3.0852607895824625e-06, 1.926570037596563e-06, 1.2003624915116862e-06,
+      7.499235931587833e-07, 4.681715842806582e-07, 2.748971376882358e-07,
+      1.5597878845372087e-07, 9.132220248431404e-08]
+    - [0.18324173282809728, 0.18502553012040046, 0.1842485220925597,
+      0.18058508193215306, 0.1742009025900058, 0.16538860388642077,
+      0.15454430021577714, 0.14213718072775403, 0.12867500904024087,
+      0.11466909226734597, 0.10060215353226307, 0.08690187116988111,
+      0.0739219091251486, 0.06193121631286882, 0.05111136409000529,
+      0.04156086261442292, 0.03330483618260867, 0.02630817545386192,
+      0.020490299889863554, 0.015739897781502678, 0.01192838467858585,
+      0.008921252065295027, 0.006586896306656598, 0.0048028726814962446,
+      0.0034597828255612147, 0.002463168983855178, 0.0017338637824857255,
+      0.0012072481478770222, 0.0008318247699014047, 0.000567441665887542,
+      0.00038341785992209847, 0.0002567438812124368, 0.0001704615963069696,
+      0.00011227440606616621, 7.340045883884717e-05, 4.7656643888064604e-05,
+      3.0747119890530374e-05, 1.97241378839534e-05, 1.2588299952662826e-05,
+      7.997991402512309e-06, 5.061920148505282e-06, 3.1933913445267373e-06,
+      2.009461797708436e-06, 1.2622050222695693e-06, 7.944679831323041e-07,
+      5.004911156792013e-07, 2.978084092534598e-07, 1.6986563762007214e-07,
+      9.56776965434815e-08, 5.568139129386671e-08]
+    - [0.12447164191871543, 0.12532091438972726, 0.1244152297955928,
+      0.12157816203740708, 0.11693617504550005, 0.11069903809714533,
+      0.10314324423198569, 0.09459102637240399, 0.08538692889821205,
+      0.0758743643697947, 0.06637440414699147, 0.05716859337297826,
+      0.04848693824086554, 0.04050150030717383, 0.03332536037236105,
+      0.027016172872714544, 0.02158317617568099, 0.016996371527991154,
+      0.013196616038885323, 0.010105550534898398, 0.0076345464615570815,
+      0.005692151745686975, 0.004189796883428194, 0.003045756794242877,
+      0.002187534079471003, 0.0015529320908222756, 0.0010901288667273384,
+      0.0007570588566851457, 0.0005203739008476525, 0.00035420276355569287,
+      0.00023887149352330643, 0.0001596933414530316, 0.0001058917950290073,
+      6.968550512871493e-05, 4.553942217293141e-05, 2.9571026130410612e-05,
+      1.9092225377839773e-05, 1.2264334054895108e-05, 7.843738561040658e-06,
+      4.998006940718856e-06, 3.175239407168517e-06, 2.0127124088264855e-06,
+      1.2740395307986754e-06, 8.08217065554497e-07, 5.125784376333282e-07,
+      3.077070974718262e-07, 1.76416778070465e-07, 9.9769344015868e-08,
+      5.583188440722487e-08, 3.229765008835886e-08]
+    - [0.0815861626440467, 0.08191333178916102, 0.08108103384939247,
+      0.07900185183280654, 0.07576736094461912, 0.0715218710107974,
+      0.06645117668425134, 0.06076860073932137, 0.054699652531346565,
+      0.04846687941028508, 0.04227634859827496, 0.036306881050279065,
+      0.030702729839736976, 0.025569928571747513, 0.020976102447489806,
+      0.016953192819060308, 0.013502329155852439, 0.010599998725721002,
+      0.008204700115800332, 0.006263392517129996, 0.004717231663767269,
+      0.00350627910037137, 0.0025730540635724524, 0.0018649463649039468,
+      0.0013356142791031134, 0.000945552641986499, 0.0006620387619389818,
+      0.00045865663728994054, 0.0003145737217871303, 0.00021370862450018752,
+      0.00014389022491178658, 9.607389097724618e-05, 6.36516928068931e-05,
+      4.187174917707588e-05, 2.7366882727351367e-05, 1.7783596422226357e-05,
+      1.1497708344612255e-05, 7.401474603937285e-06, 4.747541585619846e-06,
+      3.036697963715918e-06, 1.9385024415515493e-06, 1.2362080261426058e-06,
+      7.904599711366168e-07, 5.03706834549464e-07, 3.034298068576989e-07,
+      1.7472708133160422e-07, 9.921940272723729e-08, 5.5747611054986205e-08,
+      3.099529982538833e-08, 1.7822710491595414e-08]
+    - [0.05168528259943725, 0.05174870437445711, 0.05107232624596004,
+      0.04961838644634292, 0.0474502528472848, 0.04466352353999961,
+      0.04137866557767632, 0.03773204998649937, 0.03386624526844641,
+      0.029920560079656083, 0.02602272311638767, 0.022282377987791754,
+      0.018786793931452436, 0.015598897453897094, 0.012757460613092504,
+      0.010279073576157408, 0.008161402052193498, 0.006387187830211225,
+      0.004928482642138222, 0.003750692174043964, 0.0028161244193506255,
+      0.0020868617009606916, 0.0015268900504044282, 0.0011035110716701272,
+      0.0007881244347664391, 0.0005565038994913814, 0.00038870039180764293,
+      0.00026869837566212987, 0.00018393328372264984, 0.00012475408646353862,
+      8.389082033159229e-05, 5.596512403946055e-05, 3.7064164650845315e-05,
+      2.4385252808135084e-05, 1.5949661859189934e-05, 1.0378965825407706e-05,
+      6.724727210147143e-06, 4.341754851457116e-06, 2.7956996245347887e-06,
+      1.7969224581361807e-06, 1.154300957351496e-06, 7.439837164554608e-07,
+      4.7477201202864083e-07, 2.856003659640823e-07, 1.650341518996603e-07,
+      9.409830224533907e-08, 5.30865954923099e-08, 2.963456926582187e-08,
+      1.6370148319184945e-08, 9.356637346317852e-09]
+    - [0.03169562070516021, 0.03164486416164781, 0.03113750369842453,
+      0.03016132977266601, 0.028758484103969903, 0.026990125905219,
+      0.024931775282477437, 0.022667743230352016, 0.020285192174537624,
+      0.01786842877161066, 0.015493958963659238, 0.01322669996410929,
+      0.01111757081101239, 0.00920250192764402, 0.007502742205420327,
+      0.006026220063742976, 0.004769643792708459, 0.003721007325429038,
+      0.0028621931082407036, 0.002171421141210332, 0.0016253676111337664,
+      0.0012008537765137068, 0.0008760748562525964, 0.0006313926703104742,
+      0.0004497518508379577, 0.00031679816698177007, 0.0002207817736367104,
+      0.00015232203042421882, 0.00010409811481441482, 7.051460252563821e-05,
+      4.737623446065414e-05, 3.159296893539019e-05, 2.0925986016927697e-05,
+      1.3777749954875093e-05, 9.024290317243052e-06, 5.8850485817600235e-06,
+      3.824402152122704e-06, 2.47880527789849e-06, 1.6039857085252208e-06,
+      1.0379954709797977e-06, 6.739502498877046e-07, 4.2849117009519894e-07,
+      2.5648355542836945e-07, 1.486523080573546e-07, 8.510331466754244e-08,
+      4.8208430103776196e-08, 2.702154429555127e-08, 1.4986768979813348e-08,
+      8.225199159938174e-09, 4.673076354112931e-09]
+    - [0.018843954316266155, 0.018758085893931253, 0.0183992110407876,
+      0.017766856376011452, 0.01688807549852285, 0.015800749213751825,
+      0.014550732261955602, 0.013188501796044099, 0.011765639996573906,
+      0.010331504349667954, 0.00893039094391176, 0.0075994117443673815,
+      0.00636720206369137, 0.0052534670724959116, 0.004269282231935815,
+      0.00341799368545959, 0.0026965267602224187, 0.0020969036985158214,
+      0.001607790591468951, 0.0012159301950560796, 0.0009073628260571827,
+      0.000668383574929591, 0.00048622432031430714, 0.0003494796944597337,
+      0.0002483159013843194, 0.000174510778117578, 0.00012137464398000518,
+      8.359680980286142e-05, 5.705462121087212e-05, 3.861270170496587e-05,
+      2.5931180820674236e-05, 1.729407881849103e-05, 1.1463094187721243e-05,
+      7.557844136207262e-06, 4.960943311320391e-06, 3.244859495156467e-06,
+      2.1169237874317645e-06, 1.3790386895869709e-06, 8.994616977465771e-07,
+      5.866710227270109e-07, 3.6897316278194247e-07, 2.1962358394102807e-07,
+      1.2768599369327532e-07, 7.339825260275919e-08, 4.1747998592817174e-08,
+      2.349612632256852e-08, 1.3084813812899388e-08, 7.210236281158781e-09,
+      3.931627112682933e-09, 2.220332662933302e-09]
+    - [0.010877630776891868, 0.010793584910074412, 0.010551199984462994,
+      0.010154394411840763, 0.009619991834379525, 0.008970756396177915,
+      0.00823369662028946, 0.007438110520996381, 0.006613568873456825,
+      0.005788037490322026, 0.004986308102986284, 0.004228856372453924,
+      0.0035311841248019658, 0.0029036413784441903, 0.0023516711735966263,
+      0.0018763829918272154, 0.0014753415566711799, 0.0011434564961250043,
+      0.000873871465686868, 0.0006587740048455172, 0.0004900743369201059,
+      0.0003599278141111463, 0.0002610982927971976, 0.00018717643911618813,
+      0.00013267727064672307, 9.304569459962935e-05, 6.459864196767454e-05,
+      4.442912320165889e-05, 3.029258953729448e-05, 2.0490557829239257e-05,
+      1.376137668364866e-05, 9.183759091969998e-06, 6.095472177322806e-06,
+      4.027341582621287e-06, 2.6513574045402675e-06, 1.7410058393161354e-06,
+      1.1421454678785313e-06, 7.509453873259801e-07, 4.88478562541475e-07,
+      3.02270663476517e-07, 1.7926429198924357e-07, 1.045917150677028e-07,
+      6.036853611220336e-08, 3.447736083538001e-08, 1.9483548375093042e-08,
+      1.0894637007282693e-08, 6.0279292462326895e-09, 3.3001539355149806e-09,
+      1.7878926421958286e-09, 1.0036364728339136e-09]
+    - [0.006105352366080819, 0.006036954057686424, 0.005879375606069314,
+      0.005637389367162256, 0.00532115694416527, 0.004943974193470022,
+      0.004521291962515797, 0.004069610129678024, 0.003605358121581725,
+      0.0031438721432772826, 0.0026985597197961967, 0.002280312140578187,
+      0.0018971904914814562, 0.0015543769029898891, 0.0012543543658303778,
+      0.0009972592658872923, 0.0007813419723128453, 0.0006034717724013995,
+      0.0004596311257381852, 0.0003453577474798067, 0.0002561084364354053,
+      0.00018753326685005774, 0.00013566094866320755, 9.700488054889501e-05,
+      6.860450967660063e-05, 4.8018492619246956e-05, 3.328558191604273e-05,
+      2.2867009833956728e-05, 1.5581207350723057e-05, 1.053861661365952e-05,
+      7.0815570814056675e-06, 4.7318213861357095e-06, 3.146982197152067e-06,
+      2.0852668239030873e-06, 1.3783961314527184e-06, 9.114418709109727e-07,
+      6.02251819988754e-07, 3.86108208536434e-07, 2.3523205356179056e-07,
+      1.39489291617271e-07, 8.170244569680549e-08, 4.735013809346951e-08,
+      2.7153014467705064e-08, 1.5407263949340126e-08, 8.650548892964132e-09,
+      4.805875082217273e-09, 2.6418731543500823e-09, 1.437017695409336e-09,
+      7.734883374575997e-10, 4.315966251957179e-10]
+    - [0.003336596512235319, 0.003286266842010908, 0.003187118226732012,
+      0.0030433218459185118, 0.002860850880744744, 0.0026472630167798795,
+      0.0024111509910693598, 0.002161535668565108, 0.0019072647509542667,
+      0.0016564754641842149, 0.0014161676062166176, 0.0011919162196336274,
+      0.000987733950969018, 0.0008060749810155493, 0.0006479578251883329,
+      0.0005131749263077955, 0.00040055330032227226, 0.0003082320355291521,
+      0.0002339279335813029, 0.00017516839215280238, 0.00012947913752328467,
+      9.452227472117781e-05, 6.818643070408916e-05, 4.863509968359397e-05,
+      3.432165348891343e-05, 2.3980143726114534e-05, 1.6600443487829905e-05,
+      1.1394935970138587e-05, 7.762283146705963e-06, 5.252124772694959e-06,
+      3.533075496153698e-06, 2.365216595237434e-06, 1.5775586058196249e-06,
+      1.0505758488349458e-06, 7.000895323020252e-07, 4.594796184939591e-07,
+      2.880887906704764e-07, 1.7406553175604126e-07, 1.0348886762539372e-07,
+      6.086174153821018e-08, 3.5416361269372965e-08, 2.0392673778538423e-08,
+      1.1618634111892709e-08, 6.550080680464317e-09, 3.6538346853418176e-09,
+      2.0167952488135637e-09, 1.1015022676774379e-09, 5.952777530561331e-10,
+      3.183433049702062e-10, 1.7656688810212845e-10]
+    - [0.0017779302063878216, 0.0017433114972322133, 0.0016827025692570624,
+      0.0015992614446384767, 0.0014964096509397042, 0.001378331793571694,
+      0.001249675943314938, 0.0011152307129902036, 0.0009796131414252565,
+      0.0008469970819122531, 0.0007209047229740243, 0.0006040743969573114,
+      0.0004984076206263133, 0.0004049889812831304, 0.0003241653071027223,
+      0.00025566627816430034, 0.00019874738700496154, 0.00015233756445932938,
+      0.00011517711138299739, 8.593593030681738e-05, 6.330658239603382e-05,
+      4.607073216503121e-05, 3.314066319423569e-05, 2.357958604871502e-05,
+      1.6605459608337663e-05, 1.1583195135826845e-05, 8.009661267453071e-06,
+      5.495114265647721e-06, 3.7437593972232004e-06, 2.5352709817326934e-06,
+      1.708438353780286e-06, 1.1478358391432864e-06, 7.71119989687732e-07,
+      5.134606314696358e-07, 3.296325651393549e-07, 2.0319100043632457e-07,
+      1.2268381727509037e-07, 7.321721776303759e-08, 4.323501444349875e-08,
+      2.5262050693002088e-08, 1.4605360023390417e-08, 8.355387614200495e-09,
+      4.7296783615005245e-09, 2.6491544817536384e-09, 1.4682284372888368e-09,
+      8.0517568082183e-10, 4.369163909093338e-10, 2.345938899319151e-10,
+      1.246456652293398e-10, 6.871950045475247e-11]
+    - [0.0009249741021209297, 0.0009023404337073773, 0.0008662473529973777,
+      0.0008188869875137216, 0.0007621704293859893, 0.0006983553782791974,
+      0.0006298874844489501, 0.0005592339768503073, 0.0004887274427316706,
+      0.00042043422762770615, 0.00035605787869230366, 0.00029688297794583883,
+      0.00024375947680441504, 0.00019712305712316205, 0.00015704370535010793,
+      0.0001232928994514845, 9.54195707448254e-05, 7.282605813045956e-05,
+      5.4837203990110336e-05, 4.075808064265251e-05, 2.9918158054590683e-05,
+      2.170170945280434e-05, 1.556571901545902e-05, 1.1047452495738419e-05,
+      7.764226810627385e-06, 5.407880523534329e-06, 3.736140556990173e-06,
+      2.5626409338411706e-06, 1.7469813728265315e-06, 1.1858928547133676e-06,
+      8.038166963649862e-07, 5.411933042112445e-07, 3.5356673874623135e-07,
+      2.2194839441389227e-07, 1.3611666180048183e-07, 8.243870469734285e-08,
+      4.93988419044472e-08, 2.928953809306206e-08, 1.7183789674018794e-08,
+      9.975531506976167e-09, 5.730121247065277e-09, 3.2568836886560285e-09,
+      1.831687397276108e-09, 1.019321386166359e-09, 5.612826084173318e-10,
+      3.058177619768123e-10, 1.648748815358404e-10, 8.7954275974233e-11,
+      4.643033912568581e-11, 2.5444501203873314e-11]
+    - [0.0004704575596260176, 0.0004562562892495067, 0.0004352769344634162,
+      0.00040894967193800717, 0.000378315302407611, 0.00034456042346846054,
+      0.00030893598458697736, 0.0002726744869548956, 0.0002369148706123515,
+      0.0002026417864589921, 0.00017064371280983202, 0.0001414917493871859,
+      0.00011553834476968077, 9.293306961767054e-05, 7.365109885838859e-05,
+      5.7529418124861955e-05, 4.4305878928540893e-05, 3.3656932438324745e-05,
+      2.5230947419390896e-05, 1.8675227284743713e-05, 1.3655981794683991e-05,
+      9.87143970913294e-06, 7.0589388470633024e-06, 4.997191802665374e-06,
+      3.5050378016363434e-06, 2.4379393844186224e-06, 1.6834119968479077e-06,
+      1.156251031538716e-06, 7.92138927404133e-07, 5.38739784152062e-07,
+      3.561416406503188e-07, 2.2698494045574868e-07, 1.4134549699967967e-07,
+      8.687491811242374e-08, 5.282551096267242e-08, 3.17835369172632e-08,
+      1.892219053211469e-08, 1.1146827196640226e-08, 6.49743280085379e-09,
+      3.747511680694321e-09, 2.1387245983783977e-09, 1.2077509962251691e-09,
+      6.748552253734681e-10, 3.7312512688908435e-10, 2.0413103991093395e-10,
+      1.1050305135755173e-10, 5.919024854793514e-11, 3.137160422294874e-11,
+      1.6453793403372413e-11, 8.96287619997813e-12]
+    - [0.00023423356950749718, 0.00022563012984704988, 0.000213710679727349,
+      0.0001993637016720276, 0.00018314144487678778, 0.0001656508054890125,
+      0.00014751292317855184, 0.00012932353609614389, 0.00011161850253598563,
+      9.484739743116173e-05, 7.935689966294035e-05, 6.538437989713873e-05,
+      5.306088897766783e-05, 4.242180470534627e-05, 3.3422823367472075e-05,
+      2.5958807131742712e-05, 1.988317454317926e-05, 1.502595441892426e-05,
+      1.120919632434721e-05, 8.259029812169713e-06, 6.0141989524260884e-06,
+      4.331310970817938e-06, 3.0873093830201635e-06, 2.179864368241379e-06,
+      1.5264704567003701e-06, 1.062565579220519e-06, 7.367138787536867e-07,
+      5.054558267200032e-07, 3.369364676142037e-07, 2.17474742946072e-07,
+      1.373770748136481e-07, 8.568281963076969e-08, 5.286966200841129e-08,
+      3.227957569221131e-08, 1.9501129449731434e-08, 1.1657418386162144e-08,
+      6.89533979674747e-09, 4.035707040353171e-09, 2.3371913096904476e-09,
+      1.3393052271185658e-09, 7.594086427322191e-10, 4.260711984609143e-10,
+      2.3653722132391985e-10, 1.2993539598283003e-10, 7.062624693025126e-11,
+      3.798529061079707e-11, 2.02150792788681e-11, 1.064501101148378e-11,
+      5.547021410982155e-12, 3.0035196109175577e-12]
+    - [0.00011430908549799293, 0.00010925548580677869, 0.00010262903810613574,
+      9.495935940680843e-05, 8.653147093258797e-05, 7.764683228363457e-05,
+      6.86040704079816e-05, 5.968083834915174e-05, 5.111886362184932e-05,
+      4.3113342854702106e-05, 3.58072309511941e-05, 2.9290353175261008e-05,
+      2.360273276062563e-05, 1.8741145010900324e-05, 1.4667715927237253e-05,
+      1.1319376641756088e-05, 8.617131239081784e-06, 6.474342896121373e-06,
+      4.803534042634537e-06, 3.5214801860769927e-06, 2.5526421608945726e-06,
+      1.831191172261092e-06, 1.3019762862645152e-06, 9.198343846200812e-07,
+      6.457557667963472e-07, 4.460352713792651e-07, 2.991961294681659e-07,
+      1.9512183243798884e-07, 1.2497528598414674e-07, 7.909407148948912e-08,
+      4.9524358482359656e-08, 3.068335892462088e-08, 1.881038173874779e-08,
+      1.1410455688353013e-08, 6.848871830823477e-09, 4.0676704431111005e-09,
+      2.3904691934473904e-09, 1.3900525325056631e-09, 7.99815738996755e-10,
+      4.5536468791909334e-10, 2.565307456198365e-10, 1.4299806741586598e-10,
+      7.887358543435692e-11, 4.304707722047644e-11, 2.324697379012706e-11,
+      1.242223821392642e-11, 6.5681634397905525e-12, 3.436360510192299e-12,
+      1.7790856695225406e-12, 9.575396427362875e-13]
+    - [5.4748158484612686e-05, 5.186114341183571e-05, 4.825339972682457e-05,
+      4.422931072212073e-05, 3.9931571971377834e-05, 3.550512098118485e-05,
+      3.108837314463146e-05, 2.680537669938155e-05, 2.275980239135444e-05,
+      1.903116787007715e-05, 1.567340170823184e-05, 1.2715574436399973e-05,
+      1.0164404186539982e-05, 8.008007836135697e-06, 6.22032269393813e-06,
+      4.765660033295508e-06, 3.602950433213857e-06, 2.68939333233367e-06,
+      1.9833869650964156e-06, 1.4467356367739543e-06, 1.0458902564358082e-06,
+      7.5040077978203e-07, 5.320391016665224e-07, 3.6893339878434155e-07,
+      2.4866704889947387e-07, 1.6385727544153498e-07, 1.064129881231693e-07,
+      6.833512440309911e-08, 4.341908563365454e-08, 2.729778905066431e-08,
+      1.698184776583731e-08, 1.04532920453759e-08, 6.366956683117353e-09,
+      3.83726133024166e-09, 2.2883451508261197e-09, 1.350306483198659e-09,
+      7.884131270587521e-10, 4.554975140967764e-10, 2.6039272484431753e-10,
+      1.4729308282504928e-10, 8.244162212458523e-11, 4.565847221687755e-11,
+      2.502112848858511e-11, 1.3567601567898642e-11, 7.279640631899349e-12,
+      3.864803964551966e-12, 2.03027875534096e-12, 1.0553452046662258e-12,
+      5.42846569508216e-13, 2.9041983287660447e-13]
+    - [2.5766954475506383e-05, 2.415901630772594e-05, 2.2233976095877203e-05,
+      2.0161031187987884e-05, 1.8009184207567182e-05, 1.5845514729127568e-05,
+      1.3731432544283954e-05, 1.1719535999131475e-05, 9.85145838611892e-06,
+      8.156805106075528e-06, 6.653149867895632e-06, 5.34694320562681e-06,
+      4.235106093660203e-06, 3.3070455767186147e-06, 2.5468496242273237e-06,
+      1.9354481178259733e-06, 1.4526444688728217e-06, 1.078435624333363e-06,
+      7.929065763732273e-07, 5.760089766620136e-07, 4.104097868010723e-07,
+      2.8487426282297836e-07, 1.930946174277554e-07, 1.2873915449636274e-07,
+      8.479841601409634e-08, 5.5256312314165674e-08, 3.5627130914295854e-08,
+      2.27295276215754e-08, 1.4348636749523216e-08, 8.962755367977951e-09,
+      5.5396600601533636e-09, 3.3879372520070344e-09, 2.0502096427089075e-09,
+      1.2276423335649542e-09, 7.273712161744129e-10, 4.264332266721992e-10,
+      2.4737547022007384e-10, 1.4199495014669187e-10, 8.06491579010282e-11,
+      4.532496163702313e-11, 2.5204943250194e-11, 1.386898483731261e-11,
+      7.551170794965409e-12, 4.06812776523674e-12, 2.168630419839769e-12,
+      1.1438976753002006e-12, 5.970345717393097e-13, 3.083347356891418e-13,
+      1.5757576510332265e-13, 8.379688405208405e-14]
+    - [1.1932018223997563e-05, 1.105715542181504e-05, 1.0049779879888807e-05,
+      9.00104373609326e-06, 7.942955364548063e-06, 6.905130840465538e-06,
+      5.91332769074613e-06, 4.988327791788423e-06, 4.145317529097556e-06,
+      3.393768965665962e-06, 2.737780179659064e-06, 2.1767727226864956e-06,
+      1.706470441963911e-06, 1.319975424300001e-06, 1.0084862031195585e-06,
+      7.613606734423304e-07, 5.666352729179837e-07, 4.1337669359940475e-07,
+      2.942071560668048e-07, 2.0472548603735954e-07, 1.4006901653047745e-07,
+      9.463536454617879e-08, 6.324280636451207e-08, 4.181794450577018e-08,
+      2.7360519174833845e-08, 1.7713184877871204e-08, 1.1346963233694359e-08,
+      7.1923913567534415e-09, 4.5110500321923855e-09, 2.799578489580521e-09,
+      1.7191680156050004e-09, 1.0446111763209557e-09, 6.280607942275544e-10,
+      3.7364516833591536e-10, 2.199519051200038e-10, 1.2811699860794268e-10,
+      7.384081041193146e-11, 4.211112305329721e-11, 2.3763360886016847e-11,
+      1.3268736634064827e-11, 7.3309786577122e-12, 4.007790458032906e-12,
+      2.167997261878878e-12, 1.1604411544234246e-12, 6.146079677435958e-13,
+      3.220949535072878e-13, 1.6702455581115267e-13, 8.570129828528219e-14,
+      4.351497987467397e-14, 2.300204794139991e-14]
+    - [5.443457457424846e-06, 4.977620323736194e-06, 4.4602656244062905e-06,
+      3.939043703301332e-06, 3.428033888955824e-06, 2.9395133689779882e-06,
+      2.483469754635834e-06, 2.067290557486438e-06, 1.6956985994279696e-06,
+      1.3709531348359162e-06, 1.0931203066412716e-06, 8.595612372581245e-07,
+      6.659393799211406e-07, 5.067017816160229e-07, 3.7719228502861773e-07,
+      2.7428802769944274e-07, 1.9543140791791483e-07, 1.3708745996182588e-07,
+      9.498610475025433e-08, 6.509909720795478e-08, 4.4144758953938946e-08,
+      2.9620534868694996e-08, 1.9666057671960694e-08, 1.2919698861121842e-08,
+      8.398430725025769e-09, 5.401999854343292e-09, 3.4381250029283294e-09,
+      2.1652070266994973e-09, 1.3492358235928646e-09, 8.319303534771706e-10,
+      5.075709373498856e-10, 3.064200611446328e-10, 1.8304097196868327e-10,
+      1.0819074274228932e-10, 6.327651643923104e-11, 3.6618933550855025e-11,
+      2.09690856290848e-11, 1.188130007953439e-11, 6.661301746831667e-12,
+      3.695429486870442e-12, 2.0285298527142744e-12, 1.1018146878922634e-12,
+      5.921699734450372e-13, 3.1491610966308065e-13, 1.6571203239005228e-13,
+      8.628273053755222e-14, 4.4453339040670634e-14, 2.2661860710328692e-14,
+      1.1432240877100302e-14, 6.0068716947424355e-15]
+    - [2.4496215635099416e-06, 2.2064850261678994e-06, 1.94556006509165e-06,
+      1.691040728162999e-06, 1.4486958742546425e-06, 1.2231442756374475e-06,
+      1.0176281924679516e-06, 8.338896301984762e-07, 6.71809683839665e-07,
+      5.312281541640344e-07, 4.1127994349590435e-07, 3.1112862588103396e-07,
+      2.305328153878684e-07, 1.6793181946823847e-07, 1.206911583100276e-07,
+      8.574613733435245e-08, 6.026610600767018e-08, 4.1911096795204233e-08,
+      2.8839973778311275e-08, 1.9636829241210086e-08, 1.3229960167535276e-08,
+      8.819752138192404e-09, 5.817881814125823e-09, 3.797380182548488e-09,
+      2.4525277791064196e-09, 1.5673084009428134e-09, 9.910730311060383e-10,
+      6.201082736984809e-10, 3.8391940519023437e-10, 2.351923940614221e-10,
+      1.4256638987095086e-10, 8.551094431160776e-11, 5.075010243677573e-11,
+      2.9803194328378204e-11, 1.7318065448600247e-11, 9.957415033509501e-12,
+      5.665059982226365e-12, 3.1891363414505647e-12, 1.7764473117151432e-12,
+      9.791342589122086e-13, 5.340019368425066e-13, 2.8817353151844656e-13,
+      1.5387781678166156e-13, 8.130338242464741e-14, 4.250616093081116e-14,
+      2.1989017313985945e-14, 1.1255646136476138e-14, 5.700930037599512e-15,
+      2.8573663545334937e-15, 1.4923551466706648e-15]
+    - [1.087861503713364e-06, 9.62341091173932e-07, 8.312136048455606e-07,
+      7.059725607564541e-07, 5.885947743247368e-07, 4.807166555271372e-07,
+      3.8417540924794667e-07, 3.005471871750907e-07, 2.3060130072434527e-07,
+      1.741416044726682e-07, 1.2975576888135644e-07, 9.555898654777408e-08,
+      6.961290852110711e-08, 5.017531666493626e-08, 3.578470742402119e-08,
+      2.5253140385416835e-08, 1.763372184309723e-08, 1.2183813691479006e-08,
+      8.329773329405286e-09, 5.634998285914941e-09, 3.77194250015053e-09,
+      2.498313931414287e-09, 1.6373428454263339e-09, 1.0618004713115005e-09,
+      6.813289955638781e-10, 4.3259500487297925e-10, 2.7177956528419686e-10,
+      1.689517791765185e-10, 1.0392485089899235e-10, 6.325381459677211e-11,
+      3.8094712746005185e-11, 2.270143735025527e-11, 1.3386057269134208e-11,
+      7.810209301542105e-12, 4.5090322014532056e-12, 2.5758150234180964e-12,
+      1.455984251724763e-12, 8.143467245251571e-13, 4.506845818136243e-13,
+      2.4680088827546206e-13, 1.3373078893580505e-13, 7.170125637432221e-14,
+      3.803932440926498e-14, 1.9968686339121325e-14, 1.037234290959478e-14,
+      5.331076413387241e-15, 2.711212884040865e-15, 1.3643412262686617e-15,
+      6.794032692780127e-16, 3.527143794294186e-16]
+    - [4.4424533837495745e-07, 3.754064128434521e-07, 3.0747799807708793e-07,
+      2.4736950904213035e-07, 1.9590784608881845e-07, 1.5303801737200708e-07,
+      1.1811071980396466e-07, 9.014021773194039e-08, 6.805681114675265e-08,
+      5.0841008261358886e-08, 3.758058918279215e-08, 2.7486758061930803e-08,
+      1.989271796478036e-08, 1.4245424702310884e-08, 1.0094094083043022e-08,
+      7.07733846583376e-09, 4.910019917503887e-09, 3.370599969938962e-09,
+      2.289506294951538e-09, 1.5388175898045326e-09, 1.0233945801112333e-09,
+      6.734568178431898e-10, 4.385176376688009e-10, 2.825368171693259e-10,
+      1.8012487882842028e-10, 1.1362738853616937e-10, 7.092560026356598e-11,
+      4.380600871147651e-11, 2.6771642749114498e-11, 1.6189261100043315e-11,
+      9.687009028017677e-12, 5.735391286686155e-12, 3.360060293850362e-12,
+      1.9477883304038005e-12, 1.1172416542939397e-12, 6.341078790125243e-13,
+      3.5611465833725456e-13, 1.978915371551571e-13, 1.0881161699424765e-13,
+      5.920167262603012e-14, 3.18715628875104e-14, 1.6977878240615262e-14,
+      8.948992403487105e-15, 4.667405512892602e-15, 2.4087271116025935e-15,
+      1.230014801499113e-15, 6.215037378698824e-16, 3.1073331833664504e-16,
+      1.537366666472916e-16, 7.933463260520683e-17]
+    - [1.53316416018928e-07, 1.2580538188545112e-07, 1.0061723316018172e-07,
+      7.961231485612813e-08, 6.232712179609306e-08, 4.828127832466909e-08,
+      3.700756458686311e-08, 2.8068093636588214e-08, 2.1064249889832525e-08,
+      1.5641908838309066e-08, 1.149328492731912e-08, 8.356208482293265e-09,
+      6.0115301689683965e-09, 4.279287505951721e-09, 3.014175747827078e-09,
+      2.100759553472119e-09, 1.448754486628304e-09, 9.88607523674168e-10,
+      6.675191037007882e-10, 4.4597874174637273e-10, 2.948324539459176e-10,
+      1.92862186938313e-10, 1.248330431131211e-10, 7.9950778850508e-11,
+      5.0667154028352956e-11, 3.1771739506710725e-11, 1.9713609352970477e-11,
+      1.210324905364564e-11, 7.352727391587988e-12, 4.419830652327965e-12,
+      2.6288963605817606e-12, 1.5472196468265698e-12, 9.010339363915446e-13,
+      5.192075464266408e-13, 2.960407626478222e-13, 1.6702162442516833e-13,
+      9.324049335223192e-14, 5.1504727405885485e-14, 2.815141919486103e-14,
+      1.5225240630233132e-14, 8.147768993869074e-15, 4.314434897462134e-15,
+      2.260579596781518e-15, 1.1719966154827597e-15, 6.012340693180426e-16,
+      3.05190828013293e-16, 1.5328866553629014e-16, 7.618321214530511e-17,
+      3.7467469626157364e-17, 1.922799232706676e-17]
+    central_value: [3.830002095779685e-09, 3.68000240312462e-11]
+
+
+# This is a Gaussian distribution fitted to the numerical combination of
+# 'ATLAS Bs->mumu 2018', 'LHCb Bs->mumu 2021', and 'CMS Bs->mumu 2022'
+GSSS combination Bs->mumu 2022:
+  inspire: Greljo:2022jac
+  observables:
+    - BR(Bs->mumu)
+    - BR(B0->mumu)
+  values:
+    distribution: multivariate_normal
+    central_value: [3.3608448878336465e-09, 4.2458612570356666e-11]
+    standard_deviation: [2.8087080557123625e-10, 5.402626138662697e-11]
+    correlation:
+    - [1.0, -0.17763283049964992]
+    - [-0.17763283049964992, 1.0]
+
+
 # This is a Gaussian distribution fitted to the numerical combination of
 # 'ATLAS Bs->mumu 2018', 'CMS Bs->mumu 2019', and 'LHCb Bs->mumu 2021'
 AS combination Bs->mumu 2021:
   inspire: Altmannshofer:2021qrr
   observables:
     - BR(Bs->mumu)
     - BR(B0->mumu)
@@ -9863,14 +10882,23 @@
   url: https://indico.cern.ch/event/976688/attachments/2213706/3747159/santimaria_LHC_seminar_2021.pdf
   values:
     # to convert numbers from picoseconds to 1/GeV, multiply by
     # ps = 1.519267447878626e+12 [1/GeV],
     tau_mumu: (3.14 ± 0.44 ± 0.05) 1e12 # this is 2.07 ± 0.29 ± 0.03 ps
 
 
+CMS Bs->mumu effective lifetime 2022:
+  experiment: CMS
+  url: http://cds.cern.ch/record/2815334/
+  values:
+    # to convert numbers from picoseconds to 1/GeV, multiply by
+    # ps = 1.519267447878626e+12 [1/GeV],
+    tau_mumu: (2.78 +0.35 -0.30 ± 0.06) 1e12 # this is 1.83 +0.23 -0.20 ± 0.04 ps
+
+
 Bc lifetime:
   experiment: PDG
   inspire: Tanabashi:2018oca
   values:
     tau_Bc: (7.704 ± 0.137) 1e11
 
 
@@ -10310,14 +11338,40 @@
             0.0004599, 0.0004375, 0.0004162, 0.0003960, 0.0003767, 0.0003584, 0.0003409, 0.0003238, 0.0003071, 0.0002913, 0.0002763, 0.0002621, 0.0002486,
             0.0002358, 0.0002237, 0.0002122, 0.0002012, 0.0001909, 0.0001811, 0.0001718, 0.0001627, 0.0001539, 0.0001455, 0.0001376, 0.0001301, 0.0001231,
             0.0001164, 0.0001101, 0.0001041, 0.0000984, 0.0000931, 0.0000880, 0.0000832, 0.0000787, 0.0000742, 0.0000699, 0.0000659, 0.0000621, 0.0000586,
             0.0000552, 0.0000521, 0.0000491, 0.0000463, 0.0000436, 0.0000411, 0.0000388, 0.0000365, 0.0000343, 0.0000323, 0.0000303, 0.0000285, 0.0000268,
             0.0000252, 0.0000237, 0.0000222, 0.0000209, 0.0000196, 0.0000185, 0.0000174, 0.0000163, 0.0000153, 0.0000143, 0.0000134, 0.0000126]
 
 
+LHCb RK RK* 2022:
+  experiment: LHCb
+  inspire: LHCb:2022zom
+  values:
+    - name: <Rmue>(B+->Kll) # RK cental-q^2
+      q2min: 1.1
+      q2max: 6.0
+      value: 0.949 +0.042 -0.041 +0.022 -0.022
+    - name: <Rmue>(B+->Kll) # RK low-q^2
+      q2min: 0.1
+      q2max: 1.1
+      value: 0.994 +0.090 -0.082 +0.029 -0.027
+    - name: <Rmue>(B0->K*ll) # RK* cental-q^2
+      q2min: 1.1
+      q2max: 6.0
+      value: 1.027 +0.072 -0.068 +0.027 -0.026
+    - name: <Rmue>(B0->K*ll) # RK* low-q^2
+      q2min: 0.1
+      q2max: 1.1
+      value: 0.927 +0.093 -0.087 +0.036 -0.035
+  correlation: [[1.000, 0.015, -0.017, 0.005],
+                [0.015, 1.000, 0.004, -0.033],
+                [-0.017, 0.004, 1.000, 0.016],
+                [0.005, -0.033, 0.016, 1.000]]
+
+
 Belle B->K*mumu LFU 2016:
    experiment: Belle
    inspire: Wehle:2016yoi
    description: >
     This measurement actually performs an isospin-combined analysis
     (with unkown weights of the two isospin states), but since the isospin
     asymmetry in the lepton flavour difference should be very small,
@@ -13993,7 +15047,7285 @@
       thetamax: 0.8
       value: 4.481 ± 0.187
     - name: <dR/dtheta>(ee->WW)
       E: 205.92
       thetamin: 0.8
       thetamax: 1.0
       value: 7.584 ± 0.26
+
+ATLAS pp->ee 2016:
+  experiment: ATLAS
+  inspire: ATLAS:2017fih
+  values:
+  - name: R_13(pp->ee)
+    qmax: 85.54876
+    qmin: 80.0
+    value:
+      background_std: 69401.5708
+      counts_background: 10974.128946591254
+      counts_total: 1176847.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.079216742641075e-07
+  - name: R_13(pp->ee)
+    qmax: 91.48239
+    qmin: 85.54876
+    value:
+      background_std: 362245.73273
+      counts_background: 20197.544340420172
+      counts_total: 6608874.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.578288016852957e-07
+  - name: R_13(pp->ee)
+    qmax: 97.82756
+    qmin: 91.48239
+    value:
+      background_std: 236917.40941
+      counts_background: 14758.751538861532
+      counts_total: 3928394.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.6643422884378354e-07
+  - name: R_13(pp->ee)
+    qmax: 104.61284
+    qmin: 97.82756
+    value:
+      background_std: 25907.27369
+      counts_background: 8303.474996545438
+      counts_total: 432217.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.433985942583826e-06
+  - name: R_13(pp->ee)
+    qmax: 111.86874
+    qmin: 104.61284
+    value:
+      background_std: 8629.47379
+      counts_background: 7744.303026077903
+      counts_total: 162962.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.658077258351981e-06
+  - name: R_13(pp->ee)
+    qmax: 119.6279
+    qmin: 111.86874
+    value:
+      background_std: 4855.99299
+      counts_background: 7479.00056482295
+      counts_total: 93773.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2056724982029082e-05
+  - name: R_13(pp->ee)
+    qmax: 127.92524
+    qmin: 119.6279
+    value:
+      background_std: 3290.32109
+      counts_background: 7349.777298742665
+      counts_total: 63446.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.806483692003574e-05
+  - name: R_13(pp->ee)
+    qmax: 136.79808
+    qmin: 127.92524
+    value:
+      background_std: 2472.545
+      counts_background: 7097.990404497162
+      counts_total: 47190.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.529845178476055e-05
+  - name: R_13(pp->ee)
+    qmax: 146.28633
+    qmin: 136.79808
+    value:
+      background_std: 1906.07197
+      counts_background: 6619.998084113988
+      counts_total: 36539.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.415359516648235e-05
+  - name: R_13(pp->ee)
+    qmax: 156.43268
+    qmin: 146.28633
+    value:
+      background_std: 1531.96354
+      counts_background: 6282.7489410602875
+      counts_total: 29267.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.3779840768871884e-05
+  - name: R_13(pp->ee)
+    qmax: 167.28278
+    qmin: 156.43268
+    value:
+      background_std: 1260.16032
+      counts_background: 5859.656548202215
+      counts_total: 23874.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.628054175473133e-05
+  - name: R_13(pp->ee)
+    qmax: 178.88544
+    qmin: 167.28278
+    value:
+      background_std: 1052.39276
+      counts_background: 5277.835442619564
+      counts_total: 19689.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.028500277716987e-05
+  - name: R_13(pp->ee)
+    qmax: 191.29285
+    qmin: 178.88544
+    value:
+      background_std: 883.33112
+      counts_background: 4837.365635368392
+      counts_total: 16548.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.65923086594022e-05
+  - name: R_13(pp->ee)
+    qmax: 204.56084
+    qmin: 191.29285
+    value:
+      background_std: 742.04396
+      counts_background: 4281.768795274276
+      counts_total: 13671.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001081634337384418
+  - name: R_13(pp->ee)
+    qmax: 218.74908
+    qmin: 204.56084
+    value:
+      background_std: 627.82514
+      counts_background: 3856.6204211634854
+      counts_total: 11337.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001297591712669735
+  - name: R_13(pp->ee)
+    qmax: 233.92142
+    qmin: 218.74908
+    value:
+      background_std: 525.82479
+      counts_background: 3296.722728086122
+      counts_total: 9358.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001600221396184068
+  - name: R_13(pp->ee)
+    qmax: 250.1461
+    qmin: 233.92142
+    value:
+      background_std: 444.71135
+      counts_background: 2818.1100442860775
+      counts_total: 7877.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001975366089958675
+  - name: R_13(pp->ee)
+    qmax: 267.49612
+    qmin: 250.1461
+    value:
+      background_std: 367.66547
+      counts_background: 2408.9815482652252
+      counts_total: 6434.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00023747235174379153
+  - name: R_13(pp->ee)
+    qmax: 286.04953
+    qmin: 267.49612
+    value:
+      background_std: 314.24861
+      counts_background: 2059.2496420247057
+      counts_total: 5500.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0002936162223584367
+  - name: R_13(pp->ee)
+    qmax: 305.8898
+    qmin: 286.04953
+    value:
+      background_std: 258.88905
+      counts_background: 1699.9875967186451
+      counts_total: 4445.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003556667718937045
+  - name: R_13(pp->ee)
+    qmax: 327.10617
+    qmin: 305.8898
+    value:
+      background_std: 217.35737
+      counts_background: 1428.07788026321
+      counts_total: 3648.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0004480144439399666
+  - name: R_13(pp->ee)
+    qmax: 349.79411
+    qmin: 327.10617
+    value:
+      background_std: 181.52639
+      counts_background: 1138.5441438965217
+      counts_total: 2981.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005310545963681227
+  - name: R_13(pp->ee)
+    qmax: 374.05567
+    qmin: 349.79411
+    value:
+      background_std: 155.1601
+      counts_background: 907.7115369661385
+      counts_total: 2431.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006661026947009184
+  - name: R_13(pp->ee)
+    qmax: 400.0
+    qmin: 374.05567
+    value:
+      background_std: 128.64381
+      counts_background: 736.4024468642822
+      counts_total: 1964.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000821057973610578
+  - name: R_13(pp->ee)
+    qmax: 427.74382
+    qmin: 400.0
+    value:
+      background_std: 103.29922
+      counts_background: 576.9574935153886
+      counts_total: 1606.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0010192069080174118
+  - name: R_13(pp->ee)
+    qmax: 457.41193
+    qmin: 427.74382
+    value:
+      background_std: 85.46347
+      counts_background: 459.98301955218915
+      counts_total: 1231.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012436687644054158
+  - name: R_13(pp->ee)
+    qmax: 489.13782
+    qmin: 457.41193
+    value:
+      background_std: 73.72079
+      counts_background: 366.72437857973097
+      counts_total: 1013.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0015599358727921824
+  - name: R_13(pp->ee)
+    qmax: 523.06419
+    qmin: 489.13782
+    value:
+      background_std: 55.19929
+      counts_background: 282.35728074374333
+      counts_total: 776.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0019190218064174967
+  - name: R_13(pp->ee)
+    qmax: 559.34369
+    qmin: 523.06419
+    value:
+      background_std: 48.80979
+      counts_background: 209.95171574856192
+      counts_total: 622.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0023835569428771767
+  - name: R_13(pp->ee)
+    qmax: 598.13951
+    qmin: 559.34369
+    value:
+      background_std: 35.32162
+      counts_background: 167.3853364513252
+      counts_total: 464.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00306926940947003
+  - name: R_13(pp->ee)
+    qmax: 639.6262
+    qmin: 598.13951
+    value:
+      background_std: 30.02474
+      counts_background: 128.87735639450338
+      counts_total: 403.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003783205685801885
+  - name: R_13(pp->ee)
+    qmax: 683.99038
+    qmin: 639.6262
+    value:
+      background_std: 24.61983
+      counts_background: 95.82902209885535
+      counts_total: 300.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0048328867938694006
+  - name: R_13(pp->ee)
+    qmax: 731.43164
+    qmin: 683.99038
+    value:
+      background_std: 18.49127
+      counts_background: 71.25535263396021
+      counts_total: 219.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0061788985279947065
+  - name: R_13(pp->ee)
+    qmax: 782.16341
+    qmin: 731.43164
+    value:
+      background_std: 14.79304
+      counts_background: 52.98316906283727
+      counts_total: 202.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00771345682841781
+  - name: R_13(pp->ee)
+    qmax: 836.4139
+    qmin: 782.16341
+    value:
+      background_std: 11.664
+      counts_background: 42.24116744281099
+      counts_total: 133.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.010165575952204128
+  - name: R_13(pp->ee)
+    qmax: 894.42719
+    qmin: 836.4139
+    value:
+      background_std: 9.52662
+      counts_background: 25.929437974046724
+      counts_total: 107.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01242797370580426
+  - name: R_13(pp->ee)
+    qmax: 956.46425
+    qmin: 894.42719
+    value:
+      background_std: 7.02936
+      counts_background: 22.951305889412726
+      counts_total: 82.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.016162595737660334
+  - name: R_13(pp->ee)
+    qmax: 1022.80418
+    qmin: 956.46425
+    value:
+      background_std: 6.42159
+      counts_background: 16.196444247816817
+      counts_total: 57.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.020840379028760656
+  - name: R_13(pp->ee)
+    qmax: 1093.74541
+    qmin: 1022.80418
+    value:
+      background_std: 4.58922
+      counts_background: 11.835067295194715
+      counts_total: 43.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.027865041812088247
+  - name: R_13(pp->ee)
+    qmax: 1169.6071
+    qmin: 1093.74541
+    value:
+      background_std: 4.072
+      counts_background: 10.116872048488071
+      counts_total: 27.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.035803723505292595
+  - name: R_13(pp->ee)
+    qmax: 1250.73051
+    qmin: 1169.6071
+    value:
+      background_std: 3.55774
+      counts_background: 7.015993056428879
+      counts_total: 24.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04593082843097357
+  - name: R_13(pp->ee)
+    qmax: 1337.48061
+    qmin: 1250.73051
+    value:
+      background_std: 2.4616
+      counts_background: 4.698868287883057
+      counts_total: 12.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.06403541056796183
+  - name: R_13(pp->ee)
+    qmax: 1430.24766
+    qmin: 1337.48061
+    value:
+      background_std: 1.81931
+      counts_background: 3.3159315038208375
+      counts_total: 13.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.08673919266016257
+  - name: R_13(pp->ee)
+    qmax: 1529.44898
+    qmin: 1430.24766
+    value:
+      background_std: 1.46459
+      counts_background: 2.259847110480091
+      counts_total: 11.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.11145420943657515
+  - name: R_13(pp->ee)
+    qmax: 1635.53087
+    qmin: 1529.44898
+    value:
+      background_std: 1.08804
+      counts_background: 1.898388951473906
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.15849963717169402
+  - name: R_13(pp->ee)
+    qmax: 1748.97054
+    qmin: 1635.53087
+    value:
+      background_std: 0.93005
+      counts_background: 1.3632228684915886
+      counts_total: 7.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.21578697195602808
+  - name: R_13(pp->ee)
+    qmax: 1870.27835
+    qmin: 1748.97054
+    value:
+      background_std: 0.63117
+      counts_background: 0.7406931897077118
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.29880872349382903
+  - name: R_13(pp->ee)
+    qmax: 2000.0
+    qmin: 1870.27835
+    value:
+      background_std: 0.48462
+      counts_background: 0.5507554316034936
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.42852039805782594
+  - name: R_13(pp->ee)
+    qmax: 2138.71909
+    qmin: 2000.0
+    value:
+      background_std: 0.36813
+      counts_background: 0.40244806183924986
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.6123650966362543
+  - name: R_13(pp->ee)
+    qmax: 2287.05967
+    qmin: 2138.71909
+    value:
+      background_std: 0.28204
+      counts_background: 0.2840024714771532
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.8677570480195347
+  - name: R_13(pp->ee)
+    qmax: 2445.68909
+    qmin: 2287.05967
+    value:
+      background_std: 0.21388
+      counts_background: 0.20394064320970548
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2903519721722103
+  - name: R_13(pp->ee)
+    qmax: 2615.32097
+    qmin: 2445.68909
+    value:
+      background_std: 0.16619
+      counts_background: 0.1365865406765846
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.926655509892617
+  - name: R_13(pp->ee)
+    qmax: 2796.71844
+    qmin: 2615.32097
+    value:
+      background_std: 0.13146
+      counts_background: 0.09808205828100346
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.9324549932851895
+  - name: R_13(pp->ee)
+    qmax: 2990.69756
+    qmin: 2796.71844
+    value:
+      background_std: 0.10401
+      counts_background: 0.06343879426969366
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.533838085494976
+  - name: R_13(pp->ee)
+    qmax: 3198.13098
+    qmin: 2990.69756
+    value:
+      background_std: 0.08242
+      counts_background: 0.0424872909961412
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.081975644121295
+  - name: R_13(pp->ee)
+    qmax: 3419.95189
+    qmin: 3198.13098
+    value:
+      background_std: 0.06515
+      counts_background: 0.027480484808533566
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 11.46009601807493
+  - name: R_13(pp->ee)
+    qmax: 3657.1582
+    qmin: 3419.95189
+    value:
+      background_std: 0.05132
+      counts_background: 0.016290814897373034
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 19.33169068048448
+  - name: R_13(pp->ee)
+    qmax: 3910.81703
+    qmin: 3657.1582
+    value:
+      background_std: 0.03987
+      counts_background: 0.010175819294691284
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 32.40865776788391
+  - name: R_13(pp->ee)
+    qmax: 4182.06952
+    qmin: 3910.81703
+    value:
+      background_std: 0.03073
+      counts_background: 0.005626136448385503
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 57.27738321032179
+  - name: R_13(pp->ee)
+    qmax: 4472.13595
+    qmin: 4182.06952
+    value:
+      background_std: 0.02337
+      counts_background: 0.0032209939381416005
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 104.79375109828433
+  - name: R_13(pp->ee)
+    qmax: 4782.32127
+    qmin: 4472.13595
+    value:
+      background_std: 0.01745
+      counts_background: 0.0018764583977886877
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 207.42976237268493
+  - name: R_13(pp->ee)
+    qmax: 5114.0209
+    qmin: 4782.32127
+    value:
+      background_std: 0.01197
+      counts_background: 0.0019430219749753776
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 393.32125134990633
+
+ATLAS pp->ee 2019:
+  experiment: ATLAS
+  inspire: ATLAS:2019erb
+  values:
+  - name: R_13(pp->ee)
+    qmax: 135.0803
+    qmin: 130.0015
+    value:
+      background_std: 5000.588854114147
+      counts_background: 13446.903379204288
+      counts_total: 97949.09608780447
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2332693238148677e-05
+  - name: R_13(pp->ee)
+    qmax: 140.3576
+    qmin: 135.0803
+    value:
+      background_std: 4357.6509582467115
+      counts_background: 13228.252576729941
+      counts_total: 84590.46700920945
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4446251442417394e-05
+  - name: R_13(pp->ee)
+    qmax: 145.841
+    qmin: 140.3576
+    value:
+      background_std: 3809.8769400757465
+      counts_background: 12880.255464655524
+      counts_total: 73677.58736496375
+      distribution: general_gamma_counting_process
+      scale_factor: 1.687832468956729e-05
+  - name: R_13(pp->ee)
+    qmax: 151.5373
+    qmin: 145.841
+    value:
+      background_std: 3357.8139815115555
+      counts_background: 12377.245762429153
+      counts_total: 65298.2717265786
+      distribution: general_gamma_counting_process
+      scale_factor: 1.95402439647497e-05
+  - name: R_13(pp->ee)
+    qmax: 157.4575
+    qmin: 151.5373
+    value:
+      background_std: 2993.0645235757147
+      counts_background: 11990.855921203432
+      counts_total: 57173.48475062844
+      distribution: general_gamma_counting_process
+      scale_factor: 2.2433067165504817e-05
+  - name: R_13(pp->ee)
+    qmax: 163.609
+    qmin: 157.4575
+    value:
+      background_std: 2656.6060408763883
+      counts_background: 11430.266588630146
+      counts_total: 51011.969305676175
+      distribution: general_gamma_counting_process
+      scale_factor: 2.5872912924585207e-05
+  - name: R_13(pp->ee)
+    qmax: 170.0008
+    qmin: 163.609
+    value:
+      background_std: 2412.4247016848776
+      counts_background: 10905.906649282797
+      counts_total: 45817.07724602184
+      distribution: general_gamma_counting_process
+      scale_factor: 2.9184567585936974e-05
+  - name: R_13(pp->ee)
+    qmax: 176.6408
+    qmin: 170.0008
+    value:
+      background_std: 2181.797292029745
+      counts_background: 10287.502279210825
+      counts_total: 41014.31123306121
+      distribution: general_gamma_counting_process
+      scale_factor: 3.306245838643729e-05
+  - name: R_13(pp->ee)
+    qmax: 183.5417
+    qmin: 176.6408
+    value:
+      background_std: 1954.1188631227808
+      counts_background: 9757.089561424931
+      counts_total: 37157.82096625343
+      distribution: general_gamma_counting_process
+      scale_factor: 3.768318673487399e-05
+  - name: R_13(pp->ee)
+    qmax: 190.7122
+    qmin: 183.5417
+    value:
+      background_std: 1760.8803060321534
+      counts_background: 9231.366523721455
+      counts_total: 33242.380659475326
+      distribution: general_gamma_counting_process
+      scale_factor: 4.2741138263125134e-05
+  - name: R_13(pp->ee)
+    qmax: 198.1629
+    qmin: 190.7122
+    value:
+      background_std: 1602.9072476828815
+      counts_background: 8643.446763401971
+      counts_total: 30091.30081059541
+      distribution: general_gamma_counting_process
+      scale_factor: 4.80112479990445e-05
+  - name: R_13(pp->ee)
+    qmax: 205.9028
+    qmin: 198.1629
+    value:
+      background_std: 1453.4497184562108
+      counts_background: 8112.2121914010795
+      counts_total: 26905.019843905644
+      distribution: general_gamma_counting_process
+      scale_factor: 5.4099701415806044e-05
+  - name: R_13(pp->ee)
+    qmax: 213.9394
+    qmin: 205.9028
+    value:
+      background_std: 1312.0100412543106
+      counts_background: 7545.11334688143
+      counts_total: 24242.977217540498
+      distribution: general_gamma_counting_process
+      scale_factor: 6.0928725802191565e-05
+  - name: R_13(pp->ee)
+    qmax: 222.2975
+    qmin: 213.9394
+    value:
+      background_std: 1190.0446190750324
+      counts_background: 7003.694784802399
+      counts_total: 21812.55089957259
+      distribution: general_gamma_counting_process
+      scale_factor: 6.84071111037318e-05
+  - name: R_13(pp->ee)
+    qmax: 230.9902
+    qmin: 222.2975
+    value:
+      background_std: 1078.9245274849386
+      counts_background: 6400.317969534015
+      counts_total: 19791.862964624223
+      distribution: general_gamma_counting_process
+      scale_factor: 7.643854201559559e-05
+  - name: R_13(pp->ee)
+    qmax: 240.0039
+    qmin: 230.9902
+    value:
+      background_std: 981.7354664069255
+      counts_background: 5924.685059029112
+      counts_total: 17807.673308411715
+      distribution: general_gamma_counting_process
+      scale_factor: 8.62407749068593e-05
+  - name: R_13(pp->ee)
+    qmax: 249.3802
+    qmin: 240.0039
+    value:
+      background_std: 889.2823126646324
+      counts_background: 5395.220298379147
+      counts_total: 16295.976158627765
+      distribution: general_gamma_counting_process
+      scale_factor: 9.649122883371949e-05
+  - name: R_13(pp->ee)
+    qmax: 259.1229
+    qmin: 249.3802
+    value:
+      background_std: 793.7255297662615
+      counts_background: 4950.853869576408
+      counts_total: 14289.667537147046
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001087606655189842
+  - name: R_13(pp->ee)
+    qmax: 269.2462
+    qmin: 259.1229
+    value:
+      background_std: 719.3740771806467
+      counts_background: 4512.562837037432
+      counts_total: 13037.604152525233
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00012179109660095017
+  - name: R_13(pp->ee)
+    qmax: 279.7625
+    qmin: 269.2462
+    value:
+      background_std: 653.7372273056299
+      counts_background: 4052.707722521289
+      counts_total: 11562.813282279834
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00013724979684923984
+  - name: R_13(pp->ee)
+    qmax: 290.6922
+    qmin: 279.7625
+    value:
+      background_std: 589.656565522517
+      counts_background: 3686.0131077455826
+      counts_total: 10185.167926541993
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001537646079277784
+  - name: R_13(pp->ee)
+    qmax: 302.0488
+    qmin: 290.6922
+    value:
+      background_std: 524.1327408624023
+      counts_background: 3270.059670600919
+      counts_total: 9218.998992379236
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00017274238659341256
+  - name: R_13(pp->ee)
+    qmax: 313.8491
+    qmin: 302.0488
+    value:
+      background_std: 474.78876252421395
+      counts_background: 2949.4485567879747
+      counts_total: 8103.516491866462
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00019444276945669583
+  - name: R_13(pp->ee)
+    qmax: 326.1076
+    qmin: 313.8491
+    value:
+      background_std: 428.2289459608986
+      counts_background: 2609.607391708814
+      counts_total: 7413.335254694742
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00021789453569040658
+  - name: R_13(pp->ee)
+    qmax: 338.8478
+    qmin: 326.1076
+    value:
+      background_std: 387.2323019446182
+      counts_background: 2338.114749738156
+      counts_total: 6526.826468444991
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00024454498308601225
+  - name: R_13(pp->ee)
+    qmax: 352.0857
+    qmin: 338.8478
+    value:
+      background_std: 352.7944835921638
+      counts_background: 2088.1376517856006
+      counts_total: 5785.420059023196
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00027617480881406836
+  - name: R_13(pp->ee)
+    qmax: 365.8409
+    qmin: 352.0857
+    value:
+      background_std: 322.01254487850343
+      counts_background: 1833.8603924256438
+      counts_total: 5116.656467932042
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00031329384990679563
+  - name: R_13(pp->ee)
+    qmax: 380.13
+    qmin: 365.8409
+    value:
+      background_std: 290.83285495135436
+      counts_background: 1603.7754477699277
+      counts_total: 4611.286134228489
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00034911174867409173
+  - name: R_13(pp->ee)
+    qmax: 394.9808
+    qmin: 380.13
+    value:
+      background_std: 259.7009761921493
+      counts_background: 1417.6814840612915
+      counts_total: 4047.8983410975466
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003949383957866019
+  - name: R_13(pp->ee)
+    qmax: 410.3972
+    qmin: 394.9808
+    value:
+      background_std: 229.65524036567348
+      counts_background: 1250.3041429155573
+      counts_total: 3590.8323511844733
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0004474341452706121
+  - name: R_13(pp->ee)
+    qmax: 426.4304
+    qmin: 410.3972
+    value:
+      background_std: 203.68384695271632
+      counts_background: 1084.2595270085908
+      counts_total: 3139.3471197369486
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000502394652969665
+  - name: R_13(pp->ee)
+    qmax: 443.0861
+    qmin: 426.4304
+    value:
+      background_std: 180.46309211601982
+      counts_background: 929.1673801481127
+      counts_total: 2714.309586232467
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005685160282425192
+  - name: R_13(pp->ee)
+    qmax: 460.3964
+    qmin: 443.0861
+    value:
+      background_std: 164.0562520677799
+      counts_background: 817.4596293316953
+      counts_total: 2413.180160272831
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006441667284197498
+  - name: R_13(pp->ee)
+    qmax: 478.383
+    qmin: 460.3964
+    value:
+      background_std: 151.21565368258194
+      counts_background: 713.584028297956
+      counts_total: 1996.6996376866573
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0007278476711879326
+  - name: R_13(pp->ee)
+    qmax: 497.0722
+    qmin: 478.383
+    value:
+      background_std: 129.85622039100267
+      counts_background: 613.1550127653774
+      counts_total: 1818.8200490770755
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000824405810877622
+  - name: R_13(pp->ee)
+    qmax: 516.4871
+    qmin: 497.0722
+    value:
+      background_std: 109.71058270193336
+      counts_background: 523.2001554980269
+      counts_total: 1631.0963731925158
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0009312442275077185
+  - name: R_13(pp->ee)
+    qmax: 536.665
+    qmin: 516.4871
+    value:
+      background_std: 103.53297658059545
+      counts_background: 454.5871906281341
+      counts_total: 1367.4928859180989
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0010553631282144097
+  - name: R_13(pp->ee)
+    qmax: 557.6312
+    qmin: 536.665
+    value:
+      background_std: 93.88784842155745
+      counts_background: 397.187198322839
+      counts_total: 1269.26775976893
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012095248020111693
+  - name: R_13(pp->ee)
+    qmax: 579.4164
+    qmin: 557.6312
+    value:
+      background_std: 77.65934727626819
+      counts_background: 330.5066667843718
+      counts_total: 1080.5695533549847
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0013733533694863858
+  - name: R_13(pp->ee)
+    qmax: 602.0475
+    qmin: 579.4164
+    value:
+      background_std: 68.49151428413838
+      counts_background: 294.8093172874121
+      counts_total: 937.1021583413152
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001559360967585762
+  - name: R_13(pp->ee)
+    qmax: 625.568
+    qmin: 602.0475
+    value:
+      background_std: 61.58781286671711
+      counts_background: 249.33282193224875
+      counts_total: 813.1811647654824
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0017785323319468057
+  - name: R_13(pp->ee)
+    qmax: 650.0075
+    qmin: 625.568
+    value:
+      background_std: 54.91632379110085
+      counts_background: 208.28654226082028
+      counts_total: 706.1610340728728
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0020326209745027937
+  - name: R_13(pp->ee)
+    qmax: 675.4017
+    qmin: 650.0075
+    value:
+      background_std: 49.24721937606607
+      counts_background: 177.74281816292327
+      counts_total: 555.9057477934142
+      distribution: general_gamma_counting_process
+      scale_factor: 0.002318110242712648
+  - name: R_13(pp->ee)
+    qmax: 701.7818
+    qmin: 675.4017
+    value:
+      background_std: 41.95765059011334
+      counts_background: 150.85535618677892
+      counts_total: 506.8087793638034
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0026641125124107945
+  - name: R_13(pp->ee)
+    qmax: 729.1987
+    qmin: 701.7818
+    value:
+      background_std: 36.232091025653396
+      counts_background: 128.3887976607438
+      counts_total: 435.21427396152177
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003038931703603945
+  - name: R_13(pp->ee)
+    qmax: 757.6867
+    qmin: 729.1987
+    value:
+      background_std: 31.448674177937836
+      counts_background: 105.81648927530459
+      counts_total: 423.3756607856382
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003495874956877871
+  - name: R_13(pp->ee)
+    qmax: 787.2599
+    qmin: 757.6867
+    value:
+      background_std: 27.980615771797872
+      counts_background: 94.25018192276096
+      counts_total: 398.84895995789265
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004013458350225681
+  - name: R_13(pp->ee)
+    qmax: 818.0378
+    qmin: 787.2599
+    value:
+      background_std: 24.220760425686688
+      counts_background: 75.90914641038265
+      counts_total: 299.7511245694044
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0046219449602098025
+  - name: R_13(pp->ee)
+    qmax: 849.9666
+    qmin: 818.0378
+    value:
+      background_std: 21.780938810526123
+      counts_background: 65.42094372808647
+      counts_total: 236.00694123573948
+      distribution: general_gamma_counting_process
+      scale_factor: 0.005300675309648257
+  - name: R_13(pp->ee)
+    qmax: 883.1727
+    qmin: 849.9666
+    value:
+      background_std: 19.215492334610015
+      counts_background: 52.8355751984345
+      counts_total: 215.41871361748014
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0061180313214885314
+  - name: R_13(pp->ee)
+    qmax: 917.6761
+    qmin: 883.1727
+    value:
+      background_std: 16.20071279217406
+      counts_background: 48.63267629643907
+      counts_total: 221.29819689281416
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0070704917637696586
+  - name: R_13(pp->ee)
+    qmax: 953.5275
+    qmin: 917.6761
+    value:
+      background_std: 13.811881132488796
+      counts_background: 39.524460869806795
+      counts_total: 159.51371038435036
+      distribution: general_gamma_counting_process
+      scale_factor: 0.008185107986076986
+  - name: R_13(pp->ee)
+    qmax: 990.7707
+    qmin: 953.5275
+    value:
+      background_std: 13.175902417516886
+      counts_background: 32.7632843122609
+      counts_total: 129.13353082330747
+      distribution: general_gamma_counting_process
+      scale_factor: 0.009525662259813395
+  - name: R_13(pp->ee)
+    qmax: 1029.4777
+    qmin: 990.7707
+    value:
+      background_std: 11.659037470077081
+      counts_background: 27.223269349649232
+      counts_total: 112.49576532027582
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01106394894571722
+  - name: R_13(pp->ee)
+    qmax: 1069.6969
+    qmin: 1029.4777
+    value:
+      background_std: 9.87136032601964
+      counts_background: 24.514709760773517
+      counts_total: 92.90250290773875
+      distribution: general_gamma_counting_process
+      scale_factor: 0.012840152490616673
+  - name: R_13(pp->ee)
+    qmax: 1111.4873
+    qmin: 1069.6969
+    value:
+      background_std: 8.705970941275497
+      counts_background: 19.941773635240168
+      counts_total: 88.01472671768623
+      distribution: general_gamma_counting_process
+      scale_factor: 0.015031760330856996
+  - name: R_13(pp->ee)
+    qmax: 1154.9002
+    qmin: 1111.4873
+    value:
+      background_std: 7.842767814625907
+      counts_background: 16.67930161035911
+      counts_total: 75.27792938634673
+      distribution: general_gamma_counting_process
+      scale_factor: 0.017709511586387495
+  - name: R_13(pp->ee)
+    qmax: 1200.0193
+    qmin: 1154.9002
+    value:
+      background_std: 7.314831606268497
+      counts_background: 13.649286751347637
+      counts_total: 56.67417863502218
+      distribution: general_gamma_counting_process
+      scale_factor: 0.020425979352369422
+  - name: R_13(pp->ee)
+    qmax: 1246.9012
+    qmin: 1200.0193
+    value:
+      background_std: 6.513418863069771
+      counts_background: 11.710345740689903
+      counts_total: 63.539075129751424
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0243830964409557
+  - name: R_13(pp->ee)
+    qmax: 1295.6146
+    qmin: 1246.9012
+    value:
+      background_std: 5.521353708896579
+      counts_background: 9.80053893636672
+      counts_total: 38.09018848604091
+      distribution: general_gamma_counting_process
+      scale_factor: 0.028231052442424482
+  - name: R_13(pp->ee)
+    qmax: 1346.2192
+    qmin: 1295.6146
+    value:
+      background_std: 4.694009268181746
+      counts_background: 9.156707931912937
+      counts_total: 40.04102995107373
+      distribution: general_gamma_counting_process
+      scale_factor: 0.033909257162614614
+  - name: R_13(pp->ee)
+    qmax: 1398.8127
+    qmin: 1346.2192
+    value:
+      background_std: 3.8574711625114353
+      counts_background: 6.790775188931913
+      counts_total: 28.3155164256166
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04009624995790919
+  - name: R_13(pp->ee)
+    qmax: 1453.4609
+    qmin: 1398.8127
+    value:
+      background_std: 3.378377788764045
+      counts_background: 5.6222286920611175
+      counts_total: 22.44740373150197
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0471070903104401
+  - name: R_13(pp->ee)
+    qmax: 1510.244
+    qmin: 1453.4609
+    value:
+      background_std: 3.1048366619791468
+      counts_background: 5.824330789885145
+      counts_total: 21.468559635362947
+      distribution: general_gamma_counting_process
+      scale_factor: 0.05605466718315075
+  - name: R_13(pp->ee)
+    qmax: 1569.2317
+    qmin: 1510.244
+    value:
+      background_std: 2.5393736037251857
+      counts_background: 4.426622246863116
+      counts_total: 17.562457567401644
+      distribution: general_gamma_counting_process
+      scale_factor: 0.06717407775091293
+  - name: R_13(pp->ee)
+    qmax: 1630.4802
+    qmin: 1569.2317
+    value:
+      background_std: 2.113991020963491
+      counts_background: 3.1974777594226738
+      counts_total: 9.749244343870092
+      distribution: general_gamma_counting_process
+      scale_factor: 0.08051811110941567
+  - name: R_13(pp->ee)
+    qmax: 1694.1791
+    qmin: 1630.4802
+    value:
+      background_std: 1.9315240978219659
+      counts_background: 2.521951325381498
+      counts_total: 13.652946963709823
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0954448321661011
+  - name: R_13(pp->ee)
+    qmax: 1760.3666
+    qmin: 1694.1791
+    value:
+      background_std: 1.6926221911321264
+      counts_background: 2.291654014912636
+      counts_total: 16.58183914474875
+      distribution: general_gamma_counting_process
+      scale_factor: 0.11570464057085542
+  - name: R_13(pp->ee)
+    qmax: 1829.1236
+    qmin: 1760.3666
+    value:
+      background_std: 1.361682821855043
+      counts_background: 1.6702317082582852
+      counts_total: 8.771855311944638
+      distribution: general_gamma_counting_process
+      scale_factor: 0.14006243288425288
+  - name: R_13(pp->ee)
+    qmax: 1900.583
+    qmin: 1829.1236
+    value:
+      background_std: 1.3526428282999017
+      counts_background: 2.588502215943407
+      counts_total: 5.8442199558327825
+      distribution: general_gamma_counting_process
+      scale_factor: 0.171541450134859
+  - name: R_13(pp->ee)
+    qmax: 1974.8342
+    qmin: 1900.583
+    value:
+      background_std: 1.0166440219119595
+      counts_background: 1.2453333652849015
+      counts_total: 0.9715693367457594
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2092432338426458
+  - name: R_13(pp->ee)
+    qmax: 2051.9861
+    qmin: 1974.8342
+    value:
+      background_std: 0.8758447738018891
+      counts_background: 1.0690832979944493
+      counts_total: 1.945364105403084
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2540206377272894
+  - name: R_13(pp->ee)
+    qmax: 2132.1334
+    qmin: 2051.9861
+    value:
+      background_std: 0.7323076989773978
+      counts_background: 0.8432196384712763
+      counts_total: 8.771855311944638
+      distribution: general_gamma_counting_process
+      scale_factor: 0.3151573602388245
+  - name: R_13(pp->ee)
+    qmax: 2215.4306
+    qmin: 2132.1334
+    value:
+      background_std: 0.6225672579529163
+      counts_background: 0.6383669088289287
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.3848308840456396
+  - name: R_13(pp->ee)
+    qmax: 2301.9821
+    qmin: 2215.4306
+    value:
+      background_std: 0.5353327260232467
+      counts_background: 0.5473485414495267
+      counts_total: 4.869045766105319
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4803713478452193
+  - name: R_13(pp->ee)
+    qmax: 2391.9149
+    qmin: 2301.9821
+    value:
+      background_std: 0.44779220779209794
+      counts_background: 0.40168531051194534
+      counts_total: 2.9193262317623336
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5987878305366042
+  - name: R_13(pp->ee)
+    qmax: 2485.3393
+    qmin: 2391.9149
+    value:
+      background_std: 0.39094696744595075
+      counts_background: 0.3327677765713436
+      counts_total: 4.869045766105319
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7482562094872316
+  - name: R_13(pp->ee)
+    qmax: 2582.4354
+    qmin: 2485.3393
+    value:
+      background_std: 0.33759452477562935
+      counts_background: 0.26659839919840733
+      counts_total: 1.9453641054030664
+      distribution: general_gamma_counting_process
+      scale_factor: 0.9435029816259038
+  - name: R_13(pp->ee)
+    qmax: 2683.3248
+    qmin: 2582.4354
+    value:
+      background_std: 0.2924475697391959
+      counts_background: 0.21531147314498952
+      counts_total: 1.9453641054030664
+      distribution: general_gamma_counting_process
+      scale_factor: 1.1988471147431752
+  - name: R_13(pp->ee)
+    qmax: 2788.1558
+    qmin: 2683.3248
+    value:
+      background_std: 0.2551134283132255
+      counts_background: 0.17073605744979936
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5175353554380437
+  - name: R_13(pp->ee)
+    qmax: 2897.0567
+    qmin: 2788.1558
+    value:
+      background_std: 0.22443486979462815
+      counts_background: 0.13491272038044805
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.952669252351545
+  - name: R_13(pp->ee)
+    qmax: 3010.2376
+    qmin: 2897.0567
+    value:
+      background_std: 0.1977807518255459
+      counts_background: 0.10584081101112268
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.5023129756161775
+  - name: R_13(pp->ee)
+    qmax: 3127.7298
+    qmin: 3010.2376
+    value:
+      background_std: 0.1714685821113244
+      counts_background: 0.08107242078289494
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.2447259310769816
+  - name: R_13(pp->ee)
+    qmax: 3249.9226
+    qmin: 3127.7298
+    value:
+      background_std: 0.1495995914919013
+      counts_background: 0.06217161870903482
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.26158294106928
+  - name: R_13(pp->ee)
+    qmax: 3376.8593
+    qmin: 3249.9226
+    value:
+      background_std: 0.12989764614730645
+      counts_background: 0.04783456444454831
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.610273061459661
+  - name: R_13(pp->ee)
+    qmax: 3508.785
+    qmin: 3376.8593
+    value:
+      background_std: 0.11563780858998697
+      counts_background: 0.036053033371854636
+      counts_total: 0.9715693367457524
+      distribution: general_gamma_counting_process
+      scale_factor: 7.455924738202726
+  - name: R_13(pp->ee)
+    qmax: 3645.8646
+    qmin: 3508.785
+    value:
+      background_std: 0.09999023273953724
+      counts_background: 0.026236390256353926
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.99546044140827
+  - name: R_13(pp->ee)
+    qmax: 3788.2997
+    qmin: 3645.8646
+    value:
+      background_std: 0.08561484210451817
+      counts_background: 0.0197865569730545
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 13.585420837517379
+  - name: R_13(pp->ee)
+    qmax: 3936.2646
+    qmin: 3788.2997
+    value:
+      background_std: 0.07388368415465373
+      counts_background: 0.014347254625227372
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 18.459757051860073
+  - name: R_13(pp->ee)
+    qmax: 4090.0448
+    qmin: 3936.2646
+    value:
+      background_std: 0.06302461460316248
+      counts_background: 0.010466361273598884
+      counts_total: 0.9715693367457524
+      distribution: general_gamma_counting_process
+      scale_factor: 25.650681230111875
+  - name: R_13(pp->ee)
+    qmax: 4249.8329
+    qmin: 4090.0448
+    value:
+      background_std: 0.05481290833416443
+      counts_background: 0.0073878230583136195
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 35.51063091958176
+  - name: R_13(pp->ee)
+    qmax: 4415.8634
+    qmin: 4249.8329
+    value:
+      background_std: 0.04643474045611447
+      counts_background: 0.005513465057972382
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 50.76076976105406
+  - name: R_13(pp->ee)
+    qmax: 4588.34
+    qmin: 4415.8634
+    value:
+      background_std: 0.038981639480376584
+      counts_background: 0.003516379596285951
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 73.10315047448637
+  - name: R_13(pp->ee)
+    qmax: 4767.5952
+    qmin: 4588.34
+    value:
+      background_std: 0.031000561796046447
+      counts_background: 0.0025468025477199596
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 106.42394209196908
+  - name: R_13(pp->ee)
+    qmax: 4953.8535
+    qmin: 4767.5952
+    value:
+      background_std: 0.021350088623077475
+      counts_background: 0.0016877241333322882
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 156.8038424677342
+  - name: R_13(pp->ee)
+    qmax: 5147.3884
+    qmin: 4953.8535
+    value:
+      background_std: 0.018518244451196132
+      counts_background: 0.0011031105137100342
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 234.69830154908252
+  - name: R_13(pp->ee)
+    qmax: 5348.4372
+    qmin: 5147.3884
+    value:
+      background_std: 0.017332008085563434
+      counts_background: 0.0007122186928155025
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 359.02069531801953
+  - name: R_13(pp->ee)
+    qmax: 5557.3875
+    qmin: 5348.4372
+    value:
+      background_std: 0.014476023761680524
+      counts_background: 0.0004371690750339727
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 559.0543679036756
+  - name: R_13(pp->ee)
+    qmax: 5774.5011
+    qmin: 5557.3875
+    value:
+      background_std: 0.011412766098604794
+      counts_background: 0.0002667414011898086
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 880.2572239137857
+  - name: R_13(pp->ee)
+    qmax: 5999.885
+    qmin: 5774.5011
+    value:
+      background_std: 0.019660699632794803
+      counts_background: 0.00021127565301545443
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 609.1436469323086
+
+ATLAS pp->enu 2019:
+  experiment: ATLAS
+  inspire: ATLAS:2019lsy
+  values:
+  - mTmax: 138.982
+    mTmin: 130.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 49484.8419359949
+      counts_background: 129820.73135913502
+      counts_total: 563230.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.6383035029286187e-06
+  - mTmax: 148.585
+    mTmin: 138.982
+    name: R_13(pp->enu)
+    value:
+      background_std: 55498.444905803444
+      counts_background: 150819.18570542432
+      counts_total: 673665.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1721793318498923e-06
+  - mTmax: 158.852
+    mTmin: 148.585
+    name: R_13(pp->enu)
+    value:
+      background_std: 43770.02692843129
+      counts_background: 141096.9691326152
+      counts_total: 560331.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.657433241379074e-06
+  - mTmax: 169.828
+    mTmin: 158.852
+    name: R_13(pp->enu)
+    value:
+      background_std: 31092.242263884735
+      counts_background: 123492.29775385726
+      counts_total: 431950.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.4931113488836114e-06
+  - mTmax: 181.562
+    mTmin: 169.828
+    name: R_13(pp->enu)
+    value:
+      background_std: 21906.70777115767
+      counts_background: 104542.43332579503
+      counts_total: 324635.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.776628421187213e-06
+  - mTmax: 194.107
+    mTmin: 181.562
+    name: R_13(pp->enu)
+    value:
+      background_std: 15640.847197926973
+      counts_background: 85600.41777043986
+      counts_total: 243844.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.627806912223095e-06
+  - mTmax: 207.519
+    mTmin: 194.107
+    name: R_13(pp->enu)
+    value:
+      background_std: 10898.031044212757
+      counts_background: 68932.5647278195
+      counts_total: 184520.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.15542720466144e-06
+  - mTmax: 221.857
+    mTmin: 207.519
+    name: R_13(pp->enu)
+    value:
+      background_std: 7745.417400963231
+      counts_background: 53691.25271654329
+      counts_total: 140146.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2079889169497448e-05
+  - mTmax: 237.186
+    mTmin: 221.857
+    name: R_13(pp->enu)
+    value:
+      background_std: 5584.0849060870305
+      counts_background: 41819.8659755992
+      counts_total: 107018.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5943224938748905e-05
+  - mTmax: 253.575
+    mTmin: 237.186
+    name: R_13(pp->enu)
+    value:
+      background_std: 4156.766259887125
+      counts_background: 32573.29828846043
+      counts_total: 82526.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.104860673441654e-05
+  - mTmax: 271.095
+    mTmin: 253.575
+    name: R_13(pp->enu)
+    value:
+      background_std: 3174.1290373266174
+      counts_background: 24539.820553266094
+      counts_total: 62571.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.6429874692013637e-05
+  - mTmax: 289.827
+    mTmin: 271.095
+    name: R_13(pp->enu)
+    value:
+      background_std: 2384.8306572215984
+      counts_background: 18487.620978801562
+      counts_total: 48409.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.413673825960676e-05
+  - mTmax: 309.852
+    mTmin: 289.827
+    name: R_13(pp->enu)
+    value:
+      background_std: 1873.7928281696456
+      counts_background: 14162.026474743869
+      counts_total: 37169.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.3374881191144686e-05
+  - mTmax: 331.261
+    mTmin: 309.852
+    name: R_13(pp->enu)
+    value:
+      background_std: 1439.4149123862792
+      counts_background: 10319.66489379555
+      counts_total: 28815.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.4976886015863484e-05
+  - mTmax: 354.15
+    mTmin: 331.261
+    name: R_13(pp->enu)
+    value:
+      background_std: 1124.7987219360627
+      counts_background: 7519.791303183718
+      counts_total: 21919.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.983735327425578e-05
+  - mTmax: 378.62
+    mTmin: 354.15
+    name: R_13(pp->enu)
+    value:
+      background_std: 860.1626882944936
+      counts_background: 5479.563709228112
+      counts_total: 16774.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.113140840083532e-05
+  - mTmax: 404.781
+    mTmin: 378.62
+    name: R_13(pp->enu)
+    value:
+      background_std: 682.617048645322
+      counts_background: 3992.8792213658303
+      counts_total: 12897.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00011335202408318016
+  - mTmax: 432.749
+    mTmin: 404.781
+    name: R_13(pp->enu)
+    value:
+      background_std: 536.8088063004928
+      counts_background: 2861.4860951082856
+      counts_total: 9953.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00014377894804630837
+  - mTmax: 462.65
+    mTmin: 432.749
+    name: R_13(pp->enu)
+    value:
+      background_std: 415.87036813854627
+      counts_background: 2016.7978951875964
+      counts_total: 7535.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00018591638603231064
+  - mTmax: 494.616
+    mTmin: 462.65
+    name: R_13(pp->enu)
+    value:
+      background_std: 327.4099326139175
+      counts_background: 1445.3327570847223
+      counts_total: 5773.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00023697414219574304
+  - mTmax: 528.792
+    mTmin: 494.616
+    name: R_13(pp->enu)
+    value:
+      background_std: 259.82819288145004
+      counts_background: 1035.7938114110407
+      counts_total: 4547.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003026719415244498
+  - mTmax: 565.329
+    mTmin: 528.792
+    name: R_13(pp->enu)
+    value:
+      background_std: 209.6449560187175
+      counts_background: 754.7680448057165
+      counts_total: 3389.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00038917133148512646
+  - mTmax: 604.39
+    mTmin: 565.329
+    name: R_13(pp->enu)
+    value:
+      background_std: 161.85673331239573
+      counts_background: 506.03442716518185
+      counts_total: 2610.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005003943116325671
+  - mTmax: 646.15
+    mTmin: 604.39
+    name: R_13(pp->enu)
+    value:
+      background_std: 124.83452342124754
+      counts_background: 344.9700173072118
+      counts_total: 2012.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006485843183333087
+  - mTmax: 690.796
+    mTmin: 646.15
+    name: R_13(pp->enu)
+    value:
+      background_std: 100.70386611247854
+      counts_background: 292.0344482181367
+      counts_total: 1457.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0008317641822735494
+  - mTmax: 738.526
+    mTmin: 690.796
+    name: R_13(pp->enu)
+    value:
+      background_std: 76.50435062982301
+      counts_background: 189.37872560617632
+      counts_total: 1127.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0010895786829861827
+  - mTmax: 789.555
+    mTmin: 738.526
+    name: R_13(pp->enu)
+    value:
+      background_std: 59.719265267352384
+      counts_background: 140.31564899455563
+      counts_total: 843.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001412822577146357
+  - mTmax: 844.109
+    mTmin: 789.555
+    name: R_13(pp->enu)
+    value:
+      background_std: 50.140722564398686
+      counts_background: 98.8955724921642
+      counts_total: 623.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0017803096161370174
+  - mTmax: 902.433
+    mTmin: 844.109
+    name: R_13(pp->enu)
+    value:
+      background_std: 35.256962054222704
+      counts_background: 67.41835243374094
+      counts_total: 518.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0024157613670345063
+  - mTmax: 964.786
+    mTmin: 902.433
+    name: R_13(pp->enu)
+    value:
+      background_std: 27.023343874576295
+      counts_background: 48.31517993631411
+      counts_total: 337.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003181339294922784
+  - mTmax: 1031.45
+    mTmin: 964.786
+    name: R_13(pp->enu)
+    value:
+      background_std: 20.610596523538565
+      counts_background: 34.05291864522614
+      counts_total: 294.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004261800410656309
+  - mTmax: 1102.72
+    mTmin: 1031.45
+    name: R_13(pp->enu)
+    value:
+      background_std: 15.801791187298008
+      counts_background: 24.40393204977451
+      counts_total: 232.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.005617225180407488
+  - mTmax: 1178.91
+    mTmin: 1102.72
+    name: R_13(pp->enu)
+    value:
+      background_std: 12.092075309739018
+      counts_background: 17.20008315833659
+      counts_total: 141.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007531030901164063
+  - mTmax: 1260.36
+    mTmin: 1178.91
+    name: R_13(pp->enu)
+    value:
+      background_std: 9.236083822588933
+      counts_background: 12.122753827141004
+      counts_total: 94.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.010291406333570428
+  - mTmax: 1347.45
+    mTmin: 1260.36
+    name: R_13(pp->enu)
+    value:
+      background_std: 7.050629700264793
+      counts_background: 8.982065252640252
+      counts_total: 85.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.013889921973154359
+  - mTmax: 1440.55
+    mTmin: 1347.45
+    name: R_13(pp->enu)
+    value:
+      background_std: 5.313931243968536
+      counts_background: 6.022027927865022
+      counts_total: 62.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.019227178040903105
+  - mTmax: 1540.09
+    mTmin: 1440.55
+    name: R_13(pp->enu)
+    value:
+      background_std: 4.012313219170332
+      counts_background: 4.244372625273755
+      counts_total: 39.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.026286375406568627
+  - mTmax: 1646.5
+    mTmin: 1540.09
+    name: R_13(pp->enu)
+    value:
+      background_std: 2.9664130688494814
+      counts_background: 2.991467193105486
+      counts_total: 19.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.03661217167018156
+  - mTmax: 1760.26
+    mTmin: 1646.5
+    name: R_13(pp->enu)
+    value:
+      background_std: 2.221664521030124
+      counts_background: 2.1084095948925303
+      counts_total: 16.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.051946315689801466
+  - mTmax: 1881.89
+    mTmin: 1760.26
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.6642557842663488
+      counts_background: 1.4860236575819088
+      counts_total: 16.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07370280403066642
+  - mTmax: 2011.92
+    mTmin: 1881.89
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.2408557038083075
+      counts_background: 1.0473611561256748
+      counts_total: 6.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.10652406912436779
+  - mTmax: 2150.93
+    mTmin: 2011.92
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.9175441203948996
+      counts_background: 0.7381883765874365
+      counts_total: 9.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.15685237916048003
+  - mTmax: 2299.55
+    mTmin: 2150.93
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.6699226658253623
+      counts_background: 0.5202809710305953
+      counts_total: 7.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.23099190742964934
+  - mTmax: 2458.43
+    mTmin: 2299.55
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.49062532661644165
+      counts_background: 0.3606400503373748
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.35249089583406584
+  - mTmax: 2628.3
+    mTmin: 2458.43
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.36196939444447523
+      counts_background: 0.25418194262210525
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5393081042532946
+  - mTmax: 2809.9
+    mTmin: 2628.3
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.2642369584530569
+      counts_background: 0.17618977761286764
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.8395788818133482
+  - mTmax: 3004.05
+    mTmin: 2809.9
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.19233013273004337
+      counts_background: 0.12417994036408388
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.3372273163550168
+  - mTmax: 3211.62
+    mTmin: 3004.05
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.13940468020741487
+      counts_background: 0.08607706688769459
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.213220904042899
+  - mTmax: 3433.52
+    mTmin: 3211.62
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.10465906608625981
+      counts_background: 0.060667793430760786
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.6879888136360206
+  - mTmax: 3670.76
+    mTmin: 3433.52
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.08095785152351652
+      counts_background: 0.04205273168724137
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.413200058277911
+  - mTmax: 3924.39
+    mTmin: 3670.76
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.06416177941570102
+      counts_background: 0.029149440623341485
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 11.490881994271946
+  - mTmax: 4195.55
+    mTmin: 3924.39
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.050197835211499
+      counts_background: 0.020205343495236155
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 21.349419121997073
+  - mTmax: 4485.44
+    mTmin: 4195.55
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.0390590161901452
+      counts_background: 0.01987153935881761
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 53.13381329287313
+  - mTmax: 4795.36
+    mTmin: 4485.44
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.030206657901604487
+      counts_background: 0.01987153935881761
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 478.7342235134824
+
+ATLAS pp->mumu 2016:
+  experiment: ATLAS
+  inspire: ATLAS:2017fih
+  values:
+  - name: R_13(pp->mumu)
+    qmax: 85.54876
+    qmin: 80.0
+    value:
+      background_std: 47159.54161
+      counts_background: 6764.512232812854
+      counts_total: 826504.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2762305970254551e-06
+  - name: R_13(pp->mumu)
+    qmax: 91.48239
+    qmin: 85.54876
+    value:
+      background_std: 317634.55716
+      counts_background: 14108.902856458606
+      counts_total: 5730639.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.8178514613498493e-07
+  - name: R_13(pp->mumu)
+    qmax: 97.82756
+    qmin: 91.48239
+    value:
+      background_std: 221426.46149
+      counts_background: 11237.65450078062
+      counts_total: 4062661.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.580659037125757e-07
+  - name: R_13(pp->mumu)
+    qmax: 104.61284
+    qmin: 97.82756
+    value:
+      background_std: 23673.1391
+      counts_background: 5387.892461379928
+      counts_total: 430822.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.4936960922852982e-06
+  - name: R_13(pp->mumu)
+    qmax: 111.86874
+    qmin: 104.61284
+    value:
+      background_std: 8035.54464
+      counts_background: 5023.582206650105
+      counts_total: 149927.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.290369522877894e-06
+  - name: R_13(pp->mumu)
+    qmax: 119.6279
+    qmin: 111.86874
+    value:
+      background_std: 4269.74216
+      counts_background: 5023.582206650105
+      counts_total: 82971.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.3372407014959593e-05
+  - name: R_13(pp->mumu)
+    qmax: 127.92524
+    qmin: 119.6279
+    value:
+      background_std: 2723.04212
+      counts_background: 4936.420670223463
+      counts_total: 54641.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1054688970870164e-05
+  - name: R_13(pp->mumu)
+    qmax: 136.79808
+    qmin: 127.92524
+    value:
+      background_std: 1948.58465
+      counts_background: 4766.608240471557
+      counts_total: 39501.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.9854648690468575e-05
+  - name: R_13(pp->mumu)
+    qmax: 146.28633
+    qmin: 136.79808
+    value:
+      background_std: 1473.90656
+      counts_background: 4602.637343122306
+      counts_total: 29742.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.112847100734332e-05
+  - name: R_13(pp->mumu)
+    qmax: 156.43268
+    qmin: 146.28633
+    value:
+      background_std: 1174.61412
+      counts_background: 4291.423265461886
+      counts_total: 23871.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.222690831812434e-05
+  - name: R_13(pp->mumu)
+    qmax: 167.28278
+    qmin: 156.43268
+    value:
+      background_std: 929.80497
+      counts_background: 4071.901814092623
+      counts_total: 18942.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.850801569289413e-05
+  - name: R_13(pp->mumu)
+    qmax: 178.88544
+    qmin: 167.28278
+    value:
+      background_std: 758.69868
+      counts_background: 3665.972384998197
+      counts_total: 15482.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.721354907837495e-05
+  - name: R_13(pp->mumu)
+    qmax: 191.29285
+    qmin: 178.88544
+    value:
+      background_std: 614.04569
+      counts_background: 3300.510213938981
+      counts_total: 12495.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00011154601639580714
+  - name: R_13(pp->mumu)
+    qmax: 204.56084
+    qmin: 191.29285
+    value:
+      background_std: 515.5105
+      counts_background: 3023.9480388959396
+      counts_total: 10462.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00013751259618992973
+  - name: R_13(pp->mumu)
+    qmax: 218.74908
+    qmin: 204.56084
+    value:
+      background_std: 419.80357
+      counts_background: 2583.224566423371
+      counts_total: 8583.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001735423572841351
+  - name: R_13(pp->mumu)
+    qmax: 233.92142
+    qmin: 218.74908
+    value:
+      background_std: 354.93752
+      counts_background: 2245.697995539776
+      counts_total: 6868.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00021559836611425865
+  - name: R_13(pp->mumu)
+    qmax: 250.1461
+    qmin: 233.92142
+    value:
+      background_std: 290.98522
+      counts_background: 1918.4001035163626
+      counts_total: 5649.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0002731167148073568
+  - name: R_13(pp->mumu)
+    qmax: 267.49612
+    qmin: 250.1461
+    value:
+      background_std: 247.43115
+      counts_background: 1638.8040442129902
+      counts_total: 4723.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003374008924078145
+  - name: R_13(pp->mumu)
+    qmax: 286.04953
+    qmin: 267.49612
+    value:
+      background_std: 201.90089
+      counts_background: 1351.799128632837
+      counts_total: 3762.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0004203618744570092
+  - name: R_13(pp->mumu)
+    qmax: 305.8898
+    qmin: 286.04953
+    value:
+      background_std: 167.21174
+      counts_background: 1154.7819846894593
+      counts_total: 3064.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000505843637474153
+  - name: R_13(pp->mumu)
+    qmax: 327.10617
+    qmin: 305.8898
+    value:
+      background_std: 140.17541
+      counts_background: 952.5441959802893
+      counts_total: 2471.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000613240962561096
+  - name: R_13(pp->mumu)
+    qmax: 349.79411
+    qmin: 327.10617
+    value:
+      background_std: 111.28163
+      counts_background: 732.5965428215242
+      counts_total: 2031.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000797354458396957
+  - name: R_13(pp->mumu)
+    qmax: 374.05567
+    qmin: 349.79411
+    value:
+      background_std: 93.29852
+      counts_background: 614.9663483614243
+      counts_total: 1595.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000976717309835189
+  - name: R_13(pp->mumu)
+    qmax: 400.0
+    qmin: 374.05567
+    value:
+      background_std: 77.70347
+      counts_background: 498.465534451482
+      counts_total: 1333.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001204994600221865
+  - name: R_13(pp->mumu)
+    qmax: 427.74382
+    qmin: 400.0
+    value:
+      background_std: 61.74306
+      counts_background: 370.1793275429616
+      counts_total: 1018.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0015350528063604598
+  - name: R_13(pp->mumu)
+    qmax: 457.41193
+    qmin: 427.74382
+    value:
+      background_std: 51.3044
+      counts_background: 300.0515993082377
+      counts_total: 819.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0018938236520369333
+  - name: R_13(pp->mumu)
+    qmax: 489.13782
+    qmin: 457.41193
+    value:
+      background_std: 41.50204
+      counts_background: 230.76804756031794
+      counts_total: 675.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0023960593888305657
+  - name: R_13(pp->mumu)
+    qmax: 523.06419
+    qmin: 489.13782
+    value:
+      background_std: 33.75002
+      counts_background: 168.40359227647843
+      counts_total: 508.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.002875050419527591
+  - name: R_13(pp->mumu)
+    qmax: 559.34369
+    qmin: 523.06419
+    value:
+      background_std: 27.85797
+      counts_background: 136.50078065460167
+      counts_total: 397.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003640757290227692
+  - name: R_13(pp->mumu)
+    qmax: 598.13951
+    qmin: 559.34369
+    value:
+      background_std: 21.3442
+      counts_background: 92.87640686917166
+      counts_total: 306.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004706476979947758
+  - name: R_13(pp->mumu)
+    qmax: 639.6262
+    qmin: 598.13951
+    value:
+      background_std: 17.55967
+      counts_background: 79.34019129282822
+      counts_total: 252.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0059466057209445556
+  - name: R_13(pp->mumu)
+    qmax: 683.99038
+    qmin: 639.6262
+    value:
+      background_std: 14.07663
+      counts_background: 57.89871417152278
+      counts_total: 188.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007549747471335277
+  - name: R_13(pp->mumu)
+    qmax: 731.43164
+    qmin: 683.99038
+    value:
+      background_std: 10.86199
+      counts_background: 39.39482623328838
+      counts_total: 129.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.009806916300293492
+  - name: R_13(pp->mumu)
+    qmax: 782.16341
+    qmin: 731.43164
+    value:
+      background_std: 8.62141
+      counts_background: 28.249678752902835
+      counts_total: 97.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.012426627758492669
+  - name: R_13(pp->mumu)
+    qmax: 836.4139
+    qmin: 782.16341
+    value:
+      background_std: 6.86123
+      counts_background: 21.72667376225719
+      counts_total: 78.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.016545321809072172
+  - name: R_13(pp->mumu)
+    qmax: 894.42719
+    qmin: 836.4139
+    value:
+      background_std: 5.52516
+      counts_background: 14.526539259467864
+      counts_total: 57.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.02008708102951275
+  - name: R_13(pp->mumu)
+    qmax: 956.46425
+    qmin: 894.42719
+    value:
+      background_std: 4.55665
+      counts_background: 12.851466920699988
+      counts_total: 51.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.025461293341897798
+  - name: R_13(pp->mumu)
+    qmax: 1022.80418
+    qmin: 956.46425
+    value:
+      background_std: 3.47985
+      counts_background: 9.54398459640824
+      counts_total: 39.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0334998929733532
+  - name: R_13(pp->mumu)
+    qmax: 1093.74541
+    qmin: 1022.80418
+    value:
+      background_std: 2.75975
+      counts_background: 7.469831593577929
+      counts_total: 29.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.044837372096784914
+  - name: R_13(pp->mumu)
+    qmax: 1169.6071
+    qmin: 1093.74541
+    value:
+      background_std: 2.17145
+      counts_background: 4.822553197387249
+      counts_total: 18.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.05915717390694639
+  - name: R_13(pp->mumu)
+    qmax: 1250.73051
+    qmin: 1169.6071
+    value:
+      background_std: 1.68286
+      counts_background: 3.168433486401449
+      counts_total: 18.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07712113092077916
+  - name: R_13(pp->mumu)
+    qmax: 1337.48061
+    qmin: 1250.73051
+    value:
+      background_std: 1.32923
+      counts_background: 3.2243779751696438
+      counts_total: 14.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.10633648600532984
+  - name: R_13(pp->mumu)
+    qmax: 1430.24766
+    qmin: 1337.48061
+    value:
+      background_std: 0.87866
+      counts_background: 1.0156796632709002
+      counts_total: 12.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.14294159630178704
+  - name: R_13(pp->mumu)
+    qmax: 1529.44898
+    qmin: 1430.24766
+    value:
+      background_std: 0.66988
+      counts_background: 0.6910779352492378
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.1939725971420614
+  - name: R_13(pp->mumu)
+    qmax: 1635.53087
+    qmin: 1529.44898
+    value:
+      background_std: 0.55593
+      counts_background: 0.7542820691954563
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2562541562784672
+  - name: R_13(pp->mumu)
+    qmax: 1748.97054
+    qmin: 1635.53087
+    value:
+      background_std: 0.40035
+      counts_background: 0.5043159487171365
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.3676386752489595
+  - name: R_13(pp->mumu)
+    qmax: 1870.27835
+    qmin: 1748.97054
+    value:
+      background_std: 0.27387
+      counts_background: 0.16451905877536685
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5117948254787213
+  - name: R_13(pp->mumu)
+    qmax: 2000.0
+    qmin: 1870.27835
+    value:
+      background_std: 0.22103
+      counts_background: 0.2417942372278825
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7060929175913717
+  - name: R_13(pp->mumu)
+    qmax: 2138.71909
+    qmin: 2000.0
+    value:
+      background_std: 0.15372
+      counts_background: 0.0802713950670074
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.9724792218029669
+  - name: R_13(pp->mumu)
+    qmax: 2287.05967
+    qmin: 2138.71909
+    value:
+      background_std: 0.11179
+      counts_background: 0.05756190191731741
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4083745391102105
+  - name: R_13(pp->mumu)
+    qmax: 2445.68909
+    qmin: 2287.05967
+    value:
+      background_std: 0.08209
+      counts_background: 0.042005949972813435
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.0044780091476864
+  - name: R_13(pp->mumu)
+    qmax: 2615.32097
+    qmin: 2445.68909
+    value:
+      background_std: 0.05988
+      counts_background: 0.031746012958316444
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.91733963386076
+  - name: R_13(pp->mumu)
+    qmax: 2796.71844
+    qmin: 2615.32097
+    value:
+      background_std: 0.0421
+      counts_background: 0.01781741085520469
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.2993953037780495
+  - name: R_13(pp->mumu)
+    qmax: 2990.69756
+    qmin: 2796.71844
+    value:
+      background_std: 0.02913
+      counts_background: 0.010914573172176702
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.510226547571808
+  - name: R_13(pp->mumu)
+    qmax: 3198.13098
+    qmin: 2990.69756
+    value:
+      background_std: 0.02102
+      counts_background: 0.007426377591989643
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.568102771607448
+  - name: R_13(pp->mumu)
+    qmax: 3419.95189
+    qmin: 3198.13098
+    value:
+      background_std: 0.01555
+      counts_background: 0.004316533692595911
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 13.662409300684185
+  - name: R_13(pp->mumu)
+    qmax: 3657.1582
+    qmin: 3419.95189
+    value:
+      background_std: 0.01023
+      counts_background: 0.002553257372458486
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 21.850209058054062
+  - name: R_13(pp->mumu)
+    qmax: 3910.81703
+    qmin: 3657.1582
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 34.656276448131415
+  - name: R_13(pp->mumu)
+    qmax: 4182.06952
+    qmin: 3910.81703
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 49.54781272142746
+  - name: R_13(pp->mumu)
+    qmax: 4472.13595
+    qmin: 4182.06952
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 87.46816282633966
+  - name: R_13(pp->mumu)
+    qmax: 4782.32127
+    qmin: 4472.13595
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 121.93859151255853
+  - name: R_13(pp->mumu)
+    qmax: 5114.0209
+    qmin: 4782.32127
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 262.2375145176054
+  - name: R_13(pp->mumu)
+    qmax: 5468.72706
+    qmin: 5114.0209
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 343.38755161998483
+  - name: R_13(pp->mumu)
+    qmax: 5848.03548
+    qmin: 5468.72706
+    value:
+      counts_background: 0.001799150805370723
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2617.913300405422
+
+ATLAS pp->mumu 2019:
+  experiment: ATLAS
+  inspire: ATLAS:2019erb
+  values:
+  - name: R_13(pp->mumu)
+    qmax: 135.0803
+    qmin: 130.0015
+    value:
+      background_std: 4367.714595558474
+      counts_background: 10153.696651035758
+      counts_total: 88900.72505429288
+      distribution: general_gamma_counting_process
+      scale_factor: 1.3369345962892415e-05
+  - name: R_13(pp->mumu)
+    qmax: 140.3576
+    qmin: 135.0803
+    value:
+      background_std: 3723.6485839727693
+      counts_background: 9920.127401610305
+      counts_total: 76010.57790325048
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5898981787757855e-05
+  - name: R_13(pp->mumu)
+    qmax: 145.841
+    qmin: 140.3576
+    value:
+      background_std: 3236.9080720913894
+      counts_background: 9683.799805626148
+      counts_total: 65457.24010408282
+      distribution: general_gamma_counting_process
+      scale_factor: 1.8539400928576078e-05
+  - name: R_13(pp->mumu)
+    qmax: 151.5373
+    qmin: 145.841
+    value:
+      background_std: 2806.1162240248427
+      counts_background: 9324.157636961534
+      counts_total: 57192.287720319844
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1715730499541426e-05
+  - name: R_13(pp->mumu)
+    qmax: 157.4575
+    qmin: 151.5373
+    value:
+      background_std: 2450.637008789551
+      counts_background: 8977.872052703644
+      counts_total: 50650.36549548864
+      distribution: general_gamma_counting_process
+      scale_factor: 2.527844696386039e-05
+  - name: R_13(pp->mumu)
+    qmax: 163.609
+    qmin: 157.4575
+    value:
+      background_std: 2164.498903030556
+      counts_background: 8610.873404427524
+      counts_total: 44624.60130125474
+      distribution: general_gamma_counting_process
+      scale_factor: 2.906361503952766e-05
+  - name: R_13(pp->mumu)
+    qmax: 170.0008
+    qmin: 163.609
+    value:
+      background_std: 1920.222298832865
+      counts_background: 8258.876975724814
+      counts_total: 39180.94686790684
+      distribution: general_gamma_counting_process
+      scale_factor: 3.334107023836068e-05
+  - name: R_13(pp->mumu)
+    qmax: 176.6408
+    qmin: 170.0008
+    value:
+      background_std: 1705.1502447211092
+      counts_background: 7853.265009112155
+      counts_total: 35224.766877306836
+      distribution: general_gamma_counting_process
+      scale_factor: 3.819525942378966e-05
+  - name: R_13(pp->mumu)
+    qmax: 183.5417
+    qmin: 176.6408
+    value:
+      background_std: 1545.617453400506
+      counts_background: 7424.961349684826
+      counts_total: 31434.531451849627
+      distribution: general_gamma_counting_process
+      scale_factor: 4.271296549700928e-05
+  - name: R_13(pp->mumu)
+    qmax: 190.7122
+    qmin: 183.5417
+    value:
+      background_std: 1361.6390035916802
+      counts_background: 6991.151557647795
+      counts_total: 28236.813106458783
+      distribution: general_gamma_counting_process
+      scale_factor: 4.964223066989248e-05
+  - name: R_13(pp->mumu)
+    qmax: 198.1629
+    qmin: 190.7122
+    value:
+      background_std: 1253.7405021521731
+      counts_background: 6573.151233593104
+      counts_total: 25356.64657165797
+      distribution: general_gamma_counting_process
+      scale_factor: 5.453267356084372e-05
+  - name: R_13(pp->mumu)
+    qmax: 205.9028
+    qmin: 198.1629
+    value:
+      background_std: 1098.3565690535725
+      counts_background: 6075.875574996823
+      counts_total: 22526.59594090615
+      distribution: general_gamma_counting_process
+      scale_factor: 6.384475962493046e-05
+  - name: R_13(pp->mumu)
+    qmax: 213.9394
+    qmin: 205.9028
+    value:
+      background_std: 992.7290459400999
+      counts_background: 5695.190813520244
+      counts_total: 20180.31199254282
+      distribution: general_gamma_counting_process
+      scale_factor: 7.214698475492765e-05
+  - name: R_13(pp->mumu)
+    qmax: 222.2975
+    qmin: 213.9394
+    value:
+      background_std: 896.1748902043114
+      counts_background: 5283.247892779931
+      counts_total: 17982.10623060412
+      distribution: general_gamma_counting_process
+      scale_factor: 8.169694585037675e-05
+  - name: R_13(pp->mumu)
+    qmax: 230.9902
+    qmin: 222.2975
+    value:
+      background_std: 809.212231286829
+      counts_background: 4847.175690441768
+      counts_total: 15899.124773315576
+      distribution: general_gamma_counting_process
+      scale_factor: 9.223170235446104e-05
+  - name: R_13(pp->mumu)
+    qmax: 240.0039
+    qmin: 230.9902
+    value:
+      background_std: 730.8420363763416
+      counts_background: 4424.41975182121
+      counts_total: 14358.798423966993
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00010455881400980028
+  - name: R_13(pp->mumu)
+    qmax: 249.3802
+    qmin: 240.0039
+    value:
+      background_std: 664.432089671552
+      counts_background: 4088.453093853648
+      counts_total: 12706.672555008621
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00011802003228863011
+  - name: R_13(pp->mumu)
+    qmax: 259.1229
+    qmin: 249.3802
+    value:
+      background_std: 600.9116491230056
+      counts_background: 3744.4206371814294
+      counts_total: 11581.632690063301
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001333523043133782
+  - name: R_13(pp->mumu)
+    qmax: 269.2462
+    qmin: 259.1229
+    value:
+      background_std: 539.5037438901195
+      counts_background: 3366.338860568191
+      counts_total: 10445.632978001702
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00014984999260907078
+  - name: R_13(pp->mumu)
+    qmax: 279.7625
+    qmin: 269.2462
+    value:
+      background_std: 481.7766655760301
+      counts_background: 3059.168629698733
+      counts_total: 9214.883837706684
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00016956358618142945
+  - name: R_13(pp->mumu)
+    qmax: 290.6922
+    qmin: 279.7625
+    value:
+      background_std: 430.5313825812963
+      counts_background: 2760.3694805902355
+      counts_total: 8289.496742318039
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00019086688158066704
+  - name: R_13(pp->mumu)
+    qmax: 302.0488
+    qmin: 290.6922
+    value:
+      background_std: 382.42825286878207
+      counts_background: 2464.6658255028965
+      counts_total: 7120.62776904233
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00021569582037502934
+  - name: R_13(pp->mumu)
+    qmax: 313.8491
+    qmin: 302.0488
+    value:
+      background_std: 342.57338424915906
+      counts_background: 2201.4790502153915
+      counts_total: 6484.727335344805
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00024349719192928918
+  - name: R_13(pp->mumu)
+    qmax: 326.1076
+    qmin: 313.8491
+    value:
+      background_std: 306.1004050678098
+      counts_background: 1973.3103565915962
+      counts_total: 5623.509795073417
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0002770729480361409
+  - name: R_13(pp->mumu)
+    qmax: 338.8478
+    qmin: 326.1076
+    value:
+      background_std: 274.4678706684229
+      counts_background: 1738.0193631550799
+      counts_total: 5011.715548434577
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003121084865743795
+  - name: R_13(pp->mumu)
+    qmax: 352.0857
+    qmin: 338.8478
+    value:
+      background_std: 246.51840584259045
+      counts_background: 1541.8025161604032
+      counts_total: 4362.237611319943
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003524922041136547
+  - name: R_13(pp->mumu)
+    qmax: 365.8409
+    qmin: 352.0857
+    value:
+      background_std: 218.9502659152475
+      counts_background: 1359.5182059940296
+      counts_total: 3844.4448328256917
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00040421316902894167
+  - name: R_13(pp->mumu)
+    qmax: 380.13
+    qmin: 365.8409
+    value:
+      background_std: 198.62327140570002
+      counts_background: 1216.8477789335761
+      counts_total: 3373.409872220816
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00045262155049093436
+  - name: R_13(pp->mumu)
+    qmax: 394.9808
+    qmin: 380.13
+    value:
+      background_std: 175.62174603822345
+      counts_background: 1043.1137252969772
+      counts_total: 3075.199782381399
+      distribution: general_gamma_counting_process
+      scale_factor: 0.000515346199953781
+  - name: R_13(pp->mumu)
+    qmax: 410.3972
+    qmin: 394.9808
+    value:
+      background_std: 157.82332196945347
+      counts_background: 922.5295789032424
+      counts_total: 2715.0409331261626
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005820924460894944
+  - name: R_13(pp->mumu)
+    qmax: 426.4304
+    qmin: 410.3972
+    value:
+      background_std: 139.44109301019662
+      counts_background: 785.8839723326984
+      counts_total: 2332.826720881545
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006613531407923803
+  - name: R_13(pp->mumu)
+    qmax: 443.0861
+    qmin: 426.4304
+    value:
+      background_std: 124.04574505049224
+      counts_background: 681.5390372117919
+      counts_total: 2039.7505842876824
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0007495824096508766
+  - name: R_13(pp->mumu)
+    qmax: 460.3964
+    qmin: 443.0861
+    value:
+      background_std: 111.28258332313048
+      counts_background: 610.0170339986892
+      counts_total: 1788.8091733167446
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0008536029653024192
+  - name: R_13(pp->mumu)
+    qmax: 478.383
+    qmin: 460.3964
+    value:
+      background_std: 97.82425788700547
+      counts_background: 511.9471693577202
+      counts_total: 1591.9518481111725
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0009710101550714133
+  - name: R_13(pp->mumu)
+    qmax: 497.0722
+    qmin: 478.383
+    value:
+      background_std: 86.22812946786841
+      counts_background: 425.82508654016516
+      counts_total: 1382.6905097402805
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001099342257951573
+  - name: R_13(pp->mumu)
+    qmax: 516.4871
+    qmin: 497.0722
+    value:
+      background_std: 77.02205107162364
+      counts_background: 371.91640457090034
+      counts_total: 1222.3381474622556
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012509665545845244
+  - name: R_13(pp->mumu)
+    qmax: 536.665
+    qmin: 516.4871
+    value:
+      background_std: 68.00617861258111
+      counts_background: 316.1517695027948
+      counts_total: 1035.5403586009006
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0014293298020503268
+  - name: R_13(pp->mumu)
+    qmax: 557.6312
+    qmin: 536.665
+    value:
+      background_std: 60.25531747065475
+      counts_background: 272.38180747053616
+      counts_total: 862.5866633691002
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001634083003692843
+  - name: R_13(pp->mumu)
+    qmax: 579.4164
+    qmin: 557.6312
+    value:
+      background_std: 52.793463587154974
+      counts_background: 228.33065305467525
+      counts_total: 747.601121084075
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0018718853685534508
+  - name: R_13(pp->mumu)
+    qmax: 602.0475
+    qmin: 579.4164
+    value:
+      background_std: 46.77168397340796
+      counts_background: 196.7191772412662
+      counts_total: 657.3050925583041
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00213247365713196
+  - name: R_13(pp->mumu)
+    qmax: 625.568
+    qmin: 602.0475
+    value:
+      background_std: 41.17478142754923
+      counts_background: 165.58547765970255
+      counts_total: 589.5395359110807
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0024248550694873027
+  - name: R_13(pp->mumu)
+    qmax: 650.0075
+    qmin: 625.568
+    value:
+      background_std: 35.59135332143866
+      counts_background: 134.43853087762895
+      counts_total: 518.7695788389075
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0027999949465572094
+  - name: R_13(pp->mumu)
+    qmax: 675.4017
+    qmin: 650.0075
+    value:
+      background_std: 31.50592338622992
+      counts_background: 116.90036706652529
+      counts_total: 433.31443806054205
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0032173646200448825
+  - name: R_13(pp->mumu)
+    qmax: 701.7818
+    qmin: 675.4017
+    value:
+      background_std: 27.701379510691396
+      counts_background: 96.68738128971845
+      counts_total: 381.29817398945477
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0036835961056184263
+  - name: R_13(pp->mumu)
+    qmax: 729.1987
+    qmin: 701.7818
+    value:
+      background_std: 24.413852558671156
+      counts_background: 80.78505166867615
+      counts_total: 320.4749513348551
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004224823661838057
+  - name: R_13(pp->mumu)
+    qmax: 757.6867
+    qmin: 729.1987
+    value:
+      background_std: 21.289903046275185
+      counts_background: 65.68939614857862
+      counts_total: 242.93407215642299
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0048782033266619364
+  - name: R_13(pp->mumu)
+    qmax: 787.2599
+    qmin: 757.6867
+    value:
+      background_std: 18.6305451577818
+      counts_background: 55.191921686106184
+      counts_total: 210.5823218507958
+      distribution: general_gamma_counting_process
+      scale_factor: 0.005685927149368299
+  - name: R_13(pp->mumu)
+    qmax: 818.0378
+    qmin: 787.2599
+    value:
+      background_std: 16.536662591150815
+      counts_background: 46.44635626445527
+      counts_total: 188.9874425158228
+      distribution: general_gamma_counting_process
+      scale_factor: 0.006526492268644452
+  - name: R_13(pp->mumu)
+    qmax: 849.9666
+    qmin: 818.0378
+    value:
+      background_std: 14.505819605441038
+      counts_background: 38.80428814755235
+      counts_total: 159.5758369534162
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007561327447535445
+  - name: R_13(pp->mumu)
+    qmax: 883.1727
+    qmin: 849.9666
+    value:
+      background_std: 12.69398206148668
+      counts_background: 31.799772094128638
+      counts_total: 132.1149124444831
+      distribution: general_gamma_counting_process
+      scale_factor: 0.008728608670103418
+  - name: R_13(pp->mumu)
+    qmax: 917.6761
+    qmin: 883.1727
+    value:
+      background_std: 10.96013593066989
+      counts_background: 26.36362907327209
+      counts_total: 130.16374355967136
+      distribution: general_gamma_counting_process
+      scale_factor: 0.010091307273161725
+  - name: R_13(pp->mumu)
+    qmax: 953.5275
+    qmin: 917.6761
+    value:
+      background_std: 9.558654105300288
+      counts_background: 23.380122492950765
+      counts_total: 97.83393914976413
+      distribution: general_gamma_counting_process
+      scale_factor: 0.011737486789007353
+  - name: R_13(pp->mumu)
+    qmax: 990.7707
+    qmin: 953.5275
+    value:
+      background_std: 8.116619876003165
+      counts_background: 18.38640506850625
+      counts_total: 98.80166798124685
+      distribution: general_gamma_counting_process
+      scale_factor: 0.013692105390868953
+  - name: R_13(pp->mumu)
+    qmax: 1029.4777
+    qmin: 990.7707
+    value:
+      background_std: 6.987043676362929
+      counts_background: 15.21189421824547
+      counts_total: 81.18051581971463
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0160710899719232
+  - name: R_13(pp->mumu)
+    qmax: 1069.6969
+    qmin: 1029.4777
+    value:
+      background_std: 6.10507820981051
+      counts_background: 12.588360806599598
+      counts_total: 55.71446901078137
+      distribution: general_gamma_counting_process
+      scale_factor: 0.018679890606014583
+  - name: R_13(pp->mumu)
+    qmax: 1111.4873
+    qmin: 1069.6969
+    value:
+      background_std: 5.299848780346374
+      counts_background: 10.187765038978078
+      counts_total: 59.63166441063757
+      distribution: general_gamma_counting_process
+      scale_factor: 0.02213925417038206
+  - name: R_13(pp->mumu)
+    qmax: 1154.9002
+    qmin: 1111.4873
+    value:
+      background_std: 4.704235571766579
+      counts_background: 8.771953096827428
+      counts_total: 36.14199722366014
+      distribution: general_gamma_counting_process
+      scale_factor: 0.025995727241749172
+  - name: R_13(pp->mumu)
+    qmax: 1200.0193
+    qmin: 1154.9002
+    value:
+      background_std: 4.109596900305143
+      counts_background: 6.286152008579877
+      counts_total: 24.408232244793
+      distribution: general_gamma_counting_process
+      scale_factor: 0.029524140097346323
+  - name: R_13(pp->mumu)
+    qmax: 1246.9012
+    qmin: 1200.0193
+    value:
+      background_std: 3.5014741416758075
+      counts_background: 5.241049219066606
+      counts_total: 36.14199722366014
+      distribution: general_gamma_counting_process
+      scale_factor: 0.035347463724205386
+  - name: R_13(pp->mumu)
+    qmax: 1295.6146
+    qmin: 1246.9012
+    value:
+      background_std: 2.923171595185668
+      counts_background: 4.2503303733331395
+      counts_total: 31.25014888621801
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04219771056355407
+  - name: R_13(pp->mumu)
+    qmax: 1346.2192
+    qmin: 1295.6146
+    value:
+      background_std: 2.512368538459842
+      counts_background: 3.8819983776243974
+      counts_total: 20.49594947779133
+      distribution: general_gamma_counting_process
+      scale_factor: 0.05045499969815339
+  - name: R_13(pp->mumu)
+    qmax: 1398.8127
+    qmin: 1346.2192
+    value:
+      background_std: 2.1871160372659273
+      counts_background: 3.1071352035118855
+      counts_total: 25.38742792567412
+      distribution: general_gamma_counting_process
+      scale_factor: 0.058682989749848556
+  - name: R_13(pp->mumu)
+    qmax: 1453.4609
+    qmin: 1398.8127
+    value:
+      background_std: 1.9142288225378918
+      counts_background: 2.9117906481200126
+      counts_total: 11.704138361564704
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07044473007349586
+  - name: R_13(pp->mumu)
+    qmax: 1510.244
+    qmin: 1453.4609
+    value:
+      background_std: 1.6109747804279697
+      counts_background: 1.9734458718273507
+      counts_total: 16.58737946413429
+      distribution: general_gamma_counting_process
+      scale_factor: 0.08351175322357265
+  - name: R_13(pp->mumu)
+    qmax: 1569.2317
+    qmin: 1510.244
+    value:
+      background_std: 1.3596667617093998
+      counts_background: 1.5622776588617944
+      counts_total: 10.726629870436735
+      distribution: general_gamma_counting_process
+      scale_factor: 0.09998835035230029
+  - name: R_13(pp->mumu)
+    qmax: 1630.4802
+    qmin: 1569.2317
+    value:
+      background_std: 1.1753244807757732
+      counts_background: 1.487705918173613
+      counts_total: 9.749338664649121
+      distribution: general_gamma_counting_process
+      scale_factor: 0.12016774811866186
+  - name: R_13(pp->mumu)
+    qmax: 1694.1791
+    qmin: 1630.4802
+    value:
+      background_std: 0.9528937034579805
+      counts_background: 0.8356622771025878
+      counts_total: 2.91991134349133
+      distribution: general_gamma_counting_process
+      scale_factor: 0.14378400198027075
+  - name: R_13(pp->mumu)
+    qmax: 1760.3666
+    qmin: 1694.1791
+    value:
+      background_std: 0.8251118128615457
+      counts_background: 0.8674311841250307
+      counts_total: 4.869751887632895
+      distribution: general_gamma_counting_process
+      scale_factor: 0.17429670890943472
+  - name: R_13(pp->mumu)
+    qmax: 1829.1236
+    qmin: 1760.3666
+    value:
+      background_std: 0.6958565863982882
+      counts_background: 0.6821581505907652
+      counts_total: 3.8954990733880965
+      distribution: general_gamma_counting_process
+      scale_factor: 0.20969017935423678
+  - name: R_13(pp->mumu)
+    qmax: 1900.583
+    qmin: 1829.1236
+    value:
+      background_std: 0.5899493142426738
+      counts_background: 0.5239969594953287
+      counts_total: 6.821945865342037
+      distribution: general_gamma_counting_process
+      scale_factor: 0.24977990391086993
+  - name: R_13(pp->mumu)
+    qmax: 1974.8342
+    qmin: 1900.583
+    value:
+      background_std: 0.49092823052342044
+      counts_background: 0.43885114767648925
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 0.30756292961115134
+  - name: R_13(pp->mumu)
+    qmax: 2051.9861
+    qmin: 1974.8342
+    value:
+      background_std: 0.4291881334049234
+      counts_background: 0.48162812476032607
+      counts_total: 3.8954990733880965
+      distribution: general_gamma_counting_process
+      scale_factor: 0.37647180044702155
+  - name: R_13(pp->mumu)
+    qmax: 2132.1334
+    qmin: 2051.9861
+    value:
+      background_std: 0.3343365638196021
+      counts_background: 0.19462746985675
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4582338738034427
+  - name: R_13(pp->mumu)
+    qmax: 2215.4306
+    qmin: 2132.1334
+    value:
+      background_std: 0.2857824733113037
+      counts_background: 0.19526708767209217
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5618019999396292
+  - name: R_13(pp->mumu)
+    qmax: 2301.9821
+    qmin: 2215.4306
+    value:
+      background_std: 0.23116537164941736
+      counts_background: 0.12643808270036044
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 0.6987736111706894
+  - name: R_13(pp->mumu)
+    qmax: 2391.9149
+    qmin: 2301.9821
+    value:
+      background_std: 0.20089826500598856
+      counts_background: 0.1576924633211208
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 0.8585327857157209
+  - name: R_13(pp->mumu)
+    qmax: 2485.3393
+    qmin: 2391.9149
+    value:
+      background_std: 0.15887986626290038
+      counts_background: 0.08480789327041269
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 1.069515278976801
+  - name: R_13(pp->mumu)
+    qmax: 2582.4354
+    qmin: 2485.3393
+    value:
+      background_std: 0.1410858145400934
+      counts_background: 0.11418425270635946
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.301972263055654
+  - name: R_13(pp->mumu)
+    qmax: 2683.3248
+    qmin: 2582.4354
+    value:
+      background_std: 0.1068676666450574
+      counts_background: 0.04961113093891317
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.668772913396739
+  - name: R_13(pp->mumu)
+    qmax: 2788.1558
+    qmin: 2683.3248
+    value:
+      background_std: 0.09165593554507097
+      counts_background: 0.04562408445467029
+      counts_total: 0.9718367624821219
+      distribution: general_gamma_counting_process
+      scale_factor: 2.0212804689349286
+  - name: R_13(pp->mumu)
+    qmax: 2897.0567
+    qmin: 2788.1558
+    value:
+      background_std: 0.07266099936407698
+      counts_background: 0.029852647397427517
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.5884432174257777
+  - name: R_13(pp->mumu)
+    qmax: 3010.2376
+    qmin: 2897.0567
+    value:
+      background_std: 0.05937261374480347
+      counts_background: 0.02305575282997262
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.2616513664606708
+  - name: R_13(pp->mumu)
+    qmax: 3127.7298
+    qmin: 3010.2376
+    value:
+      background_std: 0.048897651723779155
+      counts_background: 0.021533828672332694
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.14712944045477
+  - name: R_13(pp->mumu)
+    qmax: 3249.9226
+    qmin: 3127.7298
+    value:
+      background_std: 0.04053363372415464
+      counts_background: 0.014452558190829348
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.109370450736852
+  - name: R_13(pp->mumu)
+    qmax: 3376.8593
+    qmin: 3249.9226
+    value:
+      background_std: 0.032884110998414366
+      counts_background: 0.011636818292003148
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.541208558341123
+  - name: R_13(pp->mumu)
+    qmax: 3508.785
+    qmin: 3376.8593
+    value:
+      background_std: 0.02567529578701084
+      counts_background: 0.00767366729706161
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.535774507148146
+  - name: R_13(pp->mumu)
+    qmax: 3645.8646
+    qmin: 3508.785
+    value:
+      background_std: 0.021258406573862562
+      counts_background: 0.006780896151680328
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 10.678887754304286
+  - name: R_13(pp->mumu)
+    qmax: 3788.2997
+    qmin: 3645.8646
+    value:
+      background_std: 0.017022424340037038
+      counts_background: 0.005546717917897577
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 13.776294316278825
+  - name: R_13(pp->mumu)
+    qmax: 3936.2646
+    qmin: 3788.2997
+    value:
+      background_std: 0.013641616891697666
+      counts_background: 0.003463470453841179
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 17.526333510275986
+  - name: R_13(pp->mumu)
+    qmax: 4090.0448
+    qmin: 3936.2646
+    value:
+      background_std: 0.011398526264329106
+      counts_background: 0.0031503203861262606
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 21.973882965269826
+  - name: R_13(pp->mumu)
+    qmax: 4249.8329
+    qmin: 4090.0448
+    value:
+      counts_background: 0.002082335478877652
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 29.205209784669062
+  - name: R_13(pp->mumu)
+    qmax: 4415.8634
+    qmin: 4249.8329
+    value:
+      counts_background: 0.0017217578499394992
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 38.16374407614321
+  - name: R_13(pp->mumu)
+    qmax: 4588.34
+    qmin: 4415.8634
+    value:
+      counts_background: 0.0012556895280845621
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 46.82189531633008
+  - name: R_13(pp->mumu)
+    qmax: 4767.5952
+    qmin: 4588.34
+    value:
+      counts_background: 0.0010416661644099543
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 64.27197320998265
+  - name: R_13(pp->mumu)
+    qmax: 4953.8535
+    qmin: 4767.5952
+    value:
+      counts_background: 0.0011258892192544847
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 81.1673764868627
+  - name: R_13(pp->mumu)
+    qmax: 5147.3884
+    qmin: 4953.8535
+    value:
+      counts_background: 0.0005170426780294539
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 99.92773150300667
+  - name: R_13(pp->mumu)
+    qmax: 5348.4372
+    qmin: 5147.3884
+    value:
+      counts_background: 0.0005607270986205246
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 132.74348458839472
+  - name: R_13(pp->mumu)
+    qmax: 5557.3875
+    qmin: 5348.4372
+    value:
+      counts_background: 0.00027014231729417554
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 162.634233307347
+  - name: R_13(pp->mumu)
+    qmax: 5774.5011
+    qmin: 5557.3875
+    value:
+      counts_background: 0.00021044257812091968
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 217.6082875120953
+  - name: R_13(pp->mumu)
+    qmax: 5999.885
+    qmin: 5774.5011
+    value:
+      counts_background: 0.0009004009617230382
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 55.02608893905476
+
+ATLAS pp->munu 2019:
+  experiment: ATLAS
+  inspire: ATLAS:2019lsy
+  values:
+  - mTmax: 119.581
+    mTmin: 110.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 173393.2448460692
+      counts_background: 311864.19556950964
+      counts_total: 2194000.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.183558551333135e-07
+  - mTmax: 129.997
+    mTmin: 119.581
+    name: R_13(pp->munu)
+    value:
+      background_std: 185347.68842526848
+      counts_background: 334965.4391578278
+      counts_total: 2235920.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.139253383650937e-07
+  - mTmax: 141.32
+    mTmin: 129.997
+    name: R_13(pp->munu)
+    value:
+      background_std: 137086.69374739804
+      counts_background: 275204.2727846906
+      counts_total: 1532830.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.30843667032931e-07
+  - mTmax: 153.63
+    mTmin: 141.32
+    name: R_13(pp->munu)
+    value:
+      background_std: 90970.90353681444
+      counts_background: 210511.51756797262
+      counts_total: 980250.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4960178814318527e-06
+  - mTmax: 167.011
+    mTmin: 153.63
+    name: R_13(pp->munu)
+    value:
+      background_std: 55187.39413924524
+      counts_background: 158175.03201538566
+      counts_total: 612905.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.5367232855516335e-06
+  - mTmax: 181.558
+    mTmin: 167.011
+    name: R_13(pp->munu)
+    value:
+      background_std: 32400.733223956522
+      counts_background: 116745.83059004245
+      counts_total: 389728.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.11468330741908e-06
+  - mTmax: 197.372
+    mTmin: 181.558
+    name: R_13(pp->munu)
+    value:
+      background_std: 18816.999329162023
+      counts_background: 86167.76482670868
+      counts_total: 256420.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.562284233727933e-06
+  - mTmax: 214.564
+    mTmin: 197.372
+    name: R_13(pp->munu)
+    value:
+      background_std: 11001.560721747801
+      counts_background: 62472.61068447967
+      counts_total: 172285.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.856474323178904e-06
+  - mTmax: 233.253
+    mTmin: 214.564
+    name: R_13(pp->munu)
+    value:
+      background_std: 6787.890162959327
+      counts_background: 45293.354116629445
+      counts_total: 119462.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4412265253190765e-05
+  - mTmax: 253.57
+    mTmin: 233.253
+    name: R_13(pp->munu)
+    value:
+      background_std: 4482.559073112255
+      counts_background: 32256.75604219662
+      counts_total: 83461.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.0236995712824706e-05
+  - mTmax: 275.657
+    mTmin: 253.57
+    name: R_13(pp->munu)
+    value:
+      background_std: 3092.594300793429
+      counts_background: 22565.672240758515
+      counts_total: 59443.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.8091111352459282e-05
+  - mTmax: 299.667
+    mTmin: 275.657
+    name: R_13(pp->munu)
+    value:
+      background_std: 2144.445723415727
+      counts_background: 15786.136802201023
+      counts_total: 42137.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.0155157629817596e-05
+  - mTmax: 325.769
+    mTmin: 299.667
+    name: R_13(pp->munu)
+    value:
+      background_std: 1511.5214055146557
+      counts_background: 10847.878881784714
+      counts_total: 30145.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.361211781724731e-05
+  - mTmax: 354.144
+    mTmin: 325.769
+    name: R_13(pp->munu)
+    value:
+      background_std: 1062.6283559947005
+      counts_background: 7322.429051619332
+      counts_total: 21500.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.30621477165014e-05
+  - mTmax: 384.991
+    mTmin: 354.144
+    name: R_13(pp->munu)
+    value:
+      background_std: 748.9523747775957
+      counts_background: 4942.71440530476
+      counts_total: 15241.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.980396350154575e-05
+  - mTmax: 418.524
+    mTmin: 384.991
+    name: R_13(pp->munu)
+    value:
+      background_std: 559.2949933845287
+      counts_background: 3336.382711281383
+      counts_total: 10752.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00013312926976211077
+  - mTmax: 454.979
+    mTmin: 418.524
+    name: R_13(pp->munu)
+    value:
+      background_std: 421.42780851011713
+      counts_background: 2212.21629107045
+      counts_total: 7843.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001859921295859557
+  - mTmax: 494.609
+    mTmin: 454.979
+    name: R_13(pp->munu)
+    value:
+      background_std: 321.7383409908742
+      counts_background: 1440.856366006565
+      counts_total: 5457.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00024623862733648454
+  - mTmax: 537.69
+    mTmin: 494.609
+    name: R_13(pp->munu)
+    value:
+      background_std: 239.9465672188081
+      counts_background: 938.4557359249345
+      counts_total: 4013.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00034358157741364064
+  - mTmax: 584.525
+    mTmin: 537.69
+    name: R_13(pp->munu)
+    value:
+      background_std: 183.88702799447276
+      counts_background: 611.2331451408502
+      counts_total: 2761.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0004695043536296467
+  - mTmax: 635.438
+    mTmin: 584.525
+    name: R_13(pp->munu)
+    value:
+      background_std: 138.2081337259135
+      counts_background: 412.5886164536204
+      counts_total: 2050.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006495279550335438
+  - mTmax: 690.786
+    mTmin: 635.438
+    name: R_13(pp->munu)
+    value:
+      background_std: 104.31690520855189
+      counts_background: 259.2943797404666
+      counts_total: 1401.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0008841816038939344
+  - mTmax: 750.956
+    mTmin: 690.786
+    name: R_13(pp->munu)
+    value:
+      background_std: 81.90443651622297
+      counts_background: 175.02635490532282
+      counts_total: 1056.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012005591743499255
+  - mTmax: 816.366
+    mTmin: 750.956
+    name: R_13(pp->munu)
+    value:
+      background_std: 63.05459775821269
+      counts_background: 111.97934711011833
+      counts_total: 673.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0016858815516968251
+  - mTmax: 887.473
+    mTmin: 816.366
+    name: R_13(pp->munu)
+    value:
+      background_std: 47.85252681781809
+      counts_background: 72.93416823487914
+      counts_total: 531.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.002378929594384112
+  - mTmax: 964.775
+    mTmin: 887.473
+    name: R_13(pp->munu)
+    value:
+      background_std: 29.884772152050953
+      counts_background: 51.02213419686935
+      counts_total: 339.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0037000395697988574
+  - mTmax: 1048.81
+    mTmin: 964.775
+    name: R_13(pp->munu)
+    value:
+      background_std: 21.73445316870199
+      counts_background: 31.49748386037507
+      counts_total: 237.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.005174238254625601
+  - mTmax: 1140.16
+    mTmin: 1048.81
+    name: R_13(pp->munu)
+    value:
+      background_std: 15.61168559953998
+      counts_background: 20.514879271343897
+      counts_total: 150.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007466198646398077
+  - mTmax: 1239.47
+    mTmin: 1140.16
+    name: R_13(pp->munu)
+    value:
+      background_std: 11.187807123760404
+      counts_background: 13.36171083961638
+      counts_total: 105.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01100172185890467
+  - mTmax: 1347.44
+    mTmin: 1239.47
+    name: R_13(pp->munu)
+    value:
+      background_std: 8.090867417412117
+      counts_background: 8.702723238099091
+      counts_total: 96.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.016214937698075395
+  - mTmax: 1464.8
+    mTmin: 1347.44
+    name: R_13(pp->munu)
+    value:
+      background_std: 5.861732064721911
+      counts_background: 5.668240591945363
+      counts_total: 53.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.02390337386688388
+  - mTmax: 1592.39
+    mTmin: 1464.8
+    name: R_13(pp->munu)
+    value:
+      background_std: 4.239721806470444
+      counts_background: 3.6918273199269356
+      counts_total: 36.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.035244263449434175
+  - mTmax: 1731.09
+    mTmin: 1592.39
+    name: R_13(pp->munu)
+    value:
+      background_std: 3.061547949508712
+      counts_background: 2.404553712756417
+      counts_total: 29.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.05303191512672773
+  - mTmax: 1881.87
+    mTmin: 1731.09
+    name: R_13(pp->munu)
+    value:
+      background_std: 2.218979709424131
+      counts_background: 1.5943593275816659
+      counts_total: 18.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07838762242210882
+  - mTmax: 2045.79
+    mTmin: 1881.87
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.6094064148303902
+      counts_background: 1.03843498310755
+      counts_total: 9.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.12035229841895172
+  - mTmax: 2223.98
+    mTmin: 2045.79
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.1798660461214443
+      counts_background: 0.6885429477500506
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.18151088088844602
+  - mTmax: 2417.69
+    mTmin: 2223.98
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.86915070607508
+      counts_background: 0.4484604392161544
+      counts_total: 8.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.27868241219689954
+  - mTmax: 2628.28
+    mTmin: 2417.69
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.6397040443261947
+      counts_background: 0.29735542214027355
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4288406362148017
+  - mTmax: 2857.21
+    mTmin: 2628.28
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.4678828354299824
+      counts_background: 0.19716398447712893
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.65993662594304
+  - mTmax: 3106.08
+    mTmin: 2857.21
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.3384261768295841
+      counts_background: 0.12841645879193278
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.0339214268125256
+  - mTmax: 3376.63
+    mTmin: 3106.08
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.24192533758888526
+      counts_background: 0.0851476004897484
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.6238864069933419
+  - mTmax: 3670.74
+    mTmin: 3376.63
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.17058236546210775
+      counts_background: 0.056457824311358915
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.551003391247446
+  - mTmax: 3990.47
+    mTmin: 3670.74
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.11914494667660731
+      counts_background: 0.037434829726717155
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.091595045707155
+  - mTmax: 4338.05
+    mTmin: 3990.47
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.0820679904624702
+      counts_background: 0.024821475034884872
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.565906566219575
+  - mTmax: 4715.91
+    mTmin: 4338.05
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.055953621511592076
+      counts_background: 0.019677300467498864
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 10.912599350193446
+  - mTmax: 5126.68
+    mTmin: 4715.91
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.037750974048514296
+      counts_background: 0.019677300467498864
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 19.88897136882155
+  - mTmax: 5573.22
+    mTmin: 5126.68
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.02523328957856268
+      counts_background: 0.019677300467498864
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 42.53711207391964
+  - mTmax: 6058.67
+    mTmin: 5573.22
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.01671618330130428
+      counts_background: 0.019677300467498864
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 143.20866623927168
+
+CMS pp->ee 2021:
+  experiment: CMS
+  inspire: CMS:2021ctt
+  values:
+  - name: R_13(pp->ee)
+    qmax: 65.0
+    qmin: 60.0
+    value:
+      background_std: 831.0
+      counts_background: 5701.878980308002
+      counts_total: 15452.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00012185527470961339
+  - name: R_13(pp->ee)
+    qmax: 70.0
+    qmin: 65.0
+    value:
+      background_std: 1023.3
+      counts_background: 6455.043606542603
+      counts_total: 22003.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.041585490665783e-05
+  - name: R_13(pp->ee)
+    qmax: 75.0
+    qmin: 70.0
+    value:
+      background_std: 2692.9500000000003
+      counts_background: 7865.872675685383
+      counts_total: 69945.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.648513703714104e-05
+  - name: R_13(pp->ee)
+    qmax: 80.0
+    qmin: 75.0
+    value:
+      background_std: 10302.0
+      counts_background: 9370.536765396653
+      counts_total: 304020.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.460285251233667e-06
+  - name: R_13(pp->ee)
+    qmax: 85.0
+    qmin: 80.0
+    value:
+      background_std: 50005.0
+      counts_background: 12020.799408359051
+      counts_total: 1522250.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.690077527158101e-07
+  - name: R_13(pp->ee)
+    qmax: 90.0
+    qmin: 85.0
+    value:
+      background_std: 321280.0
+      counts_background: 25138.417113316355
+      counts_total: 9638500.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.0426141482073915e-07
+  - name: R_13(pp->ee)
+    qmax: 95.0
+    qmin: 90.0
+    value:
+      background_std: 429800.0
+      counts_background: 32226.353364161692
+      counts_total: 13100500.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.666763265989404e-08
+  - name: R_13(pp->ee)
+    qmax: 100.0
+    qmin: 95.0
+    value:
+      background_std: 72980.0
+      counts_background: 14817.334342045522
+      counts_total: 2188450.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.4704648764652155e-07
+  - name: R_13(pp->ee)
+    qmax: 105.0
+    qmin: 100.0
+    value:
+      background_std: 21565.0
+      counts_background: 12540.078528575195
+      counts_total: 634750.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5807013446331753e-06
+  - name: R_13(pp->ee)
+    qmax: 110.0
+    qmin: 105.0
+    value:
+      background_std: 11210.0
+      counts_background: 12533.67770365131
+      counts_total: 330785.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.1060510844567983e-06
+  - name: R_13(pp->ee)
+    qmax: 115.0
+    qmin: 110.0
+    value:
+      background_std: 7552.0
+      counts_background: 12382.087819132976
+      counts_total: 213745.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.863852620007929e-06
+  - name: R_13(pp->ee)
+    qmax: 120.0
+    qmin: 115.0
+    value:
+      background_std: 5501.0
+      counts_background: 12095.702732163982
+      counts_total: 153970.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.893179328721299e-06
+  - name: R_13(pp->ee)
+    qmax: 125.0
+    qmin: 120.0
+    value:
+      background_std: 5257.0
+      counts_background: 11728.78965062577
+      counts_total: 118255.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.931757380176736e-06
+  - name: R_13(pp->ee)
+    qmax: 130.0
+    qmin: 125.0
+    value:
+      background_std: 5197.0
+      counts_background: 11292.004025812214
+      counts_total: 94995.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.1384475528590407e-05
+  - name: R_13(pp->ee)
+    qmax: 135.0
+    qmin: 130.0
+    value:
+      background_std: 5180.5
+      counts_background: 10912.264773388133
+      counts_total: 78355.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4125836791104324e-05
+  - name: R_13(pp->ee)
+    qmax: 140.0
+    qmin: 135.0
+    value:
+      background_std: 3200.1499999999996
+      counts_background: 10471.079468496435
+      counts_total: 65250.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.7088844016926783e-05
+  - name: R_13(pp->ee)
+    qmax: 145.0
+    qmin: 140.0
+    value:
+      background_std: 2400.1
+      counts_background: 9969.37898459165
+      counts_total: 56545.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.0407827461011443e-05
+  - name: R_13(pp->ee)
+    qmax: 150.0
+    qmin: 145.0
+    value:
+      background_std: 2193.7
+      counts_background: 9432.135822344337
+      counts_total: 48691.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.47663159105068e-05
+  - name: R_13(pp->ee)
+    qmax: 160.0
+    qmin: 150.0
+    value:
+      background_std: 4317.799999999999
+      counts_background: 17254.827825832945
+      counts_total: 79345.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5416384324049313e-05
+  - name: R_13(pp->ee)
+    qmax: 170.0
+    qmin: 160.0
+    value:
+      background_std: 2478.0
+      counts_background: 15315.666857844357
+      counts_total: 62263.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.021551726016375e-05
+  - name: R_13(pp->ee)
+    qmax: 180.0
+    qmin: 170.0
+    value:
+      background_std: 2020.1
+      counts_background: 13603.693439102217
+      counts_total: 50152.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.6749392802316055e-05
+  - name: R_13(pp->ee)
+    qmax: 190.0
+    qmin: 180.0
+    value:
+      background_std: 1637.2
+      counts_background: 11834.791436535725
+      counts_total: 40918.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.290507813517481e-05
+  - name: R_13(pp->ee)
+    qmax: 200.0
+    qmin: 190.0
+    value:
+      background_std: 1438.8999999999999
+      counts_background: 10420.17740612818
+      counts_total: 33718.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.2097818026876184e-05
+  - name: R_13(pp->ee)
+    qmax: 220.0
+    qmin: 200.0
+    value:
+      background_std: 2751.2
+      counts_background: 17000.844251358405
+      counts_total: 51164.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.9084933662945905e-05
+  - name: R_13(pp->ee)
+    qmax: 240.0
+    qmin: 220.0
+    value:
+      background_std: 1431.14
+      counts_background: 12808.032882070536
+      counts_total: 36436.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.143221958147583e-05
+  - name: R_13(pp->ee)
+    qmax: 260.0
+    qmin: 240.0
+    value:
+      background_std: 1083.64
+      counts_background: 9706.08994787363
+      counts_total: 26302.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.9588694486052555e-05
+  - name: R_13(pp->ee)
+    qmax: 280.0
+    qmin: 260.0
+    value:
+      background_std: 825.0799999999999
+      counts_background: 7357.276130193078
+      counts_total: 19516.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.155766468087255e-05
+  - name: R_13(pp->ee)
+    qmax: 300.0
+    qmin: 280.0
+    value:
+      background_std: 573.2
+      counts_background: 5584.933994927697
+      counts_total: 14567.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00011016301194453936
+  - name: R_13(pp->ee)
+    qmax: 320.0
+    qmin: 300.0
+    value:
+      background_std: 503.56
+      counts_background: 4209.347379552479
+      counts_total: 11186.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00014385852867420914
+  - name: R_13(pp->ee)
+    qmax: 340.0
+    qmin: 320.0
+    value:
+      background_std: 378.2
+      counts_background: 3272.09838538474
+      counts_total: 8636.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00018368143643359973
+  - name: R_13(pp->ee)
+    qmax: 360.0
+    qmin: 340.0
+    value:
+      background_std: 277.65999999999997
+      counts_background: 2520.9115446466994
+      counts_total: 6792.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00023468800216940207
+  - name: R_13(pp->ee)
+    qmax: 380.0
+    qmin: 360.0
+    value:
+      background_std: 261.12
+      counts_background: 1965.7874049761576
+      counts_total: 5293.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00029240951422857697
+  - name: R_13(pp->ee)
+    qmax: 400.0
+    qmin: 380.0
+    value:
+      background_std: 183.15200000000002
+      counts_background: 1540.8834033307726
+      counts_total: 4123.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003691215976650462
+  - name: R_13(pp->ee)
+    qmax: 420.0
+    qmin: 400.0
+    value:
+      background_std: 176.508
+      counts_background: 1192.8079955350063
+      counts_total: 3360.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00045310061385788814
+  - name: R_13(pp->ee)
+    qmax: 440.0
+    qmin: 420.0
+    value:
+      background_std: 116.69800000000001
+      counts_background: 949.8991571044012
+      counts_total: 2759.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005574191289649166
+  - name: R_13(pp->ee)
+    qmax: 460.0
+    qmin: 440.0
+    value:
+      background_std: 102.814
+      counts_background: 744.3888596458787
+      counts_total: 2228.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006851301539404938
+  - name: R_13(pp->ee)
+    qmax: 480.0
+    qmin: 460.0
+    value:
+      background_std: 76.174
+      counts_background: 613.8448255204651
+      counts_total: 1748.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0008196203893736208
+  - name: R_13(pp->ee)
+    qmax: 500.0
+    qmin: 480.0
+    value:
+      background_std: 64.512
+      counts_background: 552.8919083889597
+      counts_total: 1528.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0009565562876769117
+  - name: R_13(pp->ee)
+    qmax: 520.0
+    qmin: 500.0
+    value:
+      background_std: 71.322
+      counts_background: 410.8680174026359
+      counts_total: 1234.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0011664459120967233
+  - name: R_13(pp->ee)
+    qmax: 540.0
+    qmin: 520.0
+    value:
+      background_std: 47.248000000000005
+      counts_background: 325.94648171940497
+      counts_total: 1059.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0013481335925621426
+  - name: R_13(pp->ee)
+    qmax: 560.0
+    qmin: 540.0
+    value:
+      background_std: 40.428
+      counts_background: 265.285722961996
+      counts_total: 864.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.001591944132329856
+  - name: R_13(pp->ee)
+    qmax: 580.0
+    qmin: 560.0
+    value:
+      background_std: 36.858
+      counts_background: 212.9764655631463
+      counts_total: 751.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0018919061959419181
+  - name: R_13(pp->ee)
+    qmax: 600.0
+    qmin: 580.0
+    value:
+      background_std: 31.808
+      counts_background: 177.1274638240017
+      counts_total: 661.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0021567037701779855
+  - name: R_13(pp->ee)
+    qmax: 630.0
+    qmin: 600.0
+    value:
+      background_std: 51.794999999999995
+      counts_background: 209.31038175967637
+      counts_total: 792.99
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0017529219450267489
+  - name: R_13(pp->ee)
+    qmax: 660.0
+    qmin: 630.0
+    value:
+      background_std: 29.1948
+      counts_background: 159.78309327380316
+      counts_total: 639.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0021277297761460446
+  - name: R_13(pp->ee)
+    qmax: 690.0
+    qmin: 660.0
+    value:
+      background_std: 26.3487
+      counts_background: 121.75724499497386
+      counts_total: 515.01
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0025513994426335095
+  - name: R_13(pp->ee)
+    qmax: 720.0
+    qmin: 690.0
+    value:
+      background_std: 23.1792
+      counts_background: 95.56950371499626
+      counts_total: 432.99
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0031526945254715675
+  - name: R_13(pp->ee)
+    qmax: 750.0
+    qmin: 720.0
+    value:
+      background_std: 18.7224
+      counts_background: 73.36660983912986
+      counts_total: 374.01
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003894178755251911
+  - name: R_13(pp->ee)
+    qmax: 780.0
+    qmin: 750.0
+    value:
+      background_std: 16.341900000000003
+      counts_background: 58.42590015045859
+      counts_total: 311.01000000000005
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004796416903378421
+  - name: R_13(pp->ee)
+    qmax: 810.0
+    qmin: 780.0
+    value:
+      background_std: 15.481200000000001
+      counts_background: 47.350570421484804
+      counts_total: 204.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0050987105983517035
+  - name: R_13(pp->ee)
+    qmax: 840.0
+    qmin: 810.0
+    value:
+      background_std: 16.727700000000002
+      counts_background: 36.688714089415356
+      counts_total: 207.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00666658159963576
+  - name: R_13(pp->ee)
+    qmax: 870.0
+    qmin: 840.0
+    value:
+      background_std: 8.4702
+      counts_background: 31.132090758979373
+      counts_total: 156.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007763116663687077
+  - name: R_13(pp->ee)
+    qmax: 900.0
+    qmin: 870.0
+    value:
+      background_std: 7.5906
+      counts_background: 25.24566295052275
+      counts_total: 123.99900000000001
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00916131584214694
+  - name: R_13(pp->ee)
+    qmax: 950.0
+    qmin: 900.0
+    value:
+      background_std: 13.5435
+      counts_background: 31.693745296404508
+      counts_total: 177.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.006738614100882317
+  - name: R_13(pp->ee)
+    qmax: 1000.0
+    qmin: 950.0
+    value:
+      background_std: 8.2165
+      counts_background: 21.460668927830792
+      counts_total: 156.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.008662068824143233
+  - name: R_13(pp->ee)
+    qmax: 1050.0
+    qmin: 1000.0
+    value:
+      background_std: 6.4415
+      counts_background: 15.592370207910204
+      counts_total: 86.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01108553228972087
+  - name: R_13(pp->ee)
+    qmax: 1100.0
+    qmin: 1050.0
+    value:
+      background_std: 6.010999999999999
+      counts_background: 11.46937029942327
+      counts_total: 78.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.014635697669161283
+  - name: R_13(pp->ee)
+    qmax: 1150.0
+    qmin: 1100.0
+    value:
+      background_std: 4.5796
+      counts_background: 8.285761645490192
+      counts_total: 78.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01788001026268359
+  - name: R_13(pp->ee)
+    qmax: 1200.0
+    qmin: 1150.0
+    value:
+      background_std: 3.70115
+      counts_background: 6.6757844613718555
+      counts_total: 49.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.022008641076998608
+  - name: R_13(pp->ee)
+    qmax: 1250.0
+    qmin: 1200.0
+    value:
+      background_std: 3.2655999999999996
+      counts_background: 5.575763857625475
+      counts_total: 41.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.027981768594955717
+  - name: R_13(pp->ee)
+    qmax: 1310.0
+    qmin: 1250.0
+    value:
+      background_std: 3.82956
+      counts_background: 3.881897282598377
+      counts_total: 43.0002
+      distribution: general_gamma_counting_process
+      scale_factor: 0.028189579357832086
+  - name: R_13(pp->ee)
+    qmax: 1370.0
+    qmin: 1310.0
+    value:
+      background_std: 2.62758
+      counts_background: 3.2894898320115833
+      counts_total: 31.999799999999997
+      distribution: general_gamma_counting_process
+      scale_factor: 0.03673021166475208
+  - name: R_13(pp->ee)
+    qmax: 1430.0
+    qmin: 1370.0
+    value:
+      background_std: 2.13912
+      counts_background: 2.284604311977587
+      counts_total: 21.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04652771203325717
+  - name: R_13(pp->ee)
+    qmax: 1490.0
+    qmin: 1430.0
+    value:
+      background_std: 1.6299000000000001
+      counts_background: 2.087200658059648
+      counts_total: 25.0002
+      distribution: general_gamma_counting_process
+      scale_factor: 0.05873387586884946
+  - name: R_13(pp->ee)
+    qmax: 1550.0
+    qmin: 1490.0
+    value:
+      background_std: 1.45494
+      counts_background: 1.6126939070940605
+      counts_total: 15.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07454984333853684
+  - name: R_13(pp->ee)
+    qmax: 1610.0
+    qmin: 1550.0
+    value:
+      background_std: 1.13382
+      counts_background: 1.2053884468044034
+      counts_total: 15.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.09252397592977303
+  - name: R_13(pp->ee)
+    qmax: 1680.0
+    qmin: 1610.0
+    value:
+      background_std: 1.1050200000000001
+      counts_background: 1.2236338923922696
+      counts_total: 8.0003
+      distribution: general_gamma_counting_process
+      scale_factor: 0.09901519789954959
+  - name: R_13(pp->ee)
+    qmax: 1750.0
+    qmin: 1680.0
+    value:
+      background_std: 0.84287
+      counts_background: 0.7179398345861289
+      counts_total: 10.9998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.1285584740549172
+  - name: R_13(pp->ee)
+    qmax: 1820.0
+    qmin: 1750.0
+    value:
+      background_std: 0.694645
+      counts_background: 0.5992312756337012
+      counts_total: 5.99998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.1598549448996265
+  - name: R_13(pp->ee)
+    qmax: 1890.0
+    qmin: 1820.0
+    value:
+      background_std: 0.542717
+      counts_background: 0.4171331604714287
+      counts_total: 8.0003
+      distribution: general_gamma_counting_process
+      scale_factor: 0.206675088252884
+  - name: R_13(pp->ee)
+    qmax: 1970.0
+    qmin: 1890.0
+    value:
+      background_std: 0.5188159999999999
+      counts_background: 0.4448584092905549
+      counts_total: 8.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.23431764388882872
+  - name: R_13(pp->ee)
+    qmax: 2050.0
+    qmin: 1970.0
+    value:
+      background_std: 0.38783999999999996
+      counts_background: 0.2718923693807559
+      counts_total: 7.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.3023927197023978
+  - name: R_13(pp->ee)
+    qmax: 2130.0
+    qmin: 2050.0
+    value:
+      background_std: 0.318312
+      counts_background: 0.19291025053987376
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.37494084989808507
+  - name: R_13(pp->ee)
+    qmax: 2210.0
+    qmin: 2130.0
+    value:
+      background_std: 0.25441600000000003
+      counts_background: 0.14682564442984766
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4787234378231659
+  - name: R_13(pp->ee)
+    qmax: 2290.0
+    qmin: 2210.0
+    value:
+      background_std: 0.20824800000000002
+      counts_background: 0.12242352237028742
+      counts_total: 6.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.6067300756920204
+  - name: R_13(pp->ee)
+    qmax: 2370.0
+    qmin: 2290.0
+    value:
+      background_std: 0.15412800000000001
+      counts_background: 0.03659870197119725
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7842859691727891
+  - name: R_13(pp->ee)
+    qmax: 2450.0
+    qmin: 2370.0
+    value:
+      background_std: 0.13036799999999998
+      counts_background: 0.05425740153731319
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.9891962516528416
+  - name: R_13(pp->ee)
+    qmax: 2530.0
+    qmin: 2450.0
+    value:
+      background_std: 0.11268
+      counts_background: 0.08867544041149267
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2417554789784402
+  - name: R_13(pp->ee)
+    qmax: 2610.0
+    qmin: 2530.0
+    value:
+      background_std: 0.087152
+      counts_background: 0.04731888189610251
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.5573022859798031
+  - name: R_13(pp->ee)
+    qmax: 2690.0
+    qmin: 2610.0
+    value:
+      background_std: 0.0668904
+      counts_background: 0.01031996049958608
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.9354806861329976
+  - name: R_13(pp->ee)
+    qmax: 2770.0
+    qmin: 2690.0
+    value:
+      background_std: 0.0712488
+      counts_background: 0.10226825556454028
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.4135367513296275
+  - name: R_13(pp->ee)
+    qmax: 2850.0
+    qmin: 2770.0
+    value:
+      background_std: 0.0454984
+      counts_background: 0.013600717626224529
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.0264910547345614
+  - name: R_13(pp->ee)
+    qmax: 2930.0
+    qmin: 2850.0
+    value:
+      background_std: 0.0371568
+      counts_background: 0.005193782273644783
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.691785109129273
+  - name: R_13(pp->ee)
+    qmax: 3010.0
+    qmin: 2930.0
+    value:
+      background_std: 0.0305104
+      counts_background: 0.007141810885623472
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.663887518377184
+  - name: R_13(pp->ee)
+    qmax: 3090.0
+    qmin: 3010.0
+    value:
+      background_std: 0.026360799999999997
+      counts_background: 0.013010919352075259
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.759235271238098
+  - name: R_13(pp->ee)
+    qmax: 3170.0
+    qmin: 3090.0
+    value:
+      background_std: 0.0277448
+      counts_background: 0.051860368262802284
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.009412223973501
+  - name: R_13(pp->ee)
+    qmax: 3250.0
+    qmin: 3170.0
+    value:
+      background_std: 0.030994400000000002
+      counts_background: 0.035416108727459886
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.35099988620209
+  - name: R_13(pp->ee)
+    qmax: 3330.0
+    qmin: 3250.0
+    value:
+      background_std: 0.0145672
+      counts_background: 0.0021522017444984046
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 10.366255158725254
+  - name: R_13(pp->ee)
+    qmax: 3410.0
+    qmin: 3330.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 1.0
+      distribution: gamma_counting_process
+      scale_factor: 12.52151687913407
+  - name: R_13(pp->ee)
+    qmax: 3490.0
+    qmin: 3410.0
+    value:
+      counts_background: 0.010555316363877354
+      counts_total: 1.0
+      distribution: gamma_counting_process
+      scale_factor: 15.547386219091818
+  - name: R_13(pp->ee)
+    qmax: 3570.0
+    qmin: 3490.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 19.54576962703109
+  - name: R_13(pp->ee)
+    qmax: 3650.0
+    qmin: 3570.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 23.816659487454693
+  - name: R_13(pp->ee)
+    qmax: 3730.0
+    qmin: 3650.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 29.247683290763604
+  - name: R_13(pp->ee)
+    qmax: 3810.0
+    qmin: 3730.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 35.61698045164151
+  - name: R_13(pp->ee)
+    qmax: 3890.0
+    qmin: 3810.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 43.46630779273621
+  - name: R_13(pp->ee)
+    qmax: 3970.0
+    qmin: 3890.0
+    value:
+      counts_background: 0.0008000000000000042
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 53.23488853915603
+  - name: R_13(pp->ee)
+    qmax: 4070.0
+    qmin: 3970.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 53.474299420776646
+  - name: R_13(pp->ee)
+    qmax: 4170.0
+    qmin: 4070.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 67.81422641464671
+  - name: R_13(pp->ee)
+    qmax: 4270.0
+    qmin: 4170.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 89.82037585994424
+  - name: R_13(pp->ee)
+    qmax: 4370.0
+    qmin: 4270.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 120.95049004124854
+  - name: R_13(pp->ee)
+    qmax: 4470.0
+    qmin: 4370.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 153.0742674834596
+  - name: R_13(pp->ee)
+    qmax: 4570.0
+    qmin: 4470.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 206.8403584590284
+  - name: R_13(pp->ee)
+    qmax: 4670.0
+    qmin: 4570.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 276.6606293187612
+  - name: R_13(pp->ee)
+    qmax: 4770.0
+    qmin: 4670.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 371.59415210721096
+  - name: R_13(pp->ee)
+    qmax: 4870.0
+    qmin: 4770.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 532.0500353532797
+  - name: R_13(pp->ee)
+    qmax: 4970.0
+    qmin: 4870.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 759.7256104832346
+  - name: R_13(pp->ee)
+    qmax: 5070.0
+    qmin: 4970.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1321.11117251084
+  - name: R_13(pp->ee)
+    qmax: 5170.0
+    qmin: 5070.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2590.7112396792727
+  - name: R_13(pp->ee)
+    qmax: 5270.0
+    qmin: 5170.0
+    value:
+      counts_background: 0.0010000000000000052
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 17070.97424270547
+
+CMS pp->enu 2022:
+  experiment: CMS
+  inspire: CMS:2022yjm
+  values:
+  - mTmax: 480.0
+    mTmin: 440.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 501.97
+      counts_background: 685.3072038042317
+      counts_total: 3134.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00040351430141328756
+  - mTmax: 520.0
+    mTmin: 480.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 439.23
+      counts_background: 644.4853362180684
+      counts_total: 3565.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003292851481636881
+  - mTmax: 560.0
+    mTmin: 520.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 255.4
+      counts_background: 399.50539169043964
+      counts_total: 3124.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003576574602018139
+  - mTmax: 600.0
+    mTmin: 560.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 242.31
+      counts_background: 275.04985609378963
+      counts_total: 2364.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00047629376353495735
+  - mTmax: 640.0
+    mTmin: 600.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 189.27
+      counts_background: 186.2097158531025
+      counts_total: 1697.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006381973895586469
+  - mTmax: 680.0
+    mTmin: 640.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 170.35
+      counts_background: 131.44588921082314
+      counts_total: 1226.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0008572666374574982
+  - mTmax: 720.0
+    mTmin: 680.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 123.1
+      counts_background: 99.75085725305709
+      counts_total: 916.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0011387917950669679
+  - mTmax: 760.0
+    mTmin: 720.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 83.649
+      counts_background: 67.32603352969532
+      counts_total: 722.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0014857229199219265
+  - mTmax: 800.0
+    mTmin: 760.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 70.243
+      counts_background: 45.16482953991109
+      counts_total: 570.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0019496191682796162
+  - mTmax: 840.0
+    mTmin: 800.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 47.616
+      counts_background: 33.63482142821223
+      counts_total: 412.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0025113428260116377
+  - mTmax: 880.0
+    mTmin: 840.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 39.69
+      counts_background: 22.817237186465164
+      counts_total: 325.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.003196120193108419
+  - mTmax: 920.0
+    mTmin: 880.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 26.429
+      counts_background: 20.14611712961653
+      counts_total: 241.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004015067833021666
+  - mTmax: 960.0
+    mTmin: 920.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 31.361
+      counts_background: 21.33779422874737
+      counts_total: 192.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004949613109133107
+  - mTmax: 1000.0
+    mTmin: 960.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 31.685
+      counts_background: 10.462288337266457
+      counts_total: 173.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.006178535398397672
+  - mTmax: 1040.0
+    mTmin: 1000.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 22.718
+      counts_background: 8.2364967337828
+      counts_total: 126.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007722360294691018
+  - mTmax: 1080.0
+    mTmin: 1040.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 16.863
+      counts_background: 7.208204752796001
+      counts_total: 109.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00952799996465935
+  - mTmax: 1120.0
+    mTmin: 1080.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 13.256
+      counts_background: 4.713904702816089
+      counts_total: 99.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.011551867222248177
+  - mTmax: 1160.0
+    mTmin: 1120.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 15.139
+      counts_background: 4.225768874893042
+      counts_total: 82.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.013966595186166554
+  - mTmax: 1200.0
+    mTmin: 1160.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 11.375
+      counts_background: 3.001231231747037
+      counts_total: 63.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.016929148001889983
+  - mTmax: 1240.0
+    mTmin: 1200.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 10.977
+      counts_background: 2.5922113788551777
+      counts_total: 47.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.020265964296760555
+  - mTmax: 1280.0
+    mTmin: 1240.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 7.6228
+      counts_background: 2.6190116562657138
+      counts_total: 40.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.023939498404411515
+  - mTmax: 1320.0
+    mTmin: 1280.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 6.1609
+      counts_background: 1.573961256203003
+      counts_total: 38.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.028730616614956808
+  - mTmax: 1360.0
+    mTmin: 1320.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 5.2559
+      counts_background: 0.6485946929919203
+      counts_total: 32.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0340336358387083
+  - mTmax: 1400.0
+    mTmin: 1360.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 4.2782
+      counts_background: 0.832983149755952
+      counts_total: 20.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.040274915713912125
+  - mTmax: 1440.0
+    mTmin: 1400.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 5.4857
+      counts_background: 1.3645868087194162
+      counts_total: 25.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04719625551724325
+  - mTmax: 1480.0
+    mTmin: 1440.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 3.49
+      counts_background: 0.44300437972202733
+      counts_total: 23.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.056233694452867626
+  - mTmax: 1520.0
+    mTmin: 1480.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 2.5741
+      counts_background: 0.20870676586246678
+      counts_total: 13.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.06498927776787096
+  - mTmax: 1560.0
+    mTmin: 1520.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 3.3212
+      counts_background: 0.2564063893309645
+      counts_total: 16.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07583440382285062
+  - mTmax: 1600.0
+    mTmin: 1560.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 2.0185
+      counts_background: 0.209194084111491
+      counts_total: 12.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.08938833073551904
+  - mTmax: 1640.0
+    mTmin: 1600.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.7531
+      counts_background: 0.1679213170930752
+      counts_total: 15.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.10545901859592784
+  - mTmax: 1680.0
+    mTmin: 1640.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.5246
+      counts_background: 0.13160544250175407
+      counts_total: 12.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.12387817062794133
+  - mTmax: 1720.0
+    mTmin: 1680.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.4026
+      counts_background: 0.11055903601049938
+      counts_total: 8.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.13752768400781568
+  - mTmax: 1760.0
+    mTmin: 1720.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 2.5328
+      counts_background: 2.5087896803124643
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.1629184136167086
+  - mTmax: 1800.0
+    mTmin: 1760.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.1538
+      counts_background: 0.06619339776543717
+      counts_total: 6.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.1871574339330256
+  - mTmax: 1840.0
+    mTmin: 1800.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.92291
+      counts_background: 0.053245154792676636
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2148086227331264
+  - mTmax: 1880.0
+    mTmin: 1840.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 1.0027
+      counts_background: 0.041535780021137766
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.24684186286132442
+  - mTmax: 1920.0
+    mTmin: 1880.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.77083
+      counts_background: 0.039014917536967314
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.28207976992703687
+  - mTmax: 1960.0
+    mTmin: 1920.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.64178
+      counts_background: 0.027335623537809647
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.33256622030614635
+  - mTmax: 2000.0
+    mTmin: 1960.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.57077
+      counts_background: 0.022402545517260553
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.3673999580575091
+  - mTmax: 2040.0
+    mTmin: 2000.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.48499
+      counts_background: 0.0199093237708316
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4239358581749618
+  - mTmax: 2080.0
+    mTmin: 2040.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.38061
+      counts_background: 0.01965968794786311
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4824559748838243
+  - mTmax: 2120.0
+    mTmin: 2080.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.38448
+      counts_background: 0.011628533017902332
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5495914693296035
+  - mTmax: 2160.0
+    mTmin: 2120.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.34595
+      counts_background: 0.009579146676611621
+      counts_total: 4.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.623955531974494
+  - mTmax: 2200.0
+    mTmin: 2160.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.28751
+      counts_background: 0.008011712568570733
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7074818523005214
+  - mTmax: 2240.0
+    mTmin: 2200.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.23162
+      counts_background: 0.006308775741799536
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7989192358762129
+  - mTmax: 2280.0
+    mTmin: 2240.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.20254
+      counts_background: 0.0044627108367266645
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.9143662126858789
+  - mTmax: 2320.0
+    mTmin: 2280.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.19719
+      counts_background: 0.005082597943113806
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.0230199000284124
+  - mTmax: 2360.0
+    mTmin: 2320.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.18762
+      counts_background: 0.0037541919568823347
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.1612271443491535
+  - mTmax: 2400.0
+    mTmin: 2360.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.18722
+      counts_background: 0.0028450425695979074
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.325232552423057
+  - mTmax: 2440.0
+    mTmin: 2400.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.17188
+      counts_background: 0.0021370631189208847
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.4896051134189534
+  - mTmax: 2480.0
+    mTmin: 2440.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.13257
+      counts_background: 0.0022211028495023053
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.6699196961583411
+  - mTmax: 2520.0
+    mTmin: 2480.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.13645
+      counts_background: 0.0019799413836670806
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.9182667001927447
+  - mTmax: 2560.0
+    mTmin: 2520.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.10515
+      counts_background: 0.0014840411935617846
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1601846033228607
+  - mTmax: 2600.0
+    mTmin: 2560.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.092711
+      counts_background: 0.0011834381765836062
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.3730181406223143
+  - mTmax: 2640.0
+    mTmin: 2600.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.08817
+      counts_background: 0.0011685994725399921
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.7074806707651002
+  - mTmax: 2680.0
+    mTmin: 2640.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.085141
+      counts_background: 0.0008704790452127665
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.0513731023759347
+  - mTmax: 2720.0
+    mTmin: 2680.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.071156
+      counts_background: 0.0006357794469504392
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.409319330842205
+  - mTmax: 2760.0
+    mTmin: 2720.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.072658
+      counts_background: 0.0005918956143543814
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.8955165503372227
+  - mTmax: 2800.0
+    mTmin: 2760.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.06468
+      counts_background: 0.00039072955175135677
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.385738487000358
+  - mTmax: 2840.0
+    mTmin: 2800.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.05076
+      counts_background: 0.000467508353036048
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.922818728757035
+  - mTmax: 2880.0
+    mTmin: 2840.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.046606
+      counts_background: 0.00045938822644943643
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.486107009294341
+  - mTmax: 2920.0
+    mTmin: 2880.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.045623
+      counts_background: 0.00042017583423266624
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.163594225294338
+  - mTmax: 2960.0
+    mTmin: 2920.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.038283
+      counts_background: 0.0003646311259646446
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.734679925008108
+  - mTmax: 3000.0
+    mTmin: 2960.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.034014
+      counts_background: 0.0004237336825973172
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.542948219632239
+  - mTmax: 3040.0
+    mTmin: 3000.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.03435
+      counts_background: 0.00030318458293856663
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.452308090337233
+  - mTmax: 3080.0
+    mTmin: 3040.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.028267
+      counts_background: 0.00014293785953370378
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 9.408209496142524
+  - mTmax: 3120.0
+    mTmin: 3080.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.0266
+      counts_background: 0.00010191288807335522
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 10.397064314095664
+  - mTmax: 3160.0
+    mTmin: 3120.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.025352
+      counts_background: 0.0001066642884313102
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 11.74761209882719
+  - mTmax: 3200.0
+    mTmin: 3160.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.022381
+      counts_background: 0.00015515063886983884
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 12.995949212293445
+  - mTmax: 3240.0
+    mTmin: 3200.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.020585
+      counts_background: 5.5808551490762533e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 14.605886754313671
+  - mTmax: 3280.0
+    mTmin: 3240.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.018963
+      counts_background: 0.0001632506511005
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 16.341790746048606
+  - mTmax: 3320.0
+    mTmin: 3280.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.018016
+      counts_background: 0.00010756747070226397
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 18.259238605214104
+  - mTmax: 3360.0
+    mTmin: 3320.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.016291
+      counts_background: 4.9113472466873746e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 20.473452275951285
+  - mTmax: 3400.0
+    mTmin: 3360.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.015632
+      counts_background: 7.388068144672712e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 22.892370082613876
+  - mTmax: 3440.0
+    mTmin: 3400.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.014362
+      counts_background: 4.854408153932544e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 25.603296206579888
+  - mTmax: 3480.0
+    mTmin: 3440.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.01251
+      counts_background: 9.951593682421527e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 28.943093473363724
+  - mTmax: 3520.0
+    mTmin: 3480.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.011143
+      counts_background: 6.128742813172941e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 31.859729026500546
+  - mTmax: 3560.0
+    mTmin: 3520.0
+    name: R_13(pp->enu)
+    value:
+      background_std: 0.011037
+      counts_background: 6.457970483823947e-05
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 35.95503886561246
+  - mTmax: 3600.0
+    mTmin: 3560.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 6.256125241000559e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 39.43628455173676
+  - mTmax: 3640.0
+    mTmin: 3600.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.7754294506719074e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 43.72361211652484
+  - mTmax: 3680.0
+    mTmin: 3640.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.144376967443529e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 49.396519836963265
+  - mTmax: 3720.0
+    mTmin: 3680.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.76667038826407e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 54.569603133326474
+  - mTmax: 3760.0
+    mTmin: 3720.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.4438482116017164e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 60.18933491086574
+  - mTmax: 3800.0
+    mTmin: 3760.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.9541190843992314e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 66.66439351398762
+  - mTmax: 3840.0
+    mTmin: 3800.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.3146947292629724e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 75.59575077085653
+  - mTmax: 3880.0
+    mTmin: 3840.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.433095589581751e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 85.04093468303768
+  - mTmax: 3920.0
+    mTmin: 3880.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.1029300804576948e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 95.7608380914255
+  - mTmax: 3960.0
+    mTmin: 3920.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.2547047458090992e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 105.34091255960409
+  - mTmax: 4000.0
+    mTmin: 3960.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 8.367632438657121e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 116.65755896836576
+  - mTmax: 4040.0
+    mTmin: 4000.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.6837248797654785e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 130.062468100625
+  - mTmax: 4080.0
+    mTmin: 4040.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.188176009647675e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 145.47597794763095
+  - mTmax: 4120.0
+    mTmin: 4080.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.4558536757004545e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 161.8043892068633
+  - mTmax: 4160.0
+    mTmin: 4120.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 6.205610359708174e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 180.56714061251841
+  - mTmax: 4200.0
+    mTmin: 4160.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.451282835139922e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 201.8731427183309
+  - mTmax: 4240.0
+    mTmin: 4200.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.3635729766936592e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 222.38462079621561
+  - mTmax: 4280.0
+    mTmin: 4240.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.008701554240836e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 251.33693320815155
+  - mTmax: 4320.0
+    mTmin: 4280.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.3414295736258857e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 279.2313394320861
+  - mTmax: 4360.0
+    mTmin: 4320.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.229524581534205e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 311.1327925918976
+  - mTmax: 4400.0
+    mTmin: 4360.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.411695270795707e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 346.99392140335146
+  - mTmax: 4440.0
+    mTmin: 4400.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.2732795888735984e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 387.2370369366454
+  - mTmax: 4480.0
+    mTmin: 4440.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 6.864497891881006e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 423.0247210131223
+  - mTmax: 4520.0
+    mTmin: 4480.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.6460212003729596e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 479.26539729100654
+  - mTmax: 4560.0
+    mTmin: 4520.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.9778450955356363e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 529.5462239419633
+  - mTmax: 4600.0
+    mTmin: 4560.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.1422177389833648e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 588.4795816449404
+  - mTmax: 4640.0
+    mTmin: 4600.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.568658940879077e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 641.6218528299648
+  - mTmax: 4680.0
+    mTmin: 4640.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 7.984791155377944e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 739.7169892646519
+  - mTmax: 4720.0
+    mTmin: 4680.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.933671508180186e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 817.0966718872296
+  - mTmax: 4760.0
+    mTmin: 4720.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.5879126959008846e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 923.052568298723
+  - mTmax: 4800.0
+    mTmin: 4760.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.463181630904389e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1024.921164912806
+  - mTmax: 4840.0
+    mTmin: 4800.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.4916616734128875e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1126.9224541487863
+  - mTmax: 4880.0
+    mTmin: 4840.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.1274323266335804e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1261.328656514209
+  - mTmax: 4920.0
+    mTmin: 4880.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.053739792937742e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1399.956650748852
+  - mTmax: 4960.0
+    mTmin: 4920.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 6.437479818647312e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1556.5676804062232
+  - mTmax: 5000.0
+    mTmin: 4960.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.2567644552441648e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1725.0367751950323
+  - mTmax: 5040.0
+    mTmin: 5000.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.0649766439065436e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1926.8436826238556
+  - mTmax: 5080.0
+    mTmin: 5040.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.203325412649544e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2200.0798405391024
+  - mTmax: 5120.0
+    mTmin: 5080.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.726041742087404e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2431.632204644033
+  - mTmax: 5160.0
+    mTmin: 5120.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.867252783972797e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2718.112410092839
+  - mTmax: 5200.0
+    mTmin: 5160.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.508233519284025e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 3008.976091121458
+  - mTmax: 5240.0
+    mTmin: 5200.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.0779837251972395e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 3334.2145126687037
+  - mTmax: 5280.0
+    mTmin: 5240.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.08220717552389e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 3806.2889448599876
+  - mTmax: 5320.0
+    mTmin: 5280.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.056137264655654e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 4249.926131229805
+  - mTmax: 5360.0
+    mTmin: 5320.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.6799186385319906e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 4731.248722398351
+  - mTmax: 5400.0
+    mTmin: 5360.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.085987506298277e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 5383.345343434887
+  - mTmax: 5440.0
+    mTmin: 5400.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.8102184195864776e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 5873.857074774798
+  - mTmax: 5480.0
+    mTmin: 5440.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.8595231077256377e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 6747.657716416054
+  - mTmax: 5520.0
+    mTmin: 5480.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.394244779141172e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 7595.5462082709255
+  - mTmax: 5560.0
+    mTmin: 5520.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.2235001397255476e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 8458.483598060082
+  - mTmax: 5600.0
+    mTmin: 5560.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.850516627508042e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 9430.046128517019
+  - mTmax: 5640.0
+    mTmin: 5600.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.1649513034681135e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 10444.011421248497
+  - mTmax: 5680.0
+    mTmin: 5640.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.9345015733457527e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 12015.202010246
+  - mTmax: 5720.0
+    mTmin: 5680.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.162264152635207e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 14034.044059440228
+  - mTmax: 5760.0
+    mTmin: 5720.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.1816500531249325e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 15494.549440110264
+  - mTmax: 5800.0
+    mTmin: 5760.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.6000993590612424e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 18595.43125956885
+  - mTmax: 5840.0
+    mTmin: 5800.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.5627718461191266e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 20242.67342818032
+  - mTmax: 5880.0
+    mTmin: 5840.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.0161903792706209e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 23810.403295865148
+  - mTmax: 5920.0
+    mTmin: 5880.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.587251669707391e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 28930.870155265697
+  - mTmax: 5960.0
+    mTmin: 5920.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 7.940236065855564e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 34292.65787119252
+  - mTmax: 6000.0
+    mTmin: 5960.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.1407201667677625e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 41917.90208558081
+  - mTmax: 6040.0
+    mTmin: 6000.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 9.141031598388679e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 48730.75432539665
+  - mTmax: 6080.0
+    mTmin: 6040.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.8298781084494e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 61303.17657131522
+  - mTmax: 6120.0
+    mTmin: 6080.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 7.301666926456176e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 71972.85379834744
+  - mTmax: 6160.0
+    mTmin: 6120.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 7.822411433375862e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 84399.47027772808
+  - mTmax: 6200.0
+    mTmin: 6160.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.1984038714329863e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 104247.40628284871
+  - mTmax: 6240.0
+    mTmin: 6200.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.334706140812458e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 120654.25879817129
+  - mTmax: 6280.0
+    mTmin: 6240.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 8.431783902619568e-09
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 138282.82359883687
+  - mTmax: 6320.0
+    mTmin: 6280.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.813155029970277e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 147160.81217761873
+  - mTmax: 6360.0
+    mTmin: 6320.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.8683753799690182e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 185079.06169890647
+  - mTmax: 6400.0
+    mTmin: 6360.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.057573799375826e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 201366.51979006067
+  - mTmax: 6440.0
+    mTmin: 6400.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 5.453927004120833e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 256598.79611338233
+  - mTmax: 6480.0
+    mTmin: 6440.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.0671716027220986e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 290725.740290646
+  - mTmax: 6520.0
+    mTmin: 6480.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.2663346806840298e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 306606.1018124745
+  - mTmax: 6560.0
+    mTmin: 6520.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.4034117459171998e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 203881.97724314997
+  - mTmax: 6600.0
+    mTmin: 6560.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.014975731391466e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 380179.1236037249
+  - mTmax: 6640.0
+    mTmin: 6600.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 4.845789870131363e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 434810.8763701932
+  - mTmax: 6680.0
+    mTmin: 6640.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.5824822650566445e-10
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 499659.12945690413
+  - mTmax: 6720.0
+    mTmin: 6680.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.2807492962060854e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 578459.754922838
+  - mTmax: 6760.0
+    mTmin: 6720.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.8269203880691544e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 607516.8058698938
+  - mTmax: 6800.0
+    mTmin: 6760.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 3.5833460107032355e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 754965.9379987472
+  - mTmax: 6840.0
+    mTmin: 6800.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.3478336481166037e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 309643.4904872193
+  - mTmax: 6880.0
+    mTmin: 6840.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.8561472679585762e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 830098.0727409918
+  - mTmax: 6920.0
+    mTmin: 6880.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.164606019346795e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 858995.7601462529
+  - mTmax: 6960.0
+    mTmin: 6920.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 1.8470459358825692e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 766507.7165064398
+  - mTmax: 7000.0
+    mTmin: 6960.0
+    name: R_13(pp->enu)
+    value:
+      counts_background: 2.727124618225561e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1041350.6277935408
+
+CMS pp->mumu 2021:
+  experiment: CMS
+  inspire: CMS:2021ctt
+  values:
+  - name: R_13(pp->mumu)
+    qmax: 129.95
+    qmin: 120.0
+    value:
+      background_std: 7121.214999999992
+      counts_background: 9737.824805766377
+      counts_total: 161836.74999999983
+      distribution: general_gamma_counting_process
+      scale_factor: 6.63886219674713e-06
+  - name: R_13(pp->mumu)
+    qmax: 140.74
+    qmin: 129.95
+    value:
+      background_std: 5933.636800000011
+      counts_background: 12407.694138500712
+      counts_total: 148750.9400000003
+      distribution: general_gamma_counting_process
+      scale_factor: 7.545316742608385e-06
+  - name: R_13(pp->mumu)
+    qmax: 152.41
+    qmin: 140.74
+    value:
+      background_std: 4336.571999999996
+      counts_background: 13023.632672379501
+      counts_total: 118462.16999999987
+      distribution: general_gamma_counting_process
+      scale_factor: 9.820692631382591e-06
+  - name: R_13(pp->mumu)
+    qmax: 165.05
+    qmin: 152.41
+    value:
+      background_std: 4070.8384000000046
+      counts_background: 15090.863954325916
+      counts_total: 109457.34400000013
+      distribution: general_gamma_counting_process
+      scale_factor: 1.026474768552655e-05
+  - name: R_13(pp->mumu)
+    qmax: 178.75
+    qmin: 165.05
+    value:
+      background_std: 2827.6799999999976
+      counts_background: 15596.582516983219
+      counts_total: 91418.72999999992
+      distribution: general_gamma_counting_process
+      scale_factor: 1.3359013205124682e-05
+  - name: R_13(pp->mumu)
+    qmax: 193.57
+    qmin: 178.75
+    value:
+      background_std: 2144.157599999999
+      counts_background: 15039.387246468696
+      counts_total: 74643.89399999996
+      distribution: general_gamma_counting_process
+      scale_factor: 1.713588935538449e-05
+  - name: R_13(pp->mumu)
+    qmax: 209.63
+    qmin: 193.57
+    value:
+      background_std: 1699.4692000000002
+      counts_background: 14440.315894195808
+      counts_total: 60618.47000000001
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1364661053439985e-05
+  - name: R_13(pp->mumu)
+    qmax: 227.02
+    qmin: 209.63
+    value:
+      background_std: 1391.0087100000012
+      counts_background: 13115.370944250135
+      counts_total: 49128.48900000004
+      distribution: general_gamma_counting_process
+      scale_factor: 2.6772501957072506e-05
+  - name: R_13(pp->mumu)
+    qmax: 245.86
+    qmin: 227.02
+    value:
+      background_std: 1108.0934400000003
+      counts_background: 11846.440962160255
+      counts_total: 41800.308000000005
+      distribution: general_gamma_counting_process
+      scale_factor: 3.3343378325497194e-05
+  - name: R_13(pp->mumu)
+    qmax: 266.25
+    qmin: 245.86
+    value:
+      background_std: 905.1120999999994
+      counts_background: 9906.311130469863
+      counts_total: 32648.46799999998
+      distribution: general_gamma_counting_process
+      scale_factor: 4.333015127353089e-05
+  - name: R_13(pp->mumu)
+    qmax: 288.34
+    qmin: 266.25
+    value:
+      background_std: 739.9929099999993
+      counts_background: 8459.131839730098
+      counts_total: 26435.10299999997
+      distribution: general_gamma_counting_process
+      scale_factor: 5.416300782576308e-05
+  - name: R_13(pp->mumu)
+    qmax: 312.26
+    qmin: 288.34
+    value:
+      background_std: 613.7872000000004
+      counts_background: 6882.0943276267335
+      counts_total: 21187.618400000014
+      distribution: general_gamma_counting_process
+      scale_factor: 6.827104799814105e-05
+  - name: R_13(pp->mumu)
+    qmax: 338.16
+    qmin: 312.26
+    value:
+      background_std: 503.44420000000065
+      counts_background: 5550.806232855154
+      counts_total: 16796.668000000023
+      distribution: general_gamma_counting_process
+      scale_factor: 8.800172302419657e-05
+  - name: R_13(pp->mumu)
+    qmax: 366.21
+    qmin: 338.16
+    value:
+      background_std: 396.76724999999936
+      counts_background: 4372.215083799877
+      counts_total: 13169.75549999998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00011458770545969887
+  - name: R_13(pp->mumu)
+    qmax: 396.59
+    qmin: 366.21
+    value:
+      background_std: 311.09119999999996
+      counts_background: 3412.248229472873
+      counts_total: 10490.213999999998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001445235611100018
+  - name: R_13(pp->mumu)
+    qmax: 429.49
+    qmin: 396.59
+    value:
+      background_std: 242.26244000000025
+      counts_background: 2479.7114595669227
+      counts_total: 7649.9080000000085
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001890272305312742
+  - name: R_13(pp->mumu)
+    qmax: 465.12
+    qmin: 429.49
+    value:
+      background_std: 193.88064499999996
+      counts_background: 1987.848217691081
+      counts_total: 6128.003699999999
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0002363895586520066
+  - name: R_13(pp->mumu)
+    qmax: 503.71
+    qmin: 465.12
+    value:
+      background_std: 167.36482999999987
+      counts_background: 1538.0020215451727
+      counts_total: 4612.662699999997
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00031051332441116075
+  - name: R_13(pp->mumu)
+    qmax: 545.49
+    qmin: 503.71
+    value:
+      background_std: 140.1510100000001
+      counts_background: 997.3104239944079
+      counts_total: 3456.5429600000025
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0004196882985300517
+  - name: R_13(pp->mumu)
+    qmax: 590.74
+    qmin: 545.49
+    value:
+      background_std: 112.667975
+      counts_background: 738.2701471866559
+      counts_total: 2634.9075
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0005196990623977533
+  - name: R_13(pp->mumu)
+    qmax: 639.75
+    qmin: 590.74
+    value:
+      background_std: 85.89492599999998
+      counts_background: 505.9382896444369
+      counts_total: 1979.1708299999998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0007040851580270638
+  - name: R_13(pp->mumu)
+    qmax: 692.82
+    qmin: 639.75
+    value:
+      background_std: 64.87276800000005
+      counts_background: 340.5871490233496
+      counts_total: 1477.9464300000013
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0009281468484802702
+  - name: R_13(pp->mumu)
+    qmax: 750.29
+    qmin: 692.82
+    value:
+      background_std: 50.74600999999993
+      counts_background: 242.94975272099649
+      counts_total: 1015.9546599999985
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012415543238572756
+  - name: R_13(pp->mumu)
+    qmax: 812.54
+    qmin: 750.29
+    value:
+      background_std: 37.176944999999996
+      counts_background: 164.68857675237646
+      counts_total: 759.0765
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0016202682492240407
+  - name: R_13(pp->mumu)
+    qmax: 879.94
+    qmin: 812.54
+    value:
+      background_std: 26.577842000000036
+      counts_background: 103.10131781332407
+      counts_total: 573.9581800000008
+      distribution: general_gamma_counting_process
+      scale_factor: 0.00221828186409762
+  - name: R_13(pp->mumu)
+    qmax: 952.94
+    qmin: 879.94
+    value:
+      background_std: 20.075000000000003
+      counts_background: 71.69678067685018
+      counts_total: 389.017
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0030160058310544184
+  - name: R_13(pp->mumu)
+    qmax: 1032.0
+    qmin: 952.94
+    value:
+      background_std: 16.01834659999999
+      counts_background: 48.64362460396296
+      counts_total: 295.0282019999998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.004107093994648557
+  - name: R_13(pp->mumu)
+    qmax: 1117.6
+    qmin: 1032.0
+    value:
+      background_std: 10.96707199999999
+      counts_background: 28.973708612553843
+      counts_total: 201.9731999999998
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0056315816930471016
+  - name: R_13(pp->mumu)
+    qmax: 1210.3
+    qmin: 1117.6
+    value:
+      background_std: 7.776973800000003
+      counts_background: 18.975917552292035
+      counts_total: 131.98626000000007
+      distribution: general_gamma_counting_process
+      scale_factor: 0.007737418112646101
+  - name: R_13(pp->mumu)
+    qmax: 1310.7
+    qmin: 1210.3
+    value:
+      background_std: 5.860348000000005
+      counts_background: 11.777595389144965
+      counts_total: 106.99628000000011
+      distribution: general_gamma_counting_process
+      scale_factor: 0.010670808626178873
+  - name: R_13(pp->mumu)
+    qmax: 1419.4
+    qmin: 1310.7
+    value:
+      background_std: 4.029617700000002
+      counts_background: 7.110327399502672
+      counts_total: 70.97892600000003
+      distribution: general_gamma_counting_process
+      scale_factor: 0.015432354256804488
+  - name: R_13(pp->mumu)
+    qmax: 1537.2
+    qmin: 1419.4
+    value:
+      background_std: 2.8347391999999987
+      counts_background: 4.744557257978962
+      counts_total: 59.023689999999974
+      distribution: general_gamma_counting_process
+      scale_factor: 0.022300989477252738
+  - name: R_13(pp->mumu)
+    qmax: 1664.7
+    qmin: 1537.2
+    value:
+      background_std: 2.4225
+      counts_background: 4.736851544736749
+      counts_total: 26.995575
+      distribution: general_gamma_counting_process
+      scale_factor: 0.03226492701949835
+  - name: R_13(pp->mumu)
+    qmax: 1802.8
+    qmin: 1664.7
+    value:
+      background_std: 1.349043659999999
+      counts_background: 1.9522842499239974
+      counts_total: 17.99995399999999
+      distribution: general_gamma_counting_process
+      scale_factor: 0.04763836260928834
+  - name: R_13(pp->mumu)
+    qmax: 1952.4
+    qmin: 1802.8
+    value:
+      background_std: 1.137348960000001
+      counts_background: 2.5046589020574546
+      counts_total: 13.003980000000013
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07099243307721687
+  - name: R_13(pp->mumu)
+    qmax: 2114.3
+    qmin: 1952.4
+    value:
+      background_std: 0.6227807300000003
+      counts_background: 0.5955559093625553
+      counts_total: 10.995924200000006
+      distribution: general_gamma_counting_process
+      scale_factor: 0.10870827760983351
+  - name: R_13(pp->mumu)
+    qmax: 2289.7
+    qmin: 2114.3
+    value:
+      background_std: 0.4413414799999991
+      counts_background: 0.29515276868574336
+      counts_total: 5.00012779999999
+      distribution: general_gamma_counting_process
+      scale_factor: 0.167487590606583
+  - name: R_13(pp->mumu)
+    qmax: 2479.7
+    qmin: 2289.7
+    value:
+      background_std: 0.27607000000000004
+      counts_background: 0.20015551084469524
+      counts_total: 5.00137
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2674513195145638
+  - name: R_13(pp->mumu)
+    qmax: 2685.4
+    qmin: 2479.7
+    value:
+      background_std: 0.25381323000000033
+      counts_background: 0.47702046834357753
+      counts_total: 3.9998365000000056
+      distribution: general_gamma_counting_process
+      scale_factor: 0.4389009214653366
+  - name: R_13(pp->mumu)
+    qmax: 2908.1
+    qmin: 2685.4
+    value:
+      background_std: 0.11024318099999991
+      counts_background: 0.03297435038722071
+      counts_total: 1.9993783299999985
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7131174862648247
+  - name: R_13(pp->mumu)
+    qmax: 3149.4
+    qmin: 2908.1
+    value:
+      background_std: 0.06986841500000006
+      counts_background: 0.04458324569433998
+      counts_total: 1.0002126300000007
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2314791787980226
+  - name: R_13(pp->mumu)
+    qmax: 3410.7
+    qmin: 3149.4
+    value:
+      background_std: 0.05643296099999994
+      counts_background: 0.07514250176724041
+      counts_total: 1.0001518799999989
+      distribution: general_gamma_counting_process
+      scale_factor: 2.168009269460113
+  - name: R_13(pp->mumu)
+    qmax: 3693.6
+    qmin: 3410.7
+    value:
+      background_std: 0.03388293300000001
+      counts_background: 0.01668698212327797
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.926834312717107
+  - name: R_13(pp->mumu)
+    qmax: 4000.0
+    qmin: 3693.6
+    value:
+      background_std: 0.016785204800000005
+      counts_background: 0.004858630873580564
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 7.4457838699106365
+  - name: R_13(pp->mumu)
+    qmax: 4500.0
+    qmin: 4000.0
+    value:
+      background_std: 0.0198925
+      counts_background: 0.024312284528648097
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 11.631275580400724
+  - name: R_13(pp->mumu)
+    qmax: 5200.0
+    qmin: 4500.0
+    value:
+      counts_background: 0.006999999999999912
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 42.34938830898644
+
+CMS pp->munu 2022:
+  experiment: CMS
+  inspire: CMS:2022yjm
+  values:
+  - mTmax: 218.28571428571428
+    mTmin: 120.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 764326.3
+      counts_background: 735456.4777480316
+      counts_total: 8082423.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.381100504452376e-07
+  - mTmax: 316.57142857142856
+    mTmin: 218.28571428571428
+    name: R_13(pp->munu)
+    value:
+      background_std: 28257.3
+      counts_background: 60370.10313703723
+      counts_total: 293361.0
+      distribution: general_gamma_counting_process
+      scale_factor: 4.5080589494231244e-06
+  - mTmax: 414.8571428571429
+    mTmin: 316.57142857142856
+    name: R_13(pp->munu)
+    value:
+      background_std: 5851.09
+      counts_background: 11483.256415576703
+      counts_total: 59924.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1202901353921295e-05
+  - mTmax: 513.1428571428571
+    mTmin: 414.8571428571429
+    name: R_13(pp->munu)
+    value:
+      background_std: 1859.65
+      counts_background: 2834.0427140980073
+      counts_total: 18841.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.457148220281266e-05
+  - mTmax: 611.4285714285714
+    mTmin: 513.1428571428571
+    name: R_13(pp->munu)
+    value:
+      background_std: 747.879
+      counts_background: 895.805088818062
+      counts_total: 7267.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0001616463699144605
+  - mTmax: 709.7142857142858
+    mTmin: 611.4285714285714
+    name: R_13(pp->munu)
+    value:
+      background_std: 353.206
+      counts_background: 361.61575189695833
+      counts_total: 3255.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0003514780917579742
+  - mTmax: 808.0
+    mTmin: 709.7142857142858
+    name: R_13(pp->munu)
+    value:
+      background_std: 179.091
+      counts_background: 149.32036560618837
+      counts_total: 1611.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0006984493205069298
+  - mTmax: 906.2857142857143
+    mTmin: 808.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 97.7124
+      counts_background: 57.76185137943858
+      counts_total: 876.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0012935598118303038
+  - mTmax: 1004.5714285714287
+    mTmin: 906.2857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 62.5286
+      counts_background: 37.55312637975146
+      counts_total: 467.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0022871572872031763
+  - mTmax: 1102.857142857143
+    mTmin: 1004.5714285714287
+    name: R_13(pp->munu)
+    value:
+      background_std: 35.7788
+      counts_background: 17.25852637339621
+      counts_total: 282.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.0038788180897831002
+  - mTmax: 1201.142857142857
+    mTmin: 1102.857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 25.9187
+      counts_background: 15.164570356372504
+      counts_total: 178.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.006217144659820986
+  - mTmax: 1299.4285714285716
+    mTmin: 1201.142857142857
+    name: R_13(pp->munu)
+    value:
+      background_std: 14.5396
+      counts_background: 6.057353550907621
+      counts_total: 115.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01004697764321072
+  - mTmax: 1397.7142857142858
+    mTmin: 1299.4285714285716
+    name: R_13(pp->munu)
+    value:
+      background_std: 9.55914
+      counts_background: 2.7593736736576306
+      counts_total: 71.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.01541561367084377
+  - mTmax: 1496.0
+    mTmin: 1397.7142857142858
+    name: R_13(pp->munu)
+    value:
+      background_std: 6.64664
+      counts_background: 1.9520955749150137
+      counts_total: 40.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.023220193353268782
+  - mTmax: 1594.2857142857144
+    mTmin: 1496.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 5.7114
+      counts_background: 2.9067998806677164
+      counts_total: 41.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.03441546460678311
+  - mTmax: 1692.5714285714287
+    mTmin: 1594.2857142857144
+    name: R_13(pp->munu)
+    value:
+      background_std: 3.2872
+      counts_background: 0.7204998962755044
+      counts_total: 33.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.050429467699783175
+  - mTmax: 1790.857142857143
+    mTmin: 1692.5714285714287
+    name: R_13(pp->munu)
+    value:
+      background_std: 2.429
+      counts_background: 0.6367605053114246
+      counts_total: 10.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.07345482522107218
+  - mTmax: 1889.1428571428573
+    mTmin: 1790.857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.96496
+      counts_background: 1.1195918643365383
+      counts_total: 16.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.10214590783781516
+  - mTmax: 1987.4285714285716
+    mTmin: 1889.1428571428573
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.53658
+      counts_background: 0.3011358874083727
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.14426901221246954
+  - mTmax: 2085.714285714286
+    mTmin: 1987.4285714285716
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.06203
+      counts_background: 0.5289724930974729
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.20042802700410473
+  - mTmax: 2184.0
+    mTmin: 2085.714285714286
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.789811
+      counts_background: 0.25307606773948504
+      counts_total: 5.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2759213739465906
+  - mTmax: 2282.285714285714
+    mTmin: 2184.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 1.64016
+      counts_background: 0.07017318305228824
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.2486947919892465
+  - mTmax: 2380.571428571429
+    mTmin: 2282.285714285714
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.532257
+      counts_background: 0.18578587621395445
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.5215022051516215
+  - mTmax: 2478.857142857143
+    mTmin: 2380.571428571429
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.401721
+      counts_background: 0.014027089270265821
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.7015769816918597
+  - mTmax: 2577.1428571428573
+    mTmin: 2478.857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.353156
+      counts_background: 0.0572407434906522
+      counts_total: 3.0
+      distribution: general_gamma_counting_process
+      scale_factor: 0.9426817545512813
+  - mTmax: 2675.4285714285716
+    mTmin: 2577.1428571428573
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.273798
+      counts_background: 0.009280203355479627
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.2728362695780504
+  - mTmax: 2773.714285714286
+    mTmin: 2675.4285714285716
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.408859
+      counts_background: 0.3260113188814421
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 1.7081370916365182
+  - mTmax: 2872.0
+    mTmin: 2773.714285714286
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.178459
+      counts_background: 0.0050630557964758596
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.1573914897452897
+  - mTmax: 2970.2857142857147
+    mTmin: 2872.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.154555
+      counts_background: 0.02354030895411082
+      counts_total: 2.0
+      distribution: general_gamma_counting_process
+      scale_factor: 2.923616167189418
+  - mTmax: 3068.571428571429
+    mTmin: 2970.2857142857147
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.11898
+      counts_background: 0.002754887756233705
+      counts_total: 1.0
+      distribution: general_gamma_counting_process
+      scale_factor: 3.891484286778623
+  - mTmax: 3166.857142857143
+    mTmin: 3068.571428571429
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.0983986
+      counts_background: 0.002418966840862466
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 5.025321423756287
+  - mTmax: 3265.1428571428573
+    mTmin: 3166.857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.07899
+      counts_background: 0.0016655879745978085
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 6.630667669687228
+  - mTmax: 3363.4285714285716
+    mTmin: 3265.1428571428573
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.061663
+      counts_background: 0.0010220913348152952
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 8.580794897857855
+  - mTmax: 3461.714285714286
+    mTmin: 3363.4285714285716
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.05249
+      counts_background: 0.0012019722815964323
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 11.18786713539267
+  - mTmax: 3560.0
+    mTmin: 3461.714285714286
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.043518
+      counts_background: 0.0005595119230388659
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 14.229179567277571
+  - mTmax: 3658.2857142857147
+    mTmin: 3560.0
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.035888
+      counts_background: 0.0025767861577569613
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 18.633054553135672
+  - mTmax: 3756.571428571429
+    mTmin: 3658.2857142857147
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.02898
+      counts_background: 0.00032981552772133523
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 24.00049431696484
+  - mTmax: 3854.857142857143
+    mTmin: 3756.571428571429
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.02309
+      counts_background: 0.0002507929010435966
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 30.465794327480626
+  - mTmax: 3953.1428571428573
+    mTmin: 3854.857142857143
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.019
+      counts_background: 0.0002074231380965868
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 39.48173087374054
+  - mTmax: 4051.4285714285716
+    mTmin: 3953.1428571428573
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.01527
+      counts_background: 0.00010254307466266231
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 49.38721600969236
+  - mTmax: 4149.714285714286
+    mTmin: 4051.4285714285716
+    name: R_13(pp->munu)
+    value:
+      background_std: 0.0123
+      counts_background: 0.0001256563671538112
+      counts_total: 0.0
+      distribution: general_gamma_counting_process
+      scale_factor: 63.077501791994194
+  - mTmax: 4248.0
+    mTmin: 4149.714285714286
+    name: R_13(pp->munu)
+    value:
+      counts_background: 7.422452605320821e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 79.73851133087038
+  - mTmax: 4346.285714285715
+    mTmin: 4248.0
+    name: R_13(pp->munu)
+    value:
+      counts_background: 4.5836416220864686e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 100.94154898576248
+  - mTmax: 4444.571428571428
+    mTmin: 4346.285714285715
+    name: R_13(pp->munu)
+    value:
+      counts_background: 3.761930232618374e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 126.46773127308612
+  - mTmax: 4542.857142857143
+    mTmin: 4444.571428571428
+    name: R_13(pp->munu)
+    value:
+      counts_background: 2.3201214556545247e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 161.447630038755
+  - mTmax: 4641.142857142858
+    mTmin: 4542.857142857143
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.816860522123703e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 198.5475565878203
+  - mTmax: 4739.428571428572
+    mTmin: 4641.142857142858
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.29962616478234e-05
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 243.78335597070824
+  - mTmax: 4837.714285714286
+    mTmin: 4739.428571428572
+    name: R_13(pp->munu)
+    value:
+      counts_background: 8.171314021369165e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 313.00928079960136
+  - mTmax: 4936.0
+    mTmin: 4837.714285714286
+    name: R_13(pp->munu)
+    value:
+      counts_background: 5.702788130690082e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 384.08487575039294
+  - mTmax: 5034.285714285715
+    mTmin: 4936.0
+    name: R_13(pp->munu)
+    value:
+      counts_background: 2.655536816362048e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 465.19519783338
+  - mTmax: 5132.571428571428
+    mTmin: 5034.285714285715
+    name: R_13(pp->munu)
+    value:
+      counts_background: 2.1545588755475023e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 585.2980095021534
+  - mTmax: 5230.857142857143
+    mTmin: 5132.571428571428
+    name: R_13(pp->munu)
+    value:
+      counts_background: 6.715722933529167e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 712.0715988138246
+  - mTmax: 5329.142857142858
+    mTmin: 5230.857142857143
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.9201839461521176e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 869.0425101085982
+  - mTmax: 5427.428571428572
+    mTmin: 5329.142857142858
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.3061289602974232e-06
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 605.1382199610066
+  - mTmax: 5525.714285714286
+    mTmin: 5427.428571428572
+    name: R_13(pp->munu)
+    value:
+      counts_background: 9.336466069482163e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1283.8728175198783
+  - mTmax: 5624.0
+    mTmin: 5525.714285714286
+    name: R_13(pp->munu)
+    value:
+      counts_background: 7.598061149352847e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1574.479741425196
+  - mTmax: 5722.285714285715
+    mTmin: 5624.0
+    name: R_13(pp->munu)
+    value:
+      counts_background: 9.628309402163802e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 1915.653134844684
+  - mTmax: 5820.571428571429
+    mTmin: 5722.285714285715
+    name: R_13(pp->munu)
+    value:
+      counts_background: 6.803814408712961e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2144.379517263722
+  - mTmax: 5918.857142857143
+    mTmin: 5820.571428571429
+    name: R_13(pp->munu)
+    value:
+      counts_background: 4.2377277319657177e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 2577.715998415671
+  - mTmax: 6017.142857142858
+    mTmin: 5918.857142857143
+    name: R_13(pp->munu)
+    value:
+      counts_background: 6.177460889176766e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 3192.8273162849705
+  - mTmax: 6115.428571428572
+    mTmin: 6017.142857142858
+    name: R_13(pp->munu)
+    value:
+      counts_background: 3.619143173349792e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 3744.6517259682723
+  - mTmax: 6213.714285714286
+    mTmin: 6115.428571428572
+    name: R_13(pp->munu)
+    value:
+      counts_background: 3.155387757124606e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 4574.050044622984
+  - mTmax: 6312.0
+    mTmin: 6213.714285714286
+    name: R_13(pp->munu)
+    value:
+      counts_background: 3.897156780874507e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 5338.906940974334
+  - mTmax: 6410.285714285715
+    mTmin: 6312.0
+    name: R_13(pp->munu)
+    value:
+      counts_background: 2.4091380627527464e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 6319.666512062608
+  - mTmax: 6508.571428571429
+    mTmin: 6410.285714285715
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.9913188557108668e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 7059.013681710888
+  - mTmax: 6606.857142857143
+    mTmin: 6508.571428571429
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.4249113987876678e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 8550.36091241205
+  - mTmax: 6705.142857142858
+    mTmin: 6606.857142857143
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.194606974578001e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 9635.756419654661
+  - mTmax: 6803.428571428572
+    mTmin: 6705.142857142858
+    name: R_13(pp->munu)
+    value:
+      counts_background: 1.3050822275305631e-07
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 10579.458557629101
+  - mTmax: 6901.714285714286
+    mTmin: 6803.428571428572
+    name: R_13(pp->munu)
+    value:
+      counts_background: 9.860600769233048e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 12759.008661759273
+  - mTmax: 7000.0
+    mTmin: 6901.714285714286
+    name: R_13(pp->munu)
+    value:
+      counts_background: 5.7520370590772414e-08
+      counts_total: 0.0
+      distribution: gamma_counting_process
+      scale_factor: 15181.392014563447
+
+Belle B+->pi+ee 2008:
+  experiment: Belle
+  inspire: Belle:2008tjs
+  values:
+    BR_Belle(B+->piee): 1.5 +3.5-2.5 ± 0.1 ± 0.8 1e-8
+
+LHCb B->pimumu 2015:
+  experiment: LHCb
+  inspire: LHCb:2015hsa
+  values:
+    - name: <dBR/dq2>(B+->pimumu)
+      q2min: 2
+      q2max: 4
+      value: 0.62 +0.39-0.33 ± 0.02 1e-9
+    - name: <dBR/dq2>(B+->pimumu)
+      q2min: 4
+      q2max: 6
+      value: 0.85 +0.32-0.27 ± 0.02 1e-9
+    - name: <dBR/dq2>(B+->pimumu)
+      q2min: 15
+      q2max: 22
+      value: 0.47 +0.12-0.10 ± 0.01 1e-9
+
+LHCb Bs->K*mumu 2018:
+   experiment: LHCb
+   inspire: LHCb:2018rym
+   values:
+     BR_LHCb(Bs->K*0mumu): 2.9 ± 1.0 ± 0.2 ± 0.3 1e-8
```

### Comparing `flavio-2.4.0/flavio/data/parameters_correlated.yml` & `flavio-2.5.0/flavio/data/parameters_correlated.yml`

 * *Files 8% similar despite different names*

```diff
@@ -326,46 +326,40 @@
     [0.000, 0.000, 0.000, 0.000, 1.000, 0.973, 0.324, 0.372, 0.272],
     [0.000, 0.000, 0.000, 0.000, 0.000, 1.000, 0.268, 0.332, 0.269],
     [0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 1.000, 0.590, 0.515],
     [0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 1.000, 0.897],
     [0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 0.000, 1.000]]
 
 
-# B_q SM bag parameters,
-# for the bag parameters of the SM operator OVLL,
-# the "hatted" ones need to be divided by 1.517
-# (for B_q) and 1.369 (for K) to obtain the MSbar ones
-# (see also flavio.physics.mesonmixing.common.bag_msbar2rgi())
--
-  values:
-    - bag_B0_1: 0.857(66)  # =1.30(10) for Bhat. FLAG 2018 Nf=2+1
-    - bag_Bs_1: 0.890(40)  # =1.35(6) for Bhat. FLAG 2018 Nf=2+1
-  correlation: [[1, 0.94], [0.94, 1]]  # to obtain 0.038 error on BBs/BBd (FLAG)
-
-
-# B_q BSM bag parameters, FNAL/MILC 2015, arXiv:1602.03560v2
--
-  values:
-    - bag_B0_2: 0.761(68)(33)
-    - bag_B0_3: 1.07(21)(5)
-    - bag_B0_4: 1.148(83)(50)  # was 1.040(75)(45); multiplied by 1.104 due to differing definition
-    - bag_B0_5: 1.870(180)(81)  # was 0.964(93)(42); multiplied by 1.940 due to differing definition
-    - bag_Bs_2: 0.806(52)(27)
-    - bag_Bs_3: 1.10(15)(4)
-    - bag_Bs_4: 1.129(63)(38)  # was 1.022(57)(34); multiplied by 1.105 due to differing definition
-    - bag_Bs_5: 1.834(132)(60)  # was 0.943(68)(31); multiplied by 1.944 due to differing definition
-  correlation:
-    [[1,    0.282, 0.494, 0.389, 0.766, 0.201, 0.283, 0.226],
-    [0.282, 1,     0.225, 0.148, 0.179, 0.929, 0.115, 0.063],
-    [0.494, 0.225, 1,     0.528, 0.297, 0.134, 0.705, 0.332],
-    [0.389, 0.148, 0.528, 1,     0.228, 0.074, 0.318, 0.797],
-    [0.766, 0.179, 0.297, 0.228, 1,     0.329, 0.581, 0.466],
-    [0.201, 0.929, 0.134, 0.074, 0.329, 1,     0.278, 0.195],
-    [0.283, 0.115, 0.705, 0.318, 0.581, 0.278, 1,     0.581],
-    [0.226, 0.063, 0.332, 0.797, 0.466, 0.195, 0.581, 1    ]]
+# B_q SM and BSM  bag parameters, 2023 GSSS (arXiv:2212.10497) combination of
+# - KLR 2019, arXiv:1904.00940v2
+# - HPQCD 2019, arXiv:1907.01025v2
+-
+  values:
+    - bag_B0_1: 0.837 +- 0.03
+    - bag_B0_2: 0.808 +- 0.037
+    - bag_B0_3: 0.761 +- 0.053
+    - bag_B0_4: 1.163 +- 0.047  # was 1.054 +- 0.042; multiplied by 1.104 due to differing definition
+    - bag_B0_5: 1.914 +- 0.071  # was 0.986 +- 0.037; multiplied by 1.940 due to differing definition
+    - bag_Bs_1: 0.826 +- 0.029
+    - bag_Bs_2: 0.824 +- 0.037
+    - bag_Bs_3: 0.83 +- 0.053
+    - bag_Bs_4: 1.149 +- 0.045  # was 1.04 +- 0.041; multiplied by 1.105 due to differing definition
+    - bag_Bs_5: 1.873 +- 0.066  # was 0.964 +- 0.034; multiplied by 1.944 due to differing definition
+  correlation:
+    [[1.0, 0.046, 0.003, 0.022, 0.024, 0.976, 0.044, 0.006, 0.022, 0.025],
+     [0.046, 1.0, 0.132, 0.168, 0.099, 0.043, 0.983, 0.134, 0.17, 0.104],
+     [0.003, 0.132, 1.0, 0.119, 0.069, 0.005, 0.13, 0.921, 0.121, 0.073],
+     [0.022, 0.168, 0.119, 1.0, 0.186, 0.023, 0.17, 0.129, 0.984, 0.196],
+     [0.024, 0.099, 0.069, 0.186, 1.0, 0.024, 0.101, 0.075, 0.186, 0.951],
+     [0.976, 0.043, 0.005, 0.023, 0.024, 1.0, 0.044, 0.006, 0.023, 0.025],
+     [0.044, 0.983, 0.13, 0.17, 0.101, 0.044, 1.0, 0.137, 0.173, 0.106],
+     [0.006, 0.134, 0.921, 0.129, 0.075, 0.006, 0.137, 1.0, 0.131, 0.079],
+     [0.022, 0.17, 0.121, 0.984, 0.186, 0.023, 0.173, 0.131, 1.0, 0.199],
+     [0.025, 0.104, 0.073, 0.196, 0.951, 0.025, 0.106, 0.079, 0.199, 1.0]]
 
 
 # Experimental data needed for the normalization of BR(B->Xsgamma)
 -
   values:
     - C_BXlnu: 0.567(7)
     - BR(B->Xcenu)_exp: 0.1067(16)
@@ -406,61 +400,39 @@
     - K+mu3 delta_EM: 0.008(125)1e-2
   correlation:
     [[1, 0.081, 0.685, -0.147], [1, -0.147, 0.764], [1, 0.081], [1]]
 
 
 # Parameters for HQET form factors
 - values:
-    - CLN rho2_xi: 1.073 ± 0.204
-    - CLN c_xi: 0.951 ± 0.246
-    - CLN xi3: -3.769 ± 1.084
+    - CLN rho2_xi: 1.068 ± 0.206
+    - CLN c_xi: 0.946 ± 0.247
+    - CLN xi3: -3.746 ± 1.087
     - chi_2(1): -0.060 ± 0.020
     - chi_2p(1): -0.000 ± 0.020
-    - chi_2pp(1): -0.095 ± 0.219
+    - chi_2pp(1): -0.097 ± 0.218
     - chi_3p(1): 0.040 ± 0.020
-    - chi_3pp(1): -0.098 ± 0.061
-    - eta(1): 0.612 ± 0.175
-    - etap(1): -0.005 ± 0.185
-    - etapp(1): -0.298 ± 0.561
-    - CLN l_1(1): 0.125 ± 0.230
-    - CLN lp_1(1): -8.042 ± 6.574
-    - CLN l_2(1): -1.913 ± 0.362
-    - CLN lp_2(1): -3.641 ± 5.469
-    - CLN l_3(1): -3.357 ± 6.950
-    - CLN lp_3(1): 4.911 ± 6.901
-    - CLN l_4(1): -2.076 ± 1.403
-    - CLN lp_4(1): 0.164 ± 1.817
-    - CLN l_5(1): 3.393 ± 2.667
-    - CLN lp_5(1): 0.048 ± 3.014
-    - CLN l_6(1): 2.157 ± 3.758
-    - CLN lp_6(1): 0.651 ± 4.247
-  correlation:
-    [[1.000, 0.951, -0.864, -0.014, 0.000, 0.582, 0.029, 0.014, 0.028, 0.021, -0.115, -0.008, 0.957, 0.026, 0.768, 0.036, -0.288, -0.025, -0.258, -0.209, 0.047, -0.081, -0.139],
-    [0.951, 1.000, -0.961, -0.013, 0.005, 0.567, 0.031, -0.144, 0.010, -0.005, -0.014, -0.012, 0.909, 0.034, 0.645, 0.108, -0.354, -0.010, -0.228, -0.311, 0.198, -0.082, -0.075],
-    [-0.864, -0.961, 1.000, 0.012, -0.008, -0.406, -0.026, 0.194, -0.002, 0.016, -0.036, 0.007, -0.829, -0.022, -0.627, -0.147, 0.332, 0.005, 0.201, 0.329, -0.201, 0.065, 0.065],
-    [-0.014, -0.013, 0.012, 1.000, 0.021, -0.017, -0.004, 0.052, 0.013, -0.007, -0.001, -0.005, 0.076, 0.008, 0.014, -0.050, -0.008, -0.018, 0.006, 0.006, -0.010, 0.022, -0.017],
-    [0.000, 0.005, -0.008, 0.021, 1.000, -0.097, 0.000, 0.180, -0.010, -0.010, 0.011, 0.011, 0.002, 0.006, 0.013, 0.008, -0.050, 0.012, 0.003, 0.012, -0.028, 0.009, -0.005],
-    [0.582, 0.567, -0.406, -0.017, -0.097, 1.000, 0.022, 0.174, 0.056, 0.053, -0.252, -0.002, 0.556, 0.048, 0.230, -0.139, -0.221, -0.051, -0.160, -0.054, 0.130, -0.144, 0.004],
-    [0.029, 0.031, -0.026, -0.004, 0.000, 0.022, 1.000, -0.180, 0.005, -0.010, 0.001, -0.004, -0.232, 0.005, 0.030, -0.002, -0.006, -0.006, 0.002, -0.016, 0.034, -0.012, 0.015],
-    [0.014, -0.144, 0.194, 0.052, 0.180, 0.174, -0.180, 1.000, -0.010, 0.028, -0.110, -0.031, 0.061, -0.020, 0.266, -0.264, 0.182, 0.027, 0.095, 0.393, -0.530, 0.009, -0.185],
-    [0.028, 0.010, -0.002, 0.013, -0.010, 0.056, 0.005, -0.010, 1.000, -0.218, -0.224, 0.010, 0.028, 0.009, -0.000, 0.101, 0.005, -0.973, 0.182, -0.061, -0.051, 0.376, -0.168],
-    [0.021, -0.005, 0.016, -0.007, -0.010, 0.053, -0.010, 0.028, -0.218, 1.000, -0.396, 0.004, 0.022, 0.009, 0.032, -0.050, 0.143, 0.212, -0.800, 0.002, -0.078, -0.075, 0.245],
-    [-0.115, -0.014, -0.036, -0.001, 0.011, -0.252, 0.001, -0.110, -0.224, -0.396, 1.000, -0.042, -0.115, -0.000, -0.185, 0.328, -0.306, 0.210, 0.294, -0.151, 0.233, 0.143, 0.007],
-    [-0.008, -0.012, 0.007, -0.005, 0.011, -0.002, -0.004, -0.031, 0.010, 0.004, -0.042, 1.000, -0.004, -0.001, 0.022, -0.004, -0.000, 0.064, -0.105, -0.027, -0.013, -0.012, -0.011],
-    [0.957, 0.909, -0.829, 0.076, 0.002, 0.556, -0.232, 0.061, 0.028, 0.022, -0.115, -0.004, 1.000, 0.024, 0.740, 0.031, -0.277, -0.031, -0.250, -0.205, 0.036, -0.077, -0.139],
-    [0.026, 0.034, -0.022, 0.008, 0.006, 0.048, 0.005, -0.020, 0.009, 0.009, -0.000, -0.001, 0.024, 1.000, -0.048, -0.000, -0.011, -0.007, -0.015, -0.027, 0.018, -0.023, 0.026],
-    [0.768, 0.645, -0.627, 0.014, 0.013, 0.230, 0.030, 0.266, -0.000, 0.032, -0.185, 0.022, 0.740, -0.048, 1.000, -0.127, -0.092, -0.004, -0.214, 0.053, -0.171, -0.081, -0.257],
-    [0.036, 0.108, -0.147, -0.050, 0.008, -0.139, -0.002, -0.264, 0.101, -0.050, 0.328, -0.004, 0.031, -0.000, -0.127, 1.000, -0.796, -0.101, 0.001, -0.419, 0.091, 0.756, -0.448],
-    [-0.288, -0.354, 0.332, -0.008, -0.050, -0.221, -0.006, 0.182, 0.005, 0.143, -0.306, -0.000, -0.277, -0.011, -0.092, -0.796, 1.000, -0.004, -0.024, 0.268, -0.193, -0.617, 0.630],
-    [-0.025, -0.010, 0.005, -0.018, 0.012, -0.051, -0.006, 0.027, -0.973, 0.212, 0.210, 0.064, -0.031, -0.007, -0.004, -0.101, -0.004, 1.000, -0.141, 0.071, 0.045, -0.363, 0.158],
-    [-0.258, -0.228, 0.201, 0.006, 0.003, -0.160, 0.002, 0.095, 0.182, -0.800, 0.294, -0.105, -0.250, -0.015, -0.214, 0.001, -0.024, -0.141, 1.000, 0.087, 0.040, 0.078, -0.173],
-    [-0.209, -0.311, 0.329, 0.006, 0.012, -0.054, -0.016, 0.393, -0.061, 0.002, -0.151, -0.027, -0.205, -0.027, 0.053, -0.419, 0.268, 0.071, 0.087, 1.000, -0.597, 0.101, -0.271],
-    [0.047, 0.198, -0.201, -0.010, -0.028, 0.130, 0.034, -0.530, -0.051, -0.078, 0.233, -0.013, 0.036, 0.018, -0.171, 0.091, -0.193, 0.045, 0.040, -0.597, 1.000, -0.256, 0.417],
-    [-0.081, -0.082, 0.065, 0.022, 0.009, -0.144, -0.012, 0.009, 0.376, -0.075, 0.143, -0.012, -0.077, -0.023, -0.081, 0.756, -0.617, -0.363, 0.078, 0.101, -0.256, 1.000, -0.740],
-    [-0.139, -0.075, 0.065, -0.017, -0.005, 0.004, 0.015, -0.185, -0.168, 0.245, 0.007, -0.011, -0.139, 0.026, -0.257, -0.448, 0.630, 0.158, -0.173, -0.271, 0.417, -0.740, 1.000]]
+    - chi_3pp(1): -0.098 ± 0.062
+    - eta(1): 0.611 ± 0.174
+    - etap(1): -0.003 ± 0.184
+    - etapp(1): -0.309 ± 0.568
+    - CLN l_1(1): 0.124 ± 0.231
+    - CLN lp_1(1): -8.205 ± 6.609
+    - CLN l_2(1): -1.918 ± 0.363
+    - CLN lp_2(1): -3.715 ± 5.547
+    - CLN l_3(1): -3.527 ± 7.279
+    - CLN lp_3(1): 5.100 ± 7.079
+    - CLN l_4(1): -2.067 ± 1.398
+    - CLN lp_4(1): 0.147 ± 1.793
+    - CLN l_5(1): 3.410 ± 2.696
+    - CLN lp_5(1): 0.084 ± 3.023
+    - CLN l_6(1): 2.091 ± 3.836
+    - CLN lp_6(1): 0.731 ± 4.204
+  correlation:
+    [[1.0, 0.949, -0.863, -0.029, 0.003, 0.569, 0.045, 0.016, 0.006, 0.014, -0.1, -0.004, 0.958, 0.037, 0.775, 0.032, -0.283, -0.008, -0.25, -0.188, 0.025, -0.084, -0.151], [0.949, 1.0, -0.961, -0.023, 0.011, 0.551, 0.041, -0.141, -0.013, -0.002, -0.006, -0.013, 0.91, 0.039, 0.65, 0.111, -0.355, 0.01, -0.231, -0.296, 0.179, -0.075, -0.093], [-0.863, -0.961, 1.0, 0.018, -0.014, -0.389, -0.038, 0.189, 0.025, 0.01, -0.044, 0.008, -0.829, -0.026, -0.632, -0.146, 0.332, -0.02, 0.207, 0.311, -0.183, 0.059, 0.08], [-0.029, -0.023, 0.018, 1.0, -0.002, -0.028, -0.002, 0.031, -0.005, -0.002, 0.008, 0.001, 0.058, 0.002, -0.004, -0.05, 0.001, 0.005, 0.009, 0.004, -0.0, 0.01, -0.0], [0.003, 0.011, -0.014, -0.002, 1.0, -0.082, -0.001, 0.19, -0.01, -0.0, 0.017, -0.005, 0.003, 0.003, 0.011, 0.0, -0.05, 0.01, -0.004, 0.024, -0.027, 0.008, -0.003], [0.569, 0.551, -0.389, -0.028, -0.082, 1.0, 0.02, 0.195, 0.047, 0.052, -0.268, 0.001, 0.548, 0.053, 0.242, -0.165, -0.194, -0.045, -0.156, -0.031, 0.097, -0.163, -0.005], [0.045, 0.041, -0.038, -0.002, -0.001, 0.02, 1.0, -0.151, 0.005, -0.004, 0.005, 0.007, -0.213, 0.003, 0.051, 0.001, -0.009, -0.007, -0.008, -0.019, 0.007, -0.009, 0.002], [0.016, -0.141, 0.189, 0.031, 0.19, 0.195, -0.151, 1.0, 0.006, 0.009, -0.124, -0.029, 0.054, -0.021, 0.269, -0.279, 0.2, 0.009, 0.108, 0.41, -0.541, -0.007, -0.175], [0.006, -0.013, 0.025, -0.005, -0.01, 0.047, 0.005, 0.006, 1.0, -0.209, -0.225, 0.002, 0.002, -0.0, -0.015, 0.102, 0.017, -0.972, 0.179, -0.067, -0.051, 0.37, -0.156], [0.014, -0.002, 0.01, -0.002, -0.0, 0.052, -0.004, 0.009, -0.209, 1.0, -0.397, 0.0, 0.015, -0.004, 0.019, -0.042, 0.13, 0.206, -0.798, -0.006, -0.062, -0.064, 0.241], [-0.1, -0.006, -0.044, 0.008, 0.017, -0.268, 0.005, -0.124, -0.225, -0.397, 1.0, -0.025, -0.101, -0.003, -0.173, 0.35, -0.329, 0.21, 0.287, -0.166, 0.229, 0.166, -0.014], [-0.004, -0.013, 0.008, 0.001, -0.005, 0.001, 0.007, -0.029, 0.002, 0.0, -0.025, 1.0, -0.003, 0.004, 0.022, -0.014, 0.014, 0.071, -0.1, -0.015, -0.015, -0.021, 0.006], [0.958, 0.91, -0.829, 0.058, 0.003, 0.548, -0.213, 0.054, 0.002, 0.015, -0.101, -0.003, 1.0, 0.036, 0.746, 0.026, -0.272, -0.01, -0.242, -0.184, 0.021, -0.082, -0.147], [0.037, 0.039, -0.026, 0.002, 0.003, 0.053, 0.003, -0.021, -0.0, -0.004, -0.003, 0.004, 0.036, 1.0, -0.029, -0.017, -0.005, -0.001, -0.008, -0.025, 0.02, -0.045, 0.03], [0.775, 0.65, -0.632, -0.004, 0.011, 0.242, 0.051, 0.269, -0.015, 0.019, -0.173, 0.022, 0.746, -0.029, 1.0, -0.141, -0.078, 0.008, -0.204, 0.081, -0.184, -0.096, -0.25], [0.032, 0.111, -0.146, -0.05, 0.0, -0.165, 0.001, -0.279, 0.102, -0.042, 0.35, -0.014, 0.026, -0.017, -0.141, 1.0, -0.804, -0.104, -0.004, -0.443, 0.108, 0.771, -0.459], [-0.283, -0.355, 0.332, 0.001, -0.05, -0.194, -0.009, 0.2, 0.017, 0.13, -0.329, 0.014, -0.272, -0.005, -0.078, -0.804, 1.0, -0.013, -0.017, 0.292, -0.203, -0.627, 0.638], [-0.008, 0.01, -0.02, 0.005, 0.01, -0.045, -0.007, 0.009, -0.972, 0.206, 0.21, 0.071, -0.01, -0.001, 0.008, -0.104, -0.013, 1.0, -0.138, 0.078, 0.048, -0.359, 0.15], [-0.25, -0.231, 0.207, 0.009, -0.004, -0.156, -0.008, 0.108, 0.179, -0.798, 0.287, -0.1, -0.242, -0.008, -0.204, -0.004, -0.017, -0.138, 1.0, 0.094, 0.021, 0.073, -0.174], [-0.188, -0.296, 0.311, 0.004, 0.024, -0.031, -0.019, 0.41, -0.067, -0.006, -0.166, -0.015, -0.184, -0.025, 0.081, -0.443, 0.292, 0.078, 0.094, 1.0, -0.602, 0.058, -0.251], [0.025, 0.179, -0.183, -0.0, -0.027, 0.097, 0.007, -0.541, -0.051, -0.062, 0.229, -0.015, 0.021, 0.02, -0.184, 0.108, -0.203, 0.048, 0.021, -0.602, 1.0, -0.229, 0.399], [-0.084, -0.075, 0.059, 0.01, 0.008, -0.163, -0.009, -0.007, 0.37, -0.064, 0.166, -0.021, -0.082, -0.045, -0.096, 0.771, -0.627, -0.359, 0.073, 0.058, -0.229, 1.0, -0.736], [-0.151, -0.093, 0.08, -0.0, -0.003, -0.005, 0.002, -0.175, -0.156, 0.241, -0.014, 0.006, -0.147, 0.03, -0.25, -0.459, 0.638, 0.15, -0.174, -0.251, 0.399, -0.736, 1.0]]
 
 
 
 # Parameters for D->pi form factors
 # arXiv:1706.03017
 - values:
     - D->pi BSZ a0_f+: 0.612 ± 0.0355
@@ -553,8 +525,7 @@
     [0.013, 0.11, 0.187, -0.643, -0.03, 0.303, -0.057, -0.739, 0.179, -0.639, -0.066, 0.15, 0.2, -0.635, 0.007, -0.122, -0.033, 0.35, 0.011, 0.137, -0.022, 1.0, 0.19, -0.644, 0.192, -0.643, 0.139, -0.521],
     [0.446, 0.707, 0.988, -0.604, -0.013, 0.591, 0.331, -0.064, 0.994, -0.606, 0.138, 0.743, 0.994, -0.611, -0.047, -0.117, -0.02, 0.567, 0.373, 0.73, -0.252, 0.19, 1.0, -0.606, 0.992, -0.607, 0.289, -0.25],
     [-0.176, -0.33, -0.589, 0.989, 0.039, -0.501, -0.015, 0.599, -0.597, 0.993, -0.073, -0.404, -0.608, 0.994, -0.097, 0.206, 0.033, -0.509, -0.191, -0.358, 0.065, -0.644, -0.606, 1.0, -0.593, 0.991, -0.288, 0.522],
     [0.467, 0.711, 0.992, -0.597, 0.014, 0.585, 0.33, -0.062, 0.993, -0.598, 0.146, 0.75, 0.997, -0.605, -0.036, -0.13, 0.005, 0.558, 0.388, 0.74, -0.239, 0.192, 0.992, -0.593, 1.0, -0.604, 0.282, -0.254],
     [-0.177, -0.338, -0.596, 0.992, 0.039, -0.501, -0.02, 0.606, -0.603, 0.993, -0.073, -0.411, -0.615, 0.996, -0.096, 0.213, 0.032, -0.508, -0.19, -0.368, 0.056, -0.643, -0.607, 0.991, -0.604, 1.0, -0.289, 0.53],
     [0.123, 0.197, 0.282, -0.287, -0.151, 0.286, 0.186, -0.245, 0.288, -0.296, 0.007, 0.21, 0.282, -0.286, 0.279, -0.262, -0.144, 0.278, 0.136, 0.193, -0.52, 0.139, 0.289, -0.288, 0.282, -0.289, 1.0, -0.739],
     [-0.067, -0.185, -0.25, 0.529, 0.015, -0.299, 0.018, 0.558, -0.25, 0.535, -0.039, -0.212, -0.254, 0.517, -0.262, 0.406, -0.004, -0.314, -0.094, -0.202, 0.143, -0.521, -0.25, 0.522, -0.254, 0.53, -0.739, 1.0]]
-
```

### Comparing `flavio-2.4.0/flavio/data/parameters_metadata.yml` & `flavio-2.5.0/flavio/data/parameters_metadata.yml`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,118 @@
   tex: $m_{c}(m_{c})$
   description: $c$ quark mass in the $\overline{\text{MS}}$ scheme at the scale $m_c$
 m_b:
   tex: $m_{b}(m_{b})$
   description: $b$ quark mass in the $\overline{\text{MS}}$ scheme at the scale $m_b$
 
 
+# Parameters for LFV quarkonium decay
+f_J/psi:
+  tex: $f_{J/\psi}$
+  description: $J/\psi$ decay constant
+fT_J/psi:
+  tex: $f_{J/\psi}^T$
+  description: $J/\psi$ tensor decay constant
+BR_exp(J/psi->ee):
+  tex: $BR_{\rm exp}(J/\psi\to e^+ e^-)$
+  description: measured branching ratio $J/\psi\to ee$
+
+f_psi(2S):
+  tex: $f_{\psi(2S)}$
+  description: $\psi(2S)$ decay constant
+fT_psi(2S):
+  tex: $f_{\psi(2S)}^T$
+  description: $\psi(2S)$ tensor decay constant
+BR_exp(psi(2S)->ee):
+  tex: $BR_{\rm exp}(\psi(2S)\to e^+ e^-)$
+  description: measured branching ratio $\psi(2S)\to ee$
+
+f_Upsilon(1S):
+  tex: $f_{\Upsilon(1S)}$
+  description: $\Upsilon(1S)$ decay constant
+fT_Upsilon(1S):
+  tex: $f_{\Upsilon(1S)}^T$
+  description: $\Upsilon(1S)$ tensor decay constant
+BR_exp(Upsilon(1S)->ee):
+  tex: $BR_{\rm exp}(\Upsilon(1S)\to e^+ e^-)$
+  description: measured branching ratio $\Upsilon(1S)\to ee$
+
+f_Upsilon(2S):
+  tex: $f_{\Upsilon(2S)}$
+  description: $\Upsilon(2S)$ decay constant
+fT_Upsilon(2S):
+  tex: $f_{\Upsilon(2S)}^T$
+  description: $\Upsilon(2S)$ tensor decay constant
+BR_exp(Upsilon(2S)->ee):
+  tex: $BR_{\rm exp}(\Upsilon(2S)\to e^+ e^-)$
+  description: measured branching ratio $\Upsilon(2S)\to ee$
+
+f_Upsilon(3S):
+  tex: $f_{\Upsilon(3S)}$
+  description: $\Upsilon(3S)$ decay constant
+fT_Upsilon(3S):
+  tex: $f_{\Upsilon(3S)}^T$
+  description: $\Upsilon(3S)$ tensor decay constant
+BR_exp(Upsilon(3S)->ee):
+  tex: $BR_{\rm exp}(\Upsilon(3S)\to e^+ e^-)$
+  description: measured branching ratio $\Upsilon(3S)\to ee$
+
+f_eta_c(1S):
+  tex: $f_{\eta_c(1S)}$
+  description: $\eta_c(1S)$ decay constant
+a_eta_c(1S):
+  tex: $a_{\eta_c(1S)}$
+  description: $\eta_c(1S)$ anomaly decay constant
+
+f_eta_b(1S):
+  tex: $f_{\eta_b(1S)}$
+  description: $\eta_b(1S)$ decay constant
+a_eta_b(1S):
+  tex: $a_{\eta_b(1S)}$
+  description: $\eta_b(1S)$ anomaly decay constant
+
+f_chi_c0(1P):
+  tex: $f_{\chi_{c0}(1P)}$
+  description: $\chi_{c0}(1P)$ decay constant
+a_chi_c0(1P):
+  tex: $a_{\chi_{c0}(1P)}$
+  description: $\chi_{c0}(1P)$ anomaly decay constant
+
+f_chi_b0(1P):
+  tex: $f_{\chi_{b0}(1P)}$
+  description: $\chi_{b0}(1P)$ decay constant
+a_chi_b0(1P):
+  tex: $a_{\chi_{b0}(1P)}$
+  description: $\chi_{b0}(1P)$ anomaly decay constant
+
+f_chi_b0(2P):
+  tex: $f_{\chi_{b0}(2P)}$
+  description: $\chi_{b0}(2P)$ decay constant
+a_chi_b0(2P):
+  tex: $a_{\chi_{b0}(2P)}$
+  description: $\chi_{b0}(2P)$ anomaly decay constant
+
+
+# mass and lifetime of eta_b(1S) manually added, because it is not included in scikit-hep particle code
+m_eta_b(1S):
+  tex: $m_{\eta_b(1S)}$
+  description: $\eta_b(1S)$ mass
+tau_eta_b(1S):
+  tex: $\tau_{\eta_b(1S)}$
+  description: $\eta_b(1S)$ lifetime
+
+# lifetimes of scalar bottomonium not measured yet. These are theoretically calculated lifetimes from the branching ratios of radiative decays.
+tau_chi_b0(1P):
+  tex: $\tau_{\chi_{b0}(1P)}$
+  description: lifetime of $\chi_{b0}(1P)$
+tau_chi_b0(2P):
+  tex: $\tau_{\chi_{b0}(2P)}$
+  description: lifetime of $\chi_{b0}(2P)$
+
+#
 # Meson decay constants
 
 f_K+:
   tex: $f_{K^\pm}$
   description: Charged kaon decay constant
 f_K0:
   tex: $f_{K^0}$
@@ -983,18 +1087,18 @@
   tex: $\Delta_{ta}$
   description: Delta parameter for Fta form factor in KM parametrization
 
 
 # Parameters for the Bs->phi form factors (1503.05534v3)
 Bs->phi LCSR T10:
   tex: $T_1(0)$
-  description: Bs->phi T_1 parameter at q2=0 
+  description: Bs->phi T_1 parameter at q2=0
 Gamma_phi:
   tex: $\Gamma_\phi$
-  description: phi decay width 
+  description: phi decay width
 
 
 
 # experimental decay width differences
 DeltaGamma/Gamma_B0:
   tex: $\Delta \Gamma_d/\Gamma_d$
   description: Relative decay width difference in the $B_s$ system
@@ -1077,14 +1181,26 @@
 # Parameters for B->pi form factors in the BCL parametrization
 B->pi BCL m0:
   tex: $m_{B^*}^{f_0}$
   description: Resonance mass for the $B\to \pi$ scalar form factor in BCL parametrization
 B->pi BCL m+:
   tex: $m_{B^*}^{f_+}$
   description: Resonance mass for the $B\to \pi$ vector and tensor form factors in BCL parametrization
+B->pi BCL LMVD m0:
+  tex: $m_{B^*}^{f_0}$
+  description: Resonance mass for the $B\to \pi$ scalar form factor in BCL parametrization from LMVD
+B->pi BCL LMVD m+:
+  tex: $m_{B^*}^{f_+}$
+  description: Resonance mass for the $B\to \pi$ vector and tensor form factors in BCL parametrization from LMVD
+B->pi BCL LMVD m_B+:
+  tex: $m_{B^+}$
+  description: B+ mass for the $B\to \pi$ form factors in BCL parametrization from LMVD
+B->pi BCL LMVD m_pi0:
+  tex: $m_{\pi^0}$
+  description: pi0 mass for the $B\to \pi$ form factors in BCL parametrization from LMVD
 B->pi BCL a0_f+:
   tex: $a_0^{(+)}$
   description: BCL $B\to \pi$ form factor parametrization coefficient $a_0$ of $f_+$
 B->pi BCL a1_f+:
   tex: $a_1^{(+)}$
   description: BCL $B\to \pi$ form factor parametrization coefficient $a_1$ of $f_+$
 B->pi BCL a2_f+:
@@ -1885,7 +2001,18 @@
 # Parameters for Lambda->p form factors
 Lambda->p f_1(0):
   tex: $f_1(0)$
   description: $\Lambda\to p$ vector form factor $f_1$ at $q^2=0$
 Lambda->p g_1(0):
   tex: $g_1(0)$
   description: $\Lambda\to p$ axial vector form factor $g_1$ at $q^2=0$
+
+# Parameters for parton distribution functions
+PDFmembers avg=0 replicas=1-100:
+  tex: $\text{mem}_{\text{PDF}}$
+  description: member ID of PDF set where mem=0 is average on replicas and mem=1-100 are PDF replicas
+
+# Parameter for Bs->K*0mumu uncertainty inside resonant regions
+# 2209.04457, appendix B, Eq. B7, we save a relative uncertainty
+delta_BsKstarmumu:
+  tex: $\delta_{B_s^0 \to \bar{K}^{\ast 0} \mu \mu}$
+  description: relative uncertainty on the $B_s^0 \to \bar{K}^{\ast 0} \mu \mu$ branching ratio inside the resonant region
```

### Comparing `flavio-2.4.0/flavio/data/parameters_uncorrelated.yml` & `flavio-2.5.0/flavio/data/parameters_uncorrelated.yml`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,58 @@
 # Meson decay constants
 
 f_rho0: 0.212(4)  # 1501.06569 table 1
 f_omega: 0.185(5)  # 1501.06569 table 1
 f_phi: 0.231(5)  # 1501.06569 table 1
 f_Bc: 0.434(15) # 1503.05762v2 eq. (20)
 
+# Parameters for LFV quarkonium decay
+# see also Tables 9 and 11 in 1707.07144 for results of decay constants
+f_J/psi: 0.4104(17) # 2005.01845 abstract
+fT_J/psi: 0.3927(27) # 2008.02024 abstract
+BR_exp(J/psi->ee): 0.05971(32) # PDG 2021
+
+f_psi(2S): 0.2926(12) # Table 3 in 1503.04159 (0.713*f_J/psi), consistent with Tab II in hep-ph/0603164 (0.293)
+fT_psi(2S): 0.2926(12) # assuming equality to vector form factor. This is consistent with the non-relativistic color singlet model.
+BR_exp(psi(2S)->ee): 0.00793(17) # PDG 2021
+
+f_Upsilon(1S): 0.6772(97) # Eq. (29) in 2101.08103
+fT_Upsilon(1S):  0.6772(97) # assuming equality to vector form factor. This is consistent with the non-relativistic color singlet model.
+BR_exp(Upsilon(1S)->ee): 0.0238(11) # PDG 2021
+
+f_Upsilon(2S): 0.481(39) # Eq. (24) in 1408.5768
+fT_Upsilon(2S): 0.481(39) # assuming equality to vector form factor. This is consistent with the non-relativistic color singlet model.
+BR_exp(Upsilon(2S)->ee): 0.0191(16) # PDG 2021
+
+f_Upsilon(3S): 0.395(25) # using Eq.(5.45c) in 2007.01737, consistent with hep-ph/0603164 (0.388)
+fT_Upsilon(3S): 0.395(25) # assuming equality to vector form factor. This is consistent with the non-relativistic color singlet model.
+BR_exp(Upsilon(3S)->ee): 0.0218(20) # PDG 2021
+
+f_eta_c(1S): 0.387(7) # 1312.2858
+a_eta_c(1S): 0.0 # Hazard, Petrov 1607.00815
+
+f_eta_b(1S): 0.724(12) # 2101.08103
+a_eta_b(1S): 0.0 # Hazard, Petrov 1607.00815
+
+f_chi_c0(1P): 0.887 # 1510.04659 - Note, the definition of the decay constant follows 1607.00815
+a_chi_c0(1P): 0.0 # Hazard, Petrov 1607.00815
+
+f_chi_b0(1P): 0.423 # 1510.04659 - Note, the definition of the decay constant follows 1607.00815
+a_chi_b0(1P): 0.0 # Hazard, Petrov 1607.00815
+
+f_chi_b0(2P): 0.421 # 1510.04659 - Note, the definition of the decay constant follows 1607.00815
+a_chi_b0(2P): 0.0 # Hazard, Petrov 1607.00815
+
+m_eta_b(1S): 9.3987(20) # PDG 2022
+tau_eta_b(1S): 100(50) # PDG 2022 (lower error slightly increased to have symmetric errors)
+
+tau_chi_b0(1P): 815(113) # lifetime calculated following 1510.04659
+tau_chi_b0(2P): 1300(255) # calculated following 1510.04659. The final result for the lifetime has been obtained using a simple weighted average of the lifetimes estimated from BR(Upsilon(1S)+gamma) and BR(Upsilon(2S)+gamma) with errors added in quadrature.
+
+
 # Parameters needed for meson light-cone distribution amplitudes
 
 f_perp_omega: 0.135(16)  # 1503.05534v2 table 1, but at 2 GeV, error enlarged
 f_perp_phi: 0.175(4)  # 1503.05534v2 table 1, but at 2 GeV
 a2_para_omega: 0.15(12)
 a2_perp_omega: 0.14(12)
 a2_para_phi: 0.23(8)
@@ -133,14 +177,18 @@
 B->K BCL m0: 5.711 # m_Bs*(0+)
 B->K BCL m+: 5.4154 # m_Bs*(1-)
 
 # B->pi form factors
 B->pi BCL m0: 0
 B->pi BCL m+: 5.319 # m_B*(1-)
 B->pi IW a_T: 0 ± 0.2 # ±20% power correction to Isgur-Wise relation
+B->pi BCL LMVD m0: 5.540 # resonance mass used in LMVD (arXiv:2102.07233)
+B->pi BCL LMVD m+: 5.325 # resonance mass used in LMVD (arXiv:2102.07233)
+B->pi BCL LMVD m_B+: 5.279 # mB+ used in LMVD (arXiv:2102.07233)
+B->pi BCL LMVD m_pi0: 0.135 # mpi0 used in LMVD (arXiv:2102.07233)
 
 # Bs->K form factors (1501.05373v3)
 Bs->K BCL m0: 5.63 # m_B*(0+)
 Bs->K BCL m+: 5.3252 # m_B*(1-)
 
 # Parameters needed for B->gamma form factors (hep-ph/0208256)
 B->gamma KM betav: 0.28
@@ -224,18 +272,18 @@
 Lambdab->Lambda deltaC9 c_para0 Im: 0 ± 0.3
 Lambdab->Lambda deltaC9 c_perp1 Re: 0 ± 0.3
 Lambdab->Lambda deltaC9 c_perp1 Im: 0 ± 0.3
 Lambdab->Lambda deltaC9 c_para1 Re: 0 ± 0.3
 Lambdab->Lambda deltaC9 c_para1 Im: 0 ± 0.3
 
 # Parameters for the form factor calculation in the quark model of Lambdab->Lambda(1520)ll
-Lambdab->Lambda(1520) m_q: 0.2848  
+Lambdab->Lambda(1520) m_q: 0.2848
 Lambdab->Lambda(1520) m_s: 0.5553
 Lambdab->Lambda(1520) alpha_Lambdab: 0.443
-Lambdab->Lambda(1520) alpha_Lambda(1520): 0.333 
+Lambdab->Lambda(1520) alpha_Lambda(1520): 0.333
 
 Lambdab->Lambda(1520) fVt uncertainty: 1 +- 0.1
 Lambdab->Lambda(1520) fVperp uncertainty: 1 +- 0.1
 Lambdab->Lambda(1520) fV0 uncertainty: 1 +- 0.1
 Lambdab->Lambda(1520) fVg uncertainty: 1 +- 0.3
 Lambdab->Lambda(1520) fAt uncertainty: 1 +- 0.1
 Lambdab->Lambda(1520) fAperp uncertainty: 1 +- 0.1
@@ -491,7 +539,18 @@
 D->pi BSZ a0_fT: 0.506(79)
 D->pi BSZ a1_fT: 0.28(3)
 D->pi BSZ a2_fT: 0
 # D->K
 D->K BSZ a0_fT: 0.687(54)
 D->K BSZ a1_fT: 0.10(1)
 D->K BSZ a2_fT: 0
+
+# Parameters for parton distribution functions
+PDFmembers avg=0 replicas=1-100:
+  distribution: discrete_uniform
+  lowest_value: 0
+  highest_value: 100
+  central_value: 0
+
+# Parameter for Bs->K*0mumu uncertainty inside resonant regions
+# 2209.04457, appendix B, Eq. B7, we save a relative uncertainty
+delta_BsKstarmumu: 0 ± 0.078
```

### Comparing `flavio-2.4.0/flavio/data/test/2009.09313_digitized.npz` & `flavio-2.5.0/flavio/data/test/2009.09313_digitized.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/data/test/SPheno-2.spc.MSSM` & `flavio-2.5.0/flavio/data/test/SPheno-2.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/data/test/SPheno.spc.MSSM` & `flavio-2.5.0/flavio/data/test/SPheno.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/functions.py` & `flavio-2.5.0/flavio/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/io/instanceio.py` & `flavio-2.5.0/flavio/io/instanceio.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/io/test_yaml.py` & `flavio-2.5.0/flavio/io/test_yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/io/yaml.py` & `flavio-2.5.0/flavio/io/yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/math/functions.py` & `flavio-2.5.0/flavio/math/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/math/integrate.py` & `flavio-2.5.0/flavio/math/integrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 import numpy as np
 import warnings
 try:
     from scipy.integrate import AccuracyWarning # scipy >= 1.5.0
 except ImportError:
     from scipy.integrate.quadrature import AccuracyWarning # scipy <= 1.4.1
 
-def nintegrate(f, a, b, epsrel=0.005, **kwargs):
+def nintegrate_quadrature(f, a, b, epsrel=0.005, **kwargs):
     with warnings.catch_warnings():
         # ignore AccuracyWarning that is issued when an integral is zero
         warnings.filterwarnings("ignore", category=AccuracyWarning)
         return scipy.integrate.quadrature(f, a, b, rtol=epsrel, tol=0, vec_func=False, **kwargs)[0]
 
+def nintegrate(f, a, b, epsrel=0.005, **kwargs):
+    with warnings.catch_warnings():
+        # ignore AccuracyWarning that is issued when an integral is zero
+        warnings.filterwarnings("ignore", category=AccuracyWarning)
+        return scipy.integrate.quad(f, a, b, epsabs=0, epsrel=epsrel, **kwargs)[0]
+
 def nintegrate_fast(f, a, b, N=5, **kwargs):
     x = np.linspace(a,b,N)
     y = np.array([f(X) for X in x])
     f_interp = scipy.interpolate.interp1d(x, y, kind='cubic')
     x_fine = np.linspace(a,b,N*4)
     y_interp = np.array([f_interp(X) for X in x_fine])
     return np.trapz(y_interp, x=x_fine)
```

### Comparing `flavio-2.4.0/flavio/math/optimize.py` & `flavio-2.5.0/flavio/math/optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/math/test_math.py` & `flavio-2.5.0/flavio/math/test_math.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/math/test_optimize.py` & `flavio-2.5.0/flavio/math/test_optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/measurements.py` & `flavio-2.5.0/flavio/measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/parameters.py` & `flavio-2.5.0/flavio/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     with open(filename, 'r') as f:
         _read_yaml_object_metadata(f, constraints)
 
 def _read_yaml_object_values(obj, constraints):
     parameters = yaml.safe_load(obj)
     for parameter_name, value in parameters.items():
         p = Parameter[parameter_name] # this will raise an error if the parameter doesn't exist!
-        constraints.set_constraint(parameter_name, value)
+        if isinstance(value, dict):
+            constraints.set_constraint(parameter_name, constraint_dict=value)
+        else:
+            constraints.set_constraint(parameter_name, value)
 
 def _read_yaml_object_new(obj):
     """Read parameter constraints from a YAML stream or file that are compatible
     with the format generated by the `get_yaml` method of
     `flavio.classes.ParameterConstraints`."""
     parameters = yaml.safe_load(obj)
     return ParameterConstraints.from_yaml_dict(parameters)
@@ -155,14 +158,21 @@
         'rho+': 213,
         'rho0': 113,
         't': 6,
         'tau': 15,
         'u': 2,
         'p': 2212,
         'n': 2112,
+        'Upsilon(1S)' : 553,
+        'Upsilon(2S)' : 100553,
+        'Upsilon(3S)' : 200553,
+        'eta_c(1S)' : 441,
+        'chi_c0(1P)' : 10441,
+        'chi_b0(1P)' : 10551,
+        'chi_b0(2P)' : 110551,
     }
     _pdg_particles_inv = {v:k for k,v in PDG_PARTICLES.items()}
     _pdg_tex_regex = re.compile(
         r"^([A-Za-z\\/]+)" # latin or greek letters or slash
         r"(?:_\{(.*?)\})*" # _{...}
         r"(?:\^\{(.*?)\})*" # ^{...}
         r"(?:\((.*?)\))*" # (...)
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/__init__.py` & `flavio-2.5.0/flavio/physics/bdecays/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/angular.py` & `flavio-2.5.0/flavio/physics/bdecays/angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bc_lifetime.py` & `flavio-2.5.0/flavio/physics/bdecays/bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bll.py` & `flavio-2.5.0/flavio/physics/bdecays/bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bllgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/bllgamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,16 @@
 def dGdsMN(s, par, B, ff, ff0, lep, wc):
     return dG1dsMN(s, par, B, ff, ff0, lep, wc) + dG2dsMN(s, par, B, ff, ff0, lep, wc) + dG12dsMN(s, par, B, ff, ff0, lep, wc)
 
 
 def bllg_dbrdq2(q2, wc_obj, par, B, lep):
     if q2 >= 8.7 and q2 < 14 and lep != 'tau':
         warnings.warn("The predictions in the region of narrow charmonium resonances are not meaningful")
+    if q2 >= 0.7 and q2 < 1.1:
+        warnings.warn("Numerical integration in the region of phi, rho and omega resonances may be unreliable.")
     tauB = par['tau_'+B]
     ml = par['m_'+lep]
     mB = par['m_'+B]
     scale = config['renormalization scale']['bllgamma']
     ff = get_ff(q2, par, B)
     ff0 = get_ff(0, par, B)
     label = meson_quark[B]+lep+lep
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/blnu.py` & `flavio-2.5.0/flavio/physics/bdecays/blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bpll.py` & `flavio-2.5.0/flavio/physics/bdecays/bpll.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 # form factors
 def get_ff(q2, par, B, P):
     ff_name = meson_ff[(B,P)] + ' form factor'
     return AuxiliaryQuantity[ff_name].prediction(par_dict=par, wc_obj=None, q2=q2)
 
 # get subleading hadronic contribution
 def get_subleading(q2, wc_obj, par_dict, B, P, lep, cp_conjugate):
+    if 'B' in B and 'pi' in P:
+        # skip subleading correction for B->pi decays
+        return {}
     if q2 <= 9:
         sub_name = B+'->'+P + 'll subleading effects at low q2'
         return AuxiliaryQuantity[sub_name].prediction(par_dict=par_dict, wc_obj=wc_obj, q2=q2, cp_conjugate=cp_conjugate)
     elif q2 > 14:
         sub_name = B+'->'+P + 'll subleading effects at high q2'
         return AuxiliaryQuantity[sub_name].prediction(par_dict=par_dict, wc_obj=wc_obj, q2=q2, cp_conjugate=cp_conjugate)
     else:
@@ -145,14 +148,27 @@
         ml = par['m_'+lep]
         ml = par['m_'+lep]
         q2max = (mB-mP)**2
         q2min = (ml+ml)**2
         return bpll_dbrdq2_int(q2min, q2max, wc_obj, par, B, P, lep)*(q2max-q2min)
     return fct
 
+def bpll_dbrdq2_Belle_func(B, P, lep):
+    def fct(wc_obj, par):
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="The predictions in the region of narrow charmonium resonances are not meaningful")
+            warnings.filterwarnings("ignore", message="The QCDF corrections should not be trusted .*")
+            mB = par['m_'+B]
+            mP = par['m_'+P]
+            ml = par['m_'+lep]
+            ml = par['m_'+lep]
+            q2max = (mB-mP)**2
+            q2min = (ml+ml)**2
+            return bpll_dbrdq2_int(q2min, q2max, wc_obj, par, B, P, lep, epsrel=0.0002)*(q2max-q2min)
+    return fct
 
 def bpll_dbrdq2_func(B, P, lep):
     def fct(wc_obj, par, q2):
         return bpll_dbrdq2(q2, wc_obj, par, B, P, lep)
     return fct
 
 def bpll_obs_int_ratio_func(func_num, func_den, B, P, lep):
@@ -202,14 +218,16 @@
 'ACP': {'func_num': dGdq2_cpdiff, 'tex': r'A_\text{CP}', 'desc': 'Direct CP asymmetry'},
 'AFB': {'func_num': AFB_cpaverage_num, 'tex': r'A_\text{FB}', 'desc': 'forward-backward asymmetry'},
 'FH': {'func_num': FH_cpaverage_num, 'tex': r'F_H', 'desc': 'flat term'},
 }
 _hadr = {
 'B0->K': {'tex': r"B^0\to K^0", 'B': 'B0', 'P': 'K0', },
 'B+->K': {'tex': r"B^\pm\to K^\pm ", 'B': 'B+', 'P': 'K+', },
+'B0->pi': {'tex': r"\bar B^0\to \pi^0", 'B': 'B0', 'P': 'pi0', },
+'B+->pi': {'tex': r"B^\pm\to \pi^\pm ", 'B': 'B+', 'P': 'pi+', },
 }
 _hadr_lfv = {
 'B0->K': {'tex': r"\bar B^0\to \bar K^0", 'B': 'B0', 'P': 'K0', },
 'B+->K': {'tex': r"B^-\to K^-", 'B': 'B+', 'P': 'K+', },
 'B0->pi': {'tex': r"\bar B^0\to \pi^0", 'B': 'B0', 'P': 'pi0', },
 'B+->pi': {'tex': r"B^-\to \pi^-", 'B': 'B+', 'P': 'pi+', },
 }
@@ -252,14 +270,22 @@
         _obs_name = "dBR/dq2("+M+l+l+")"
         _obs = Observable(name=_obs_name, arguments=['q2'])
         _obs.set_description(r"Differential branching ratio of $" + _process_tex + r"$")
         _obs.tex = r"$\frac{d\text{BR}}{dq^2}(" + _process_tex + r")$"
         _obs.add_taxonomy(_process_taxonomy)
         Prediction(_obs_name, bpll_dbrdq2_func(_hadr[M]['B'], _hadr[M]['P'], l))
 
+        if l == 'e' and M == 'B+->pi':
+            _obs_name = "BR_Belle("+M+l+l+")"
+            _obs = Observable(name=_obs_name)
+            _obs.set_description(r"Branching ratio of $" + _process_tex + r"$")
+            _obs.tex = r"$\text{BR}(" + _process_tex + r")$"
+            _obs.add_taxonomy(_process_taxonomy)
+            Prediction(_obs_name, bpll_dbrdq2_Belle_func(_hadr[M]['B'], _hadr[M]['P'], l))
+
         # only for tau: total branching ratio
         if l == 'tau':
             _obs_name = "BR("+M+l+l+")"
             _obs = Observable(name=_obs_name)
             _obs.set_description(r"Branching ratio of $" + _process_tex + r"$")
             _obs.tex = r"$\text{BR}(" + _process_tex + r")$"
             _obs.add_taxonomy(_process_taxonomy)
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bpll_lfv.py` & `flavio-2.5.0/flavio/physics/bdecays/bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bpll_subleading.py` & `flavio-2.5.0/flavio/physics/bdecays/bpll_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bplnu.py` & `flavio-2.5.0/flavio/physics/bdecays/bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bpnunu.py` & `flavio-2.5.0/flavio/physics/bdecays/bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/amplitudes.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/amplitudes.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     if q2 >= 8.9:
         return {('0' ,'V'): 0, ('pl' ,'V'): 0, ('mi' ,'V'): 0, }
     ss_name = B+'->'+V+'ll spectator scattering'
     return AuxiliaryQuantity[ss_name].prediction(par_dict=par_dict, wc_obj=wc_obj, q2=q2, cp_conjugate=cp_conjugate)
 
 # get subleading hadronic contribution at low q2
 def get_subleading(q2, wc_obj, par_dict, B, V, cp_conjugate):
+    if B=='Bs' and V == 'K*0':
+        # skip subleading contribution for Bs->K*0 for now
+        return {}
     if q2 <= 9:
         sub_name = B+'->'+V+ 'll subleading effects at low q2'
         return AuxiliaryQuantity[sub_name].prediction(par_dict=par_dict, wc_obj=wc_obj, q2=q2, cp_conjugate=cp_conjugate)
     elif q2 > 14:
         sub_name = B+'->'+V+ 'll subleading effects at high q2'
         return AuxiliaryQuantity[sub_name].prediction(par_dict=par_dict, wc_obj=wc_obj, q2=q2, cp_conjugate=cp_conjugate)
     else:
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/lfv.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/nonfactorizable.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/nonfactorizable.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def function(wc_obj, par_dict, q2, cp_conjugate):
         return flavio.physics.bdecays.bvll.qcdf_interpolate.helicity_amps_qcdf(q2, par_dict, B, V, cp_conjugate, contribution)
     return function
 
 # loop over hadronic transitions and lepton flavours
 # BTW, it is not necessary to loop over tau: for tautau final states, the minimum
 # q2=4*mtau**2 is so high that QCDF is not valid anymore anyway!
-for had in [('B0','K*0'), ('B+','K*+'), ('B0','rho0'), ('B+','rho+'), ('Bs','phi'), ]:
+for had in [('B0','K*0'), ('B+','K*+'), ('B0','rho0'), ('B+','rho+'), ('Bs','phi'), ('Bs', 'K*0'), ]:
     process = had[0] + '->' + had[1] + 'll' # e.g. B0->K*0mumu
     quantity = process + ' spectator scattering'
     a = AuxiliaryQuantity(name=quantity, arguments=['q2', 'cp_conjugate'])
     a.description = ('Contribution to ' + process + ' helicity amplitudes from'
                     ' non-factorizable spectator scattering.')
 
     # Implementation: QCD factorization
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/observables.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/observables_bs.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/observables_bs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 the finite life-time difference between the $B_s$ mass eigenstates,
 see arXiv:1502.05509."""
 
 import flavio
 from . import observables
 from flavio.classes import Observable, Prediction
 import cmath
+import warnings
 
 def bsvll_obs(function, q2, wc_obj, par, B, V, lep):
     ml = par['m_'+lep]
     mB = par['m_'+B]
     mV = par['m_'+V]
     y = par['DeltaGamma/Gamma_'+B]/2.
     if q2 < 4*ml**2 or q2 > (mB-mV)**2:
@@ -117,25 +118,38 @@
         num = bsvll_obs(func_num, q2, wc_obj, par, B, V, lep)
         if num == 0:
             return 0
         denom = bsvll_obs(func_den, q2, wc_obj, par, B, V, lep)
         return num/denom
     return fct
 
+# function for the LHCb (1804.07167) Bs->K*0 integrated branching ratio
+def bsvll_dbrdq2_19_func(B, P, lep):
+    def fct(wc_obj, par):
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="The predictions in the region of narrow charmonium resonances are not meaningful.*")
+            warnings.filterwarnings("ignore", message="The QCDF corrections should not be trusted*")
+
+            q2max = 19
+            q2min = 0.1
+            return (1+par['delta_BsKstarmumu'])*bsvll_dbrdq2_int(q2min, q2max, wc_obj, par, B, P, lep)*(q2max-q2min)
+    return fct
+
 # Observable and Prediction instances
 
 _tex = {'e': 'e', 'mu': '\mu', 'tau': r'\tau'}
 _observables = {
 'FL': {'func_num': FL_num_Bs, 'tex': r'\overline{F_L}', 'desc': 'Time-averaged longitudinal polarization fraction'},
 'S3': {'func_num': lambda y, J, J_bar, J_h: S_experiment_num_Bs(y, J, J_bar, J_h, 3), 'tex': r'\overline{S_3}', 'desc': 'Time-averaged, CP-averaged angular observable'},
 'S4': {'func_num': lambda y, J, J_bar, J_h: S_experiment_num_Bs(y, J, J_bar, J_h, 4), 'tex': r'\overline{S_4}', 'desc': 'Time-averaged, CP-averaged angular observable'},
 'S7': {'func_num': lambda y, J, J_bar, J_h: S_experiment_num_Bs(y, J, J_bar, J_h, 7), 'tex': r'\overline{S_7}', 'desc': 'Time-averaged, CP-averaged angular observable'},
 }
 _hadr = {
 'Bs->phi': {'tex': r"B_s\to \phi ", 'B': 'Bs', 'V': 'phi', },
+'Bs->K*0': {'tex': r"B_s\to K^* ", 'B': 'Bs', 'V': 'K*0', },
 }
 for l in ['e', 'mu', 'tau']:
     for M in _hadr.keys():
 
         _process_tex = _hadr[M]['tex'] +_tex[l]+r"^+"+_tex[l]+r"^-"
         _process_taxonomy = r'Process :: $b$ hadron decays :: FCNC decays :: $B\to V\ell^+\ell^-$ :: $' + _process_tex + r"$"
 
@@ -169,14 +183,23 @@
         _obs_name = "dBR/dq2("+M+l+l+")"
         _obs = Observable(name=_obs_name, arguments=['q2'])
         _obs.set_description(r"Differential time-integrated branching ratio of $" + _hadr[M]['tex'] +_tex[l]+r"^+"+_tex[l]+"^-$")
         _obs.tex = r"$\frac{d\overline{\text{BR}}}{dq^2}(" + _hadr[M]['tex'] +_tex[l]+r"^+"+_tex[l]+"^-)$"
         _obs.add_taxonomy(_process_taxonomy)
         Prediction(_obs_name, bsvll_dbrdq2_func(_hadr[M]['B'], _hadr[M]['V'], l))
 
+        # for Bs->K*0 mu mu we add a separate observable for the measurement in 1804.07167
+        if M == 'Bs->K*0' and l == 'mu':
+            _obs_name = "BR_LHCb("+M+l+l+")"
+            _obs = Observable(name=_obs_name)
+            _obs.set_description(r"Branching ratio of $" + _hadr[M]['tex'] +_tex[l]+r"^+"+_tex[l]+"^-$ measured by LHCb in 2018")
+            _obs.tex = r"$\overline{\text{BR}}(" + _hadr[M]['tex'] +_tex[l]+r"^+"+_tex[l]+"^-)$"
+            _obs.add_taxonomy(_process_taxonomy)
+            Prediction(_obs_name, bsvll_dbrdq2_19_func(_hadr[M]['B'], _hadr[M]['V'], l))
+
 # Lepton flavour ratios
 for l in [('mu','e'), ('tau','mu'),]:
     for M in _hadr.keys():
 
         # binned ratio of BRs
         _obs_name = "<R"+l[0]+l[1]+">("+M+"ll)"
         _obs = Observable(name=_obs_name, arguments=['q2min', 'q2max'])
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/qcdf.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/qcdf_interpolate.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/subleading.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/test_bvll.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/test_bvll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/test_lfv.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/test_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/test_qcdf.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/test_qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py` & `flavio-2.5.0/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvlnu.py` & `flavio-2.5.0/flavio/physics/bdecays/bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bvnunu.py` & `flavio-2.5.0/flavio/physics/bdecays/bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bxgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bxll.py` & `flavio-2.5.0/flavio/physics/bdecays/bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bxll_qed.py` & `flavio-2.5.0/flavio/physics/bdecays/bxll_qed.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/bxlnu.py` & `flavio-2.5.0/flavio/physics/bdecays/bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/common.py` & `flavio-2.5.0/flavio/physics/bdecays/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ('Lambdab','Lambda'): 'bs',
 ('Lambdab','Lambda(1520)'): 'bs',
 ('B0','pi0'): 'bd',
 ('B+','pi+'): 'bd',
 ('B0','rho0'): 'bd',
 ('B+','rho+'): 'bd',
 ('B0','omega'): 'bd',
+('Bs','K*0'): 'bd',
 ('Bs','K+'): 'bu',
 ('Bs','K*+'): 'bu',
 ('B0','pi+'): 'bu',
 ('B0','rho+'): 'bu',
 ('B0','pi+'): 'bu',
 ('B+','pi0'): 'bu',
 ('B+','rho0'): 'bu',
@@ -51,14 +52,15 @@
 
 meson_spectator = {
 ('B+','K+'): 'u',
 ('B0','K0'): 'd',
 ('B+','K*+'): 'u',
 ('B0','K*0'): 'd',
 ('Bs','phi'): 's',
+('Bs', 'K*0'): 's',
 }
 
 quark_charge = {
 'u':  2/3.,
 'd': -1/3.,
 's': -1/3.,
 }
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bcl.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bsz.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/btop.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/btop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flavio.physics.bdecays.formfactors.b_p import bcl, cln, bsz
+from flavio.physics.bdecays.formfactors.b_p import bcl, cln, bsz, bcl_lmvd
 from flavio.classes import AuxiliaryQuantity, Implementation
 from flavio.config import config
 
 processes_H2L = ['B->K', 'B->pi']  # heavy to light
 processes_H2H = ['B->D', ]  # heavy to heavy
 
 
@@ -26,14 +26,19 @@
     i.set_description("3-parameter BCL parametrization (see arXiv:0807.2722).")
 
     iname = p + ' BCL4'
     i = Implementation(name=iname, quantity=quantity,
                    function=ff_function(bcl.ff, p, n=4))
     i.set_description("4-parameter BCL parametrization (see arXiv:0807.2722).")
 
+    iname = p + ' BCL4-LMVD'
+    i = Implementation(name=iname, quantity=quantity,
+                   function=ff_function(bcl_lmvd.ff, p, n=4))
+    i.set_description("4-parameter BCL parametrization from LMVD (see arXiv:2102.07233).")
+
     iname = p + ' BCL3-IW'
     i = Implementation(name=iname, quantity=quantity,
                    function=ff_function(bcl.ff_isgurwise, p,
                    scale=config['renormalization scale']['bpll'], n=3))
     i.set_description("3-parameter BCL parametrization using improved Isgur-Wise relation"
                       " for the tensor form factor")
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_p/cln.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_p/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/bsz.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/btov.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/cln.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/cln.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from math import sqrt, pi
 from flavio.physics.bdecays.common import meson_ff
 from flavio.physics.bdecays.formfactors import hqet
 from flavio.physics.bdecays.formfactors import common
 from flavio.classes import AuxiliaryQuantity
 from flavio.physics.running import running
+from flavio.physics.common import lambda_K
 
 process_dict = {}
 process_dict['B->D*'] = {'B': 'B0', 'V': 'D*+', 'q': 'b->c'}
 
 
 def h_to_A(mB, mV, h, q2):
     """Convert HQET form factors to the standard basis.
@@ -30,17 +31,16 @@
     ff['A12'] = ((ff['A1'] * (mB + mV)**2 * (mB**2 - mV**2 - q2)
                  - ff['A2'] * (mB**4 + (mV**2 - q2)**2
                  - 2 * mB**2 * (mV**2 + q2)))
                  / (16. * mB * mV**2 * (mB + mV)))
     del ff['A2']
     # conversion from T_2, T_3 to T_23
     ff['T23'] = ((mB**2 - mV**2) * (mB**2 + 3 * mV**2 - q2) * ff['T2']
-                 - (mB**4 + (mV**2 - q2)**2
-                 - 2 * mB**2 * (mV**2 + q2)) * ff['T3']
-                 ) / (8 * mB * (mB - mV) * mV**2)
+                 - lambda_K(mB**2, mV**2, q2) * ff['T3']
+                ) / (8 * mB * (mB - mV) * mV**2)
     del ff['T3']
     return ff
 
 def ff(process, q2, par, scale, order_z=3, order_z_slp=2, order_z_sslp=1):
     r"""Central value of $B\to V$ form factors in the lattice convention
     CLN parametrization.
 
@@ -77,24 +77,26 @@
                    + epsc * (L[2] - L[5])
                    + epsb * (L[1] - L[4])
                    + epsc**2 * (ell[2] - ell[5]))
     h['A1'] = xi * (1 + ash * CA1
                     + epsc * (L[2] - L[5] * (w - 1)/(w + 1))
                     + epsb * (L[1] - L[4] * (w - 1)/(w + 1))
                     + epsc**2 * (ell[2] - ell[5] * (w - 1)/(w + 1)))
-    h['A2'] = xi * (ash * CA2 + epsc * (L[3] + L[6]))
+    h['A2'] = xi * (ash * CA2
+                    + epsc * (L[3] + L[6])
+                    + epsc**2 * (ell[3] + ell[6]))
     h['A3'] = xi * (1 + ash * (CA1 + CA3)
                     + epsc * (L[2] - L[3] + L[6] - L[5])
                     + epsb * (L[1] - L[4])
                     + epsc**2 * (ell[2] - ell[3] + ell[6] - ell[5]))
     h['T1'] = xi * (1 + ash * (CT1 + (w - 1)/2 * (CT2 - CT3))
                     + epsc * L[2]
                     + epsb * L[1]
                     + epsc**2 * ell[2])
     h['T2'] = xi * (ash * (w + 1)/2 * (CT2 + CT3)
                     + epsc * L[5]
                     - epsb * L[4]
-                    + epsc * ell[5])
+                    + epsc**2 * ell[5])
     h['T3'] = xi * (ash * CT2
                     + epsc * (L[6] - L[3])
-                    + epsc * (ell[6] - ell[3]))
+                    + epsc**2 * (ell[6] - ell[3]))
     return h_to_A(mB, mV, h, q2)
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/clnexp.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/clnexp.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/isgurwise.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/isgurwise.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/sse.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/b_v/test_btov.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/b_v/test_btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/common.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/hqet.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/hqet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 from functools import lru_cache
 from flavio.math.functions import li2
 from flavio.physics.running import running
 from flavio.physics.bdecays.formfactors import common
 
 
 def get_hqet_parameters(par):
+    # use value from EOS fit of arXiv:1908.09398
+    # https://github.com/eos/eos/blob/417d909b35f7eac3b1ac7b6a552ff68aa20ff41d/eos/form-factors/mesonic-hqet.hh#L185-L191
     p = {}
-    # The scale here is fixed to 2.7 GeV ~ sqrt(m_b^pole * m_c^pole)
-    alphas = running.get_alpha(par, scale=2.7, nf_out=5)['alpha_s']
+    alphas = 0.26
     p['ash'] = alphas / pi
-    p['mb1S'] = running.get_mb_1S(par)
+    p['mb1S'] = 4.71
     p['mb'] = p['mb1S'] * (1 + 2 * alphas**2 / 9)
     p['mc'] = p['mb'] - 3.4
-    mBbar = (par['m_B0'] + 3 * par['m_B*0']) / 4
+    mBbar = 5.313
     # eq. (25); note the comment about the renormalon cancellation thereafter
-    p['Lambdabar'] = mBbar - p['mb'] + par['lambda_1'] / (2 * p['mb1S'])
+    lambda_1 = -0.3
+    p['Lambdabar'] = mBbar - p['mb'] + lambda_1 / (2 * p['mb1S'])
     p['epsc'] = p['Lambdabar'] / (2 * p['mc'])
     p['epsb'] = p['Lambdabar'] / (2 * p['mb'])
     p['zc'] = p['mc'] / p['mb']
     return p
 
 def xi(z, rho2, c, xi3, order_z):
     r"""Leading-order Isgur-Wise function:
-    
+
     $$\xi(z)=1-\rho^2 (w-1) + c (w-1)^2 + \xi^{(3)} (w-1)^3/6
-    
+
     where w=w(z) is expanded in $z$ up to an including terms of order
     `z**order_z`.
     """
     xi = (1
           - rho2    * common.w_minus_1_pow_n(z, n=1, order_z=order_z)
           + c       * common.w_minus_1_pow_n(z, n=2, order_z=order_z)
           + xi3 / 6 * common.w_minus_1_pow_n(z, n=3, order_z=order_z))
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/sse.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/formfactors/test_cln.py` & `flavio-2.5.0/flavio/physics/bdecays/formfactors/test_cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/lambdablambda1520ll.py` & `flavio-2.5.0/flavio/physics/bdecays/lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/lambdablambdall.py` & `flavio-2.5.0/flavio/physics/bdecays/lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/lambdablambdall_subleading.py` & `flavio-2.5.0/flavio/physics/bdecays/lambdablambdall_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/matrixelements.py` & `flavio-2.5.0/flavio/physics/bdecays/matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_angular.py` & `flavio-2.5.0/flavio/physics/bdecays/test_angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bc_lifetime.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bll.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bllgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bllgamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,11 @@
 par = c.get_central_all()
 
 wc_obj = WilsonCoefficients()
 
 class TestBllgamma(unittest.TestCase):
     def test_bllgamma(self):
         # numerical comparison to the code used for 1708.02649
-        self.assertAlmostEqual(bllg_dbrdq2_int(0.04465, 8.641, wc_obj, par, 'Bs', 'mu')*10**9, 8.4, places=0)
+        #self.assertAlmostEqual(bllg_dbrdq2_int(0.04465, 8.641, wc_obj, par, 'Bs', 'mu')*10**9, 8.4, places=0)
         self.assertAlmostEqual(bllg_dbrdq2_int(15.84, 28.27, wc_obj, par, 'Bs', 'mu')*10**9, 1.7, places=0)
-        self.assertAlmostEqual(bllg_dbrdq2_int(0.04465, 8.641, wc_obj, par, 'Bs', 'e')*10**9, 9.0, places=0)
+        #self.assertAlmostEqual(bllg_dbrdq2_int(0.04465, 8.641, wc_obj, par, 'Bs', 'e')*10**9, 9.0, places=0)
         self.assertAlmostEqual(bllg_dbrdq2_int(15.84, 28.27, wc_obj, par, 'Bs', 'e')*10**9, 1.4, places=0)
-        
-
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_blnu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bpll.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bpll_lfv.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bplnu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bpnunu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bvgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bvlnu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bvnunu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bxgamma.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bxll.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_bxlnu.py` & `flavio-2.5.0/flavio/physics/bdecays/test_bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_lambdablambda1520ll.py` & `flavio-2.5.0/flavio/physics/bdecays/test_lambdablambda1520ll.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,18 +79,18 @@
 class TestLambdabLambda1520ll(TestLambdabLambda1520):
 
     def test_lambdablambda1520ll_binned_qmff_sm(self):
         # compare to SM values in table 1 of 2005.09602 using the quark model form factors
         # Differences due to C9eff = C9 and C7eff = C7
         flavio.config['implementation']['Lambdab->Lambda(1520) form factor'] = 'Lambdab->Lambda(1520) MCN'
 
-        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.397, rtol=0.17, scalef=1e9, q2min=0.1, q2max=3)
-        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 1.29, rtol=0.07, scalef=1e9, q2min=3, q2max=6)
-        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 3.22, rtol=0.09, scalef=1e9, q2min=6, q2max=8.68)
-        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.95, rtol=0.07, scalef=1e9, q2min=1, q2max=6)
+        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.397, rtol=0.18, scalef=1e9, q2min=0.1, q2max=3)
+        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 1.29, rtol=0.08, scalef=1e9, q2min=3, q2max=6)
+        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 3.22, rtol=0.10, scalef=1e9, q2min=6, q2max=8.68)
+        self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.95, rtol=0.08, scalef=1e9, q2min=1, q2max=6)
 
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', 0.048, rtol=0.57, q2min=0.1, q2max=3)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.127, rtol=0.16, q2min=3, q2max=6)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.235, rtol=0.03, q2min=6, q2max=8.68)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.098, rtol=0.24, q2min=1, q2max=6)
```

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_lambdablambdall.py` & `flavio-2.5.0/flavio/physics/bdecays/test_lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_matrixelements.py` & `flavio-2.5.0/flavio/physics/bdecays/test_matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/test_wc.py` & `flavio-2.5.0/flavio/physics/bdecays/test_wc.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/bdecays/wilsoncoefficients.py` & `flavio-2.5.0/flavio/physics/bdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/betadecays/common.py` & `flavio-2.5.0/flavio/physics/betadecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/betadecays/ft.py` & `flavio-2.5.0/flavio/physics/betadecays/ft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/betadecays/test_betadecays.py` & `flavio-2.5.0/flavio/physics/betadecays/test_betadecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ckm.py` & `flavio-2.5.0/flavio/physics/ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/common.py` & `flavio-2.5.0/flavio/physics/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat` & `flavio-2.5.0/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/README` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/README`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat` & `flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat` & `flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d` & `flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat` & `flavio-2.5.0/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json` & `flavio-2.5.0/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz` & `flavio-2.5.0/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 109606 bytes, number of entries: 24
+Zip file size: 146774 bytes, number of entries: 32
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 all.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 WA.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 O8.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 QSS.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 CP conjugate all.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 CP conjugate WA.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 B0->K*0 CP conjugate O8.npy
@@ -19,8 +19,16 @@
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi WA.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi O8.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi QSS.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi CP conjugate all.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi CP conjugate WA.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi CP conjugate O8.npy
 ?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->phi CP conjugate QSS.npy
-24 files, 106752 bytes uncompressed, 106752 bytes compressed:  0.0%
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 all.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 WA.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 O8.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 QSS.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 CP conjugate all.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 CP conjugate WA.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 CP conjugate O8.npy
+?rw-------  2.0 unx     4448 b- stor 80-Jan-01 00:00 Bs->K*0 CP conjugate QSS.npy
+32 files, 142336 bytes uncompressed, 142336 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_ifw2i81z_/tmpg5oe32un_.zip

```diff
@@ -66,8 +66,32 @@
 
 Filename: Bs->phi CP conjugate O8.npy
 Comment: 
 
 Filename: Bs->phi CP conjugate QSS.npy
 Comment: 
 
+Filename: Bs->K*0 all.npy
+Comment: 
+
+Filename: Bs->K*0 WA.npy
+Comment: 
+
+Filename: Bs->K*0 O8.npy
+Comment: 
+
+Filename: Bs->K*0 QSS.npy
+Comment: 
+
+Filename: Bs->K*0 CP conjugate all.npy
+Comment: 
+
+Filename: Bs->K*0 CP conjugate WA.npy
+Comment: 
+
+Filename: Bs->K*0 CP conjugate O8.npy
+Comment: 
+
+Filename: Bs->K*0 CP conjugate QSS.npy
+Comment: 
+
 Zip file comment:
```

### Comparing `flavio-2.4.0/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy` & `flavio-2.5.0/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/dlnu.py` & `flavio-2.5.0/flavio/physics/ddecays/dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/dplnu.py` & `flavio-2.5.0/flavio/physics/ddecays/dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/formfactors/__init__.py` & `flavio-2.5.0/flavio/physics/ddecays/formfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/formfactors/bcl.py` & `flavio-2.5.0/flavio/physics/ddecays/formfactors/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/formfactors/bsz.py` & `flavio-2.5.0/flavio/physics/ddecays/formfactors/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/formfactors/test_formfactors.py` & `flavio-2.5.0/flavio/physics/ddecays/formfactors/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/test_dlnu.py` & `flavio-2.5.0/flavio/physics/ddecays/test_dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/ddecays/test_dplnu.py` & `flavio-2.5.0/flavio/physics/ddecays/test_dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/edms/common.py` & `flavio-2.5.0/flavio/physics/edms/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/edms/neutronedm.py` & `flavio-2.5.0/flavio/physics/edms/neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/edms/paraedm.py` & `flavio-2.5.0/flavio/physics/edms/paraedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/edms/test_neutronedm.py` & `flavio-2.5.0/flavio/physics/edms/test_neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/eft.py` & `flavio-2.5.0/flavio/physics/eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/elements.py` & `flavio-2.5.0/flavio/physics/elements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/higgs/decay.py` & `flavio-2.5.0/flavio/physics/higgs/decay.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/higgs/production.py` & `flavio-2.5.0/flavio/physics/higgs/production.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/higgs/signalstrength.py` & `flavio-2.5.0/flavio/physics/higgs/signalstrength.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/higgs/test_higgs.py` & `flavio-2.5.0/flavio/physics/higgs/test_higgs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/higgs/width.py` & `flavio-2.5.0/flavio/physics/higgs/width.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/formfactors.py` & `flavio-2.5.0/flavio/physics/kdecays/formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/kll.py` & `flavio-2.5.0/flavio/physics/kdecays/kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/klnu.py` & `flavio-2.5.0/flavio/physics/kdecays/klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/kpilnu.py` & `flavio-2.5.0/flavio/physics/kdecays/kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/kpinunu.py` & `flavio-2.5.0/flavio/physics/kdecays/kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/kpipi.py` & `flavio-2.5.0/flavio/physics/kdecays/kpipi.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/lambdaplnu.py` & `flavio-2.5.0/flavio/physics/kdecays/lambdaplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/test_formfactors.py` & `flavio-2.5.0/flavio/physics/kdecays/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/test_kll.py` & `flavio-2.5.0/flavio/physics/kdecays/test_kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/test_klnu.py` & `flavio-2.5.0/flavio/physics/kdecays/test_klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/test_kpilnu.py` & `flavio-2.5.0/flavio/physics/kdecays/test_kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/test_kpinunu.py` & `flavio-2.5.0/flavio/physics/kdecays/test_kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/kdecays/wilsoncoefficients.py` & `flavio-2.5.0/flavio/physics/kdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mdms/al.py` & `flavio-2.5.0/flavio/physics/mdms/al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mdms/test_al.py` & `flavio-2.5.0/flavio/physics/mdms/test_al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mesonmixing/amplitude.py` & `flavio-2.5.0/flavio/physics/mesonmixing/amplitude.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mesonmixing/common.py` & `flavio-2.5.0/flavio/physics/mesonmixing/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mesonmixing/observables.py` & `flavio-2.5.0/flavio/physics/mesonmixing/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mesonmixing/test_mesonmixing.py` & `flavio-2.5.0/flavio/physics/mesonmixing/test_mesonmixing.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mesonmixing/wilsoncoefficient.py` & `flavio-2.5.0/flavio/physics/mesonmixing/wilsoncoefficient.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mudecays/mu3e.py` & `flavio-2.5.0/flavio/physics/mudecays/mu3e.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mudecays/mueconversion.py` & `flavio-2.5.0/flavio/physics/mudecays/mueconversion.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mudecays/muegamma.py` & `flavio-2.5.0/flavio/physics/mudecays/muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/mudecays/test_muegamma.py` & `flavio-2.5.0/flavio/physics/mudecays/test_muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/neutrinos/test_trident.py` & `flavio-2.5.0/flavio/physics/neutrinos/test_trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/neutrinos/trident.py` & `flavio-2.5.0/flavio/physics/neutrinos/trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/running/betafunctions.py` & `flavio-2.5.0/flavio/physics/running/betafunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/running/masses.py` & `flavio-2.5.0/flavio/physics/running/masses.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/running/running.py` & `flavio-2.5.0/flavio/physics/running/running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/running/test_running.py` & `flavio-2.5.0/flavio/physics/running/test_running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/scattering/ee_ww.py` & `flavio-2.5.0/flavio/physics/scattering/ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/scattering/test_ee_ww.py` & `flavio-2.5.0/flavio/physics/scattering/test_ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/common.py` & `flavio-2.5.0/flavio/physics/taudecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/tau3l.py` & `flavio-2.5.0/flavio/physics/taudecays/tau3l.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/taulgamma.py` & `flavio-2.5.0/flavio/physics/taudecays/taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/taulnunu.py` & `flavio-2.5.0/flavio/physics/taudecays/taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/taupl.py` & `flavio-2.5.0/flavio/physics/taudecays/taupl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/taupnu.py` & `flavio-2.5.0/flavio/physics/taudecays/taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/tauvl.py` & `flavio-2.5.0/flavio/physics/taudecays/tauvl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/test_taulgamma.py` & `flavio-2.5.0/flavio/physics/taudecays/test_taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/test_taulnunu.py` & `flavio-2.5.0/flavio/physics/taudecays/test_taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/taudecays/test_taupnu.py` & `flavio-2.5.0/flavio/physics/taudecays/test_taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/test_ckm.py` & `flavio-2.5.0/flavio/physics/test_ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/test_common.py` & `flavio-2.5.0/flavio/physics/test_common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/test_eft.py` & `flavio-2.5.0/flavio/physics/test_eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/units.py` & `flavio-2.5.0/flavio/physics/units.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/wdecays/gammaw.py` & `flavio-2.5.0/flavio/physics/wdecays/gammaw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/wdecays/mw.py` & `flavio-2.5.0/flavio/physics/wdecays/mw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/wdecays/test_mW.py` & `flavio-2.5.0/flavio/physics/wdecays/test_mW.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/wdecays/test_wdecays.py` & `flavio-2.5.0/flavio/physics/wdecays/test_wdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/zdecays/afbz.py` & `flavio-2.5.0/flavio/physics/zdecays/afbz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/zdecays/gammaz.py` & `flavio-2.5.0/flavio/physics/zdecays/gammaz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/zdecays/gammazsm.py` & `flavio-2.5.0/flavio/physics/zdecays/gammazsm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/zdecays/smeftew.py` & `flavio-2.5.0/flavio/physics/zdecays/smeftew.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/physics/zdecays/test_zdecays.py` & `flavio-2.5.0/flavio/physics/zdecays/test_zdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/plots/__init__.py` & `flavio-2.5.0/flavio/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/plots/colors.py` & `flavio-2.5.0/flavio/plots/colors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/plots/plotfunctions.py` & `flavio-2.5.0/flavio/plots/plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/plots/test_plotfunctions.py` & `flavio-2.5.0/flavio/plots/test_plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/statistics/functions.py` & `flavio-2.5.0/flavio/statistics/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/statistics/likelihood.py` & `flavio-2.5.0/flavio/statistics/likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/statistics/probability.py` & `flavio-2.5.0/flavio/statistics/probability.py`

 * *Files 10% similar despite different names*

```diff
@@ -175,14 +175,62 @@
         return confidence_level(nsigma) * self.half_range
 
     def get_error_right(self, nsigma=1, **kwargs):
         """Return the upper error"""
         return confidence_level(nsigma) * self.half_range
 
 
+class DiscreteUniformDistribution(ProbabilityDistribution):
+    """Distribution with a finite number of integer values having equal probability"""
+
+    def __init__(self, lowest_value, highest_value, central_value=None):
+        """Initialize the distribution.
+
+        Parameters:
+
+        - lowest_value: lowest integer value `a`
+        - highest_value: highest integer value `b`
+        - central_value (optional): integer within [a,b]. Default is int((a+b)/2)
+        """
+        if central_value and (
+            central_value > highest_value
+            or central_value < lowest_value
+        ):
+            raise ValueError('`central_value` must in the interval [`lowest_value`, `highest_value`].')
+        central_value = int((lowest_value+highest_value)/2) if central_value is None else int(central_value)
+        self.lowest_value = int(lowest_value)
+        self.highest_value = int(highest_value)
+        self.range = np.arange(self.lowest_value,self.highest_value+1)
+        super().__init__(central_value, support=(self.lowest_value, self.highest_value))
+
+    def __repr__(self):
+        return (
+            'flavio.statistics.probability.DiscreteUniformDistribution'
+            f'({self.support[0]}, {self.support[1]}, {self.central_value})'
+        )
+
+    def get_random(self, size=None):
+        return np.random.randint(self.support[0], self.support[1]+1, size=size)
+
+    def _logpdf(self, x):
+        if x in self.range:
+            return -np.log(len(self.range))
+        else:
+            return -np.inf
+
+    def logpdf(self, x):
+        _lpvect = np.vectorize(self._logpdf)
+        return _lpvect(x)
+
+    def get_error_left(self, *args, **kwargs):
+        return 0
+
+    def get_error_right(self, *args, **kwargs):
+        return 0
+
 
 class DeltaDistribution(ProbabilityDistribution):
     """Delta Distrubution that is non-vanishing only at a single point."""
 
     def __init__(self, central_value):
         """Initialize the distribution.
 
@@ -538,17 +586,18 @@
     def __init__(self, a, loc, scale):
         if loc > 0:
             raise ValueError("loc must be negative or zero")
         # "frozen" scipy distribution object
         self.scipy_dist = scipy.stats.gamma(a=a, loc=loc, scale=scale)
         mode = loc + (a-1)*scale
         # support extends until the CDF is roughly "6 sigma"
-        support_limit = self.scipy_dist.ppf(1-2e-9)
+        support_min = min(self.scipy_dist.ppf(1e-9), mode)
+        support_max = self.scipy_dist.ppf(1-1e-9)
         super().__init__(central_value=mode, # the mode
-                         support=(loc, support_limit))
+                         support=(support_min, support_max))
         self.a = a
         self.loc = loc
         self.scale = scale
 
     def __repr__(self):
         return 'flavio.statistics.probability.GammaDistribution' + \
                '({}, {}, {})'.format(self.a, self.loc, self.scale)
@@ -602,17 +651,18 @@
             raise ValueError("loc must be negative or zero")
         # "frozen" scipy distribution object (without restricting x>0!)
         self.scipy_dist = scipy.stats.gamma(a=a, loc=loc, scale=scale)
         mode = loc + (a-1)*scale
         if mode < 0:
             mode = 0
         # support extends until the CDF is roughly "6 sigma", assuming x>0
-        support_limit = self.scipy_dist.ppf(1-2e-9*(1-self.scipy_dist.cdf(0)))
+        support_min = max(min(self.scipy_dist.ppf(1e-9), mode), 0)
+        support_max = self.scipy_dist.ppf(1-1e-9*(1-self.scipy_dist.cdf(0)))
         super().__init__(central_value=mode, # the mode
-                         support=(0, support_limit))
+                         support=(support_min, support_max))
         self.a = a
         self.loc = loc
         self.scale = scale
         # scale factor for PDF to account for x>0
         self._pdf_scale = 1/(1 - self.scipy_dist.cdf(0))
 
     def __repr__(self):
@@ -684,67 +734,132 @@
             # is smaller than the PDF at the boundary of this range, return the
             # boundary of the range as the right-hand error
             return one_sided_error
         else:
             a = self._find_error_cdf(confidence_level(nsigma))
             return self.ppf(a + confidence_level(nsigma)) - self.central_value
 
-class GammaUpperLimit(GammaDistributionPositive):
+class GammaCountingProcess(GammaDistributionPositive):
+    r"""Gamma distribution with x restricted to be positive appropriate for
+    a positive quantitity obtained from a low-statistics counting experiment,
+    e.g. a rare decay rate, given in terms of event counts and a scale factor.
+    The diference to `GammaUpperLimit` is that the scale factor has to be given
+    directly and is not expressed in terms of an upper limit.
+    """
+    def __init__(self, *,
+                 scale_factor=1,
+                 counts_total=None,
+                 counts_background=None,
+                 counts_signal=None):
+        r"""Initialize the distribution.
+
+        Parameters:
+
+        - `scale_factor`: scale factor by which the number of counts is multiplied
+          to get the observable of interest.
+        - `counts_total`: observed total number (signal and background) of counts.
+        - `counts_background`: expected mean number of expected background counts
+        - `counts_signal`: mean observed number of signal events
+
+        Of the three parameters `counts_total`, `counts_background`, and
+        `counts_signal`, only two must be specified. The third one will
+        be determined from the relation
+
+        `counts_total = counts_signal + counts_background`
+        """
+        if scale_factor <= 0:
+            raise ValueError("Scale factor should be positive")
+        self.scale_factor = scale_factor
+        if counts_total is not None and counts_total < 0:
+            raise ValueError("counts_total should be a positive number, zero, or None")
+        if counts_background is not None and counts_background < 0:
+            raise ValueError("counts_background should be a positive number, zero, or None")
+        if [counts_total, counts_signal, counts_background].count(None) == 0:
+            # if all three are specified, check the relation holds!
+            if abs((counts_total - counts_background - counts_signal)/(counts_total if counts_total != 0 else 1)) > 1e-15:
+                raise ValueError("The relation `counts_total = counts_signal + counts_background` is not satisfied")
+        if [counts_total, counts_signal, counts_background].count(None) > 1:
+            raise ValueError("Of the three parameters `counts_total`, `counts_background`, and `counts_signal`, two must be specified")
+        if counts_background is None:
+            self.counts_background = counts_total - counts_signal
+        else:
+            self.counts_background = counts_background
+        if counts_signal is None:
+            self.counts_signal = counts_total - counts_background
+        else:
+            self.counts_signal = counts_signal
+        if counts_total is None:
+            self.counts_total = counts_signal + counts_background
+        else:
+            self.counts_total = counts_total
+        super().__init__(
+            a = self.counts_total + 1,
+            loc = -self.counts_background * self.scale_factor,
+            scale = self.scale_factor
+        )
+
+    def __repr__(self):
+        return ('flavio.statistics.probability.GammaCountingProcess'
+                '(scale_factor={}, counts_total={}, counts_signal={})').format(
+                    self.scale_factor,
+                    self.counts_total,
+                    self.counts_signal
+                )
+
+class GammaUpperLimit(GammaCountingProcess):
     r"""Gamma distribution with x restricted to be positive appropriate for
     a positive quantitity obtained from a low-statistics counting experiment,
-    e.g. a rare decay rate, given an upper limit on x."""
+    e.g. a rare decay rate, given an upper limit on x.
+    The diference to `GammaCountingProcess` is that a scale factor is determined
+    from the upper limit and not specified directly."""
 
-    def __init__(self, counts_total, counts_background, limit, confidence_level):
+    def __init__(self, *,
+                 limit, confidence_level,
+                 counts_total=None,
+                 counts_background=None,
+                 counts_signal=None):
         r"""Initialize the distribution.
 
         Parameters:
 
-        - counts_total: observed total number (signal and background) of counts.
-        - counts_background: number of expected background counts, assumed to be
-          known.
         - limit: upper limit on x, which is proportional (with a positive
           proportionality factor) to the number of signal events.
         - confidence_level: confidence level of the upper limit, i.e. the value
           of the CDF at the limit. Float between 0 and 1. Frequently used values
           are 0.90 and 0.95.
+        - `counts_total`: observed total number (signal and background) of counts.
+        - `counts_background`: expected mean number of expected background counts
+        - `counts_signal`: mean observed number of signal events
         """
         if confidence_level > 1 or confidence_level < 0:
             raise ValueError("Confidence level should be between 0 und 1")
         if limit <= 0:
             raise ValueError("The upper limit should be a positive number")
-        if counts_total < 0:
-            raise ValueError("counts_total should be a positive number or zero")
-        if counts_background < 0:
-            raise ValueError("counts_background should be a positive number or zero")
         self.limit = limit
         self.confidence_level = confidence_level
-        self.counts_total = counts_total
-        self.counts_background = counts_background
-        a, loc, scale = self._get_a_loc_scale()
-        super().__init__(a=a, loc=loc, scale=scale)
-
+        dist_unscaled = GammaCountingProcess(
+                 scale_factor=1,
+                 counts_total=counts_total,
+                 counts_background=counts_background,
+                 counts_signal=counts_signal)
+        limit_unscaled = dist_unscaled.ppf(self.confidence_level)
+        # use the value of the limit to determine the scale factor
+        scale_factor = self.limit / limit_unscaled
+        super().__init__(
+            scale_factor=scale_factor,
+            counts_total=counts_total,
+            counts_background=counts_background)
 
     def __repr__(self):
-        return 'flavio.statistics.probability.GammaUpperLimit' + \
-               '({}, {}, {}, {})'.format(self.counts_total,
-                                         self.counts_background,
-                                         self.limit,
-                                         self.confidence_level)
-
-    def _get_a_loc_scale(self):
-        """Convert the counts and limit to the input parameters needed for
-        GammaDistributionPositive"""
-        a = self.counts_total + 1
-        loc_unscaled = -self.counts_background
-        dist_unscaled = GammaDistributionPositive(a=a, loc=loc_unscaled, scale=1)
-        limit_unscaled = dist_unscaled.ppf(self.confidence_level)
-        # rescale
-        scale = self.limit/limit_unscaled
-        loc = -self.counts_background*scale
-        return a, loc, scale
+        return ('flavio.statistics.probability.GammaUpperLimit'
+                '(limit={}, confidence_level={}, counts_total={}, counts_background={})'
+               ).format(self.limit,
+                        self.confidence_level,
+                        self.counts_total,
+                        self.counts_background)
 
 class NumericalDistribution(ProbabilityDistribution):
     """Univariate distribution defined in terms of numerical values for the
     PDF."""
 
     def __init__(self, x, y, central_value=None):
         """Initialize a 1D numerical distribution.
@@ -877,204 +992,271 @@
     def from_pd(cls, pd, nsteps=1000):
         if isinstance(pd, NumericalDistribution):
             return pd
         _x = np.linspace(pd.support[0], pd.support[-1], nsteps)
         _y = np.exp(pd.logpdf(_x))
         return cls(central_value=pd.central_value, x=_x, y=_y)
 
-
 class GeneralGammaDistributionPositive(NumericalDistribution):
-    r"""Distribution appropriate for
-    a positive quantitity obtained from a low-statistics counting experiment,
-    e.g. a rare decay rate.
-    The difference to `GammaUpperLimit` is that this class also allows to
+    r"""Distribution appropriate for cases in which a strictly positive quantity
+    described by a Gamma distribution has an additional Gaussian uncertainty, which
+    is specified by a Gaussian standard deviation. The result is a numerical
+    distribution obtained from the convolution of a normal distribution
+    (with the Gaussian standard deviation) and a gamma distribution, restricted to
+    positive values. Note that the convolution is done before applying the scale factor
+    """
+
+    def __init__(self, *, a, loc, scale, gaussian_standard_deviation):
+        r"""Initialize the distribution.
+
+        The parameters `a`, `loc`, and `scale` are the same as in `GammaDistributionPositive`.
+        The parameter `gaussian_standard_deviation` defines a normal distribution that
+        is convoluted with the gamma distribution. Note that the convolution is performed
+        before the `scale` factor is applied.
+
+        If `gaussian_standard_deviation=0`, it makes more sense to use
+        `GammaDistributionPositive`, which is equivalent but analytical rather than
+        numerical.
+        """
+        if loc > 0:
+            raise ValueError("loc must be negative or zero")
+        self.a = a
+        self.loc = loc
+        self.scale = scale
+        self.gaussian_standard_deviation = gaussian_standard_deviation
+        x, y = self._get_xy()
+        if self.gaussian_standard_deviation/np.sqrt(self.counts_total+1) < 1/100:
+            self.gaussian_standard_deviation = 0
+            warnings.warn("For vanishing or very small Gaussian standard deviation, "
+                          "it is safer to use GammaDistributionPositive instead of "
+                          "GeneralGammaDistributionPositive to avoid numerical "
+                          "instability.")
+        super().__init__(x=x, y=y)
+
+    def __repr__(self):
+        return ('flavio.statistics.probability.GeneralGammaDistributionPositive'
+               '(a={}, loc={}, scale={}, gaussian_standard_deviation={})'.format(
+                    self.a,
+                    self.loc,
+                    self.scale,
+                    self.gaussian_standard_deviation
+                ))
+
+    def _get_xy(self):
+        loc_scaled = self.loc/self.scale
+        if self.gaussian_standard_deviation == 0:
+            # this is a bit pointless as in this case it makes more
+            # sense to use GammaDistributionPositive itself
+            gamma_unscaled = GammaDistributionPositive(a = self.a,
+                                                       loc = loc_scaled,
+                                                       scale = 1)
+            num_unscaled = NumericalDistribution.from_pd(gamma_unscaled)
+        else:
+            # define a gamma distribution (with x>loc, not x>0!) and convolve
+            # it with a Gaussian
+            gamma_unscaled = GammaDistribution(a = self.a,
+                                               loc = loc_scaled,
+                                               scale = 1)
+            norm_bg = NormalDistribution(0, self.gaussian_standard_deviation)
+            num_unscaled = convolve_distributions([gamma_unscaled, norm_bg], central_values='sum')
+        # now that we have convolved, add the mirrored values from below x=loc and
+        # then cut off anything below x=0
+        x = num_unscaled.x
+        y = num_unscaled.y_norm
+        if loc_scaled in x:
+            to_mirror = y[x<=loc_scaled][::-1]
+            y_pos = y[len(to_mirror)-1:len(to_mirror)*2-1]
+            y[len(to_mirror)-1:len(to_mirror)*2-1] += to_mirror[:len(y_pos)]
+        else:
+            to_mirror = y[x<loc_scaled][::-1]
+            y_pos = y[len(to_mirror):len(to_mirror)*2]
+            y[len(to_mirror):len(to_mirror)*2] += to_mirror[:len(y_pos)]
+        y = y[x >= 0]
+        x = x[x >= 0]
+        if x[0] != 0:  #  make sure the PDF at 0 exists
+            x = np.insert(x, 0, 0.)  # add 0 as first element
+            y = np.insert(y, 0, y[0])  # copy first element
+        x = x * self.scale
+        return x, y
+
+class GeneralGammaCountingProcess(GeneralGammaDistributionPositive):
+    r"""Distribution appropriate for a positive quantitity obtained from a
+    low-statistics counting experiment, e.g. a rare decay rate.
+    The difference to `GammaCountingProcess` is that this class also allows to
     specify an uncertainty on the number of background events. The result
     is a numerical distribution obtained from the convolution of a normal
     distribution (for the background uncertainty) and a gamma distribution,
     restricted to positive values.
-    In contrast to `GammaUpperLimit`, the scale factor (the relational between
-    the observable of interest and the raw number of counts) is not determined
-    from a limit and a confidence level, but specified explicitly.
-    For the case of a limit, see `GeneralGammaUpperLimit`.
+    In contrast to `GeneralGammaUpperLimit`, the scale factor (the relational
+    between the observable of interest and the raw number of counts) is not
+    determined from a limit and a confidence level, but specified explicitly.
     """
 
-    def __init__(self,
+    def __init__(self, *,
                  scale_factor=1,
                  counts_total=None,
                  counts_background=None,
                  counts_signal=None,
-                 background_variance=0):
+                 background_std=0):
         r"""Initialize the distribution.
 
         Parameters:
 
-        Parameters:
-
         - `scale_factor`: scale factor by which the number of counts is multiplied
           to get the observable of interest.
         - `counts_total`: observed total number (signal and background) of counts.
         - `counts_background`: expected mean number of expected background counts
-        - `counts_signal`: mean obseved number of signal events
-        - `background_variance`: standard deviation of the expected number of
+        - `counts_signal`: mean observed number of signal events
+        - `background_std`: standard deviation of the expected number of
           background events
 
         Of the three parameters `counts_total`, `counts_background`, and
         `counts_signal`, only two must be specified. The third one will
         be determined from the relation
 
         `counts_total = counts_signal + counts_background`
 
         Note that if `background_variance=0`, it makes more sense to use
-        `GammaUpperLimit`, which is equivalent but analytical rather than
+        `GammaCountingProcess`, which is equivalent but analytical rather than
         numerical.
         """
         if scale_factor <= 0:
             raise ValueError("Scale factor should be positive")
         self.scale_factor = scale_factor
         if counts_total is not None and counts_total < 0:
             raise ValueError("counts_total should be a positive number, zero, or None")
-        if counts_background is not None and counts_background <= 0:
-            raise ValueError("counts_background should be a positive number or None")
-        if background_variance < 0:
-            raise ValueError("background_variance should be a positive number")
+        if counts_background is not None and counts_background < 0:
+            raise ValueError("counts_background should be a positive number, zero, or None")
+        if background_std < 0:
+            raise ValueError("background_std should be a positive number")
         if [counts_total, counts_signal, counts_background].count(None) == 0:
             # if all three are specified, check the relation holds!
             if abs((counts_total - counts_background - counts_signal)/(counts_total if counts_total != 0 else 1)) > 1e-15:
                 raise ValueError("The relation `counts_total = counts_signal + counts_background` is not satisfied")
+        if [counts_total, counts_signal, counts_background].count(None) > 1:
+            raise ValueError("Of the three parameters `counts_total`, `counts_background`, and `counts_signal`, two must be specified")
         if counts_background is None:
             self.counts_background = counts_total - counts_signal
         else:
             self.counts_background = counts_background
         if counts_signal is None:
             self.counts_signal = counts_total - counts_background
         else:
             self.counts_signal = counts_signal
         if counts_total is None:
             self.counts_total = counts_signal + counts_background
         else:
             self.counts_total = counts_total
-        self.background_variance = background_variance
-        x, y = self._get_xy()
-        if self.counts_total != 0 and self.background_variance/self.counts_total <= 1/100.:
-            warnings.warn("For vanishing or very small background variance, "
-                          "it is safer to use GammaUpperLimit instead of "
-                          "GeneralGammaUpperLimit to avoid numerical "
-                          "instability.")
-        super().__init__(x=x, y=y)
+        self.background_std = background_std
+        if self.background_std/np.sqrt(self.counts_total+1) < 1/100:
+            self.background_std = 0
+            warnings.warn("For vanishing or very small background standard "
+                          "deviation, it is safer to use GammaCountingProcess "
+                          "instead of GeneralGammaCountingProcess to avoid "
+                          "numerical instability.")
+        super().__init__(
+            a = self.counts_total + 1,
+            loc = -self.counts_background * self.scale_factor,
+            scale = self.scale_factor,
+            gaussian_standard_deviation = background_std
+        )
 
     def __repr__(self):
-        return ('flavio.statistics.probability.GeneralGammaDistributionPositive'
-               '({}, counts_total={}, counts_signal={}, '
-               'background_variance={})').format(self.scale_factor,
+        return ('flavio.statistics.probability.GeneralGammaCountingProcess'
+               '(scale_factor={}, counts_total={}, counts_signal={}, '
+               'background_std={})').format(self.scale_factor,
                                                 self.counts_total,
                                                 self.counts_signal,
-                                                self.background_variance)
+                                                self.background_std)
 
-    def _get_xy(self):
-        if self.background_variance == 0:
-            # this is a bit pointless as in this case it makes more
-            # sense to use GammaUpperLimit itself
-            gamma_unscaled = GammaDistributionPositive(a = self.counts_total + 1,
-                                                       loc = -self.counts_background,
-                                                       scale = 1)
-            num_unscaled = NumericalDistribution.from_pd(gamma_unscaled)
-        else:
-            # define a gamma distribution (with x>loc, not x>0!) and convolve
-            # it with a Gaussian
-            gamma_unscaled = GammaDistribution(a = self.counts_total + 1,
-                                               loc = -self.counts_background,
-                                               scale = 1)
-            norm_bg = NormalDistribution(0, self.background_variance)
-            num_unscaled = convolve_distributions([gamma_unscaled, norm_bg], central_values='sum')
-        # now that we have convolved, cut off anything below x=0
-        x = num_unscaled.x
-        y = num_unscaled.y_norm
-        y = y[np.where(x >= 0)]
-        x = x[np.where(x >= 0)]
-        if x[0] != 0:  #  make sure the PDF at 0 exists
-            x = np.insert(x, 0, 0.)  # add 0 as first element
-            y = np.insert(y, 0, y[0])  # copy first element
-        y[0]
-        num_unscaled = NumericalDistribution(x, y)
-        x = x * self.scale_factor
-        return x, y
 
-
-class GeneralGammaUpperLimit(GeneralGammaDistributionPositive):
+class GeneralGammaUpperLimit(GeneralGammaCountingProcess):
     r"""Distribution appropriate for
     a positive quantitity obtained from a low-statistics counting experiment,
     e.g. a rare decay rate, given an upper limit on x.
     The difference to `GammaUpperLimit` is that this class also allows to
     specify an uncertainty on the number of background events. The result
     is a numerical distribution obtained from the convolution of a normal
     distribution (for the background uncertainty) and a gamma distribution,
     restricted to positive values.
     The only difference to `GeneralGammaDistributionPositive` is that the scale
     factor is determined from the limit and confidence level.
     """
 
-    def __init__(self,
+    def __init__(self, *,
                  limit, confidence_level,
                  counts_total=None,
                  counts_background=None,
                  counts_signal=None,
-                 background_variance=0):
+                 background_std=None,
+                 background_variance=None):
         r"""Initialize the distribution.
 
         Parameters:
 
         Parameters:
 
         - `limit`: upper limit on x, which is proportional (with a positive
           proportionality factor) to the number of signal events.
         - `confidence_level`: confidence level of the upper limit, i.e. the value
           of the CDF at the limit. Float between 0 and 1. Frequently used values
           are 0.90 and 0.95.
         - `counts_total`: observed total number (signal and background) of counts.
         - `counts_background`: expected mean number of expected background counts
-        - `counts_signal`: mean obseved number of signal events
-        - `background_variance`: standard deviation of the expected number of
+        - `counts_signal`: mean observed number of signal events
+        - `background_std`: standard deviation of the expected number of
           background events
+        - `background_variance`: alias of `background_std` for backward
+          compatibility
 
         Of the three parameters `counts_total`, `counts_background`, and
         `counts_signal`, only two must be specified. The third one will
         be determined from the relation
 
         `counts_total = counts_signal + counts_background`
 
-        Note that if `background_variance=0`, it makes more sense to use
+        Note that if `background_std=0`, it makes more sense to use
         `GammaUpperLimit`, which is equivalent but analytical rather than
         numerical.
         """
+        if background_variance is not None:
+            warnings.warn(f'The argument `background_variance` is deprecated. Use `background_std` instead.', DeprecationWarning, stacklevel=2)
+            if background_std is not None and background_std != background_variance:
+                raise ValueError('Setting `background_std` and its alias `background_variance` to different values is inconsistent.')
+            else:
+                background_std = background_variance
+        elif background_std is None:
+            background_std = 0
+        self.background_variance = background_std
         self.limit = limit
         self.confidence_level = confidence_level
-        _d_unscaled = GeneralGammaDistributionPositive(
+        _d_unscaled = GeneralGammaCountingProcess(
             scale_factor=1,
             counts_total=counts_total,
             counts_background=counts_background,
             counts_signal=counts_signal,
-            background_variance=background_variance)
+            background_std=background_std)
         limit_unscaled = _d_unscaled.ppf(self.confidence_level)
         # use the value of the limit to determine the scale factor
         scale_factor = self.limit / limit_unscaled
         super().__init__(
             scale_factor=scale_factor,
             counts_total=counts_total,
             counts_background=counts_background,
             counts_signal=counts_signal,
-            background_variance=background_variance)
+            background_std=background_std)
 
     def __repr__(self):
         return ('flavio.statistics.probability.GeneralGammaUpperLimit'
-               '({}, {}, counts_total={}, counts_signal={}, '
-               'background_variance={})').format(self.limit,
+               '(limit={}, confidence_level={}, counts_total={}, counts_background={}, '
+               'background_std={})').format(self.limit,
                                                 self.confidence_level,
                                                 self.counts_total,
-                                                self.counts_signal,
-                                                self.background_variance)
+                                                self.counts_background,
+                                                self.background_std)
 
 
 class KernelDensityEstimate(NumericalDistribution):
     """Univariate kernel density estimate.
 
     Parameters:
```

### Comparing `flavio-2.4.0/flavio/statistics/test_functions.py` & `flavio-2.5.0/flavio/statistics/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/statistics/test_likelihood.py` & `flavio-2.5.0/flavio/statistics/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/statistics/test_probability.py` & `flavio-2.5.0/flavio/statistics/test_probability.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     def test_gamma(self):
         # check for loc above and below a-1
         for  loc in (-5, -15):
             p = GammaDistribution(a=11, loc=loc, scale=1)
             self.assertEqual(p.central_value, loc + 10)
             r = p.get_random(10)
             self.assertEqual(len(r), 10)
-            self.assertAlmostEqual(p.cdf(p.support[1]), 1-2e-9, delta=0.1e-9)
-            self.assertAlmostEqual(p.ppf(1-2e-9), p.support[1], delta=0.0001)
-            self.assertEqual(loc, p.support[0])
+            self.assertAlmostEqual(p.cdf(p.support[1]), 1-1e-9, delta=0.1e-9)
+            self.assertAlmostEqual(p.ppf(1-1e-9), p.support[1], delta=0.0001)
+            self.assertEqual(p.scipy_dist.ppf(1e-9), p.support[0])
         # nearly normal distribution
         p = GammaDistribution(a=10001, loc=0, scale=1)
         self.assertAlmostEqual(p.error_left, sqrt(10000), delta=1)
         self.assertAlmostEqual(p.get_error_left(nsigma=2), 2*sqrt(10000), delta=2)
         self.assertAlmostEqual(p.error_right, sqrt(10000), delta=1)
         self.assertAlmostEqual(p.get_error_right(nsigma=2), 2*sqrt(10000), delta=2)
 
@@ -87,17 +87,17 @@
             p = GammaDistributionPositive(a=11, loc=loc, scale=1)
             self.assertEqual(p.central_value, max(loc + 10, 0))
             r = p.get_random(10)
             self.assertEqual(len(r), 10)
             self.assertTrue(np.min(r) >= 0)
             self.assertEqual(p.logpdf(-0.1), -np.inf)
             self.assertEqual(p.cdf(0), 0)
-            self.assertAlmostEqual(p.cdf(p.support[1]), 1-2e-9, delta=0.1e-9)
+            self.assertAlmostEqual(p.cdf(p.support[1]), 1-1e-9, delta=0.1e-9)
             self.assertAlmostEqual(p.ppf(0), 0, places=14)
-            self.assertAlmostEqual(p.ppf(1-2e-9), p.support[1], delta=0.0001)
+            self.assertAlmostEqual(p.ppf(1-1e-9), p.support[1], delta=0.0001)
             self.assertEqual(p.cdf(-1), 0)
         p = GammaDistributionPositive(a=11, loc=-9, scale=1)
         self.assertEqual(p.central_value, 1)
         self.assertEqual(p.error_left, 1)
         # nearly normal distribution
         p = GammaDistributionPositive(a=10001, loc=0, scale=1)
         self.assertAlmostEqual(p.error_left, sqrt(10000), delta=1)
@@ -123,34 +123,53 @@
         # check that large-statistics Gamma and Gauss give nearly same PDF
         for x in [0, 1, 2, 3, 4]:
             self.assertAlmostEqual(p.logpdf(x), p_norm.logpdf(x), delta=0.1)
 
     def test_general_gamma_limit(self):
         p = GeneralGammaUpperLimit(counts_total=30, counts_background=10,
                             limit=2e-5, confidence_level=0.68,
-                            background_variance=5)
+                            background_std=5)
         self.assertAlmostEqual(p.cdf(2e-5), 0.68, delta=0.0001)
         # background excess
         p = GeneralGammaUpperLimit(counts_total=30, counts_background=50,
                             limit=2e5, confidence_level=0.68,
-                            background_variance=25)
+                            background_std=25)
         self.assertAlmostEqual(p.cdf(2e5), 0.68, delta=0.0001)
         p = GeneralGammaUpperLimit(counts_total=10000, counts_background=10000,
                             limit=3., confidence_level=0.95,
-                            background_variance=1000)
+                            background_std=1000)
         p_norm = GaussianUpperLimit(limit=3., confidence_level=0.95)
         # check that large-statistics Gamma and Gauss give nearly same PDF
         for x in [1, 2, 3, 4]:
             self.assertAlmostEqual(p.logpdf(x), p_norm.logpdf(x), delta=0.1)
         # check that warning is raised for very small background variance
         with self.assertWarns(Warning):
             GeneralGammaUpperLimit(counts_total=10000, counts_background=10000,
                             limit=3., confidence_level=0.95,
-                            background_variance=10)
+                            background_std=1)
 
+    def test_counting_process(self):
+        # check that GeneralGammaCountingProcess with background_std set to 0
+        # gives the same pdf as GammaCountingProcess
+        for counts_total in [100, 200, 300]:
+            for counts_background in [25, 50, 100]:
+                for scale_factor in [1, 2, 3]:
+                    p_gcp = GammaCountingProcess(scale_factor=scale_factor,
+                                                 counts_total=counts_total,
+                                                 counts_background=counts_background)
+                    p_ggcp = GeneralGammaCountingProcess(scale_factor=scale_factor,
+                                                         counts_total=counts_total,
+                                                         counts_background=counts_background,
+                                                         background_std=0)
+                    for x in np.linspace(0, 1000, 500):
+                        pdf_gcp = np.exp(p_gcp.logpdf(x))
+                        pdf_ggcp = p_ggcp.pdf(x)
+                        if pdf_gcp > 1e-5 and pdf_ggcp > 1e-5:
+                            err = np.abs((pdf_gcp - pdf_ggcp)/pdf_gcp)
+                            self.assertLess(err, 1e-3, msg=f'x={x}, pdf_gcp={pdf_gcp}, pdf_ggcp={pdf_ggcp}')
 
     def test_numerical(self):
         x = np.arange(-5,7,0.01)
         y = scipy.stats.norm.pdf(x, loc=1)
         y_crazy = 14.7 * y # multiply PDF by crazy number
         p_num = NumericalDistribution(x, y_crazy)
         p_norm = NormalDistribution(1, 1)
@@ -463,18 +482,18 @@
                          fsp + 'UniformDistribution(1, 2)')
         self.assertEqual(repr(GaussianUpperLimit(1e-9, 0.95)),
                          fsp + 'GaussianUpperLimit(1e-09, 0.95)')
         self.assertEqual(repr(GammaDistribution(5, -2, 1.5)),
                          fsp + 'GammaDistribution(5, -2, 1.5)')
         self.assertEqual(repr(GammaDistributionPositive(5, -2, 1.5)),
                          fsp + 'GammaDistributionPositive(5, -2, 1.5)')
-        self.assertEqual(repr(GammaUpperLimit(15, 10, 1e-9, 0.95)),
-                         fsp + 'GammaUpperLimit(15, 10, 1e-09, 0.95)')
-        self.assertEqual(repr(GeneralGammaUpperLimit(1e-9, 0.95, counts_total=15, counts_background=10, background_variance=0.2)),
-                         fsp + 'GeneralGammaUpperLimit(1e-09, 0.95, counts_total=15, counts_signal=5, background_variance=0.2)')
+        self.assertEqual(repr(GammaUpperLimit(limit=1e-9, confidence_level=0.95, counts_total=15, counts_background=10)),
+                         fsp + 'GammaUpperLimit(limit=1e-09, confidence_level=0.95, counts_total=15, counts_background=10)')
+        self.assertEqual(repr(GeneralGammaUpperLimit(limit=1e-9, confidence_level=0.95, counts_total=15, counts_background=10, background_std=0.2)),
+                         fsp + 'GeneralGammaUpperLimit(limit=1e-09, confidence_level=0.95, counts_total=15, counts_background=10, background_std=0.2)')
         self.assertEqual(repr(MultivariateNormalDistribution([1., 2], [[2, 0.1], [0.1, 2]])),
                          fsp + 'MultivariateNormalDistribution([1.0, 2], [[2, 0.1], [0.1, 2]])')
         self.assertEqual(repr(NumericalDistribution([1., 2], [3, 4.])),
                          fsp + 'NumericalDistribution([1.0, 2], [3, 4.0])')
         self.assertEqual(repr(GaussianKDE([1, 2, 3], 0.1)),
                          fsp + 'GaussianKDE([1, 2, 3], 0.1, 3)')
         self.assertEqual(repr(KernelDensityEstimate([1, 2, 3], NormalDistribution(0, 0.5))),
@@ -496,14 +515,17 @@
          'gamma_upper_limit': GammaUpperLimit,
          'general_gamma_upper_limit': GeneralGammaUpperLimit,
          'numerical': NumericalDistribution,
          'multivariate_normal': MultivariateNormalDistribution,
          'multivariate_numerical': MultivariateNumericalDistribution,
          'gaussian_kde': GaussianKDE,
          'general_gamma_positive': GeneralGammaDistributionPositive,
+         'gamma_counting_process': GammaCountingProcess,
+         'general_gamma_counting_process': GeneralGammaCountingProcess,
+         'discrete_uniform': DiscreteUniformDistribution,
         }
         for k, v in class_from_string_old.items():
             self.assertEqual(v.class_to_string(), k)
             self.assertEqual(string_to_class(k), v)
             self.assertEqual(string_to_class(v.__name__), v)
         self.assertEqual(class_from_string_old,
                         {k: v for k, v in class_from_string.items()
@@ -553,16 +575,16 @@
             HalfNormalDistribution(1, -2),
             AsymmetricNormalDistribution(1, 2, 3.),
             DeltaDistribution(-3.),
             UniformDistribution(1, 2),
             GaussianUpperLimit(1e-9, 0.95),
             GammaDistribution(5, -2, 1.5),
             GammaDistributionPositive(5, -2, 1.5),
-            GammaUpperLimit(15, 10, 1e-9, 0.95),
-            GeneralGammaUpperLimit(1e-9, 0.95, counts_total=15, counts_background=10, background_variance=0.2),
+            GammaUpperLimit(counts_total=15, counts_background=10, limit=1e-9, confidence_level=0.95),
+            GeneralGammaUpperLimit(limit=1e-9, confidence_level=0.95, counts_total=15, counts_background=10, background_std=0.2),
             MultivariateNormalDistribution([1., 2], [[2, 0.1], [0.1, 2]]),
             NumericalDistribution([1., 2], [3, 4.]),
             GaussianKDE([1, 2, 3], 0.1),
             KernelDensityEstimate([1, 2, 3], NormalDistribution(0, 0.5)),
             MultivariateNumericalDistribution([[1., 2], [10., 20]], [[3, 4.],[5, 6.]], [2, 3])
         ]
         for p in ps:
```

### Comparing `flavio-2.4.0/flavio/test_citations.py` & `flavio-2.5.0/flavio/test_citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/test_classes.py` & `flavio-2.5.0/flavio/test_classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/test_functions.py` & `flavio-2.5.0/flavio/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/test_measurements.py` & `flavio-2.5.0/flavio/test_measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/test_parameters.py` & `flavio-2.5.0/flavio/test_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.assertEqual(par_dict['alpha_s'],  0.1182)
         self.assertEqual(par_dict['Gamma12_Bs_c'],  -48.0)
         # parameters from the PDG file
         self.assertEqual(par_dict['m_W'], 80.379)
         self.assertEqual(par_dict['tau_phi'], 1/4.249e-3)
         # just check if the random values are numbers
         for par_random in default_parameters.get_random_all().values():
-            self.assertIsInstance(par_random, float)
+            self.assertIsInstance(par_random, (float, int))
         for par_random in default_parameters.get_random_all(size=2).values():
             self.assertEqual(par_random.shape, (2,))
 
     def test_constraints_from_string(self):
         pds = constraints_from_string('1.36(34)(3) 1e-3')
         for pd in pds:
             self.assertEqual(pd.get_central(), 1.36e-3)
```

### Comparing `flavio-2.4.0/flavio/test_parseerrors.py` & `flavio-2.5.0/flavio/test_parseerrors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio/util.py` & `flavio-2.5.0/flavio/util.py`

 * *Files identical despite different names*

### Comparing `flavio-2.4.0/flavio.egg-info/PKG-INFO` & `flavio-2.5.0/flavio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.4.0
+Version: 2.5.0
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -68,14 +68,16 @@
 - Christoph Langenbruch
 - Christoph Niehoff
 - Markus Prim
 - Albert Puig
 - Méril Reboud
 - Stefanie Reichert
 - Niladri Sahoo
+- Jakub Šalko
+- Michael Schmidt
 - Aleks Smolkovič
 - Peter Stangl
 - Olcyr Sumensari
 - Felicia Volle
 - Zeren Simon Wang
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.4.0 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.0 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
@@ -21,17 +21,18 @@
 [Github's issue system](https://github.com/flav-io/flavio/issues) rather than
 by E-mail. Thanks! ## Contributors Maintainer: - Peter Stangl (@peterstangl)
 Original author: - David M. Straub (@DavidMStraub) Contributors (in
 alphabetical order): - Jason Aebischer - Jorge Alda Gallo - Frederik Beaujean -
 Adam Falkowski - Tobias Felkl - Ece GÃ¼rler - MatÄj Hudec - Matthew Kirk -
 Jonathan Kriewald - Jacky Kumar - Christoph Langenbruch - Christoph Niehoff -
 Markus Prim - Albert Puig - MÃ©ril Reboud - Stefanie Reichert - Niladri Sahoo -
-Aleks SmolkoviÄ - Peter Stangl - Olcyr Sumensari - Felicia Volle - Zeren Simon
-Wang ## License flavio is released under the MIT license. ## Citation If you
-use flavio in a scientific publication, please cite: > D. Straub, "flavio: a
-Python package for flavour and precision phenomenology in the Standard Model
-and beyond", [arXiv:1810.08132](https://arxiv.org/abs/1810.08132) This paper
-contains many references to results in the literature that went into the code.
-Please also consider citing the relevant original literature, where the real
-work was done. The flavio repository itself is also citable via a DOI provided
-by Zenodo: [![DOI](https://zenodo.org/badge/22356/flav-io/flavio.svg)](https://
-zenodo.org/badge/latestdoi/22356/flav-io/flavio)
+Jakub Å alko - Michael Schmidt - Aleks SmolkoviÄ - Peter Stangl - Olcyr
+Sumensari - Felicia Volle - Zeren Simon Wang ## License flavio is released
+under the MIT license. ## Citation If you use flavio in a scientific
+publication, please cite: > D. Straub, "flavio: a Python package for flavour
+and precision phenomenology in the Standard Model and beyond", [arXiv:
+1810.08132](https://arxiv.org/abs/1810.08132) This paper contains many
+references to results in the literature that went into the code. Please also
+consider citing the relevant original literature, where the real work was done.
+The flavio repository itself is also citable via a DOI provided by Zenodo: [!
+[DOI](https://zenodo.org/badge/22356/flav-io/flavio.svg)](https://zenodo.org/
+badge/latestdoi/22356/flav-io/flavio)
```

### Comparing `flavio-2.4.0/flavio.egg-info/SOURCES.txt` & `flavio-2.5.0/flavio.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -119,15 +119,17 @@
 flavio/physics/bdecays/formfactors/common.py
 flavio/physics/bdecays/formfactors/hqet.py
 flavio/physics/bdecays/formfactors/test_cln.py
 flavio/physics/bdecays/formfactors/b_gamma/__init__.py
 flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
 flavio/physics/bdecays/formfactors/b_p/__init__.py
 flavio/physics/bdecays/formfactors/b_p/bcl.py
+flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
 flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
+flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
 flavio/physics/bdecays/formfactors/b_p/bsz.py
 flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
 flavio/physics/bdecays/formfactors/b_p/btop.py
 flavio/physics/bdecays/formfactors/b_p/cln.py
 flavio/physics/bdecays/formfactors/b_p/isgurwise.py
 flavio/physics/bdecays/formfactors/b_p/test_btop.py
 flavio/physics/bdecays/formfactors/b_v/__init__.py
@@ -214,14 +216,20 @@
 flavio/physics/ddecays/rge.py
 flavio/physics/ddecays/test_dlnu.py
 flavio/physics/ddecays/test_dplnu.py
 flavio/physics/ddecays/formfactors/__init__.py
 flavio/physics/ddecays/formfactors/bcl.py
 flavio/physics/ddecays/formfactors/bsz.py
 flavio/physics/ddecays/formfactors/test_formfactors.py
+flavio/physics/dileptons/__init__.py
+flavio/physics/dileptons/partondist.py
+flavio/physics/dileptons/ppll.py
+flavio/physics/dileptons/pplnu.py
+flavio/physics/dileptons/test_ppll.py
+flavio/physics/dileptons/test_pplnu.py
 flavio/physics/edms/__init__.py
 flavio/physics/edms/common.py
 flavio/physics/edms/neutronedm.py
 flavio/physics/edms/paraedm.py
 flavio/physics/edms/slcouplings.py
 flavio/physics/edms/test_neutronedm.py
 flavio/physics/edms/test_paraedm.py
@@ -262,14 +270,23 @@
 flavio/physics/mudecays/muegamma.py
 flavio/physics/mudecays/test_mu3e.py
 flavio/physics/mudecays/test_mueconversion.py
 flavio/physics/mudecays/test_muegamma.py
 flavio/physics/neutrinos/__init__.py
 flavio/physics/neutrinos/test_trident.py
 flavio/physics/neutrinos/trident.py
+flavio/physics/quarkonium/Pll.py
+flavio/physics/quarkonium/Sll.py
+flavio/physics/quarkonium/Vll.py
+flavio/physics/quarkonium/Vllgamma.py
+flavio/physics/quarkonium/__init__.py
+flavio/physics/quarkonium/test_Pll.py
+flavio/physics/quarkonium/test_Sll.py
+flavio/physics/quarkonium/test_Vll.py
+flavio/physics/quarkonium/test_Vllgamma.py
 flavio/physics/running/__init__.py
 flavio/physics/running/betafunctions.py
 flavio/physics/running/masses.py
 flavio/physics/running/running.py
 flavio/physics/running/test_running.py
 flavio/physics/scattering/__init__.py
 flavio/physics/scattering/ee_ww.py
```

### Comparing `flavio-2.4.0/setup.py` & `flavio-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,14 @@
                 'physics/data/arXiv-1602-01399v1/*',
                 'physics/data/arXiv-1811-00983v1/*',
                 'physics/data/qcdf_interpolate/*',
                 'physics/data/wcsm/*',
                 ]
       },
       install_requires=['numpy>=1.20.0', 'scipy', 'setuptools>=3.3', 'pyyaml',
-                        'ckmutil', 'wilson>=2.0', 'particle>=0.16.0', ],
+                        'ckmutil', 'wilson>=2.0', 'particle>=0.16.0', 'parton>=0.2.1', ],
       extras_require={
             'testing': ['nose2'],
             'plotting': ['matplotlib>=2.0'],
             'sampling': ['iminuit>=2.0'],
             },
     )
```

