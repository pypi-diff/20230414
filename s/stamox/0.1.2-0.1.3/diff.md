# Comparing `tmp/stamox-0.1.2.tar.gz` & `tmp/stamox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stamox-0.1.2.tar", last modified: Fri Apr 14 06:52:39 2023, max compression
+gzip compressed data, was "stamox-0.1.3.tar", last modified: Fri Apr 14 06:57:37 2023, max compression
```

## Comparing `stamox-0.1.2.tar` & `stamox-0.1.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612581 stamox-0.1.2/
--rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.2/LICENCE
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:52:39.612434 stamox-0.1.2/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     3921 2023-04-10 09:03:02.000000 stamox-0.1.2/README.md
--rw-r--r--   0 jiayaobo   (501) staff       (20)      413 2023-03-28 10:26:52.000000 stamox-0.1.2/pyproject.toml
--rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-14 06:52:39.612618 stamox-0.1.2/setup.cfg
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1121 2023-04-14 06:52:34.000000 stamox-0.1.2/setup.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602023 stamox-0.1.2/stamox/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      610 2023-04-10 07:38:29.000000 stamox-0.1.2/stamox/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602873 stamox-0.1.2/stamox/anova/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       70 2023-03-28 10:30:02.000000 stamox-0.1.2/stamox/anova/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.603131 stamox-0.1.2/stamox/anova/one_way/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.2/stamox/anova/one_way/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4298 2023-04-10 07:41:59.000000 stamox-0.1.2/stamox/anova/one_way/_aov.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-11 10:08:22.000000 stamox-0.1.2/stamox/basic.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.603384 stamox-0.1.2/stamox/cluster/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-10 07:00:50.000000 stamox-0.1.2/stamox/cluster/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5151 2023-04-14 05:37:17.000000 stamox-0.1.2/stamox/cluster/_kmeans.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.604313 stamox-0.1.2/stamox/core/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      630 2023-04-10 07:21:03.000000 stamox-0.1.2/stamox/core/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      231 2023-04-13 16:45:38.000000 stamox-0.1.2/stamox/core/_func_state.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-14 05:56:50.000000 stamox-0.1.2/stamox/core/_utils.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2921 2023-04-14 06:25:15.000000 stamox-0.1.2/stamox/core/base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2324 2023-04-14 06:17:30.000000 stamox-0.1.2/stamox/core/jit.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6174 2023-04-14 06:17:16.000000 stamox-0.1.2/stamox/core/maps.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-14 06:43:29.000000 stamox-0.1.2/stamox/core/pipe.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.607523 stamox-0.1.2/stamox/distribution/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1680 2023-04-13 15:54:20.000000 stamox-0.1.2/stamox/distribution/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6173 2023-04-14 05:36:26.000000 stamox-0.1.2/stamox/distribution/_beta.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5559 2023-04-13 15:59:27.000000 stamox-0.1.2/stamox/distribution/_binomial.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6371 2023-04-13 14:31:34.000000 stamox-0.1.2/stamox/distribution/_cauchy.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5117 2023-04-08 16:53:06.000000 stamox-0.1.2/stamox/distribution/_chisq.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2220 2023-04-08 17:08:44.000000 stamox-0.1.2/stamox/distribution/_ecdf.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5675 2023-04-08 16:55:44.000000 stamox-0.1.2/stamox/distribution/_exp.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5942 2023-04-08 16:57:42.000000 stamox-0.1.2/stamox/distribution/_f.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6307 2023-04-08 16:59:05.000000 stamox-0.1.2/stamox/distribution/_gamma.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      787 2023-03-29 10:43:04.000000 stamox-0.1.2/stamox/distribution/_geom.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6467 2023-04-08 17:01:47.000000 stamox-0.1.2/stamox/distribution/_laplace.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7228 2023-04-08 17:00:17.000000 stamox-0.1.2/stamox/distribution/_normal.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6385 2023-04-08 17:03:09.000000 stamox-0.1.2/stamox/distribution/_pareto.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5449 2023-04-13 15:59:19.000000 stamox-0.1.2/stamox/distribution/_poisson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1067 2023-04-05 14:34:37.000000 stamox-0.1.2/stamox/distribution/_q_discrete_search.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1873 2023-03-29 10:43:29.000000 stamox-0.1.2/stamox/distribution/_rademacher.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6920 2023-04-08 17:04:47.000000 stamox-0.1.2/stamox/distribution/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1144 2023-03-29 10:43:56.000000 stamox-0.1.2/stamox/distribution/_triangular.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6220 2023-04-08 17:06:06.000000 stamox-0.1.2/stamox/distribution/_uniform.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5556 2023-04-08 16:42:13.000000 stamox-0.1.2/stamox/distribution/_weibull.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.607777 stamox-0.1.2/stamox/experimental/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-13 16:31:36.000000 stamox-0.1.2/stamox/experimental/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1351 2023-04-13 16:31:43.000000 stamox-0.1.2/stamox/experimental/better_partial.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608033 stamox-0.1.2/stamox/experimental/decomposition/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-11 10:10:40.000000 stamox-0.1.2/stamox/experimental/decomposition/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-10 07:40:46.000000 stamox-0.1.2/stamox/experimental/decomposition/_pca.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608422 stamox-0.1.2/stamox/experimental/maps/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-11 10:10:44.000000 stamox-0.1.2/stamox/experimental/maps/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-03-27 09:56:00.000000 stamox-0.1.2/stamox/experimental/maps/auto_map.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-03-28 10:31:15.000000 stamox-0.1.2/stamox/experimental/maps/cube_map.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608674 stamox-0.1.2/stamox/experimental/nn/
--rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-12 13:43:28.000000 stamox-0.1.2/stamox/experimental/nn/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608980 stamox-0.1.2/stamox/formula/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-08 13:01:51.000000 stamox-0.1.2/stamox/formula/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1415 2023-04-11 10:10:07.000000 stamox-0.1.2/stamox/formula/_formula.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.610682 stamox-0.1.2/stamox/hypothesis/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      814 2023-04-14 06:42:01.000000 stamox-0.1.2/stamox/hypothesis/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2540 2023-04-14 06:37:22.000000 stamox-0.1.2/stamox/hypothesis/_bartlett.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      734 2023-03-29 10:40:56.000000 stamox-0.1.2/stamox/hypothesis/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2283 2023-04-06 14:56:52.000000 stamox-0.1.2/stamox/hypothesis/_durbin_watson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2740 2023-04-14 06:41:22.000000 stamox-0.1.2/stamox/hypothesis/_friedman.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      806 2023-03-29 10:41:12.000000 stamox-0.1.2/stamox/hypothesis/_p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      837 2023-03-29 10:41:19.000000 stamox-0.1.2/stamox/hypothesis/_pearsonr.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5033 2023-04-14 06:41:48.000000 stamox-0.1.2/stamox/hypothesis/_shapiro_wilk.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      954 2023-03-29 10:41:28.000000 stamox-0.1.2/stamox/hypothesis/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1179 2023-03-21 16:44:14.000000 stamox-0.1.2/stamox/hypothesis/cor2ci.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      485 2023-03-21 16:44:03.000000 stamox-0.1.2/stamox/hypothesis/cor2p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1029 2023-03-16 09:09:37.000000 stamox-0.1.2/stamox/hypothesis/corr.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.611054 stamox-0.1.2/stamox/math/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-10 03:27:30.000000 stamox-0.1.2/stamox/math/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1255 2023-04-10 03:26:51.000000 stamox-0.1.2/stamox/math/combination.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      670 2023-04-05 11:46:28.000000 stamox-0.1.2/stamox/math/special.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.611422 stamox-0.1.2/stamox/regression/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-13 07:01:57.000000 stamox-0.1.2/stamox/regression/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-12 13:26:06.000000 stamox-0.1.2/stamox/regression/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7062 2023-04-10 10:29:07.000000 stamox-0.1.2/stamox/regression/_lm.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612014 stamox-0.1.2/stamox/sample/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      343 2023-04-14 06:48:40.000000 stamox-0.1.2/stamox/sample/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2835 2023-04-09 14:28:45.000000 stamox-0.1.2/stamox/sample/_bootstrap.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1821 2023-04-14 06:48:11.000000 stamox-0.1.2/stamox/sample/_jackknife.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      888 2023-04-10 09:45:17.000000 stamox-0.1.2/stamox/transformation.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602723 stamox-0.1.2/stamox.egg-info/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2133 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/SOURCES.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/dependency_links.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)      385 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/requires.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/top_level.txt
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612185 stamox-0.1.2/tests/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1747 2023-04-08 15:17:53.000000 stamox-0.1.2/tests/test_basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.277423 stamox-0.1.3/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.3/LICENCE
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:57:37.277289 stamox-0.1.3/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     3921 2023-04-10 09:03:02.000000 stamox-0.1.3/README.md
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      413 2023-03-28 10:26:52.000000 stamox-0.1.3/pyproject.toml
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-14 06:57:37.277465 stamox-0.1.3/setup.cfg
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1121 2023-04-14 06:56:34.000000 stamox-0.1.3/setup.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.266378 stamox-0.1.3/stamox/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      610 2023-04-10 07:38:29.000000 stamox-0.1.3/stamox/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267207 stamox-0.1.3/stamox/anova/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       70 2023-03-28 10:30:02.000000 stamox-0.1.3/stamox/anova/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267508 stamox-0.1.3/stamox/anova/one_way/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.3/stamox/anova/one_way/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4298 2023-04-10 07:41:59.000000 stamox-0.1.3/stamox/anova/one_way/_aov.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-11 10:08:22.000000 stamox-0.1.3/stamox/basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267790 stamox-0.1.3/stamox/cluster/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-10 07:00:50.000000 stamox-0.1.3/stamox/cluster/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5151 2023-04-14 05:37:17.000000 stamox-0.1.3/stamox/cluster/_kmeans.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.268741 stamox-0.1.3/stamox/core/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      630 2023-04-10 07:21:03.000000 stamox-0.1.3/stamox/core/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      231 2023-04-13 16:45:38.000000 stamox-0.1.3/stamox/core/_func_state.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-14 05:56:50.000000 stamox-0.1.3/stamox/core/_utils.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2921 2023-04-14 06:25:15.000000 stamox-0.1.3/stamox/core/base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2324 2023-04-14 06:17:30.000000 stamox-0.1.3/stamox/core/jit.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6336 2023-04-14 06:56:15.000000 stamox-0.1.3/stamox/core/maps.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-14 06:43:29.000000 stamox-0.1.3/stamox/core/pipe.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272202 stamox-0.1.3/stamox/distribution/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1680 2023-04-13 15:54:20.000000 stamox-0.1.3/stamox/distribution/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6173 2023-04-14 05:36:26.000000 stamox-0.1.3/stamox/distribution/_beta.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5559 2023-04-13 15:59:27.000000 stamox-0.1.3/stamox/distribution/_binomial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6371 2023-04-13 14:31:34.000000 stamox-0.1.3/stamox/distribution/_cauchy.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5117 2023-04-08 16:53:06.000000 stamox-0.1.3/stamox/distribution/_chisq.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2220 2023-04-08 17:08:44.000000 stamox-0.1.3/stamox/distribution/_ecdf.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5675 2023-04-08 16:55:44.000000 stamox-0.1.3/stamox/distribution/_exp.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5942 2023-04-08 16:57:42.000000 stamox-0.1.3/stamox/distribution/_f.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6307 2023-04-08 16:59:05.000000 stamox-0.1.3/stamox/distribution/_gamma.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      787 2023-03-29 10:43:04.000000 stamox-0.1.3/stamox/distribution/_geom.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6467 2023-04-08 17:01:47.000000 stamox-0.1.3/stamox/distribution/_laplace.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7228 2023-04-08 17:00:17.000000 stamox-0.1.3/stamox/distribution/_normal.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6385 2023-04-08 17:03:09.000000 stamox-0.1.3/stamox/distribution/_pareto.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5449 2023-04-13 15:59:19.000000 stamox-0.1.3/stamox/distribution/_poisson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1067 2023-04-05 14:34:37.000000 stamox-0.1.3/stamox/distribution/_q_discrete_search.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1873 2023-03-29 10:43:29.000000 stamox-0.1.3/stamox/distribution/_rademacher.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6920 2023-04-08 17:04:47.000000 stamox-0.1.3/stamox/distribution/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1144 2023-03-29 10:43:56.000000 stamox-0.1.3/stamox/distribution/_triangular.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6220 2023-04-08 17:06:06.000000 stamox-0.1.3/stamox/distribution/_uniform.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5556 2023-04-08 16:42:13.000000 stamox-0.1.3/stamox/distribution/_weibull.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272503 stamox-0.1.3/stamox/experimental/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-13 16:31:36.000000 stamox-0.1.3/stamox/experimental/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1351 2023-04-13 16:31:43.000000 stamox-0.1.3/stamox/experimental/better_partial.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.272823 stamox-0.1.3/stamox/experimental/decomposition/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-11 10:10:40.000000 stamox-0.1.3/stamox/experimental/decomposition/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-10 07:40:46.000000 stamox-0.1.3/stamox/experimental/decomposition/_pca.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273249 stamox-0.1.3/stamox/experimental/maps/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-11 10:10:44.000000 stamox-0.1.3/stamox/experimental/maps/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-03-27 09:56:00.000000 stamox-0.1.3/stamox/experimental/maps/auto_map.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-03-28 10:31:15.000000 stamox-0.1.3/stamox/experimental/maps/cube_map.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273381 stamox-0.1.3/stamox/experimental/nn/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-12 13:43:28.000000 stamox-0.1.3/stamox/experimental/nn/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.273620 stamox-0.1.3/stamox/formula/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-08 13:01:51.000000 stamox-0.1.3/stamox/formula/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1415 2023-04-11 10:10:07.000000 stamox-0.1.3/stamox/formula/_formula.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.275451 stamox-0.1.3/stamox/hypothesis/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      814 2023-04-14 06:42:01.000000 stamox-0.1.3/stamox/hypothesis/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2540 2023-04-14 06:37:22.000000 stamox-0.1.3/stamox/hypothesis/_bartlett.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      734 2023-03-29 10:40:56.000000 stamox-0.1.3/stamox/hypothesis/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2283 2023-04-06 14:56:52.000000 stamox-0.1.3/stamox/hypothesis/_durbin_watson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2740 2023-04-14 06:41:22.000000 stamox-0.1.3/stamox/hypothesis/_friedman.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      806 2023-03-29 10:41:12.000000 stamox-0.1.3/stamox/hypothesis/_p.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      837 2023-03-29 10:41:19.000000 stamox-0.1.3/stamox/hypothesis/_pearsonr.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5033 2023-04-14 06:41:48.000000 stamox-0.1.3/stamox/hypothesis/_shapiro_wilk.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      954 2023-03-29 10:41:28.000000 stamox-0.1.3/stamox/hypothesis/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1179 2023-03-21 16:44:14.000000 stamox-0.1.3/stamox/hypothesis/cor2ci.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      485 2023-03-21 16:44:03.000000 stamox-0.1.3/stamox/hypothesis/cor2p.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1029 2023-03-16 09:09:37.000000 stamox-0.1.3/stamox/hypothesis/corr.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276003 stamox-0.1.3/stamox/math/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-10 03:27:30.000000 stamox-0.1.3/stamox/math/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1255 2023-04-10 03:26:51.000000 stamox-0.1.3/stamox/math/combination.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      670 2023-04-05 11:46:28.000000 stamox-0.1.3/stamox/math/special.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276503 stamox-0.1.3/stamox/regression/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-13 07:01:57.000000 stamox-0.1.3/stamox/regression/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-12 13:26:06.000000 stamox-0.1.3/stamox/regression/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7062 2023-04-10 10:29:07.000000 stamox-0.1.3/stamox/regression/_lm.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.276908 stamox-0.1.3/stamox/sample/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      343 2023-04-14 06:48:40.000000 stamox-0.1.3/stamox/sample/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2835 2023-04-09 14:28:45.000000 stamox-0.1.3/stamox/sample/_bootstrap.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1821 2023-04-14 06:48:11.000000 stamox-0.1.3/stamox/sample/_jackknife.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      888 2023-04-10 09:45:17.000000 stamox-0.1.3/stamox/transformation.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.267053 stamox-0.1.3/stamox.egg-info/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2133 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      385 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/requires.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-14 06:57:37.000000 stamox-0.1.3/stamox.egg-info/top_level.txt
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:57:37.277044 stamox-0.1.3/tests/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1747 2023-04-08 15:17:53.000000 stamox-0.1.3/tests/test_basic.py
```

### Comparing `stamox-0.1.2/LICENCE` & `stamox-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/PKG-INFO` & `stamox-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `stamox-0.1.2/README.md` & `stamox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/setup.py` & `stamox-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 PACKAGE_NAME = "stamox"
 AUTHOR = "Jia Yaobo"
 URL = "https://github.com/jiayaobo/stamox"
 
 LICENSE = "Apache 2.0"
 DESCRIPTION = "Accelerate Your Statistical Analysis with JAX."
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
```

### Comparing `stamox-0.1.2/stamox/__init__.py` & `stamox-0.1.3/stamox/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/anova/one_way/_aov.py` & `stamox-0.1.3/stamox/anova/one_way/_aov.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/basic.py` & `stamox-0.1.3/stamox/basic.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/cluster/_kmeans.py` & `stamox-0.1.3/stamox/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/core/__init__.py` & `stamox-0.1.3/stamox/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/core/base.py` & `stamox-0.1.3/stamox/core/base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/core/jit.py` & `stamox-0.1.3/stamox/core/jit.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/core/maps.py` & `stamox-0.1.3/stamox/core/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,18 @@
         >>> f = lambda x: x + 1
         >>> f = pipe_vmap(f)
         >>> g = f >> f >> f
         >>> g(jnp.array([1, 2, 3]))
         Array([4, 5, 6], dtype=int32)
     """
     if name is None and func is not None:
-        name = func.__name__
+        if hasattr(func, "name"):
+            name = func.name
+        else:
+            name = func.__name__
 
     @wraps(func)
     def wrap(func: Callable[P, T]) -> Callable:
         if isinstance(func, Functional):
             func = func.func
         fn = filter_vmap(
             func,
@@ -77,15 +80,18 @@
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_vmap(f)
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(jnp.array([1, 2, 3]))
         Array([7, 8, 9], dtype=int32)
     """
     if name is None and func is not None:
-        name = func.__name__
+        if hasattr(func, "name"):
+            name = func.name
+        else:
+            name = func.__name__
 
     @wraps(func)
     def wrap(func: Callable[P, T]) -> Callable:
         if isinstance(func, Functional):
             func = func.func
 
         @wraps(func)
```

### Comparing `stamox-0.1.2/stamox/core/pipe.py` & `stamox-0.1.3/stamox/core/pipe.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/__init__.py` & `stamox-0.1.3/stamox/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_beta.py` & `stamox-0.1.3/stamox/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_binomial.py` & `stamox-0.1.3/stamox/distribution/_binomial.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_cauchy.py` & `stamox-0.1.3/stamox/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_chisq.py` & `stamox-0.1.3/stamox/distribution/_chisq.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_ecdf.py` & `stamox-0.1.3/stamox/distribution/_ecdf.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_exp.py` & `stamox-0.1.3/stamox/distribution/_exp.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_f.py` & `stamox-0.1.3/stamox/distribution/_f.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_gamma.py` & `stamox-0.1.3/stamox/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_geom.py` & `stamox-0.1.3/stamox/distribution/_geom.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_laplace.py` & `stamox-0.1.3/stamox/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_normal.py` & `stamox-0.1.3/stamox/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_pareto.py` & `stamox-0.1.3/stamox/distribution/_pareto.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_poisson.py` & `stamox-0.1.3/stamox/distribution/_poisson.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_q_discrete_search.py` & `stamox-0.1.3/stamox/distribution/_q_discrete_search.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_rademacher.py` & `stamox-0.1.3/stamox/distribution/_rademacher.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_t.py` & `stamox-0.1.3/stamox/distribution/_t.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_triangular.py` & `stamox-0.1.3/stamox/distribution/_triangular.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_uniform.py` & `stamox-0.1.3/stamox/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/distribution/_weibull.py` & `stamox-0.1.3/stamox/distribution/_weibull.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/experimental/better_partial.py` & `stamox-0.1.3/stamox/experimental/better_partial.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/experimental/decomposition/_pca.py` & `stamox-0.1.3/stamox/experimental/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/experimental/maps/auto_map.py` & `stamox-0.1.3/stamox/experimental/maps/auto_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/experimental/maps/cube_map.py` & `stamox-0.1.3/stamox/experimental/maps/cube_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/formula/_formula.py` & `stamox-0.1.3/stamox/formula/_formula.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/__init__.py` & `stamox-0.1.3/stamox/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_bartlett.py` & `stamox-0.1.3/stamox/hypothesis/_bartlett.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_base.py` & `stamox-0.1.3/stamox/hypothesis/_base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_durbin_watson.py` & `stamox-0.1.3/stamox/hypothesis/_durbin_watson.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_friedman.py` & `stamox-0.1.3/stamox/hypothesis/_friedman.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_p.py` & `stamox-0.1.3/stamox/hypothesis/_p.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_pearsonr.py` & `stamox-0.1.3/stamox/hypothesis/_pearsonr.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_shapiro_wilk.py` & `stamox-0.1.3/stamox/hypothesis/_shapiro_wilk.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/_t.py` & `stamox-0.1.3/stamox/hypothesis/_t.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/cor2ci.py` & `stamox-0.1.3/stamox/hypothesis/cor2ci.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/hypothesis/corr.py` & `stamox-0.1.3/stamox/hypothesis/corr.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/math/combination.py` & `stamox-0.1.3/stamox/math/combination.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/math/special.py` & `stamox-0.1.3/stamox/math/special.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/regression/_base.py` & `stamox-0.1.3/stamox/regression/_base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/regression/_lm.py` & `stamox-0.1.3/stamox/regression/_lm.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/sample/_bootstrap.py` & `stamox-0.1.3/stamox/sample/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/sample/_jackknife.py` & `stamox-0.1.3/stamox/sample/_jackknife.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox/transformation.py` & `stamox-0.1.3/stamox/transformation.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/stamox.egg-info/PKG-INFO` & `stamox-0.1.3/stamox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `stamox-0.1.2/stamox.egg-info/SOURCES.txt` & `stamox-0.1.3/stamox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stamox-0.1.2/tests/test_basic.py` & `stamox-0.1.3/tests/test_basic.py`

 * *Files identical despite different names*

