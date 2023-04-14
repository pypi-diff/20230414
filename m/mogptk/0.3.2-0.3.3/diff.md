# Comparing `tmp/mogptk-0.3.2.tar.gz` & `tmp/mogptk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mogptk-0.3.2.tar", last modified: Thu Dec 29 16:02:50 2022, max compression
+gzip compressed data, was "mogptk-0.3.3.tar", last modified: Fri Apr 14 14:08:24 2023, max compression
```

## Comparing `mogptk-0.3.2.tar` & `mogptk-0.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2022-12-29 16:02:50.743573 mogptk-0.3.2/
--rw-r--r--   0 taco      (1000) users      (100)      115 2022-04-24 22:51:10.000000 mogptk-0.3.2/.gitignore
--rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.3.2/LICENSE
--rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.3.2/MANIFEST.in
--rw-r--r--   0 taco      (1000) users      (100)    10631 2022-12-29 16:02:50.743573 mogptk-0.3.2/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)    10230 2022-07-17 20:41:27.000000 mogptk-0.3.2/README.md
--rwxr-xr-x   0 taco      (1000) users      (100)       99 2022-06-01 13:42:52.000000 mogptk-0.3.2/build.sh
--rwxr-xr-x   0 taco      (1000) users      (100)     1083 2022-07-14 17:48:19.000000 mogptk-0.3.2/build_docs.sh
--rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.3.2/config.mako
--rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.3.2/head.mako
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2022-12-29 16:02:50.740240 mogptk-0.3.2/mogptk/
--rw-r--r--   0 taco      (1000) users      (100)      360 2022-06-28 22:19:05.000000 mogptk-0.3.2/mogptk/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)    56121 2022-06-28 23:33:16.000000 mogptk-0.3.2/mogptk/data.py
--rw-r--r--   0 taco      (1000) users      (100)    29065 2022-05-26 18:32:31.000000 mogptk-0.3.2/mogptk/dataset.py
--rw-r--r--   0 taco      (1000) users      (100)     7226 2022-05-12 16:46:24.000000 mogptk-0.3.2/mogptk/documentation.md
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2022-12-29 16:02:50.743573 mogptk-0.3.2/mogptk/gpr/
--rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.3.2/mogptk/gpr/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     2738 2022-05-10 02:07:17.000000 mogptk-0.3.2/mogptk/gpr/config.py
--rw-r--r--   0 taco      (1000) users      (100)    16624 2022-06-28 22:03:02.000000 mogptk-0.3.2/mogptk/gpr/kernel.py
--rw-r--r--   0 taco      (1000) users      (100)    26313 2022-06-14 15:18:49.000000 mogptk-0.3.2/mogptk/gpr/likelihood.py
--rw-r--r--   0 taco      (1000) users      (100)     3119 2022-08-02 19:14:49.000000 mogptk-0.3.2/mogptk/gpr/mean.py
--rw-r--r--   0 taco      (1000) users      (100)    38750 2022-07-05 15:26:39.000000 mogptk-0.3.2/mogptk/gpr/model.py
--rw-r--r--   0 taco      (1000) users      (100)    29785 2022-12-29 15:57:38.000000 mogptk-0.3.2/mogptk/gpr/multioutput.py
--rw-r--r--   0 taco      (1000) users      (100)    10377 2022-05-21 17:05:07.000000 mogptk-0.3.2/mogptk/gpr/parameter.py
--rw-r--r--   0 taco      (1000) users      (100)     1271 2022-07-05 15:23:28.000000 mogptk-0.3.2/mogptk/gpr/plot.py
--rw-r--r--   0 taco      (1000) users      (100)    29625 2022-06-28 22:33:08.000000 mogptk-0.3.2/mogptk/gpr/singleoutput.py
--rw-r--r--   0 taco      (1000) users      (100)     2451 2022-05-09 21:37:57.000000 mogptk-0.3.2/mogptk/gpr/util.py
--rw-r--r--   0 taco      (1000) users      (100)     5701 2022-05-26 16:06:50.000000 mogptk-0.3.2/mogptk/init.py
--rw-r--r--   0 taco      (1000) users      (100)    41031 2022-12-29 15:56:59.000000 mogptk-0.3.2/mogptk/model.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2022-12-29 16:02:50.743573 mogptk-0.3.2/mogptk/models/
--rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.3.2/mogptk/models/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     4693 2022-12-29 15:58:20.000000 mogptk-0.3.2/mogptk/models/conv.py
--rw-r--r--   0 taco      (1000) users      (100)     5113 2022-12-29 15:58:44.000000 mogptk-0.3.2/mogptk/models/csm.py
--rw-r--r--   0 taco      (1000) users      (100)     7226 2022-12-29 15:58:53.000000 mogptk-0.3.2/mogptk/models/mohsm.py
--rw-r--r--   0 taco      (1000) users      (100)    12081 2022-12-29 15:59:00.000000 mogptk-0.3.2/mogptk/models/mosm.py
--rw-r--r--   0 taco      (1000) users      (100)     7516 2022-12-29 15:59:17.000000 mogptk-0.3.2/mogptk/models/sm.py
--rw-r--r--   0 taco      (1000) users      (100)     5551 2022-12-29 15:59:09.000000 mogptk-0.3.2/mogptk/models/sm_lmc.py
--rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.3.2/mogptk/transformer.py
--rw-r--r--   0 taco      (1000) users      (100)    10128 2022-05-31 15:51:52.000000 mogptk-0.3.2/mogptk/util.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2022-12-29 16:02:50.743573 mogptk-0.3.2/mogptk.egg-info/
--rw-r--r--   0 taco      (1000) users      (100)    10631 2022-12-29 16:02:50.000000 mogptk-0.3.2/mogptk.egg-info/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)      810 2022-12-29 16:02:50.000000 mogptk-0.3.2/mogptk.egg-info/SOURCES.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2022-12-29 16:02:50.000000 mogptk-0.3.2/mogptk.egg-info/dependency_links.txt
--rw-r--r--   0 taco      (1000) users      (100)       74 2022-12-29 16:02:50.000000 mogptk-0.3.2/mogptk.egg-info/requires.txt
--rw-r--r--   0 taco      (1000) users      (100)        7 2022-12-29 16:02:50.000000 mogptk-0.3.2/mogptk.egg-info/top_level.txt
--rwxr-xr-x   0 taco      (1000) users      (100)       36 2020-01-27 19:27:01.000000 mogptk-0.3.2/publish.sh
--rw-r--r--   0 taco      (1000) users      (100)       79 2022-12-29 16:02:50.746907 mogptk-0.3.2/setup.cfg
--rw-r--r--   0 taco      (1000) users      (100)      944 2022-12-29 16:00:29.000000 mogptk-0.3.2/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/
+-rw-r--r--   0 taco      (1000) users      (100)      115 2022-04-24 22:51:10.000000 mogptk-0.3.3/.gitignore
+-rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.3.3/LICENSE
+-rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.3.3/MANIFEST.in
+-rw-r--r--   0 taco      (1000) users      (100)    10833 2023-04-14 14:08:24.656745 mogptk-0.3.3/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)    10432 2023-03-31 14:19:49.000000 mogptk-0.3.3/README.md
+-rwxr-xr-x   0 taco      (1000) users      (100)       99 2022-06-01 13:42:52.000000 mogptk-0.3.3/build.sh
+-rwxr-xr-x   0 taco      (1000) users      (100)     1083 2022-07-14 17:48:19.000000 mogptk-0.3.3/build_docs.sh
+-rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.3.3/config.mako
+-rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.3.3/head.mako
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.653412 mogptk-0.3.3/mogptk/
+-rw-r--r--   0 taco      (1000) users      (100)      360 2022-06-28 22:19:05.000000 mogptk-0.3.3/mogptk/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)    56121 2022-06-28 23:33:16.000000 mogptk-0.3.3/mogptk/data.py
+-rw-r--r--   0 taco      (1000) users      (100)    29065 2022-05-26 18:32:31.000000 mogptk-0.3.3/mogptk/dataset.py
+-rw-r--r--   0 taco      (1000) users      (100)     7226 2022-05-12 16:46:24.000000 mogptk-0.3.3/mogptk/documentation.md
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/mogptk/gpr/
+-rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.3.3/mogptk/gpr/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     2738 2022-05-10 02:07:17.000000 mogptk-0.3.3/mogptk/gpr/config.py
+-rw-r--r--   0 taco      (1000) users      (100)    16624 2022-06-28 22:03:02.000000 mogptk-0.3.3/mogptk/gpr/kernel.py
+-rw-r--r--   0 taco      (1000) users      (100)    26313 2022-06-14 15:18:49.000000 mogptk-0.3.3/mogptk/gpr/likelihood.py
+-rw-r--r--   0 taco      (1000) users      (100)     3119 2022-08-02 19:14:49.000000 mogptk-0.3.3/mogptk/gpr/mean.py
+-rw-r--r--   0 taco      (1000) users      (100)    38753 2023-03-22 02:23:05.000000 mogptk-0.3.3/mogptk/gpr/model.py
+-rw-r--r--   0 taco      (1000) users      (100)    29785 2022-12-29 15:57:38.000000 mogptk-0.3.3/mogptk/gpr/multioutput.py
+-rw-r--r--   0 taco      (1000) users      (100)    10377 2022-05-21 17:05:07.000000 mogptk-0.3.3/mogptk/gpr/parameter.py
+-rw-r--r--   0 taco      (1000) users      (100)     1209 2023-03-22 02:14:00.000000 mogptk-0.3.3/mogptk/gpr/plot.py
+-rw-r--r--   0 taco      (1000) users      (100)    29625 2022-06-28 22:33:08.000000 mogptk-0.3.3/mogptk/gpr/singleoutput.py
+-rw-r--r--   0 taco      (1000) users      (100)     2451 2022-05-09 21:37:57.000000 mogptk-0.3.3/mogptk/gpr/util.py
+-rw-r--r--   0 taco      (1000) users      (100)     5701 2023-03-22 02:04:42.000000 mogptk-0.3.3/mogptk/init.py
+-rw-r--r--   0 taco      (1000) users      (100)    41046 2023-03-28 15:50:48.000000 mogptk-0.3.3/mogptk/model.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/mogptk/models/
+-rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.3.3/mogptk/models/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     4693 2022-12-29 15:58:20.000000 mogptk-0.3.3/mogptk/models/conv.py
+-rw-r--r--   0 taco      (1000) users      (100)     5113 2022-12-29 15:58:44.000000 mogptk-0.3.3/mogptk/models/csm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7226 2022-12-29 15:58:53.000000 mogptk-0.3.3/mogptk/models/mohsm.py
+-rw-r--r--   0 taco      (1000) users      (100)    12081 2022-12-29 15:59:00.000000 mogptk-0.3.3/mogptk/models/mosm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7516 2022-12-29 15:59:17.000000 mogptk-0.3.3/mogptk/models/sm.py
+-rw-r--r--   0 taco      (1000) users      (100)     5551 2022-12-29 15:59:09.000000 mogptk-0.3.3/mogptk/models/sm_lmc.py
+-rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.3.3/mogptk/transformer.py
+-rw-r--r--   0 taco      (1000) users      (100)    10128 2022-05-31 15:51:52.000000 mogptk-0.3.3/mogptk/util.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.653412 mogptk-0.3.3/mogptk.egg-info/
+-rw-r--r--   0 taco      (1000) users      (100)    10833 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)      810 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/SOURCES.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/dependency_links.txt
+-rw-r--r--   0 taco      (1000) users      (100)       74 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/requires.txt
+-rw-r--r--   0 taco      (1000) users      (100)        7 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/top_level.txt
+-rwxr-xr-x   0 taco      (1000) users      (100)       36 2020-01-27 19:27:01.000000 mogptk-0.3.3/publish.sh
+-rw-r--r--   0 taco      (1000) users      (100)       79 2023-04-14 14:08:24.656745 mogptk-0.3.3/setup.cfg
+-rw-r--r--   0 taco      (1000) users      (100)      944 2023-04-14 14:07:40.000000 mogptk-0.3.3/setup.py
```

### Comparing `mogptk-0.3.2/LICENSE` & `mogptk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/PKG-INFO` & `mogptk-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
@@ -148,14 +148,15 @@
 - [O.A. Guerrero, G. Castañeda, How Does Government Expenditure Impact Sustainable Development? Studying the Multidimensional Link between Budgets and Development Gaps](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3800218)
 - [T.V. Vo, et al., Federated Estimation of Causal Effects from Observational Data](https://arxiv.org/abs/2106.00456)
 - [Q. Lin, et al., Multi-output Gaussian process prediction for computationally expensive problems with multiple levels of fidelity](https://www.sciencedirect.com/science/article/pii/S0950705121004147?casa_token=9CDCb7EpGKUAAAAA:nn6LhsAIYn0b5o9JkRJgz4GlPY4pAYeKz-Xchf-1yxJ5czbLLw7jaBQRF3IXtcs6M1fUYkT0aEI)
 - [S. Covino, et al., Detecting the periodicity of highly irregularly sampled light-curves with GPs](https://arxiv.org/abs/2203.03614)
 - [Y. Jung, J. Park, Scalable Inference for Hybrid Bayesian HMM using GP Emission](https://www.tandfonline.com/doi/abs/10.1080/10618600.2021.2023021)
 - [H. Liu, et al., Scalable multi-task GPs with neural embedding of coregionalization](https://www.sciencedirect.com/science/article/abs/pii/S0950705122003641)
 - [L.M. Rivera-Muñoz, et al., Missing Data Estimation in a Low-Cost Sensor network for Measuring Air Quality](https://link.springer.com/article/10.1007/s11270-021-05363-1)
+- [G. Caballero, et al., Synergy of Sentinel-1 and Sentinel-2 Time Series for Cloud-Free Vegetation Water Content Mapping with Multi-Output Gaussian Processes](https://www.mdpi.com/2072-4292/15/7/1822)
 
 ### Used in code
 - https://github.com/jdjmoon/TRF
 - https://github.com/ErickRosete/Multivariate_regression
 - https://github.com/clara-risk/fire_weather_interpolate
 - https://github.com/becre2021/multichannels-corrnp
 - https://github.com/ArthurLeroy/MAGMAclust
```

### Comparing `mogptk-0.3.2/README.md` & `mogptk-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 - [O.A. Guerrero, G. Castañeda, How Does Government Expenditure Impact Sustainable Development? Studying the Multidimensional Link between Budgets and Development Gaps](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3800218)
 - [T.V. Vo, et al., Federated Estimation of Causal Effects from Observational Data](https://arxiv.org/abs/2106.00456)
 - [Q. Lin, et al., Multi-output Gaussian process prediction for computationally expensive problems with multiple levels of fidelity](https://www.sciencedirect.com/science/article/pii/S0950705121004147?casa_token=9CDCb7EpGKUAAAAA:nn6LhsAIYn0b5o9JkRJgz4GlPY4pAYeKz-Xchf-1yxJ5czbLLw7jaBQRF3IXtcs6M1fUYkT0aEI)
 - [S. Covino, et al., Detecting the periodicity of highly irregularly sampled light-curves with GPs](https://arxiv.org/abs/2203.03614)
 - [Y. Jung, J. Park, Scalable Inference for Hybrid Bayesian HMM using GP Emission](https://www.tandfonline.com/doi/abs/10.1080/10618600.2021.2023021)
 - [H. Liu, et al., Scalable multi-task GPs with neural embedding of coregionalization](https://www.sciencedirect.com/science/article/abs/pii/S0950705122003641)
 - [L.M. Rivera-Muñoz, et al., Missing Data Estimation in a Low-Cost Sensor network for Measuring Air Quality](https://link.springer.com/article/10.1007/s11270-021-05363-1)
+- [G. Caballero, et al., Synergy of Sentinel-1 and Sentinel-2 Time Series for Cloud-Free Vegetation Water Content Mapping with Multi-Output Gaussian Processes](https://www.mdpi.com/2072-4292/15/7/1822)
 
 ### Used in code
 - https://github.com/jdjmoon/TRF
 - https://github.com/ErickRosete/Multivariate_regression
 - https://github.com/clara-risk/fire_weather_interpolate
 - https://github.com/becre2021/multichannels-corrnp
 - https://github.com/ArthurLeroy/MAGMAclust
```

### Comparing `mogptk-0.3.2/build_docs.sh` & `mogptk-0.3.3/build_docs.sh`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/config.mako` & `mogptk-0.3.3/config.mako`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/data.py` & `mogptk-0.3.3/mogptk/data.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/dataset.py` & `mogptk-0.3.3/mogptk/dataset.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/documentation.md` & `mogptk-0.3.3/mogptk/documentation.md`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/config.py` & `mogptk-0.3.3/mogptk/gpr/config.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/kernel.py` & `mogptk-0.3.3/mogptk/gpr/kernel.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/likelihood.py` & `mogptk-0.3.3/mogptk/gpr/likelihood.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/mean.py` & `mogptk-0.3.3/mogptk/gpr/mean.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/model.py` & `mogptk-0.3.3/mogptk/gpr/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         rangeWidth = max([len(val[1]) for val in vals])
         for val in vals:
             #print("%-*s  %-*s  %s" % (nameWidth, val[0], rangeWidth, val[1], val[2]), file=file)
             print("%-*s  %s" % (nameWidth, val[0], val[2]), file=file)
 
     def _cholesky(self, K, add_jitter=False):
         if add_jitter:
-            K += (self.jitter * K.diagonal().mean()).repeat(K.shape[0]).diagflat()
+            K = K + (self.jitter * K.diagonal().mean()).repeat(K.shape[0]).diagflat()
         try:
             return torch.linalg.cholesky(K)
         except RuntimeError as e:
             print("ERROR:", e.args[0], file=sys.__stdout__)
             if K.isnan().any():
                 print("ERROR: kernel matrix has NaNs!", file=sys.__stdout__)
             if K.isinf().any():
```

### Comparing `mogptk-0.3.2/mogptk/gpr/multioutput.py` & `mogptk-0.3.3/mogptk/gpr/multioutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/parameter.py` & `mogptk-0.3.3/mogptk/gpr/parameter.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/plot.py` & `mogptk-0.3.3/mogptk/gpr/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-import warnings
-warnings.simplefilter('ignore', UserWarning)
-
 def plot_gram(K):
     fig, ax = plt.subplots(1, 1, figsize=(6,6))
     fig.suptitle('Matrix is not positive semi-definitive', fontsize=16)
 
     K = K.detach().cpu().numpy()
     K_real = K[~np.isnan(K) & ~np.isinf(K)]
     if len(K_real) != 0:
```

### Comparing `mogptk-0.3.2/mogptk/gpr/singleoutput.py` & `mogptk-0.3.3/mogptk/gpr/singleoutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/gpr/util.py` & `mogptk-0.3.3/mogptk/gpr/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/init.py` & `mogptk-0.3.3/mogptk/init.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/model.py` & `mogptk-0.3.3/mogptk/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,16 +112,16 @@
     def __init__(self, inducing_points=10, init_inducing_points='grid', variance=None, jitter=1e-6):
         self.inducing_points = inducing_points
         self.init_inducing_points = init_inducing_points
         self.variance = variance
         self.jitter = jitter
 
     def _build(self, kernel, x, y, y_err=None, mean=None, name=None):
-        if variance is None:
-            variance = [1.0] * kernel.output_dims
+        if self.variance is None:
+            self.variance = [1.0] * kernel.output_dims
         return gpr.Snelson(kernel, x, y, Z=self.inducing_points, Z_init=self.init_inducing_points, variance=self.variance, jitter=self.jitter, mean=mean, name=name)
 
 class OpperArchambeau:
     """
     Inference using Opper and Archambeau 2009 for Gaussian process regression.
 
     Args:
@@ -129,15 +129,15 @@
         jitter (float): Jitter added before calculating a Cholesky.
     """
     def __init__(self, likelihood=gpr.GaussianLikelihood(1.0), jitter=1e-6):
         self.likelihood = likelihood
         self.jitter = jitter
 
     def _build(self, kernel, x, y, y_err=None, mean=None, name=None):
-        return gpr.OpperArchambeau(kernel, x, y, likelihood=likelihood, jitter=self.jitter, mean=mean, name=name)
+        return gpr.OpperArchambeau(kernel, x, y, likelihood=self.likelihood, jitter=self.jitter, mean=mean, name=name)
 
 class Titsias:
     """
     Inference using Titsias 2009 for Gaussian process regression.
 
     Args:
         inducing_points (int,list): Number of inducing points or the locations of the inducing points.
```

### Comparing `mogptk-0.3.2/mogptk/models/conv.py` & `mogptk-0.3.3/mogptk/models/conv.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/models/csm.py` & `mogptk-0.3.3/mogptk/models/csm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/models/mohsm.py` & `mogptk-0.3.3/mogptk/models/mohsm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/models/mosm.py` & `mogptk-0.3.3/mogptk/models/mosm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/models/sm.py` & `mogptk-0.3.3/mogptk/models/sm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/models/sm_lmc.py` & `mogptk-0.3.3/mogptk/models/sm_lmc.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/transformer.py` & `mogptk-0.3.3/mogptk/transformer.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk/util.py` & `mogptk-0.3.3/mogptk/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/mogptk.egg-info/PKG-INFO` & `mogptk-0.3.3/mogptk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
@@ -148,14 +148,15 @@
 - [O.A. Guerrero, G. Castañeda, How Does Government Expenditure Impact Sustainable Development? Studying the Multidimensional Link between Budgets and Development Gaps](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3800218)
 - [T.V. Vo, et al., Federated Estimation of Causal Effects from Observational Data](https://arxiv.org/abs/2106.00456)
 - [Q. Lin, et al., Multi-output Gaussian process prediction for computationally expensive problems with multiple levels of fidelity](https://www.sciencedirect.com/science/article/pii/S0950705121004147?casa_token=9CDCb7EpGKUAAAAA:nn6LhsAIYn0b5o9JkRJgz4GlPY4pAYeKz-Xchf-1yxJ5czbLLw7jaBQRF3IXtcs6M1fUYkT0aEI)
 - [S. Covino, et al., Detecting the periodicity of highly irregularly sampled light-curves with GPs](https://arxiv.org/abs/2203.03614)
 - [Y. Jung, J. Park, Scalable Inference for Hybrid Bayesian HMM using GP Emission](https://www.tandfonline.com/doi/abs/10.1080/10618600.2021.2023021)
 - [H. Liu, et al., Scalable multi-task GPs with neural embedding of coregionalization](https://www.sciencedirect.com/science/article/abs/pii/S0950705122003641)
 - [L.M. Rivera-Muñoz, et al., Missing Data Estimation in a Low-Cost Sensor network for Measuring Air Quality](https://link.springer.com/article/10.1007/s11270-021-05363-1)
+- [G. Caballero, et al., Synergy of Sentinel-1 and Sentinel-2 Time Series for Cloud-Free Vegetation Water Content Mapping with Multi-Output Gaussian Processes](https://www.mdpi.com/2072-4292/15/7/1822)
 
 ### Used in code
 - https://github.com/jdjmoon/TRF
 - https://github.com/ErickRosete/Multivariate_regression
 - https://github.com/clara-risk/fire_weather_interpolate
 - https://github.com/becre2021/multichannels-corrnp
 - https://github.com/ArthurLeroy/MAGMAclust
```

### Comparing `mogptk-0.3.2/mogptk.egg-info/SOURCES.txt` & `mogptk-0.3.3/mogptk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.2/setup.py` & `mogptk-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='mogptk',
-      version='0.3.2',
+      version='0.3.3',
       description='Multi-Output Gaussian Process ToolKit',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/GAMES-UChile/mogptk',
       author='Taco de Wolff, Alejandro Cuevas, Felipe Tobar',
       author_email='tacodewolff@gmail.com',
       license='MIT',
```

