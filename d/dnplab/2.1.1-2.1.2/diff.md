# Comparing `tmp/dnplab-2.1.1.tar.gz` & `tmp/dnplab-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-q2g1nmw3\dnplab-2.1.1.tar", last modified: Fri Mar 31 19:37:33 2023, max compression
+gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-ojv70wkx\dnplab-2.1.2.tar", last modified: Fri Apr 14 17:52:39 2023, max compression
```

## Comparing `dnplab-2.1.1.tar` & `dnplab-2.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.657487 dnplab-2.1.1/
--rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2374 2023-03-31 19:37:33.657487 dnplab-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.223394 dnplab-2.1.1/dnplab/
--rw-rw-rw-   0        0        0      573 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.245328 dnplab-2.1.1/dnplab/analysis/
--rw-rw-rw-   0        0        0      161 2023-03-16 14:57:31.000000 dnplab-2.1.1/dnplab/analysis/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/analysis/enhancement_profiles.py
--rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/analysis/hydration.py
--rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/analysis/relaxation_fit.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.251312 dnplab-2.1.1/dnplab/constants/
--rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.1/dnplab/constants/__init__.py
--rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/constants/constants.py
--rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/constants/mrProperties.py
--rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/constants/radicalProperties.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.290568 dnplab-2.1.1/dnplab/core/
--rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.1/dnplab/core/__init__.py
--rw-rw-rw-   0        0        0    36820 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/core/base.py
--rw-rw-rw-   0        0        0     6793 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/core/coord.py
--rw-rw-rw-   0        0        0     7420 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/core/data.py
--rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/core/ufunc.py
--rw-rw-rw-   0        0        0     1428 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/core/util.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.302534 dnplab-2.1.1/dnplab/fitting/
--rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.1/dnplab/fitting/__init__.py
--rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/fitting/general.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.434723 dnplab-2.1.1/dnplab/io/
--rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/__init__.py
--rw-rw-rw-   0        0        0    15036 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/bes3t.py
--rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/io/cnsi.py
--rw-rw-rw-   0        0        0     5932 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/io/delta.py
--rw-rw-rw-   0        0        0     5740 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/h5.py
--rw-rw-rw-   0        0        0     6862 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/io/load.py
--rw-rw-rw-   0        0        0     3730 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/io/load_csv.py
--rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/io/power.py
--rw-rw-rw-   0        0        0    10252 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/io/prospa.py
--rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/io/random.py
--rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/save.py
--rw-rw-rw-   0        0        0     4969 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/specman.py
--rw-rw-rw-   0        0        0     2799 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/io/tnmr.py
--rw-rw-rw-   0        0        0    20170 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/topspin.py
--rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/vna.py
--rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/vnmrj.py
--rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/io/winepr.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.446346 dnplab-2.1.1/dnplab/math/
--rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.1/dnplab/math/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/math/lineshape.py
--rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/math/relaxation.py
--rw-rw-rw-   0        0        0     3985 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/math/window.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.462575 dnplab-2.1.1/dnplab/plotting/
--rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.1/dnplab/plotting/__init__.py
--rw-rw-rw-   0        0        0     8091 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/plotting/general.py
--rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/plotting/image.py
--rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/plotting/stack_plot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.514554 dnplab-2.1.1/dnplab/processing/
--rw-rw-rw-   0        0        0      270 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/processing/__init__.py
--rw-rw-rw-   0        0        0     7427 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/processing/align.py
--rw-rw-rw-   0        0        0     2828 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/processing/apodization.py
--rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/processing/conversion.py
--rw-rw-rw-   0        0        0     5159 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/processing/fft.py
--rw-rw-rw-   0        0        0     8703 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/processing/helpers.py
--rw-rw-rw-   0        0        0     3607 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/processing/integration.py
--rw-rw-rw-   0        0        0     2080 2023-03-16 14:57:24.000000 dnplab-2.1.1/dnplab/processing/offset.py
--rw-rw-rw-   0        0        0     9313 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/processing/phase.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.520569 dnplab-2.1.1/dnplab/reporting/
--rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.1/dnplab/reporting/__init__.py
--rw-rw-rw-   0        0        0       23 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/version.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.540643 dnplab-2.1.1/dnplab/widgets/
--rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/widgets/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.1/dnplab/widgets/align_widget.py
--rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.1/dnplab/widgets/phase_widget.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.234357 dnplab-2.1.1/dnplab.egg-info/
--rw-rw-rw-   0        0        0     2374 2023-03-31 19:37:33.000000 dnplab-2.1.1/dnplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2023-03-31 19:37:33.000000 dnplab-2.1.1/dnplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 19:37:33.000000 dnplab-2.1.1/dnplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-31 19:37:33.000000 dnplab-2.1.1/dnplab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-31 19:37:33.000000 dnplab-2.1.1/dnplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 19:37:33.658485 dnplab-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1358 2023-03-24 14:33:33.000000 dnplab-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:37:33.655524 dnplab-2.1.1/unittests/
--rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.1/unittests/__init__.py
--rw-rw-rw-   0        0        0     2223 2023-03-31 19:37:00.000000 dnplab-2.1.1/unittests/test_data_class.py
--rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.1/unittests/test_dnp_nmr.py
--rw-rw-rw-   0        0        0     3606 2023-03-31 19:37:00.000000 dnplab-2.1.1/unittests/test_dnp_tools.py
--rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.1/unittests/test_general_fit.py
--rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.1/unittests/test_hydration.py
--rw-rw-rw-   0        0        0    10338 2023-03-24 14:33:33.000000 dnplab-2.1.1/unittests/test_io.py
--rw-rw-rw-   0        0        0     1884 2022-08-30 17:05:30.000000 dnplab-2.1.1/unittests/test_load.py
--rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.1/unittests/test_nddata_core.py
--rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.1/unittests/test_save.py
--rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.1/unittests/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.538852 dnplab-2.1.2/
+-rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2374 2023-04-14 17:52:39.537854 dnplab-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.175392 dnplab-2.1.2/dnplab/
+-rw-rw-rw-   0        0        0      573 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.197361 dnplab-2.1.2/dnplab/analysis/
+-rw-rw-rw-   0        0        0      161 2023-03-16 14:57:31.000000 dnplab-2.1.2/dnplab/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/analysis/enhancement_profiles.py
+-rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/analysis/hydration.py
+-rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/analysis/relaxation_fit.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.204342 dnplab-2.1.2/dnplab/constants/
+-rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/constants/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/constants.py
+-rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/mrProperties.py
+-rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/radicalProperties.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.255776 dnplab-2.1.2/dnplab/core/
+-rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/core/__init__.py
+-rw-rw-rw-   0        0        0    36820 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/base.py
+-rw-rw-rw-   0        0        0     6793 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/coord.py
+-rw-rw-rw-   0        0        0     7420 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/data.py
+-rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/core/ufunc.py
+-rw-rw-rw-   0        0        0     1428 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/core/util.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.266744 dnplab-2.1.2/dnplab/fitting/
+-rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/fitting/__init__.py
+-rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/fitting/general.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.420259 dnplab-2.1.2/dnplab/io/
+-rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/__init__.py
+-rw-rw-rw-   0        0        0    15036 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/bes3t.py
+-rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/cnsi.py
+-rw-rw-rw-   0        0        0     5932 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/delta.py
+-rw-rw-rw-   0        0        0     5740 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/h5.py
+-rw-rw-rw-   0        0        0     6862 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/load.py
+-rw-rw-rw-   0        0        0     3730 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/load_csv.py
+-rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/power.py
+-rw-rw-rw-   0        0        0    10252 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/prospa.py
+-rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/random.py
+-rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/save.py
+-rw-rw-rw-   0        0        0     4969 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/specman.py
+-rw-rw-rw-   0        0        0     2799 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/tnmr.py
+-rw-rw-rw-   0        0        0    20170 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/topspin.py
+-rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/vna.py
+-rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/vnmrj.py
+-rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/winepr.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.432230 dnplab-2.1.2/dnplab/math/
+-rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.2/dnplab/math/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/math/lineshape.py
+-rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/math/relaxation.py
+-rw-rw-rw-   0        0        0     3985 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/math/window.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.448214 dnplab-2.1.2/dnplab/plotting/
+-rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/plotting/__init__.py
+-rw-rw-rw-   0        0        0     8149 2023-04-14 17:51:32.000000 dnplab-2.1.2/dnplab/plotting/general.py
+-rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/plotting/image.py
+-rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/plotting/stack_plot.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.505829 dnplab-2.1.2/dnplab/processing/
+-rw-rw-rw-   0        0        0      270 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/__init__.py
+-rw-rw-rw-   0        0        0     7427 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/processing/align.py
+-rw-rw-rw-   0        0        0     2828 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/apodization.py
+-rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/processing/conversion.py
+-rw-rw-rw-   0        0        0     5159 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/fft.py
+-rw-rw-rw-   0        0        0     8703 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/helpers.py
+-rw-rw-rw-   0        0        0     3607 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/integration.py
+-rw-rw-rw-   0        0        0     2080 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/offset.py
+-rw-rw-rw-   0        0        0     9313 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/phase.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.509846 dnplab-2.1.2/dnplab/reporting/
+-rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/reporting/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-14 17:51:32.000000 dnplab-2.1.2/dnplab/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.524788 dnplab-2.1.2/dnplab/widgets/
+-rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/widgets/align_widget.py
+-rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/widgets/phase_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.186391 dnplab-2.1.2/dnplab.egg-info/
+-rw-rw-rw-   0        0        0     2374 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 17:52:39.538852 dnplab-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1358 2023-03-24 14:33:33.000000 dnplab-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.536886 dnplab-2.1.2/unittests/
+-rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.2/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2223 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_data_class.py
+-rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_dnp_nmr.py
+-rw-rw-rw-   0        0        0     3606 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_dnp_tools.py
+-rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_general_fit.py
+-rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_hydration.py
+-rw-rw-rw-   0        0        0    10338 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_io.py
+-rw-rw-rw-   0        0        0     1884 2022-08-30 17:05:30.000000 dnplab-2.1.2/unittests/test_load.py
+-rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_nddata_core.py
+-rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_save.py
+-rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/testing.py
```

### Comparing `dnplab-2.1.1/LICENSE.txt` & `dnplab-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/PKG-INFO` & `dnplab-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.1
+Version: 2.1.2
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.1/README.md` & `dnplab-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/__init__.py` & `dnplab-2.1.2/dnplab/__init__.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/analysis/enhancement_profiles.py` & `dnplab-2.1.2/dnplab/analysis/enhancement_profiles.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/analysis/hydration.py` & `dnplab-2.1.2/dnplab/analysis/hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/analysis/relaxation_fit.py` & `dnplab-2.1.2/dnplab/analysis/relaxation_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/constants/mrProperties.py` & `dnplab-2.1.2/dnplab/constants/mrProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/constants/radicalProperties.py` & `dnplab-2.1.2/dnplab/constants/radicalProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/core/base.py` & `dnplab-2.1.2/dnplab/core/base.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/core/coord.py` & `dnplab-2.1.2/dnplab/core/coord.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/core/data.py` & `dnplab-2.1.2/dnplab/core/data.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/core/ufunc.py` & `dnplab-2.1.2/dnplab/core/ufunc.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/core/util.py` & `dnplab-2.1.2/dnplab/core/util.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/fitting/general.py` & `dnplab-2.1.2/dnplab/fitting/general.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/bes3t.py` & `dnplab-2.1.2/dnplab/io/bes3t.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/cnsi.py` & `dnplab-2.1.2/dnplab/io/cnsi.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/delta.py` & `dnplab-2.1.2/dnplab/io/delta.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/h5.py` & `dnplab-2.1.2/dnplab/io/h5.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/load.py` & `dnplab-2.1.2/dnplab/io/load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/load_csv.py` & `dnplab-2.1.2/dnplab/io/load_csv.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/power.py` & `dnplab-2.1.2/dnplab/io/power.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/prospa.py` & `dnplab-2.1.2/dnplab/io/prospa.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/random.py` & `dnplab-2.1.2/dnplab/io/random.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/save.py` & `dnplab-2.1.2/dnplab/io/save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/specman.py` & `dnplab-2.1.2/dnplab/io/specman.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/tnmr.py` & `dnplab-2.1.2/dnplab/io/tnmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/topspin.py` & `dnplab-2.1.2/dnplab/io/topspin.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/vna.py` & `dnplab-2.1.2/dnplab/io/vna.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/vnmrj.py` & `dnplab-2.1.2/dnplab/io/vnmrj.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/io/winepr.py` & `dnplab-2.1.2/dnplab/io/winepr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/math/lineshape.py` & `dnplab-2.1.2/dnplab/math/lineshape.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/math/relaxation.py` & `dnplab-2.1.2/dnplab/math/relaxation.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/math/window.py` & `dnplab-2.1.2/dnplab/math/window.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/plotting/general.py` & `dnplab-2.1.2/dnplab/plotting/general.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as _plt
 import numpy as _np
 from warnings import warn
 
 from ..core.data import DNPData
 
 dark_green = "#46812B"
 light_green = "#67AE3E"
 dark_grey = "#4D4D4F"
 light_grey = "#A7A9AC"
 orange = "#F37021"
 
-plt.rcParams["lines.linewidth"] = 1.5
-plt.rcParams["axes.prop_cycle"] = plt.cycler(
+_plt.rcParams["lines.linewidth"] = 1.5
+_plt.rcParams["axes.prop_cycle"] = _plt.cycler(
     color=[orange, dark_green, light_green, dark_grey, light_grey]
 )
 
-show = plt.show
+show = _plt.show
 
 # hand curated list of plotting arguments that are forwarded, note that this should probably be in a config file (refactoring needed)
 forwarded_pyplot_plots = [
     "semilogy",
     "semilogx",
     "polar",
     "loglog",
@@ -85,20 +85,20 @@
 
     # will try to plot various pyplot utility plot functions into same axis, the use should know what he does!
     # no unittest added, but only hand tested with semilogy and normal plot works as intended ni fancy_plot)
     use_default = True
     plot_function_list = []
     for k in forwarded_pyplot_plots:
         if bool(kwargs.pop(k, None)):
-            plot_function_list.append(getattr(plt, k))
+            plot_function_list.append(getattr(_plt, k))
             use_default = False
     for f in plot_function_list:
         f(coord, data.values.real, *args, **kwargs)
     if use_default:
-        plt.plot(coord, data.values.real, *args, **kwargs)
+        _plt.plot(coord, data.values.real, *args, **kwargs)
     data.fold()
 
 
 def fancy_plot(data, xlim=[], title="", showPar=False, *args, **kwargs):
     """Streamline Plot function for dnpdata objects
 
     This function creates streamlined plots for NMR and EPR spectra. The type of the spectrum is detected from the attribute "experiment_type" of the dnpdata object. Currently the following types are implemented: nmr_spectrum, epr_spectrum, enhancements_P, and inversion_recovery. The function will automatically format the plot according to the "experiment_type" attribute.
@@ -134,48 +134,48 @@
         return
 
     if "dim" in kwargs:
         dim = kwargs.pop("dim")
     else:
         dim = data.dims[0]
 
-    plt.grid(True)
-    plt.title(title)
+    _plt.grid(True)
+    _plt.title(title)
 
     if data.attrs["experiment_type"] == "nmr_spectrum":
         coord = data.coords[dim]
         data.unfold(dim)
 
-        plt.plot(coord, data.values.real, *args, **kwargs)
-        plt.xlabel("Chemical Shift $\delta$ (ppm)")
-        plt.ylabel("NMR Signal Intensity (a.u.)")
+        _plt.plot(coord, data.values.real, *args, **kwargs)
+        _plt.xlabel("Chemical Shift $\delta$ (ppm)")
+        _plt.ylabel("NMR Signal Intensity (a.u.)")
 
-        plt.xlim(max(coord), min(coord))
+        _plt.xlim(max(coord), min(coord))
 
         if xlim != []:
-            plt.xlim(xlim[1], xlim[0])
+            _plt.xlim(xlim[1], xlim[0])
 
         if showPar == True:
             parameterString = "Freq: " + str(round(data.attrs["nmr_frequency"], 4))
 
             box_style = dict(boxstyle="round", facecolor="white", alpha=0.25)
-            xmin, xmax, ymin, ymax = plt.axis()
+            xmin, xmax, ymin, ymax = _plt.axis()
 
-            plt.text(xmin * 0.95, ymax / 10, parameterString, bbox=box_style)
+            _plt.text(xmin * 0.95, ymax / 10, parameterString, bbox=box_style)
 
     elif data.attrs["experiment_type"] == "epr_spectrum":
         coord = data.coords[dim]
         data.unfold(dim)
 
-        plt.plot(coord, data.values.real, *args, **kwargs)
-        plt.xlabel("Magnetic Field $B_{0}$ (mT)")
-        plt.ylabel("EPR Signal Intensity (a.u.)")
+        _plt.plot(coord, data.values.real, *args, **kwargs)
+        _plt.xlabel("Magnetic Field $B_{0}$ (mT)")
+        _plt.ylabel("EPR Signal Intensity (a.u.)")
 
         if xlim != []:
-            plt.xlim(xlim[0], xlim[1])
+            _plt.xlim(xlim[0], xlim[1])
 
         if showPar == True:
             SW = coord[-1] - coord[0]
 
             parameterString = (
                 "MF: "
                 + str(round(data.attrs["frequency"], 4))
@@ -190,69 +190,71 @@
                 + "\nNS: "
                 + str(data.attrs["nscans"])
                 + "\nTM: "
                 + str(round(data.attrs["temperature"], 1))
             )
 
             box_style = dict(boxstyle="round", facecolor="white", alpha=0.25)
-            xmin, xmax, ymin, ymax = plt.axis()
+            xmin, xmax, ymin, ymax = _plt.axis()
 
-            plt.text(xmin * 1.001, ymin * 0.90, parameterString, bbox=box_style)
+            _plt.text(xmin * 1.001, ymin * 0.90, parameterString, bbox=box_style)
 
     elif (
         data.attrs["experiment_type"] == "enhancements_P"
         or data.attrs["experiment_type"] == "enhancements_PdBm"
     ):
         coord = data.coords[dim]
         data.unfold(dim)
 
-        plt.plot(coord, data.values.real, marker="o", fillstyle="none", *args, **kwargs)
-        plt.xlabel("Microwave Power (dBm)")
-        plt.ylabel("DNP Enhancement")
+        _plt.plot(
+            coord, data.values.real, marker="o", fillstyle="none", *args, **kwargs
+        )
+        _plt.xlabel("Microwave Power (dBm)")
+        _plt.ylabel("DNP Enhancement")
 
         if xlim != []:
-            plt.xlim(xlim[0], xlim[1])
+            _plt.xlim(xlim[0], xlim[1])
 
         # if showPar == True:
 
     elif data.attrs["experiment_type"] == "enhancements_PW":
         coord = data.coords[dim]
         data.unfold(dim)
 
-        plt.plot(
+        _plt.plot(
             coord * 1e-3,
             data.values.real,
             marker="o",
             fillstyle="none",
             *args,
             **kwargs
         )
-        plt.xlabel("Microwave Power (W)")
-        plt.ylabel("DNP Enhancement")
+        _plt.xlabel("Microwave Power (W)")
+        _plt.ylabel("DNP Enhancement")
 
         if xlim != []:
-            plt.xlim(xlim[0], xlim[1])
+            _plt.xlim(xlim[0], xlim[1])
 
         # if showPar == True:
 
     elif data.attrs["experiment_type"] == "inversion_recovery":
-        plt.plot(
+        _plt.plot(
             data.coords["t1"],
             data.values.real,
             marker="o",
             fillstyle="none",
             *args,
             **kwargs
         )
 
-        plt.xlabel("Evolution Time T1 (s)")
-        plt.ylabel("NMR Amplitude [a.u.]")
+        _plt.xlabel("Evolution Time T1 (s)")
+        _plt.ylabel("NMR Amplitude [a.u.]")
 
         if xlim != []:
-            plt.xlim(xlim[0], xlim[1])
+            _plt.xlim(xlim[0], xlim[1])
 
         # if showPar == True:
 
     else:
         plot(data, *args, **kwargs)
 
     data.fold()
```

### Comparing `dnplab-2.1.1/dnplab/plotting/image.py` & `dnplab-2.1.2/dnplab/plotting/image.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/plotting/stack_plot.py` & `dnplab-2.1.2/dnplab/plotting/stack_plot.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/align.py` & `dnplab-2.1.2/dnplab/processing/align.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/apodization.py` & `dnplab-2.1.2/dnplab/processing/apodization.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/conversion.py` & `dnplab-2.1.2/dnplab/processing/conversion.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/fft.py` & `dnplab-2.1.2/dnplab/processing/fft.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/helpers.py` & `dnplab-2.1.2/dnplab/processing/helpers.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/integration.py` & `dnplab-2.1.2/dnplab/processing/integration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/offset.py` & `dnplab-2.1.2/dnplab/processing/offset.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/processing/phase.py` & `dnplab-2.1.2/dnplab/processing/phase.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/widgets/align_widget.py` & `dnplab-2.1.2/dnplab/widgets/align_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab/widgets/phase_widget.py` & `dnplab-2.1.2/dnplab/widgets/phase_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/dnplab.egg-info/PKG-INFO` & `dnplab-2.1.2/dnplab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.1
+Version: 2.1.2
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.1/dnplab.egg-info/SOURCES.txt` & `dnplab-2.1.2/dnplab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/setup.py` & `dnplab-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_data_class.py` & `dnplab-2.1.2/unittests/test_data_class.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_dnp_nmr.py` & `dnplab-2.1.2/unittests/test_dnp_nmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_dnp_tools.py` & `dnplab-2.1.2/unittests/test_dnp_tools.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_general_fit.py` & `dnplab-2.1.2/unittests/test_general_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_hydration.py` & `dnplab-2.1.2/unittests/test_hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_io.py` & `dnplab-2.1.2/unittests/test_io.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_load.py` & `dnplab-2.1.2/unittests/test_load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_nddata_core.py` & `dnplab-2.1.2/unittests/test_nddata_core.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/test_save.py` & `dnplab-2.1.2/unittests/test_save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.1/unittests/testing.py` & `dnplab-2.1.2/unittests/testing.py`

 * *Files identical despite different names*

