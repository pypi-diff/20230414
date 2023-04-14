# Comparing `tmp/stamox-0.1.0.tar.gz` & `tmp/stamox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stamox-0.1.0.tar", last modified: Mon Apr 10 09:39:25 2023, max compression
+gzip compressed data, was "stamox-0.1.2.tar", last modified: Fri Apr 14 06:52:39 2023, max compression
```

## Comparing `stamox-0.1.0.tar` & `stamox-0.1.2.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.289557 stamox-0.1.0/
--rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.0/LICENCE
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-10 09:39:25.289425 stamox-0.1.0/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     3921 2023-04-10 09:03:02.000000 stamox-0.1.0/README.md
--rw-r--r--   0 jiayaobo   (501) staff       (20)      413 2023-03-28 10:26:52.000000 stamox-0.1.0/pyproject.toml
--rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-10 09:39:25.289600 stamox-0.1.0/setup.cfg
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1109 2023-04-10 09:39:12.000000 stamox-0.1.0/setup.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.280610 stamox-0.1.0/stamox/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      610 2023-04-10 07:38:29.000000 stamox-0.1.0/stamox/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.281449 stamox-0.1.0/stamox/anova/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       70 2023-03-28 10:30:02.000000 stamox-0.1.0/stamox/anova/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.281801 stamox-0.1.0/stamox/anova/one_way/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.0/stamox/anova/one_way/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4298 2023-04-10 07:41:59.000000 stamox-0.1.0/stamox/anova/one_way/_aov.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1176 2023-04-09 14:03:13.000000 stamox-0.1.0/stamox/basic.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.282092 stamox-0.1.0/stamox/cluster/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-10 07:00:50.000000 stamox-0.1.0/stamox/cluster/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5136 2023-04-10 07:47:23.000000 stamox-0.1.0/stamox/cluster/_kmeans.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.283193 stamox-0.1.0/stamox/core/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      630 2023-04-10 07:21:03.000000 stamox-0.1.0/stamox/core/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      342 2023-04-10 07:20:46.000000 stamox-0.1.0/stamox/core/_func_state.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      501 2023-03-29 11:36:31.000000 stamox-0.1.0/stamox/core/_utils.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2913 2023-04-10 07:18:15.000000 stamox-0.1.0/stamox/core/base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2266 2023-04-09 15:21:12.000000 stamox-0.1.0/stamox/core/jit.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6250 2023-04-09 15:21:18.000000 stamox-0.1.0/stamox/core/maps.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6188 2023-04-09 16:12:50.000000 stamox-0.1.0/stamox/core/pipe.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.285615 stamox-0.1.0/stamox/distribution/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1407 2023-04-08 17:07:07.000000 stamox-0.1.0/stamox/distribution/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6173 2023-04-08 16:48:52.000000 stamox-0.1.0/stamox/distribution/_beta.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2125 2023-04-05 12:24:09.000000 stamox-0.1.0/stamox/distribution/_binomial.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6371 2023-04-08 16:51:22.000000 stamox-0.1.0/stamox/distribution/_cauchy.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5117 2023-04-08 16:53:06.000000 stamox-0.1.0/stamox/distribution/_chisq.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2220 2023-04-08 17:08:44.000000 stamox-0.1.0/stamox/distribution/_ecdf.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5675 2023-04-08 16:55:44.000000 stamox-0.1.0/stamox/distribution/_exp.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5942 2023-04-08 16:57:42.000000 stamox-0.1.0/stamox/distribution/_f.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6307 2023-04-08 16:59:05.000000 stamox-0.1.0/stamox/distribution/_gamma.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      787 2023-03-29 10:43:04.000000 stamox-0.1.0/stamox/distribution/_geom.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6467 2023-04-08 17:01:47.000000 stamox-0.1.0/stamox/distribution/_laplace.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7228 2023-04-08 17:00:17.000000 stamox-0.1.0/stamox/distribution/_normal.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6385 2023-04-08 17:03:09.000000 stamox-0.1.0/stamox/distribution/_pareto.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4664 2023-04-08 13:01:51.000000 stamox-0.1.0/stamox/distribution/_poisson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1067 2023-04-05 14:34:37.000000 stamox-0.1.0/stamox/distribution/_q_discrete_search.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1873 2023-03-29 10:43:29.000000 stamox-0.1.0/stamox/distribution/_rademacher.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6920 2023-04-08 17:04:47.000000 stamox-0.1.0/stamox/distribution/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1144 2023-03-29 10:43:56.000000 stamox-0.1.0/stamox/distribution/_triangular.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6220 2023-04-08 17:06:06.000000 stamox-0.1.0/stamox/distribution/_uniform.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5556 2023-04-08 16:42:13.000000 stamox-0.1.0/stamox/distribution/_weibull.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.285745 stamox-0.1.0/stamox/experimental/
--rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-10 07:39:11.000000 stamox-0.1.0/stamox/experimental/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.285983 stamox-0.1.0/stamox/experimental/decomposition/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       48 2023-03-29 10:44:29.000000 stamox-0.1.0/stamox/experimental/decomposition/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-10 07:40:46.000000 stamox-0.1.0/stamox/experimental/decomposition/_pca.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.286357 stamox-0.1.0/stamox/experimental/maps/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-03-28 10:29:23.000000 stamox-0.1.0/stamox/experimental/maps/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-03-27 09:56:00.000000 stamox-0.1.0/stamox/experimental/maps/auto_map.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-03-28 10:31:15.000000 stamox-0.1.0/stamox/experimental/maps/cube_map.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.286608 stamox-0.1.0/stamox/formula/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-08 13:01:51.000000 stamox-0.1.0/stamox/formula/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1414 2023-04-08 15:52:00.000000 stamox-0.1.0/stamox/formula/_formula.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.288050 stamox-0.1.0/stamox/hypothesis/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      553 2023-04-06 15:02:17.000000 stamox-0.1.0/stamox/hypothesis/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     3145 2023-04-06 14:50:06.000000 stamox-0.1.0/stamox/hypothesis/_bartlett.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      734 2023-03-29 10:40:56.000000 stamox-0.1.0/stamox/hypothesis/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2283 2023-04-06 14:56:52.000000 stamox-0.1.0/stamox/hypothesis/_durbin_watson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2776 2023-04-06 14:50:50.000000 stamox-0.1.0/stamox/hypothesis/_friedman.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      806 2023-03-29 10:41:12.000000 stamox-0.1.0/stamox/hypothesis/_p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      837 2023-03-29 10:41:19.000000 stamox-0.1.0/stamox/hypothesis/_pearsonr.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5069 2023-04-06 15:01:55.000000 stamox-0.1.0/stamox/hypothesis/_shapiro_wilk.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      954 2023-03-29 10:41:28.000000 stamox-0.1.0/stamox/hypothesis/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1179 2023-03-21 16:44:14.000000 stamox-0.1.0/stamox/hypothesis/cor2ci.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      485 2023-03-21 16:44:03.000000 stamox-0.1.0/stamox/hypothesis/cor2p.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1029 2023-03-16 09:09:37.000000 stamox-0.1.0/stamox/hypothesis/corr.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.288390 stamox-0.1.0/stamox/math/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-10 03:27:30.000000 stamox-0.1.0/stamox/math/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1255 2023-04-10 03:26:51.000000 stamox-0.1.0/stamox/math/combination.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      670 2023-04-05 11:46:28.000000 stamox-0.1.0/stamox/math/special.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.288743 stamox-0.1.0/stamox/regression/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      101 2023-04-08 14:17:50.000000 stamox-0.1.0/stamox/regression/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2445 2023-04-09 13:44:20.000000 stamox-0.1.0/stamox/regression/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7098 2023-04-09 14:03:38.000000 stamox-0.1.0/stamox/regression/_lm.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.289115 stamox-0.1.0/stamox/sample/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      228 2023-04-04 14:38:25.000000 stamox-0.1.0/stamox/sample/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2835 2023-04-09 14:28:45.000000 stamox-0.1.0/stamox/sample/_bootstrap.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1826 2023-04-06 15:17:13.000000 stamox-0.1.0/stamox/sample/_jackknife.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      881 2023-04-09 14:07:31.000000 stamox-0.1.0/stamox/transformation.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.281299 stamox-0.1.0/stamox.egg-info/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-10 09:39:25.000000 stamox-0.1.0/stamox.egg-info/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2060 2023-04-10 09:39:25.000000 stamox-0.1.0/stamox.egg-info/SOURCES.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-10 09:39:25.000000 stamox-0.1.0/stamox.egg-info/dependency_links.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)      379 2023-04-10 09:39:25.000000 stamox-0.1.0/stamox.egg-info/requires.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-10 09:39:25.000000 stamox-0.1.0/stamox.egg-info/top_level.txt
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-10 09:39:25.289237 stamox-0.1.0/tests/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1747 2023-04-08 15:17:53.000000 stamox-0.1.0/tests/test_basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612581 stamox-0.1.2/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.2/LICENCE
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:52:39.612434 stamox-0.1.2/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     3921 2023-04-10 09:03:02.000000 stamox-0.1.2/README.md
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      413 2023-03-28 10:26:52.000000 stamox-0.1.2/pyproject.toml
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-14 06:52:39.612618 stamox-0.1.2/setup.cfg
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1121 2023-04-14 06:52:34.000000 stamox-0.1.2/setup.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602023 stamox-0.1.2/stamox/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      610 2023-04-10 07:38:29.000000 stamox-0.1.2/stamox/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602873 stamox-0.1.2/stamox/anova/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       70 2023-03-28 10:30:02.000000 stamox-0.1.2/stamox/anova/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.603131 stamox-0.1.2/stamox/anova/one_way/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.2/stamox/anova/one_way/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4298 2023-04-10 07:41:59.000000 stamox-0.1.2/stamox/anova/one_way/_aov.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-11 10:08:22.000000 stamox-0.1.2/stamox/basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.603384 stamox-0.1.2/stamox/cluster/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-10 07:00:50.000000 stamox-0.1.2/stamox/cluster/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5151 2023-04-14 05:37:17.000000 stamox-0.1.2/stamox/cluster/_kmeans.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.604313 stamox-0.1.2/stamox/core/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      630 2023-04-10 07:21:03.000000 stamox-0.1.2/stamox/core/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      231 2023-04-13 16:45:38.000000 stamox-0.1.2/stamox/core/_func_state.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-14 05:56:50.000000 stamox-0.1.2/stamox/core/_utils.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2921 2023-04-14 06:25:15.000000 stamox-0.1.2/stamox/core/base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2324 2023-04-14 06:17:30.000000 stamox-0.1.2/stamox/core/jit.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6174 2023-04-14 06:17:16.000000 stamox-0.1.2/stamox/core/maps.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-14 06:43:29.000000 stamox-0.1.2/stamox/core/pipe.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.607523 stamox-0.1.2/stamox/distribution/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1680 2023-04-13 15:54:20.000000 stamox-0.1.2/stamox/distribution/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6173 2023-04-14 05:36:26.000000 stamox-0.1.2/stamox/distribution/_beta.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5559 2023-04-13 15:59:27.000000 stamox-0.1.2/stamox/distribution/_binomial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6371 2023-04-13 14:31:34.000000 stamox-0.1.2/stamox/distribution/_cauchy.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5117 2023-04-08 16:53:06.000000 stamox-0.1.2/stamox/distribution/_chisq.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2220 2023-04-08 17:08:44.000000 stamox-0.1.2/stamox/distribution/_ecdf.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5675 2023-04-08 16:55:44.000000 stamox-0.1.2/stamox/distribution/_exp.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5942 2023-04-08 16:57:42.000000 stamox-0.1.2/stamox/distribution/_f.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6307 2023-04-08 16:59:05.000000 stamox-0.1.2/stamox/distribution/_gamma.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      787 2023-03-29 10:43:04.000000 stamox-0.1.2/stamox/distribution/_geom.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6467 2023-04-08 17:01:47.000000 stamox-0.1.2/stamox/distribution/_laplace.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7228 2023-04-08 17:00:17.000000 stamox-0.1.2/stamox/distribution/_normal.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6385 2023-04-08 17:03:09.000000 stamox-0.1.2/stamox/distribution/_pareto.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5449 2023-04-13 15:59:19.000000 stamox-0.1.2/stamox/distribution/_poisson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1067 2023-04-05 14:34:37.000000 stamox-0.1.2/stamox/distribution/_q_discrete_search.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1873 2023-03-29 10:43:29.000000 stamox-0.1.2/stamox/distribution/_rademacher.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6920 2023-04-08 17:04:47.000000 stamox-0.1.2/stamox/distribution/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1144 2023-03-29 10:43:56.000000 stamox-0.1.2/stamox/distribution/_triangular.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6220 2023-04-08 17:06:06.000000 stamox-0.1.2/stamox/distribution/_uniform.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5556 2023-04-08 16:42:13.000000 stamox-0.1.2/stamox/distribution/_weibull.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.607777 stamox-0.1.2/stamox/experimental/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-13 16:31:36.000000 stamox-0.1.2/stamox/experimental/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1351 2023-04-13 16:31:43.000000 stamox-0.1.2/stamox/experimental/better_partial.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608033 stamox-0.1.2/stamox/experimental/decomposition/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-11 10:10:40.000000 stamox-0.1.2/stamox/experimental/decomposition/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-10 07:40:46.000000 stamox-0.1.2/stamox/experimental/decomposition/_pca.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608422 stamox-0.1.2/stamox/experimental/maps/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-11 10:10:44.000000 stamox-0.1.2/stamox/experimental/maps/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-03-27 09:56:00.000000 stamox-0.1.2/stamox/experimental/maps/auto_map.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-03-28 10:31:15.000000 stamox-0.1.2/stamox/experimental/maps/cube_map.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608674 stamox-0.1.2/stamox/experimental/nn/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        0 2023-04-12 13:43:28.000000 stamox-0.1.2/stamox/experimental/nn/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.608980 stamox-0.1.2/stamox/formula/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-08 13:01:51.000000 stamox-0.1.2/stamox/formula/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1415 2023-04-11 10:10:07.000000 stamox-0.1.2/stamox/formula/_formula.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.610682 stamox-0.1.2/stamox/hypothesis/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      814 2023-04-14 06:42:01.000000 stamox-0.1.2/stamox/hypothesis/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2540 2023-04-14 06:37:22.000000 stamox-0.1.2/stamox/hypothesis/_bartlett.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      734 2023-03-29 10:40:56.000000 stamox-0.1.2/stamox/hypothesis/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2283 2023-04-06 14:56:52.000000 stamox-0.1.2/stamox/hypothesis/_durbin_watson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2740 2023-04-14 06:41:22.000000 stamox-0.1.2/stamox/hypothesis/_friedman.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      806 2023-03-29 10:41:12.000000 stamox-0.1.2/stamox/hypothesis/_p.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      837 2023-03-29 10:41:19.000000 stamox-0.1.2/stamox/hypothesis/_pearsonr.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5033 2023-04-14 06:41:48.000000 stamox-0.1.2/stamox/hypothesis/_shapiro_wilk.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      954 2023-03-29 10:41:28.000000 stamox-0.1.2/stamox/hypothesis/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1179 2023-03-21 16:44:14.000000 stamox-0.1.2/stamox/hypothesis/cor2ci.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      485 2023-03-21 16:44:03.000000 stamox-0.1.2/stamox/hypothesis/cor2p.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1029 2023-03-16 09:09:37.000000 stamox-0.1.2/stamox/hypothesis/corr.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.611054 stamox-0.1.2/stamox/math/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-10 03:27:30.000000 stamox-0.1.2/stamox/math/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1255 2023-04-10 03:26:51.000000 stamox-0.1.2/stamox/math/combination.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      670 2023-04-05 11:46:28.000000 stamox-0.1.2/stamox/math/special.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.611422 stamox-0.1.2/stamox/regression/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-13 07:01:57.000000 stamox-0.1.2/stamox/regression/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-12 13:26:06.000000 stamox-0.1.2/stamox/regression/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7062 2023-04-10 10:29:07.000000 stamox-0.1.2/stamox/regression/_lm.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612014 stamox-0.1.2/stamox/sample/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      343 2023-04-14 06:48:40.000000 stamox-0.1.2/stamox/sample/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2835 2023-04-09 14:28:45.000000 stamox-0.1.2/stamox/sample/_bootstrap.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1821 2023-04-14 06:48:11.000000 stamox-0.1.2/stamox/sample/_jackknife.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      888 2023-04-10 09:45:17.000000 stamox-0.1.2/stamox/transformation.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.602723 stamox-0.1.2/stamox.egg-info/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4245 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2133 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      385 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/requires.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-14 06:52:39.000000 stamox-0.1.2/stamox.egg-info/top_level.txt
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-14 06:52:39.612185 stamox-0.1.2/tests/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1747 2023-04-08 15:17:53.000000 stamox-0.1.2/tests/test_basic.py
```

### Comparing `stamox-0.1.0/LICENCE` & `stamox-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/PKG-INFO` & `stamox-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.0
+Version: 0.1.2
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `stamox-0.1.0/README.md` & `stamox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/setup.py` & `stamox-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.1.0"
+VERSION = "0.1.2"
 PACKAGE_NAME = "stamox"
 AUTHOR = "Jia Yaobo"
 URL = "https://github.com/jiayaobo/stamox"
 
 LICENSE = "Apache 2.0"
 DESCRIPTION = "Accelerate Your Statistical Analysis with JAX."
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
@@ -20,14 +20,15 @@
     "jaxtyping>=0.2.14",
     "typing_extensions>=4.5.0",
     "equinox>=0.10.1",
     "jaxopt>=0.6",
     "pandas>=1.5.3",
     "patsy>=0.5.3",
     "tensorflow-probability>=0.19.0",
+    "scipy"
 ]
 TESTS_REQUIRES = ["pytest", "scipy", "numpy", "sklearn", "statsmodels"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
```

### Comparing `stamox-0.1.0/stamox/__init__.py` & `stamox-0.1.2/stamox/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/anova/one_way/_aov.py` & `stamox-0.1.2/stamox/anova/one_way/_aov.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/basic.py` & `stamox-0.1.2/stamox/basic.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 sum = make_partial_pipe(jnp.sum)
 prod = make_partial_pipe(jnp.prod)
 cumsum = make_partial_pipe(jnp.cumsum)
 cumprod = make_partial_pipe(jnp.cumprod)
 diff = make_partial_pipe(jnp.diff)
 cov = make_partial_pipe(jnp.cov)
 corrcoef = make_partial_pipe(jnp.corrcoef)
+arcsin = make_partial_pipe(jnp.arcsin)
+arccos = make_partial_pipe(jnp.arccos)
 
 
 @make_partial_pipe
 def scale(x: ArrayLike, axis: int = 0) -> ArrayLike:
     """Calculate standardized x along axis.
 
     Args:
```

### Comparing `stamox-0.1.0/stamox/cluster/_kmeans.py` & `stamox-0.1.2/stamox/cluster/_kmeans.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.tot_withinss = tot_withinss
 
     def _predict(self, x: ArrayLike):
         # predict the cluster for new data
         return vq(x, self.centers)[0]
 
 
-@make_partial_pipe
+@make_partial_pipe(name="kmeans")
 def kmeans(
     x: ArrayLike,
     n_cluster: int,
     restarts: int = 10,
     max_iters: int = 100,
     dtype: jnp.dtype = jnp.float32,
     *,
```

### Comparing `stamox-0.1.0/stamox/core/__init__.py` & `stamox-0.1.2/stamox/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/core/base.py` & `stamox-0.1.2/stamox/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 class Functional(eqx.Module):
     """General Function"""
-
     _name: str
     _fn: Callable[P, T]
     _is_partial: bool
     _is_fully_partial: bool
 
     def __init__(
         self,
@@ -29,15 +28,16 @@
             fn (Optional[Callable|None], optional): Callable object.
         """
         super().__init__()
         self._name = name
         self._fn = fn
         self._is_partial = is_partial
         self._is_fully_partial = is_fully_partial
-
+    
+    
     @property
     def name(self):
         """Get the name of the function."""
         return self._name
 
     @property
     def func(self):
```

### Comparing `stamox-0.1.0/stamox/core/jit.py` & `stamox-0.1.2/stamox/core/jit.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def pipe_jit(
-    func: Callable[P, T], *, donate: str = "none", name: str = None
+    func: Callable[P, T] = None, *, donate: str = "none", name: str = None
 ) -> Callable[P, T]:
     """Creates a pipeable jitted functional from a given function.
 
     Args:
         func: The function to create the functional from.
         donate: Optional donation string.
         name: Optional name for the functional.
@@ -28,30 +28,31 @@
         >>> f = lambda x: x + 1
         >>> f = pipe_jit(f)
         >>> g = f >> f >> f
         >>> g(1)
         4
     """
     if name is None and func is not None:
-        name = func.__name__
+        if hasattr(func, "name"):
+            name = func.name
+        else:
+            name = func.__name__
 
     @wraps(func)
     def wrap(func: Callable[P, T]) -> Callable:
         fn = filter_jit(func, donate=donate)
 
-        @wraps(func)
-        def create_functional(*args, **kwargs):
-            return Functional(name=name, fn=fn)(*args, **kwargs)
-
-        return create_functional
+        return Functional(name=name, fn=fn)
 
     return wrap if func is None else wrap(func)
 
 
-def partial_pipe_jit(func: Callable[P, T], *, name: str = None) -> Callable[P, T]:
+def partial_pipe_jit(
+    func: Callable[P, T] = None, *, name: str = None
+) -> Callable[P, T]:
     """Creates a partial pipeable jitted functional from a given function.
 
     Args:
         func (Callable[P, T]): _description_
         name (str, optional): _description_. Defaults to None.
 
     Returns:
@@ -62,15 +63,18 @@
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_jit(f)
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(1)
         7
     """
     if name is None and func is not None:
-        name = func.__name__
+        if hasattr(func, "name"):
+            name = func.name
+        else:
+            name = func.__name__
 
     @wraps(func)
     def wrap(func: Callable[P, T]) -> Callable:
         @wraps(func)
         def partial_fn(*args, donate: str = "none", **kwargs):
             fn = filter_jit(func, donate=donate)
             fn = partial(fn, **kwargs)
```

### Comparing `stamox-0.1.0/stamox/core/maps.py` & `stamox-0.1.2/stamox/core/maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def pipe_vmap(
-    func: Callable[P, T],
+    func: Callable[P, T] = None,
     *,
     in_axes=0,
     out_axes=0,
     axis_name: Hashable = None,
     axis_size: int | None = None,
     name: str = None
 ) -> Callable[P, T]:
@@ -51,25 +51,22 @@
         fn = filter_vmap(
             func,
             in_axes=in_axes,
             out_axes=out_axes,
             axis_name=axis_name,
             axis_size=axis_size,
         )
-
-        @wraps(func)
-        def create_functional(*args):
-            return Functional(name=name, fn=fn)(*args)
-
-        return create_functional
+        return Functional(name=name, fn=fn)
 
     return wrap if func is None else wrap(func)
 
 
-def partial_pipe_vmap(func: Callable[P, T], *, name: str = None) -> Callable[P, T]:
+def partial_pipe_vmap(
+    func: Callable[P, T] = None, *, name: str = None
+) -> Callable[P, T]:
     """Partially apply a function to a vmap.
 
     Args:
         func (Callable[P, T]): The function to partially apply.
         name (str, optional): The name of the function. Defaults to None.
 
     Returns:
@@ -80,16 +77,14 @@
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_vmap(f)
         >>> g = f(y=1) >> f(y=2) >> f(y=3)
         >>> g(jnp.array([1, 2, 3]))
         Array([7, 8, 9], dtype=int32)
     """
     if name is None and func is not None:
-        if isinstance(func, Functional):
-            name = func.name
         name = func.__name__
 
     @wraps(func)
     def wrap(func: Callable[P, T]) -> Callable:
         if isinstance(func, Functional):
             func = func.func
 
@@ -106,25 +101,25 @@
             fn = filter_vmap(
                 fn,
                 in_axes=in_axes,
                 out_axes=out_axes,
                 axis_name=axis_name,
                 axis_size=axis_size,
             )
-            if len(args) !=0:
+            if len(args) != 0:
                 return fn(*args)
             return Functional(name=name, fn=fn)
 
         return partial_fn
 
     return wrap if func is None else wrap(func)
 
 
 def pipe_pmap(
-    func: Callable[P, T],
+    func: Callable[P, T] = None,
     *,
     in_axes=0,
     out_axes=0,
     axis_name: Hashable = None,
     axis_size: int | None = None,
     name: str = None
 ) -> Callable[P, T]:
@@ -146,38 +141,39 @@
         >>> f = lambda x: x + 1
         >>> f = pipe_pmap(f)
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
         fn = filter_pmap(
             func,
             in_axes=in_axes,
             out_axes=out_axes,
             axis_name=axis_name,
             axis_size=axis_size,
         )
 
-        @wraps(func)
-        def create_functional(*args):
-            return Functional(name=name, fn=fn)(*args)
-
-        return create_functional
+        return Functional(name=name, fn=fn)
 
     return wrap if func is None else wrap(func)
 
 
-def partial_pipe_pmap(func: Callable[P, T], *, name: str = None) -> Callable[P, T]:
+def partial_pipe_pmap(
+    func: Callable[P, T] = None, *, name: str = None
+) -> Callable[P, T]:
     """Partially apply a function to a pipe.
 
     Args:
         func (Callable[P, T]): The function to partially apply.
         name (str, optional): The name of the function. Defaults to None.
 
     Returns:
@@ -188,15 +184,18 @@
         >>> f = lambda x, y: x + y
         >>> f = partial_pipe_pmap(f)
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

### Comparing `stamox-0.1.0/stamox/core/pipe.py` & `stamox-0.1.2/stamox/core/pipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -176,28 +176,28 @@
         ...     return x + 1
         >>> h = add >> add >> add
         >>> h(1)
         4
     """
 
     if name is None and func is not None:
-        name = func.__name__
+        if hasattr(func, "name"):
+            name = func.name
+        else:
+            name = func.__name__
 
     @wraps(func)
-    def wrap(func: Callable[P, T]):
+    def wrap(func: Callable[P, T]) -> Callable[P, T]:
         if isinstance(func, Functional):
             func = func.func
 
-        @wraps(func)
-        def create_functional(*args, **kwargs):
-            return Functional(name=name, fn=func)(*args, **kwargs)
-
-        return create_functional
+        functional = Functional(name=name, fn=func)
+        return functional
 
-    return wrap(func) if func is not None else wrap
+    return wrap if func is None else wrap(func)
 
 
 def make_partial_pipe(
     func: Optional[Callable[P, T]] = None, name: str = None
 ) -> Callable[P, T]:
     """Makes a Partial Function Pipe.
 
@@ -214,15 +214,18 @@
         ... def add(x, y):
         ...     return x + y
         >>> h = add(y=1) >> add(y=2) >> add(y=3)
         >>> h(1)
         7
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

### Comparing `stamox-0.1.0/stamox/distribution/__init__.py` & `stamox-0.1.2/stamox/distribution/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from stamox.distribution._beta import dbeta, pbeta, qbeta, rbeta
+from stamox.distribution._binomial import dbinom, pbinom, qbinom, rbinom
 from stamox.distribution._cauchy import dcauchy, pcauchy, qcauchy, rcauchy
 from stamox.distribution._chisq import dchisq, pchisq, qchisq, rchisq
 from stamox.distribution._ecdf import ecdf, step_fun
 from stamox.distribution._exp import dexp, pexp, qexp, rexp
 from stamox.distribution._f import dF, pF, qF, rF
 from stamox.distribution._gamma import dgamma, pgamma, qgamma, rgamma
 from stamox.distribution._laplace import dlaplace, plaplace, qlaplace, rlaplace
 from stamox.distribution._normal import dnorm, pnorm, qnorm, rnorm
 from stamox.distribution._pareto import dpareto, ppareto, qpareto, rpareto
+from stamox.distribution._poisson import dpoisson, ppoisson, qpoisson, rpoisson
 from stamox.distribution._t import dt, pt, qt, rt
 from stamox.distribution._uniform import dunif, punif, qunif, runif
 
 
 __all__ = [
     "pt",
     "qt",
     "rt",
     "dt",
+    "pbinom",
+    "qbinom",
+    "rbinom",
+    "dbinom",
     "pnorm",
     "qnorm",
     "rnorm",
     "dnorm",
     "pbeta",
     "qbeta",
     "rbeta",
@@ -37,14 +43,18 @@
     "qchisq",
     "rchisq",
     "dchisq",
     "ppareto",
     "qpareto",
     "rpareto",
     "dpareto",
+    "ppoisson",
+    "qpoisson",
+    "rpoisson",
+    "dpoisson",
     "pF",
     "qF",
     "dF",
     "rF",
     "pcauchy",
     "qcauchy",
     "rcauchy",
```

### Comparing `stamox-0.1.0/stamox/distribution/_beta.py` & `stamox-0.1.2/stamox/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_cauchy.py` & `stamox-0.1.2/stamox/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_chisq.py` & `stamox-0.1.2/stamox/distribution/_chisq.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_ecdf.py` & `stamox-0.1.2/stamox/distribution/_ecdf.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_exp.py` & `stamox-0.1.2/stamox/distribution/_exp.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_f.py` & `stamox-0.1.2/stamox/distribution/_f.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_gamma.py` & `stamox-0.1.2/stamox/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_geom.py` & `stamox-0.1.2/stamox/distribution/_geom.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_laplace.py` & `stamox-0.1.2/stamox/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_normal.py` & `stamox-0.1.2/stamox/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_pareto.py` & `stamox-0.1.2/stamox/distribution/_pareto.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_poisson.py` & `stamox-0.1.2/stamox/distribution/_poisson.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 from equinox import filter_jit, filter_vmap
+from jax import pure_callback, ShapeDtypeStruct
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jax.scipy.special import gammainc, gammaln
 from jaxtyping import Array, ArrayLike, Bool, Float
-from tensorflow_probability.substrates.jax.distributions.poisson import Poisson
+from scipy.stats import poisson
 
 from ..core import make_partial_pipe
 
 
 @filter_jit
 def _ppoisson(x: Union[Float, ArrayLike], rate: Union[Float, ArrayLike]) -> Array:
     k = jnp.floor(x) + 1.0
@@ -20,27 +21,29 @@
 
 @make_partial_pipe
 def ppoisson(
     q: Union[Float, ArrayLike],
     rate: Union[Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-) -> Array:
+    dtype=jnp.float32,
+) -> ArrayLike:
     """Computes the cumulative distribution function of the Poisson distribution.
 
     Args:
         q (Union[Float, ArrayLike]): The value at which to evaluate the CDF.
         rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
         lower_tail (bool, optional): Whether to compute the lower tail of the CDF. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
 
     Returns:
         ArrayLike: The cumulative distribution function of the Poisson distribution evaluated at `q`.
     """
-    q = jnp.asarray(q)
+    q = jnp.asarray(q, dtype=dtype)
     q = jnp.atleast_1d(q)
     p = filter_vmap(_ppoisson)(q, rate)
     if not lower_tail:
         p = 1 - p
     if log_prob:
         p = jnp.log(p)
     return p
@@ -56,99 +59,107 @@
 
 @make_partial_pipe
 def dpoisson(
     x: Union[Float, ArrayLike],
     rate: Union[Float, ArrayLike],
     lower_tail=True,
     log_prob=False,
-) -> Array:
+    dtype=jnp.float32,
+) -> ArrayLike:
     """Computes the probability density function of the Poisson distribution.
 
     Args:
         x (Union[Float, ArrayLike]): The value at which to evaluate the PDF.
         rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
         lower_tail (bool, optional): Whether to compute the lower tail of the PDF. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float32.
 
     Returns:
-        Array: The probability density function of the Poisson distribution evaluated at `x`.
+        ArrayLike: The probability density function of the Poisson distribution evaluated at `x`.
     """
-    x = jnp.asarray(x)
+    x = jnp.asarray(x, dtype=dtype)
     x = jnp.atleast_1d(x)
     grads = filter_vmap(_dpoisson)(x, rate)
     if not lower_tail:
         grads = 1 - grads
     if log_prob:
         grads = jnp.log(grads)
     return grads
 
 
 @filter_jit
 def _rpoisson(
-    key: KeyArray, rate: Union[Float, ArrayLike], sample_shape: Optional[Shape] = None
+    key: KeyArray,
+    rate: Union[Float, ArrayLike],
+    sample_shape: Optional[Shape] = None,
+    dtype=jnp.int32,
 ):
-    return jrand.poisson(key, rate, shape=sample_shape)
+    return jrand.poisson(key, rate, shape=sample_shape, dtype=dtype)
 
 
 @make_partial_pipe
 def rpoisson(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     rate: Union[Float, ArrayLike] = None,
     lower_tail=True,
     log_prob=False,
-) -> Array:
+    dtype=jnp.int32,
+) -> ArrayLike:
     """Generates samples from the Poisson distribution.
 
     Args:
         key (KeyArray): Random number generator state used for random sampling.
         rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
         sample_shape (Optional[Shape], optional): Shape of the output array. Defaults to None.
         lower_tail (bool, optional): Whether to return the lower tail probability. Defaults to True.
         log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int32.
 
     Returns:
-        Array: Samples from the Poisson distribution.
+        ArrayLike: Samples from the Poisson distribution.
     """
-    rvs = _rpoisson(key, rate, sample_shape=sample_shape)
+    rvs = _rpoisson(key, rate, sample_shape=sample_shape, dtype=dtype)
     if not lower_tail:
         rvs = 1 - rvs
     if log_prob:
         rvs = jnp.log(rvs)
     return rvs
 
 
 @filter_jit
-def _qpoisson(q, rate):
-    """
-    Computes the p-th quantile of a Poisson distribution with mean rate use approximate
-    """
-    pass
-
-
-    
+def _qpoisson(q, rate, dtype):
+    result_shape_type = ShapeDtypeStruct(jnp.shape(q), dtype)
+    _scp_poisson_ppf = lambda q, rate: poisson(rate).ppf(q).astype(dtype)
+    p = pure_callback(_scp_poisson_ppf, result_shape_type, q, rate)
+    return p
 
 
 @make_partial_pipe
 def qpoisson(
-    q: Union[Float, ArrayLike],
+    p: Union[Float, ArrayLike],
     rate: Union[Float, ArrayLike],
     lower_tail: Bool = True,
     log_prob: Bool = False,
+    dtype=jnp.int32,
 ) -> ArrayLike:
     """Computes the quantile function of the Poisson distribution.
 
     Args:
-        q (Union[Float, ArrayLike]): The quantile at which to evaluate the quantile function.
+        p (Union[Float, ArrayLike]): The probability at which to evaluate the quantile function.
         rate (Union[Float, ArrayLike]): The rate parameter of the Poisson distribution.
+        lower_tail (bool, optional): Whether to compute the lower tail of the quantile function. Defaults to True.
+        log_prob (bool, optional): Whether to return the log probability. Defaults to False.
+        dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.int32.
 
     Returns:
-        Array: The quantile function of the Poisson distribution evaluated at `q`.
+        ArrayLike: The quantile function of the Poisson distribution evaluated at `p`.
     """
-    ImportWarning("qpoisson is not yet well tested.")
-    raise NotImplementedError("Not Implemented Yet!")
-    q = jnp.atleast_1d(q)
+    p = jnp.asarray(p)
+    p = jnp.atleast_1d(p)
     if not lower_tail:
-        q = 1 - q
+        p = 1 - p
     if log_prob:
-        q = jnp.exp(q)
-    return filter_vmap(_qpoisson)(q, rate)
+        p = jnp.exp(p)
+    q = filter_vmap(_qpoisson)(p, rate, dtype)
+    return q
```

### Comparing `stamox-0.1.0/stamox/distribution/_q_discrete_search.py` & `stamox-0.1.2/stamox/distribution/_q_discrete_search.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_rademacher.py` & `stamox-0.1.2/stamox/distribution/_rademacher.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_t.py` & `stamox-0.1.2/stamox/distribution/_t.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_triangular.py` & `stamox-0.1.2/stamox/distribution/_triangular.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_uniform.py` & `stamox-0.1.2/stamox/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/distribution/_weibull.py` & `stamox-0.1.2/stamox/distribution/_weibull.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/experimental/decomposition/_pca.py` & `stamox-0.1.2/stamox/experimental/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/experimental/maps/auto_map.py` & `stamox-0.1.2/stamox/experimental/maps/auto_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/experimental/maps/cube_map.py` & `stamox-0.1.2/stamox/experimental/maps/cube_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/formula/_formula.py` & `stamox-0.1.2/stamox/formula/_formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         formula: A string representation of a formula.
         eval_env: An environment mapping column names to arrays which patsy can use when evaluating a formula.
         NA_action: A string specifying how to handle missing values. One of "drop", "raise", or "na_action".
         return_type: A string specifying the return type. One of "matrix", "dataframe", or "design_info".
 
     Returns:
         Matrices: A named tuple containing the design matrices for the response and predictors, as well as the names of the columns in each matrix.
+
     """
     y, X = patsy.dmatrices(
         formula, data, eval_env=eval_env, NA_action=NA_action, return_type=return_type
     )
     return Matrices(
         jnp.asarray(y, dtype=dtype),
         jnp.asarray(X, dtype=dtype),
```

### Comparing `stamox-0.1.0/stamox/hypothesis/__init__.py` & `stamox-0.1.2/stamox/hypothesis/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from stamox.hypothesis._bartlett import bartlett_test, BartlettTest
+from stamox.core import make_pipe
+from stamox.hypothesis._bartlett import bartlett_test_fun, BartlettTest
 from stamox.hypothesis._base import HypoTest
 from stamox.hypothesis._durbin_watson import durbin_watson_test, DurbinWatsonTest
-from stamox.hypothesis._friedman import friedman_test, FriedmanTest
-from stamox.hypothesis._shapiro_wilk import shapiro_wilk_test, ShapiroWilkTest
+from stamox.hypothesis._friedman import friedman_test_fun, FriedmanTest
+from stamox.hypothesis._shapiro_wilk import shapiro_wilk_test_fun, ShapiroWilkTest
 
 
+bartlett_test = make_pipe(bartlett_test_fun, name="bartlett_test")
+friedman_test = make_pipe(friedman_test_fun, name="friedman_test")
+shapiro_wilk_test = make_pipe(shapiro_wilk_test_fun, name="shapiro_wilk_test")
+
 __all__ = [
     "HypoTest",
     "bartlett_test",
     "BartlettTest",
     "durbin_watson_test",
     "DurbinWatsonTest",
     "friedman_test",
     "FriedmanTest",
     "shapiro_wilk_test",
     "ShapiroWilkTest",
-]
+]
```

### Comparing `stamox-0.1.0/stamox/hypothesis/_bartlett.py` & `stamox-0.1.2/stamox/hypothesis/_bartlett.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-"""
-In statistics, Bartlett's test, named after Maurice Stevenson Bartlett, is used to test homoscedasticity, 
-that is, if multiple samples are from populations with equal variances.Some statistical tests, 
-such as the analysis of variance, assume that variances are equal across groups or samples, 
-which can be verified with Bartlett's test.
-"""
+# ::: stamox/hypothesis/_bartlett.py ::: 1 of 1 (100%)
 
 from functools import partial
 from typing import Sequence
 
 import jax.numpy as jnp
 from equinox import filter_jit
 from jax import vmap
 from jaxtyping import ArrayLike
 
-from ..core import make_pipe
 from ..distribution import pchisq
 from ._base import HypoTest
 
 
 class BartlettTest(HypoTest):
     """Class for performing a Bartlett's test.
 
     This class is used to perform a Bartlett's test, which tests the null hypothesis that all input samples are from populations with equal variances.
 
     Attributes:
         statistic (float): The test statistic.
         parameters (int): The degrees of freedom.
         p_value (float): The p-value of the test.
     """
+
     def __init__(
         self,
         statistic=None,
         parameters=None,
         p_value=None,
         estimate=None,
         null_value=None,
@@ -51,16 +46,15 @@
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
     @property
     def df(self):
         return self.parameters
 
 
-@make_pipe
-def bartlett_test(*samples: Sequence[ArrayLike]) -> BartlettTest:
+def bartlett_test_fun(*samples: Sequence[ArrayLike]) -> BartlettTest:
     """Calculates the Bartlett test statistic for multiple samples.
 
     Args:
         *samples Sequence[ArrayLike]): A sequence of 1-D arrays, each containing
             a sample of scores. All samples must have the same length.
 
     Returns:
@@ -72,25 +66,16 @@
     """
     samples = jnp.vstack(samples)
     return _bartlett(samples)
 
 
 @filter_jit
 def _bartlett(samples):
-    """Calculates the Bartlett test statistic for multiple samples.
-
-    Args:
-        samples (array_like): A 2-D array, each row containing a sample of
-            scores. All samples must have the same length.
-
-    Returns:
-        float: The Bartlett test statistic.
-    """
     k = samples.shape[0]
-    Ni = jnp.asarray(vmap(jnp.size, in_axes=(0,))(samples), dtype=jnp.float32)
+    Ni = jnp.asarray(vmap(jnp.size, in_axes=(0,))(samples), dtype=samples.dtype)
     ssq = vmap(partial(jnp.var, ddof=1), in_axes=(0,))(samples)
     Ntot = jnp.sum(Ni, axis=0)
     spsq = jnp.sum((Ni - 1) * ssq, axis=0) / (1.0 * (Ntot - k))
     numer = (Ntot * 1.0 - k) * jnp.log(spsq) - jnp.sum(
         (Ni - 1.0) * jnp.log(ssq), axis=0
     )
     denom = 1.0 + 1.0 / (3 * (k - 1)) * (
```

### Comparing `stamox-0.1.0/stamox/hypothesis/_base.py` & `stamox-0.1.2/stamox/hypothesis/_base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/_durbin_watson.py` & `stamox-0.1.2/stamox/hypothesis/_durbin_watson.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/_friedman.py` & `stamox-0.1.2/stamox/hypothesis/_friedman.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import jax.numpy as jnp
 from equinox import filter_jit
 from jax import vmap
 from jax.scipy.stats import rankdata
 from jaxtyping import ArrayLike
 
-from ..core import make_pipe
 from ..distribution import pchisq
 from ._base import HypoTest
 
 
 class FriedmanTest(HypoTest):
     """Class for performing Friedman Rank Sum Test.
 
@@ -42,16 +41,15 @@
             statistic, parameters, p_value, estimate, null_value, alternative, name
         )
     
     def __repr__(self):
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
 
-@make_pipe
-def friedman_test(*samples: Sequence[ArrayLike]) -> FriedmanTest:
+def friedman_test_fun(*samples: Sequence[ArrayLike]) -> FriedmanTest:
     """Computes the Friedman statistic for a set of samples.
 
     Args:
         *samples: A sequence of samples, each sample being a sequence of
             observations.
 
     Returns:
```

### Comparing `stamox-0.1.0/stamox/hypothesis/_p.py` & `stamox-0.1.2/stamox/hypothesis/_p.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/_pearsonr.py` & `stamox-0.1.2/stamox/hypothesis/_pearsonr.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/_shapiro_wilk.py` & `stamox-0.1.2/stamox/hypothesis/_shapiro_wilk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import jax.numpy as jnp
 from equinox import filter_jit
 from jax import lax, vmap
 from jaxtyping import ArrayLike
 
-from ..core import make_pipe
 from ..distribution import pnorm, qnorm
 from ._base import HypoTest
 
 
 _g = [-2.273, 0.459]
 _c1 = [0.0, 0.221157, -0.147981, -2.07119, 4.434685, -2.706056]
 _c2 = [0.0, 0.042981, -0.293762, -1.752461, 5.682633, -3.582633]
@@ -42,16 +41,15 @@
             statistic, parameters, p_value, estimate, null_value, alternative, name
         )
 
     def __repr__(self):
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
 
-@make_pipe
-def shapiro_wilk_test(x: ArrayLike) -> ShapiroWilkTest:
+def shapiro_wilk_test_fun(x: ArrayLike) -> ShapiroWilkTest:
     """Computes the Shapiro-Wilk test for normality.
 
     Args:
         x (ArrayLike): The data to be tested.
 
     Returns:
         ShapiroWilkTest: The Shapiro-Wilk Test object.
```

### Comparing `stamox-0.1.0/stamox/hypothesis/_t.py` & `stamox-0.1.2/stamox/hypothesis/_t.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/cor2ci.py` & `stamox-0.1.2/stamox/hypothesis/cor2ci.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/hypothesis/corr.py` & `stamox-0.1.2/stamox/hypothesis/corr.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/math/combination.py` & `stamox-0.1.2/stamox/math/combination.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/math/special.py` & `stamox-0.1.2/stamox/math/special.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/regression/_base.py` & `stamox-0.1.2/stamox/regression/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     _rank: int
     _dtype: jnp.dtype
 
     def __init__(
         self,
         in_features,
         out_features,
-        coefs = None,
-        df_resid = None,
-        df_model = None,
-        n_obs = None,
-        resid = None,
-        fitted_values = None,
-        rank = None,
-        dtype = jnp.float32,
-        name = "RegState"
+        coefs=None,
+        df_resid=None,
+        df_model=None,
+        n_obs=None,
+        resid=None,
+        fitted_values=None,
+        rank=None,
+        dtype=jnp.float32,
+        name="RegState",
     ):
         super().__init__(name=name, fn=None)
         self.in_features = in_features
         self.out_features = out_features
         if coefs is None:
             coefs = jnp.zeros((in_features, out_features))
         self._coefs = coefs
@@ -43,15 +43,15 @@
         self._fitted_values = fitted_values
         self._rank = rank
         self._dtype = dtype
 
     @property
     def params(self):
         return self._coefs
-    
+
     @property
     def coefs(self):
         return self._coefs
 
     @property
     def coefs_X(self):
         return self.params[1:, :]
@@ -63,46 +63,41 @@
     @property
     def df_resid(self):
         return self._df_resid
 
     @property
     def df_model(self):
         return self._df_model
-    
+
     @property
     def n_obs(self):
         return self._n_obs
 
     @property
     def resid(self):
         return self._resid
 
     @property
     def fitted_values(self):
         return self._fitted_values
-    
+
     @property
     def rank(self):
         return self._rank
-    
+
     @property
     def dtype(self):
         return self._dtype
-
-    def __call__(self, X):
+    
+    def _transform(self, X):
         if X.shape[1] == self.in_features:
             return jnp.matmul(X, self.params)
         else:
             return jnp.matmul(X, self.coefs_X) + self.intercept
 
+    def _predict(self, X):
+        return self._transform(X)
+
     def _summary(self):
-        summary = f"""
-        Model: {self.name}
-        Number of observations: {self.df_resid + self.df_model}
-        Degrees of freedom: {self.df_resid} (residuals) / {self.df_model} (model)
-        Rank: {self._rank}
-        Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
-        """
-        return summary
-        
+        return "Not Implement Yet"
+
 
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stamox-0.1.0/stamox/regression/_lm.py` & `stamox-0.1.2/stamox/regression/_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         >>> import numpy as np
         >>> np.random.seed(42)
         >>> X = np.random.uniform(size=(1000, 3))
         >>> y = (
                 3 * X[:, 0]
                 + 2 * X[:, 1]
                 - 7 * X[:, 2]
-                + np.random.standard_t(10, size=(1000,))
+                + 1.
             )
         >>> data = pd.DataFrame(
                 np.concatenate([X, y.reshape((-1, 1))], axis=1),
                 columns=["x1", "x2", "x3", "y"],
             )
         >>> res = lm(data, "y ~ x1 + x2 + x3")
         >>> res.coefs
```

### Comparing `stamox-0.1.0/stamox/sample/_bootstrap.py` & `stamox-0.1.2/stamox/sample/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.0/stamox/sample/_jackknife.py` & `stamox-0.1.2/stamox/sample/_jackknife.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 from ..core import make_partial_pipe
 
 
 ReturnValue = TypeVar("ReturnValue")
 
 
-@make_partial_pipe
-@filter_jit
-def jackknife_sample(data: ArrayLike) -> ArrayLike:
+def jackknife_sample_fun(data: ArrayLike) -> ArrayLike:
     """Generates `num_samples` jackknife samples from `data` with replacement.
 
     Args:
         data (array-like): The original data.
 
     Returns:
         ArrayLike: An array of size (len(data)-1, len(data)) containing the jackknife samples.
@@ -40,15 +38,15 @@
         return x[idx]
 
     samples = filter_vmap(apply_except_one, in_axes=(None, 0))(data, jnp.arange(n))
 
     return samples
 
 
-@make_partial_pipe
+@make_partial_pipe(name="jackknife")
 def jackknife(data: ArrayLike, call: Callable[..., ReturnValue]) -> PyTree:
     """Computes the jackknife estimate of a given data set.
 
     Args:
         data (ArrayLike): The data set to be analyzed.
         call (Callable[..., ReturnValue]): A function to be applied to each sample.
 
@@ -58,9 +56,9 @@
     Example:
         >>> import jax.numpy as jnp
         >>> from stamox.sample import jackknife
         >>> data = jnp.arange(3)
         >>> jackknife(data, lambda x: jnp.mean(x))
         Array([1.5, 1. , 0.5], dtype=float32)
     """
-    samples = jackknife_sample(data)
+    samples = jackknife_sample_fun(data)
     return filter_jit(filter_vmap(lambda x: call(x)))(samples)
```

### Comparing `stamox-0.1.0/stamox/transformation.py` & `stamox-0.1.2/stamox/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Computes the Box-Cox transformation of a given array.
 
     Args:
         x: An array-like object to be transformed.
         lmbda: An array-like object containing the lambda values for the transformation.
 
     Returns:
-        The transformed array.
+        The boxcox transformed array.
 
     Example:
         >>> from stamox.transformation import boxcox
         >>> import jax.numpy as jnp
         >>> x = jnp.array([1, 2, 3, 4, 5], dtype=jnp.float32)
         >>> lmbda = jnp.array([0, 0, 0, 0, 0], dtype=jnp.float32)
         >>> boxcox(x, lmbda)
```

### Comparing `stamox-0.1.0/stamox.egg-info/PKG-INFO` & `stamox-0.1.2/stamox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.0
+Version: 0.1.2
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `stamox-0.1.0/stamox.egg-info/SOURCES.txt` & `stamox-0.1.2/stamox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 stamox/distribution/_q_discrete_search.py
 stamox/distribution/_rademacher.py
 stamox/distribution/_t.py
 stamox/distribution/_triangular.py
 stamox/distribution/_uniform.py
 stamox/distribution/_weibull.py
 stamox/experimental/__init__.py
+stamox/experimental/better_partial.py
 stamox/experimental/decomposition/__init__.py
 stamox/experimental/decomposition/_pca.py
 stamox/experimental/maps/__init__.py
 stamox/experimental/maps/auto_map.py
 stamox/experimental/maps/cube_map.py
+stamox/experimental/nn/__init__.py
 stamox/formula/__init__.py
 stamox/formula/_formula.py
 stamox/hypothesis/__init__.py
 stamox/hypothesis/_bartlett.py
 stamox/hypothesis/_base.py
 stamox/hypothesis/_durbin_watson.py
 stamox/hypothesis/_friedman.py
```

### Comparing `stamox-0.1.0/tests/test_basic.py` & `stamox-0.1.2/tests/test_basic.py`

 * *Files identical despite different names*

