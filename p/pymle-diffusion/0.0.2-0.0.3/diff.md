# Comparing `tmp/pymle-diffusion-0.0.2.tar.gz` & `tmp/pymle-diffusion-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymle-diffusion-0.0.2.tar", last modified: Fri Apr 14 00:23:25 2023, max compression
+gzip compressed data, was "pymle-diffusion-0.0.3.tar", last modified: Fri Apr 14 00:29:46 2023, max compression
```

## Comparing `pymle-diffusion-0.0.2.tar` & `pymle-diffusion-0.0.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:25.789895 pymle-diffusion-0.0.2/
--rw-rw-rw-   0        0        0       70 2023-04-13 23:55:37.000000 pymle-diffusion-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-01-16 00:38:30.000000 pymle-diffusion-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      718 2023-04-14 00:23:25.789895 pymle-diffusion-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5934 2023-04-14 00:21:59.000000 pymle-diffusion-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.472833 pymle-diffusion-0.0.2/examples/
--rw-rw-rw-   0        0        0     2894 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.2/examples/Example_CIR_MLE.py
--rw-rw-rw-   0        0        0     3221 2023-04-14 00:19:13.000000 pymle-diffusion-0.0.2/examples/RealDataExample_CIR_Fit_Interest.py
--rw-rw-rw-   0        0        0     2537 2023-04-14 00:18:54.000000 pymle-diffusion-0.0.2/examples/RealDataExample_CKLS_Fit_Interest.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.476935 pymle-diffusion-0.0.2/pymle/
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.2/pymle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.488021 pymle-diffusion-0.0.2/pymle/core/
--rw-rw-rw-   0        0        0     6169 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/core/Model.py
--rw-rw-rw-   0        0        0    11256 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/core/TransitionDensity.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.653306 pymle-diffusion-0.0.2/pymle/ctmc/
--rw-rw-rw-   0        0        0     3789 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/ctmc/CTMCEstimator.py
--rw-rw-rw-   0        0        0     3905 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/ctmc/Generator1D.py
--rw-rw-rw-   0        0        0     3043 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/ctmc/StateSpace.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/ctmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.667541 pymle-diffusion-0.0.2/pymle/data/
--rw-rw-rw-   0        0        0   236026 2021-04-14 16:41:45.000000 pymle-diffusion-0.0.2/pymle/data/10yrCMrate.csv
--rw-rw-rw-   0        0        0   100149 2021-05-25 00:05:40.000000 pymle-diffusion-0.0.2/pymle/data/FX_EUR_USD.csv
--rw-rw-rw-   0        0        0   133138 2021-05-17 23:32:17.000000 pymle-diffusion-0.0.2/pymle/data/VIX.csv
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.2/pymle/data/__init__.py
--rw-rw-rw-   0        0        0      508 2023-04-14 00:14:06.000000 pymle-diffusion-0.0.2/pymle/data/loader.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.684274 pymle-diffusion-0.0.2/pymle/fit/
--rw-rw-rw-   0        0        0     2314 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/fit/AnalyticalMLE.py
--rw-rw-rw-   0        0        0     4032 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/fit/Estimator.py
--rw-rw-rw-   0        0        0     3662 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/fit/LikelihoodEstimator.py
--rw-rw-rw-   0        0        0     3598 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/fit/Minimizer.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/fit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.806327 pymle-diffusion-0.0.2/pymle/models/
--rw-rw-rw-   0        0        0     3810 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/AitSahalia96.py
--rw-rw-rw-   0        0        0     1874 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/BrownianMotion.py
--rw-rw-rw-   0        0        0     3059 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/CEV.py
--rw-rw-rw-   0        0        0     4685 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/CIR.py
--rw-rw-rw-   0        0        0     1084 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/CKLS.py
--rw-rw-rw-   0        0        0     3979 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/FellerRoot.py
--rw-rw-rw-   0        0        0     3512 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/GeometricBM.py
--rw-rw-rw-   0        0        0      936 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Hyperbolic.py
--rw-rw-rw-   0        0        0     1024 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Hyperbolic2.py
--rw-rw-rw-   0        0        0     2898 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/IGBM.py
--rw-rw-rw-   0        0        0     3848 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Jacobi.py
--rw-rw-rw-   0        0        0     2253 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/LinearSDE1.py
--rw-rw-rw-   0        0        0     2536 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/LinearSDE2.py
--rw-rw-rw-   0        0        0     3070 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Logistic.py
--rw-rw-rw-   0        0        0     3741 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/ModifiedCIR.py
--rw-rw-rw-   0        0        0     3250 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/NonLinearSDE.py
--rw-rw-rw-   0        0        0     2485 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/OrnsteinUhlenbeck.py
--rw-rw-rw-   0        0        0     3927 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Pearson.py
--rw-rw-rw-   0        0        0     3465 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/PeralVerhulst.py
--rw-rw-rw-   0        0        0     3401 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/RadialOU.py
--rw-rw-rw-   0        0        0     3783 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/Threehalf.py
--rw-rw-rw-   0        0        0      924 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.899961 pymle-diffusion-0.0.2/pymle/sim/
--rw-rw-rw-   0        0        0     3877 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/sim/Simulator1D.py
--rw-rw-rw-   0        0        0     7678 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/sim/Stepper.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.2/pymle/sim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:24.911191 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/
--rw-rw-rw-   0        0        0      718 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2219 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.2/pymle_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-14 22:19:45.000000 pymle-diffusion-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-04-14 00:01:59.000000 pymle-diffusion-0.0.2/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:25.541753 pymle-diffusion-0.0.2/scripts/
--rw-rw-rw-   0        0        0     2015 2023-03-17 14:37:13.000000 pymle-diffusion-0.0.2/scripts/Script_1_For_Submission_LOCAL.py
--rw-rw-rw-   0        0        0     2369 2023-03-17 14:36:44.000000 pymle-diffusion-0.0.2/scripts/Script_2_For_Submission_LOCAL.py
--rw-rw-rw-   0        0        0     2626 2023-03-17 14:46:02.000000 pymle-diffusion-0.0.2/scripts/Script_3_For_Submission_LOCAL.py
--rw-rw-rw-   0        0        0     7006 2023-03-17 14:46:02.000000 pymle-diffusion-0.0.2/scripts/Script_COMBINED_For_Submission_LOCAL.py
--rw-rw-rw-   0        0        0     2698 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_CTMC_Converge_LOCAL.py
--rw-rw-rw-   0        0        0     2056 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_EffectOfBinning_LOCAL.py
--rw-rw-rw-   0        0        0     5822 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL.py
--rw-rw-rw-   0        0        0     5818 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL2.py
--rw-rw-rw-   0        0        0     5819 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL3.py
--rw-rw-rw-   0        0        0      102 2022-07-24 02:24:00.000000 pymle-diffusion-0.0.2/scripts/Test_Fit_10yrRate_LOCAL.py
--rw-rw-rw-   0        0        0     4336 2023-03-17 12:54:52.000000 pymle-diffusion-0.0.2/scripts/Test_Initial_LOCAL.py
--rw-rw-rw-   0        0        0     1670 2021-04-13 00:02:14.000000 pymle-diffusion-0.0.2/scripts/Test_Likelihood_Convergence_LOCAL.py
--rw-rw-rw-   0        0        0     3782 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.2/scripts/Test_Param_Histograms_LOCAL.py
--rw-rw-rw-   0        0        0        0 2021-02-13 13:32:20.000000 pymle-diffusion-0.0.2/scripts/__init__.py
--rw-rw-rw-   0        0        0      111 2023-04-14 00:23:25.790893 pymle-diffusion-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-04-14 00:01:59.000000 pymle-diffusion-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:25.546388 pymle-diffusion-0.0.2/tests/
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:25.650046 pymle-diffusion-0.0.2/tests/fit/
--rw-rw-rw-   0        0        0     3929 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.2/tests/fit/Test_AnalyticalMLE.py
--rw-rw-rw-   0        0        0        0 2023-01-01 00:52:35.000000 pymle-diffusion-0.0.2/tests/fit/__init__.py
--rw-rw-rw-   0        0        0      361 2023-01-01 00:53:32.000000 pymle-diffusion-0.0.2/tests/fit/suite.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:23:25.747276 pymle-diffusion-0.0.2/tests/models/
--rw-rw-rw-   0        0        0      658 2023-01-01 00:51:44.000000 pymle-diffusion-0.0.2/tests/models/Test_CEV.py
--rw-rw-rw-   0        0        0        0 2022-12-31 23:16:13.000000 pymle-diffusion-0.0.2/tests/models/__init__.py
--rw-rw-rw-   0        0        0      334 2022-12-31 23:17:37.000000 pymle-diffusion-0.0.2/tests/models/suite.py
--rw-rw-rw-   0        0        0      415 2023-01-01 00:54:06.000000 pymle-diffusion-0.0.2/tests/test_runner.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.764366 pymle-diffusion-0.0.3/
+-rw-rw-rw-   0        0        0       70 2023-04-13 23:55:37.000000 pymle-diffusion-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-01-16 00:38:30.000000 pymle-diffusion-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      718 2023-04-14 00:29:46.764366 pymle-diffusion-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5934 2023-04-14 00:21:59.000000 pymle-diffusion-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.495554 pymle-diffusion-0.0.3/examples/
+-rw-rw-rw-   0        0        0     2894 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.3/examples/Example_CIR_MLE.py
+-rw-rw-rw-   0        0        0     3221 2023-04-14 00:19:13.000000 pymle-diffusion-0.0.3/examples/RealDataExample_CIR_Fit_Interest.py
+-rw-rw-rw-   0        0        0     2537 2023-04-14 00:18:54.000000 pymle-diffusion-0.0.3/examples/RealDataExample_CKLS_Fit_Interest.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.498888 pymle-diffusion-0.0.3/pymle/
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.3/pymle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.510798 pymle-diffusion-0.0.3/pymle/core/
+-rw-rw-rw-   0        0        0     6169 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/core/Model.py
+-rw-rw-rw-   0        0        0    11256 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/core/TransitionDensity.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.525699 pymle-diffusion-0.0.3/pymle/ctmc/
+-rw-rw-rw-   0        0        0     3789 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/ctmc/CTMCEstimator.py
+-rw-rw-rw-   0        0        0     3905 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/ctmc/Generator1D.py
+-rw-rw-rw-   0        0        0     3043 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/ctmc/StateSpace.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/ctmc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.570510 pymle-diffusion-0.0.3/pymle/data/
+-rw-rw-rw-   0        0        0   236026 2021-04-14 16:41:45.000000 pymle-diffusion-0.0.3/pymle/data/10yrCMrate.csv
+-rw-rw-rw-   0        0        0   100149 2021-05-25 00:05:40.000000 pymle-diffusion-0.0.3/pymle/data/FX_EUR_USD.csv
+-rw-rw-rw-   0        0        0   133138 2021-05-17 23:32:17.000000 pymle-diffusion-0.0.3/pymle/data/VIX.csv
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.3/pymle/data/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-04-14 00:14:06.000000 pymle-diffusion-0.0.3/pymle/data/loader.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.589399 pymle-diffusion-0.0.3/pymle/fit/
+-rw-rw-rw-   0        0        0     2314 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/fit/AnalyticalMLE.py
+-rw-rw-rw-   0        0        0     4032 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/fit/Estimator.py
+-rw-rw-rw-   0        0        0     3662 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/fit/LikelihoodEstimator.py
+-rw-rw-rw-   0        0        0     3598 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/fit/Minimizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/fit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.669087 pymle-diffusion-0.0.3/pymle/models/
+-rw-rw-rw-   0        0        0     3810 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/AitSahalia96.py
+-rw-rw-rw-   0        0        0     1874 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/BrownianMotion.py
+-rw-rw-rw-   0        0        0     3059 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/CEV.py
+-rw-rw-rw-   0        0        0     4685 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/CIR.py
+-rw-rw-rw-   0        0        0     1084 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/CKLS.py
+-rw-rw-rw-   0        0        0     3979 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/FellerRoot.py
+-rw-rw-rw-   0        0        0     3512 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/GeometricBM.py
+-rw-rw-rw-   0        0        0      936 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Hyperbolic.py
+-rw-rw-rw-   0        0        0     1024 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Hyperbolic2.py
+-rw-rw-rw-   0        0        0     2898 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/IGBM.py
+-rw-rw-rw-   0        0        0     3848 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Jacobi.py
+-rw-rw-rw-   0        0        0     2253 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/LinearSDE1.py
+-rw-rw-rw-   0        0        0     2536 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/LinearSDE2.py
+-rw-rw-rw-   0        0        0     3070 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Logistic.py
+-rw-rw-rw-   0        0        0     3741 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/ModifiedCIR.py
+-rw-rw-rw-   0        0        0     3250 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/NonLinearSDE.py
+-rw-rw-rw-   0        0        0     2485 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/OrnsteinUhlenbeck.py
+-rw-rw-rw-   0        0        0     3927 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Pearson.py
+-rw-rw-rw-   0        0        0     3465 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/PeralVerhulst.py
+-rw-rw-rw-   0        0        0     3401 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/RadialOU.py
+-rw-rw-rw-   0        0        0     3783 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/Threehalf.py
+-rw-rw-rw-   0        0        0      924 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.679575 pymle-diffusion-0.0.3/pymle/sim/
+-rw-rw-rw-   0        0        0     3877 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/sim/Simulator1D.py
+-rw-rw-rw-   0        0        0     7678 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/sim/Stepper.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.3/pymle/sim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.691388 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/
+-rw-rw-rw-   0        0        0      718 2023-04-14 00:29:46.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-04-14 00:29:46.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:29:46.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 00:23:24.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-04-14 00:29:46.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 00:29:46.000000 pymle-diffusion-0.0.3/pymle_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-14 22:19:45.000000 pymle-diffusion-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-04-14 00:01:59.000000 pymle-diffusion-0.0.3/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.734962 pymle-diffusion-0.0.3/scripts/
+-rw-rw-rw-   0        0        0     2015 2023-03-17 14:37:13.000000 pymle-diffusion-0.0.3/scripts/Script_1_For_Submission_LOCAL.py
+-rw-rw-rw-   0        0        0     2369 2023-03-17 14:36:44.000000 pymle-diffusion-0.0.3/scripts/Script_2_For_Submission_LOCAL.py
+-rw-rw-rw-   0        0        0     2626 2023-03-17 14:46:02.000000 pymle-diffusion-0.0.3/scripts/Script_3_For_Submission_LOCAL.py
+-rw-rw-rw-   0        0        0     7006 2023-03-17 14:46:02.000000 pymle-diffusion-0.0.3/scripts/Script_COMBINED_For_Submission_LOCAL.py
+-rw-rw-rw-   0        0        0     2698 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_CTMC_Converge_LOCAL.py
+-rw-rw-rw-   0        0        0     2056 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_EffectOfBinning_LOCAL.py
+-rw-rw-rw-   0        0        0     5822 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL.py
+-rw-rw-rw-   0        0        0     5818 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL2.py
+-rw-rw-rw-   0        0        0     5819 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL3.py
+-rw-rw-rw-   0        0        0      102 2022-07-24 02:24:00.000000 pymle-diffusion-0.0.3/scripts/Test_Fit_10yrRate_LOCAL.py
+-rw-rw-rw-   0        0        0     4336 2023-03-17 12:54:52.000000 pymle-diffusion-0.0.3/scripts/Test_Initial_LOCAL.py
+-rw-rw-rw-   0        0        0     1670 2021-04-13 00:02:14.000000 pymle-diffusion-0.0.3/scripts/Test_Likelihood_Convergence_LOCAL.py
+-rw-rw-rw-   0        0        0     3782 2023-03-10 16:18:09.000000 pymle-diffusion-0.0.3/scripts/Test_Param_Histograms_LOCAL.py
+-rw-rw-rw-   0        0        0        0 2021-02-13 13:32:20.000000 pymle-diffusion-0.0.3/scripts/__init__.py
+-rw-rw-rw-   0        0        0      111 2023-04-14 00:29:46.765363 pymle-diffusion-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-04-14 00:28:30.000000 pymle-diffusion-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.739404 pymle-diffusion-0.0.3/tests/
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.749637 pymle-diffusion-0.0.3/tests/fit/
+-rw-rw-rw-   0        0        0     3929 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.3/tests/fit/Test_AnalyticalMLE.py
+-rw-rw-rw-   0        0        0        0 2023-01-01 00:52:35.000000 pymle-diffusion-0.0.3/tests/fit/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-01-01 00:53:32.000000 pymle-diffusion-0.0.3/tests/fit/suite.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:29:46.760376 pymle-diffusion-0.0.3/tests/models/
+-rw-rw-rw-   0        0        0      658 2023-01-01 00:51:44.000000 pymle-diffusion-0.0.3/tests/models/Test_CEV.py
+-rw-rw-rw-   0        0        0        0 2022-12-31 23:16:13.000000 pymle-diffusion-0.0.3/tests/models/__init__.py
+-rw-rw-rw-   0        0        0      334 2022-12-31 23:17:37.000000 pymle-diffusion-0.0.3/tests/models/suite.py
+-rw-rw-rw-   0        0        0      415 2023-01-01 00:54:06.000000 pymle-diffusion-0.0.3/tests/test_runner.py
```

### Comparing `pymle-diffusion-0.0.2/LICENSE` & `pymle-diffusion-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/PKG-INFO` & `pymle-diffusion-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymle-diffusion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Maximum Likelihood Estimation (MLE) and simulation for SDE
 Home-page: https://github.com/jkirkby3/pymle
 Author: Justin Lars Kirkby
 Author-email: jkirkby33@gmail.com
 License: MIT
 Description: Maximum Likelihood Estimation (MLE) and simulation for Stochastic Differential Equations (SDE)
 Keywords: sde mle maximum likelihood difussion estimation simulation
```

### Comparing `pymle-diffusion-0.0.2/README.md` & `pymle-diffusion-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/examples/Example_CIR_MLE.py` & `pymle-diffusion-0.0.3/examples/Example_CIR_MLE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/examples/RealDataExample_CIR_Fit_Interest.py` & `pymle-diffusion-0.0.3/examples/RealDataExample_CIR_Fit_Interest.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/examples/RealDataExample_CKLS_Fit_Interest.py` & `pymle-diffusion-0.0.3/examples/RealDataExample_CKLS_Fit_Interest.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/core/Model.py` & `pymle-diffusion-0.0.3/pymle/core/Model.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/core/TransitionDensity.py` & `pymle-diffusion-0.0.3/pymle/core/TransitionDensity.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/ctmc/CTMCEstimator.py` & `pymle-diffusion-0.0.3/pymle/ctmc/CTMCEstimator.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/ctmc/Generator1D.py` & `pymle-diffusion-0.0.3/pymle/ctmc/Generator1D.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/ctmc/StateSpace.py` & `pymle-diffusion-0.0.3/pymle/ctmc/StateSpace.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/data/10yrCMrate.csv` & `pymle-diffusion-0.0.3/pymle/data/10yrCMrate.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/data/FX_EUR_USD.csv` & `pymle-diffusion-0.0.3/pymle/data/FX_EUR_USD.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/data/VIX.csv` & `pymle-diffusion-0.0.3/pymle/data/VIX.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/fit/AnalyticalMLE.py` & `pymle-diffusion-0.0.3/pymle/fit/AnalyticalMLE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/fit/Estimator.py` & `pymle-diffusion-0.0.3/pymle/fit/Estimator.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/fit/LikelihoodEstimator.py` & `pymle-diffusion-0.0.3/pymle/fit/LikelihoodEstimator.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/fit/Minimizer.py` & `pymle-diffusion-0.0.3/pymle/fit/Minimizer.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/AitSahalia96.py` & `pymle-diffusion-0.0.3/pymle/models/AitSahalia96.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/BrownianMotion.py` & `pymle-diffusion-0.0.3/pymle/models/BrownianMotion.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/CEV.py` & `pymle-diffusion-0.0.3/pymle/models/CEV.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/CIR.py` & `pymle-diffusion-0.0.3/pymle/models/CIR.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/CKLS.py` & `pymle-diffusion-0.0.3/pymle/models/CKLS.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/FellerRoot.py` & `pymle-diffusion-0.0.3/pymle/models/FellerRoot.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/GeometricBM.py` & `pymle-diffusion-0.0.3/pymle/models/GeometricBM.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Hyperbolic.py` & `pymle-diffusion-0.0.3/pymle/models/Hyperbolic.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Hyperbolic2.py` & `pymle-diffusion-0.0.3/pymle/models/Hyperbolic2.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/IGBM.py` & `pymle-diffusion-0.0.3/pymle/models/IGBM.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Jacobi.py` & `pymle-diffusion-0.0.3/pymle/models/Jacobi.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/LinearSDE1.py` & `pymle-diffusion-0.0.3/pymle/models/LinearSDE1.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/LinearSDE2.py` & `pymle-diffusion-0.0.3/pymle/models/LinearSDE2.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Logistic.py` & `pymle-diffusion-0.0.3/pymle/models/Logistic.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/ModifiedCIR.py` & `pymle-diffusion-0.0.3/pymle/models/ModifiedCIR.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/NonLinearSDE.py` & `pymle-diffusion-0.0.3/pymle/models/NonLinearSDE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/OrnsteinUhlenbeck.py` & `pymle-diffusion-0.0.3/pymle/models/OrnsteinUhlenbeck.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Pearson.py` & `pymle-diffusion-0.0.3/pymle/models/Pearson.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/PeralVerhulst.py` & `pymle-diffusion-0.0.3/pymle/models/PeralVerhulst.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/RadialOU.py` & `pymle-diffusion-0.0.3/pymle/models/RadialOU.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/Threehalf.py` & `pymle-diffusion-0.0.3/pymle/models/Threehalf.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/models/__init__.py` & `pymle-diffusion-0.0.3/pymle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/sim/Simulator1D.py` & `pymle-diffusion-0.0.3/pymle/sim/Simulator1D.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle/sim/Stepper.py` & `pymle-diffusion-0.0.3/pymle/sim/Stepper.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/pymle_diffusion.egg-info/PKG-INFO` & `pymle-diffusion-0.0.3/pymle_diffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymle-diffusion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Maximum Likelihood Estimation (MLE) and simulation for SDE
 Home-page: https://github.com/jkirkby3/pymle
 Author: Justin Lars Kirkby
 Author-email: jkirkby33@gmail.com
 License: MIT
 Description: Maximum Likelihood Estimation (MLE) and simulation for Stochastic Differential Equations (SDE)
 Keywords: sde mle maximum likelihood difussion estimation simulation
```

### Comparing `pymle-diffusion-0.0.2/pymle_diffusion.egg-info/SOURCES.txt` & `pymle-diffusion-0.0.3/pymle_diffusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Script_1_For_Submission_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Script_1_For_Submission_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Script_2_For_Submission_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Script_2_For_Submission_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Script_3_For_Submission_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Script_3_For_Submission_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Script_COMBINED_For_Submission_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Script_COMBINED_For_Submission_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_CTMC_Converge_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_CTMC_Converge_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_EffectOfBinning_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_EffectOfBinning_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL2.py` & `pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL2.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Exact_Vs_CTMC_Table_LOCAL3.py` & `pymle-diffusion-0.0.3/scripts/Test_Exact_Vs_CTMC_Table_LOCAL3.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Initial_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_Initial_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Likelihood_Convergence_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_Likelihood_Convergence_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/scripts/Test_Param_Histograms_LOCAL.py` & `pymle-diffusion-0.0.3/scripts/Test_Param_Histograms_LOCAL.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/setup.py` & `pymle-diffusion-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='pymle-diffusion',
-      version='0.0.2',
+      version='0.0.3',
       description='Maximum Likelihood Estimation (MLE) and simulation for SDE',
       long_description='Maximum Likelihood Estimation (MLE) and simulation for '
                        'Stochastic Differential Equations (SDE)',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.7',
@@ -16,17 +16,15 @@
       url='https://github.com/jkirkby3/pymle',
       author='Justin Lars Kirkby',
       author_email='jkirkby33@gmail.com',
       license='MIT',
       packages=find_packages(),
       python_requires=">=3.7",
       install_requires=[
-          'numba~=0.53.1',
-          'seaborn~=0.11.1',
-          'setuptools~=56.0.0',
-          'numpy~=1.20.2',
-          'scipy~=1.6.2',
-          'pandas~=1.2.3',
-          'matplotlib~=3.4.1'
+          'numba',
+          'setuptools',
+          'numpy',
+          'scipy',
+          'pandas',
       ],
       include_package_data=True,
       zip_safe=False)
```

### Comparing `pymle-diffusion-0.0.2/tests/fit/Test_AnalyticalMLE.py` & `pymle-diffusion-0.0.3/tests/fit/Test_AnalyticalMLE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.2/tests/models/Test_CEV.py` & `pymle-diffusion-0.0.3/tests/models/Test_CEV.py`

 * *Files identical despite different names*

