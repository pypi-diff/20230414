# Comparing `tmp/Orange3-Explain-0.6.2.tar.gz` & `tmp/Orange3-Explain-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Explain-0.6.2.tar", last modified: Thu Dec 15 11:25:03 2022, max compression
+gzip compressed data, was "dist/Orange3-Explain-0.6.3.tar", last modified: Fri Apr 14 08:11:51 2023, max compression
```

## Comparing `Orange3-Explain-0.6.2.tar` & `Orange3-Explain-0.6.3.tar`

### file list

```diff
@@ -1,143 +1,167 @@
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.034792 Orange3-Explain-0.6.2/
--rw-r--r--   0 primoz     (501) staff       (20)    35147 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/LICENSE.txt
--rw-r--r--   0 primoz     (501) staff       (20)      127 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/MANIFEST.in
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.990698 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/
--rw-r--r--   0 primoz     (501) staff       (20)     1085 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)     5109 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/SOURCES.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/dependency_links.txt
--rw-r--r--   0 primoz     (501) staff       (20)      196 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/entry_points.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/namespace_packages.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2022-07-28 09:49:17.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/not-zip-safe
--rw-r--r--   0 primoz     (501) staff       (20)      164 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/requires.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2022-12-15 11:25:02.000000 Orange3-Explain-0.6.2/Orange3_Explain.egg-info/top_level.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1085 2022-12-15 11:25:03.034631 Orange3-Explain-0.6.2/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)      735 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/README.md
--rw-r--r--   0 primoz     (501) staff       (20)      545 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/README.pypi
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.991348 Orange3-Explain-0.6.2/doc/
--rw-r--r--   0 primoz     (501) staff       (20)     7465 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/Makefile
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.987806 Orange3-Explain-0.6.2/doc/_build/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.992302 Orange3-Explain-0.6.2/doc/_build/html/
--rw-r--r--   0 primoz     (501) staff       (20)      230 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/.buildinfo
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.995950 Orange3-Explain-0.6.2/doc/_build/html/_images/
--rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Model-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Model.png
--rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Prediction-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Prediction.png
--rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/ICE-example.png
--rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/ICE.png
--rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Permutation-Importance-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_images/Permutation-Importance.png
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.996120 Orange3-Explain-0.6.2/doc/_build/html/_sources/
--rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:02.997031 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-model.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-prediction.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-predictions.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/ice.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/permutation-importance.md.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.000687 Orange3-Explain-0.6.2/doc/_build/html/_static/
--rw-r--r--   0 primoz     (501) staff       (20)     4418 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 primoz     (501) staff       (20)    14621 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/basic.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.001022 Orange3-Explain-0.6.2/doc/_build/html/_static/css/
--rw-r--r--   0 primoz     (501) staff       (20)     3229 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.019085 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/
--rw-r--r--   0 primoz     (501) staff       (20)    87624 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)    67312 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)    86288 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 primoz     (501) staff       (20)    66444 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   165742 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 primoz     (501) staff       (20)   444379 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 primoz     (501) staff       (20)   165548 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 primoz     (501) staff       (20)    98024 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 primoz     (501) staff       (20)    77160 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   323344 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   193308 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309728 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)   184912 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   328412 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   195704 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309192 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 primoz     (501) staff       (20)   182708 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   131657 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/css/theme.css
--rw-r--r--   0 primoz     (501) staff       (20)      458 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/custom.css
--rw-r--r--   0 primoz     (501) staff       (20)     4472 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/doctools.js
--rw-r--r--   0 primoz     (501) staff       (20)      415 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 primoz     (501) staff       (20)      286 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/file.png
--rw-r--r--   0 primoz     (501) staff       (20)   288580 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 primoz     (501) staff       (20)    89501 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/jquery.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.020166 Orange3-Explain-0.6.2/doc/_build/html/_static/js/
--rw-r--r--   0 primoz     (501) staff       (20)      934 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/js/badge_only.js
--rw-r--r--   0 primoz     (501) staff       (20)     4370 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     2734 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     5023 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/js/theme.js
--rw-r--r--   0 primoz     (501) staff       (20)     4758 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/language_data.js
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/minus.png
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/plus.png
--rw-r--r--   0 primoz     (501) staff       (20)     4846 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/pygments.css
--rw-r--r--   0 primoz     (501) staff       (20)    18215 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 primoz     (501) staff       (20)     4712 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 primoz     (501) staff       (20)    68420 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 primoz     (501) staff       (20)    19530 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.2/doc/_build/html/_static/underscore.js
--rw-r--r--   0 primoz     (501) staff       (20)     3837 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/genindex.html
--rw-r--r--   0 primoz     (501) staff       (20)     5904 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/index.html
--rw-r--r--   0 primoz     (501) staff       (20)      351 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/objects.inv
--rw-r--r--   0 primoz     (501) staff       (20)     4236 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/search.html
--rw-r--r--   0 primoz     (501) staff       (20)     5924 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/searchindex.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.021018 Orange3-Explain-0.6.2/doc/_build/html/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     8808 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-model.html
--rw-r--r--   0 primoz     (501) staff       (20)    10517 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-prediction.html
--rw-r--r--   0 primoz     (501) staff       (20)     5716 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-predictions.html
--rw-r--r--   0 primoz     (501) staff       (20)     7150 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/widgets/ice.html
--rw-r--r--   0 primoz     (501) staff       (20)     7481 2022-12-15 11:23:49.000000 Orange3-Explain-0.6.2/doc/_build/html/widgets/permutation-importance.html
--rw-r--r--   0 primoz     (501) staff       (20)     9531 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/conf.py
--rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/index.rst
--rw-r--r--   0 primoz     (501) staff       (20)     7009 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/make.bat
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.022072 Orange3-Explain-0.6.2/doc/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/explain-model.md
--rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/explain-prediction.md
--rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/explain-predictions.md
--rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.2/doc/widgets/ice.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.028546 Orange3-Explain-0.6.2/doc/widgets/images/
--rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Explain-Model-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Explain-Model.png
--rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Explain-Prediction-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Explain-Prediction.png
--rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/widgets/images/ICE-example.png
--rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/doc/widgets/images/ICE.png
--rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Permutation-Importance-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/images/Permutation-Importance.png
--rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/doc/widgets/permutation-importance.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.028713 Orange3-Explain-0.6.2/orangecontrib/
--rw-r--r--   0 primoz     (501) staff       (20)      164 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.029183 Orange3-Explain-0.6.2/orangecontrib/explain/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    24334 2022-12-15 11:21:20.000000 Orange3-Explain-0.6.2/orangecontrib/explain/explainer.py
--rw-r--r--   0 primoz     (501) staff       (20)     7285 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/inspection.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.029650 Orange3-Explain-0.6.2/orangecontrib/explain/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    25379 2022-12-15 11:21:20.000000 Orange3-Explain-0.6.2/orangecontrib/explain/tests/test_explainer.py
--rw-r--r--   0 primoz     (501) staff       (20)    15039 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/tests/test_inspection.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.032228 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     1059 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.033192 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/
--rw-r--r--   0 primoz     (501) staff       (20)      738 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainModel.svg
--rw-r--r--   0 primoz     (501) staff       (20)      517 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainPred.svg
--rw-r--r--   0 primoz     (501) staff       (20)      842 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainPredictions.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1199 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ICE.svg
--rw-r--r--   0 primoz     (501) staff       (20)      595 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/PermutationImportance.svg
--rw-r--r--   0 primoz     (501) staff       (20)    24815 2022-10-27 09:59:01.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainfeaturebase.py
--rw-r--r--   0 primoz     (501) staff       (20)    19507 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainmodel.py
--rw-r--r--   0 primoz     (501) staff       (20)    27206 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainprediction.py
--rw-r--r--   0 primoz     (501) staff       (20)    32622 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainpredictions.py
--rw-r--r--   0 primoz     (501) staff       (20)    32238 2022-12-15 11:16:07.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owice.py
--rw-r--r--   0 primoz     (501) staff       (20)    14596 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owpermutationimportance.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-12-15 11:25:03.034323 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    17230 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainmodel.py
--rw-r--r--   0 primoz     (501) staff       (20)     9615 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainprediction.py
--rw-r--r--   0 primoz     (501) staff       (20)    21495 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py
--rw-r--r--   0 primoz     (501) staff       (20)     7859 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owice.py
--rw-r--r--   0 primoz     (501) staff       (20)    18373 2022-12-15 11:23:17.000000 Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py
--rw-r--r--   0 primoz     (501) staff       (20)       97 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.2/pyproject.toml
--rw-r--r--   0 primoz     (501) staff       (20)       38 2022-12-15 11:25:03.034833 Orange3-Explain-0.6.2/setup.cfg
--rw-r--r--   0 primoz     (501) staff       (20)     3075 2022-12-15 11:24:30.000000 Orange3-Explain-0.6.2/setup.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.945424 Orange3-Explain-0.6.3/
+-rw-r--r--   0 vesna      (501) staff       (20)      335 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/.coveragerc
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.828996 Orange3-Explain-0.6.3/.github/
+-rw-r--r--   0 vesna      (501) staff       (20)      646 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/.github/FUNDING.yml
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.830351 Orange3-Explain-0.6.3/.github/workflows/
+-rw-r--r--   0 vesna      (501) staff       (20)      175 2022-12-13 07:19:56.000000 Orange3-Explain-0.6.3/.github/workflows/rebase.yml
+-rw-r--r--   0 vesna      (501) staff       (20)      885 2023-04-14 08:02:30.000000 Orange3-Explain-0.6.3/.github/workflows/test.yml
+-rw-r--r--   0 vesna      (501) staff       (20)      211 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/.gitignore
+-rw-r--r--   0 vesna      (501) staff       (20)    35147 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/LICENSE.txt
+-rw-r--r--   0 vesna      (501) staff       (20)      127 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/MANIFEST.in
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.833356 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/
+-rw-r--r--   0 vesna      (501) staff       (20)     1202 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/PKG-INFO
+-rw-r--r--   0 vesna      (501) staff       (20)     5710 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/SOURCES.txt
+-rw-r--r--   0 vesna      (501) staff       (20)        1 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/dependency_links.txt
+-rw-r--r--   0 vesna      (501) staff       (20)      197 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/entry_points.txt
+-rw-r--r--   0 vesna      (501) staff       (20)       14 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/namespace_packages.txt
+-rw-r--r--   0 vesna      (501) staff       (20)        1 2020-12-23 08:41:31.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/not-zip-safe
+-rw-r--r--   0 vesna      (501) staff       (20)      164 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/requires.txt
+-rw-r--r--   0 vesna      (501) staff       (20)       14 2023-04-14 08:11:51.000000 Orange3-Explain-0.6.3/Orange3_Explain.egg-info/top_level.txt
+-rw-r--r--   0 vesna      (501) staff       (20)     1202 2023-04-14 08:11:51.945050 Orange3-Explain-0.6.3/PKG-INFO
+-rw-r--r--   0 vesna      (501) staff       (20)      735 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/README.md
+-rw-r--r--   0 vesna      (501) staff       (20)      545 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/README.pypi
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.835189 Orange3-Explain-0.6.3/doc/
+-rw-r--r--   0 vesna      (501) staff       (20)     7465 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/Makefile
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.820796 Orange3-Explain-0.6.3/doc/_build/
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.839061 Orange3-Explain-0.6.3/doc/_build/html/
+-rw-r--r--   0 vesna      (501) staff       (20)      230 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/.buildinfo
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.849830 Orange3-Explain-0.6.3/doc/_build/html/_images/
+-rw-r--r--   0 vesna      (501) staff       (20)   148240 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Model-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   184281 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Model.png
+-rw-r--r--   0 vesna      (501) staff       (20)   162676 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Prediction-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   186086 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Prediction.png
+-rw-r--r--   0 vesna      (501) staff       (20)    91768 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/ICE-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    70136 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/ICE.png
+-rw-r--r--   0 vesna      (501) staff       (20)    84574 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Permutation-Importance-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    28226 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/_build/html/_images/Permutation-Importance.png
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.850327 Orange3-Explain-0.6.3/doc/_build/html/_sources/
+-rw-r--r--   0 vesna      (501) staff       (20)      360 2022-08-03 08:51:25.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.853032 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/
+-rw-r--r--   0 vesna      (501) staff       (20)     3396 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-model.md.txt
+-rw-r--r--   0 vesna      (501) staff       (20)     4778 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-prediction.md.txt
+-rw-r--r--   0 vesna      (501) staff       (20)      770 2022-01-24 17:12:37.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-predictions.md.txt
+-rw-r--r--   0 vesna      (501) staff       (20)     1901 2022-10-18 11:03:44.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/ice.md.txt
+-rw-r--r--   0 vesna      (501) staff       (20)     2016 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/permutation-importance.md.txt
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.862513 Orange3-Explain-0.6.3/doc/_build/html/_static/
+-rw-r--r--   0 vesna      (501) staff       (20)    13647 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/basic.css
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.863765 Orange3-Explain-0.6.3/doc/_build/html/_static/css/
+-rw-r--r--   0 vesna      (501) staff       (20)     3275 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.893029 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/
+-rw-r--r--   0 vesna      (501) staff       (20)    87624 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 vesna      (501) staff       (20)    67312 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)    86288 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 vesna      (501) staff       (20)    66444 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   165742 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 vesna      (501) staff       (20)   444379 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 vesna      (501) staff       (20)   165548 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 vesna      (501) staff       (20)    98024 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 vesna      (501) staff       (20)    77160 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   323344 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 vesna      (501) staff       (20)   193308 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   309728 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 vesna      (501) staff       (20)   184912 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   328412 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 vesna      (501) staff       (20)   195704 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   309192 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 vesna      (501) staff       (20)   182708 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 vesna      (501) staff       (20)   129674 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/css/theme.css
+-rw-r--r--   0 vesna      (501) staff       (20)      458 2021-12-16 09:23:17.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/custom.css
+-rw-r--r--   0 vesna      (501) staff       (20)     9416 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 vesna      (501) staff       (20)      350 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 vesna      (501) staff       (20)      286 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/file.png
+-rw-r--r--   0 vesna      (501) staff       (20)   287630 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 vesna      (501) staff       (20)    89476 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/jquery.js
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.896724 Orange3-Explain-0.6.3/doc/_build/html/_static/js/
+-rw-r--r--   0 vesna      (501) staff       (20)      934 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 vesna      (501) staff       (20)     4370 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 vesna      (501) staff       (20)     2734 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 vesna      (501) staff       (20)     5023 2021-11-26 12:08:54.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/js/theme.js
+-rw-r--r--   0 vesna      (501) staff       (20)    10847 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 vesna      (501) staff       (20)       90 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/minus.png
+-rw-r--r--   0 vesna      (501) staff       (20)       90 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/plus.png
+-rw-r--r--   0 vesna      (501) staff       (20)     4846 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 vesna      (501) staff       (20)    16323 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 vesna      (501) staff       (20)    35168 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 vesna      (501) staff       (20)    12140 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/html/_static/underscore.js
+-rw-r--r--   0 vesna      (501) staff       (20)     3713 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/genindex.html
+-rw-r--r--   0 vesna      (501) staff       (20)     5780 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/index.html
+-rw-r--r--   0 vesna      (501) staff       (20)      351 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/objects.inv
+-rw-r--r--   0 vesna      (501) staff       (20)     4112 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/search.html
+-rw-r--r--   0 vesna      (501) staff       (20)     3817 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/searchindex.js
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.898783 Orange3-Explain-0.6.3/doc/_build/html/widgets/
+-rw-r--r--   0 vesna      (501) staff       (20)     8599 2022-04-20 06:00:25.000000 Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-model.html
+-rw-r--r--   0 vesna      (501) staff       (20)    10308 2022-04-20 06:00:25.000000 Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-prediction.html
+-rw-r--r--   0 vesna      (501) staff       (20)     5280 2022-04-20 06:00:25.000000 Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-predictions.html
+-rw-r--r--   0 vesna      (501) staff       (20)     7023 2022-10-20 07:55:22.000000 Orange3-Explain-0.6.3/doc/_build/html/widgets/ice.html
+-rw-r--r--   0 vesna      (501) staff       (20)     7272 2022-04-20 06:00:25.000000 Orange3-Explain-0.6.3/doc/_build/html/widgets/permutation-importance.html
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.821039 Orange3-Explain-0.6.3/doc/_build/htmlhelp/
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.908230 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/
+-rw-r--r--   0 vesna      (501) staff       (20)   148240 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Model-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   184281 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Model.png
+-rw-r--r--   0 vesna      (501) staff       (20)   162676 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Prediction-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   186086 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Prediction.png
+-rw-r--r--   0 vesna      (501) staff       (20)    91768 2022-08-03 11:28:34.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/ICE-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    70136 2022-08-03 11:28:34.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/ICE.png
+-rw-r--r--   0 vesna      (501) staff       (20)    84574 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Permutation-Importance-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    28226 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Permutation-Importance.png
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.909777 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_static/
+-rw-r--r--   0 vesna      (501) staff       (20)      286 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_static/file.png
+-rw-r--r--   0 vesna      (501) staff       (20)       90 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_static/minus.png
+-rw-r--r--   0 vesna      (501) staff       (20)       90 2020-11-25 08:41:53.000000 Orange3-Explain-0.6.3/doc/_build/htmlhelp/_static/plus.png
+-rw-r--r--   0 vesna      (501) staff       (20)     9531 2021-12-16 09:23:17.000000 Orange3-Explain-0.6.3/doc/conf.py
+-rw-r--r--   0 vesna      (501) staff       (20)      360 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/doc/index.rst
+-rw-r--r--   0 vesna      (501) staff       (20)     7009 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/make.bat
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.910112 Orange3-Explain-0.6.3/doc/static/
+-rw-r--r--   0 vesna      (501) staff       (20)      458 2021-12-16 09:23:17.000000 Orange3-Explain-0.6.3/doc/static/custom.css
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.912691 Orange3-Explain-0.6.3/doc/widgets/
+-rw-r--r--   0 vesna      (501) staff       (20)     3396 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/explain-model.md
+-rw-r--r--   0 vesna      (501) staff       (20)     4778 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/explain-prediction.md
+-rw-r--r--   0 vesna      (501) staff       (20)      770 2022-01-24 17:12:37.000000 Orange3-Explain-0.6.3/doc/widgets/explain-predictions.md
+-rw-r--r--   0 vesna      (501) staff       (20)     1901 2022-10-18 11:03:44.000000 Orange3-Explain-0.6.3/doc/widgets/ice.md
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.924858 Orange3-Explain-0.6.3/doc/widgets/images/
+-rw-r--r--   0 vesna      (501) staff       (20)   148240 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/images/Explain-Model-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   184281 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/images/Explain-Model.png
+-rw-r--r--   0 vesna      (501) staff       (20)   162676 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/images/Explain-Prediction-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)   186086 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/doc/widgets/images/Explain-Prediction.png
+-rw-r--r--   0 vesna      (501) staff       (20)    91768 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/doc/widgets/images/ICE-example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    70136 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/doc/widgets/images/ICE.png
+-rw-r--r--   0 vesna      (501) staff       (20)    84574 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/widgets/images/Permutation-Importance-Example.png
+-rw-r--r--   0 vesna      (501) staff       (20)    28226 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/widgets/images/Permutation-Importance.png
+-rw-r--r--   0 vesna      (501) staff       (20)     2016 2021-05-25 09:41:33.000000 Orange3-Explain-0.6.3/doc/widgets/permutation-importance.md
+-rw-r--r--   0 vesna      (501) staff       (20)     1399 2022-10-18 11:03:44.000000 Orange3-Explain-0.6.3/doc/widgets.json
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.925625 Orange3-Explain-0.6.3/orangecontrib/
+-rw-r--r--   0 vesna      (501) staff       (20)      164 2021-12-21 07:01:31.000000 Orange3-Explain-0.6.3/orangecontrib/__init__.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.926924 Orange3-Explain-0.6.3/orangecontrib/explain/
+-rw-r--r--   0 vesna      (501) staff       (20)        0 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/__init__.py
+-rw-r--r--   0 vesna      (501) staff       (20)    24970 2023-04-14 08:02:30.000000 Orange3-Explain-0.6.3/orangecontrib/explain/explainer.py
+-rw-r--r--   0 vesna      (501) staff       (20)     7285 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/inspection.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.928684 Orange3-Explain-0.6.3/orangecontrib/explain/tests/
+-rw-r--r--   0 vesna      (501) staff       (20)        0 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/orangecontrib/explain/tests/__init__.py
+-rw-r--r--   0 vesna      (501) staff       (20)    29073 2023-04-14 08:02:30.000000 Orange3-Explain-0.6.3/orangecontrib/explain/tests/test_explainer.py
+-rw-r--r--   0 vesna      (501) staff       (20)    15039 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/tests/test_inspection.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.936363 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/
+-rw-r--r--   0 vesna      (501) staff       (20)     1059 2021-12-16 09:23:17.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/__init__.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.939462 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/
+-rw-r--r--   0 vesna      (501) staff       (20)      738 2022-01-20 14:37:00.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainModel.svg
+-rw-r--r--   0 vesna      (501) staff       (20)      517 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainPred.svg
+-rw-r--r--   0 vesna      (501) staff       (20)      842 2022-01-21 13:07:24.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainPredictions.svg
+-rw-r--r--   0 vesna      (501) staff       (20)     1199 2022-08-04 05:59:33.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ICE.svg
+-rw-r--r--   0 vesna      (501) staff       (20)      595 2021-03-18 07:40:02.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/PermutationImportance.svg
+-rw-r--r--   0 vesna      (501) staff       (20)    24815 2022-12-13 11:22:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainfeaturebase.py
+-rw-r--r--   0 vesna      (501) staff       (20)    19507 2022-12-13 12:26:57.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainmodel.py
+-rw-r--r--   0 vesna      (501) staff       (20)    27206 2022-12-13 07:19:56.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainprediction.py
+-rw-r--r--   0 vesna      (501) staff       (20)    32622 2022-04-19 08:42:40.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainpredictions.py
+-rw-r--r--   0 vesna      (501) staff       (20)    32238 2022-12-14 12:29:03.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owice.py
+-rw-r--r--   0 vesna      (501) staff       (20)    14596 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owpermutationimportance.py
+-rw-r--r--   0 vesna      (501) staff       (20)    11197 2021-12-17 11:01:34.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/shap_debug.py
+drwxr-xr-x   0 vesna      (501) staff       (20)        0 2023-04-14 08:11:51.944042 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/
+-rw-r--r--   0 vesna      (501) staff       (20)        0 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/__init__.py
+-rw-r--r--   0 vesna      (501) staff       (20)    17230 2022-12-13 07:19:56.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainmodel.py
+-rw-r--r--   0 vesna      (501) staff       (20)     9615 2022-04-08 13:08:33.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainprediction.py
+-rw-r--r--   0 vesna      (501) staff       (20)    21495 2022-04-19 08:42:40.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py
+-rw-r--r--   0 vesna      (501) staff       (20)     7859 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owice.py
+-rw-r--r--   0 vesna      (501) staff       (20)    18373 2022-12-16 10:10:14.000000 Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py
+-rw-r--r--   0 vesna      (501) staff       (20)       97 2020-12-23 08:39:44.000000 Orange3-Explain-0.6.3/pyproject.toml
+-rw-r--r--   0 vesna      (501) staff       (20)       38 2023-04-14 08:11:51.945510 Orange3-Explain-0.6.3/setup.cfg
+-rw-r--r--   0 vesna      (501) staff       (20)     3075 2023-04-14 08:10:11.000000 Orange3-Explain-0.6.3/setup.py
+-rw-r--r--   0 vesna      (501) staff       (20)     1426 2023-04-14 08:02:30.000000 Orange3-Explain-0.6.3/tox.ini
```

### Comparing `Orange3-Explain-0.6.2/LICENSE.txt` & `Orange3-Explain-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/Orange3_Explain.egg-info/PKG-INFO` & `Orange3-Explain-0.6.3/Orange3_Explain.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: Orange3-Explain
-Version: 0.6.2
+Version: 0.6.3
 Summary: Orange3 add-on for explanatory AI
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
+Description: Orange3 Explain
+        ===============
+        
+        Orange3 Explain is an add-on for the [Orange3](http://orange.biolab.si)
+        data mining suite. It provides extensions for explanatory AI.
+        See [documentation](http://orange3-explain.readthedocs.org/).
+        
+        Features
+        --------
+        - Explains a classification or regression model. Explains which features
+          contribute the most and how they contribute toward the prediction for a
+          specific class.
+        - Explains which features contribute the most to the prediction for a single
+          instance based on the model and how they contribute.
+        
 Keywords: orange3 add-on,orange3-explain
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
-License-File: LICENSE.txt
-
-Orange3 Explain
-===============
-
-Orange3 Explain is an add-on for the [Orange3](http://orange.biolab.si)
-data mining suite. It provides extensions for explanatory AI.
-See [documentation](http://orange3-explain.readthedocs.org/).
-
-Features
---------
-- Explains a classification or regression model. Explains which features
-  contribute the most and how they contribute toward the prediction for a
-  specific class.
-- Explains which features contribute the most to the prediction for a single
-  instance based on the model and how they contribute.
```

### Comparing `Orange3-Explain-0.6.2/Orange3_Explain.egg-info/SOURCES.txt` & `Orange3-Explain-0.6.3/Orange3_Explain.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,65 @@
+.coveragerc
+.gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
 README.pypi
 pyproject.toml
 setup.py
+tox.ini
+.github/FUNDING.yml
+.github/workflows/rebase.yml
+.github/workflows/test.yml
 Orange3_Explain.egg-info/PKG-INFO
 Orange3_Explain.egg-info/SOURCES.txt
 Orange3_Explain.egg-info/dependency_links.txt
 Orange3_Explain.egg-info/entry_points.txt
 Orange3_Explain.egg-info/namespace_packages.txt
 Orange3_Explain.egg-info/not-zip-safe
 Orange3_Explain.egg-info/requires.txt
 Orange3_Explain.egg-info/top_level.txt
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/make.bat
+doc/widgets.json
 doc/_build/html/.buildinfo
 doc/_build/html/genindex.html
 doc/_build/html/index.html
 doc/_build/html/objects.inv
 doc/_build/html/search.html
 doc/_build/html/searchindex.js
 doc/_build/html/_images/Explain-Model-Example.png
 doc/_build/html/_images/Explain-Model.png
 doc/_build/html/_images/Explain-Prediction-Example.png
 doc/_build/html/_images/Explain-Prediction.png
-doc/_build/html/_images/ICE-example.png
+doc/_build/html/_images/ICE-Example.png
 doc/_build/html/_images/ICE.png
 doc/_build/html/_images/Permutation-Importance-Example.png
 doc/_build/html/_images/Permutation-Importance.png
 doc/_build/html/_sources/index.rst.txt
 doc/_build/html/_sources/widgets/explain-model.md.txt
 doc/_build/html/_sources/widgets/explain-prediction.md.txt
 doc/_build/html/_sources/widgets/explain-predictions.md.txt
 doc/_build/html/_sources/widgets/ice.md.txt
 doc/_build/html/_sources/widgets/permutation-importance.md.txt
-doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
 doc/_build/html/_static/basic.css
 doc/_build/html/_static/custom.css
 doc/_build/html/_static/doctools.js
 doc/_build/html/_static/documentation_options.js
 doc/_build/html/_static/file.png
-doc/_build/html/_static/jquery-3.6.0.js
+doc/_build/html/_static/jquery-3.5.1.js
 doc/_build/html/_static/jquery.js
 doc/_build/html/_static/language_data.js
 doc/_build/html/_static/minus.png
 doc/_build/html/_static/plus.png
 doc/_build/html/_static/pygments.css
 doc/_build/html/_static/searchtools.js
-doc/_build/html/_static/sphinx_highlight.js
-doc/_build/html/_static/underscore-1.13.1.js
+doc/_build/html/_static/underscore-1.3.1.js
 doc/_build/html/_static/underscore.js
 doc/_build/html/_static/css/badge_only.css
 doc/_build/html/_static/css/theme.css
 doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
 doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
 doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
 doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
@@ -76,14 +81,26 @@
 doc/_build/html/_static/js/html5shiv.min.js
 doc/_build/html/_static/js/theme.js
 doc/_build/html/widgets/explain-model.html
 doc/_build/html/widgets/explain-prediction.html
 doc/_build/html/widgets/explain-predictions.html
 doc/_build/html/widgets/ice.html
 doc/_build/html/widgets/permutation-importance.html
+doc/_build/htmlhelp/_images/Explain-Model-Example.png
+doc/_build/htmlhelp/_images/Explain-Model.png
+doc/_build/htmlhelp/_images/Explain-Prediction-Example.png
+doc/_build/htmlhelp/_images/Explain-Prediction.png
+doc/_build/htmlhelp/_images/ICE-Example.png
+doc/_build/htmlhelp/_images/ICE.png
+doc/_build/htmlhelp/_images/Permutation-Importance-Example.png
+doc/_build/htmlhelp/_images/Permutation-Importance.png
+doc/_build/htmlhelp/_static/file.png
+doc/_build/htmlhelp/_static/minus.png
+doc/_build/htmlhelp/_static/plus.png
+doc/static/custom.css
 doc/widgets/explain-model.md
 doc/widgets/explain-prediction.md
 doc/widgets/explain-predictions.md
 doc/widgets/ice.md
 doc/widgets/permutation-importance.md
 doc/widgets/images/Explain-Model-Example.png
 doc/widgets/images/Explain-Model.png
@@ -103,14 +120,15 @@
 orangecontrib/explain/widgets/__init__.py
 orangecontrib/explain/widgets/owexplainfeaturebase.py
 orangecontrib/explain/widgets/owexplainmodel.py
 orangecontrib/explain/widgets/owexplainprediction.py
 orangecontrib/explain/widgets/owexplainpredictions.py
 orangecontrib/explain/widgets/owice.py
 orangecontrib/explain/widgets/owpermutationimportance.py
+orangecontrib/explain/widgets/shap_debug.py
 orangecontrib/explain/widgets/icons/ExplainModel.svg
 orangecontrib/explain/widgets/icons/ExplainPred.svg
 orangecontrib/explain/widgets/icons/ExplainPredictions.svg
 orangecontrib/explain/widgets/icons/ICE.svg
 orangecontrib/explain/widgets/icons/PermutationImportance.svg
 orangecontrib/explain/widgets/tests/__init__.py
 orangecontrib/explain/widgets/tests/test_owexplainmodel.py
```

### Comparing `Orange3-Explain-0.6.2/PKG-INFO` & `Orange3-Explain-0.6.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: Orange3-Explain
-Version: 0.6.2
+Version: 0.6.3
 Summary: Orange3 add-on for explanatory AI
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
+Description: Orange3 Explain
+        ===============
+        
+        Orange3 Explain is an add-on for the [Orange3](http://orange.biolab.si)
+        data mining suite. It provides extensions for explanatory AI.
+        See [documentation](http://orange3-explain.readthedocs.org/).
+        
+        Features
+        --------
+        - Explains a classification or regression model. Explains which features
+          contribute the most and how they contribute toward the prediction for a
+          specific class.
+        - Explains which features contribute the most to the prediction for a single
+          instance based on the model and how they contribute.
+        
 Keywords: orange3 add-on,orange3-explain
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
-License-File: LICENSE.txt
-
-Orange3 Explain
-===============
-
-Orange3 Explain is an add-on for the [Orange3](http://orange.biolab.si)
-data mining suite. It provides extensions for explanatory AI.
-See [documentation](http://orange3-explain.readthedocs.org/).
-
-Features
---------
-- Explains a classification or regression model. Explains which features
-  contribute the most and how they contribute toward the prediction for a
-  specific class.
-- Explains which features contribute the most to the prediction for a single
-  instance based on the model and how they contribute.
```

### Comparing `Orange3-Explain-0.6.2/README.md` & `Orange3-Explain-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/README.pypi` & `Orange3-Explain-0.6.3/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/Makefile` & `Orange3-Explain-0.6.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Model-Example.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Model-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Model.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Model.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Prediction-Example.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Prediction-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Explain-Prediction.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Explain-Prediction.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/ICE-example.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/ICE-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/ICE.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/ICE.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Permutation-Importance-Example.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Permutation-Importance-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_images/Permutation-Importance.png` & `Orange3-Explain-0.6.3/doc/_build/html/_images/Permutation-Importance.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-model.md.txt` & `Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-model.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-prediction.md.txt` & `Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-prediction.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/explain-predictions.md.txt` & `Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/explain-predictions.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/ice.md.txt` & `Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/ice.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_sources/widgets/permutation-importance.md.txt` & `Orange3-Explain-0.6.3/doc/_build/html/_sources/widgets/permutation-importance.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/basic.css` & `Orange3-Explain-0.6.3/doc/_build/html/_static/basic.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2020 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -126,15 +126,15 @@
     background-position: 0 7px;
 }
 
 ul.search li a {
     font-weight: bold;
 }
 
-ul.search li p.context {
+ul.search li div.context {
     color: #888;
     margin: 2px 0 0 30px;
     text-align: left;
 }
 
 ul.keywordmatches li.goodmatch a {
     font-weight: bold;
@@ -218,39 +218,39 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 360px;
+    min-width: 450px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
+
 a.brackets:before,
 span.brackets > a:before{
     content: "[";
 }
 
 a.brackets:after,
 span.brackets > a:after {
     content: "]";
 }
 
-
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -273,33 +273,33 @@
 }
 
 p.rubric {
     margin-top: 30px;
     font-weight: bold;
 }
 
-img.align-left, figure.align-left, .figure.align-left, object.align-left {
+img.align-left, .figure.align-left, object.align-left {
     clear: left;
     float: left;
     margin-right: 1em;
 }
 
-img.align-right, figure.align-right, .figure.align-right, object.align-right {
+img.align-right, .figure.align-right, object.align-right {
     clear: right;
     float: right;
     margin-left: 1em;
 }
 
-img.align-center, figure.align-center, .figure.align-center, object.align-center {
+img.align-center, .figure.align-center, object.align-center {
   display: block;
   margin-left: auto;
   margin-right: auto;
 }
 
-img.align-default, figure.align-default, .figure.align-default {
+img.align-default, .figure.align-default {
   display: block;
   margin-left: auto;
   margin-right: auto;
 }
 
 .align-left {
     text-align: left;
@@ -315,34 +315,35 @@
 
 .align-right {
     text-align: right;
 }
 
 /* -- sidebars -------------------------------------------------------------- */
 
-div.sidebar,
-aside.sidebar {
+div.sidebar {
     margin: 0 0 0.5em 1em;
     border: 1px solid #ddb;
     padding: 7px;
     background-color: #ffe;
     width: 40%;
     float: right;
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
+
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
+
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -372,22 +373,20 @@
     text-align: center;
     margin-top: 25px;
 }
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
-aside.sidebar > :last-child,
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
-aside.sidebar::after,
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -422,14 +421,18 @@
     padding: 1px 8px 1px 5px;
     border-top: 0;
     border-left: 0;
     border-right: 0;
     border-bottom: 1px solid #aaa;
 }
 
+table.footnote td, table.footnote th {
+    border: 0 !important;
+}
+
 th {
     text-align: left;
     padding-right: 5px;
 }
 
 table.citation {
     border-left: solid 1px gray;
@@ -448,30 +451,28 @@
 th > :last-child,
 td > :last-child {
     margin-bottom: 0px;
 }
 
 /* -- figures --------------------------------------------------------------- */
 
-div.figure, figure {
+div.figure {
     margin: 0.5em;
     padding: 0.5em;
 }
 
-div.figure p.caption, figcaption {
+div.figure p.caption {
     padding: 0.3em;
 }
 
-div.figure p.caption span.caption-number,
-figcaption span.caption-number {
+div.figure p.caption span.caption-number {
     font-style: italic;
 }
 
-div.figure p.caption span.caption-text,
-figcaption span.caption-text {
+div.figure p.caption span.caption-text {
 }
 
 /* -- field list styles ----------------------------------------------------- */
 
 table.field-list td, table.field-list th {
     border: 0 !important;
 }
@@ -498,71 +499,14 @@
     margin: 1em 0;
 }
 
 table.hlist td {
     vertical-align: top;
 }
 
-/* -- object description styles --------------------------------------------- */
-
-.sig {
-	font-family: 'Consolas', 'Menlo', 'DejaVu Sans Mono', 'Bitstream Vera Sans Mono', monospace;
-}
-
-.sig-name, code.descname {
-    background-color: transparent;
-    font-weight: bold;
-}
-
-.sig-name {
-	font-size: 1.1em;
-}
-
-code.descname {
-    font-size: 1.2em;
-}
-
-.sig-prename, code.descclassname {
-    background-color: transparent;
-}
-
-.optional {
-    font-size: 1.3em;
-}
-
-.sig-paren {
-    font-size: larger;
-}
-
-.sig-param.n {
-	font-style: italic;
-}
-
-/* C++ specific styling */
-
-.sig-inline.c-texpr,
-.sig-inline.cpp-texpr {
-	font-family: unset;
-}
-
-.sig.c   .k, .sig.c   .kt,
-.sig.cpp .k, .sig.cpp .kt {
-	color: #0033B3;
-}
-
-.sig.c   .m,
-.sig.cpp .m {
-	color: #1750EB;
-}
-
-.sig.c   .s, .sig.c   .sc,
-.sig.cpp .s, .sig.cpp .sc {
-	color: #067D17;
-}
-
 
 /* -- other body styles ----------------------------------------------------- */
 
 ol.arabic {
     list-style: decimal;
 }
 
@@ -604,14 +548,15 @@
     margin-top: 0;
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
+
 dl.footnote > dt,
 dl.citation > dt {
     float: left;
     margin-right: 0.5em;
 }
 
 dl.footnote > dd,
@@ -632,19 +577,19 @@
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
+
 dl.field-list > dt:after {
     content: ":";
 }
 
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
 
@@ -680,14 +625,22 @@
 }
 
 dl.glossary dt {
     font-weight: bold;
     font-size: 1.1em;
 }
 
+.optional {
+    font-size: 1.3em;
+}
+
+.sig-paren {
+    font-size: larger;
+}
+
 .versionmodified {
     font-style: italic;
 }
 
 .system-message {
     background-color: #fda;
     padding: 5px;
@@ -720,17 +673,16 @@
 
 .classifier {
     font-style: oblique;
 }
 
 .classifier:before {
     font-style: normal;
-    margin: 0 0.5em;
+    margin: 0.5em;
     content: ":";
-    display: inline-block;
 }
 
 abbr, acronym {
     border-bottom: dotted 1px;
     cursor: help;
 }
 
@@ -746,15 +698,14 @@
 }
 
 span.pre {
     -moz-hyphens: none;
     -ms-hyphens: none;
     -webkit-hyphens: none;
     hyphens: none;
-    white-space: nowrap;
 }
 
 div[class*="highlight-"] {
     margin: 1em 0;
 }
 
 td.linenos pre {
@@ -810,34 +761,40 @@
 
 div.code-block-caption code {
     background-color: transparent;
 }
 
 table.highlighttable td.linenos,
 span.linenos,
-div.highlight span.gp {  /* gp: Generic.Prompt */
-  user-select: none;
-  -webkit-user-select: text; /* Safari fallback only */
-  -webkit-user-select: none; /* Chrome/Safari */
-  -moz-user-select: none; /* Firefox */
-  -ms-user-select: none; /* IE10+ */
+div.doctest > div.highlight span.gp {  /* gp: Generic.Prompt */
+    user-select: none;
 }
 
 div.code-block-caption span.caption-number {
     padding: 0.1em 0.3em;
     font-style: italic;
 }
 
 div.code-block-caption span.caption-text {
 }
 
 div.literal-block-wrapper {
     margin: 1em 0;
 }
 
+code.descname {
+    background-color: transparent;
+    font-weight: bold;
+    font-size: 1.2em;
+}
+
+code.descclassname {
+    background-color: transparent;
+}
+
 code.xref, a code {
     background-color: transparent;
     font-weight: bold;
 }
 
 h1 code, h2 code, h3 code, h4 code, h5 code, h6 code {
     background-color: transparent;
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/badge_only.css` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/badge_only.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:FontAwesome;font-style:normal;font-weight:400;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#FontAwesome) format("svg")}.fa:before{font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1}.fa:before,a .fa{text-decoration:inherit}.fa:before,a .fa,li .fa{display:inline-block}li .fa-large:before{width:1.875em}ul.fas{list-style-type:none;margin-left:2em;text-indent:-.8em}ul.fas li .fa{width:.8em}ul.fas li .fa-large:before{vertical-align:baseline}.fa-book:before,.icon-book:before{content:"\f02d"}.fa-caret-down:before,.icon-caret-down:before{content:"\f0d7"}.fa-caret-up:before,.icon-caret-up:before{content:"\f0d8"}.fa-caret-left:before,.icon-caret-left:before{content:"\f0d9"}.fa-caret-right:before,.icon-caret-right:before{content:"\f0da"}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60}.rst-versions .rst-current-version:after{clear:both;content:"";display:block}.rst-versions .rst-current-version .fa{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}
+.fa:before{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:FontAwesome;font-style:normal;font-weight:400;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#FontAwesome) format("svg")}.fa:before{font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1}.fa:before,a .fa{text-decoration:inherit}.fa:before,a .fa,li .fa{display:inline-block}li .fa-large:before{width:1.875em}ul.fas{list-style-type:none;margin-left:2em;text-indent:-.8em}ul.fas li .fa{width:.8em}ul.fas li .fa-large:before{vertical-align:baseline}.fa-book:before,.icon-book:before{content:"\f02d"}.fa-caret-down:before,.icon-caret-down:before{content:"\f0d7"}.fa-caret-up:before,.icon-caret-up:before{content:"\f0d8"}.fa-caret-left:before,.icon-caret-left:before{content:"\f0d9"}.fa-caret-right:before,.icon-caret-right:before{content:"\f0da"}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60}.rst-versions .rst-current-version:after{clear:both;content:"";display:block}.rst-versions .rst-current-version .fa{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold-italic.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-bold.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal-italic.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal.woff` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/fonts/lato-normal.woff2` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/css/theme.css` & `Orange3-Explain-0.6.3/doc/_build/html/_static/css/theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,4 +1,4 @@
-html{box-sizing:border-box}*,:after,:before{box-sizing:inherit}article,aside,details,figcaption,figure,footer,header,hgroup,nav,section{display:block}audio,canvas,video{display:inline-block;*display:inline;*zoom:1}[hidden],audio:not([controls]){display:none}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}blockquote{margin:0}dfn{font-style:italic}ins{background:#ff9;text-decoration:none}ins,mark{color:#000}mark{background:#ff0;font-style:italic;font-weight:700}.rst-content code,.rst-content tt,code,kbd,pre,samp{font-family:monospace,serif;_font-family:courier new,monospace;font-size:1em}pre{white-space:pre}q{quotes:none}q:after,q:before{content:"";content:none}small{font-size:85%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}dl,ol,ul{margin:0;padding:0;list-style:none;list-style-image:none}li{list-style:none}dd{margin:0}img{border:0;-ms-interpolation-mode:bicubic;vertical-align:middle;max-width:100%}svg:not(:root){overflow:hidden}figure,form{margin:0}label{cursor:pointer}button,input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}button,input{line-height:normal}button,input[type=button],input[type=reset],input[type=submit]{cursor:pointer;-webkit-appearance:button;*overflow:visible}button[disabled],input[disabled]{cursor:default}input[type=search]{-webkit-appearance:textfield;-moz-box-sizing:content-box;-webkit-box-sizing:content-box;box-sizing:content-box}textarea{resize:vertical}table{border-collapse:collapse;border-spacing:0}td{vertical-align:top}.chromeframe{margin:.2em 0;background:#ccc;color:#000;padding:.2em 0}.ir{display:block;border:0;text-indent:-999em;overflow:hidden;background-color:transparent;background-repeat:no-repeat;text-align:left;direction:ltr;*line-height:0}.ir br{display:none}.hidden{display:none!important;visibility:hidden}.visuallyhidden{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.visuallyhidden.focusable:active,.visuallyhidden.focusable:focus{clip:auto;height:auto;margin:0;overflow:visible;position:static;width:auto}.invisible{visibility:hidden}.relative{position:relative}big,small{font-size:100%}@media print{body,html,section{background:none!important}*{box-shadow:none!important;text-shadow:none!important;filter:none!important;-ms-filter:none!important}a,a:visited{text-decoration:underline}.ir a:after,a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}@page{margin:.5cm}.rst-content .toctree-wrapper>p.caption,h2,h3,p{orphans:3;widows:3}.rst-content .toctree-wrapper>p.caption,h2,h3{page-break-after:avoid}}.btn,.fa:before,.icon:before,.rst-content .admonition,.rst-content .admonition-title:before,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .code-block-caption .headerlink:before,.rst-content .danger,.rst-content .eqno .headerlink:before,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-alert,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before,input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week],select,textarea{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}/*!
+html{box-sizing:border-box}*,:after,:before{box-sizing:inherit}article,aside,details,figcaption,figure,footer,header,hgroup,nav,section{display:block}audio,canvas,video{display:inline-block;*display:inline;*zoom:1}[hidden],audio:not([controls]){display:none}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}blockquote{margin:0}dfn{font-style:italic}ins{background:#ff9;text-decoration:none}ins,mark{color:#000}mark{background:#ff0;font-style:italic;font-weight:700}.rst-content code,.rst-content tt,code,kbd,pre,samp{font-family:monospace,serif;_font-family:courier new,monospace;font-size:1em}pre{white-space:pre}q{quotes:none}q:after,q:before{content:"";content:none}small{font-size:85%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}dl,ol,ul{margin:0;padding:0;list-style:none;list-style-image:none}li{list-style:none}dd{margin:0}img{border:0;-ms-interpolation-mode:bicubic;vertical-align:middle;max-width:100%}svg:not(:root){overflow:hidden}figure,form{margin:0}label{cursor:pointer}button,input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}button,input{line-height:normal}button,input[type=button],input[type=reset],input[type=submit]{cursor:pointer;-webkit-appearance:button;*overflow:visible}button[disabled],input[disabled]{cursor:default}input[type=search]{-webkit-appearance:textfield;-moz-box-sizing:content-box;-webkit-box-sizing:content-box;box-sizing:content-box}textarea{resize:vertical}table{border-collapse:collapse;border-spacing:0}td{vertical-align:top}.chromeframe{margin:.2em 0;background:#ccc;color:#000;padding:.2em 0}.ir{display:block;border:0;text-indent:-999em;overflow:hidden;background-color:transparent;background-repeat:no-repeat;text-align:left;direction:ltr;*line-height:0}.ir br{display:none}.hidden{display:none!important;visibility:hidden}.visuallyhidden{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.visuallyhidden.focusable:active,.visuallyhidden.focusable:focus{clip:auto;height:auto;margin:0;overflow:visible;position:static;width:auto}.invisible{visibility:hidden}.relative{position:relative}big,small{font-size:100%}@media print{body,html,section{background:none!important}*{box-shadow:none!important;text-shadow:none!important;filter:none!important;-ms-filter:none!important}a,a:visited{text-decoration:underline}.ir a:after,a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}@page{margin:.5cm}.rst-content .toctree-wrapper>p.caption,h2,h3,p{orphans:3;widows:3}.rst-content .toctree-wrapper>p.caption,h2,h3{page-break-after:avoid}}.btn,.fa:before,.icon:before,.rst-content .admonition,.rst-content .admonition-title:before,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .code-block-caption .headerlink:before,.rst-content .danger,.rst-content .eqno .headerlink:before,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-alert,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before,.wy-nav-top a,.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a,input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week],select,textarea{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}/*!
  *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
  *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
- */@font-face{font-family:FontAwesome;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713);src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix&v=4.7.0) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#fontawesomeregular) format("svg");font-weight:400;font-style:normal}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{display:inline-block;font:normal normal normal 14px/1 FontAwesome;font-size:inherit;text-rendering:auto;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.fa-lg{font-size:1.33333em;line-height:.75em;vertical-align:-15%}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-fw{width:1.28571em;text-align:center}.fa-ul{padding-left:0;margin-left:2.14286em;list-style-type:none}.fa-ul>li{position:relative}.fa-li{position:absolute;left:-2.14286em;width:2.14286em;top:.14286em;text-align:center}.fa-li.fa-lg{left:-1.85714em}.fa-border{padding:.2em .25em .15em;border:.08em solid #eee;border-radius:.1em}.fa-pull-left{float:left}.fa-pull-right{float:right}.fa-pull-left.icon,.fa.fa-pull-left,.rst-content .code-block-caption .fa-pull-left.headerlink,.rst-content .eqno .fa-pull-left.headerlink,.rst-content .fa-pull-left.admonition-title,.rst-content code.download span.fa-pull-left:first-child,.rst-content dl dt .fa-pull-left.headerlink,.rst-content h1 .fa-pull-left.headerlink,.rst-content h2 .fa-pull-left.headerlink,.rst-content h3 .fa-pull-left.headerlink,.rst-content h4 .fa-pull-left.headerlink,.rst-content h5 .fa-pull-left.headerlink,.rst-content h6 .fa-pull-left.headerlink,.rst-content p .fa-pull-left.headerlink,.rst-content table>caption .fa-pull-left.headerlink,.rst-content tt.download span.fa-pull-left:first-child,.wy-menu-vertical li.current>a button.fa-pull-left.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-left.toctree-expand,.wy-menu-vertical li button.fa-pull-left.toctree-expand{margin-right:.3em}.fa-pull-right.icon,.fa.fa-pull-right,.rst-content .code-block-caption .fa-pull-right.headerlink,.rst-content .eqno .fa-pull-right.headerlink,.rst-content .fa-pull-right.admonition-title,.rst-content code.download span.fa-pull-right:first-child,.rst-content dl dt .fa-pull-right.headerlink,.rst-content h1 .fa-pull-right.headerlink,.rst-content h2 .fa-pull-right.headerlink,.rst-content h3 .fa-pull-right.headerlink,.rst-content h4 .fa-pull-right.headerlink,.rst-content h5 .fa-pull-right.headerlink,.rst-content h6 .fa-pull-right.headerlink,.rst-content p .fa-pull-right.headerlink,.rst-content table>caption .fa-pull-right.headerlink,.rst-content tt.download span.fa-pull-right:first-child,.wy-menu-vertical li.current>a button.fa-pull-right.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-right.toctree-expand,.wy-menu-vertical li button.fa-pull-right.toctree-expand{margin-left:.3em}.pull-right{float:right}.pull-left{float:left}.fa.pull-left,.pull-left.icon,.rst-content .code-block-caption .pull-left.headerlink,.rst-content .eqno .pull-left.headerlink,.rst-content .pull-left.admonition-title,.rst-content code.download span.pull-left:first-child,.rst-content dl dt .pull-left.headerlink,.rst-content h1 .pull-left.headerlink,.rst-content h2 .pull-left.headerlink,.rst-content h3 .pull-left.headerlink,.rst-content h4 .pull-left.headerlink,.rst-content h5 .pull-left.headerlink,.rst-content h6 .pull-left.headerlink,.rst-content p .pull-left.headerlink,.rst-content table>caption .pull-left.headerlink,.rst-content tt.download span.pull-left:first-child,.wy-menu-vertical li.current>a button.pull-left.toctree-expand,.wy-menu-vertical li.on a button.pull-left.toctree-expand,.wy-menu-vertical li button.pull-left.toctree-expand{margin-right:.3em}.fa.pull-right,.pull-right.icon,.rst-content .code-block-caption .pull-right.headerlink,.rst-content .eqno .pull-right.headerlink,.rst-content .pull-right.admonition-title,.rst-content code.download span.pull-right:first-child,.rst-content dl dt .pull-right.headerlink,.rst-content h1 .pull-right.headerlink,.rst-content h2 .pull-right.headerlink,.rst-content h3 .pull-right.headerlink,.rst-content h4 .pull-right.headerlink,.rst-content h5 .pull-right.headerlink,.rst-content h6 .pull-right.headerlink,.rst-content p .pull-right.headerlink,.rst-content table>caption .pull-right.headerlink,.rst-content tt.download span.pull-right:first-child,.wy-menu-vertical li.current>a button.pull-right.toctree-expand,.wy-menu-vertical li.on a button.pull-right.toctree-expand,.wy-menu-vertical li button.pull-right.toctree-expand{margin-left:.3em}.fa-spin{-webkit-animation:fa-spin 2s linear infinite;animation:fa-spin 2s linear infinite}.fa-pulse{-webkit-animation:fa-spin 1s steps(8) infinite;animation:fa-spin 1s steps(8) infinite}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}.fa-rotate-90{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";-webkit-transform:rotate(90deg);-ms-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";-webkit-transform:rotate(180deg);-ms-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";-webkit-transform:rotate(270deg);-ms-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";-webkit-transform:scaleY(-1);-ms-transform:scaleY(-1);transform:scaleY(-1)}:root .fa-flip-horizontal,:root .fa-flip-vertical,:root .fa-rotate-90,:root .fa-rotate-180,:root .fa-rotate-270{filter:none}.fa-stack{position:relative;display:inline-block;width:2em;height:2em;line-height:2em;vertical-align:middle}.fa-stack-1x,.fa-stack-2x{position:absolute;left:0;width:100%;text-align:center}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:#fff}.fa-glass:before{content:""}.fa-music:before{content:""}.fa-search:before,.icon-search:before{content:""}.fa-envelope-o:before{content:""}.fa-heart:before{content:""}.fa-star:before{content:""}.fa-star-o:before{content:""}.fa-user:before{content:""}.fa-film:before{content:""}.fa-th-large:before{content:""}.fa-th:before{content:""}.fa-th-list:before{content:""}.fa-check:before{content:""}.fa-close:before,.fa-remove:before,.fa-times:before{content:""}.fa-search-plus:before{content:""}.fa-search-minus:before{content:""}.fa-power-off:before{content:""}.fa-signal:before{content:""}.fa-cog:before,.fa-gear:before{content:""}.fa-trash-o:before{content:""}.fa-home:before,.icon-home:before{content:""}.fa-file-o:before{content:""}.fa-clock-o:before{content:""}.fa-road:before{content:""}.fa-download:before,.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{content:""}.fa-arrow-circle-o-down:before{content:""}.fa-arrow-circle-o-up:before{content:""}.fa-inbox:before{content:""}.fa-play-circle-o:before{content:""}.fa-repeat:before,.fa-rotate-right:before{content:""}.fa-refresh:before{content:""}.fa-list-alt:before{content:""}.fa-lock:before{content:""}.fa-flag:before{content:""}.fa-headphones:before{content:""}.fa-volume-off:before{content:""}.fa-volume-down:before{content:""}.fa-volume-up:before{content:""}.fa-qrcode:before{content:""}.fa-barcode:before{content:""}.fa-tag:before{content:""}.fa-tags:before{content:""}.fa-book:before,.icon-book:before{content:""}.fa-bookmark:before{content:""}.fa-print:before{content:""}.fa-camera:before{content:""}.fa-font:before{content:""}.fa-bold:before{content:""}.fa-italic:before{content:""}.fa-text-height:before{content:""}.fa-text-width:before{content:""}.fa-align-left:before{content:""}.fa-align-center:before{content:""}.fa-align-right:before{content:""}.fa-align-justify:before{content:""}.fa-list:before{content:""}.fa-dedent:before,.fa-outdent:before{content:""}.fa-indent:before{content:""}.fa-video-camera:before{content:""}.fa-image:before,.fa-photo:before,.fa-picture-o:before{content:""}.fa-pencil:before{content:""}.fa-map-marker:before{content:""}.fa-adjust:before{content:""}.fa-tint:before{content:""}.fa-edit:before,.fa-pencil-square-o:before{content:""}.fa-share-square-o:before{content:""}.fa-check-square-o:before{content:""}.fa-arrows:before{content:""}.fa-step-backward:before{content:""}.fa-fast-backward:before{content:""}.fa-backward:before{content:""}.fa-play:before{content:""}.fa-pause:before{content:""}.fa-stop:before{content:""}.fa-forward:before{content:""}.fa-fast-forward:before{content:""}.fa-step-forward:before{content:""}.fa-eject:before{content:""}.fa-chevron-left:before{content:""}.fa-chevron-right:before{content:""}.fa-plus-circle:before{content:""}.fa-minus-circle:before{content:""}.fa-times-circle:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before{content:""}.fa-check-circle:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before{content:""}.fa-question-circle:before{content:""}.fa-info-circle:before{content:""}.fa-crosshairs:before{content:""}.fa-times-circle-o:before{content:""}.fa-check-circle-o:before{content:""}.fa-ban:before{content:""}.fa-arrow-left:before{content:""}.fa-arrow-right:before{content:""}.fa-arrow-up:before{content:""}.fa-arrow-down:before{content:""}.fa-mail-forward:before,.fa-share:before{content:""}.fa-expand:before{content:""}.fa-compress:before{content:""}.fa-plus:before{content:""}.fa-minus:before{content:""}.fa-asterisk:before{content:""}.fa-exclamation-circle:before,.rst-content .admonition-title:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before{content:""}.fa-gift:before{content:""}.fa-leaf:before{content:""}.fa-fire:before,.icon-fire:before{content:""}.fa-eye:before{content:""}.fa-eye-slash:before{content:""}.fa-exclamation-triangle:before,.fa-warning:before{content:""}.fa-plane:before{content:""}.fa-calendar:before{content:""}.fa-random:before{content:""}.fa-comment:before{content:""}.fa-magnet:before{content:""}.fa-chevron-up:before{content:""}.fa-chevron-down:before{content:""}.fa-retweet:before{content:""}.fa-shopping-cart:before{content:""}.fa-folder:before{content:""}.fa-folder-open:before{content:""}.fa-arrows-v:before{content:""}.fa-arrows-h:before{content:""}.fa-bar-chart-o:before,.fa-bar-chart:before{content:""}.fa-twitter-square:before{content:""}.fa-facebook-square:before{content:""}.fa-camera-retro:before{content:""}.fa-key:before{content:""}.fa-cogs:before,.fa-gears:before{content:""}.fa-comments:before{content:""}.fa-thumbs-o-up:before{content:""}.fa-thumbs-o-down:before{content:""}.fa-star-half:before{content:""}.fa-heart-o:before{content:""}.fa-sign-out:before{content:""}.fa-linkedin-square:before{content:""}.fa-thumb-tack:before{content:""}.fa-external-link:before{content:""}.fa-sign-in:before{content:""}.fa-trophy:before{content:""}.fa-github-square:before{content:""}.fa-upload:before{content:""}.fa-lemon-o:before{content:""}.fa-phone:before{content:""}.fa-square-o:before{content:""}.fa-bookmark-o:before{content:""}.fa-phone-square:before{content:""}.fa-twitter:before{content:""}.fa-facebook-f:before,.fa-facebook:before{content:""}.fa-github:before,.icon-github:before{content:""}.fa-unlock:before{content:""}.fa-credit-card:before{content:""}.fa-feed:before,.fa-rss:before{content:""}.fa-hdd-o:before{content:""}.fa-bullhorn:before{content:""}.fa-bell:before{content:""}.fa-certificate:before{content:""}.fa-hand-o-right:before{content:""}.fa-hand-o-left:before{content:""}.fa-hand-o-up:before{content:""}.fa-hand-o-down:before{content:""}.fa-arrow-circle-left:before,.icon-circle-arrow-left:before{content:""}.fa-arrow-circle-right:before,.icon-circle-arrow-right:before{content:""}.fa-arrow-circle-up:before{content:""}.fa-arrow-circle-down:before{content:""}.fa-globe:before{content:""}.fa-wrench:before{content:""}.fa-tasks:before{content:""}.fa-filter:before{content:""}.fa-briefcase:before{content:""}.fa-arrows-alt:before{content:""}.fa-group:before,.fa-users:before{content:""}.fa-chain:before,.fa-link:before,.icon-link:before{content:""}.fa-cloud:before{content:""}.fa-flask:before{content:""}.fa-cut:before,.fa-scissors:before{content:""}.fa-copy:before,.fa-files-o:before{content:""}.fa-paperclip:before{content:""}.fa-floppy-o:before,.fa-save:before{content:""}.fa-square:before{content:""}.fa-bars:before,.fa-navicon:before,.fa-reorder:before{content:""}.fa-list-ul:before{content:""}.fa-list-ol:before{content:""}.fa-strikethrough:before{content:""}.fa-underline:before{content:""}.fa-table:before{content:""}.fa-magic:before{content:""}.fa-truck:before{content:""}.fa-pinterest:before{content:""}.fa-pinterest-square:before{content:""}.fa-google-plus-square:before{content:""}.fa-google-plus:before{content:""}.fa-money:before{content:""}.fa-caret-down:before,.icon-caret-down:before,.wy-dropdown .caret:before{content:""}.fa-caret-up:before{content:""}.fa-caret-left:before{content:""}.fa-caret-right:before{content:""}.fa-columns:before{content:""}.fa-sort:before,.fa-unsorted:before{content:""}.fa-sort-desc:before,.fa-sort-down:before{content:""}.fa-sort-asc:before,.fa-sort-up:before{content:""}.fa-envelope:before{content:""}.fa-linkedin:before{content:""}.fa-rotate-left:before,.fa-undo:before{content:""}.fa-gavel:before,.fa-legal:before{content:""}.fa-dashboard:before,.fa-tachometer:before{content:""}.fa-comment-o:before{content:""}.fa-comments-o:before{content:""}.fa-bolt:before,.fa-flash:before{content:""}.fa-sitemap:before{content:""}.fa-umbrella:before{content:""}.fa-clipboard:before,.fa-paste:before{content:""}.fa-lightbulb-o:before{content:""}.fa-exchange:before{content:""}.fa-cloud-download:before{content:""}.fa-cloud-upload:before{content:""}.fa-user-md:before{content:""}.fa-stethoscope:before{content:""}.fa-suitcase:before{content:""}.fa-bell-o:before{content:""}.fa-coffee:before{content:""}.fa-cutlery:before{content:""}.fa-file-text-o:before{content:""}.fa-building-o:before{content:""}.fa-hospital-o:before{content:""}.fa-ambulance:before{content:""}.fa-medkit:before{content:""}.fa-fighter-jet:before{content:""}.fa-beer:before{content:""}.fa-h-square:before{content:""}.fa-plus-square:before{content:""}.fa-angle-double-left:before{content:""}.fa-angle-double-right:before{content:""}.fa-angle-double-up:before{content:""}.fa-angle-double-down:before{content:""}.fa-angle-left:before{content:""}.fa-angle-right:before{content:""}.fa-angle-up:before{content:""}.fa-angle-down:before{content:""}.fa-desktop:before{content:""}.fa-laptop:before{content:""}.fa-tablet:before{content:""}.fa-mobile-phone:before,.fa-mobile:before{content:""}.fa-circle-o:before{content:""}.fa-quote-left:before{content:""}.fa-quote-right:before{content:""}.fa-spinner:before{content:""}.fa-circle:before{content:""}.fa-mail-reply:before,.fa-reply:before{content:""}.fa-github-alt:before{content:""}.fa-folder-o:before{content:""}.fa-folder-open-o:before{content:""}.fa-smile-o:before{content:""}.fa-frown-o:before{content:""}.fa-meh-o:before{content:""}.fa-gamepad:before{content:""}.fa-keyboard-o:before{content:""}.fa-flag-o:before{content:""}.fa-flag-checkered:before{content:""}.fa-terminal:before{content:""}.fa-code:before{content:""}.fa-mail-reply-all:before,.fa-reply-all:before{content:""}.fa-star-half-empty:before,.fa-star-half-full:before,.fa-star-half-o:before{content:""}.fa-location-arrow:before{content:""}.fa-crop:before{content:""}.fa-code-fork:before{content:""}.fa-chain-broken:before,.fa-unlink:before{content:""}.fa-question:before{content:""}.fa-info:before{content:""}.fa-exclamation:before{content:""}.fa-superscript:before{content:""}.fa-subscript:before{content:""}.fa-eraser:before{content:""}.fa-puzzle-piece:before{content:""}.fa-microphone:before{content:""}.fa-microphone-slash:before{content:""}.fa-shield:before{content:""}.fa-calendar-o:before{content:""}.fa-fire-extinguisher:before{content:""}.fa-rocket:before{content:""}.fa-maxcdn:before{content:""}.fa-chevron-circle-left:before{content:""}.fa-chevron-circle-right:before{content:""}.fa-chevron-circle-up:before{content:""}.fa-chevron-circle-down:before{content:""}.fa-html5:before{content:""}.fa-css3:before{content:""}.fa-anchor:before{content:""}.fa-unlock-alt:before{content:""}.fa-bullseye:before{content:""}.fa-ellipsis-h:before{content:""}.fa-ellipsis-v:before{content:""}.fa-rss-square:before{content:""}.fa-play-circle:before{content:""}.fa-ticket:before{content:""}.fa-minus-square:before{content:""}.fa-minus-square-o:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before{content:""}.fa-level-up:before{content:""}.fa-level-down:before{content:""}.fa-check-square:before{content:""}.fa-pencil-square:before{content:""}.fa-external-link-square:before{content:""}.fa-share-square:before{content:""}.fa-compass:before{content:""}.fa-caret-square-o-down:before,.fa-toggle-down:before{content:""}.fa-caret-square-o-up:before,.fa-toggle-up:before{content:""}.fa-caret-square-o-right:before,.fa-toggle-right:before{content:""}.fa-eur:before,.fa-euro:before{content:""}.fa-gbp:before{content:""}.fa-dollar:before,.fa-usd:before{content:""}.fa-inr:before,.fa-rupee:before{content:""}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen:before{content:""}.fa-rouble:before,.fa-rub:before,.fa-ruble:before{content:""}.fa-krw:before,.fa-won:before{content:""}.fa-bitcoin:before,.fa-btc:before{content:""}.fa-file:before{content:""}.fa-file-text:before{content:""}.fa-sort-alpha-asc:before{content:""}.fa-sort-alpha-desc:before{content:""}.fa-sort-amount-asc:before{content:""}.fa-sort-amount-desc:before{content:""}.fa-sort-numeric-asc:before{content:""}.fa-sort-numeric-desc:before{content:""}.fa-thumbs-up:before{content:""}.fa-thumbs-down:before{content:""}.fa-youtube-square:before{content:""}.fa-youtube:before{content:""}.fa-xing:before{content:""}.fa-xing-square:before{content:""}.fa-youtube-play:before{content:""}.fa-dropbox:before{content:""}.fa-stack-overflow:before{content:""}.fa-instagram:before{content:""}.fa-flickr:before{content:""}.fa-adn:before{content:""}.fa-bitbucket:before,.icon-bitbucket:before{content:""}.fa-bitbucket-square:before{content:""}.fa-tumblr:before{content:""}.fa-tumblr-square:before{content:""}.fa-long-arrow-down:before{content:""}.fa-long-arrow-up:before{content:""}.fa-long-arrow-left:before{content:""}.fa-long-arrow-right:before{content:""}.fa-apple:before{content:""}.fa-windows:before{content:""}.fa-android:before{content:""}.fa-linux:before{content:""}.fa-dribbble:before{content:""}.fa-skype:before{content:""}.fa-foursquare:before{content:""}.fa-trello:before{content:""}.fa-female:before{content:""}.fa-male:before{content:""}.fa-gittip:before,.fa-gratipay:before{content:""}.fa-sun-o:before{content:""}.fa-moon-o:before{content:""}.fa-archive:before{content:""}.fa-bug:before{content:""}.fa-vk:before{content:""}.fa-weibo:before{content:""}.fa-renren:before{content:""}.fa-pagelines:before{content:""}.fa-stack-exchange:before{content:""}.fa-arrow-circle-o-right:before{content:""}.fa-arrow-circle-o-left:before{content:""}.fa-caret-square-o-left:before,.fa-toggle-left:before{content:""}.fa-dot-circle-o:before{content:""}.fa-wheelchair:before{content:""}.fa-vimeo-square:before{content:""}.fa-try:before,.fa-turkish-lira:before{content:""}.fa-plus-square-o:before,.wy-menu-vertical li button.toctree-expand:before{content:""}.fa-space-shuttle:before{content:""}.fa-slack:before{content:""}.fa-envelope-square:before{content:""}.fa-wordpress:before{content:""}.fa-openid:before{content:""}.fa-bank:before,.fa-institution:before,.fa-university:before{content:""}.fa-graduation-cap:before,.fa-mortar-board:before{content:""}.fa-yahoo:before{content:""}.fa-google:before{content:""}.fa-reddit:before{content:""}.fa-reddit-square:before{content:""}.fa-stumbleupon-circle:before{content:""}.fa-stumbleupon:before{content:""}.fa-delicious:before{content:""}.fa-digg:before{content:""}.fa-pied-piper-pp:before{content:""}.fa-pied-piper-alt:before{content:""}.fa-drupal:before{content:""}.fa-joomla:before{content:""}.fa-language:before{content:""}.fa-fax:before{content:""}.fa-building:before{content:""}.fa-child:before{content:""}.fa-paw:before{content:""}.fa-spoon:before{content:""}.fa-cube:before{content:""}.fa-cubes:before{content:""}.fa-behance:before{content:""}.fa-behance-square:before{content:""}.fa-steam:before{content:""}.fa-steam-square:before{content:""}.fa-recycle:before{content:""}.fa-automobile:before,.fa-car:before{content:""}.fa-cab:before,.fa-taxi:before{content:""}.fa-tree:before{content:""}.fa-spotify:before{content:""}.fa-deviantart:before{content:""}.fa-soundcloud:before{content:""}.fa-database:before{content:""}.fa-file-pdf-o:before{content:""}.fa-file-word-o:before{content:""}.fa-file-excel-o:before{content:""}.fa-file-powerpoint-o:before{content:""}.fa-file-image-o:before,.fa-file-photo-o:before,.fa-file-picture-o:before{content:""}.fa-file-archive-o:before,.fa-file-zip-o:before{content:""}.fa-file-audio-o:before,.fa-file-sound-o:before{content:""}.fa-file-movie-o:before,.fa-file-video-o:before{content:""}.fa-file-code-o:before{content:""}.fa-vine:before{content:""}.fa-codepen:before{content:""}.fa-jsfiddle:before{content:""}.fa-life-bouy:before,.fa-life-buoy:before,.fa-life-ring:before,.fa-life-saver:before,.fa-support:before{content:""}.fa-circle-o-notch:before{content:""}.fa-ra:before,.fa-rebel:before,.fa-resistance:before{content:""}.fa-empire:before,.fa-ge:before{content:""}.fa-git-square:before{content:""}.fa-git:before{content:""}.fa-hacker-news:before,.fa-y-combinator-square:before,.fa-yc-square:before{content:""}.fa-tencent-weibo:before{content:""}.fa-qq:before{content:""}.fa-wechat:before,.fa-weixin:before{content:""}.fa-paper-plane:before,.fa-send:before{content:""}.fa-paper-plane-o:before,.fa-send-o:before{content:""}.fa-history:before{content:""}.fa-circle-thin:before{content:""}.fa-header:before{content:""}.fa-paragraph:before{content:""}.fa-sliders:before{content:""}.fa-share-alt:before{content:""}.fa-share-alt-square:before{content:""}.fa-bomb:before{content:""}.fa-futbol-o:before,.fa-soccer-ball-o:before{content:""}.fa-tty:before{content:""}.fa-binoculars:before{content:""}.fa-plug:before{content:""}.fa-slideshare:before{content:""}.fa-twitch:before{content:""}.fa-yelp:before{content:""}.fa-newspaper-o:before{content:""}.fa-wifi:before{content:""}.fa-calculator:before{content:""}.fa-paypal:before{content:""}.fa-google-wallet:before{content:""}.fa-cc-visa:before{content:""}.fa-cc-mastercard:before{content:""}.fa-cc-discover:before{content:""}.fa-cc-amex:before{content:""}.fa-cc-paypal:before{content:""}.fa-cc-stripe:before{content:""}.fa-bell-slash:before{content:""}.fa-bell-slash-o:before{content:""}.fa-trash:before{content:""}.fa-copyright:before{content:""}.fa-at:before{content:""}.fa-eyedropper:before{content:""}.fa-paint-brush:before{content:""}.fa-birthday-cake:before{content:""}.fa-area-chart:before{content:""}.fa-pie-chart:before{content:""}.fa-line-chart:before{content:""}.fa-lastfm:before{content:""}.fa-lastfm-square:before{content:""}.fa-toggle-off:before{content:""}.fa-toggle-on:before{content:""}.fa-bicycle:before{content:""}.fa-bus:before{content:""}.fa-ioxhost:before{content:""}.fa-angellist:before{content:""}.fa-cc:before{content:""}.fa-ils:before,.fa-shekel:before,.fa-sheqel:before{content:""}.fa-meanpath:before{content:""}.fa-buysellads:before{content:""}.fa-connectdevelop:before{content:""}.fa-dashcube:before{content:""}.fa-forumbee:before{content:""}.fa-leanpub:before{content:""}.fa-sellsy:before{content:""}.fa-shirtsinbulk:before{content:""}.fa-simplybuilt:before{content:""}.fa-skyatlas:before{content:""}.fa-cart-plus:before{content:""}.fa-cart-arrow-down:before{content:""}.fa-diamond:before{content:""}.fa-ship:before{content:""}.fa-user-secret:before{content:""}.fa-motorcycle:before{content:""}.fa-street-view:before{content:""}.fa-heartbeat:before{content:""}.fa-venus:before{content:""}.fa-mars:before{content:""}.fa-mercury:before{content:""}.fa-intersex:before,.fa-transgender:before{content:""}.fa-transgender-alt:before{content:""}.fa-venus-double:before{content:""}.fa-mars-double:before{content:""}.fa-venus-mars:before{content:""}.fa-mars-stroke:before{content:""}.fa-mars-stroke-v:before{content:""}.fa-mars-stroke-h:before{content:""}.fa-neuter:before{content:""}.fa-genderless:before{content:""}.fa-facebook-official:before{content:""}.fa-pinterest-p:before{content:""}.fa-whatsapp:before{content:""}.fa-server:before{content:""}.fa-user-plus:before{content:""}.fa-user-times:before{content:""}.fa-bed:before,.fa-hotel:before{content:""}.fa-viacoin:before{content:""}.fa-train:before{content:""}.fa-subway:before{content:""}.fa-medium:before{content:""}.fa-y-combinator:before,.fa-yc:before{content:""}.fa-optin-monster:before{content:""}.fa-opencart:before{content:""}.fa-expeditedssl:before{content:""}.fa-battery-4:before,.fa-battery-full:before,.fa-battery:before{content:""}.fa-battery-3:before,.fa-battery-three-quarters:before{content:""}.fa-battery-2:before,.fa-battery-half:before{content:""}.fa-battery-1:before,.fa-battery-quarter:before{content:""}.fa-battery-0:before,.fa-battery-empty:before{content:""}.fa-mouse-pointer:before{content:""}.fa-i-cursor:before{content:""}.fa-object-group:before{content:""}.fa-object-ungroup:before{content:""}.fa-sticky-note:before{content:""}.fa-sticky-note-o:before{content:""}.fa-cc-jcb:before{content:""}.fa-cc-diners-club:before{content:""}.fa-clone:before{content:""}.fa-balance-scale:before{content:""}.fa-hourglass-o:before{content:""}.fa-hourglass-1:before,.fa-hourglass-start:before{content:""}.fa-hourglass-2:before,.fa-hourglass-half:before{content:""}.fa-hourglass-3:before,.fa-hourglass-end:before{content:""}.fa-hourglass:before{content:""}.fa-hand-grab-o:before,.fa-hand-rock-o:before{content:""}.fa-hand-paper-o:before,.fa-hand-stop-o:before{content:""}.fa-hand-scissors-o:before{content:""}.fa-hand-lizard-o:before{content:""}.fa-hand-spock-o:before{content:""}.fa-hand-pointer-o:before{content:""}.fa-hand-peace-o:before{content:""}.fa-trademark:before{content:""}.fa-registered:before{content:""}.fa-creative-commons:before{content:""}.fa-gg:before{content:""}.fa-gg-circle:before{content:""}.fa-tripadvisor:before{content:""}.fa-odnoklassniki:before{content:""}.fa-odnoklassniki-square:before{content:""}.fa-get-pocket:before{content:""}.fa-wikipedia-w:before{content:""}.fa-safari:before{content:""}.fa-chrome:before{content:""}.fa-firefox:before{content:""}.fa-opera:before{content:""}.fa-internet-explorer:before{content:""}.fa-television:before,.fa-tv:before{content:""}.fa-contao:before{content:""}.fa-500px:before{content:""}.fa-amazon:before{content:""}.fa-calendar-plus-o:before{content:""}.fa-calendar-minus-o:before{content:""}.fa-calendar-times-o:before{content:""}.fa-calendar-check-o:before{content:""}.fa-industry:before{content:""}.fa-map-pin:before{content:""}.fa-map-signs:before{content:""}.fa-map-o:before{content:""}.fa-map:before{content:""}.fa-commenting:before{content:""}.fa-commenting-o:before{content:""}.fa-houzz:before{content:""}.fa-vimeo:before{content:""}.fa-black-tie:before{content:""}.fa-fonticons:before{content:""}.fa-reddit-alien:before{content:""}.fa-edge:before{content:""}.fa-credit-card-alt:before{content:""}.fa-codiepie:before{content:""}.fa-modx:before{content:""}.fa-fort-awesome:before{content:""}.fa-usb:before{content:""}.fa-product-hunt:before{content:""}.fa-mixcloud:before{content:""}.fa-scribd:before{content:""}.fa-pause-circle:before{content:""}.fa-pause-circle-o:before{content:""}.fa-stop-circle:before{content:""}.fa-stop-circle-o:before{content:""}.fa-shopping-bag:before{content:""}.fa-shopping-basket:before{content:""}.fa-hashtag:before{content:""}.fa-bluetooth:before{content:""}.fa-bluetooth-b:before{content:""}.fa-percent:before{content:""}.fa-gitlab:before,.icon-gitlab:before{content:""}.fa-wpbeginner:before{content:""}.fa-wpforms:before{content:""}.fa-envira:before{content:""}.fa-universal-access:before{content:""}.fa-wheelchair-alt:before{content:""}.fa-question-circle-o:before{content:""}.fa-blind:before{content:""}.fa-audio-description:before{content:""}.fa-volume-control-phone:before{content:""}.fa-braille:before{content:""}.fa-assistive-listening-systems:before{content:""}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before{content:""}.fa-deaf:before,.fa-deafness:before,.fa-hard-of-hearing:before{content:""}.fa-glide:before{content:""}.fa-glide-g:before{content:""}.fa-sign-language:before,.fa-signing:before{content:""}.fa-low-vision:before{content:""}.fa-viadeo:before{content:""}.fa-viadeo-square:before{content:""}.fa-snapchat:before{content:""}.fa-snapchat-ghost:before{content:""}.fa-snapchat-square:before{content:""}.fa-pied-piper:before{content:""}.fa-first-order:before{content:""}.fa-yoast:before{content:""}.fa-themeisle:before{content:""}.fa-google-plus-circle:before,.fa-google-plus-official:before{content:""}.fa-fa:before,.fa-font-awesome:before{content:""}.fa-handshake-o:before{content:""}.fa-envelope-open:before{content:""}.fa-envelope-open-o:before{content:""}.fa-linode:before{content:""}.fa-address-book:before{content:""}.fa-address-book-o:before{content:""}.fa-address-card:before,.fa-vcard:before{content:""}.fa-address-card-o:before,.fa-vcard-o:before{content:""}.fa-user-circle:before{content:""}.fa-user-circle-o:before{content:""}.fa-user-o:before{content:""}.fa-id-badge:before{content:""}.fa-drivers-license:before,.fa-id-card:before{content:""}.fa-drivers-license-o:before,.fa-id-card-o:before{content:""}.fa-quora:before{content:""}.fa-free-code-camp:before{content:""}.fa-telegram:before{content:""}.fa-thermometer-4:before,.fa-thermometer-full:before,.fa-thermometer:before{content:""}.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:""}.fa-thermometer-2:before,.fa-thermometer-half:before{content:""}.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:""}.fa-thermometer-0:before,.fa-thermometer-empty:before{content:""}.fa-shower:before{content:""}.fa-bath:before,.fa-bathtub:before,.fa-s15:before{content:""}.fa-podcast:before{content:""}.fa-window-maximize:before{content:""}.fa-window-minimize:before{content:""}.fa-window-restore:before{content:""}.fa-times-rectangle:before,.fa-window-close:before{content:""}.fa-times-rectangle-o:before,.fa-window-close-o:before{content:""}.fa-bandcamp:before{content:""}.fa-grav:before{content:""}.fa-etsy:before{content:""}.fa-imdb:before{content:""}.fa-ravelry:before{content:""}.fa-eercast:before{content:""}.fa-microchip:before{content:""}.fa-snowflake-o:before{content:""}.fa-superpowers:before{content:""}.fa-wpexplorer:before{content:""}.fa-meetup:before{content:""}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-dropdown .caret,.wy-inline-validate.wy-inline-validate-danger .wy-input-context,.wy-inline-validate.wy-inline-validate-info .wy-input-context,.wy-inline-validate.wy-inline-validate-success .wy-input-context,.wy-inline-validate.wy-inline-validate-warning .wy-input-context,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{font-family:inherit}.fa:before,.icon:before,.rst-content .admonition-title:before,.rst-content .code-block-caption .headerlink:before,.rst-content .eqno .headerlink:before,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before{font-family:FontAwesome;display:inline-block;font-style:normal;font-weight:400;line-height:1;text-decoration:inherit}.rst-content .code-block-caption a .headerlink,.rst-content .eqno a .headerlink,.rst-content a .admonition-title,.rst-content code.download a span:first-child,.rst-content dl dt a .headerlink,.rst-content h1 a .headerlink,.rst-content h2 a .headerlink,.rst-content h3 a .headerlink,.rst-content h4 a .headerlink,.rst-content h5 a .headerlink,.rst-content h6 a .headerlink,.rst-content p.caption a .headerlink,.rst-content p a .headerlink,.rst-content table>caption a .headerlink,.rst-content tt.download a span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li a button.toctree-expand,a .fa,a .icon,a .rst-content .admonition-title,a .rst-content .code-block-caption .headerlink,a .rst-content .eqno .headerlink,a .rst-content code.download span:first-child,a .rst-content dl dt .headerlink,a .rst-content h1 .headerlink,a .rst-content h2 .headerlink,a .rst-content h3 .headerlink,a .rst-content h4 .headerlink,a .rst-content h5 .headerlink,a .rst-content h6 .headerlink,a .rst-content p.caption .headerlink,a .rst-content p .headerlink,a .rst-content table>caption .headerlink,a .rst-content tt.download span:first-child,a .wy-menu-vertical li button.toctree-expand{display:inline-block;text-decoration:inherit}.btn .fa,.btn .icon,.btn .rst-content .admonition-title,.btn .rst-content .code-block-caption .headerlink,.btn .rst-content .eqno .headerlink,.btn .rst-content code.download span:first-child,.btn .rst-content dl dt .headerlink,.btn .rst-content h1 .headerlink,.btn .rst-content h2 .headerlink,.btn .rst-content h3 .headerlink,.btn .rst-content h4 .headerlink,.btn .rst-content h5 .headerlink,.btn .rst-content h6 .headerlink,.btn .rst-content p .headerlink,.btn .rst-content table>caption .headerlink,.btn .rst-content tt.download span:first-child,.btn .wy-menu-vertical li.current>a button.toctree-expand,.btn .wy-menu-vertical li.on a button.toctree-expand,.btn .wy-menu-vertical li button.toctree-expand,.nav .fa,.nav .icon,.nav .rst-content .admonition-title,.nav .rst-content .code-block-caption .headerlink,.nav .rst-content .eqno .headerlink,.nav .rst-content code.download span:first-child,.nav .rst-content dl dt .headerlink,.nav .rst-content h1 .headerlink,.nav .rst-content h2 .headerlink,.nav .rst-content h3 .headerlink,.nav .rst-content h4 .headerlink,.nav .rst-content h5 .headerlink,.nav .rst-content h6 .headerlink,.nav .rst-content p .headerlink,.nav .rst-content table>caption .headerlink,.nav .rst-content tt.download span:first-child,.nav .wy-menu-vertical li.current>a button.toctree-expand,.nav .wy-menu-vertical li.on a button.toctree-expand,.nav .wy-menu-vertical li button.toctree-expand,.rst-content .btn .admonition-title,.rst-content .code-block-caption .btn .headerlink,.rst-content .code-block-caption .nav .headerlink,.rst-content .eqno .btn .headerlink,.rst-content .eqno .nav .headerlink,.rst-content .nav .admonition-title,.rst-content code.download .btn span:first-child,.rst-content code.download .nav span:first-child,.rst-content dl dt .btn .headerlink,.rst-content dl dt .nav .headerlink,.rst-content h1 .btn .headerlink,.rst-content h1 .nav .headerlink,.rst-content h2 .btn .headerlink,.rst-content h2 .nav .headerlink,.rst-content h3 .btn .headerlink,.rst-content h3 .nav .headerlink,.rst-content h4 .btn .headerlink,.rst-content h4 .nav .headerlink,.rst-content h5 .btn .headerlink,.rst-content h5 .nav .headerlink,.rst-content h6 .btn .headerlink,.rst-content h6 .nav .headerlink,.rst-content p .btn .headerlink,.rst-content p .nav .headerlink,.rst-content table>caption .btn .headerlink,.rst-content table>caption .nav .headerlink,.rst-content tt.download .btn span:first-child,.rst-content tt.download .nav span:first-child,.wy-menu-vertical li .btn button.toctree-expand,.wy-menu-vertical li.current>a .btn button.toctree-expand,.wy-menu-vertical li.current>a .nav button.toctree-expand,.wy-menu-vertical li .nav button.toctree-expand,.wy-menu-vertical li.on a .btn button.toctree-expand,.wy-menu-vertical li.on a .nav button.toctree-expand{display:inline}.btn .fa-large.icon,.btn .fa.fa-large,.btn .rst-content .code-block-caption .fa-large.headerlink,.btn .rst-content .eqno .fa-large.headerlink,.btn .rst-content .fa-large.admonition-title,.btn .rst-content code.download span.fa-large:first-child,.btn .rst-content dl dt .fa-large.headerlink,.btn .rst-content h1 .fa-large.headerlink,.btn .rst-content h2 .fa-large.headerlink,.btn .rst-content h3 .fa-large.headerlink,.btn .rst-content h4 .fa-large.headerlink,.btn .rst-content h5 .fa-large.headerlink,.btn .rst-content h6 .fa-large.headerlink,.btn .rst-content p .fa-large.headerlink,.btn .rst-content table>caption .fa-large.headerlink,.btn .rst-content tt.download span.fa-large:first-child,.btn .wy-menu-vertical li button.fa-large.toctree-expand,.nav .fa-large.icon,.nav .fa.fa-large,.nav .rst-content .code-block-caption .fa-large.headerlink,.nav .rst-content .eqno .fa-large.headerlink,.nav .rst-content .fa-large.admonition-title,.nav .rst-content code.download span.fa-large:first-child,.nav .rst-content dl dt .fa-large.headerlink,.nav .rst-content h1 .fa-large.headerlink,.nav .rst-content h2 .fa-large.headerlink,.nav .rst-content h3 .fa-large.headerlink,.nav .rst-content h4 .fa-large.headerlink,.nav .rst-content h5 .fa-large.headerlink,.nav .rst-content h6 .fa-large.headerlink,.nav .rst-content p .fa-large.headerlink,.nav .rst-content table>caption .fa-large.headerlink,.nav .rst-content tt.download span.fa-large:first-child,.nav .wy-menu-vertical li button.fa-large.toctree-expand,.rst-content .btn .fa-large.admonition-title,.rst-content .code-block-caption .btn .fa-large.headerlink,.rst-content .code-block-caption .nav .fa-large.headerlink,.rst-content .eqno .btn .fa-large.headerlink,.rst-content .eqno .nav .fa-large.headerlink,.rst-content .nav .fa-large.admonition-title,.rst-content code.download .btn span.fa-large:first-child,.rst-content code.download .nav span.fa-large:first-child,.rst-content dl dt .btn .fa-large.headerlink,.rst-content dl dt .nav .fa-large.headerlink,.rst-content h1 .btn .fa-large.headerlink,.rst-content h1 .nav .fa-large.headerlink,.rst-content h2 .btn .fa-large.headerlink,.rst-content h2 .nav .fa-large.headerlink,.rst-content h3 .btn .fa-large.headerlink,.rst-content h3 .nav .fa-large.headerlink,.rst-content h4 .btn .fa-large.headerlink,.rst-content h4 .nav .fa-large.headerlink,.rst-content h5 .btn .fa-large.headerlink,.rst-content h5 .nav .fa-large.headerlink,.rst-content h6 .btn .fa-large.headerlink,.rst-content h6 .nav .fa-large.headerlink,.rst-content p .btn .fa-large.headerlink,.rst-content p .nav .fa-large.headerlink,.rst-content table>caption .btn .fa-large.headerlink,.rst-content table>caption .nav .fa-large.headerlink,.rst-content tt.download .btn span.fa-large:first-child,.rst-content tt.download .nav span.fa-large:first-child,.wy-menu-vertical li .btn button.fa-large.toctree-expand,.wy-menu-vertical li .nav button.fa-large.toctree-expand{line-height:.9em}.btn .fa-spin.icon,.btn .fa.fa-spin,.btn .rst-content .code-block-caption .fa-spin.headerlink,.btn .rst-content .eqno .fa-spin.headerlink,.btn .rst-content .fa-spin.admonition-title,.btn .rst-content code.download span.fa-spin:first-child,.btn .rst-content dl dt .fa-spin.headerlink,.btn .rst-content h1 .fa-spin.headerlink,.btn .rst-content h2 .fa-spin.headerlink,.btn .rst-content h3 .fa-spin.headerlink,.btn .rst-content h4 .fa-spin.headerlink,.btn .rst-content h5 .fa-spin.headerlink,.btn .rst-content h6 .fa-spin.headerlink,.btn .rst-content p .fa-spin.headerlink,.btn .rst-content table>caption .fa-spin.headerlink,.btn .rst-content tt.download span.fa-spin:first-child,.btn .wy-menu-vertical li button.fa-spin.toctree-expand,.nav .fa-spin.icon,.nav .fa.fa-spin,.nav .rst-content .code-block-caption .fa-spin.headerlink,.nav .rst-content .eqno .fa-spin.headerlink,.nav .rst-content .fa-spin.admonition-title,.nav .rst-content code.download span.fa-spin:first-child,.nav .rst-content dl dt .fa-spin.headerlink,.nav .rst-content h1 .fa-spin.headerlink,.nav .rst-content h2 .fa-spin.headerlink,.nav .rst-content h3 .fa-spin.headerlink,.nav .rst-content h4 .fa-spin.headerlink,.nav .rst-content h5 .fa-spin.headerlink,.nav .rst-content h6 .fa-spin.headerlink,.nav .rst-content p .fa-spin.headerlink,.nav .rst-content table>caption .fa-spin.headerlink,.nav .rst-content tt.download span.fa-spin:first-child,.nav .wy-menu-vertical li button.fa-spin.toctree-expand,.rst-content .btn .fa-spin.admonition-title,.rst-content .code-block-caption .btn .fa-spin.headerlink,.rst-content .code-block-caption .nav .fa-spin.headerlink,.rst-content .eqno .btn .fa-spin.headerlink,.rst-content .eqno .nav .fa-spin.headerlink,.rst-content .nav .fa-spin.admonition-title,.rst-content code.download .btn span.fa-spin:first-child,.rst-content code.download .nav span.fa-spin:first-child,.rst-content dl dt .btn .fa-spin.headerlink,.rst-content dl dt .nav .fa-spin.headerlink,.rst-content h1 .btn .fa-spin.headerlink,.rst-content h1 .nav .fa-spin.headerlink,.rst-content h2 .btn .fa-spin.headerlink,.rst-content h2 .nav .fa-spin.headerlink,.rst-content h3 .btn .fa-spin.headerlink,.rst-content h3 .nav .fa-spin.headerlink,.rst-content h4 .btn .fa-spin.headerlink,.rst-content h4 .nav .fa-spin.headerlink,.rst-content h5 .btn .fa-spin.headerlink,.rst-content h5 .nav .fa-spin.headerlink,.rst-content h6 .btn .fa-spin.headerlink,.rst-content h6 .nav .fa-spin.headerlink,.rst-content p .btn .fa-spin.headerlink,.rst-content p .nav .fa-spin.headerlink,.rst-content table>caption .btn .fa-spin.headerlink,.rst-content table>caption .nav .fa-spin.headerlink,.rst-content tt.download .btn span.fa-spin:first-child,.rst-content tt.download .nav span.fa-spin:first-child,.wy-menu-vertical li .btn button.fa-spin.toctree-expand,.wy-menu-vertical li .nav button.fa-spin.toctree-expand{display:inline-block}.btn.fa:before,.btn.icon:before,.rst-content .btn.admonition-title:before,.rst-content .code-block-caption .btn.headerlink:before,.rst-content .eqno .btn.headerlink:before,.rst-content code.download span.btn:first-child:before,.rst-content dl dt .btn.headerlink:before,.rst-content h1 .btn.headerlink:before,.rst-content h2 .btn.headerlink:before,.rst-content h3 .btn.headerlink:before,.rst-content h4 .btn.headerlink:before,.rst-content h5 .btn.headerlink:before,.rst-content h6 .btn.headerlink:before,.rst-content p .btn.headerlink:before,.rst-content table>caption .btn.headerlink:before,.rst-content tt.download span.btn:first-child:before,.wy-menu-vertical li button.btn.toctree-expand:before{opacity:.5;-webkit-transition:opacity .05s ease-in;-moz-transition:opacity .05s ease-in;transition:opacity .05s ease-in}.btn.fa:hover:before,.btn.icon:hover:before,.rst-content .btn.admonition-title:hover:before,.rst-content .code-block-caption .btn.headerlink:hover:before,.rst-content .eqno .btn.headerlink:hover:before,.rst-content code.download span.btn:first-child:hover:before,.rst-content dl dt .btn.headerlink:hover:before,.rst-content h1 .btn.headerlink:hover:before,.rst-content h2 .btn.headerlink:hover:before,.rst-content h3 .btn.headerlink:hover:before,.rst-content h4 .btn.headerlink:hover:before,.rst-content h5 .btn.headerlink:hover:before,.rst-content h6 .btn.headerlink:hover:before,.rst-content p .btn.headerlink:hover:before,.rst-content table>caption .btn.headerlink:hover:before,.rst-content tt.download span.btn:first-child:hover:before,.wy-menu-vertical li button.btn.toctree-expand:hover:before{opacity:1}.btn-mini .fa:before,.btn-mini .icon:before,.btn-mini .rst-content .admonition-title:before,.btn-mini .rst-content .code-block-caption .headerlink:before,.btn-mini .rst-content .eqno .headerlink:before,.btn-mini .rst-content code.download span:first-child:before,.btn-mini .rst-content dl dt .headerlink:before,.btn-mini .rst-content h1 .headerlink:before,.btn-mini .rst-content h2 .headerlink:before,.btn-mini .rst-content h3 .headerlink:before,.btn-mini .rst-content h4 .headerlink:before,.btn-mini .rst-content h5 .headerlink:before,.btn-mini .rst-content h6 .headerlink:before,.btn-mini .rst-content p .headerlink:before,.btn-mini .rst-content table>caption .headerlink:before,.btn-mini .rst-content tt.download span:first-child:before,.btn-mini .wy-menu-vertical li button.toctree-expand:before,.rst-content .btn-mini .admonition-title:before,.rst-content .code-block-caption .btn-mini .headerlink:before,.rst-content .eqno .btn-mini .headerlink:before,.rst-content code.download .btn-mini span:first-child:before,.rst-content dl dt .btn-mini .headerlink:before,.rst-content h1 .btn-mini .headerlink:before,.rst-content h2 .btn-mini .headerlink:before,.rst-content h3 .btn-mini .headerlink:before,.rst-content h4 .btn-mini .headerlink:before,.rst-content h5 .btn-mini .headerlink:before,.rst-content h6 .btn-mini .headerlink:before,.rst-content p .btn-mini .headerlink:before,.rst-content table>caption .btn-mini .headerlink:before,.rst-content tt.download .btn-mini span:first-child:before,.wy-menu-vertical li .btn-mini button.toctree-expand:before{font-size:14px;vertical-align:-15%}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.wy-alert{padding:12px;line-height:24px;margin-bottom:24px;background:#e7f2fa}.rst-content .admonition-title,.wy-alert-title{font-weight:700;display:block;color:#fff;background:#6ab0de;padding:6px 12px;margin:-12px -12px 12px}.rst-content .danger,.rst-content .error,.rst-content .wy-alert-danger.admonition,.rst-content .wy-alert-danger.admonition-todo,.rst-content .wy-alert-danger.attention,.rst-content .wy-alert-danger.caution,.rst-content .wy-alert-danger.hint,.rst-content .wy-alert-danger.important,.rst-content .wy-alert-danger.note,.rst-content .wy-alert-danger.seealso,.rst-content .wy-alert-danger.tip,.rst-content .wy-alert-danger.warning,.wy-alert.wy-alert-danger{background:#fdf3f2}.rst-content .danger .admonition-title,.rst-content .danger .wy-alert-title,.rst-content .error .admonition-title,.rst-content .error .wy-alert-title,.rst-content .wy-alert-danger.admonition-todo .admonition-title,.rst-content .wy-alert-danger.admonition-todo .wy-alert-title,.rst-content .wy-alert-danger.admonition .admonition-title,.rst-content .wy-alert-danger.admonition .wy-alert-title,.rst-content .wy-alert-danger.attention .admonition-title,.rst-content .wy-alert-danger.attention .wy-alert-title,.rst-content .wy-alert-danger.caution .admonition-title,.rst-content .wy-alert-danger.caution .wy-alert-title,.rst-content .wy-alert-danger.hint .admonition-title,.rst-content .wy-alert-danger.hint .wy-alert-title,.rst-content .wy-alert-danger.important .admonition-title,.rst-content .wy-alert-danger.important .wy-alert-title,.rst-content .wy-alert-danger.note .admonition-title,.rst-content .wy-alert-danger.note .wy-alert-title,.rst-content .wy-alert-danger.seealso .admonition-title,.rst-content .wy-alert-danger.seealso .wy-alert-title,.rst-content .wy-alert-danger.tip .admonition-title,.rst-content .wy-alert-danger.tip .wy-alert-title,.rst-content .wy-alert-danger.warning .admonition-title,.rst-content .wy-alert-danger.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-danger .admonition-title,.wy-alert.wy-alert-danger .rst-content .admonition-title,.wy-alert.wy-alert-danger .wy-alert-title{background:#f29f97}.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .warning,.rst-content .wy-alert-warning.admonition,.rst-content .wy-alert-warning.danger,.rst-content .wy-alert-warning.error,.rst-content .wy-alert-warning.hint,.rst-content .wy-alert-warning.important,.rst-content .wy-alert-warning.note,.rst-content .wy-alert-warning.seealso,.rst-content .wy-alert-warning.tip,.wy-alert.wy-alert-warning{background:#ffedcc}.rst-content .admonition-todo .admonition-title,.rst-content .admonition-todo .wy-alert-title,.rst-content .attention .admonition-title,.rst-content .attention .wy-alert-title,.rst-content .caution .admonition-title,.rst-content .caution .wy-alert-title,.rst-content .warning .admonition-title,.rst-content .warning .wy-alert-title,.rst-content .wy-alert-warning.admonition .admonition-title,.rst-content .wy-alert-warning.admonition .wy-alert-title,.rst-content .wy-alert-warning.danger .admonition-title,.rst-content .wy-alert-warning.danger .wy-alert-title,.rst-content .wy-alert-warning.error .admonition-title,.rst-content .wy-alert-warning.error .wy-alert-title,.rst-content .wy-alert-warning.hint .admonition-title,.rst-content .wy-alert-warning.hint .wy-alert-title,.rst-content .wy-alert-warning.important .admonition-title,.rst-content .wy-alert-warning.important .wy-alert-title,.rst-content .wy-alert-warning.note .admonition-title,.rst-content .wy-alert-warning.note .wy-alert-title,.rst-content .wy-alert-warning.seealso .admonition-title,.rst-content .wy-alert-warning.seealso .wy-alert-title,.rst-content .wy-alert-warning.tip .admonition-title,.rst-content .wy-alert-warning.tip .wy-alert-title,.rst-content .wy-alert.wy-alert-warning .admonition-title,.wy-alert.wy-alert-warning .rst-content .admonition-title,.wy-alert.wy-alert-warning .wy-alert-title{background:#f0b37e}.rst-content .note,.rst-content .seealso,.rst-content .wy-alert-info.admonition,.rst-content .wy-alert-info.admonition-todo,.rst-content .wy-alert-info.attention,.rst-content .wy-alert-info.caution,.rst-content .wy-alert-info.danger,.rst-content .wy-alert-info.error,.rst-content .wy-alert-info.hint,.rst-content .wy-alert-info.important,.rst-content .wy-alert-info.tip,.rst-content .wy-alert-info.warning,.wy-alert.wy-alert-info{background:#e7f2fa}.rst-content .note .admonition-title,.rst-content .note .wy-alert-title,.rst-content .seealso .admonition-title,.rst-content .seealso .wy-alert-title,.rst-content .wy-alert-info.admonition-todo .admonition-title,.rst-content .wy-alert-info.admonition-todo .wy-alert-title,.rst-content .wy-alert-info.admonition .admonition-title,.rst-content .wy-alert-info.admonition .wy-alert-title,.rst-content .wy-alert-info.attention .admonition-title,.rst-content .wy-alert-info.attention .wy-alert-title,.rst-content .wy-alert-info.caution .admonition-title,.rst-content .wy-alert-info.caution .wy-alert-title,.rst-content .wy-alert-info.danger .admonition-title,.rst-content .wy-alert-info.danger .wy-alert-title,.rst-content .wy-alert-info.error .admonition-title,.rst-content .wy-alert-info.error .wy-alert-title,.rst-content .wy-alert-info.hint .admonition-title,.rst-content .wy-alert-info.hint .wy-alert-title,.rst-content .wy-alert-info.important .admonition-title,.rst-content .wy-alert-info.important .wy-alert-title,.rst-content .wy-alert-info.tip .admonition-title,.rst-content .wy-alert-info.tip .wy-alert-title,.rst-content .wy-alert-info.warning .admonition-title,.rst-content .wy-alert-info.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-info .admonition-title,.wy-alert.wy-alert-info .rst-content .admonition-title,.wy-alert.wy-alert-info .wy-alert-title{background:#6ab0de}.rst-content .hint,.rst-content .important,.rst-content .tip,.rst-content .wy-alert-success.admonition,.rst-content .wy-alert-success.admonition-todo,.rst-content .wy-alert-success.attention,.rst-content .wy-alert-success.caution,.rst-content .wy-alert-success.danger,.rst-content .wy-alert-success.error,.rst-content .wy-alert-success.note,.rst-content .wy-alert-success.seealso,.rst-content .wy-alert-success.warning,.wy-alert.wy-alert-success{background:#dbfaf4}.rst-content .hint .admonition-title,.rst-content .hint .wy-alert-title,.rst-content .important .admonition-title,.rst-content .important .wy-alert-title,.rst-content .tip .admonition-title,.rst-content .tip .wy-alert-title,.rst-content .wy-alert-success.admonition-todo .admonition-title,.rst-content .wy-alert-success.admonition-todo .wy-alert-title,.rst-content .wy-alert-success.admonition .admonition-title,.rst-content .wy-alert-success.admonition .wy-alert-title,.rst-content .wy-alert-success.attention .admonition-title,.rst-content .wy-alert-success.attention .wy-alert-title,.rst-content .wy-alert-success.caution .admonition-title,.rst-content .wy-alert-success.caution .wy-alert-title,.rst-content .wy-alert-success.danger .admonition-title,.rst-content .wy-alert-success.danger .wy-alert-title,.rst-content .wy-alert-success.error .admonition-title,.rst-content .wy-alert-success.error .wy-alert-title,.rst-content .wy-alert-success.note .admonition-title,.rst-content .wy-alert-success.note .wy-alert-title,.rst-content .wy-alert-success.seealso .admonition-title,.rst-content .wy-alert-success.seealso .wy-alert-title,.rst-content .wy-alert-success.warning .admonition-title,.rst-content .wy-alert-success.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-success .admonition-title,.wy-alert.wy-alert-success .rst-content .admonition-title,.wy-alert.wy-alert-success .wy-alert-title{background:#1abc9c}.rst-content .wy-alert-neutral.admonition,.rst-content .wy-alert-neutral.admonition-todo,.rst-content .wy-alert-neutral.attention,.rst-content .wy-alert-neutral.caution,.rst-content .wy-alert-neutral.danger,.rst-content .wy-alert-neutral.error,.rst-content .wy-alert-neutral.hint,.rst-content .wy-alert-neutral.important,.rst-content .wy-alert-neutral.note,.rst-content .wy-alert-neutral.seealso,.rst-content .wy-alert-neutral.tip,.rst-content .wy-alert-neutral.warning,.wy-alert.wy-alert-neutral{background:#f3f6f6}.rst-content .wy-alert-neutral.admonition-todo .admonition-title,.rst-content .wy-alert-neutral.admonition-todo .wy-alert-title,.rst-content .wy-alert-neutral.admonition .admonition-title,.rst-content .wy-alert-neutral.admonition .wy-alert-title,.rst-content .wy-alert-neutral.attention .admonition-title,.rst-content .wy-alert-neutral.attention .wy-alert-title,.rst-content .wy-alert-neutral.caution .admonition-title,.rst-content .wy-alert-neutral.caution .wy-alert-title,.rst-content .wy-alert-neutral.danger .admonition-title,.rst-content .wy-alert-neutral.danger .wy-alert-title,.rst-content .wy-alert-neutral.error .admonition-title,.rst-content .wy-alert-neutral.error .wy-alert-title,.rst-content .wy-alert-neutral.hint .admonition-title,.rst-content .wy-alert-neutral.hint .wy-alert-title,.rst-content .wy-alert-neutral.important .admonition-title,.rst-content .wy-alert-neutral.important .wy-alert-title,.rst-content .wy-alert-neutral.note .admonition-title,.rst-content .wy-alert-neutral.note .wy-alert-title,.rst-content .wy-alert-neutral.seealso .admonition-title,.rst-content .wy-alert-neutral.seealso .wy-alert-title,.rst-content .wy-alert-neutral.tip .admonition-title,.rst-content .wy-alert-neutral.tip .wy-alert-title,.rst-content .wy-alert-neutral.warning .admonition-title,.rst-content .wy-alert-neutral.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-neutral .admonition-title,.wy-alert.wy-alert-neutral .rst-content .admonition-title,.wy-alert.wy-alert-neutral .wy-alert-title{color:#404040;background:#e1e4e5}.rst-content .wy-alert-neutral.admonition-todo a,.rst-content .wy-alert-neutral.admonition a,.rst-content .wy-alert-neutral.attention a,.rst-content .wy-alert-neutral.caution a,.rst-content .wy-alert-neutral.danger a,.rst-content .wy-alert-neutral.error a,.rst-content .wy-alert-neutral.hint a,.rst-content .wy-alert-neutral.important a,.rst-content .wy-alert-neutral.note a,.rst-content .wy-alert-neutral.seealso a,.rst-content .wy-alert-neutral.tip a,.rst-content .wy-alert-neutral.warning a,.wy-alert.wy-alert-neutral a{color:#2980b9}.rst-content .admonition-todo p:last-child,.rst-content .admonition p:last-child,.rst-content .attention p:last-child,.rst-content .caution p:last-child,.rst-content .danger p:last-child,.rst-content .error p:last-child,.rst-content .hint p:last-child,.rst-content .important p:last-child,.rst-content .note p:last-child,.rst-content .seealso p:last-child,.rst-content .tip p:last-child,.rst-content .warning p:last-child,.wy-alert p:last-child{margin-bottom:0}.wy-tray-container{position:fixed;bottom:0;left:0;z-index:600}.wy-tray-container li{display:block;width:300px;background:transparent;color:#fff;text-align:center;box-shadow:0 5px 5px 0 rgba(0,0,0,.1);padding:0 24px;min-width:20%;opacity:0;height:0;line-height:56px;overflow:hidden;-webkit-transition:all .3s ease-in;-moz-transition:all .3s ease-in;transition:all .3s ease-in}.wy-tray-container li.wy-tray-item-success{background:#27ae60}.wy-tray-container li.wy-tray-item-info{background:#2980b9}.wy-tray-container li.wy-tray-item-warning{background:#e67e22}.wy-tray-container li.wy-tray-item-danger{background:#e74c3c}.wy-tray-container li.on{opacity:1;height:56px}@media screen and (max-width:768px){.wy-tray-container{bottom:auto;top:0;width:100%}.wy-tray-container li{width:100%}}button{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle;cursor:pointer;line-height:normal;-webkit-appearance:button;*overflow:visible}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}button[disabled]{cursor:default}.btn{display:inline-block;border-radius:2px;line-height:normal;white-space:nowrap;text-align:center;cursor:pointer;font-size:100%;padding:6px 12px 8px;color:#fff;border:1px solid rgba(0,0,0,.1);background-color:#27ae60;text-decoration:none;font-weight:400;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 2px -1px hsla(0,0%,100%,.5),inset 0 -2px 0 0 rgba(0,0,0,.1);outline-none:false;vertical-align:middle;*display:inline;zoom:1;-webkit-user-drag:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;-webkit-transition:all .1s linear;-moz-transition:all .1s linear;transition:all .1s linear}.btn-hover{background:#2e8ece;color:#fff}.btn:hover{background:#2cc36b;color:#fff}.btn:focus{background:#2cc36b;outline:0}.btn:active{box-shadow:inset 0 -1px 0 0 rgba(0,0,0,.05),inset 0 2px 0 0 rgba(0,0,0,.1);padding:8px 12px 6px}.btn:visited{color:#fff}.btn-disabled,.btn-disabled:active,.btn-disabled:focus,.btn-disabled:hover,.btn:disabled{background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=40);opacity:.4;cursor:not-allowed;box-shadow:none}.btn::-moz-focus-inner{padding:0;border:0}.btn-small{font-size:80%}.btn-info{background-color:#2980b9!important}.btn-info:hover{background-color:#2e8ece!important}.btn-neutral{background-color:#f3f6f6!important;color:#404040!important}.btn-neutral:hover{background-color:#e5ebeb!important;color:#404040}.btn-neutral:visited{color:#404040!important}.btn-success{background-color:#27ae60!important}.btn-success:hover{background-color:#295!important}.btn-danger{background-color:#e74c3c!important}.btn-danger:hover{background-color:#ea6153!important}.btn-warning{background-color:#e67e22!important}.btn-warning:hover{background-color:#e98b39!important}.btn-invert{background-color:#222}.btn-invert:hover{background-color:#2f2f2f!important}.btn-link{background-color:transparent!important;color:#2980b9;box-shadow:none;border-color:transparent!important}.btn-link:active,.btn-link:hover{background-color:transparent!important;color:#409ad5!important;box-shadow:none}.btn-link:visited{color:#9b59b6}.wy-btn-group .btn,.wy-control .btn{vertical-align:middle}.wy-btn-group{margin-bottom:24px;*zoom:1}.wy-btn-group:after,.wy-btn-group:before{display:table;content:""}.wy-btn-group:after{clear:both}.wy-dropdown{position:relative;display:inline-block}.wy-dropdown-active .wy-dropdown-menu{display:block}.wy-dropdown-menu{position:absolute;left:0;display:none;float:left;top:100%;min-width:100%;background:#fcfcfc;z-index:100;border:1px solid #cfd7dd;box-shadow:0 2px 2px 0 rgba(0,0,0,.1);padding:12px}.wy-dropdown-menu>dd>a{display:block;clear:both;color:#404040;white-space:nowrap;font-size:90%;padding:0 12px;cursor:pointer}.wy-dropdown-menu>dd>a:hover{background:#2980b9;color:#fff}.wy-dropdown-menu>dd.divider{border-top:1px solid #cfd7dd;margin:6px 0}.wy-dropdown-menu>dd.search{padding-bottom:12px}.wy-dropdown-menu>dd.search input[type=search]{width:100%}.wy-dropdown-menu>dd.call-to-action{background:#e3e3e3;text-transform:uppercase;font-weight:500;font-size:80%}.wy-dropdown-menu>dd.call-to-action:hover{background:#e3e3e3}.wy-dropdown-menu>dd.call-to-action .btn{color:#fff}.wy-dropdown.wy-dropdown-up .wy-dropdown-menu{bottom:100%;top:auto;left:auto;right:0}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu{background:#fcfcfc;margin-top:2px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a{padding:6px 12px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a:hover{background:#2980b9;color:#fff}.wy-dropdown.wy-dropdown-left .wy-dropdown-menu{right:0;left:auto;text-align:right}.wy-dropdown-arrow:before{content:" ";border-bottom:5px solid #f5f5f5;border-left:5px solid transparent;border-right:5px solid transparent;position:absolute;display:block;top:-4px;left:50%;margin-left:-3px}.wy-dropdown-arrow.wy-dropdown-arrow-left:before{left:11px}.wy-form-stacked select{display:block}.wy-form-aligned .wy-help-inline,.wy-form-aligned input,.wy-form-aligned label,.wy-form-aligned select,.wy-form-aligned textarea{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-form-aligned .wy-control-group>label{display:inline-block;vertical-align:middle;width:10em;margin:6px 12px 0 0;float:left}.wy-form-aligned .wy-control{float:left}.wy-form-aligned .wy-control label{display:block}.wy-form-aligned .wy-control select{margin-top:6px}fieldset{margin:0}fieldset,legend{border:0;padding:0}legend{width:100%;white-space:normal;margin-bottom:24px;font-size:150%;*margin-left:-7px}label,legend{display:block}label{margin:0 0 .3125em;color:#333;font-size:90%}input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}.wy-control-group{margin-bottom:24px;max-width:1200px;margin-left:auto;margin-right:auto;*zoom:1}.wy-control-group:after,.wy-control-group:before{display:table;content:""}.wy-control-group:after{clear:both}.wy-control-group.wy-control-group-required>label:after{content:" *";color:#e74c3c}.wy-control-group .wy-form-full,.wy-control-group .wy-form-halves,.wy-control-group .wy-form-thirds{padding-bottom:12px}.wy-control-group .wy-form-full input[type=color],.wy-control-group .wy-form-full input[type=date],.wy-control-group .wy-form-full input[type=datetime-local],.wy-control-group .wy-form-full input[type=datetime],.wy-control-group .wy-form-full input[type=email],.wy-control-group .wy-form-full input[type=month],.wy-control-group .wy-form-full input[type=number],.wy-control-group .wy-form-full input[type=password],.wy-control-group .wy-form-full input[type=search],.wy-control-group .wy-form-full input[type=tel],.wy-control-group .wy-form-full input[type=text],.wy-control-group .wy-form-full input[type=time],.wy-control-group .wy-form-full input[type=url],.wy-control-group .wy-form-full input[type=week],.wy-control-group .wy-form-full select,.wy-control-group .wy-form-halves input[type=color],.wy-control-group .wy-form-halves input[type=date],.wy-control-group .wy-form-halves input[type=datetime-local],.wy-control-group .wy-form-halves input[type=datetime],.wy-control-group .wy-form-halves input[type=email],.wy-control-group .wy-form-halves input[type=month],.wy-control-group .wy-form-halves input[type=number],.wy-control-group .wy-form-halves input[type=password],.wy-control-group .wy-form-halves input[type=search],.wy-control-group .wy-form-halves input[type=tel],.wy-control-group .wy-form-halves input[type=text],.wy-control-group .wy-form-halves input[type=time],.wy-control-group .wy-form-halves input[type=url],.wy-control-group .wy-form-halves input[type=week],.wy-control-group .wy-form-halves select,.wy-control-group .wy-form-thirds input[type=color],.wy-control-group .wy-form-thirds input[type=date],.wy-control-group .wy-form-thirds input[type=datetime-local],.wy-control-group .wy-form-thirds input[type=datetime],.wy-control-group .wy-form-thirds input[type=email],.wy-control-group .wy-form-thirds input[type=month],.wy-control-group .wy-form-thirds input[type=number],.wy-control-group .wy-form-thirds input[type=password],.wy-control-group .wy-form-thirds input[type=search],.wy-control-group .wy-form-thirds input[type=tel],.wy-control-group .wy-form-thirds input[type=text],.wy-control-group .wy-form-thirds input[type=time],.wy-control-group .wy-form-thirds input[type=url],.wy-control-group .wy-form-thirds input[type=week],.wy-control-group .wy-form-thirds select{width:100%}.wy-control-group .wy-form-full{float:left;display:block;width:100%;margin-right:0}.wy-control-group .wy-form-full:last-child{margin-right:0}.wy-control-group .wy-form-halves{float:left;display:block;margin-right:2.35765%;width:48.82117%}.wy-control-group .wy-form-halves:last-child,.wy-control-group .wy-form-halves:nth-of-type(2n){margin-right:0}.wy-control-group .wy-form-halves:nth-of-type(odd){clear:left}.wy-control-group .wy-form-thirds{float:left;display:block;margin-right:2.35765%;width:31.76157%}.wy-control-group .wy-form-thirds:last-child,.wy-control-group .wy-form-thirds:nth-of-type(3n){margin-right:0}.wy-control-group .wy-form-thirds:nth-of-type(3n+1){clear:left}.wy-control-group.wy-control-group-no-input .wy-control,.wy-control-no-input{margin:6px 0 0;font-size:90%}.wy-control-no-input{display:inline-block}.wy-control-group.fluid-input input[type=color],.wy-control-group.fluid-input input[type=date],.wy-control-group.fluid-input input[type=datetime-local],.wy-control-group.fluid-input input[type=datetime],.wy-control-group.fluid-input input[type=email],.wy-control-group.fluid-input input[type=month],.wy-control-group.fluid-input input[type=number],.wy-control-group.fluid-input input[type=password],.wy-control-group.fluid-input input[type=search],.wy-control-group.fluid-input input[type=tel],.wy-control-group.fluid-input input[type=text],.wy-control-group.fluid-input input[type=time],.wy-control-group.fluid-input input[type=url],.wy-control-group.fluid-input input[type=week]{width:100%}.wy-form-message-inline{padding-left:.3em;color:#666;font-size:90%}.wy-form-message{display:block;color:#999;font-size:70%;margin-top:.3125em;font-style:italic}.wy-form-message p{font-size:inherit;font-style:italic;margin-bottom:6px}.wy-form-message p:last-child{margin-bottom:0}input{line-height:normal}input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;*overflow:visible}input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week]{-webkit-appearance:none;padding:6px;display:inline-block;border:1px solid #ccc;font-size:80%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 3px #ddd;border-radius:0;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}input[type=datetime-local]{padding:.34375em .625em}input[disabled]{cursor:default}input[type=checkbox],input[type=radio]{padding:0;margin-right:.3125em;*height:13px;*width:13px}input[type=checkbox],input[type=radio],input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus{outline:0;outline:thin dotted\9;border-color:#333}input.no-focus:focus{border-color:#ccc!important}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:thin dotted #333;outline:1px auto #129fea}input[type=color][disabled],input[type=date][disabled],input[type=datetime-local][disabled],input[type=datetime][disabled],input[type=email][disabled],input[type=month][disabled],input[type=number][disabled],input[type=password][disabled],input[type=search][disabled],input[type=tel][disabled],input[type=text][disabled],input[type=time][disabled],input[type=url][disabled],input[type=week][disabled]{cursor:not-allowed;background-color:#fafafa}input:focus:invalid,select:focus:invalid,textarea:focus:invalid{color:#e74c3c;border:1px solid #e74c3c}input:focus:invalid:focus,select:focus:invalid:focus,textarea:focus:invalid:focus{border-color:#e74c3c}input[type=checkbox]:focus:invalid:focus,input[type=file]:focus:invalid:focus,input[type=radio]:focus:invalid:focus{outline-color:#e74c3c}input.wy-input-large{padding:12px;font-size:100%}textarea{overflow:auto;vertical-align:top;width:100%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif}select,textarea{padding:.5em .625em;display:inline-block;border:1px solid #ccc;font-size:80%;box-shadow:inset 0 1px 3px #ddd;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}select{border:1px solid #ccc;background-color:#fff}select[multiple]{height:auto}select:focus,textarea:focus{outline:0}input[readonly],select[disabled],select[readonly],textarea[disabled],textarea[readonly]{cursor:not-allowed;background-color:#fafafa}input[type=checkbox][disabled],input[type=radio][disabled]{cursor:not-allowed}.wy-checkbox,.wy-radio{margin:6px 0;color:#404040;display:block}.wy-checkbox input,.wy-radio input{vertical-align:baseline}.wy-form-message-inline{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-input-prefix,.wy-input-suffix{white-space:nowrap;padding:6px}.wy-input-prefix .wy-input-context,.wy-input-suffix .wy-input-context{line-height:27px;padding:0 8px;display:inline-block;font-size:80%;background-color:#f3f6f6;border:1px solid #ccc;color:#999}.wy-input-suffix .wy-input-context{border-left:0}.wy-input-prefix .wy-input-context{border-right:0}.wy-switch{position:relative;display:block;height:24px;margin-top:12px;cursor:pointer}.wy-switch:before{left:0;top:0;width:36px;height:12px;background:#ccc}.wy-switch:after,.wy-switch:before{position:absolute;content:"";display:block;border-radius:4px;-webkit-transition:all .2s ease-in-out;-moz-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.wy-switch:after{width:18px;height:18px;background:#999;left:-3px;top:-3px}.wy-switch span{position:absolute;left:48px;display:block;font-size:12px;color:#ccc;line-height:1}.wy-switch.active:before{background:#1e8449}.wy-switch.active:after{left:24px;background:#27ae60}.wy-switch.disabled{cursor:not-allowed;opacity:.8}.wy-control-group.wy-control-group-error .wy-form-message,.wy-control-group.wy-control-group-error>label{color:#e74c3c}.wy-control-group.wy-control-group-error input[type=color],.wy-control-group.wy-control-group-error input[type=date],.wy-control-group.wy-control-group-error input[type=datetime-local],.wy-control-group.wy-control-group-error input[type=datetime],.wy-control-group.wy-control-group-error input[type=email],.wy-control-group.wy-control-group-error input[type=month],.wy-control-group.wy-control-group-error input[type=number],.wy-control-group.wy-control-group-error input[type=password],.wy-control-group.wy-control-group-error input[type=search],.wy-control-group.wy-control-group-error input[type=tel],.wy-control-group.wy-control-group-error input[type=text],.wy-control-group.wy-control-group-error input[type=time],.wy-control-group.wy-control-group-error input[type=url],.wy-control-group.wy-control-group-error input[type=week],.wy-control-group.wy-control-group-error textarea{border:1px solid #e74c3c}.wy-inline-validate{white-space:nowrap}.wy-inline-validate .wy-input-context{padding:.5em .625em;display:inline-block;font-size:80%}.wy-inline-validate.wy-inline-validate-success .wy-input-context{color:#27ae60}.wy-inline-validate.wy-inline-validate-danger .wy-input-context{color:#e74c3c}.wy-inline-validate.wy-inline-validate-warning .wy-input-context{color:#e67e22}.wy-inline-validate.wy-inline-validate-info .wy-input-context{color:#2980b9}.rotate-90{-webkit-transform:rotate(90deg);-moz-transform:rotate(90deg);-ms-transform:rotate(90deg);-o-transform:rotate(90deg);transform:rotate(90deg)}.rotate-180{-webkit-transform:rotate(180deg);-moz-transform:rotate(180deg);-ms-transform:rotate(180deg);-o-transform:rotate(180deg);transform:rotate(180deg)}.rotate-270{-webkit-transform:rotate(270deg);-moz-transform:rotate(270deg);-ms-transform:rotate(270deg);-o-transform:rotate(270deg);transform:rotate(270deg)}.mirror{-webkit-transform:scaleX(-1);-moz-transform:scaleX(-1);-ms-transform:scaleX(-1);-o-transform:scaleX(-1);transform:scaleX(-1)}.mirror.rotate-90{-webkit-transform:scaleX(-1) rotate(90deg);-moz-transform:scaleX(-1) rotate(90deg);-ms-transform:scaleX(-1) rotate(90deg);-o-transform:scaleX(-1) rotate(90deg);transform:scaleX(-1) rotate(90deg)}.mirror.rotate-180{-webkit-transform:scaleX(-1) rotate(180deg);-moz-transform:scaleX(-1) rotate(180deg);-ms-transform:scaleX(-1) rotate(180deg);-o-transform:scaleX(-1) rotate(180deg);transform:scaleX(-1) rotate(180deg)}.mirror.rotate-270{-webkit-transform:scaleX(-1) rotate(270deg);-moz-transform:scaleX(-1) rotate(270deg);-ms-transform:scaleX(-1) rotate(270deg);-o-transform:scaleX(-1) rotate(270deg);transform:scaleX(-1) rotate(270deg)}@media only screen and (max-width:480px){.wy-form button[type=submit]{margin:.7em 0 0}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=text],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week],.wy-form label{margin-bottom:.3em;display:block}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week]{margin-bottom:0}.wy-form-aligned .wy-control-group label{margin-bottom:.3em;text-align:left;display:block;width:100%}.wy-form-aligned .wy-control{margin:1.5em 0 0}.wy-form-message,.wy-form-message-inline,.wy-form .wy-help-inline{display:block;font-size:80%;padding:6px 0}}@media screen and (max-width:768px){.tablet-hide{display:none}}@media screen and (max-width:480px){.mobile-hide{display:none}}.float-left{float:left}.float-right{float:right}.full-width{width:100%}.rst-content table.docutils,.rst-content table.field-list,.wy-table{border-collapse:collapse;border-spacing:0;empty-cells:show;margin-bottom:24px}.rst-content table.docutils caption,.rst-content table.field-list caption,.wy-table caption{color:#000;font:italic 85%/1 arial,sans-serif;padding:1em 0;text-align:center}.rst-content table.docutils td,.rst-content table.docutils th,.rst-content table.field-list td,.rst-content table.field-list th,.wy-table td,.wy-table th{font-size:90%;margin:0;overflow:visible;padding:8px 16px}.rst-content table.docutils td:first-child,.rst-content table.docutils th:first-child,.rst-content table.field-list td:first-child,.rst-content table.field-list th:first-child,.wy-table td:first-child,.wy-table th:first-child{border-left-width:0}.rst-content table.docutils thead,.rst-content table.field-list thead,.wy-table thead{color:#000;text-align:left;vertical-align:bottom;white-space:nowrap}.rst-content table.docutils thead th,.rst-content table.field-list thead th,.wy-table thead th{font-weight:700;border-bottom:2px solid #e1e4e5}.rst-content table.docutils td,.rst-content table.field-list td,.wy-table td{background-color:transparent;vertical-align:middle}.rst-content table.docutils td p,.rst-content table.field-list td p,.wy-table td p{line-height:18px}.rst-content table.docutils td p:last-child,.rst-content table.field-list td p:last-child,.wy-table td p:last-child{margin-bottom:0}.rst-content table.docutils .wy-table-cell-min,.rst-content table.field-list .wy-table-cell-min,.wy-table .wy-table-cell-min{width:1%;padding-right:0}.rst-content table.docutils .wy-table-cell-min input[type=checkbox],.rst-content table.field-list .wy-table-cell-min input[type=checkbox],.wy-table .wy-table-cell-min input[type=checkbox]{margin:0}.wy-table-secondary{color:grey;font-size:90%}.wy-table-tertiary{color:grey;font-size:80%}.rst-content table.docutils:not(.field-list) tr:nth-child(2n-1) td,.wy-table-backed,.wy-table-odd td,.wy-table-striped tr:nth-child(2n-1) td{background-color:#f3f6f6}.rst-content table.docutils,.wy-table-bordered-all{border:1px solid #e1e4e5}.rst-content table.docutils td,.wy-table-bordered-all td{border-bottom:1px solid #e1e4e5;border-left:1px solid #e1e4e5}.rst-content table.docutils tbody>tr:last-child td,.wy-table-bordered-all tbody>tr:last-child td{border-bottom-width:0}.wy-table-bordered{border:1px solid #e1e4e5}.wy-table-bordered-rows td{border-bottom:1px solid #e1e4e5}.wy-table-bordered-rows tbody>tr:last-child td{border-bottom-width:0}.wy-table-horizontal td,.wy-table-horizontal th{border-width:0 0 1px;border-bottom:1px solid #e1e4e5}.wy-table-horizontal tbody>tr:last-child td{border-bottom-width:0}.wy-table-responsive{margin-bottom:24px;max-width:100%;overflow:auto}.wy-table-responsive table{margin-bottom:0!important}.wy-table-responsive table td,.wy-table-responsive table th{white-space:nowrap}a{color:#2980b9;text-decoration:none;cursor:pointer}a:hover{color:#3091d1}a:visited{color:#9b59b6}html{height:100%}body,html{overflow-x:hidden}body{font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;font-weight:400;color:#404040;min-height:100%;background:#edf0f2}.wy-text-left{text-align:left}.wy-text-center{text-align:center}.wy-text-right{text-align:right}.wy-text-large{font-size:120%}.wy-text-normal{font-size:100%}.wy-text-small,small{font-size:80%}.wy-text-strike{text-decoration:line-through}.wy-text-warning{color:#e67e22!important}a.wy-text-warning:hover{color:#eb9950!important}.wy-text-info{color:#2980b9!important}a.wy-text-info:hover{color:#409ad5!important}.wy-text-success{color:#27ae60!important}a.wy-text-success:hover{color:#36d278!important}.wy-text-danger{color:#e74c3c!important}a.wy-text-danger:hover{color:#ed7669!important}.wy-text-neutral{color:#404040!important}a.wy-text-neutral:hover{color:#595959!important}.rst-content .toctree-wrapper>p.caption,h1,h2,h3,h4,h5,h6,legend{margin-top:0;font-weight:700;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif}p{line-height:24px;font-size:16px;margin:0 0 24px}h1{font-size:175%}.rst-content .toctree-wrapper>p.caption,h2{font-size:150%}h3{font-size:125%}h4{font-size:115%}h5{font-size:110%}h6{font-size:100%}hr{display:block;height:1px;border:0;border-top:1px solid #e1e4e5;margin:24px 0;padding:0}.rst-content code,.rst-content tt,code{white-space:nowrap;max-width:100%;background:#fff;border:1px solid #e1e4e5;font-size:75%;padding:0 5px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#e74c3c;overflow-x:auto}.rst-content tt.code-large,code.code-large{font-size:90%}.rst-content .section ul,.rst-content .toctree-wrapper ul,.rst-content section ul,.wy-plain-list-disc,article ul{list-style:disc;line-height:24px;margin-bottom:24px}.rst-content .section ul li,.rst-content .toctree-wrapper ul li,.rst-content section ul li,.wy-plain-list-disc li,article ul li{list-style:disc;margin-left:24px}.rst-content .section ul li p:last-child,.rst-content .section ul li ul,.rst-content .toctree-wrapper ul li p:last-child,.rst-content .toctree-wrapper ul li ul,.rst-content section ul li p:last-child,.rst-content section ul li ul,.wy-plain-list-disc li p:last-child,.wy-plain-list-disc li ul,article ul li p:last-child,article ul li ul{margin-bottom:0}.rst-content .section ul li li,.rst-content .toctree-wrapper ul li li,.rst-content section ul li li,.wy-plain-list-disc li li,article ul li li{list-style:circle}.rst-content .section ul li li li,.rst-content .toctree-wrapper ul li li li,.rst-content section ul li li li,.wy-plain-list-disc li li li,article ul li li li{list-style:square}.rst-content .section ul li ol li,.rst-content .toctree-wrapper ul li ol li,.rst-content section ul li ol li,.wy-plain-list-disc li ol li,article ul li ol li{list-style:decimal}.rst-content .section ol,.rst-content .section ol.arabic,.rst-content .toctree-wrapper ol,.rst-content .toctree-wrapper ol.arabic,.rst-content section ol,.rst-content section ol.arabic,.wy-plain-list-decimal,article ol{list-style:decimal;line-height:24px;margin-bottom:24px}.rst-content .section ol.arabic li,.rst-content .section ol li,.rst-content .toctree-wrapper ol.arabic li,.rst-content .toctree-wrapper ol li,.rst-content section ol.arabic li,.rst-content section ol li,.wy-plain-list-decimal li,article ol li{list-style:decimal;margin-left:24px}.rst-content .section ol.arabic li ul,.rst-content .section ol li p:last-child,.rst-content .section ol li ul,.rst-content .toctree-wrapper ol.arabic li ul,.rst-content .toctree-wrapper ol li p:last-child,.rst-content .toctree-wrapper ol li ul,.rst-content section ol.arabic li ul,.rst-content section ol li p:last-child,.rst-content section ol li ul,.wy-plain-list-decimal li p:last-child,.wy-plain-list-decimal li ul,article ol li p:last-child,article ol li ul{margin-bottom:0}.rst-content .section ol.arabic li ul li,.rst-content .section ol li ul li,.rst-content .toctree-wrapper ol.arabic li ul li,.rst-content .toctree-wrapper ol li ul li,.rst-content section ol.arabic li ul li,.rst-content section ol li ul li,.wy-plain-list-decimal li ul li,article ol li ul li{list-style:disc}.wy-breadcrumbs{*zoom:1}.wy-breadcrumbs:after,.wy-breadcrumbs:before{display:table;content:""}.wy-breadcrumbs:after{clear:both}.wy-breadcrumbs>li{display:inline-block;padding-top:5px}.wy-breadcrumbs>li.wy-breadcrumbs-aside{float:right}.rst-content .wy-breadcrumbs>li code,.rst-content .wy-breadcrumbs>li tt,.wy-breadcrumbs>li .rst-content tt,.wy-breadcrumbs>li code{all:inherit;color:inherit}.breadcrumb-item:before{content:"/";color:#bbb;font-size:13px;padding:0 6px 0 3px}.wy-breadcrumbs-extra{margin-bottom:0;color:#b3b3b3;font-size:80%;display:inline-block}@media screen and (max-width:480px){.wy-breadcrumbs-extra,.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}@media print{.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}html{font-size:16px}.wy-affix{position:fixed;top:1.618em}.wy-menu a:hover{text-decoration:none}.wy-menu-horiz{*zoom:1}.wy-menu-horiz:after,.wy-menu-horiz:before{display:table;content:""}.wy-menu-horiz:after{clear:both}.wy-menu-horiz li,.wy-menu-horiz ul{display:inline-block}.wy-menu-horiz li:hover{background:hsla(0,0%,100%,.1)}.wy-menu-horiz li.divide-left{border-left:1px solid #404040}.wy-menu-horiz li.divide-right{border-right:1px solid #404040}.wy-menu-horiz a{height:32px;display:inline-block;line-height:32px;padding:0 16px}.wy-menu-vertical{width:300px}.wy-menu-vertical header,.wy-menu-vertical p.caption{color:#55a5d9;height:32px;line-height:32px;padding:0 1.618em;margin:12px 0 0;display:block;font-weight:700;text-transform:uppercase;font-size:85%;white-space:nowrap}.wy-menu-vertical ul{margin-bottom:0}.wy-menu-vertical li.divide-top{border-top:1px solid #404040}.wy-menu-vertical li.divide-bottom{border-bottom:1px solid #404040}.wy-menu-vertical li.current{background:#e3e3e3}.wy-menu-vertical li.current a{color:grey;border-right:1px solid #c9c9c9;padding:.4045em 2.427em}.wy-menu-vertical li.current a:hover{background:#d6d6d6}.rst-content .wy-menu-vertical li tt,.wy-menu-vertical li .rst-content tt,.wy-menu-vertical li code{border:none;background:inherit;color:inherit;padding-left:0;padding-right:0}.wy-menu-vertical li button.toctree-expand{display:block;float:left;margin-left:-1.2em;line-height:18px;color:#4d4d4d;border:none;background:none;padding:0}.wy-menu-vertical li.current>a,.wy-menu-vertical li.on a{color:#404040;font-weight:700;position:relative;background:#fcfcfc;border:none;padding:.4045em 1.618em}.wy-menu-vertical li.current>a:hover,.wy-menu-vertical li.on a:hover{background:#fcfcfc}.wy-menu-vertical li.current>a:hover button.toctree-expand,.wy-menu-vertical li.on a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand{display:block;line-height:18px;color:#333}.wy-menu-vertical li.toctree-l1.current>a{border-bottom:1px solid #c9c9c9;border-top:1px solid #c9c9c9}.wy-menu-vertical .toctree-l1.current .toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .toctree-l11>ul{display:none}.wy-menu-vertical .toctree-l1.current .current.toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .current.toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .current.toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .current.toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .current.toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .current.toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .current.toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .current.toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .current.toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .current.toctree-l11>ul{display:block}.wy-menu-vertical li.toctree-l3,.wy-menu-vertical li.toctree-l4{font-size:.9em}.wy-menu-vertical li.toctree-l2 a,.wy-menu-vertical li.toctree-l3 a,.wy-menu-vertical li.toctree-l4 a,.wy-menu-vertical li.toctree-l5 a,.wy-menu-vertical li.toctree-l6 a,.wy-menu-vertical li.toctree-l7 a,.wy-menu-vertical li.toctree-l8 a,.wy-menu-vertical li.toctree-l9 a,.wy-menu-vertical li.toctree-l10 a{color:#404040}.wy-menu-vertical li.toctree-l2 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l3 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l4 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l5 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l6 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l7 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l8 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l9 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l10 a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a,.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a,.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a,.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a,.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a,.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a,.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a,.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{display:block}.wy-menu-vertical li.toctree-l2.current>a{padding:.4045em 2.427em}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{padding:.4045em 1.618em .4045em 4.045em}.wy-menu-vertical li.toctree-l3.current>a{padding:.4045em 4.045em}.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{padding:.4045em 1.618em .4045em 5.663em}.wy-menu-vertical li.toctree-l4.current>a{padding:.4045em 5.663em}.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a{padding:.4045em 1.618em .4045em 7.281em}.wy-menu-vertical li.toctree-l5.current>a{padding:.4045em 7.281em}.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a{padding:.4045em 1.618em .4045em 8.899em}.wy-menu-vertical li.toctree-l6.current>a{padding:.4045em 8.899em}.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a{padding:.4045em 1.618em .4045em 10.517em}.wy-menu-vertical li.toctree-l7.current>a{padding:.4045em 10.517em}.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a{padding:.4045em 1.618em .4045em 12.135em}.wy-menu-vertical li.toctree-l8.current>a{padding:.4045em 12.135em}.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a{padding:.4045em 1.618em .4045em 13.753em}.wy-menu-vertical li.toctree-l9.current>a{padding:.4045em 13.753em}.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a{padding:.4045em 1.618em .4045em 15.371em}.wy-menu-vertical li.toctree-l10.current>a{padding:.4045em 15.371em}.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{padding:.4045em 1.618em .4045em 16.989em}.wy-menu-vertical li.toctree-l2.current>a,.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{background:#c9c9c9}.wy-menu-vertical li.toctree-l2 button.toctree-expand{color:#a3a3a3}.wy-menu-vertical li.toctree-l3.current>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{background:#bdbdbd}.wy-menu-vertical li.toctree-l3 button.toctree-expand{color:#969696}.wy-menu-vertical li.current ul{display:block}.wy-menu-vertical li ul{margin-bottom:0;display:none}.wy-menu-vertical li ul li a{margin-bottom:0;color:#d9d9d9;font-weight:400}.wy-menu-vertical a{line-height:18px;padding:.4045em 1.618em;display:block;position:relative;font-size:90%;color:#d9d9d9}.wy-menu-vertical a:hover{background-color:#4e4a4a;cursor:pointer}.wy-menu-vertical a:hover button.toctree-expand{color:#d9d9d9}.wy-menu-vertical a:active{background-color:#2980b9;cursor:pointer;color:#fff}.wy-menu-vertical a:active button.toctree-expand{color:#fff}.wy-side-nav-search{display:block;width:300px;padding:.809em;margin-bottom:.809em;z-index:200;background-color:#2980b9;text-align:center;color:#fcfcfc}.wy-side-nav-search input[type=text]{width:100%;border-radius:50px;padding:6px 12px;border-color:#2472a4}.wy-side-nav-search img{display:block;margin:auto auto .809em;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a{color:#fcfcfc;font-size:100%;font-weight:700;display:inline-block;padding:4px 6px;margin-bottom:.809em;max-width:100%}.wy-side-nav-search .wy-dropdown>a:hover,.wy-side-nav-search>a:hover{background:hsla(0,0%,100%,.1)}.wy-side-nav-search .wy-dropdown>a img.logo,.wy-side-nav-search>a img.logo{display:block;margin:0 auto;height:auto;width:auto;border-radius:0;max-width:100%;background:transparent}.wy-side-nav-search .wy-dropdown>a.icon img.logo,.wy-side-nav-search>a.icon img.logo{margin-top:.85em}.wy-side-nav-search>div.version{margin-top:-.4045em;margin-bottom:.809em;font-weight:400;color:hsla(0,0%,100%,.3)}.wy-nav .wy-menu-vertical header{color:#2980b9}.wy-nav .wy-menu-vertical a{color:#b3b3b3}.wy-nav .wy-menu-vertical a:hover{background-color:#2980b9;color:#fff}[data-menu-wrap]{-webkit-transition:all .2s ease-in;-moz-transition:all .2s ease-in;transition:all .2s ease-in;position:absolute;opacity:1;width:100%;opacity:0}[data-menu-wrap].move-center{left:0;right:auto;opacity:1}[data-menu-wrap].move-left{right:auto;left:-100%;opacity:0}[data-menu-wrap].move-right{right:-100%;left:auto;opacity:0}.wy-body-for-nav{background:#fcfcfc}.wy-grid-for-nav{position:absolute;width:100%;height:100%}.wy-nav-side{position:fixed;top:0;bottom:0;left:0;padding-bottom:2em;width:300px;overflow-x:hidden;overflow-y:hidden;min-height:100%;color:#9b9b9b;background:#343131;z-index:200}.wy-side-scroll{width:320px;position:relative;overflow-x:hidden;overflow-y:scroll;height:100%}.wy-nav-top{display:none;background:#2980b9;color:#fff;padding:.4045em .809em;position:relative;line-height:50px;text-align:center;font-size:100%;*zoom:1}.wy-nav-top:after,.wy-nav-top:before{display:table;content:""}.wy-nav-top:after{clear:both}.wy-nav-top a{color:#fff;font-weight:700}.wy-nav-top img{margin-right:12px;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-nav-top i{font-size:30px;float:left;cursor:pointer;padding-top:inherit}.wy-nav-content-wrap{margin-left:300px;background:#fcfcfc;min-height:100%}.wy-nav-content{padding:1.618em 3.236em;height:100%;max-width:800px;margin:auto}.wy-body-mask{position:fixed;width:100%;height:100%;background:rgba(0,0,0,.2);display:none;z-index:499}.wy-body-mask.on{display:block}footer{color:grey}footer p{margin-bottom:12px}.rst-content footer span.commit tt,footer span.commit .rst-content tt,footer span.commit code{padding:0;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:1em;background:none;border:none;color:grey}.rst-footer-buttons{*zoom:1}.rst-footer-buttons:after,.rst-footer-buttons:before{width:100%;display:table;content:""}.rst-footer-buttons:after{clear:both}.rst-breadcrumbs-buttons{margin-top:12px;*zoom:1}.rst-breadcrumbs-buttons:after,.rst-breadcrumbs-buttons:before{display:table;content:""}.rst-breadcrumbs-buttons:after{clear:both}#search-results .search li{margin-bottom:24px;border-bottom:1px solid #e1e4e5;padding-bottom:24px}#search-results .search li:first-child{border-top:1px solid #e1e4e5;padding-top:24px}#search-results .search li a{font-size:120%;margin-bottom:12px;display:inline-block}#search-results .context{color:grey;font-size:90%}.genindextable li>ul{margin-left:24px}@media screen and (max-width:768px){.wy-body-for-nav{background:#fcfcfc}.wy-nav-top{display:block}.wy-nav-side{left:-300px}.wy-nav-side.shift{width:85%;left:0}.wy-menu.wy-menu-vertical,.wy-side-nav-search,.wy-side-scroll{width:auto}.wy-nav-content-wrap{margin-left:0}.wy-nav-content-wrap .wy-nav-content{padding:1.618em}.wy-nav-content-wrap.shift{position:fixed;min-width:100%;left:85%;top:0;height:100%;overflow:hidden}}@media screen and (min-width:1100px){.wy-nav-content-wrap{background:rgba(0,0,0,.05)}.wy-nav-content{margin:0;background:#fcfcfc}}@media print{.rst-versions,.wy-nav-side,footer{display:none}.wy-nav-content-wrap{margin-left:0}}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60;*zoom:1}.rst-versions .rst-current-version:after,.rst-versions .rst-current-version:before{display:table;content:""}.rst-versions .rst-current-version:after{clear:both}.rst-content .code-block-caption .rst-versions .rst-current-version .headerlink,.rst-content .eqno .rst-versions .rst-current-version .headerlink,.rst-content .rst-versions .rst-current-version .admonition-title,.rst-content code.download .rst-versions .rst-current-version span:first-child,.rst-content dl dt .rst-versions .rst-current-version .headerlink,.rst-content h1 .rst-versions .rst-current-version .headerlink,.rst-content h2 .rst-versions .rst-current-version .headerlink,.rst-content h3 .rst-versions .rst-current-version .headerlink,.rst-content h4 .rst-versions .rst-current-version .headerlink,.rst-content h5 .rst-versions .rst-current-version .headerlink,.rst-content h6 .rst-versions .rst-current-version .headerlink,.rst-content p .rst-versions .rst-current-version .headerlink,.rst-content table>caption .rst-versions .rst-current-version .headerlink,.rst-content tt.download .rst-versions .rst-current-version span:first-child,.rst-versions .rst-current-version .fa,.rst-versions .rst-current-version .icon,.rst-versions .rst-current-version .rst-content .admonition-title,.rst-versions .rst-current-version .rst-content .code-block-caption .headerlink,.rst-versions .rst-current-version .rst-content .eqno .headerlink,.rst-versions .rst-current-version .rst-content code.download span:first-child,.rst-versions .rst-current-version .rst-content dl dt .headerlink,.rst-versions .rst-current-version .rst-content h1 .headerlink,.rst-versions .rst-current-version .rst-content h2 .headerlink,.rst-versions .rst-current-version .rst-content h3 .headerlink,.rst-versions .rst-current-version .rst-content h4 .headerlink,.rst-versions .rst-current-version .rst-content h5 .headerlink,.rst-versions .rst-current-version .rst-content h6 .headerlink,.rst-versions .rst-current-version .rst-content p .headerlink,.rst-versions .rst-current-version .rst-content table>caption .headerlink,.rst-versions .rst-current-version .rst-content tt.download span:first-child,.rst-versions .rst-current-version .wy-menu-vertical li button.toctree-expand,.wy-menu-vertical li .rst-versions .rst-current-version button.toctree-expand{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}.rst-content .toctree-wrapper>p.caption,.rst-content h1,.rst-content h2,.rst-content h3,.rst-content h4,.rst-content h5,.rst-content h6{margin-bottom:24px}.rst-content img{max-width:100%;height:auto}.rst-content div.figure,.rst-content figure{margin-bottom:24px}.rst-content div.figure .caption-text,.rst-content figure .caption-text{font-style:italic}.rst-content div.figure p:last-child.caption,.rst-content figure p:last-child.caption{margin-bottom:0}.rst-content div.figure.align-center,.rst-content figure.align-center{text-align:center}.rst-content .section>a>img,.rst-content .section>img,.rst-content section>a>img,.rst-content section>img{margin-bottom:24px}.rst-content abbr[title]{text-decoration:none}.rst-content.style-external-links a.reference.external:after{font-family:FontAwesome;content:"\f08e";color:#b3b3b3;vertical-align:super;font-size:60%;margin:0 .2em}.rst-content blockquote{margin-left:24px;line-height:24px;margin-bottom:24px}.rst-content pre.literal-block{white-space:pre;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;display:block;overflow:auto}.rst-content div[class^=highlight],.rst-content pre.literal-block{border:1px solid #e1e4e5;overflow-x:auto;margin:1px 0 24px}.rst-content div[class^=highlight] div[class^=highlight],.rst-content pre.literal-block div[class^=highlight]{padding:0;border:none;margin:0}.rst-content div[class^=highlight] td.code{width:100%}.rst-content .linenodiv pre{border-right:1px solid #e6e9ea;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;user-select:none;pointer-events:none}.rst-content div[class^=highlight] pre{white-space:pre;margin:0;padding:12px;display:block;overflow:auto}.rst-content div[class^=highlight] pre .hll{display:block;margin:0 -12px;padding:0 12px}.rst-content .linenodiv pre,.rst-content div[class^=highlight] pre,.rst-content pre.literal-block{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:12px;line-height:1.4}.rst-content div.highlight .gp,.rst-content div.highlight span.linenos{user-select:none;pointer-events:none}.rst-content div.highlight span.linenos{display:inline-block;padding-left:0;padding-right:12px;margin-right:12px;border-right:1px solid #e6e9ea}.rst-content .code-block-caption{font-style:italic;font-size:85%;line-height:1;padding:1em 0;text-align:center}@media print{.rst-content .codeblock,.rst-content div[class^=highlight],.rst-content div[class^=highlight] pre{white-space:pre-wrap}}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning{clear:both}.rst-content .admonition-todo .last,.rst-content .admonition-todo>:last-child,.rst-content .admonition .last,.rst-content .admonition>:last-child,.rst-content .attention .last,.rst-content .attention>:last-child,.rst-content .caution .last,.rst-content .caution>:last-child,.rst-content .danger .last,.rst-content .danger>:last-child,.rst-content .error .last,.rst-content .error>:last-child,.rst-content .hint .last,.rst-content .hint>:last-child,.rst-content .important .last,.rst-content .important>:last-child,.rst-content .note .last,.rst-content .note>:last-child,.rst-content .seealso .last,.rst-content .seealso>:last-child,.rst-content .tip .last,.rst-content .tip>:last-child,.rst-content .warning .last,.rst-content .warning>:last-child{margin-bottom:0}.rst-content .admonition-title:before{margin-right:4px}.rst-content .admonition table{border-color:rgba(0,0,0,.1)}.rst-content .admonition table td,.rst-content .admonition table th{background:transparent!important;border-color:rgba(0,0,0,.1)!important}.rst-content .section ol.loweralpha,.rst-content .section ol.loweralpha>li,.rst-content .toctree-wrapper ol.loweralpha,.rst-content .toctree-wrapper ol.loweralpha>li,.rst-content section ol.loweralpha,.rst-content section ol.loweralpha>li{list-style:lower-alpha}.rst-content .section ol.upperalpha,.rst-content .section ol.upperalpha>li,.rst-content .toctree-wrapper ol.upperalpha,.rst-content .toctree-wrapper ol.upperalpha>li,.rst-content section ol.upperalpha,.rst-content section ol.upperalpha>li{list-style:upper-alpha}.rst-content .section ol li>*,.rst-content .section ul li>*,.rst-content .toctree-wrapper ol li>*,.rst-content .toctree-wrapper ul li>*,.rst-content section ol li>*,.rst-content section ul li>*{margin-top:12px;margin-bottom:12px}.rst-content .section ol li>:first-child,.rst-content .section ul li>:first-child,.rst-content .toctree-wrapper ol li>:first-child,.rst-content .toctree-wrapper ul li>:first-child,.rst-content section ol li>:first-child,.rst-content section ul li>:first-child{margin-top:0}.rst-content .section ol li>p,.rst-content .section ol li>p:last-child,.rst-content .section ul li>p,.rst-content .section ul li>p:last-child,.rst-content .toctree-wrapper ol li>p,.rst-content .toctree-wrapper ol li>p:last-child,.rst-content .toctree-wrapper ul li>p,.rst-content .toctree-wrapper ul li>p:last-child,.rst-content section ol li>p,.rst-content section ol li>p:last-child,.rst-content section ul li>p,.rst-content section ul li>p:last-child{margin-bottom:12px}.rst-content .section ol li>p:only-child,.rst-content .section ol li>p:only-child:last-child,.rst-content .section ul li>p:only-child,.rst-content .section ul li>p:only-child:last-child,.rst-content .toctree-wrapper ol li>p:only-child,.rst-content .toctree-wrapper ol li>p:only-child:last-child,.rst-content .toctree-wrapper ul li>p:only-child,.rst-content .toctree-wrapper ul li>p:only-child:last-child,.rst-content section ol li>p:only-child,.rst-content section ol li>p:only-child:last-child,.rst-content section ul li>p:only-child,.rst-content section ul li>p:only-child:last-child{margin-bottom:0}.rst-content .section ol li>ol,.rst-content .section ol li>ul,.rst-content .section ul li>ol,.rst-content .section ul li>ul,.rst-content .toctree-wrapper ol li>ol,.rst-content .toctree-wrapper ol li>ul,.rst-content .toctree-wrapper ul li>ol,.rst-content .toctree-wrapper ul li>ul,.rst-content section ol li>ol,.rst-content section ol li>ul,.rst-content section ul li>ol,.rst-content section ul li>ul{margin-bottom:12px}.rst-content .section ol.simple li>*,.rst-content .section ol.simple li ol,.rst-content .section ol.simple li ul,.rst-content .section ul.simple li>*,.rst-content .section ul.simple li ol,.rst-content .section ul.simple li ul,.rst-content .toctree-wrapper ol.simple li>*,.rst-content .toctree-wrapper ol.simple li ol,.rst-content .toctree-wrapper ol.simple li ul,.rst-content .toctree-wrapper ul.simple li>*,.rst-content .toctree-wrapper ul.simple li ol,.rst-content .toctree-wrapper ul.simple li ul,.rst-content section ol.simple li>*,.rst-content section ol.simple li ol,.rst-content section ol.simple li ul,.rst-content section ul.simple li>*,.rst-content section ul.simple li ol,.rst-content section ul.simple li ul{margin-top:0;margin-bottom:0}.rst-content .line-block{margin-left:0;margin-bottom:24px;line-height:24px}.rst-content .line-block .line-block{margin-left:24px;margin-bottom:0}.rst-content .topic-title{font-weight:700;margin-bottom:12px}.rst-content .toc-backref{color:#404040}.rst-content .align-right{float:right;margin:0 0 24px 24px}.rst-content .align-left{float:left;margin:0 24px 24px 0}.rst-content .align-center{margin:auto}.rst-content .align-center:not(table){display:block}.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink{opacity:0;font-size:14px;font-family:FontAwesome;margin-left:.5em}.rst-content .code-block-caption .headerlink:focus,.rst-content .code-block-caption:hover .headerlink,.rst-content .eqno .headerlink:focus,.rst-content .eqno:hover .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink:focus,.rst-content .toctree-wrapper>p.caption:hover .headerlink,.rst-content dl dt .headerlink:focus,.rst-content dl dt:hover .headerlink,.rst-content h1 .headerlink:focus,.rst-content h1:hover .headerlink,.rst-content h2 .headerlink:focus,.rst-content h2:hover .headerlink,.rst-content h3 .headerlink:focus,.rst-content h3:hover .headerlink,.rst-content h4 .headerlink:focus,.rst-content h4:hover .headerlink,.rst-content h5 .headerlink:focus,.rst-content h5:hover .headerlink,.rst-content h6 .headerlink:focus,.rst-content h6:hover .headerlink,.rst-content p.caption .headerlink:focus,.rst-content p.caption:hover .headerlink,.rst-content p .headerlink:focus,.rst-content p:hover .headerlink,.rst-content table>caption .headerlink:focus,.rst-content table>caption:hover .headerlink{opacity:1}.rst-content p a{overflow-wrap:anywhere}.rst-content .wy-table td p,.rst-content .wy-table td ul,.rst-content .wy-table th p,.rst-content .wy-table th ul,.rst-content table.docutils td p,.rst-content table.docutils td ul,.rst-content table.docutils th p,.rst-content table.docutils th ul,.rst-content table.field-list td p,.rst-content table.field-list td ul,.rst-content table.field-list th p,.rst-content table.field-list th ul{font-size:inherit}.rst-content .btn:focus{outline:2px solid}.rst-content table>caption .headerlink:after{font-size:12px}.rst-content .centered{text-align:center}.rst-content .sidebar{float:right;width:40%;display:block;margin:0 0 24px 24px;padding:24px;background:#f3f6f6;border:1px solid #e1e4e5}.rst-content .sidebar dl,.rst-content .sidebar p,.rst-content .sidebar ul{font-size:90%}.rst-content .sidebar .last,.rst-content .sidebar>:last-child{margin-bottom:0}.rst-content .sidebar .sidebar-title{display:block;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif;font-weight:700;background:#e1e4e5;padding:6px 12px;margin:-24px -24px 24px;font-size:100%}.rst-content .highlighted{background:#f1c40f;box-shadow:0 0 0 2px #f1c40f;display:inline;font-weight:700}.rst-content .citation-reference,.rst-content .footnote-reference{vertical-align:baseline;position:relative;top:-.4em;line-height:0;font-size:90%}.rst-content .hlist{width:100%}.rst-content dl dt span.classifier:before{content:" : "}.rst-content dl dt span.classifier-delimiter{display:none!important}html.writer-html4 .rst-content table.docutils.citation,html.writer-html4 .rst-content table.docutils.footnote{background:none;border:none}html.writer-html4 .rst-content table.docutils.citation td,html.writer-html4 .rst-content table.docutils.citation tr,html.writer-html4 .rst-content table.docutils.footnote td,html.writer-html4 .rst-content table.docutils.footnote tr{border:none;background-color:transparent!important;white-space:normal}html.writer-html4 .rst-content table.docutils.citation td.label,html.writer-html4 .rst-content table.docutils.footnote td.label{padding-left:0;padding-right:0;vertical-align:top}html.writer-html5 .rst-content dl.citation,html.writer-html5 .rst-content dl.field-list,html.writer-html5 .rst-content dl.footnote{display:grid;grid-template-columns:max-content auto}html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dt{padding-left:1rem}html.writer-html5 .rst-content dl.citation>dt:after,html.writer-html5 .rst-content dl.field-list>dt:after,html.writer-html5 .rst-content dl.footnote>dt:after{content:":"}html.writer-html5 .rst-content dl.citation>dd,html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.field-list>dd,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dd,html.writer-html5 .rst-content dl.footnote>dt{margin-bottom:0}html.writer-html5 .rst-content dl.citation,html.writer-html5 .rst-content dl.footnote{font-size:.9rem}html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.footnote>dt{margin:0 .5rem .5rem 0;line-height:1.2rem;word-break:break-all;font-weight:400}html.writer-html5 .rst-content dl.citation>dt>span.brackets,html.writer-html5 .rst-content dl.footnote>dt>span.brackets{margin-right:.5rem}html.writer-html5 .rst-content dl.citation>dt>span.brackets:before,html.writer-html5 .rst-content dl.footnote>dt>span.brackets:before{content:"["}html.writer-html5 .rst-content dl.citation>dt>span.brackets:after,html.writer-html5 .rst-content dl.footnote>dt>span.brackets:after{content:"]"}html.writer-html5 .rst-content dl.citation>dt>span.fn-backref,html.writer-html5 .rst-content dl.footnote>dt>span.fn-backref{font-style:italic}html.writer-html5 .rst-content dl.citation>dd,html.writer-html5 .rst-content dl.footnote>dd{margin:0 0 .5rem;line-height:1.2rem}html.writer-html5 .rst-content dl.citation>dd p,html.writer-html5 .rst-content dl.footnote>dd p,html.writer-html5 .rst-content dl.option-list kbd{font-size:.9rem}.rst-content dl.citation,.rst-content table.docutils.footnote,html.writer-html4 .rst-content table.docutils.citation,html.writer-html5 .rst-content dl.footnote{color:grey}.rst-content dl.citation code,.rst-content dl.citation tt,.rst-content table.docutils.footnote code,.rst-content table.docutils.footnote tt,html.writer-html4 .rst-content table.docutils.citation code,html.writer-html4 .rst-content table.docutils.citation tt,html.writer-html5 .rst-content dl.footnote code,html.writer-html5 .rst-content dl.footnote tt{color:#555}.rst-content .wy-table-responsive.citation,.rst-content .wy-table-responsive.footnote{margin-bottom:0}.rst-content .wy-table-responsive.citation+:not(.citation),.rst-content .wy-table-responsive.footnote+:not(.footnote){margin-top:24px}.rst-content .wy-table-responsive.citation:last-child,.rst-content .wy-table-responsive.footnote:last-child{margin-bottom:24px}.rst-content table.docutils th{border-color:#e1e4e5}html.writer-html5 .rst-content table.docutils th{border:1px solid #e1e4e5}html.writer-html5 .rst-content table.docutils td>p,html.writer-html5 .rst-content table.docutils th>p{line-height:1rem;margin-bottom:0;font-size:.9rem}.rst-content table.docutils td .last,.rst-content table.docutils td .last>:last-child{margin-bottom:0}.rst-content table.field-list,.rst-content table.field-list td{border:none}.rst-content table.field-list td p{line-height:inherit}.rst-content table.field-list td>strong{display:inline-block}.rst-content table.field-list .field-name{padding-right:10px;text-align:left;white-space:nowrap}.rst-content table.field-list .field-body{text-align:left}.rst-content code,.rst-content tt{color:#000;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;padding:2px 5px}.rst-content code big,.rst-content code em,.rst-content tt big,.rst-content tt em{font-size:100%!important;line-height:normal}.rst-content code.literal,.rst-content tt.literal{color:#e74c3c;white-space:normal}.rst-content code.xref,.rst-content tt.xref,a .rst-content code,a .rst-content tt{font-weight:700;color:#404040;overflow-wrap:normal}.rst-content kbd,.rst-content pre,.rst-content samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace}.rst-content a code,.rst-content a tt{color:#2980b9}.rst-content dl{margin-bottom:24px}.rst-content dl dt{font-weight:700;margin-bottom:12px}.rst-content dl ol,.rst-content dl p,.rst-content dl table,.rst-content dl ul{margin-bottom:12px}.rst-content dl dd{margin:0 0 12px 24px;line-height:24px}.rst-content dl dd>ol:last-child,.rst-content dl dd>p:last-child,.rst-content dl dd>table:last-child,.rst-content dl dd>ul:last-child{margin-bottom:0}html.writer-html4 .rst-content dl:not(.docutils),html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple){margin-bottom:24px}html.writer-html4 .rst-content dl:not(.docutils)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt{display:table;margin:6px 0;font-size:90%;line-height:normal;background:#e7f2fa;color:#2980b9;border-top:3px solid #6ab0de;padding:6px;position:relative}html.writer-html4 .rst-content dl:not(.docutils)>dt:before,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt:before{color:#6ab0de}html.writer-html4 .rst-content dl:not(.docutils)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt{margin-bottom:6px;border:none;border-left:3px solid #ccc;background:#f0f0f0;color:#555}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils)>dt:first-child,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt:first-child{margin-top:0}html.writer-html4 .rst-content dl:not(.docutils) code.descclassname,html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descclassname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descname{background-color:transparent;border:none;padding:0;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descname{font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .optional,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .optional{display:inline-block;padding:0 4px;color:#000;font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .property,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .property{display:inline-block;padding-right:8px;max-width:100%}html.writer-html4 .rst-content dl:not(.docutils) .k,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .k{font-style:italic}html.writer-html4 .rst-content dl:not(.docutils) .descclassname,html.writer-html4 .rst-content dl:not(.docutils) .descname,html.writer-html4 .rst-content dl:not(.docutils) .sig-name,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .sig-name{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#000}.rst-content .viewcode-back,.rst-content .viewcode-link{display:inline-block;color:#27ae60;font-size:80%;padding-left:24px}.rst-content .viewcode-back{display:block;float:right}.rst-content p.rubric{margin-bottom:12px;font-weight:700}.rst-content code.download,.rst-content tt.download{background:inherit;padding:inherit;font-weight:400;font-family:inherit;font-size:inherit;color:inherit;border:inherit;white-space:inherit}.rst-content code.download span:first-child,.rst-content tt.download span:first-child{-webkit-font-smoothing:subpixel-antialiased}.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{margin-right:4px}.rst-content .guilabel{border:1px solid #7fbbe3;background:#e7f2fa;font-size:80%;font-weight:700;border-radius:4px;padding:2.4px 6px;margin:auto 2px}.rst-content :not(dl.option-list)>:not(dt):not(kbd):not(.kbd)>.kbd,.rst-content :not(dl.option-list)>:not(dt):not(kbd):not(.kbd)>kbd{color:inherit;font-size:80%;background-color:#fff;border:1px solid #a6a6a6;border-radius:4px;box-shadow:0 2px grey;padding:2.4px 6px;margin:auto 0}.rst-content .versionmodified{font-style:italic}@media screen and (max-width:480px){.rst-content .sidebar{width:100%}}span[id*=MathJax-Span]{color:#404040}.math{text-align:center}@font-face{font-family:Lato;src:url(fonts/lato-normal.woff2?bd03a2cc277bbbc338d464e679fe9942) format("woff2"),url(fonts/lato-normal.woff?27bd77b9162d388cb8d4c4217c7c5e2a) format("woff");font-weight:400;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold.woff2?cccb897485813c7c256901dbca54ecf2) format("woff2"),url(fonts/lato-bold.woff?d878b6c29b10beca227e9eef4246111b) format("woff");font-weight:700;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold-italic.woff2?0b6bb6725576b072c5d0b02ecdd1900d) format("woff2"),url(fonts/lato-bold-italic.woff?9c7e4e9eb485b4a121c760e61bc3707c) format("woff");font-weight:700;font-style:italic;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-normal-italic.woff2?4eb103b4d12be57cb1d040ed5e162e9d) format("woff2"),url(fonts/lato-normal-italic.woff?f28f2d6482446544ef1ea1ccc6dd5892) format("woff");font-weight:400;font-style:italic;font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:400;src:url(fonts/Roboto-Slab-Regular.woff2?7abf5b8d04d26a2cafea937019bca958) format("woff2"),url(fonts/Roboto-Slab-Regular.woff?c1be9284088d487c5e3ff0a10a92e58c) format("woff");font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:700;src:url(fonts/Roboto-Slab-Bold.woff2?9984f4a9bda09be08e83f2506954adbe) format("woff2"),url(fonts/Roboto-Slab-Bold.woff?bed5564a116b05148e3b3bea6fb1162a) format("woff");font-display:block}
+ */@font-face{font-family:FontAwesome;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713);src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix&v=4.7.0) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#fontawesomeregular) format("svg");font-weight:400;font-style:normal}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{display:inline-block;font:normal normal normal 14px/1 FontAwesome;font-size:inherit;text-rendering:auto;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.fa-lg{font-size:1.33333em;line-height:.75em;vertical-align:-15%}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-fw{width:1.28571em;text-align:center}.fa-ul{padding-left:0;margin-left:2.14286em;list-style-type:none}.fa-ul>li{position:relative}.fa-li{position:absolute;left:-2.14286em;width:2.14286em;top:.14286em;text-align:center}.fa-li.fa-lg{left:-1.85714em}.fa-border{padding:.2em .25em .15em;border:.08em solid #eee;border-radius:.1em}.fa-pull-left{float:left}.fa-pull-right{float:right}.fa-pull-left.icon,.fa.fa-pull-left,.rst-content .code-block-caption .fa-pull-left.headerlink,.rst-content .eqno .fa-pull-left.headerlink,.rst-content .fa-pull-left.admonition-title,.rst-content code.download span.fa-pull-left:first-child,.rst-content dl dt .fa-pull-left.headerlink,.rst-content h1 .fa-pull-left.headerlink,.rst-content h2 .fa-pull-left.headerlink,.rst-content h3 .fa-pull-left.headerlink,.rst-content h4 .fa-pull-left.headerlink,.rst-content h5 .fa-pull-left.headerlink,.rst-content h6 .fa-pull-left.headerlink,.rst-content p .fa-pull-left.headerlink,.rst-content table>caption .fa-pull-left.headerlink,.rst-content tt.download span.fa-pull-left:first-child,.wy-menu-vertical li.current>a button.fa-pull-left.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-left.toctree-expand,.wy-menu-vertical li button.fa-pull-left.toctree-expand{margin-right:.3em}.fa-pull-right.icon,.fa.fa-pull-right,.rst-content .code-block-caption .fa-pull-right.headerlink,.rst-content .eqno .fa-pull-right.headerlink,.rst-content .fa-pull-right.admonition-title,.rst-content code.download span.fa-pull-right:first-child,.rst-content dl dt .fa-pull-right.headerlink,.rst-content h1 .fa-pull-right.headerlink,.rst-content h2 .fa-pull-right.headerlink,.rst-content h3 .fa-pull-right.headerlink,.rst-content h4 .fa-pull-right.headerlink,.rst-content h5 .fa-pull-right.headerlink,.rst-content h6 .fa-pull-right.headerlink,.rst-content p .fa-pull-right.headerlink,.rst-content table>caption .fa-pull-right.headerlink,.rst-content tt.download span.fa-pull-right:first-child,.wy-menu-vertical li.current>a button.fa-pull-right.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-right.toctree-expand,.wy-menu-vertical li button.fa-pull-right.toctree-expand{margin-left:.3em}.pull-right{float:right}.pull-left{float:left}.fa.pull-left,.pull-left.icon,.rst-content .code-block-caption .pull-left.headerlink,.rst-content .eqno .pull-left.headerlink,.rst-content .pull-left.admonition-title,.rst-content code.download span.pull-left:first-child,.rst-content dl dt .pull-left.headerlink,.rst-content h1 .pull-left.headerlink,.rst-content h2 .pull-left.headerlink,.rst-content h3 .pull-left.headerlink,.rst-content h4 .pull-left.headerlink,.rst-content h5 .pull-left.headerlink,.rst-content h6 .pull-left.headerlink,.rst-content p .pull-left.headerlink,.rst-content table>caption .pull-left.headerlink,.rst-content tt.download span.pull-left:first-child,.wy-menu-vertical li.current>a button.pull-left.toctree-expand,.wy-menu-vertical li.on a button.pull-left.toctree-expand,.wy-menu-vertical li button.pull-left.toctree-expand{margin-right:.3em}.fa.pull-right,.pull-right.icon,.rst-content .code-block-caption .pull-right.headerlink,.rst-content .eqno .pull-right.headerlink,.rst-content .pull-right.admonition-title,.rst-content code.download span.pull-right:first-child,.rst-content dl dt .pull-right.headerlink,.rst-content h1 .pull-right.headerlink,.rst-content h2 .pull-right.headerlink,.rst-content h3 .pull-right.headerlink,.rst-content h4 .pull-right.headerlink,.rst-content h5 .pull-right.headerlink,.rst-content h6 .pull-right.headerlink,.rst-content p .pull-right.headerlink,.rst-content table>caption .pull-right.headerlink,.rst-content tt.download span.pull-right:first-child,.wy-menu-vertical li.current>a button.pull-right.toctree-expand,.wy-menu-vertical li.on a button.pull-right.toctree-expand,.wy-menu-vertical li button.pull-right.toctree-expand{margin-left:.3em}.fa-spin{-webkit-animation:fa-spin 2s linear infinite;animation:fa-spin 2s linear infinite}.fa-pulse{-webkit-animation:fa-spin 1s steps(8) infinite;animation:fa-spin 1s steps(8) infinite}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}.fa-rotate-90{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";-webkit-transform:rotate(90deg);-ms-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";-webkit-transform:rotate(180deg);-ms-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";-webkit-transform:rotate(270deg);-ms-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";-webkit-transform:scaleY(-1);-ms-transform:scaleY(-1);transform:scaleY(-1)}:root .fa-flip-horizontal,:root .fa-flip-vertical,:root .fa-rotate-90,:root .fa-rotate-180,:root .fa-rotate-270{filter:none}.fa-stack{position:relative;display:inline-block;width:2em;height:2em;line-height:2em;vertical-align:middle}.fa-stack-1x,.fa-stack-2x{position:absolute;left:0;width:100%;text-align:center}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:#fff}.fa-glass:before{content:""}.fa-music:before{content:""}.fa-search:before,.icon-search:before{content:""}.fa-envelope-o:before{content:""}.fa-heart:before{content:""}.fa-star:before{content:""}.fa-star-o:before{content:""}.fa-user:before{content:""}.fa-film:before{content:""}.fa-th-large:before{content:""}.fa-th:before{content:""}.fa-th-list:before{content:""}.fa-check:before{content:""}.fa-close:before,.fa-remove:before,.fa-times:before{content:""}.fa-search-plus:before{content:""}.fa-search-minus:before{content:""}.fa-power-off:before{content:""}.fa-signal:before{content:""}.fa-cog:before,.fa-gear:before{content:""}.fa-trash-o:before{content:""}.fa-home:before,.icon-home:before{content:""}.fa-file-o:before{content:""}.fa-clock-o:before{content:""}.fa-road:before{content:""}.fa-download:before,.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{content:""}.fa-arrow-circle-o-down:before{content:""}.fa-arrow-circle-o-up:before{content:""}.fa-inbox:before{content:""}.fa-play-circle-o:before{content:""}.fa-repeat:before,.fa-rotate-right:before{content:""}.fa-refresh:before{content:""}.fa-list-alt:before{content:""}.fa-lock:before{content:""}.fa-flag:before{content:""}.fa-headphones:before{content:""}.fa-volume-off:before{content:""}.fa-volume-down:before{content:""}.fa-volume-up:before{content:""}.fa-qrcode:before{content:""}.fa-barcode:before{content:""}.fa-tag:before{content:""}.fa-tags:before{content:""}.fa-book:before,.icon-book:before{content:""}.fa-bookmark:before{content:""}.fa-print:before{content:""}.fa-camera:before{content:""}.fa-font:before{content:""}.fa-bold:before{content:""}.fa-italic:before{content:""}.fa-text-height:before{content:""}.fa-text-width:before{content:""}.fa-align-left:before{content:""}.fa-align-center:before{content:""}.fa-align-right:before{content:""}.fa-align-justify:before{content:""}.fa-list:before{content:""}.fa-dedent:before,.fa-outdent:before{content:""}.fa-indent:before{content:""}.fa-video-camera:before{content:""}.fa-image:before,.fa-photo:before,.fa-picture-o:before{content:""}.fa-pencil:before{content:""}.fa-map-marker:before{content:""}.fa-adjust:before{content:""}.fa-tint:before{content:""}.fa-edit:before,.fa-pencil-square-o:before{content:""}.fa-share-square-o:before{content:""}.fa-check-square-o:before{content:""}.fa-arrows:before{content:""}.fa-step-backward:before{content:""}.fa-fast-backward:before{content:""}.fa-backward:before{content:""}.fa-play:before{content:""}.fa-pause:before{content:""}.fa-stop:before{content:""}.fa-forward:before{content:""}.fa-fast-forward:before{content:""}.fa-step-forward:before{content:""}.fa-eject:before{content:""}.fa-chevron-left:before{content:""}.fa-chevron-right:before{content:""}.fa-plus-circle:before{content:""}.fa-minus-circle:before{content:""}.fa-times-circle:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before{content:""}.fa-check-circle:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before{content:""}.fa-question-circle:before{content:""}.fa-info-circle:before{content:""}.fa-crosshairs:before{content:""}.fa-times-circle-o:before{content:""}.fa-check-circle-o:before{content:""}.fa-ban:before{content:""}.fa-arrow-left:before{content:""}.fa-arrow-right:before{content:""}.fa-arrow-up:before{content:""}.fa-arrow-down:before{content:""}.fa-mail-forward:before,.fa-share:before{content:""}.fa-expand:before{content:""}.fa-compress:before{content:""}.fa-plus:before{content:""}.fa-minus:before{content:""}.fa-asterisk:before{content:""}.fa-exclamation-circle:before,.rst-content .admonition-title:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before{content:""}.fa-gift:before{content:""}.fa-leaf:before{content:""}.fa-fire:before,.icon-fire:before{content:""}.fa-eye:before{content:""}.fa-eye-slash:before{content:""}.fa-exclamation-triangle:before,.fa-warning:before{content:""}.fa-plane:before{content:""}.fa-calendar:before{content:""}.fa-random:before{content:""}.fa-comment:before{content:""}.fa-magnet:before{content:""}.fa-chevron-up:before{content:""}.fa-chevron-down:before{content:""}.fa-retweet:before{content:""}.fa-shopping-cart:before{content:""}.fa-folder:before{content:""}.fa-folder-open:before{content:""}.fa-arrows-v:before{content:""}.fa-arrows-h:before{content:""}.fa-bar-chart-o:before,.fa-bar-chart:before{content:""}.fa-twitter-square:before{content:""}.fa-facebook-square:before{content:""}.fa-camera-retro:before{content:""}.fa-key:before{content:""}.fa-cogs:before,.fa-gears:before{content:""}.fa-comments:before{content:""}.fa-thumbs-o-up:before{content:""}.fa-thumbs-o-down:before{content:""}.fa-star-half:before{content:""}.fa-heart-o:before{content:""}.fa-sign-out:before{content:""}.fa-linkedin-square:before{content:""}.fa-thumb-tack:before{content:""}.fa-external-link:before{content:""}.fa-sign-in:before{content:""}.fa-trophy:before{content:""}.fa-github-square:before{content:""}.fa-upload:before{content:""}.fa-lemon-o:before{content:""}.fa-phone:before{content:""}.fa-square-o:before{content:""}.fa-bookmark-o:before{content:""}.fa-phone-square:before{content:""}.fa-twitter:before{content:""}.fa-facebook-f:before,.fa-facebook:before{content:""}.fa-github:before,.icon-github:before{content:""}.fa-unlock:before{content:""}.fa-credit-card:before{content:""}.fa-feed:before,.fa-rss:before{content:""}.fa-hdd-o:before{content:""}.fa-bullhorn:before{content:""}.fa-bell:before{content:""}.fa-certificate:before{content:""}.fa-hand-o-right:before{content:""}.fa-hand-o-left:before{content:""}.fa-hand-o-up:before{content:""}.fa-hand-o-down:before{content:""}.fa-arrow-circle-left:before,.icon-circle-arrow-left:before{content:""}.fa-arrow-circle-right:before,.icon-circle-arrow-right:before{content:""}.fa-arrow-circle-up:before{content:""}.fa-arrow-circle-down:before{content:""}.fa-globe:before{content:""}.fa-wrench:before{content:""}.fa-tasks:before{content:""}.fa-filter:before{content:""}.fa-briefcase:before{content:""}.fa-arrows-alt:before{content:""}.fa-group:before,.fa-users:before{content:""}.fa-chain:before,.fa-link:before,.icon-link:before{content:""}.fa-cloud:before{content:""}.fa-flask:before{content:""}.fa-cut:before,.fa-scissors:before{content:""}.fa-copy:before,.fa-files-o:before{content:""}.fa-paperclip:before{content:""}.fa-floppy-o:before,.fa-save:before{content:""}.fa-square:before{content:""}.fa-bars:before,.fa-navicon:before,.fa-reorder:before{content:""}.fa-list-ul:before{content:""}.fa-list-ol:before{content:""}.fa-strikethrough:before{content:""}.fa-underline:before{content:""}.fa-table:before{content:""}.fa-magic:before{content:""}.fa-truck:before{content:""}.fa-pinterest:before{content:""}.fa-pinterest-square:before{content:""}.fa-google-plus-square:before{content:""}.fa-google-plus:before{content:""}.fa-money:before{content:""}.fa-caret-down:before,.icon-caret-down:before,.wy-dropdown .caret:before{content:""}.fa-caret-up:before{content:""}.fa-caret-left:before{content:""}.fa-caret-right:before{content:""}.fa-columns:before{content:""}.fa-sort:before,.fa-unsorted:before{content:""}.fa-sort-desc:before,.fa-sort-down:before{content:""}.fa-sort-asc:before,.fa-sort-up:before{content:""}.fa-envelope:before{content:""}.fa-linkedin:before{content:""}.fa-rotate-left:before,.fa-undo:before{content:""}.fa-gavel:before,.fa-legal:before{content:""}.fa-dashboard:before,.fa-tachometer:before{content:""}.fa-comment-o:before{content:""}.fa-comments-o:before{content:""}.fa-bolt:before,.fa-flash:before{content:""}.fa-sitemap:before{content:""}.fa-umbrella:before{content:""}.fa-clipboard:before,.fa-paste:before{content:""}.fa-lightbulb-o:before{content:""}.fa-exchange:before{content:""}.fa-cloud-download:before{content:""}.fa-cloud-upload:before{content:""}.fa-user-md:before{content:""}.fa-stethoscope:before{content:""}.fa-suitcase:before{content:""}.fa-bell-o:before{content:""}.fa-coffee:before{content:""}.fa-cutlery:before{content:""}.fa-file-text-o:before{content:""}.fa-building-o:before{content:""}.fa-hospital-o:before{content:""}.fa-ambulance:before{content:""}.fa-medkit:before{content:""}.fa-fighter-jet:before{content:""}.fa-beer:before{content:""}.fa-h-square:before{content:""}.fa-plus-square:before{content:""}.fa-angle-double-left:before{content:""}.fa-angle-double-right:before{content:""}.fa-angle-double-up:before{content:""}.fa-angle-double-down:before{content:""}.fa-angle-left:before{content:""}.fa-angle-right:before{content:""}.fa-angle-up:before{content:""}.fa-angle-down:before{content:""}.fa-desktop:before{content:""}.fa-laptop:before{content:""}.fa-tablet:before{content:""}.fa-mobile-phone:before,.fa-mobile:before{content:""}.fa-circle-o:before{content:""}.fa-quote-left:before{content:""}.fa-quote-right:before{content:""}.fa-spinner:before{content:""}.fa-circle:before{content:""}.fa-mail-reply:before,.fa-reply:before{content:""}.fa-github-alt:before{content:""}.fa-folder-o:before{content:""}.fa-folder-open-o:before{content:""}.fa-smile-o:before{content:""}.fa-frown-o:before{content:""}.fa-meh-o:before{content:""}.fa-gamepad:before{content:""}.fa-keyboard-o:before{content:""}.fa-flag-o:before{content:""}.fa-flag-checkered:before{content:""}.fa-terminal:before{content:""}.fa-code:before{content:""}.fa-mail-reply-all:before,.fa-reply-all:before{content:""}.fa-star-half-empty:before,.fa-star-half-full:before,.fa-star-half-o:before{content:""}.fa-location-arrow:before{content:""}.fa-crop:before{content:""}.fa-code-fork:before{content:""}.fa-chain-broken:before,.fa-unlink:before{content:""}.fa-question:before{content:""}.fa-info:before{content:""}.fa-exclamation:before{content:""}.fa-superscript:before{content:""}.fa-subscript:before{content:""}.fa-eraser:before{content:""}.fa-puzzle-piece:before{content:""}.fa-microphone:before{content:""}.fa-microphone-slash:before{content:""}.fa-shield:before{content:""}.fa-calendar-o:before{content:""}.fa-fire-extinguisher:before{content:""}.fa-rocket:before{content:""}.fa-maxcdn:before{content:""}.fa-chevron-circle-left:before{content:""}.fa-chevron-circle-right:before{content:""}.fa-chevron-circle-up:before{content:""}.fa-chevron-circle-down:before{content:""}.fa-html5:before{content:""}.fa-css3:before{content:""}.fa-anchor:before{content:""}.fa-unlock-alt:before{content:""}.fa-bullseye:before{content:""}.fa-ellipsis-h:before{content:""}.fa-ellipsis-v:before{content:""}.fa-rss-square:before{content:""}.fa-play-circle:before{content:""}.fa-ticket:before{content:""}.fa-minus-square:before{content:""}.fa-minus-square-o:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before{content:""}.fa-level-up:before{content:""}.fa-level-down:before{content:""}.fa-check-square:before{content:""}.fa-pencil-square:before{content:""}.fa-external-link-square:before{content:""}.fa-share-square:before{content:""}.fa-compass:before{content:""}.fa-caret-square-o-down:before,.fa-toggle-down:before{content:""}.fa-caret-square-o-up:before,.fa-toggle-up:before{content:""}.fa-caret-square-o-right:before,.fa-toggle-right:before{content:""}.fa-eur:before,.fa-euro:before{content:""}.fa-gbp:before{content:""}.fa-dollar:before,.fa-usd:before{content:""}.fa-inr:before,.fa-rupee:before{content:""}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen:before{content:""}.fa-rouble:before,.fa-rub:before,.fa-ruble:before{content:""}.fa-krw:before,.fa-won:before{content:""}.fa-bitcoin:before,.fa-btc:before{content:""}.fa-file:before{content:""}.fa-file-text:before{content:""}.fa-sort-alpha-asc:before{content:""}.fa-sort-alpha-desc:before{content:""}.fa-sort-amount-asc:before{content:""}.fa-sort-amount-desc:before{content:""}.fa-sort-numeric-asc:before{content:""}.fa-sort-numeric-desc:before{content:""}.fa-thumbs-up:before{content:""}.fa-thumbs-down:before{content:""}.fa-youtube-square:before{content:""}.fa-youtube:before{content:""}.fa-xing:before{content:""}.fa-xing-square:before{content:""}.fa-youtube-play:before{content:""}.fa-dropbox:before{content:""}.fa-stack-overflow:before{content:""}.fa-instagram:before{content:""}.fa-flickr:before{content:""}.fa-adn:before{content:""}.fa-bitbucket:before,.icon-bitbucket:before{content:""}.fa-bitbucket-square:before{content:""}.fa-tumblr:before{content:""}.fa-tumblr-square:before{content:""}.fa-long-arrow-down:before{content:""}.fa-long-arrow-up:before{content:""}.fa-long-arrow-left:before{content:""}.fa-long-arrow-right:before{content:""}.fa-apple:before{content:""}.fa-windows:before{content:""}.fa-android:before{content:""}.fa-linux:before{content:""}.fa-dribbble:before{content:""}.fa-skype:before{content:""}.fa-foursquare:before{content:""}.fa-trello:before{content:""}.fa-female:before{content:""}.fa-male:before{content:""}.fa-gittip:before,.fa-gratipay:before{content:""}.fa-sun-o:before{content:""}.fa-moon-o:before{content:""}.fa-archive:before{content:""}.fa-bug:before{content:""}.fa-vk:before{content:""}.fa-weibo:before{content:""}.fa-renren:before{content:""}.fa-pagelines:before{content:""}.fa-stack-exchange:before{content:""}.fa-arrow-circle-o-right:before{content:""}.fa-arrow-circle-o-left:before{content:""}.fa-caret-square-o-left:before,.fa-toggle-left:before{content:""}.fa-dot-circle-o:before{content:""}.fa-wheelchair:before{content:""}.fa-vimeo-square:before{content:""}.fa-try:before,.fa-turkish-lira:before{content:""}.fa-plus-square-o:before,.wy-menu-vertical li button.toctree-expand:before{content:""}.fa-space-shuttle:before{content:""}.fa-slack:before{content:""}.fa-envelope-square:before{content:""}.fa-wordpress:before{content:""}.fa-openid:before{content:""}.fa-bank:before,.fa-institution:before,.fa-university:before{content:""}.fa-graduation-cap:before,.fa-mortar-board:before{content:""}.fa-yahoo:before{content:""}.fa-google:before{content:""}.fa-reddit:before{content:""}.fa-reddit-square:before{content:""}.fa-stumbleupon-circle:before{content:""}.fa-stumbleupon:before{content:""}.fa-delicious:before{content:""}.fa-digg:before{content:""}.fa-pied-piper-pp:before{content:""}.fa-pied-piper-alt:before{content:""}.fa-drupal:before{content:""}.fa-joomla:before{content:""}.fa-language:before{content:""}.fa-fax:before{content:""}.fa-building:before{content:""}.fa-child:before{content:""}.fa-paw:before{content:""}.fa-spoon:before{content:""}.fa-cube:before{content:""}.fa-cubes:before{content:""}.fa-behance:before{content:""}.fa-behance-square:before{content:""}.fa-steam:before{content:""}.fa-steam-square:before{content:""}.fa-recycle:before{content:""}.fa-automobile:before,.fa-car:before{content:""}.fa-cab:before,.fa-taxi:before{content:""}.fa-tree:before{content:""}.fa-spotify:before{content:""}.fa-deviantart:before{content:""}.fa-soundcloud:before{content:""}.fa-database:before{content:""}.fa-file-pdf-o:before{content:""}.fa-file-word-o:before{content:""}.fa-file-excel-o:before{content:""}.fa-file-powerpoint-o:before{content:""}.fa-file-image-o:before,.fa-file-photo-o:before,.fa-file-picture-o:before{content:""}.fa-file-archive-o:before,.fa-file-zip-o:before{content:""}.fa-file-audio-o:before,.fa-file-sound-o:before{content:""}.fa-file-movie-o:before,.fa-file-video-o:before{content:""}.fa-file-code-o:before{content:""}.fa-vine:before{content:""}.fa-codepen:before{content:""}.fa-jsfiddle:before{content:""}.fa-life-bouy:before,.fa-life-buoy:before,.fa-life-ring:before,.fa-life-saver:before,.fa-support:before{content:""}.fa-circle-o-notch:before{content:""}.fa-ra:before,.fa-rebel:before,.fa-resistance:before{content:""}.fa-empire:before,.fa-ge:before{content:""}.fa-git-square:before{content:""}.fa-git:before{content:""}.fa-hacker-news:before,.fa-y-combinator-square:before,.fa-yc-square:before{content:""}.fa-tencent-weibo:before{content:""}.fa-qq:before{content:""}.fa-wechat:before,.fa-weixin:before{content:""}.fa-paper-plane:before,.fa-send:before{content:""}.fa-paper-plane-o:before,.fa-send-o:before{content:""}.fa-history:before{content:""}.fa-circle-thin:before{content:""}.fa-header:before{content:""}.fa-paragraph:before{content:""}.fa-sliders:before{content:""}.fa-share-alt:before{content:""}.fa-share-alt-square:before{content:""}.fa-bomb:before{content:""}.fa-futbol-o:before,.fa-soccer-ball-o:before{content:""}.fa-tty:before{content:""}.fa-binoculars:before{content:""}.fa-plug:before{content:""}.fa-slideshare:before{content:""}.fa-twitch:before{content:""}.fa-yelp:before{content:""}.fa-newspaper-o:before{content:""}.fa-wifi:before{content:""}.fa-calculator:before{content:""}.fa-paypal:before{content:""}.fa-google-wallet:before{content:""}.fa-cc-visa:before{content:""}.fa-cc-mastercard:before{content:""}.fa-cc-discover:before{content:""}.fa-cc-amex:before{content:""}.fa-cc-paypal:before{content:""}.fa-cc-stripe:before{content:""}.fa-bell-slash:before{content:""}.fa-bell-slash-o:before{content:""}.fa-trash:before{content:""}.fa-copyright:before{content:""}.fa-at:before{content:""}.fa-eyedropper:before{content:""}.fa-paint-brush:before{content:""}.fa-birthday-cake:before{content:""}.fa-area-chart:before{content:""}.fa-pie-chart:before{content:""}.fa-line-chart:before{content:""}.fa-lastfm:before{content:""}.fa-lastfm-square:before{content:""}.fa-toggle-off:before{content:""}.fa-toggle-on:before{content:""}.fa-bicycle:before{content:""}.fa-bus:before{content:""}.fa-ioxhost:before{content:""}.fa-angellist:before{content:""}.fa-cc:before{content:""}.fa-ils:before,.fa-shekel:before,.fa-sheqel:before{content:""}.fa-meanpath:before{content:""}.fa-buysellads:before{content:""}.fa-connectdevelop:before{content:""}.fa-dashcube:before{content:""}.fa-forumbee:before{content:""}.fa-leanpub:before{content:""}.fa-sellsy:before{content:""}.fa-shirtsinbulk:before{content:""}.fa-simplybuilt:before{content:""}.fa-skyatlas:before{content:""}.fa-cart-plus:before{content:""}.fa-cart-arrow-down:before{content:""}.fa-diamond:before{content:""}.fa-ship:before{content:""}.fa-user-secret:before{content:""}.fa-motorcycle:before{content:""}.fa-street-view:before{content:""}.fa-heartbeat:before{content:""}.fa-venus:before{content:""}.fa-mars:before{content:""}.fa-mercury:before{content:""}.fa-intersex:before,.fa-transgender:before{content:""}.fa-transgender-alt:before{content:""}.fa-venus-double:before{content:""}.fa-mars-double:before{content:""}.fa-venus-mars:before{content:""}.fa-mars-stroke:before{content:""}.fa-mars-stroke-v:before{content:""}.fa-mars-stroke-h:before{content:""}.fa-neuter:before{content:""}.fa-genderless:before{content:""}.fa-facebook-official:before{content:""}.fa-pinterest-p:before{content:""}.fa-whatsapp:before{content:""}.fa-server:before{content:""}.fa-user-plus:before{content:""}.fa-user-times:before{content:""}.fa-bed:before,.fa-hotel:before{content:""}.fa-viacoin:before{content:""}.fa-train:before{content:""}.fa-subway:before{content:""}.fa-medium:before{content:""}.fa-y-combinator:before,.fa-yc:before{content:""}.fa-optin-monster:before{content:""}.fa-opencart:before{content:""}.fa-expeditedssl:before{content:""}.fa-battery-4:before,.fa-battery-full:before,.fa-battery:before{content:""}.fa-battery-3:before,.fa-battery-three-quarters:before{content:""}.fa-battery-2:before,.fa-battery-half:before{content:""}.fa-battery-1:before,.fa-battery-quarter:before{content:""}.fa-battery-0:before,.fa-battery-empty:before{content:""}.fa-mouse-pointer:before{content:""}.fa-i-cursor:before{content:""}.fa-object-group:before{content:""}.fa-object-ungroup:before{content:""}.fa-sticky-note:before{content:""}.fa-sticky-note-o:before{content:""}.fa-cc-jcb:before{content:""}.fa-cc-diners-club:before{content:""}.fa-clone:before{content:""}.fa-balance-scale:before{content:""}.fa-hourglass-o:before{content:""}.fa-hourglass-1:before,.fa-hourglass-start:before{content:""}.fa-hourglass-2:before,.fa-hourglass-half:before{content:""}.fa-hourglass-3:before,.fa-hourglass-end:before{content:""}.fa-hourglass:before{content:""}.fa-hand-grab-o:before,.fa-hand-rock-o:before{content:""}.fa-hand-paper-o:before,.fa-hand-stop-o:before{content:""}.fa-hand-scissors-o:before{content:""}.fa-hand-lizard-o:before{content:""}.fa-hand-spock-o:before{content:""}.fa-hand-pointer-o:before{content:""}.fa-hand-peace-o:before{content:""}.fa-trademark:before{content:""}.fa-registered:before{content:""}.fa-creative-commons:before{content:""}.fa-gg:before{content:""}.fa-gg-circle:before{content:""}.fa-tripadvisor:before{content:""}.fa-odnoklassniki:before{content:""}.fa-odnoklassniki-square:before{content:""}.fa-get-pocket:before{content:""}.fa-wikipedia-w:before{content:""}.fa-safari:before{content:""}.fa-chrome:before{content:""}.fa-firefox:before{content:""}.fa-opera:before{content:""}.fa-internet-explorer:before{content:""}.fa-television:before,.fa-tv:before{content:""}.fa-contao:before{content:""}.fa-500px:before{content:""}.fa-amazon:before{content:""}.fa-calendar-plus-o:before{content:""}.fa-calendar-minus-o:before{content:""}.fa-calendar-times-o:before{content:""}.fa-calendar-check-o:before{content:""}.fa-industry:before{content:""}.fa-map-pin:before{content:""}.fa-map-signs:before{content:""}.fa-map-o:before{content:""}.fa-map:before{content:""}.fa-commenting:before{content:""}.fa-commenting-o:before{content:""}.fa-houzz:before{content:""}.fa-vimeo:before{content:""}.fa-black-tie:before{content:""}.fa-fonticons:before{content:""}.fa-reddit-alien:before{content:""}.fa-edge:before{content:""}.fa-credit-card-alt:before{content:""}.fa-codiepie:before{content:""}.fa-modx:before{content:""}.fa-fort-awesome:before{content:""}.fa-usb:before{content:""}.fa-product-hunt:before{content:""}.fa-mixcloud:before{content:""}.fa-scribd:before{content:""}.fa-pause-circle:before{content:""}.fa-pause-circle-o:before{content:""}.fa-stop-circle:before{content:""}.fa-stop-circle-o:before{content:""}.fa-shopping-bag:before{content:""}.fa-shopping-basket:before{content:""}.fa-hashtag:before{content:""}.fa-bluetooth:before{content:""}.fa-bluetooth-b:before{content:""}.fa-percent:before{content:""}.fa-gitlab:before,.icon-gitlab:before{content:""}.fa-wpbeginner:before{content:""}.fa-wpforms:before{content:""}.fa-envira:before{content:""}.fa-universal-access:before{content:""}.fa-wheelchair-alt:before{content:""}.fa-question-circle-o:before{content:""}.fa-blind:before{content:""}.fa-audio-description:before{content:""}.fa-volume-control-phone:before{content:""}.fa-braille:before{content:""}.fa-assistive-listening-systems:before{content:""}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before{content:""}.fa-deaf:before,.fa-deafness:before,.fa-hard-of-hearing:before{content:""}.fa-glide:before{content:""}.fa-glide-g:before{content:""}.fa-sign-language:before,.fa-signing:before{content:""}.fa-low-vision:before{content:""}.fa-viadeo:before{content:""}.fa-viadeo-square:before{content:""}.fa-snapchat:before{content:""}.fa-snapchat-ghost:before{content:""}.fa-snapchat-square:before{content:""}.fa-pied-piper:before{content:""}.fa-first-order:before{content:""}.fa-yoast:before{content:""}.fa-themeisle:before{content:""}.fa-google-plus-circle:before,.fa-google-plus-official:before{content:""}.fa-fa:before,.fa-font-awesome:before{content:""}.fa-handshake-o:before{content:""}.fa-envelope-open:before{content:""}.fa-envelope-open-o:before{content:""}.fa-linode:before{content:""}.fa-address-book:before{content:""}.fa-address-book-o:before{content:""}.fa-address-card:before,.fa-vcard:before{content:""}.fa-address-card-o:before,.fa-vcard-o:before{content:""}.fa-user-circle:before{content:""}.fa-user-circle-o:before{content:""}.fa-user-o:before{content:""}.fa-id-badge:before{content:""}.fa-drivers-license:before,.fa-id-card:before{content:""}.fa-drivers-license-o:before,.fa-id-card-o:before{content:""}.fa-quora:before{content:""}.fa-free-code-camp:before{content:""}.fa-telegram:before{content:""}.fa-thermometer-4:before,.fa-thermometer-full:before,.fa-thermometer:before{content:""}.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:""}.fa-thermometer-2:before,.fa-thermometer-half:before{content:""}.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:""}.fa-thermometer-0:before,.fa-thermometer-empty:before{content:""}.fa-shower:before{content:""}.fa-bath:before,.fa-bathtub:before,.fa-s15:before{content:""}.fa-podcast:before{content:""}.fa-window-maximize:before{content:""}.fa-window-minimize:before{content:""}.fa-window-restore:before{content:""}.fa-times-rectangle:before,.fa-window-close:before{content:""}.fa-times-rectangle-o:before,.fa-window-close-o:before{content:""}.fa-bandcamp:before{content:""}.fa-grav:before{content:""}.fa-etsy:before{content:""}.fa-imdb:before{content:""}.fa-ravelry:before{content:""}.fa-eercast:before{content:""}.fa-microchip:before{content:""}.fa-snowflake-o:before{content:""}.fa-superpowers:before{content:""}.fa-wpexplorer:before{content:""}.fa-meetup:before{content:""}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-dropdown .caret,.wy-inline-validate.wy-inline-validate-danger .wy-input-context,.wy-inline-validate.wy-inline-validate-info .wy-input-context,.wy-inline-validate.wy-inline-validate-success .wy-input-context,.wy-inline-validate.wy-inline-validate-warning .wy-input-context,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{font-family:inherit}.fa:before,.icon:before,.rst-content .admonition-title:before,.rst-content .code-block-caption .headerlink:before,.rst-content .eqno .headerlink:before,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before{font-family:FontAwesome;display:inline-block;font-style:normal;font-weight:400;line-height:1;text-decoration:inherit}.rst-content .code-block-caption a .headerlink,.rst-content .eqno a .headerlink,.rst-content a .admonition-title,.rst-content code.download a span:first-child,.rst-content dl dt a .headerlink,.rst-content h1 a .headerlink,.rst-content h2 a .headerlink,.rst-content h3 a .headerlink,.rst-content h4 a .headerlink,.rst-content h5 a .headerlink,.rst-content h6 a .headerlink,.rst-content p.caption a .headerlink,.rst-content p a .headerlink,.rst-content table>caption a .headerlink,.rst-content tt.download a span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li a button.toctree-expand,a .fa,a .icon,a .rst-content .admonition-title,a .rst-content .code-block-caption .headerlink,a .rst-content .eqno .headerlink,a .rst-content code.download span:first-child,a .rst-content dl dt .headerlink,a .rst-content h1 .headerlink,a .rst-content h2 .headerlink,a .rst-content h3 .headerlink,a .rst-content h4 .headerlink,a .rst-content h5 .headerlink,a .rst-content h6 .headerlink,a .rst-content p.caption .headerlink,a .rst-content p .headerlink,a .rst-content table>caption .headerlink,a .rst-content tt.download span:first-child,a .wy-menu-vertical li button.toctree-expand{display:inline-block;text-decoration:inherit}.btn .fa,.btn .icon,.btn .rst-content .admonition-title,.btn .rst-content .code-block-caption .headerlink,.btn .rst-content .eqno .headerlink,.btn .rst-content code.download span:first-child,.btn .rst-content dl dt .headerlink,.btn .rst-content h1 .headerlink,.btn .rst-content h2 .headerlink,.btn .rst-content h3 .headerlink,.btn .rst-content h4 .headerlink,.btn .rst-content h5 .headerlink,.btn .rst-content h6 .headerlink,.btn .rst-content p .headerlink,.btn .rst-content table>caption .headerlink,.btn .rst-content tt.download span:first-child,.btn .wy-menu-vertical li.current>a button.toctree-expand,.btn .wy-menu-vertical li.on a button.toctree-expand,.btn .wy-menu-vertical li button.toctree-expand,.nav .fa,.nav .icon,.nav .rst-content .admonition-title,.nav .rst-content .code-block-caption .headerlink,.nav .rst-content .eqno .headerlink,.nav .rst-content code.download span:first-child,.nav .rst-content dl dt .headerlink,.nav .rst-content h1 .headerlink,.nav .rst-content h2 .headerlink,.nav .rst-content h3 .headerlink,.nav .rst-content h4 .headerlink,.nav .rst-content h5 .headerlink,.nav .rst-content h6 .headerlink,.nav .rst-content p .headerlink,.nav .rst-content table>caption .headerlink,.nav .rst-content tt.download span:first-child,.nav .wy-menu-vertical li.current>a button.toctree-expand,.nav .wy-menu-vertical li.on a button.toctree-expand,.nav .wy-menu-vertical li button.toctree-expand,.rst-content .btn .admonition-title,.rst-content .code-block-caption .btn .headerlink,.rst-content .code-block-caption .nav .headerlink,.rst-content .eqno .btn .headerlink,.rst-content .eqno .nav .headerlink,.rst-content .nav .admonition-title,.rst-content code.download .btn span:first-child,.rst-content code.download .nav span:first-child,.rst-content dl dt .btn .headerlink,.rst-content dl dt .nav .headerlink,.rst-content h1 .btn .headerlink,.rst-content h1 .nav .headerlink,.rst-content h2 .btn .headerlink,.rst-content h2 .nav .headerlink,.rst-content h3 .btn .headerlink,.rst-content h3 .nav .headerlink,.rst-content h4 .btn .headerlink,.rst-content h4 .nav .headerlink,.rst-content h5 .btn .headerlink,.rst-content h5 .nav .headerlink,.rst-content h6 .btn .headerlink,.rst-content h6 .nav .headerlink,.rst-content p .btn .headerlink,.rst-content p .nav .headerlink,.rst-content table>caption .btn .headerlink,.rst-content table>caption .nav .headerlink,.rst-content tt.download .btn span:first-child,.rst-content tt.download .nav span:first-child,.wy-menu-vertical li .btn button.toctree-expand,.wy-menu-vertical li.current>a .btn button.toctree-expand,.wy-menu-vertical li.current>a .nav button.toctree-expand,.wy-menu-vertical li .nav button.toctree-expand,.wy-menu-vertical li.on a .btn button.toctree-expand,.wy-menu-vertical li.on a .nav button.toctree-expand{display:inline}.btn .fa-large.icon,.btn .fa.fa-large,.btn .rst-content .code-block-caption .fa-large.headerlink,.btn .rst-content .eqno .fa-large.headerlink,.btn .rst-content .fa-large.admonition-title,.btn .rst-content code.download span.fa-large:first-child,.btn .rst-content dl dt .fa-large.headerlink,.btn .rst-content h1 .fa-large.headerlink,.btn .rst-content h2 .fa-large.headerlink,.btn .rst-content h3 .fa-large.headerlink,.btn .rst-content h4 .fa-large.headerlink,.btn .rst-content h5 .fa-large.headerlink,.btn .rst-content h6 .fa-large.headerlink,.btn .rst-content p .fa-large.headerlink,.btn .rst-content table>caption .fa-large.headerlink,.btn .rst-content tt.download span.fa-large:first-child,.btn .wy-menu-vertical li button.fa-large.toctree-expand,.nav .fa-large.icon,.nav .fa.fa-large,.nav .rst-content .code-block-caption .fa-large.headerlink,.nav .rst-content .eqno .fa-large.headerlink,.nav .rst-content .fa-large.admonition-title,.nav .rst-content code.download span.fa-large:first-child,.nav .rst-content dl dt .fa-large.headerlink,.nav .rst-content h1 .fa-large.headerlink,.nav .rst-content h2 .fa-large.headerlink,.nav .rst-content h3 .fa-large.headerlink,.nav .rst-content h4 .fa-large.headerlink,.nav .rst-content h5 .fa-large.headerlink,.nav .rst-content h6 .fa-large.headerlink,.nav .rst-content p .fa-large.headerlink,.nav .rst-content table>caption .fa-large.headerlink,.nav .rst-content tt.download span.fa-large:first-child,.nav .wy-menu-vertical li button.fa-large.toctree-expand,.rst-content .btn .fa-large.admonition-title,.rst-content .code-block-caption .btn .fa-large.headerlink,.rst-content .code-block-caption .nav .fa-large.headerlink,.rst-content .eqno .btn .fa-large.headerlink,.rst-content .eqno .nav .fa-large.headerlink,.rst-content .nav .fa-large.admonition-title,.rst-content code.download .btn span.fa-large:first-child,.rst-content code.download .nav span.fa-large:first-child,.rst-content dl dt .btn .fa-large.headerlink,.rst-content dl dt .nav .fa-large.headerlink,.rst-content h1 .btn .fa-large.headerlink,.rst-content h1 .nav .fa-large.headerlink,.rst-content h2 .btn .fa-large.headerlink,.rst-content h2 .nav .fa-large.headerlink,.rst-content h3 .btn .fa-large.headerlink,.rst-content h3 .nav .fa-large.headerlink,.rst-content h4 .btn .fa-large.headerlink,.rst-content h4 .nav .fa-large.headerlink,.rst-content h5 .btn .fa-large.headerlink,.rst-content h5 .nav .fa-large.headerlink,.rst-content h6 .btn .fa-large.headerlink,.rst-content h6 .nav .fa-large.headerlink,.rst-content p .btn .fa-large.headerlink,.rst-content p .nav .fa-large.headerlink,.rst-content table>caption .btn .fa-large.headerlink,.rst-content table>caption .nav .fa-large.headerlink,.rst-content tt.download .btn span.fa-large:first-child,.rst-content tt.download .nav span.fa-large:first-child,.wy-menu-vertical li .btn button.fa-large.toctree-expand,.wy-menu-vertical li .nav button.fa-large.toctree-expand{line-height:.9em}.btn .fa-spin.icon,.btn .fa.fa-spin,.btn .rst-content .code-block-caption .fa-spin.headerlink,.btn .rst-content .eqno .fa-spin.headerlink,.btn .rst-content .fa-spin.admonition-title,.btn .rst-content code.download span.fa-spin:first-child,.btn .rst-content dl dt .fa-spin.headerlink,.btn .rst-content h1 .fa-spin.headerlink,.btn .rst-content h2 .fa-spin.headerlink,.btn .rst-content h3 .fa-spin.headerlink,.btn .rst-content h4 .fa-spin.headerlink,.btn .rst-content h5 .fa-spin.headerlink,.btn .rst-content h6 .fa-spin.headerlink,.btn .rst-content p .fa-spin.headerlink,.btn .rst-content table>caption .fa-spin.headerlink,.btn .rst-content tt.download span.fa-spin:first-child,.btn .wy-menu-vertical li button.fa-spin.toctree-expand,.nav .fa-spin.icon,.nav .fa.fa-spin,.nav .rst-content .code-block-caption .fa-spin.headerlink,.nav .rst-content .eqno .fa-spin.headerlink,.nav .rst-content .fa-spin.admonition-title,.nav .rst-content code.download span.fa-spin:first-child,.nav .rst-content dl dt .fa-spin.headerlink,.nav .rst-content h1 .fa-spin.headerlink,.nav .rst-content h2 .fa-spin.headerlink,.nav .rst-content h3 .fa-spin.headerlink,.nav .rst-content h4 .fa-spin.headerlink,.nav .rst-content h5 .fa-spin.headerlink,.nav .rst-content h6 .fa-spin.headerlink,.nav .rst-content p .fa-spin.headerlink,.nav .rst-content table>caption .fa-spin.headerlink,.nav .rst-content tt.download span.fa-spin:first-child,.nav .wy-menu-vertical li button.fa-spin.toctree-expand,.rst-content .btn .fa-spin.admonition-title,.rst-content .code-block-caption .btn .fa-spin.headerlink,.rst-content .code-block-caption .nav .fa-spin.headerlink,.rst-content .eqno .btn .fa-spin.headerlink,.rst-content .eqno .nav .fa-spin.headerlink,.rst-content .nav .fa-spin.admonition-title,.rst-content code.download .btn span.fa-spin:first-child,.rst-content code.download .nav span.fa-spin:first-child,.rst-content dl dt .btn .fa-spin.headerlink,.rst-content dl dt .nav .fa-spin.headerlink,.rst-content h1 .btn .fa-spin.headerlink,.rst-content h1 .nav .fa-spin.headerlink,.rst-content h2 .btn .fa-spin.headerlink,.rst-content h2 .nav .fa-spin.headerlink,.rst-content h3 .btn .fa-spin.headerlink,.rst-content h3 .nav .fa-spin.headerlink,.rst-content h4 .btn .fa-spin.headerlink,.rst-content h4 .nav .fa-spin.headerlink,.rst-content h5 .btn .fa-spin.headerlink,.rst-content h5 .nav .fa-spin.headerlink,.rst-content h6 .btn .fa-spin.headerlink,.rst-content h6 .nav .fa-spin.headerlink,.rst-content p .btn .fa-spin.headerlink,.rst-content p .nav .fa-spin.headerlink,.rst-content table>caption .btn .fa-spin.headerlink,.rst-content table>caption .nav .fa-spin.headerlink,.rst-content tt.download .btn span.fa-spin:first-child,.rst-content tt.download .nav span.fa-spin:first-child,.wy-menu-vertical li .btn button.fa-spin.toctree-expand,.wy-menu-vertical li .nav button.fa-spin.toctree-expand{display:inline-block}.btn.fa:before,.btn.icon:before,.rst-content .btn.admonition-title:before,.rst-content .code-block-caption .btn.headerlink:before,.rst-content .eqno .btn.headerlink:before,.rst-content code.download span.btn:first-child:before,.rst-content dl dt .btn.headerlink:before,.rst-content h1 .btn.headerlink:before,.rst-content h2 .btn.headerlink:before,.rst-content h3 .btn.headerlink:before,.rst-content h4 .btn.headerlink:before,.rst-content h5 .btn.headerlink:before,.rst-content h6 .btn.headerlink:before,.rst-content p .btn.headerlink:before,.rst-content table>caption .btn.headerlink:before,.rst-content tt.download span.btn:first-child:before,.wy-menu-vertical li button.btn.toctree-expand:before{opacity:.5;-webkit-transition:opacity .05s ease-in;-moz-transition:opacity .05s ease-in;transition:opacity .05s ease-in}.btn.fa:hover:before,.btn.icon:hover:before,.rst-content .btn.admonition-title:hover:before,.rst-content .code-block-caption .btn.headerlink:hover:before,.rst-content .eqno .btn.headerlink:hover:before,.rst-content code.download span.btn:first-child:hover:before,.rst-content dl dt .btn.headerlink:hover:before,.rst-content h1 .btn.headerlink:hover:before,.rst-content h2 .btn.headerlink:hover:before,.rst-content h3 .btn.headerlink:hover:before,.rst-content h4 .btn.headerlink:hover:before,.rst-content h5 .btn.headerlink:hover:before,.rst-content h6 .btn.headerlink:hover:before,.rst-content p .btn.headerlink:hover:before,.rst-content table>caption .btn.headerlink:hover:before,.rst-content tt.download span.btn:first-child:hover:before,.wy-menu-vertical li button.btn.toctree-expand:hover:before{opacity:1}.btn-mini .fa:before,.btn-mini .icon:before,.btn-mini .rst-content .admonition-title:before,.btn-mini .rst-content .code-block-caption .headerlink:before,.btn-mini .rst-content .eqno .headerlink:before,.btn-mini .rst-content code.download span:first-child:before,.btn-mini .rst-content dl dt .headerlink:before,.btn-mini .rst-content h1 .headerlink:before,.btn-mini .rst-content h2 .headerlink:before,.btn-mini .rst-content h3 .headerlink:before,.btn-mini .rst-content h4 .headerlink:before,.btn-mini .rst-content h5 .headerlink:before,.btn-mini .rst-content h6 .headerlink:before,.btn-mini .rst-content p .headerlink:before,.btn-mini .rst-content table>caption .headerlink:before,.btn-mini .rst-content tt.download span:first-child:before,.btn-mini .wy-menu-vertical li button.toctree-expand:before,.rst-content .btn-mini .admonition-title:before,.rst-content .code-block-caption .btn-mini .headerlink:before,.rst-content .eqno .btn-mini .headerlink:before,.rst-content code.download .btn-mini span:first-child:before,.rst-content dl dt .btn-mini .headerlink:before,.rst-content h1 .btn-mini .headerlink:before,.rst-content h2 .btn-mini .headerlink:before,.rst-content h3 .btn-mini .headerlink:before,.rst-content h4 .btn-mini .headerlink:before,.rst-content h5 .btn-mini .headerlink:before,.rst-content h6 .btn-mini .headerlink:before,.rst-content p .btn-mini .headerlink:before,.rst-content table>caption .btn-mini .headerlink:before,.rst-content tt.download .btn-mini span:first-child:before,.wy-menu-vertical li .btn-mini button.toctree-expand:before{font-size:14px;vertical-align:-15%}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.wy-alert{padding:12px;line-height:24px;margin-bottom:24px;background:#e7f2fa}.rst-content .admonition-title,.wy-alert-title{font-weight:700;display:block;color:#fff;background:#6ab0de;padding:6px 12px;margin:-12px -12px 12px}.rst-content .danger,.rst-content .error,.rst-content .wy-alert-danger.admonition,.rst-content .wy-alert-danger.admonition-todo,.rst-content .wy-alert-danger.attention,.rst-content .wy-alert-danger.caution,.rst-content .wy-alert-danger.hint,.rst-content .wy-alert-danger.important,.rst-content .wy-alert-danger.note,.rst-content .wy-alert-danger.seealso,.rst-content .wy-alert-danger.tip,.rst-content .wy-alert-danger.warning,.wy-alert.wy-alert-danger{background:#fdf3f2}.rst-content .danger .admonition-title,.rst-content .danger .wy-alert-title,.rst-content .error .admonition-title,.rst-content .error .wy-alert-title,.rst-content .wy-alert-danger.admonition-todo .admonition-title,.rst-content .wy-alert-danger.admonition-todo .wy-alert-title,.rst-content .wy-alert-danger.admonition .admonition-title,.rst-content .wy-alert-danger.admonition .wy-alert-title,.rst-content .wy-alert-danger.attention .admonition-title,.rst-content .wy-alert-danger.attention .wy-alert-title,.rst-content .wy-alert-danger.caution .admonition-title,.rst-content .wy-alert-danger.caution .wy-alert-title,.rst-content .wy-alert-danger.hint .admonition-title,.rst-content .wy-alert-danger.hint .wy-alert-title,.rst-content .wy-alert-danger.important .admonition-title,.rst-content .wy-alert-danger.important .wy-alert-title,.rst-content .wy-alert-danger.note .admonition-title,.rst-content .wy-alert-danger.note .wy-alert-title,.rst-content .wy-alert-danger.seealso .admonition-title,.rst-content .wy-alert-danger.seealso .wy-alert-title,.rst-content .wy-alert-danger.tip .admonition-title,.rst-content .wy-alert-danger.tip .wy-alert-title,.rst-content .wy-alert-danger.warning .admonition-title,.rst-content .wy-alert-danger.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-danger .admonition-title,.wy-alert.wy-alert-danger .rst-content .admonition-title,.wy-alert.wy-alert-danger .wy-alert-title{background:#f29f97}.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .warning,.rst-content .wy-alert-warning.admonition,.rst-content .wy-alert-warning.danger,.rst-content .wy-alert-warning.error,.rst-content .wy-alert-warning.hint,.rst-content .wy-alert-warning.important,.rst-content .wy-alert-warning.note,.rst-content .wy-alert-warning.seealso,.rst-content .wy-alert-warning.tip,.wy-alert.wy-alert-warning{background:#ffedcc}.rst-content .admonition-todo .admonition-title,.rst-content .admonition-todo .wy-alert-title,.rst-content .attention .admonition-title,.rst-content .attention .wy-alert-title,.rst-content .caution .admonition-title,.rst-content .caution .wy-alert-title,.rst-content .warning .admonition-title,.rst-content .warning .wy-alert-title,.rst-content .wy-alert-warning.admonition .admonition-title,.rst-content .wy-alert-warning.admonition .wy-alert-title,.rst-content .wy-alert-warning.danger .admonition-title,.rst-content .wy-alert-warning.danger .wy-alert-title,.rst-content .wy-alert-warning.error .admonition-title,.rst-content .wy-alert-warning.error .wy-alert-title,.rst-content .wy-alert-warning.hint .admonition-title,.rst-content .wy-alert-warning.hint .wy-alert-title,.rst-content .wy-alert-warning.important .admonition-title,.rst-content .wy-alert-warning.important .wy-alert-title,.rst-content .wy-alert-warning.note .admonition-title,.rst-content .wy-alert-warning.note .wy-alert-title,.rst-content .wy-alert-warning.seealso .admonition-title,.rst-content .wy-alert-warning.seealso .wy-alert-title,.rst-content .wy-alert-warning.tip .admonition-title,.rst-content .wy-alert-warning.tip .wy-alert-title,.rst-content .wy-alert.wy-alert-warning .admonition-title,.wy-alert.wy-alert-warning .rst-content .admonition-title,.wy-alert.wy-alert-warning .wy-alert-title{background:#f0b37e}.rst-content .note,.rst-content .seealso,.rst-content .wy-alert-info.admonition,.rst-content .wy-alert-info.admonition-todo,.rst-content .wy-alert-info.attention,.rst-content .wy-alert-info.caution,.rst-content .wy-alert-info.danger,.rst-content .wy-alert-info.error,.rst-content .wy-alert-info.hint,.rst-content .wy-alert-info.important,.rst-content .wy-alert-info.tip,.rst-content .wy-alert-info.warning,.wy-alert.wy-alert-info{background:#e7f2fa}.rst-content .note .admonition-title,.rst-content .note .wy-alert-title,.rst-content .seealso .admonition-title,.rst-content .seealso .wy-alert-title,.rst-content .wy-alert-info.admonition-todo .admonition-title,.rst-content .wy-alert-info.admonition-todo .wy-alert-title,.rst-content .wy-alert-info.admonition .admonition-title,.rst-content .wy-alert-info.admonition .wy-alert-title,.rst-content .wy-alert-info.attention .admonition-title,.rst-content .wy-alert-info.attention .wy-alert-title,.rst-content .wy-alert-info.caution .admonition-title,.rst-content .wy-alert-info.caution .wy-alert-title,.rst-content .wy-alert-info.danger .admonition-title,.rst-content .wy-alert-info.danger .wy-alert-title,.rst-content .wy-alert-info.error .admonition-title,.rst-content .wy-alert-info.error .wy-alert-title,.rst-content .wy-alert-info.hint .admonition-title,.rst-content .wy-alert-info.hint .wy-alert-title,.rst-content .wy-alert-info.important .admonition-title,.rst-content .wy-alert-info.important .wy-alert-title,.rst-content .wy-alert-info.tip .admonition-title,.rst-content .wy-alert-info.tip .wy-alert-title,.rst-content .wy-alert-info.warning .admonition-title,.rst-content .wy-alert-info.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-info .admonition-title,.wy-alert.wy-alert-info .rst-content .admonition-title,.wy-alert.wy-alert-info .wy-alert-title{background:#6ab0de}.rst-content .hint,.rst-content .important,.rst-content .tip,.rst-content .wy-alert-success.admonition,.rst-content .wy-alert-success.admonition-todo,.rst-content .wy-alert-success.attention,.rst-content .wy-alert-success.caution,.rst-content .wy-alert-success.danger,.rst-content .wy-alert-success.error,.rst-content .wy-alert-success.note,.rst-content .wy-alert-success.seealso,.rst-content .wy-alert-success.warning,.wy-alert.wy-alert-success{background:#dbfaf4}.rst-content .hint .admonition-title,.rst-content .hint .wy-alert-title,.rst-content .important .admonition-title,.rst-content .important .wy-alert-title,.rst-content .tip .admonition-title,.rst-content .tip .wy-alert-title,.rst-content .wy-alert-success.admonition-todo .admonition-title,.rst-content .wy-alert-success.admonition-todo .wy-alert-title,.rst-content .wy-alert-success.admonition .admonition-title,.rst-content .wy-alert-success.admonition .wy-alert-title,.rst-content .wy-alert-success.attention .admonition-title,.rst-content .wy-alert-success.attention .wy-alert-title,.rst-content .wy-alert-success.caution .admonition-title,.rst-content .wy-alert-success.caution .wy-alert-title,.rst-content .wy-alert-success.danger .admonition-title,.rst-content .wy-alert-success.danger .wy-alert-title,.rst-content .wy-alert-success.error .admonition-title,.rst-content .wy-alert-success.error .wy-alert-title,.rst-content .wy-alert-success.note .admonition-title,.rst-content .wy-alert-success.note .wy-alert-title,.rst-content .wy-alert-success.seealso .admonition-title,.rst-content .wy-alert-success.seealso .wy-alert-title,.rst-content .wy-alert-success.warning .admonition-title,.rst-content .wy-alert-success.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-success .admonition-title,.wy-alert.wy-alert-success .rst-content .admonition-title,.wy-alert.wy-alert-success .wy-alert-title{background:#1abc9c}.rst-content .wy-alert-neutral.admonition,.rst-content .wy-alert-neutral.admonition-todo,.rst-content .wy-alert-neutral.attention,.rst-content .wy-alert-neutral.caution,.rst-content .wy-alert-neutral.danger,.rst-content .wy-alert-neutral.error,.rst-content .wy-alert-neutral.hint,.rst-content .wy-alert-neutral.important,.rst-content .wy-alert-neutral.note,.rst-content .wy-alert-neutral.seealso,.rst-content .wy-alert-neutral.tip,.rst-content .wy-alert-neutral.warning,.wy-alert.wy-alert-neutral{background:#f3f6f6}.rst-content .wy-alert-neutral.admonition-todo .admonition-title,.rst-content .wy-alert-neutral.admonition-todo .wy-alert-title,.rst-content .wy-alert-neutral.admonition .admonition-title,.rst-content .wy-alert-neutral.admonition .wy-alert-title,.rst-content .wy-alert-neutral.attention .admonition-title,.rst-content .wy-alert-neutral.attention .wy-alert-title,.rst-content .wy-alert-neutral.caution .admonition-title,.rst-content .wy-alert-neutral.caution .wy-alert-title,.rst-content .wy-alert-neutral.danger .admonition-title,.rst-content .wy-alert-neutral.danger .wy-alert-title,.rst-content .wy-alert-neutral.error .admonition-title,.rst-content .wy-alert-neutral.error .wy-alert-title,.rst-content .wy-alert-neutral.hint .admonition-title,.rst-content .wy-alert-neutral.hint .wy-alert-title,.rst-content .wy-alert-neutral.important .admonition-title,.rst-content .wy-alert-neutral.important .wy-alert-title,.rst-content .wy-alert-neutral.note .admonition-title,.rst-content .wy-alert-neutral.note .wy-alert-title,.rst-content .wy-alert-neutral.seealso .admonition-title,.rst-content .wy-alert-neutral.seealso .wy-alert-title,.rst-content .wy-alert-neutral.tip .admonition-title,.rst-content .wy-alert-neutral.tip .wy-alert-title,.rst-content .wy-alert-neutral.warning .admonition-title,.rst-content .wy-alert-neutral.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-neutral .admonition-title,.wy-alert.wy-alert-neutral .rst-content .admonition-title,.wy-alert.wy-alert-neutral .wy-alert-title{color:#404040;background:#e1e4e5}.rst-content .wy-alert-neutral.admonition-todo a,.rst-content .wy-alert-neutral.admonition a,.rst-content .wy-alert-neutral.attention a,.rst-content .wy-alert-neutral.caution a,.rst-content .wy-alert-neutral.danger a,.rst-content .wy-alert-neutral.error a,.rst-content .wy-alert-neutral.hint a,.rst-content .wy-alert-neutral.important a,.rst-content .wy-alert-neutral.note a,.rst-content .wy-alert-neutral.seealso a,.rst-content .wy-alert-neutral.tip a,.rst-content .wy-alert-neutral.warning a,.wy-alert.wy-alert-neutral a{color:#2980b9}.rst-content .admonition-todo p:last-child,.rst-content .admonition p:last-child,.rst-content .attention p:last-child,.rst-content .caution p:last-child,.rst-content .danger p:last-child,.rst-content .error p:last-child,.rst-content .hint p:last-child,.rst-content .important p:last-child,.rst-content .note p:last-child,.rst-content .seealso p:last-child,.rst-content .tip p:last-child,.rst-content .warning p:last-child,.wy-alert p:last-child{margin-bottom:0}.wy-tray-container{position:fixed;bottom:0;left:0;z-index:600}.wy-tray-container li{display:block;width:300px;background:transparent;color:#fff;text-align:center;box-shadow:0 5px 5px 0 rgba(0,0,0,.1);padding:0 24px;min-width:20%;opacity:0;height:0;line-height:56px;overflow:hidden;-webkit-transition:all .3s ease-in;-moz-transition:all .3s ease-in;transition:all .3s ease-in}.wy-tray-container li.wy-tray-item-success{background:#27ae60}.wy-tray-container li.wy-tray-item-info{background:#2980b9}.wy-tray-container li.wy-tray-item-warning{background:#e67e22}.wy-tray-container li.wy-tray-item-danger{background:#e74c3c}.wy-tray-container li.on{opacity:1;height:56px}@media screen and (max-width:768px){.wy-tray-container{bottom:auto;top:0;width:100%}.wy-tray-container li{width:100%}}button{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle;cursor:pointer;line-height:normal;-webkit-appearance:button;*overflow:visible}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}button[disabled]{cursor:default}.btn{display:inline-block;border-radius:2px;line-height:normal;white-space:nowrap;text-align:center;cursor:pointer;font-size:100%;padding:6px 12px 8px;color:#fff;border:1px solid rgba(0,0,0,.1);background-color:#27ae60;text-decoration:none;font-weight:400;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 2px -1px hsla(0,0%,100%,.5),inset 0 -2px 0 0 rgba(0,0,0,.1);outline-none:false;vertical-align:middle;*display:inline;zoom:1;-webkit-user-drag:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;-webkit-transition:all .1s linear;-moz-transition:all .1s linear;transition:all .1s linear}.btn-hover{background:#2e8ece;color:#fff}.btn:hover{background:#2cc36b;color:#fff}.btn:focus{background:#2cc36b;outline:0}.btn:active{box-shadow:inset 0 -1px 0 0 rgba(0,0,0,.05),inset 0 2px 0 0 rgba(0,0,0,.1);padding:8px 12px 6px}.btn:visited{color:#fff}.btn-disabled,.btn-disabled:active,.btn-disabled:focus,.btn-disabled:hover,.btn:disabled{background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=40);opacity:.4;cursor:not-allowed;box-shadow:none}.btn::-moz-focus-inner{padding:0;border:0}.btn-small{font-size:80%}.btn-info{background-color:#2980b9!important}.btn-info:hover{background-color:#2e8ece!important}.btn-neutral{background-color:#f3f6f6!important;color:#404040!important}.btn-neutral:hover{background-color:#e5ebeb!important;color:#404040}.btn-neutral:visited{color:#404040!important}.btn-success{background-color:#27ae60!important}.btn-success:hover{background-color:#295!important}.btn-danger{background-color:#e74c3c!important}.btn-danger:hover{background-color:#ea6153!important}.btn-warning{background-color:#e67e22!important}.btn-warning:hover{background-color:#e98b39!important}.btn-invert{background-color:#222}.btn-invert:hover{background-color:#2f2f2f!important}.btn-link{background-color:transparent!important;color:#2980b9;box-shadow:none;border-color:transparent!important}.btn-link:active,.btn-link:hover{background-color:transparent!important;color:#409ad5!important;box-shadow:none}.btn-link:visited{color:#9b59b6}.wy-btn-group .btn,.wy-control .btn{vertical-align:middle}.wy-btn-group{margin-bottom:24px;*zoom:1}.wy-btn-group:after,.wy-btn-group:before{display:table;content:""}.wy-btn-group:after{clear:both}.wy-dropdown{position:relative;display:inline-block}.wy-dropdown-active .wy-dropdown-menu{display:block}.wy-dropdown-menu{position:absolute;left:0;display:none;float:left;top:100%;min-width:100%;background:#fcfcfc;z-index:100;border:1px solid #cfd7dd;box-shadow:0 2px 2px 0 rgba(0,0,0,.1);padding:12px}.wy-dropdown-menu>dd>a{display:block;clear:both;color:#404040;white-space:nowrap;font-size:90%;padding:0 12px;cursor:pointer}.wy-dropdown-menu>dd>a:hover{background:#2980b9;color:#fff}.wy-dropdown-menu>dd.divider{border-top:1px solid #cfd7dd;margin:6px 0}.wy-dropdown-menu>dd.search{padding-bottom:12px}.wy-dropdown-menu>dd.search input[type=search]{width:100%}.wy-dropdown-menu>dd.call-to-action{background:#e3e3e3;text-transform:uppercase;font-weight:500;font-size:80%}.wy-dropdown-menu>dd.call-to-action:hover{background:#e3e3e3}.wy-dropdown-menu>dd.call-to-action .btn{color:#fff}.wy-dropdown.wy-dropdown-up .wy-dropdown-menu{bottom:100%;top:auto;left:auto;right:0}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu{background:#fcfcfc;margin-top:2px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a{padding:6px 12px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a:hover{background:#2980b9;color:#fff}.wy-dropdown.wy-dropdown-left .wy-dropdown-menu{right:0;left:auto;text-align:right}.wy-dropdown-arrow:before{content:" ";border-bottom:5px solid #f5f5f5;border-left:5px solid transparent;border-right:5px solid transparent;position:absolute;display:block;top:-4px;left:50%;margin-left:-3px}.wy-dropdown-arrow.wy-dropdown-arrow-left:before{left:11px}.wy-form-stacked select{display:block}.wy-form-aligned .wy-help-inline,.wy-form-aligned input,.wy-form-aligned label,.wy-form-aligned select,.wy-form-aligned textarea{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-form-aligned .wy-control-group>label{display:inline-block;vertical-align:middle;width:10em;margin:6px 12px 0 0;float:left}.wy-form-aligned .wy-control{float:left}.wy-form-aligned .wy-control label{display:block}.wy-form-aligned .wy-control select{margin-top:6px}fieldset{margin:0}fieldset,legend{border:0;padding:0}legend{width:100%;white-space:normal;margin-bottom:24px;font-size:150%;*margin-left:-7px}label,legend{display:block}label{margin:0 0 .3125em;color:#333;font-size:90%}input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}.wy-control-group{margin-bottom:24px;max-width:1200px;margin-left:auto;margin-right:auto;*zoom:1}.wy-control-group:after,.wy-control-group:before{display:table;content:""}.wy-control-group:after{clear:both}.wy-control-group.wy-control-group-required>label:after{content:" *";color:#e74c3c}.wy-control-group .wy-form-full,.wy-control-group .wy-form-halves,.wy-control-group .wy-form-thirds{padding-bottom:12px}.wy-control-group .wy-form-full input[type=color],.wy-control-group .wy-form-full input[type=date],.wy-control-group .wy-form-full input[type=datetime-local],.wy-control-group .wy-form-full input[type=datetime],.wy-control-group .wy-form-full input[type=email],.wy-control-group .wy-form-full input[type=month],.wy-control-group .wy-form-full input[type=number],.wy-control-group .wy-form-full input[type=password],.wy-control-group .wy-form-full input[type=search],.wy-control-group .wy-form-full input[type=tel],.wy-control-group .wy-form-full input[type=text],.wy-control-group .wy-form-full input[type=time],.wy-control-group .wy-form-full input[type=url],.wy-control-group .wy-form-full input[type=week],.wy-control-group .wy-form-full select,.wy-control-group .wy-form-halves input[type=color],.wy-control-group .wy-form-halves input[type=date],.wy-control-group .wy-form-halves input[type=datetime-local],.wy-control-group .wy-form-halves input[type=datetime],.wy-control-group .wy-form-halves input[type=email],.wy-control-group .wy-form-halves input[type=month],.wy-control-group .wy-form-halves input[type=number],.wy-control-group .wy-form-halves input[type=password],.wy-control-group .wy-form-halves input[type=search],.wy-control-group .wy-form-halves input[type=tel],.wy-control-group .wy-form-halves input[type=text],.wy-control-group .wy-form-halves input[type=time],.wy-control-group .wy-form-halves input[type=url],.wy-control-group .wy-form-halves input[type=week],.wy-control-group .wy-form-halves select,.wy-control-group .wy-form-thirds input[type=color],.wy-control-group .wy-form-thirds input[type=date],.wy-control-group .wy-form-thirds input[type=datetime-local],.wy-control-group .wy-form-thirds input[type=datetime],.wy-control-group .wy-form-thirds input[type=email],.wy-control-group .wy-form-thirds input[type=month],.wy-control-group .wy-form-thirds input[type=number],.wy-control-group .wy-form-thirds input[type=password],.wy-control-group .wy-form-thirds input[type=search],.wy-control-group .wy-form-thirds input[type=tel],.wy-control-group .wy-form-thirds input[type=text],.wy-control-group .wy-form-thirds input[type=time],.wy-control-group .wy-form-thirds input[type=url],.wy-control-group .wy-form-thirds input[type=week],.wy-control-group .wy-form-thirds select{width:100%}.wy-control-group .wy-form-full{float:left;display:block;width:100%;margin-right:0}.wy-control-group .wy-form-full:last-child{margin-right:0}.wy-control-group .wy-form-halves{float:left;display:block;margin-right:2.35765%;width:48.82117%}.wy-control-group .wy-form-halves:last-child,.wy-control-group .wy-form-halves:nth-of-type(2n){margin-right:0}.wy-control-group .wy-form-halves:nth-of-type(odd){clear:left}.wy-control-group .wy-form-thirds{float:left;display:block;margin-right:2.35765%;width:31.76157%}.wy-control-group .wy-form-thirds:last-child,.wy-control-group .wy-form-thirds:nth-of-type(3n){margin-right:0}.wy-control-group .wy-form-thirds:nth-of-type(3n+1){clear:left}.wy-control-group.wy-control-group-no-input .wy-control,.wy-control-no-input{margin:6px 0 0;font-size:90%}.wy-control-no-input{display:inline-block}.wy-control-group.fluid-input input[type=color],.wy-control-group.fluid-input input[type=date],.wy-control-group.fluid-input input[type=datetime-local],.wy-control-group.fluid-input input[type=datetime],.wy-control-group.fluid-input input[type=email],.wy-control-group.fluid-input input[type=month],.wy-control-group.fluid-input input[type=number],.wy-control-group.fluid-input input[type=password],.wy-control-group.fluid-input input[type=search],.wy-control-group.fluid-input input[type=tel],.wy-control-group.fluid-input input[type=text],.wy-control-group.fluid-input input[type=time],.wy-control-group.fluid-input input[type=url],.wy-control-group.fluid-input input[type=week]{width:100%}.wy-form-message-inline{padding-left:.3em;color:#666;font-size:90%}.wy-form-message{display:block;color:#999;font-size:70%;margin-top:.3125em;font-style:italic}.wy-form-message p{font-size:inherit;font-style:italic;margin-bottom:6px}.wy-form-message p:last-child{margin-bottom:0}input{line-height:normal}input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;*overflow:visible}input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week]{-webkit-appearance:none;padding:6px;display:inline-block;border:1px solid #ccc;font-size:80%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 3px #ddd;border-radius:0;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}input[type=datetime-local]{padding:.34375em .625em}input[disabled]{cursor:default}input[type=checkbox],input[type=radio]{padding:0;margin-right:.3125em;*height:13px;*width:13px}input[type=checkbox],input[type=radio],input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus{outline:0;outline:thin dotted\9;border-color:#333}input.no-focus:focus{border-color:#ccc!important}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:thin dotted #333;outline:1px auto #129fea}input[type=color][disabled],input[type=date][disabled],input[type=datetime-local][disabled],input[type=datetime][disabled],input[type=email][disabled],input[type=month][disabled],input[type=number][disabled],input[type=password][disabled],input[type=search][disabled],input[type=tel][disabled],input[type=text][disabled],input[type=time][disabled],input[type=url][disabled],input[type=week][disabled]{cursor:not-allowed;background-color:#fafafa}input:focus:invalid,select:focus:invalid,textarea:focus:invalid{color:#e74c3c;border:1px solid #e74c3c}input:focus:invalid:focus,select:focus:invalid:focus,textarea:focus:invalid:focus{border-color:#e74c3c}input[type=checkbox]:focus:invalid:focus,input[type=file]:focus:invalid:focus,input[type=radio]:focus:invalid:focus{outline-color:#e74c3c}input.wy-input-large{padding:12px;font-size:100%}textarea{overflow:auto;vertical-align:top;width:100%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif}select,textarea{padding:.5em .625em;display:inline-block;border:1px solid #ccc;font-size:80%;box-shadow:inset 0 1px 3px #ddd;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}select{border:1px solid #ccc;background-color:#fff}select[multiple]{height:auto}select:focus,textarea:focus{outline:0}input[readonly],select[disabled],select[readonly],textarea[disabled],textarea[readonly]{cursor:not-allowed;background-color:#fafafa}input[type=checkbox][disabled],input[type=radio][disabled]{cursor:not-allowed}.wy-checkbox,.wy-radio{margin:6px 0;color:#404040;display:block}.wy-checkbox input,.wy-radio input{vertical-align:baseline}.wy-form-message-inline{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-input-prefix,.wy-input-suffix{white-space:nowrap;padding:6px}.wy-input-prefix .wy-input-context,.wy-input-suffix .wy-input-context{line-height:27px;padding:0 8px;display:inline-block;font-size:80%;background-color:#f3f6f6;border:1px solid #ccc;color:#999}.wy-input-suffix .wy-input-context{border-left:0}.wy-input-prefix .wy-input-context{border-right:0}.wy-switch{position:relative;display:block;height:24px;margin-top:12px;cursor:pointer}.wy-switch:before{left:0;top:0;width:36px;height:12px;background:#ccc}.wy-switch:after,.wy-switch:before{position:absolute;content:"";display:block;border-radius:4px;-webkit-transition:all .2s ease-in-out;-moz-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.wy-switch:after{width:18px;height:18px;background:#999;left:-3px;top:-3px}.wy-switch span{position:absolute;left:48px;display:block;font-size:12px;color:#ccc;line-height:1}.wy-switch.active:before{background:#1e8449}.wy-switch.active:after{left:24px;background:#27ae60}.wy-switch.disabled{cursor:not-allowed;opacity:.8}.wy-control-group.wy-control-group-error .wy-form-message,.wy-control-group.wy-control-group-error>label{color:#e74c3c}.wy-control-group.wy-control-group-error input[type=color],.wy-control-group.wy-control-group-error input[type=date],.wy-control-group.wy-control-group-error input[type=datetime-local],.wy-control-group.wy-control-group-error input[type=datetime],.wy-control-group.wy-control-group-error input[type=email],.wy-control-group.wy-control-group-error input[type=month],.wy-control-group.wy-control-group-error input[type=number],.wy-control-group.wy-control-group-error input[type=password],.wy-control-group.wy-control-group-error input[type=search],.wy-control-group.wy-control-group-error input[type=tel],.wy-control-group.wy-control-group-error input[type=text],.wy-control-group.wy-control-group-error input[type=time],.wy-control-group.wy-control-group-error input[type=url],.wy-control-group.wy-control-group-error input[type=week],.wy-control-group.wy-control-group-error textarea{border:1px solid #e74c3c}.wy-inline-validate{white-space:nowrap}.wy-inline-validate .wy-input-context{padding:.5em .625em;display:inline-block;font-size:80%}.wy-inline-validate.wy-inline-validate-success .wy-input-context{color:#27ae60}.wy-inline-validate.wy-inline-validate-danger .wy-input-context{color:#e74c3c}.wy-inline-validate.wy-inline-validate-warning .wy-input-context{color:#e67e22}.wy-inline-validate.wy-inline-validate-info .wy-input-context{color:#2980b9}.rotate-90{-webkit-transform:rotate(90deg);-moz-transform:rotate(90deg);-ms-transform:rotate(90deg);-o-transform:rotate(90deg);transform:rotate(90deg)}.rotate-180{-webkit-transform:rotate(180deg);-moz-transform:rotate(180deg);-ms-transform:rotate(180deg);-o-transform:rotate(180deg);transform:rotate(180deg)}.rotate-270{-webkit-transform:rotate(270deg);-moz-transform:rotate(270deg);-ms-transform:rotate(270deg);-o-transform:rotate(270deg);transform:rotate(270deg)}.mirror{-webkit-transform:scaleX(-1);-moz-transform:scaleX(-1);-ms-transform:scaleX(-1);-o-transform:scaleX(-1);transform:scaleX(-1)}.mirror.rotate-90{-webkit-transform:scaleX(-1) rotate(90deg);-moz-transform:scaleX(-1) rotate(90deg);-ms-transform:scaleX(-1) rotate(90deg);-o-transform:scaleX(-1) rotate(90deg);transform:scaleX(-1) rotate(90deg)}.mirror.rotate-180{-webkit-transform:scaleX(-1) rotate(180deg);-moz-transform:scaleX(-1) rotate(180deg);-ms-transform:scaleX(-1) rotate(180deg);-o-transform:scaleX(-1) rotate(180deg);transform:scaleX(-1) rotate(180deg)}.mirror.rotate-270{-webkit-transform:scaleX(-1) rotate(270deg);-moz-transform:scaleX(-1) rotate(270deg);-ms-transform:scaleX(-1) rotate(270deg);-o-transform:scaleX(-1) rotate(270deg);transform:scaleX(-1) rotate(270deg)}@media only screen and (max-width:480px){.wy-form button[type=submit]{margin:.7em 0 0}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=text],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week],.wy-form label{margin-bottom:.3em;display:block}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week]{margin-bottom:0}.wy-form-aligned .wy-control-group label{margin-bottom:.3em;text-align:left;display:block;width:100%}.wy-form-aligned .wy-control{margin:1.5em 0 0}.wy-form-message,.wy-form-message-inline,.wy-form .wy-help-inline{display:block;font-size:80%;padding:6px 0}}@media screen and (max-width:768px){.tablet-hide{display:none}}@media screen and (max-width:480px){.mobile-hide{display:none}}.float-left{float:left}.float-right{float:right}.full-width{width:100%}.rst-content table.docutils,.rst-content table.field-list,.wy-table{border-collapse:collapse;border-spacing:0;empty-cells:show;margin-bottom:24px}.rst-content table.docutils caption,.rst-content table.field-list caption,.wy-table caption{color:#000;font:italic 85%/1 arial,sans-serif;padding:1em 0;text-align:center}.rst-content table.docutils td,.rst-content table.docutils th,.rst-content table.field-list td,.rst-content table.field-list th,.wy-table td,.wy-table th{font-size:90%;margin:0;overflow:visible;padding:8px 16px}.rst-content table.docutils td:first-child,.rst-content table.docutils th:first-child,.rst-content table.field-list td:first-child,.rst-content table.field-list th:first-child,.wy-table td:first-child,.wy-table th:first-child{border-left-width:0}.rst-content table.docutils thead,.rst-content table.field-list thead,.wy-table thead{color:#000;text-align:left;vertical-align:bottom;white-space:nowrap}.rst-content table.docutils thead th,.rst-content table.field-list thead th,.wy-table thead th{font-weight:700;border-bottom:2px solid #e1e4e5}.rst-content table.docutils td,.rst-content table.field-list td,.wy-table td{background-color:transparent;vertical-align:middle}.rst-content table.docutils td p,.rst-content table.field-list td p,.wy-table td p{line-height:18px}.rst-content table.docutils td p:last-child,.rst-content table.field-list td p:last-child,.wy-table td p:last-child{margin-bottom:0}.rst-content table.docutils .wy-table-cell-min,.rst-content table.field-list .wy-table-cell-min,.wy-table .wy-table-cell-min{width:1%;padding-right:0}.rst-content table.docutils .wy-table-cell-min input[type=checkbox],.rst-content table.field-list .wy-table-cell-min input[type=checkbox],.wy-table .wy-table-cell-min input[type=checkbox]{margin:0}.wy-table-secondary{color:grey;font-size:90%}.wy-table-tertiary{color:grey;font-size:80%}.rst-content table.docutils:not(.field-list) tr:nth-child(2n-1) td,.wy-table-backed,.wy-table-odd td,.wy-table-striped tr:nth-child(2n-1) td{background-color:#f3f6f6}.rst-content table.docutils,.wy-table-bordered-all{border:1px solid #e1e4e5}.rst-content table.docutils td,.wy-table-bordered-all td{border-bottom:1px solid #e1e4e5;border-left:1px solid #e1e4e5}.rst-content table.docutils tbody>tr:last-child td,.wy-table-bordered-all tbody>tr:last-child td{border-bottom-width:0}.wy-table-bordered{border:1px solid #e1e4e5}.wy-table-bordered-rows td{border-bottom:1px solid #e1e4e5}.wy-table-bordered-rows tbody>tr:last-child td{border-bottom-width:0}.wy-table-horizontal td,.wy-table-horizontal th{border-width:0 0 1px;border-bottom:1px solid #e1e4e5}.wy-table-horizontal tbody>tr:last-child td{border-bottom-width:0}.wy-table-responsive{margin-bottom:24px;max-width:100%;overflow:auto}.wy-table-responsive table{margin-bottom:0!important}.wy-table-responsive table td,.wy-table-responsive table th{white-space:nowrap}a{color:#2980b9;text-decoration:none;cursor:pointer}a:hover{color:#3091d1}a:visited{color:#9b59b6}html{height:100%}body,html{overflow-x:hidden}body{font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;font-weight:400;color:#404040;min-height:100%;background:#edf0f2}.wy-text-left{text-align:left}.wy-text-center{text-align:center}.wy-text-right{text-align:right}.wy-text-large{font-size:120%}.wy-text-normal{font-size:100%}.wy-text-small,small{font-size:80%}.wy-text-strike{text-decoration:line-through}.wy-text-warning{color:#e67e22!important}a.wy-text-warning:hover{color:#eb9950!important}.wy-text-info{color:#2980b9!important}a.wy-text-info:hover{color:#409ad5!important}.wy-text-success{color:#27ae60!important}a.wy-text-success:hover{color:#36d278!important}.wy-text-danger{color:#e74c3c!important}a.wy-text-danger:hover{color:#ed7669!important}.wy-text-neutral{color:#404040!important}a.wy-text-neutral:hover{color:#595959!important}.rst-content .toctree-wrapper>p.caption,h1,h2,h3,h4,h5,h6,legend{margin-top:0;font-weight:700;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif}p{line-height:24px;font-size:16px;margin:0 0 24px}h1{font-size:175%}.rst-content .toctree-wrapper>p.caption,h2{font-size:150%}h3{font-size:125%}h4{font-size:115%}h5{font-size:110%}h6{font-size:100%}hr{display:block;height:1px;border:0;border-top:1px solid #e1e4e5;margin:24px 0;padding:0}.rst-content code,.rst-content tt,code{white-space:nowrap;max-width:100%;background:#fff;border:1px solid #e1e4e5;font-size:75%;padding:0 5px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#e74c3c;overflow-x:auto}.rst-content tt.code-large,code.code-large{font-size:90%}.rst-content .section ul,.rst-content .toctree-wrapper ul,.rst-content section ul,.wy-plain-list-disc,article ul{list-style:disc;line-height:24px;margin-bottom:24px}.rst-content .section ul li,.rst-content .toctree-wrapper ul li,.rst-content section ul li,.wy-plain-list-disc li,article ul li{list-style:disc;margin-left:24px}.rst-content .section ul li p:last-child,.rst-content .section ul li ul,.rst-content .toctree-wrapper ul li p:last-child,.rst-content .toctree-wrapper ul li ul,.rst-content section ul li p:last-child,.rst-content section ul li ul,.wy-plain-list-disc li p:last-child,.wy-plain-list-disc li ul,article ul li p:last-child,article ul li ul{margin-bottom:0}.rst-content .section ul li li,.rst-content .toctree-wrapper ul li li,.rst-content section ul li li,.wy-plain-list-disc li li,article ul li li{list-style:circle}.rst-content .section ul li li li,.rst-content .toctree-wrapper ul li li li,.rst-content section ul li li li,.wy-plain-list-disc li li li,article ul li li li{list-style:square}.rst-content .section ul li ol li,.rst-content .toctree-wrapper ul li ol li,.rst-content section ul li ol li,.wy-plain-list-disc li ol li,article ul li ol li{list-style:decimal}.rst-content .section ol,.rst-content .section ol.arabic,.rst-content .toctree-wrapper ol,.rst-content .toctree-wrapper ol.arabic,.rst-content section ol,.rst-content section ol.arabic,.wy-plain-list-decimal,article ol{list-style:decimal;line-height:24px;margin-bottom:24px}.rst-content .section ol.arabic li,.rst-content .section ol li,.rst-content .toctree-wrapper ol.arabic li,.rst-content .toctree-wrapper ol li,.rst-content section ol.arabic li,.rst-content section ol li,.wy-plain-list-decimal li,article ol li{list-style:decimal;margin-left:24px}.rst-content .section ol.arabic li ul,.rst-content .section ol li p:last-child,.rst-content .section ol li ul,.rst-content .toctree-wrapper ol.arabic li ul,.rst-content .toctree-wrapper ol li p:last-child,.rst-content .toctree-wrapper ol li ul,.rst-content section ol.arabic li ul,.rst-content section ol li p:last-child,.rst-content section ol li ul,.wy-plain-list-decimal li p:last-child,.wy-plain-list-decimal li ul,article ol li p:last-child,article ol li ul{margin-bottom:0}.rst-content .section ol.arabic li ul li,.rst-content .section ol li ul li,.rst-content .toctree-wrapper ol.arabic li ul li,.rst-content .toctree-wrapper ol li ul li,.rst-content section ol.arabic li ul li,.rst-content section ol li ul li,.wy-plain-list-decimal li ul li,article ol li ul li{list-style:disc}.wy-breadcrumbs{*zoom:1}.wy-breadcrumbs:after,.wy-breadcrumbs:before{display:table;content:""}.wy-breadcrumbs:after{clear:both}.wy-breadcrumbs li{display:inline-block}.wy-breadcrumbs li.wy-breadcrumbs-aside{float:right}.wy-breadcrumbs li a{display:inline-block;padding:5px}.wy-breadcrumbs li a:first-child{padding-left:0}.rst-content .wy-breadcrumbs li tt,.wy-breadcrumbs li .rst-content tt,.wy-breadcrumbs li code{padding:5px;border:none;background:none}.rst-content .wy-breadcrumbs li tt.literal,.wy-breadcrumbs li .rst-content tt.literal,.wy-breadcrumbs li code.literal{color:#404040}.wy-breadcrumbs-extra{margin-bottom:0;color:#b3b3b3;font-size:80%;display:inline-block}@media screen and (max-width:480px){.wy-breadcrumbs-extra,.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}@media print{.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}html{font-size:16px}.wy-affix{position:fixed;top:1.618em}.wy-menu a:hover{text-decoration:none}.wy-menu-horiz{*zoom:1}.wy-menu-horiz:after,.wy-menu-horiz:before{display:table;content:""}.wy-menu-horiz:after{clear:both}.wy-menu-horiz li,.wy-menu-horiz ul{display:inline-block}.wy-menu-horiz li:hover{background:hsla(0,0%,100%,.1)}.wy-menu-horiz li.divide-left{border-left:1px solid #404040}.wy-menu-horiz li.divide-right{border-right:1px solid #404040}.wy-menu-horiz a{height:32px;display:inline-block;line-height:32px;padding:0 16px}.wy-menu-vertical{width:300px}.wy-menu-vertical header,.wy-menu-vertical p.caption{color:#55a5d9;height:32px;line-height:32px;padding:0 1.618em;margin:12px 0 0;display:block;font-weight:700;text-transform:uppercase;font-size:85%;white-space:nowrap}.wy-menu-vertical ul{margin-bottom:0}.wy-menu-vertical li.divide-top{border-top:1px solid #404040}.wy-menu-vertical li.divide-bottom{border-bottom:1px solid #404040}.wy-menu-vertical li.current{background:#e3e3e3}.wy-menu-vertical li.current a{color:grey;border-right:1px solid #c9c9c9;padding:.4045em 2.427em}.wy-menu-vertical li.current a:hover{background:#d6d6d6}.rst-content .wy-menu-vertical li tt,.wy-menu-vertical li .rst-content tt,.wy-menu-vertical li code{border:none;background:inherit;color:inherit;padding-left:0;padding-right:0}.wy-menu-vertical li button.toctree-expand{display:block;float:left;margin-left:-1.2em;line-height:18px;color:#4d4d4d;border:none;background:none;padding:0}.wy-menu-vertical li.current>a,.wy-menu-vertical li.on a{color:#404040;font-weight:700;position:relative;background:#fcfcfc;border:none;padding:.4045em 1.618em}.wy-menu-vertical li.current>a:hover,.wy-menu-vertical li.on a:hover{background:#fcfcfc}.wy-menu-vertical li.current>a:hover button.toctree-expand,.wy-menu-vertical li.on a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand{display:block;line-height:18px;color:#333}.wy-menu-vertical li.toctree-l1.current>a{border-bottom:1px solid #c9c9c9;border-top:1px solid #c9c9c9}.wy-menu-vertical .toctree-l1.current .toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .toctree-l11>ul{display:none}.wy-menu-vertical .toctree-l1.current .current.toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .current.toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .current.toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .current.toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .current.toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .current.toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .current.toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .current.toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .current.toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .current.toctree-l11>ul{display:block}.wy-menu-vertical li.toctree-l3,.wy-menu-vertical li.toctree-l4{font-size:.9em}.wy-menu-vertical li.toctree-l2 a,.wy-menu-vertical li.toctree-l3 a,.wy-menu-vertical li.toctree-l4 a,.wy-menu-vertical li.toctree-l5 a,.wy-menu-vertical li.toctree-l6 a,.wy-menu-vertical li.toctree-l7 a,.wy-menu-vertical li.toctree-l8 a,.wy-menu-vertical li.toctree-l9 a,.wy-menu-vertical li.toctree-l10 a{color:#404040}.wy-menu-vertical li.toctree-l2 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l3 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l4 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l5 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l6 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l7 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l8 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l9 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l10 a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a,.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a,.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a,.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a,.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a,.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a,.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a,.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{display:block}.wy-menu-vertical li.toctree-l2.current>a{padding:.4045em 2.427em}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{padding:.4045em 1.618em .4045em 4.045em}.wy-menu-vertical li.toctree-l3.current>a{padding:.4045em 4.045em}.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{padding:.4045em 1.618em .4045em 5.663em}.wy-menu-vertical li.toctree-l4.current>a{padding:.4045em 5.663em}.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a{padding:.4045em 1.618em .4045em 7.281em}.wy-menu-vertical li.toctree-l5.current>a{padding:.4045em 7.281em}.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a{padding:.4045em 1.618em .4045em 8.899em}.wy-menu-vertical li.toctree-l6.current>a{padding:.4045em 8.899em}.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a{padding:.4045em 1.618em .4045em 10.517em}.wy-menu-vertical li.toctree-l7.current>a{padding:.4045em 10.517em}.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a{padding:.4045em 1.618em .4045em 12.135em}.wy-menu-vertical li.toctree-l8.current>a{padding:.4045em 12.135em}.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a{padding:.4045em 1.618em .4045em 13.753em}.wy-menu-vertical li.toctree-l9.current>a{padding:.4045em 13.753em}.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a{padding:.4045em 1.618em .4045em 15.371em}.wy-menu-vertical li.toctree-l10.current>a{padding:.4045em 15.371em}.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{padding:.4045em 1.618em .4045em 16.989em}.wy-menu-vertical li.toctree-l2.current>a,.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{background:#c9c9c9}.wy-menu-vertical li.toctree-l2 button.toctree-expand{color:#a3a3a3}.wy-menu-vertical li.toctree-l3.current>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{background:#bdbdbd}.wy-menu-vertical li.toctree-l3 button.toctree-expand{color:#969696}.wy-menu-vertical li.current ul{display:block}.wy-menu-vertical li ul{margin-bottom:0;display:none}.wy-menu-vertical li ul li a{margin-bottom:0;color:#d9d9d9;font-weight:400}.wy-menu-vertical a{line-height:18px;padding:.4045em 1.618em;display:block;position:relative;font-size:90%;color:#d9d9d9}.wy-menu-vertical a:hover{background-color:#4e4a4a;cursor:pointer}.wy-menu-vertical a:hover button.toctree-expand{color:#d9d9d9}.wy-menu-vertical a:active{background-color:#2980b9;cursor:pointer;color:#fff}.wy-menu-vertical a:active button.toctree-expand{color:#fff}.wy-side-nav-search{display:block;width:300px;padding:.809em;margin-bottom:.809em;z-index:200;background-color:#2980b9;text-align:center;color:#fcfcfc}.wy-side-nav-search input[type=text]{width:100%;border-radius:50px;padding:6px 12px;border-color:#2472a4}.wy-side-nav-search img{display:block;margin:auto auto .809em;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a{color:#fcfcfc;font-size:100%;font-weight:700;display:inline-block;padding:4px 6px;margin-bottom:.809em;max-width:100%}.wy-side-nav-search .wy-dropdown>a:hover,.wy-side-nav-search>a:hover{background:hsla(0,0%,100%,.1)}.wy-side-nav-search .wy-dropdown>a img.logo,.wy-side-nav-search>a img.logo{display:block;margin:0 auto;height:auto;width:auto;border-radius:0;max-width:100%;background:transparent}.wy-side-nav-search .wy-dropdown>a.icon img.logo,.wy-side-nav-search>a.icon img.logo{margin-top:.85em}.wy-side-nav-search>div.version{margin-top:-.4045em;margin-bottom:.809em;font-weight:400;color:hsla(0,0%,100%,.3)}.wy-nav .wy-menu-vertical header{color:#2980b9}.wy-nav .wy-menu-vertical a{color:#b3b3b3}.wy-nav .wy-menu-vertical a:hover{background-color:#2980b9;color:#fff}[data-menu-wrap]{-webkit-transition:all .2s ease-in;-moz-transition:all .2s ease-in;transition:all .2s ease-in;position:absolute;opacity:1;width:100%;opacity:0}[data-menu-wrap].move-center{left:0;right:auto;opacity:1}[data-menu-wrap].move-left{right:auto;left:-100%;opacity:0}[data-menu-wrap].move-right{right:-100%;left:auto;opacity:0}.wy-body-for-nav{background:#fcfcfc}.wy-grid-for-nav{position:absolute;width:100%;height:100%}.wy-nav-side{position:fixed;top:0;bottom:0;left:0;padding-bottom:2em;width:300px;overflow-x:hidden;overflow-y:hidden;min-height:100%;color:#9b9b9b;background:#343131;z-index:200}.wy-side-scroll{width:320px;position:relative;overflow-x:hidden;overflow-y:scroll;height:100%}.wy-nav-top{display:none;background:#2980b9;color:#fff;padding:.4045em .809em;position:relative;line-height:50px;text-align:center;font-size:100%;*zoom:1}.wy-nav-top:after,.wy-nav-top:before{display:table;content:""}.wy-nav-top:after{clear:both}.wy-nav-top a{color:#fff;font-weight:700}.wy-nav-top img{margin-right:12px;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-nav-top i{font-size:30px;float:left;cursor:pointer;padding-top:inherit}.wy-nav-content-wrap{margin-left:300px;background:#fcfcfc;min-height:100%}.wy-nav-content{padding:1.618em 3.236em;height:100%;max-width:800px;margin:auto}.wy-body-mask{position:fixed;width:100%;height:100%;background:rgba(0,0,0,.2);display:none;z-index:499}.wy-body-mask.on{display:block}footer{color:grey}footer p{margin-bottom:12px}.rst-content footer span.commit tt,footer span.commit .rst-content tt,footer span.commit code{padding:0;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:1em;background:none;border:none;color:grey}.rst-footer-buttons{*zoom:1}.rst-footer-buttons:after,.rst-footer-buttons:before{width:100%;display:table;content:""}.rst-footer-buttons:after{clear:both}.rst-breadcrumbs-buttons{margin-top:12px;*zoom:1}.rst-breadcrumbs-buttons:after,.rst-breadcrumbs-buttons:before{display:table;content:""}.rst-breadcrumbs-buttons:after{clear:both}#search-results .search li{margin-bottom:24px;border-bottom:1px solid #e1e4e5;padding-bottom:24px}#search-results .search li:first-child{border-top:1px solid #e1e4e5;padding-top:24px}#search-results .search li a{font-size:120%;margin-bottom:12px;display:inline-block}#search-results .context{color:grey;font-size:90%}.genindextable li>ul{margin-left:24px}@media screen and (max-width:768px){.wy-body-for-nav{background:#fcfcfc}.wy-nav-top{display:block}.wy-nav-side{left:-300px}.wy-nav-side.shift{width:85%;left:0}.wy-menu.wy-menu-vertical,.wy-side-nav-search,.wy-side-scroll{width:auto}.wy-nav-content-wrap{margin-left:0}.wy-nav-content-wrap .wy-nav-content{padding:1.618em}.wy-nav-content-wrap.shift{position:fixed;min-width:100%;left:85%;top:0;height:100%;overflow:hidden}}@media screen and (min-width:1100px){.wy-nav-content-wrap{background:rgba(0,0,0,.05)}.wy-nav-content{margin:0;background:#fcfcfc}}@media print{.rst-versions,.wy-nav-side,footer{display:none}.wy-nav-content-wrap{margin-left:0}}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60;*zoom:1}.rst-versions .rst-current-version:after,.rst-versions .rst-current-version:before{display:table;content:""}.rst-versions .rst-current-version:after{clear:both}.rst-content .code-block-caption .rst-versions .rst-current-version .headerlink,.rst-content .eqno .rst-versions .rst-current-version .headerlink,.rst-content .rst-versions .rst-current-version .admonition-title,.rst-content code.download .rst-versions .rst-current-version span:first-child,.rst-content dl dt .rst-versions .rst-current-version .headerlink,.rst-content h1 .rst-versions .rst-current-version .headerlink,.rst-content h2 .rst-versions .rst-current-version .headerlink,.rst-content h3 .rst-versions .rst-current-version .headerlink,.rst-content h4 .rst-versions .rst-current-version .headerlink,.rst-content h5 .rst-versions .rst-current-version .headerlink,.rst-content h6 .rst-versions .rst-current-version .headerlink,.rst-content p .rst-versions .rst-current-version .headerlink,.rst-content table>caption .rst-versions .rst-current-version .headerlink,.rst-content tt.download .rst-versions .rst-current-version span:first-child,.rst-versions .rst-current-version .fa,.rst-versions .rst-current-version .icon,.rst-versions .rst-current-version .rst-content .admonition-title,.rst-versions .rst-current-version .rst-content .code-block-caption .headerlink,.rst-versions .rst-current-version .rst-content .eqno .headerlink,.rst-versions .rst-current-version .rst-content code.download span:first-child,.rst-versions .rst-current-version .rst-content dl dt .headerlink,.rst-versions .rst-current-version .rst-content h1 .headerlink,.rst-versions .rst-current-version .rst-content h2 .headerlink,.rst-versions .rst-current-version .rst-content h3 .headerlink,.rst-versions .rst-current-version .rst-content h4 .headerlink,.rst-versions .rst-current-version .rst-content h5 .headerlink,.rst-versions .rst-current-version .rst-content h6 .headerlink,.rst-versions .rst-current-version .rst-content p .headerlink,.rst-versions .rst-current-version .rst-content table>caption .headerlink,.rst-versions .rst-current-version .rst-content tt.download span:first-child,.rst-versions .rst-current-version .wy-menu-vertical li button.toctree-expand,.wy-menu-vertical li .rst-versions .rst-current-version button.toctree-expand{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}.rst-content .toctree-wrapper>p.caption,.rst-content h1,.rst-content h2,.rst-content h3,.rst-content h4,.rst-content h5,.rst-content h6{margin-bottom:24px}.rst-content img{max-width:100%;height:auto}.rst-content div.figure,.rst-content figure{margin-bottom:24px}.rst-content div.figure .caption-text,.rst-content figure .caption-text{font-style:italic}.rst-content div.figure p:last-child.caption,.rst-content figure p:last-child.caption{margin-bottom:0}.rst-content div.figure.align-center,.rst-content figure.align-center{text-align:center}.rst-content .section>a>img,.rst-content .section>img,.rst-content section>a>img,.rst-content section>img{margin-bottom:24px}.rst-content abbr[title]{text-decoration:none}.rst-content.style-external-links a.reference.external:after{font-family:FontAwesome;content:"\f08e";color:#b3b3b3;vertical-align:super;font-size:60%;margin:0 .2em}.rst-content blockquote{margin-left:24px;line-height:24px;margin-bottom:24px}.rst-content pre.literal-block{white-space:pre;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;display:block;overflow:auto}.rst-content div[class^=highlight],.rst-content pre.literal-block{border:1px solid #e1e4e5;overflow-x:auto;margin:1px 0 24px}.rst-content div[class^=highlight] div[class^=highlight],.rst-content pre.literal-block div[class^=highlight]{padding:0;border:none;margin:0}.rst-content div[class^=highlight] td.code{width:100%}.rst-content .linenodiv pre{border-right:1px solid #e6e9ea;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;user-select:none;pointer-events:none}.rst-content div[class^=highlight] pre{white-space:pre;margin:0;padding:12px;display:block;overflow:auto}.rst-content div[class^=highlight] pre .hll{display:block;margin:0 -12px;padding:0 12px}.rst-content .linenodiv pre,.rst-content div[class^=highlight] pre,.rst-content pre.literal-block{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:12px;line-height:1.4}.rst-content div.highlight .gp,.rst-content div.highlight span.linenos{user-select:none;pointer-events:none}.rst-content div.highlight span.linenos{display:inline-block;padding-left:0;padding-right:12px;margin-right:12px;border-right:1px solid #e6e9ea}.rst-content .code-block-caption{font-style:italic;font-size:85%;line-height:1;padding:1em 0;text-align:center}@media print{.rst-content .codeblock,.rst-content div[class^=highlight],.rst-content div[class^=highlight] pre{white-space:pre-wrap}}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning{clear:both}.rst-content .admonition-todo .last,.rst-content .admonition-todo>:last-child,.rst-content .admonition .last,.rst-content .admonition>:last-child,.rst-content .attention .last,.rst-content .attention>:last-child,.rst-content .caution .last,.rst-content .caution>:last-child,.rst-content .danger .last,.rst-content .danger>:last-child,.rst-content .error .last,.rst-content .error>:last-child,.rst-content .hint .last,.rst-content .hint>:last-child,.rst-content .important .last,.rst-content .important>:last-child,.rst-content .note .last,.rst-content .note>:last-child,.rst-content .seealso .last,.rst-content .seealso>:last-child,.rst-content .tip .last,.rst-content .tip>:last-child,.rst-content .warning .last,.rst-content .warning>:last-child{margin-bottom:0}.rst-content .admonition-title:before{margin-right:4px}.rst-content .admonition table{border-color:rgba(0,0,0,.1)}.rst-content .admonition table td,.rst-content .admonition table th{background:transparent!important;border-color:rgba(0,0,0,.1)!important}.rst-content .section ol.loweralpha,.rst-content .section ol.loweralpha>li,.rst-content .toctree-wrapper ol.loweralpha,.rst-content .toctree-wrapper ol.loweralpha>li,.rst-content section ol.loweralpha,.rst-content section ol.loweralpha>li{list-style:lower-alpha}.rst-content .section ol.upperalpha,.rst-content .section ol.upperalpha>li,.rst-content .toctree-wrapper ol.upperalpha,.rst-content .toctree-wrapper ol.upperalpha>li,.rst-content section ol.upperalpha,.rst-content section ol.upperalpha>li{list-style:upper-alpha}.rst-content .section ol li>*,.rst-content .section ul li>*,.rst-content .toctree-wrapper ol li>*,.rst-content .toctree-wrapper ul li>*,.rst-content section ol li>*,.rst-content section ul li>*{margin-top:12px;margin-bottom:12px}.rst-content .section ol li>:first-child,.rst-content .section ul li>:first-child,.rst-content .toctree-wrapper ol li>:first-child,.rst-content .toctree-wrapper ul li>:first-child,.rst-content section ol li>:first-child,.rst-content section ul li>:first-child{margin-top:0}.rst-content .section ol li>p,.rst-content .section ol li>p:last-child,.rst-content .section ul li>p,.rst-content .section ul li>p:last-child,.rst-content .toctree-wrapper ol li>p,.rst-content .toctree-wrapper ol li>p:last-child,.rst-content .toctree-wrapper ul li>p,.rst-content .toctree-wrapper ul li>p:last-child,.rst-content section ol li>p,.rst-content section ol li>p:last-child,.rst-content section ul li>p,.rst-content section ul li>p:last-child{margin-bottom:12px}.rst-content .section ol li>p:only-child,.rst-content .section ol li>p:only-child:last-child,.rst-content .section ul li>p:only-child,.rst-content .section ul li>p:only-child:last-child,.rst-content .toctree-wrapper ol li>p:only-child,.rst-content .toctree-wrapper ol li>p:only-child:last-child,.rst-content .toctree-wrapper ul li>p:only-child,.rst-content .toctree-wrapper ul li>p:only-child:last-child,.rst-content section ol li>p:only-child,.rst-content section ol li>p:only-child:last-child,.rst-content section ul li>p:only-child,.rst-content section ul li>p:only-child:last-child{margin-bottom:0}.rst-content .section ol li>ol,.rst-content .section ol li>ul,.rst-content .section ul li>ol,.rst-content .section ul li>ul,.rst-content .toctree-wrapper ol li>ol,.rst-content .toctree-wrapper ol li>ul,.rst-content .toctree-wrapper ul li>ol,.rst-content .toctree-wrapper ul li>ul,.rst-content section ol li>ol,.rst-content section ol li>ul,.rst-content section ul li>ol,.rst-content section ul li>ul{margin-bottom:12px}.rst-content .section ol.simple li>*,.rst-content .section ol.simple li ol,.rst-content .section ol.simple li ul,.rst-content .section ul.simple li>*,.rst-content .section ul.simple li ol,.rst-content .section ul.simple li ul,.rst-content .toctree-wrapper ol.simple li>*,.rst-content .toctree-wrapper ol.simple li ol,.rst-content .toctree-wrapper ol.simple li ul,.rst-content .toctree-wrapper ul.simple li>*,.rst-content .toctree-wrapper ul.simple li ol,.rst-content .toctree-wrapper ul.simple li ul,.rst-content section ol.simple li>*,.rst-content section ol.simple li ol,.rst-content section ol.simple li ul,.rst-content section ul.simple li>*,.rst-content section ul.simple li ol,.rst-content section ul.simple li ul{margin-top:0;margin-bottom:0}.rst-content .line-block{margin-left:0;margin-bottom:24px;line-height:24px}.rst-content .line-block .line-block{margin-left:24px;margin-bottom:0}.rst-content .topic-title{font-weight:700;margin-bottom:12px}.rst-content .toc-backref{color:#404040}.rst-content .align-right{float:right;margin:0 0 24px 24px}.rst-content .align-left{float:left;margin:0 24px 24px 0}.rst-content .align-center{margin:auto}.rst-content .align-center:not(table){display:block}.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink{opacity:0;font-size:14px;font-family:FontAwesome;margin-left:.5em}.rst-content .code-block-caption .headerlink:focus,.rst-content .code-block-caption:hover .headerlink,.rst-content .eqno .headerlink:focus,.rst-content .eqno:hover .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink:focus,.rst-content .toctree-wrapper>p.caption:hover .headerlink,.rst-content dl dt .headerlink:focus,.rst-content dl dt:hover .headerlink,.rst-content h1 .headerlink:focus,.rst-content h1:hover .headerlink,.rst-content h2 .headerlink:focus,.rst-content h2:hover .headerlink,.rst-content h3 .headerlink:focus,.rst-content h3:hover .headerlink,.rst-content h4 .headerlink:focus,.rst-content h4:hover .headerlink,.rst-content h5 .headerlink:focus,.rst-content h5:hover .headerlink,.rst-content h6 .headerlink:focus,.rst-content h6:hover .headerlink,.rst-content p.caption .headerlink:focus,.rst-content p.caption:hover .headerlink,.rst-content p .headerlink:focus,.rst-content p:hover .headerlink,.rst-content table>caption .headerlink:focus,.rst-content table>caption:hover .headerlink{opacity:1}.rst-content .btn:focus{outline:2px solid}.rst-content table>caption .headerlink:after{font-size:12px}.rst-content .centered{text-align:center}.rst-content .sidebar{float:right;width:40%;display:block;margin:0 0 24px 24px;padding:24px;background:#f3f6f6;border:1px solid #e1e4e5}.rst-content .sidebar dl,.rst-content .sidebar p,.rst-content .sidebar ul{font-size:90%}.rst-content .sidebar .last,.rst-content .sidebar>:last-child{margin-bottom:0}.rst-content .sidebar .sidebar-title{display:block;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif;font-weight:700;background:#e1e4e5;padding:6px 12px;margin:-24px -24px 24px;font-size:100%}.rst-content .highlighted{background:#f1c40f;box-shadow:0 0 0 2px #f1c40f;display:inline;font-weight:700}.rst-content .citation-reference,.rst-content .footnote-reference{vertical-align:baseline;position:relative;top:-.4em;line-height:0;font-size:90%}.rst-content .hlist{width:100%}.rst-content dl dt span.classifier:before{content:" : "}.rst-content dl dt span.classifier-delimiter{display:none!important}html.writer-html4 .rst-content table.docutils.citation,html.writer-html4 .rst-content table.docutils.footnote{background:none;border:none}html.writer-html4 .rst-content table.docutils.citation td,html.writer-html4 .rst-content table.docutils.citation tr,html.writer-html4 .rst-content table.docutils.footnote td,html.writer-html4 .rst-content table.docutils.footnote tr{border:none;background-color:transparent!important;white-space:normal}html.writer-html4 .rst-content table.docutils.citation td.label,html.writer-html4 .rst-content table.docutils.footnote td.label{padding-left:0;padding-right:0;vertical-align:top}html.writer-html5 .rst-content dl.field-list,html.writer-html5 .rst-content dl.footnote{display:grid;grid-template-columns:max-content auto}html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dt{padding-left:1rem}html.writer-html5 .rst-content dl.field-list>dt:after,html.writer-html5 .rst-content dl.footnote>dt:after{content:":"}html.writer-html5 .rst-content dl.field-list>dd,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dd,html.writer-html5 .rst-content dl.footnote>dt{margin-bottom:0}html.writer-html5 .rst-content dl.footnote{font-size:.9rem}html.writer-html5 .rst-content dl.footnote>dt{margin:0 .5rem .5rem 0;line-height:1.2rem;word-break:break-all;font-weight:400}html.writer-html5 .rst-content dl.footnote>dt>span.brackets{margin-right:.5rem}html.writer-html5 .rst-content dl.footnote>dt>span.brackets:before{content:"["}html.writer-html5 .rst-content dl.footnote>dt>span.brackets:after{content:"]"}html.writer-html5 .rst-content dl.footnote>dt>span.fn-backref{font-style:italic}html.writer-html5 .rst-content dl.footnote>dd{margin:0 0 .5rem;line-height:1.2rem}html.writer-html5 .rst-content dl.footnote>dd p,html.writer-html5 .rst-content dl.option-list kbd{font-size:.9rem}.rst-content table.docutils.footnote,html.writer-html4 .rst-content table.docutils.citation,html.writer-html5 .rst-content dl.footnote{color:grey}.rst-content table.docutils.footnote code,.rst-content table.docutils.footnote tt,html.writer-html4 .rst-content table.docutils.citation code,html.writer-html4 .rst-content table.docutils.citation tt,html.writer-html5 .rst-content dl.footnote code,html.writer-html5 .rst-content dl.footnote tt{color:#555}.rst-content .wy-table-responsive.citation,.rst-content .wy-table-responsive.footnote{margin-bottom:0}.rst-content .wy-table-responsive.citation+:not(.citation),.rst-content .wy-table-responsive.footnote+:not(.footnote){margin-top:24px}.rst-content .wy-table-responsive.citation:last-child,.rst-content .wy-table-responsive.footnote:last-child{margin-bottom:24px}.rst-content table.docutils th{border-color:#e1e4e5}html.writer-html5 .rst-content table.docutils th{border:1px solid #e1e4e5}html.writer-html5 .rst-content table.docutils td>p,html.writer-html5 .rst-content table.docutils th>p{line-height:1rem;margin-bottom:0;font-size:.9rem}.rst-content table.docutils td .last,.rst-content table.docutils td .last>:last-child{margin-bottom:0}.rst-content table.field-list,.rst-content table.field-list td{border:none}.rst-content table.field-list td p{font-size:inherit;line-height:inherit}.rst-content table.field-list td>strong{display:inline-block}.rst-content table.field-list .field-name{padding-right:10px;text-align:left;white-space:nowrap}.rst-content table.field-list .field-body{text-align:left}.rst-content code,.rst-content tt{color:#000;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;padding:2px 5px}.rst-content code big,.rst-content code em,.rst-content tt big,.rst-content tt em{font-size:100%!important;line-height:normal}.rst-content code.literal,.rst-content tt.literal{color:#e74c3c;white-space:normal}.rst-content code.xref,.rst-content tt.xref,a .rst-content code,a .rst-content tt{font-weight:700;color:#404040}.rst-content kbd,.rst-content pre,.rst-content samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace}.rst-content a code,.rst-content a tt{color:#2980b9}.rst-content dl{margin-bottom:24px}.rst-content dl dt{font-weight:700;margin-bottom:12px}.rst-content dl ol,.rst-content dl p,.rst-content dl table,.rst-content dl ul{margin-bottom:12px}.rst-content dl dd{margin:0 0 12px 24px;line-height:24px}html.writer-html4 .rst-content dl:not(.docutils),html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple){margin-bottom:24px}html.writer-html4 .rst-content dl:not(.docutils)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt{display:table;margin:6px 0;font-size:90%;line-height:normal;background:#e7f2fa;color:#2980b9;border-top:3px solid #6ab0de;padding:6px;position:relative}html.writer-html4 .rst-content dl:not(.docutils)>dt:before,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt:before{color:#6ab0de}html.writer-html4 .rst-content dl:not(.docutils)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.field-list)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dl:not(.field-list)>dt{margin-bottom:6px;border:none;border-left:3px solid #ccc;background:#f0f0f0;color:#555}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.field-list)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dl:not(.field-list)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils)>dt:first-child,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt:first-child{margin-top:0}html.writer-html4 .rst-content dl:not(.docutils) code.descclassname,html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descclassname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descname{background-color:transparent;border:none;padding:0;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descname{font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .optional,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .optional{display:inline-block;padding:0 4px;color:#000;font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .property,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .property{display:inline-block;padding-right:8px;max-width:100%}html.writer-html4 .rst-content dl:not(.docutils) .k,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .k{font-style:italic}html.writer-html4 .rst-content dl:not(.docutils) .descclassname,html.writer-html4 .rst-content dl:not(.docutils) .descname,html.writer-html4 .rst-content dl:not(.docutils) .sig-name,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .sig-name{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#000}.rst-content .viewcode-back,.rst-content .viewcode-link{display:inline-block;color:#27ae60;font-size:80%;padding-left:24px}.rst-content .viewcode-back{display:block;float:right}.rst-content p.rubric{margin-bottom:12px;font-weight:700}.rst-content code.download,.rst-content tt.download{background:inherit;padding:inherit;font-weight:400;font-family:inherit;font-size:inherit;color:inherit;border:inherit;white-space:inherit}.rst-content code.download span:first-child,.rst-content tt.download span:first-child{-webkit-font-smoothing:subpixel-antialiased}.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{margin-right:4px}.rst-content .guilabel{border:1px solid #7fbbe3;background:#e7f2fa;font-size:80%;font-weight:700;border-radius:4px;padding:2.4px 6px;margin:auto 2px}.rst-content .versionmodified{font-style:italic}@media screen and (max-width:480px){.rst-content .sidebar{width:100%}}span[id*=MathJax-Span]{color:#404040}.math{text-align:center}@font-face{font-family:Lato;src:url(fonts/lato-normal.woff2?bd03a2cc277bbbc338d464e679fe9942) format("woff2"),url(fonts/lato-normal.woff?27bd77b9162d388cb8d4c4217c7c5e2a) format("woff");font-weight:400;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold.woff2?cccb897485813c7c256901dbca54ecf2) format("woff2"),url(fonts/lato-bold.woff?d878b6c29b10beca227e9eef4246111b) format("woff");font-weight:700;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold-italic.woff2?0b6bb6725576b072c5d0b02ecdd1900d) format("woff2"),url(fonts/lato-bold-italic.woff?9c7e4e9eb485b4a121c760e61bc3707c) format("woff");font-weight:700;font-style:italic;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-normal-italic.woff2?4eb103b4d12be57cb1d040ed5e162e9d) format("woff2"),url(fonts/lato-normal-italic.woff?f28f2d6482446544ef1ea1ccc6dd5892) format("woff");font-weight:400;font-style:italic;font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:400;src:url(fonts/Roboto-Slab-Regular.woff2?7abf5b8d04d26a2cafea937019bca958) format("woff2"),url(fonts/Roboto-Slab-Regular.woff?c1be9284088d487c5e3ff0a10a92e58c) format("woff");font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:700;src:url(fonts/Roboto-Slab-Bold.woff2?9984f4a9bda09be08e83f2506954adbe) format("woff2"),url(fonts/Roboto-Slab-Bold.woff?bed5564a116b05148e3b3bea6fb1162a) format("woff");font-display:block}
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/jquery-3.6.0.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/jquery-3.5.1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 /*!
- * jQuery JavaScript Library v3.6.0
+ * jQuery JavaScript Library v3.5.1
  * https://jquery.com/
  *
  * Includes Sizzle.js
  * https://sizzlejs.com/
  *
- * Copyright OpenJS Foundation and other contributors
+ * Copyright JS Foundation and other contributors
  * Released under the MIT license
  * https://jquery.org/license
  *
- * Date: 2021-03-02T17:08Z
+ * Date: 2020-05-04T22:49Z
  */
 (function(global, factory) {
 
     "use strict";
 
     if (typeof module === "object" && typeof module.exports === "object") {
 
@@ -76,19 +76,15 @@
 
     var isFunction = function isFunction(obj) {
 
         // Support: Chrome <=57, Firefox <=52
         // In some browsers, typeof returns "function" for HTML <object> elements
         // (i.e., `typeof document.createElement( "object" ) === "function"`).
         // We don't want to classify *any* DOM node as a function.
-        // Support: QtWeb <=3.8.5, WebKit <=534.34, wkhtmltopdf tool <=0.12.5
-        // Plus for old WebKit, typeof returns "function" for HTML collections
-        // (e.g., `typeof document.getElementsByTagName("div") === "function"`). (gh-4756)
-        return typeof obj === "function" && typeof obj.nodeType !== "number" &&
-            typeof obj.item !== "function";
+        return typeof obj === "function" && typeof obj.nodeType !== "number";
     };
 
 
     var isWindow = function isWindow(obj) {
         return obj != null && obj === obj.window;
     };
 
@@ -147,15 +143,15 @@
     /* global Symbol */
     // Defining this global in .eslintrc.json would create a danger of using the global
     // unguarded in another place, it seems safer to define global only for this module
 
 
 
     var
-        version = "3.6.0",
+        version = "3.5.1",
 
         // Define a local copy of jQuery
         jQuery = function(selector, context) {
 
             // The jQuery object is actually just the init constructor 'enhanced'
             // Need init if jQuery is called (just allow error to be thrown if not included)
             return new jQuery.fn.init(selector, context);
@@ -519,22 +515,22 @@
         }
 
         return type === "array" || length === 0 ||
             typeof length === "number" && length > 0 && (length - 1) in obj;
     }
     var Sizzle =
         /*!
-         * Sizzle CSS Selector Engine v2.3.6
+         * Sizzle CSS Selector Engine v2.3.5
          * https://sizzlejs.com/
          *
          * Copyright JS Foundation and other contributors
          * Released under the MIT license
          * https://js.foundation/
          *
-         * Date: 2021-02-16
+         * Date: 2020-03-14
          */
         (function(window) {
             var i,
                 support,
                 Expr,
                 getText,
                 isXML,
@@ -1112,16 +1108,16 @@
 
             /**
              * Detects XML nodes
              * @param {Element|Object} elem An element or a document
              * @returns {Boolean} True iff elem is a non-HTML XML node
              */
             isXML = Sizzle.isXML = function(elem) {
-                var namespace = elem && elem.namespaceURI,
-                    docElem = elem && (elem.ownerDocument || elem).documentElement;
+                var namespace = elem.namespaceURI,
+                    docElem = (elem.ownerDocument || elem).documentElement;
 
                 // Support: IE <=8
                 // Assume HTML when documentElement doesn't yet exist, such as inside loading iframes
                 // https://bugs.jquery.com/ticket/4833
                 return !rhtml.test(namespace || docElem && docElem.nodeName || "HTML");
             };
 
@@ -3052,15 +3048,15 @@
 
 
 
     function nodeName(elem, name) {
 
         return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
 
-    }
+    };
     var rsingleTag = (/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i);
 
 
 
     // Implement the identical functionality for filter and not
     function winnow(elements, qualifier, not) {
         if (isFunction(qualifier)) {
@@ -4028,47 +4024,47 @@
                 // count of unprocessed arguments
                 i = remaining,
 
                 // subordinate fulfillment data
                 resolveContexts = Array(i),
                 resolveValues = slice.call(arguments),
 
-                // the primary Deferred
-                primary = jQuery.Deferred(),
+                // the master Deferred
+                master = jQuery.Deferred(),
 
                 // subordinate callback factory
                 updateFunc = function(i) {
                     return function(value) {
                         resolveContexts[i] = this;
                         resolveValues[i] = arguments.length > 1 ? slice.call(arguments) : value;
                         if (!(--remaining)) {
-                            primary.resolveWith(resolveContexts, resolveValues);
+                            master.resolveWith(resolveContexts, resolveValues);
                         }
                     };
                 };
 
             // Single- and empty arguments are adopted like Promise.resolve
             if (remaining <= 1) {
-                adoptValue(singleValue, primary.done(updateFunc(i)).resolve, primary.reject,
+                adoptValue(singleValue, master.done(updateFunc(i)).resolve, master.reject,
                     !remaining);
 
                 // Use .then() to unwrap secondary thenables (cf. gh-3000)
-                if (primary.state() === "pending" ||
+                if (master.state() === "pending" ||
                     isFunction(resolveValues[i] && resolveValues[i].then)) {
 
-                    return primary.then();
+                    return master.then();
                 }
             }
 
             // Multiple arguments are aggregated like Promise.all array elements
             while (i--) {
-                adoptValue(resolveValues[i], updateFunc(i), primary.reject);
+                adoptValue(resolveValues[i], updateFunc(i), master.reject);
             }
 
-            return primary.promise();
+            return master.promise();
         }
     });
 
 
     // These usually indicate a programmer mistake during development,
     // warn about them ASAP rather than swallowing them by default.
     var rerrorNames = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
@@ -5121,15 +5117,18 @@
             }
         }
 
         return fragment;
     }
 
 
-    var rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
+    var
+        rkeyEvent = /^key/,
+        rmouseEvent = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+        rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
 
     function returnTrue() {
         return true;
     }
 
     function returnFalse() {
         return false;
@@ -5690,21 +5689,15 @@
                             result = {};
                         }
                         if (saved !== result) {
 
                             // Cancel the outer synthetic event
                             event.stopImmediatePropagation();
                             event.preventDefault();
-
-                            // Support: Chrome 86+
-                            // In Chrome, if an element having a focusout handler is blurred by
-                            // clicking outside of it, it invokes the handler synchronously. If
-                            // that handler calls `.remove()` on the element, the data is cleared,
-                            // leaving `result` undefined. We need to guard against this.
-                            return result && result.value;
+                            return result.value;
                         }
 
                         // If this is an inner synthetic event for an event with a bubbling surrogate
                         // (focus or blur), assume that the surrogate already propagated from triggering the
                         // native event and prevent that from happening again here.
                         // This technically gets the ordering wrong w.r.t. to `.trigger()` (in which the
                         // bubbling surrogate propagates *after* the non-bubbling base), but that seems
@@ -5861,15 +5854,42 @@
         pointerId: true,
         pointerType: true,
         screenX: true,
         screenY: true,
         targetTouches: true,
         toElement: true,
         touches: true,
-        which: true
+
+        which: function(event) {
+            var button = event.button;
+
+            // Add which for key events
+            if (event.which == null && rkeyEvent.test(event.type)) {
+                return event.charCode != null ? event.charCode : event.keyCode;
+            }
+
+            // Add which for click: 1 === left; 2 === middle; 3 === right
+            if (!event.which && button !== undefined && rmouseEvent.test(event.type)) {
+                if (button & 1) {
+                    return 1;
+                }
+
+                if (button & 2) {
+                    return 3;
+                }
+
+                if (button & 4) {
+                    return 2;
+                }
+
+                return 0;
+            }
+
+            return event.which;
+        }
     }, jQuery.event.addProp);
 
     jQuery.each({
         focus: "focusin",
         blur: "focusout"
     }, function(type, delegateType) {
         jQuery.event.special[type] = {
@@ -5890,20 +5910,14 @@
                 // Force setup before trigger
                 leverageNative(this, type);
 
                 // Return non-false to allow normal event-path propagation
                 return true;
             },
 
-            // Suppress native focus or blur as it's already being fired
-            // in leverageNative.
-            _default: function() {
-                return true;
-            },
-
             delegateType: delegateType
         };
     });
 
     // Create mouseenter/leave events using mouseover/out and event-time checks
     // so that event delegation works in jQuery.
     // Do the same for pointerenter/pointerleave and pointerover/pointerout
@@ -6567,51 +6581,32 @@
             },
 
             // Support: IE 9 - 11+, Edge 15 - 18+
             // IE/Edge misreport `getComputedStyle` of table rows with width/height
             // set in CSS while `offset*` properties report correct values.
             // Behavior in IE 9 is more subtle than in newer versions & it passes
             // some versions of this test; make sure not to make it pass there!
-            //
-            // Support: Firefox 70+
-            // Only Firefox includes border widths
-            // in computed dimensions. (gh-4529)
             reliableTrDimensions: function() {
                 var table, tr, trChild, trStyle;
                 if (reliableTrDimensionsVal == null) {
                     table = document.createElement("table");
                     tr = document.createElement("tr");
                     trChild = document.createElement("div");
 
-                    table.style.cssText = "position:absolute;left:-11111px;border-collapse:separate";
-                    tr.style.cssText = "border:1px solid";
-
-                    // Support: Chrome 86+
-                    // Height set through cssText does not get applied.
-                    // Computed height then comes back as 0.
+                    table.style.cssText = "position:absolute;left:-11111px";
                     tr.style.height = "1px";
                     trChild.style.height = "9px";
 
-                    // Support: Android 8 Chrome 86+
-                    // In our bodyBackground.html iframe,
-                    // display for all div elements is set to "inline",
-                    // which causes a problem only in Android 8 Chrome 86.
-                    // Ensuring the div is display: block
-                    // gets around this issue.
-                    trChild.style.display = "block";
-
                     documentElement
                         .appendChild(table)
                         .appendChild(tr)
                         .appendChild(trChild);
 
                     trStyle = window.getComputedStyle(tr);
-                    reliableTrDimensionsVal = (parseInt(trStyle.height, 10) +
-                        parseInt(trStyle.borderTopWidth, 10) +
-                        parseInt(trStyle.borderBottomWidth, 10)) === tr.offsetHeight;
+                    reliableTrDimensionsVal = parseInt(trStyle.height) > 3;
 
                     documentElement.removeChild(table);
                 }
                 return reliableTrDimensionsVal;
             }
         });
     })();
@@ -7818,15 +7813,14 @@
                     var anim = Animation(this, jQuery.extend({}, prop), optall);
 
                     // Empty animations, or finishing resolves immediately
                     if (empty || dataPriv.get(this, "finish")) {
                         anim.stop(true);
                     }
                 };
-
             doAnimation.finish = doAnimation;
 
             return empty || optall.queue === false ?
                 this.each(doAnimation) :
                 this.queue(optall.queue, doAnimation);
         },
         stop: function(type, clearQueue, gotoEnd) {
@@ -8770,15 +8764,17 @@
             while ((cur = eventPath[i++]) && !event.isPropagationStopped()) {
                 lastElement = cur;
                 event.type = i > 1 ?
                     bubbleType :
                     special.bindType || type;
 
                 // jQuery handler
-                handle = (dataPriv.get(cur, "events") || Object.create(null))[event.type] &&
+                handle = (
+                        dataPriv.get(cur, "events") || Object.create(null)
+                    )[event.type] &&
                     dataPriv.get(cur, "handle");
                 if (handle) {
                     handle.apply(cur, data);
                 }
 
                 // Native handler
                 handle = ontype && cur[ontype];
@@ -8921,34 +8917,29 @@
 
     var rquery = (/\?/);
 
 
 
     // Cross-browser xml parsing
     jQuery.parseXML = function(data) {
-        var xml, parserErrorElem;
+        var xml;
         if (!data || typeof data !== "string") {
             return null;
         }
 
         // Support: IE 9 - 11 only
         // IE throws on parseFromString with invalid input.
         try {
             xml = (new window.DOMParser()).parseFromString(data, "text/xml");
-        } catch (e) {}
+        } catch (e) {
+            xml = undefined;
+        }
 
-        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
-        if (!xml || parserErrorElem) {
-            jQuery.error("Invalid XML: " + (
-                parserErrorElem ?
-                jQuery.map(parserErrorElem.childNodes, function(el) {
-                    return el.textContent;
-                }).join("\n") :
-                data
-            ));
+        if (!xml || xml.getElementsByTagName("parsererror").length) {
+            jQuery.error("Invalid XML: " + data);
         }
         return xml;
     };
 
 
     var
         rbracket = /\[\]$/,
@@ -9038,45 +9029,47 @@
     jQuery.fn.extend({
         serialize: function() {
             return jQuery.param(this.serializeArray());
         },
         serializeArray: function() {
             return this.map(function() {
 
-                // Can add propHook for "elements" to filter or add form elements
-                var elements = jQuery.prop(this, "elements");
-                return elements ? jQuery.makeArray(elements) : this;
-            }).filter(function() {
-                var type = this.type;
-
-                // Use .is( ":disabled" ) so that fieldset[disabled] works
-                return this.name && !jQuery(this).is(":disabled") &&
-                    rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
-                    (this.checked || !rcheckableType.test(type));
-            }).map(function(_i, elem) {
-                var val = jQuery(this).val();
+                    // Can add propHook for "elements" to filter or add form elements
+                    var elements = jQuery.prop(this, "elements");
+                    return elements ? jQuery.makeArray(elements) : this;
+                })
+                .filter(function() {
+                    var type = this.type;
 
-                if (val == null) {
-                    return null;
-                }
+                    // Use .is( ":disabled" ) so that fieldset[disabled] works
+                    return this.name && !jQuery(this).is(":disabled") &&
+                        rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
+                        (this.checked || !rcheckableType.test(type));
+                })
+                .map(function(_i, elem) {
+                    var val = jQuery(this).val();
 
-                if (Array.isArray(val)) {
-                    return jQuery.map(val, function(val) {
-                        return {
-                            name: elem.name,
-                            value: val.replace(rCRLF, "\r\n")
-                        };
-                    });
-                }
+                    if (val == null) {
+                        return null;
+                    }
 
-                return {
-                    name: elem.name,
-                    value: val.replace(rCRLF, "\r\n")
-                };
-            }).get();
+                    if (Array.isArray(val)) {
+                        return jQuery.map(val, function(val) {
+                            return {
+                                name: elem.name,
+                                value: val.replace(rCRLF, "\r\n")
+                            };
+                        });
+                    }
+
+                    return {
+                        name: elem.name,
+                        value: val.replace(rCRLF, "\r\n")
+                    };
+                }).get();
         }
     });
 
 
     var
         r20 = /%20/g,
         rhash = /#.*$/,
@@ -9107,15 +9100,14 @@
         transports = {},
 
         // Avoid comment-prolog char sequence (#10098); must appease lint and evade compression
         allTypes = "*/".concat("*"),
 
         // Anchor tag for parsing the document origin
         originAnchor = document.createElement("a");
-
     originAnchor.href = location.href;
 
     // Base "constructor" for jQuery.ajaxPrefilter and jQuery.ajaxTransport
     function addToPrefiltersOrTransports(structure) {
 
         // dataTypeExpression is optional and defaults to "*"
         return function(dataTypeExpression, func) {
@@ -9805,18 +9797,16 @@
                 isSuccess = status >= 200 && status < 300 || status === 304;
 
                 // Get response data
                 if (responses) {
                     response = ajaxHandleResponses(s, jqXHR, responses);
                 }
 
-                // Use a noop converter for missing script but not if jsonp
-                if (!isSuccess &&
-                    jQuery.inArray("script", s.dataTypes) > -1 &&
-                    jQuery.inArray("json", s.dataTypes) < 0) {
+                // Use a noop converter for missing script
+                if (!isSuccess && jQuery.inArray("script", s.dataTypes) > -1) {
                     s.converters["text script"] = function() {};
                 }
 
                 // Convert no matter what (that way responseXXX fields are always set)
                 response = ajaxConvert(s, response, jqXHR, isSuccess);
 
                 // If successful, handle type chaining
@@ -10551,14 +10541,20 @@
                 props.left = (options.left - curOffset.left) + curLeft;
             }
 
             if ("using" in options) {
                 options.using.call(elem, props);
 
             } else {
+                if (typeof props.top === "number") {
+                    props.top += "px";
+                }
+                if (typeof props.left === "number") {
+                    props.left += "px";
+                }
                 curElem.css(props);
             }
         }
     };
 
     jQuery.fn.extend({
 
@@ -10732,58 +10728,59 @@
 
     // Create innerHeight, innerWidth, height, width, outerHeight and outerWidth methods
     jQuery.each({
         Height: "height",
         Width: "width"
     }, function(name, type) {
         jQuery.each({
-            padding: "inner" + name,
-            content: type,
-            "": "outer" + name
-        }, function(defaultExtra, funcName) {
-
-            // Margin is only for outerHeight, outerWidth
-            jQuery.fn[funcName] = function(margin, value) {
-                var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
-                    extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
-
-                return access(this, function(elem, type, value) {
-                    var doc;
-
-                    if (isWindow(elem)) {
-
-                        // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
-                        return funcName.indexOf("outer") === 0 ?
-                            elem["inner" + name] :
-                            elem.document.documentElement["client" + name];
-                    }
-
-                    // Get document width or height
-                    if (elem.nodeType === 9) {
-                        doc = elem.documentElement;
-
-                        // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
-                        // whichever is greatest
-                        return Math.max(
-                            elem.body["scroll" + name], doc["scroll" + name],
-                            elem.body["offset" + name], doc["offset" + name],
-                            doc["client" + name]
-                        );
-                    }
+                padding: "inner" + name,
+                content: type,
+                "": "outer" + name
+            },
+            function(defaultExtra, funcName) {
 
-                    return value === undefined ?
+                // Margin is only for outerHeight, outerWidth
+                jQuery.fn[funcName] = function(margin, value) {
+                    var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
+                        extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
+
+                    return access(this, function(elem, type, value) {
+                        var doc;
+
+                        if (isWindow(elem)) {
+
+                            // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
+                            return funcName.indexOf("outer") === 0 ?
+                                elem["inner" + name] :
+                                elem.document.documentElement["client" + name];
+                        }
+
+                        // Get document width or height
+                        if (elem.nodeType === 9) {
+                            doc = elem.documentElement;
+
+                            // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
+                            // whichever is greatest
+                            return Math.max(
+                                elem.body["scroll" + name], doc["scroll" + name],
+                                elem.body["offset" + name], doc["offset" + name],
+                                doc["client" + name]
+                            );
+                        }
 
-                        // Get width or height on the element, requesting but not forcing parseFloat
-                        jQuery.css(elem, type, extra) :
+                        return value === undefined ?
 
-                        // Set width or height on the element
-                        jQuery.style(elem, type, value, extra);
-                }, type, chainable ? margin : undefined, chainable);
-            };
-        });
+                            // Get width or height on the element, requesting but not forcing parseFloat
+                            jQuery.css(elem, type, extra) :
+
+                            // Set width or height on the element
+                            jQuery.style(elem, type, value, extra);
+                    }, type, chainable ? margin : undefined, chainable);
+                };
+            });
     });
 
 
     jQuery.each([
         "ajaxStart",
         "ajaxStop",
         "ajaxComplete",
@@ -10820,28 +10817,26 @@
         },
 
         hover: function(fnOver, fnOut) {
             return this.mouseenter(fnOver).mouseleave(fnOut || fnOver);
         }
     });
 
-    jQuery.each(
-        ("blur focus focusin focusout resize scroll click dblclick " +
+    jQuery.each(("blur focus focusin focusout resize scroll click dblclick " +
             "mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave " +
             "change select submit keydown keypress keyup contextmenu").split(" "),
         function(_i, name) {
 
             // Handle event binding
             jQuery.fn[name] = function(data, fn) {
                 return arguments.length > 0 ?
                     this.on(name, null, data, fn) :
                     this.trigger(name);
             };
-        }
-    );
+        });
 
 
 
 
     // Support: Android <=4.0 only
     // Make sure we trim BOM and NBSP
     var rtrim = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/jquery.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/jquery.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! jQuery v3.6.0 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(C, e) {
     "use strict";
@@ -19,15 +19,15 @@
         n = {},
         o = n.toString,
         v = n.hasOwnProperty,
         a = v.toString,
         l = a.call(Object),
         y = {},
         m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
+            return "function" == typeof e && "number" != typeof e.nodeType
         },
         x = function(e) {
             return null != e && e === e.window
         },
         E = C.document,
         c = {
             type: !0,
@@ -42,15 +42,15 @@
             for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
     function w(e) {
         return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
     }
-    var f = "3.6.0",
+    var f = "3.5.1",
         S = function(e, t) {
             return new S.fn.init(e, t)
         };
 
     function p(e) {
         var t = !!e && "length" in e && e.length,
             n = w(e);
@@ -182,18 +182,18 @@
             p = n.document,
             k = 0,
             r = 0,
             m = ue(),
             x = ue(),
             A = ue(),
             N = ue(),
-            j = function(e, t) {
+            D = function(e, t) {
                 return e === t && (l = !0), 0
             },
-            D = {}.hasOwnProperty,
+            j = {}.hasOwnProperty,
             t = [],
             q = t.pop,
             L = t.push,
             H = t.push,
             O = t.slice,
             P = function(e, t) {
                 for (var n = 0, r = e.length; n < r; n++)
@@ -360,16 +360,16 @@
             })
         }
 
         function ye(e) {
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
         for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e && e.namespaceURI,
-                    n = e && (e.ownerDocument || e).documentElement;
+                var t = e.namespaceURI,
+                    n = (e.ownerDocument || e).documentElement;
                 return !Y.test(t || n && n.nodeName || "HTML")
             }, T = se.setDocument = function(e) {
                 var t, n, r = e ? e.ownerDocument || e : p;
                 return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
                     return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
                 }), d.attributes = ce(function(e) {
                     return e.className = "i", !e.getAttribute("className")
@@ -431,15 +431,15 @@
                         r = t && t.parentNode;
                     return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
                 } : function(e, t) {
                     if (t)
                         while (t = t.parentNode)
                             if (t === e) return !0;
                     return !1
-                }, j = t ? function(e, t) {
+                }, D = t ? function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
                     return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && y(p, e) ? -1 : t == C || t.ownerDocument == p && y(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n, r = 0,
                         i = e.parentNode,
@@ -466,25 +466,25 @@
                 }
                 return 0 < se(t, C, null, [e]).length
             }, se.contains = function(e, t) {
                 return (e.ownerDocument || e) != C && T(e), y(e, t)
             }, se.attr = function(e, t) {
                 (e.ownerDocument || e) != C && T(e);
                 var n = b.attrHandle[t.toLowerCase()],
-                    r = n && D.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
+                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
                 return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
             }, se.escape = function(e) {
                 return (e + "").replace(re, ie)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
             }, se.uniqueSort = function(e) {
                 var t, n = [],
                     r = 0,
                     i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(j), l) {
+                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
                     while (t = e[i++]) t === e[i] && (r = n.push(i));
                     while (r--) e.splice(n[r], 1)
                 }
                 return u = null, e
             }, o = se.getText = function(e) {
                 var t, n = "",
                     r = 0,
@@ -880,15 +880,15 @@
                     if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
                         if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
             return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = S.split("").sort(j).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+        }, d.sortStable = S.split("").sort(D).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
             return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
         }), ce(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || fe("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), d.attributes && ce(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -918,15 +918,15 @@
         k = S.expr.match.needsContext;
 
     function A(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
     var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function j(e, n, r) {
+    function D(e, n, r) {
         return m(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
         }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== r
         }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < i.call(n, e) !== r
         }) : S.filter(n, e, r)
@@ -944,38 +944,38 @@
                 for (t = 0; t < r; t++)
                     if (S.contains(i[t], this)) return !0
             }));
             for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
             return 1 < r ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(j(this, e || [], !1))
+            return this.pushStack(D(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(j(this, e || [], !0))
+            return this.pushStack(D(this, e || [], !0))
         },
         is: function(e) {
-            return !!j(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
+            return !!D(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var D, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    var j, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
     (S.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || D, "string" == typeof e) {
+        if (n = n || j, "string" == typeof e) {
             if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
                 if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
                     for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
             return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
         return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
-    }).prototype = S.fn, D = S(E);
+    }).prototype = S.fn, j = S(E);
     var L = /^(?:parents|prev(?:Until|All))/,
         H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
@@ -1514,70 +1514,72 @@
             if (r && -1 < S.inArray(o, r)) i && i.push(o);
             else if (l = ie(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
             c = 0;
             while (o = a[c++]) he.test(o.type || "") && n.push(o)
         }
         return f
     }
-    var be = /^([^.]*)(?:\.(.+)|)/;
+    var be = /^key/,
+        we = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+        Te = /^([^.]*)(?:\.(.+)|)/;
 
-    function we() {
+    function Ce() {
         return !0
     }
 
-    function Te() {
+    function Ee() {
         return !1
     }
 
-    function Ce(e, t) {
+    function Se(e, t) {
         return e === function() {
             try {
                 return E.activeElement
             } catch (e) {}
         }() == ("focus" === t)
     }
 
-    function Ee(e, t, n, r, i, o) {
+    function ke(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ee(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) ke(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Te;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Ee;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
             return S().off(e), a.apply(this, arguments)
         }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
             S.event.add(this, t, i, r, n)
         })
     }
 
-    function Se(e, i, o) {
+    function Ae(e, i, o) {
         o ? (Y.set(e, i, !1), S.event.add(e, i, {
             namespace: !1,
             handler: function(e) {
                 var t, n, r = Y.get(this, i);
                 if (1 & e.isTrigger && this[i]) {
                     if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n && n.value
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
                 } else r.length && (Y.set(this, i, {
                     value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
                 }), e.stopImmediatePropagation())
             }
-        })) : void 0 === Y.get(e, i) && S.event.add(e, i, we)
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, Ce)
     }
     S.event = {
         global: {},
         add: function(t, e, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.get(t);
             if (V(t)) {
                 n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
                     return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
                 }), l = (e = (e || "").match(P) || [""]).length;
-                while (l--) d = g = (s = be.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                while (l--) d = g = (s = Te.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
                     needsContext: i && S.expr.match.needsContext.test(i),
@@ -1586,15 +1588,15 @@
             }
         },
         remove: function(e, t, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.hasData(e) && Y.get(e);
             if (v && (u = v.events)) {
                 l = (t = (t || "").match(P) || [""]).length;
                 while (l--)
-                    if (d = g = (s = be.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                    if (d = g = (s = Te.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
                         f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
                         a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                     } else
                         for (d in u) S.event.remove(e, d + t[l], n, r, !0);
                 S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
@@ -1656,19 +1658,19 @@
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click", we), !1
+                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click", Ce), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click"), !0
+                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
                     return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
@@ -1677,32 +1679,32 @@
                 }
             }
         }
     }, S.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
     }, S.Event = function(e, t) {
         if (!(this instanceof S.Event)) return new S.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? we : Te, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ce : Ee, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
     }, S.Event.prototype = {
         constructor: S.Event,
-        isDefaultPrevented: Te,
-        isPropagationStopped: Te,
-        isImmediatePropagationStopped: Te,
+        isDefaultPrevented: Ee,
+        isPropagationStopped: Ee,
+        isImmediatePropagationStopped: Ee,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = we, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = Ce, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = we, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = Ce, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = we, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = Ce, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
     }, S.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
@@ -1727,28 +1729,28 @@
         pointerId: !0,
         pointerType: !0,
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
-        which: !0
+        which: function(e) {
+            var t = e.button;
+            return null == e.which && be.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && we.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
+        }
     }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(e, t) {
         S.event.special[e] = {
             setup: function() {
-                return Se(this, e, Ce), !1
+                return Ae(this, e, Se), !1
             },
             trigger: function() {
-                return Se(this, e), !0
-            },
-            _default: function() {
-                return !0
+                return Ae(this, e), !0
             },
             delegateType: t
         }
     }), S.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
@@ -1761,95 +1763,95 @@
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
                 return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
     }), S.fn.extend({
         on: function(e, t, n, r) {
-            return Ee(this, e, t, n, r)
+            return ke(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return Ee(this, e, t, n, r, 1)
+            return ke(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
             if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Te), this.each(function() {
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ee), this.each(function() {
                 S.event.remove(this, e, n, t)
             })
         }
     });
-    var ke = /<script|<style|<link/i,
-        Ae = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        Ne = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var Ne = /<script|<style|<link/i,
+        De = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        je = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-    function je(e, t) {
+    function qe(e, t) {
         return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function De(e) {
+    function Le(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function qe(e) {
+    function He(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Le(e, t) {
+    function Oe(e, t) {
         var n, r, i, o, a, s;
         if (1 === t.nodeType) {
             if (Y.hasData(e) && (s = Y.get(e).events))
                 for (i in Y.remove(t, "handle events"), s)
                     for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
             Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function He(n, r, i, o) {
+    function Pe(n, r, i, o) {
         r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
             h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && Ae.test(d)) return n.each(function(e) {
+        if (h || 1 < f && "string" == typeof d && !y.checkClone && De.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), He(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), Pe(t, r, i, o)
         });
         if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = S.map(ve(e, "script"), De)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+            for (s = (a = S.map(ve(e, "script"), Le)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, S.map(a, qe), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, S.map(a, He), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }, l) : b(u.textContent.replace(Ne, ""), u, l))
+                }, l) : b(u.textContent.replace(je, ""), u, l))
         }
         return n
     }
 
-    function Oe(e, t, n) {
+    function Re(e, t, n) {
         for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ve(r)), r.parentNode && (n && ie(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
         return e
     }
     S.extend({
         htmlPrefilter: function(e) {
             return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
                 f = ie(e);
             if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Le(o[r], a[r]);
-                else Le(e, c);
+                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Oe(o[r], a[r]);
+                else Oe(e, c);
             return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
         },
         cleanData: function(e) {
             for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
                 if (V(n)) {
                     if (t = n[Y.expando]) {
                         if (t.events)
@@ -1857,46 +1859,46 @@
                         n[Y.expando] = void 0
                     }
                     n[Q.expando] && (n[Q.expando] = void 0)
                 }
         }
     }), S.fn.extend({
         detach: function(e) {
-            return Oe(this, e, !0)
+            return Re(this, e, !0)
         },
         remove: function(e) {
-            return Oe(this, e)
+            return Re(this, e)
         },
         text: function(e) {
             return $(this, function(e) {
                 return void 0 === e ? S.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return He(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || je(this, e).appendChild(e)
+            return Pe(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || qe(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return He(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = je(this, e);
+                    var t = qe(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return He(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return He(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
             for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ve(e, !1)), e.textContent = "");
             return this
         },
@@ -1907,27 +1909,27 @@
         },
         html: function(e) {
             return $(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !ke.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                if ("string" == typeof e && !Ne.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
                     e = S.htmlPrefilter(e);
                     try {
                         for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ve(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return He(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 var t = this.parentNode;
                 S.inArray(this, n) < 0 && (S.cleanData(ve(this)), t && t.replaceChild(e, this))
             }, n)
         }
     }), S.each({
         appendTo: "append",
         prependTo: "prepend",
@@ -1936,33 +1938,33 @@
         replaceAll: "replaceWith"
     }, function(e, a) {
         S.fn[e] = function(e) {
             for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var Pe = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
-        Re = function(e) {
+    var Me = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Ie = function(e) {
             var t = e.ownerDocument.defaultView;
             return t && t.opener || (t = C), t.getComputedStyle(e)
         },
-        Me = function(e, t, n) {
+        We = function(e, t, n) {
             var r, i, o = {};
             for (i in t) o[i] = e.style[i], e.style[i] = t[i];
             for (i in r = n.call(e), t) e.style[i] = o[i];
             return r
         },
-        Ie = new RegExp(ne.join("|"), "i");
+        Fe = new RegExp(ne.join("|"), "i");
 
-    function We(e, t, n) {
+    function Be(e, t, n) {
         var r, i, o, a, s = e.style;
-        return (n = n || Re(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Pe.test(a) && Ie.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+        return (n = n || Ie(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Me.test(a) && Fe.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function Fe(e, t) {
+    function $e(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
@@ -1993,79 +1995,79 @@
                 return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
             },
             reliableTrDimensions: function() {
                 var e, t, n, r;
-                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, re.removeChild(e)), a
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px", t.style.height = "1px", n.style.height = "9px", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = 3 < parseInt(r.height), re.removeChild(e)), a
             }
         }))
     }();
-    var Be = ["Webkit", "Moz", "ms"],
-        $e = E.createElement("div").style,
-        _e = {};
-
-    function ze(e) {
-        var t = S.cssProps[e] || _e[e];
-        return t || (e in $e ? e : _e[e] = function(e) {
+    var _e = ["Webkit", "Moz", "ms"],
+        ze = E.createElement("div").style,
+        Ue = {};
+
+    function Xe(e) {
+        var t = S.cssProps[e] || Ue[e];
+        return t || (e in ze ? e : Ue[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = Be.length;
+                n = _e.length;
             while (n--)
-                if ((e = Be[n] + t) in $e) return e
+                if ((e = _e[n] + t) in ze) return e
         }(e) || e)
     }
-    var Ue = /^(none|table(?!-c[ea]).+)/,
-        Xe = /^--/,
-        Ve = {
+    var Ve = /^(none|table(?!-c[ea]).+)/,
+        Ge = /^--/,
+        Ye = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Ge = {
+        Qe = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Ye(e, t, n) {
+    function Je(e, t, n) {
         var r = te.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function Qe(e, t, n, r, i, o) {
+    function Ke(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
             u = 0;
         if (n === (r ? "border" : "content")) return 0;
         for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
         return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function Je(e, t, n) {
-        var r = Re(e),
+    function Ze(e, t, n) {
+        var r = Ie(e),
             i = (!y.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
             o = i,
-            a = We(e, t, r),
+            a = Be(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if (Pe.test(a)) {
+        if (Me.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Qe(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function Ke(e, t, n, r, i) {
-        return new Ke.prototype.init(e, t, n, r, i)
+    function et(e, t, n, r, i) {
+        return new et.prototype.init(e, t, n, r, i)
     }
     S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = We(e, "opacity");
+                        var n = Be(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2089,152 +2091,152 @@
             zIndex: !0,
             zoom: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
                 var i, o, a, s = X(t),
-                    u = Xe.test(t),
+                    u = Ge.test(t),
                     l = e.style;
-                if (u || (t = ze(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                if (u || (t = Xe(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
                 "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
             var i, o, a, s = X(t);
-            return Xe.test(t) || (t = ze(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = We(e, t, r)), "normal" === i && t in Ge && (i = Ge[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            return Ge.test(t) || (t = Xe(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
     }), S.each(["height", "width"], function(e, u) {
         S.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ue.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Je(e, u, n) : Me(e, Ve, function() {
-                    return Je(e, u, n)
+                if (t) return !Ve.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : We(e, Ye, function() {
+                    return Ze(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Re(e),
+                var r, i = Ie(e),
                     o = !y.scrollboxSize() && "absolute" === i.position,
                     a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
-                    s = n ? Qe(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Qe(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Ye(0, t, s)
+                    s = n ? Ke(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
             }
         }
-    }), S.cssHooks.marginLeft = Fe(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(We(e, "marginLeft")) || e.getBoundingClientRect().left - Me(e, {
+    }), S.cssHooks.marginLeft = $e(y.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - We(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
     }), S.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
         S.cssHooks[i + o] = {
             expand: function(e) {
                 for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (S.cssHooks[i + o].set = Ye)
+        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
     }), S.fn.extend({
         css: function(e, t) {
             return $(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Re(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                    for (r = Ie(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                     return o
                 }
                 return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((S.Tween = Ke).prototype = {
-        constructor: Ke,
+    }), ((S.Tween = et).prototype = {
+        constructor: et,
         init: function(e, t, n, r, i, o) {
             this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = Ke.propHooks[this.prop];
-            return e && e.get ? e.get(this) : Ke.propHooks._default.get(this)
+            var e = et.propHooks[this.prop];
+            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = Ke.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : Ke.propHooks._default.set(this), this
+            var t, n = et.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
         }
-    }).init.prototype = Ke.prototype, (Ke.propHooks = {
+    }).init.prototype = et.prototype, (et.propHooks = {
         _default: {
             get: function(e) {
                 var t;
                 return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[ze(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Xe(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = Ke.propHooks.scrollLeft = {
+    }).scrollTop = et.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
     }, S.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, S.fx = Ke.prototype.init, S.fx.step = {};
-    var Ze, et, tt, nt, rt = /^(?:toggle|show|hide)$/,
-        it = /queueHooks$/;
+    }, S.fx = et.prototype.init, S.fx.step = {};
+    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
+        at = /queueHooks$/;
 
-    function ot() {
-        et && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(ot) : C.setTimeout(ot, S.fx.interval), S.fx.tick())
+    function st() {
+        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
     }
 
-    function at() {
+    function ut() {
         return C.setTimeout(function() {
-            Ze = void 0
-        }), Ze = Date.now()
+            tt = void 0
+        }), tt = Date.now()
     }
 
-    function st(e, t) {
+    function lt(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
         for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function ut(e, t, n) {
-        for (var r, i = (lt.tweeners[t] || []).concat(lt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function ct(e, t, n) {
+        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function lt(o, e, t) {
+    function ft(o, e, t) {
         var n, a, r = 0,
-            i = lt.prefilters.length,
+            i = ft.prefilters.length,
             s = S.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = Ze || at(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
                 props: S.extend({}, e),
                 opts: S.extend(!0, {
                     specialEasing: {},
                     easing: S.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: Ze || at(),
+                startTime: tt || ut(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
                     var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
@@ -2249,31 +2251,31 @@
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
                     if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = lt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return S.map(c, ut, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    S.Animation = S.extend(lt, {
+    S.Animation = S.extend(ft, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
                 return se(n.elem, e, te.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
             m(e) ? (t = e, e = ["*"]) : e = e.match(P);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], lt.tweeners[n] = lt.tweeners[n] || [], lt.tweeners[n].unshift(t)
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
                 g = e.nodeType && ae(e),
@@ -2281,33 +2283,33 @@
             for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
                         a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], rt.test(i)) {
+                if (i = t[r], ot.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
                     d[r] = v && v[r] || S.style(e, r)
                 } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
                 for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
                     })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Y.access(e, "fxshow", {
                     display: l
                 }), o && (v.hidden = !g), g && le([e], !0), p.done(function() {
                     for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
-                })), u = ut(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                })), u = ct(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? lt.prefilters.unshift(e) : lt.prefilters.push(e)
+            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
         }
     }), S.speed = function(e, t, n) {
         var r = e && "object" == typeof e ? S.extend({}, e) : {
             complete: n || !n && t || m(e) && e,
             duration: e,
             easing: n && t || t && !m(t) && t
         };
@@ -2320,15 +2322,15 @@
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
             var i = S.isEmptyObject(t),
                 o = S.speed(e, n, r),
                 a = function() {
-                    var e = lt(this, S.extend({}, t), o);
+                    var e = ft(this, S.extend({}, t), o);
                     (i || Y.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
@@ -2337,15 +2339,15 @@
             return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
                     n = S.timers,
                     r = Y.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && it.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
                 !e && o || S.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
                 var e, t = Y.get(this),
@@ -2357,20 +2359,20 @@
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
     }), S.each(["toggle", "show", "hide"], function(e, r) {
         var i = S.fn[r];
         S.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(st(r, !0), e, t, n)
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
         }
     }), S.each({
-        slideDown: st("show"),
-        slideUp: st("hide"),
-        slideToggle: st("toggle"),
+        slideDown: lt("show"),
+        slideUp: lt("hide"),
+        slideToggle: lt("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
@@ -2379,48 +2381,48 @@
     }, function(e, r) {
         S.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
     }), S.timers = [], S.fx.tick = function() {
         var e, t = 0,
             n = S.timers;
-        for (Ze = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || S.fx.stop(), Ze = void 0
+        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), tt = void 0
     }, S.fx.timer = function(e) {
         S.timers.push(e), S.fx.start()
     }, S.fx.interval = 13, S.fx.start = function() {
-        et || (et = !0, ot())
+        nt || (nt = !0, st())
     }, S.fx.stop = function() {
-        et = null
+        nt = null
     }, S.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
     }, S.fn.delay = function(r, e) {
         return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
             var n = C.setTimeout(e, r);
             t.stop = function() {
                 C.clearTimeout(n)
             }
         })
-    }, tt = E.createElement("input"), nt = E.createElement("select").appendChild(E.createElement("option")), tt.type = "checkbox", y.checkOn = "" !== tt.value, y.optSelected = nt.selected, (tt = E.createElement("input")).value = "t", tt.type = "radio", y.radioValue = "t" === tt.value;
-    var ct, ft = S.expr.attrHandle;
+    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", y.checkOn = "" !== rt.value, y.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", y.radioValue = "t" === rt.value;
+    var pt, dt = S.expr.attrHandle;
     S.fn.extend({
         attr: function(e, t) {
             return $(this, S.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
                 S.removeAttr(this, e)
             })
         }
     }), S.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? ct : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
                     if (!y.radioValue && "radio" === t && A(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
@@ -2430,37 +2432,37 @@
         },
         removeAttr: function(e, t) {
             var n, r = 0,
                 i = t && t.match(P);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), ct = {
+    }), pt = {
         set: function(e, t, n) {
             return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
     }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = ft[t] || S.find.attr;
-        ft[t] = function(e, t, n) {
+        var a = dt[t] || S.find.attr;
+        dt[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = ft[o], ft[o] = r, r = null != a(e, t, n) ? o : null, ft[o] = i), r
+            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
         }
     });
-    var pt = /^(?:input|select|textarea|button)$/i,
-        dt = /^(?:a|area)$/i;
+    var ht = /^(?:input|select|textarea|button)$/i,
+        gt = /^(?:a|area)$/i;
 
-    function ht(e) {
+    function vt(e) {
         return (e.match(P) || []).join(" ")
     }
 
-    function gt(e) {
+    function yt(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function vt(e) {
+    function mt(e) {
         return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
     }
     S.fn.extend({
         prop: function(e, t) {
             return $(this, S.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
@@ -2473,15 +2475,15 @@
             var r, i, o = e.nodeType;
             if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
                     var t = S.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : pt.test(e.nodeName) || dt.test(e.nodeName) && e.href ? 0 : -1
+                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
@@ -2496,77 +2498,77 @@
         }
     }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
         S.propFix[this.toLowerCase()] = this
     }), S.fn.extend({
         addClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).addClass(t.call(this, e, gt(this)))
+                S(this).addClass(t.call(this, e, yt(this)))
             });
-            if ((e = vt(t)).length)
+            if ((e = mt(t)).length)
                 while (n = this[u++])
-                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
+                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
                         a = 0;
                         while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = ht(r)) && n.setAttribute("class", s)
+                        i !== (s = vt(r)) && n.setAttribute("class", s)
                     } return this
         },
         removeClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).removeClass(t.call(this, e, gt(this)))
+                S(this).removeClass(t.call(this, e, yt(this)))
             });
             if (!arguments.length) return this.attr("class", "");
-            if ((e = vt(t)).length)
+            if ((e = mt(t)).length)
                 while (n = this[u++])
-                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
+                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
                         a = 0;
                         while (o = e[a++])
                             while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = ht(r)) && n.setAttribute("class", s)
+                        i !== (s = vt(r)) && n.setAttribute("class", s)
                     } return this
         },
         toggleClass: function(i, t) {
             var o = typeof i,
                 a = "string" === o || Array.isArray(i);
             return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                S(this).toggleClass(i.call(this, e, gt(this), t), t)
+                S(this).toggleClass(i.call(this, e, yt(this), t), t)
             }) : this.each(function() {
                 var e, t, n, r;
                 if (a) {
-                    t = 0, n = S(this), r = vt(i);
+                    t = 0, n = S(this), r = mt(i);
                     while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = gt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
+                } else void 0 !== i && "boolean" !== o || ((e = yt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
             })
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + ht(gt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + vt(yt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var yt = /\r/g;
+    var xt = /\r/g;
     S.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
             return arguments.length ? (i = m(n), this.each(function(e) {
                 var t;
                 1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
                 })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(yt, "") : null == e ? "" : e : void 0
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
         }
     }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
                     var t = S.find.attr(e, "value");
-                    return null != t ? t : ht(S.text(e))
+                    return null != t ? t : vt(S.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
@@ -2592,31 +2594,31 @@
             set: function(e, t) {
                 if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
         }, y.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), y.focusin = "onfocusin" in C;
-    var mt = /^(?:focusinfocus|focusoutblur)$/,
-        xt = function(e) {
+    var bt = /^(?:focusinfocus|focusoutblur)$/,
+        wt = function(e) {
             e.stopPropagation()
         };
     S.extend(S.event, {
         trigger: function(e, t, n, r) {
             var i, o, a, s, u, l, c, f, p = [n || E],
                 d = v.call(e, "type") ? e.type : e,
                 h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !mt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
                 if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, mt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
                     a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
                 }
                 i = 0;
                 while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, xt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, xt), S.event.triggered = void 0, a && (n[u] = a)), e.result
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
             var r = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
@@ -2648,135 +2650,135 @@
             teardown: function() {
                 var e = this.ownerDocument || this.document || this,
                     t = Y.access(e, r) - 1;
                 t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
             }
         }
     });
-    var bt = C.location,
-        wt = {
+    var Tt = C.location,
+        Ct = {
             guid: Date.now()
         },
-        Tt = /\?/;
+        Et = /\?/;
     S.parseXML = function(e) {
-        var t, n;
+        var t;
         if (!e || "string" != typeof e) return null;
         try {
             t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {}
-        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, function(e) {
-            return e.textContent
-        }).join("\n") : e)), t
+        } catch (e) {
+            t = void 0
+        }
+        return t && !t.getElementsByTagName("parsererror").length || S.error("Invalid XML: " + e), t
     };
-    var Ct = /\[\]$/,
-        Et = /\r?\n/g,
-        St = /^(?:submit|button|image|reset|file)$/i,
-        kt = /^(?:input|select|textarea|keygen)/i;
+    var St = /\[\]$/,
+        kt = /\r?\n/g,
+        At = /^(?:submit|button|image|reset|file)$/i,
+        Nt = /^(?:input|select|textarea|keygen)/i;
 
-    function At(n, e, r, i) {
+    function Dt(n, e, r, i) {
         var t;
         if (Array.isArray(e)) S.each(e, function(e, t) {
-            r || Ct.test(n) ? i(n, t) : At(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+            r || St.test(n) ? i(n, t) : Dt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
         else if (r || "object" !== w(e)) i(n, e);
         else
-            for (t in e) At(n + "[" + t + "]", e[t], r, i)
+            for (t in e) Dt(n + "[" + t + "]", e[t], r, i)
     }
     S.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
                 var n = m(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
         if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) At(n, e[n], t, i);
+            for (n in e) Dt(n, e[n], t, i);
         return r.join("&")
     }, S.fn.extend({
         serialize: function() {
             return S.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
                 var e = S.prop(this, "elements");
                 return e ? S.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !S(this).is(":disabled") && kt.test(this.nodeName) && !St.test(e) && (this.checked || !pe.test(e))
+                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
             }).map(function(e, t) {
                 var n = S(this).val();
                 return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(Et, "\r\n")
+                        value: e.replace(kt, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(Et, "\r\n")
+                    value: n.replace(kt, "\r\n")
                 }
             }).get()
         }
     });
-    var Nt = /%20/g,
-        jt = /#.*$/,
-        Dt = /([?&])_=[^&]*/,
-        qt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Lt = /^(?:GET|HEAD)$/,
-        Ht = /^\/\//,
-        Ot = {},
-        Pt = {},
-        Rt = "*/".concat("*"),
-        Mt = E.createElement("a");
+    var jt = /%20/g,
+        qt = /#.*$/,
+        Lt = /([?&])_=[^&]*/,
+        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Ot = /^(?:GET|HEAD)$/,
+        Pt = /^\/\//,
+        Rt = {},
+        Mt = {},
+        It = "*/".concat("*"),
+        Wt = E.createElement("a");
 
-    function It(o) {
+    function Ft(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
                 i = e.toLowerCase().match(P) || [];
             if (m(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function Wt(t, i, o, a) {
+    function Bt(t, i, o, a) {
         var s = {},
-            u = t === Pt;
+            u = t === Mt;
 
         function l(e) {
             var r;
             return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function Ft(e, t) {
+    function $t(e, t) {
         var n, r, i = S.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
         return r && S.extend(!0, e, r), e
     }
-    Mt.href = bt.href, S.extend({
+    Wt.href = Tt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: bt.href,
+            url: Tt.href,
             type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(bt.protocol),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": Rt,
+                "*": It,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2796,18 +2798,18 @@
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? Ft(Ft(e, S.ajaxSettings), t) : Ft(S.ajaxSettings, e)
+            return t ? $t($t(e, S.ajaxSettings), t) : $t(S.ajaxSettings, e)
         },
-        ajaxPrefilter: It(Ot),
-        ajaxTransport: It(Pt),
+        ajaxPrefilter: Ft(Rt),
+        ajaxTransport: Ft(Mt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
             var c, f, p, n, d, r, h, g, i, o, v = S.ajaxSetup({}, t),
                 y = v.context || v,
                 m = v.context && (y.nodeType || y.jquery) ? S(y) : S.event,
                 x = S.Deferred(),
                 b = S.Callbacks("once memory"),
@@ -2818,15 +2820,15 @@
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = qt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2846,26 +2848,26 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || bt.href) + "").replace(Ht, bt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
+            if (x.promise(T), v.url = ((e || v.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
                 r = E.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Mt.protocol + "//" + Mt.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Wt(Ot, v, t, T), h) return T;
-            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Lt.test(v.type), f = v.url.replace(jt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Nt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Tt.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Dt, "$1"), o = (Tt.test(f) ? "&" : "?") + "_=" + wt.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + Rt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Bt(Rt, v, t, T), h) return T;
+            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ot.test(v.type), f = v.url.replace(qt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(jt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Et.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + It + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Wt(Pt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Bt(Mt, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
                 v.async && 0 < v.timeout && (d = C.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
@@ -2893,15 +2895,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && S.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -2999,30 +3001,30 @@
     }, S.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
     }, S.ajaxSettings.xhr = function() {
         try {
             return new C.XMLHttpRequest
         } catch (e) {}
     };
-    var Bt = {
+    var _t = {
             0: 200,
             1223: 204
         },
-        $t = S.ajaxSettings.xhr();
-    y.cors = !!$t && "withCredentials" in $t, y.ajax = $t = !!$t, S.ajaxTransport(function(i) {
+        zt = S.ajaxSettings.xhr();
+    y.cors = !!zt && "withCredentials" in zt, y.ajax = zt = !!zt, S.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || $t && !i.crossDomain) return {
+        if (y.cors || zt && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Bt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
                     4 === r.readyState && C.setTimeout(function() {
@@ -3067,38 +3069,38 @@
                 }), E.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var _t, zt = [],
-        Ut = /(=)\?(?=&|$)|\?\?/;
+    var Ut, Xt = [],
+        Vt = /(=)\?(?=&|$)|\?\?/;
     S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = zt.pop() || S.expando + "_" + wt.guid++;
+            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
             return this[e] = !0, e
         }
     }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Ut.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Ut.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Ut, "$1" + r) : !1 !== e.jsonp && (e.url += (Tt.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
             return o || S.error(r + " was not called"), o[0]
         }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, zt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((_t = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === _t.childNodes.length), S.parseHTML = function(e, t, n) {
+    }), y.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
         return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
         var r, i, o
     }, S.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = ht(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
+        return -1 < s && (r = vt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
             o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
@@ -3111,15 +3113,15 @@
             return t === e.elem
         }).length
     }, S.offset = {
         setOffset: function(e, t, n) {
             var r, i, o, a, s, u, l = S.css(e, "position"),
                 c = S(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : ("number" == typeof f.top && (f.top += "px"), "number" == typeof f.left && (f.left += "px"), c.css(f))
         }
     }, S.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
                 S.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
@@ -3166,16 +3168,16 @@
             return $(this, function(e, t, n) {
                 var r;
                 if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
     }), S.each(["top", "left"], function(e, n) {
-        S.cssHooks[n] = Fe(y.pixelPosition, function(e, t) {
-            if (t) return t = We(e, n), Pe.test(t) ? S(e).position()[n] + "px" : t
+        S.cssHooks[n] = $e(y.pixelPosition, function(e, t) {
+            if (t) return t = Be(e, n), Me.test(t) ? S(e).position()[n] + "px" : t
         })
     }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
         S.each({
             padding: "inner" + a,
@@ -3212,29 +3214,29 @@
             return this.mouseenter(e).mouseleave(t || e)
         }
     }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
         S.fn[n] = function(e, t) {
             return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
         }
     });
-    var Xt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var Gt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
     S.proxy = function(e, t) {
         var n, r, i;
         if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
             return e.apply(t || this, r.concat(s.call(arguments)))
         }).guid = e.guid = e.guid || S.guid++, i
     }, S.holdReady = function(e) {
         e ? S.readyWait++ : S.ready(!0)
     }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
         var t = S.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
     }, S.trim = function(e) {
-        return null == e ? "" : (e + "").replace(Xt, "")
+        return null == e ? "" : (e + "").replace(Gt, "")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
         return S
     });
-    var Vt = C.jQuery,
-        Gt = C.$;
+    var Yt = C.jQuery,
+        Qt = C.$;
     return S.noConflict = function(e) {
-        return C.$ === S && (C.$ = Gt), e && C.jQuery === S && (C.jQuery = Vt), S
+        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
     }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/js/badge_only.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/js/html5shiv-printshiv.min.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/js/html5shiv.min.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/js/theme.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/pygments.css` & `Orange3-Explain-0.6.3/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/_static/searchtools.js` & `Orange3-Explain-0.6.3/doc/_build/html/_static/searchtools.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,577 +1,539 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2020 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
-"use strict";
 
-/**
- * Simple result scoring code.
- */
-if (typeof Scorer === "undefined") {
+if (!Scorer) {
+    /**
+     * Simple result scoring code.
+     */
     var Scorer = {
         // Implement the following function to further tweak the score for each result
-        // The function takes a result array [docname, title, anchor, descr, score, filename]
+        // The function takes a result array [filename, title, anchor, descr, score]
         // and returns the new score.
         /*
-        score: result => {
-          const [docname, title, anchor, descr, score, filename] = result
-          return score
+        score: function(result) {
+          return result[4];
         },
         */
 
         // query matches the full name of an object
         objNameMatch: 11,
         // or matches in the last dotted part of the object name
         objPartialMatch: 6,
         // Additive scores depending on the priority of the object
         objPrio: {
             0: 15, // used to be importantResults
             1: 5, // used to be objectResults
-            2: -5, // used to be unimportantResults
-        },
+            2: -5
+        }, // used to be unimportantResults
         //  Used when the priority is not in the mapping.
         objPrioDefault: 0,
 
         // query found in title
         title: 15,
         partialTitle: 7,
         // query found in terms
         term: 5,
-        partialTerm: 2,
+        partialTerm: 2
     };
 }
 
-const _removeChildren = (element) => {
-    while (element && element.lastChild) element.removeChild(element.lastChild);
-};
-
-/**
- * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
- */
-const _escapeRegExp = (string) =>
-    string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
-
-const _displayItem = (item, searchTerms) => {
-    const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
-    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
-    const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
-    const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
-    const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
-
-    const [docName, title, anchor, descr, score, _filename] = item;
-
-    let listItem = document.createElement("li");
-    let requestUrl;
-    let linkUrl;
-    if (docBuilder === "dirhtml") {
-        // dirhtml builder
-        let dirname = docName + "/";
-        if (dirname.match(/\/index\/$/))
-            dirname = dirname.substring(0, dirname.length - 6);
-        else if (dirname === "index/") dirname = "";
-        requestUrl = docUrlRoot + dirname;
-        linkUrl = requestUrl;
-    } else {
-        // normal html builders
-        requestUrl = docUrlRoot + docName + docFileSuffix;
-        linkUrl = docName + docLinkSuffix;
+if (!splitQuery) {
+    function splitQuery(query) {
+        return query.split(/\s+/);
     }
-    let linkEl = listItem.appendChild(document.createElement("a"));
-    linkEl.href = linkUrl + anchor;
-    linkEl.dataset.score = score;
-    linkEl.innerHTML = title;
-    if (descr)
-        listItem.appendChild(document.createElement("span")).innerHTML =
-        " (" + descr + ")";
-    else if (showSearchSummary)
-        fetch(requestUrl)
-        .then((responseData) => responseData.text())
-        .then((data) => {
-            if (data)
-                listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms)
-                );
-        });
-    Search.output.appendChild(listItem);
-};
-const _finishSearch = (resultCount) => {
-    Search.stopPulse();
-    Search.title.innerText = _("Search Results");
-    if (!resultCount)
-        Search.status.innerText = Documentation.gettext(
-            "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
-        );
-    else
-        Search.status.innerText = _(
-            `Search finished, found ${resultCount} page(s) matching the search query.`
-        );
-};
-const _displayNextItem = (
-    results,
-    resultCount,
-    searchTerms
-) => {
-    // results left, load the summary and display it
-    // this is intended to be dynamic (don't sub resultsCount)
-    if (results.length) {
-        _displayItem(results.pop(), searchTerms);
-        setTimeout(
-            () => _displayNextItem(results, resultCount, searchTerms),
-            5
-        );
-    }
-    // search finished, update title and status message
-    else _finishSearch(resultCount);
-};
-
-/**
- * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
- * custom function per language.
- *
- * The regular expression works by splitting the string on consecutive characters
- * that are not Unicode letters, numbers, underscores, or emoji characters.
- * This is the same as ``\W+`` in Python, preserving the surrogate pair area.
- */
-if (typeof splitQuery === "undefined") {
-    var splitQuery = (query) => query
-        .split(/[^\p{Letter}\p{Number}_\p{Emoji_Presentation}]+/gu)
-        .filter(term => term) // remove remaining empty strings
 }
 
 /**
  * Search Module
  */
-const Search = {
+var Search = {
+
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: (htmlString) => {
-        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
-        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
-            el.remove()
-        });
-        const docContent = htmlElement.querySelector('[role="main"]');
-        if (docContent !== undefined) return docContent.textContent;
-        console.warn(
-            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
-        );
-        return "";
+    htmlToText: function(htmlString) {
+        var virtualDocument = document.implementation.createHTMLDocument('virtual');
+        var htmlElement = $(htmlString, virtualDocument);
+        htmlElement.find('.headerlink').remove();
+        docContent = htmlElement.find('[role=main]')[0];
+        if (docContent === undefined) {
+            console.warn("Content block not found. Sphinx search tries to obtain it " +
+                "via '[role=main]'. Could you check your theme or template.");
+            return "";
+        }
+        return docContent.textContent || docContent.innerText;
     },
 
-    init: () => {
-        const query = new URLSearchParams(window.location.search).get("q");
-        document
-            .querySelectorAll('input[name="q"]')
-            .forEach((el) => (el.value = query));
-        if (query) Search.performSearch(query);
+    init: function() {
+        var params = $.getQueryParameters();
+        if (params.q) {
+            var query = params.q[0];
+            $('input[name="q"]')[0].value = query;
+            this.performSearch(query);
+        }
     },
 
-    loadIndex: (url) =>
-        (document.body.appendChild(document.createElement("script")).src = url),
+    loadIndex: function(url) {
+        $.ajax({
+            type: "GET",
+            url: url,
+            data: null,
+            dataType: "script",
+            cache: true,
+            complete: function(jqxhr, textstatus) {
+                if (textstatus != "success") {
+                    document.getElementById("searchindexloader").src = url;
+                }
+            }
+        });
+    },
 
-    setIndex: (index) => {
-        Search._index = index;
-        if (Search._queued_query !== null) {
-            const query = Search._queued_query;
-            Search._queued_query = null;
-            Search.query(query);
+    setIndex: function(index) {
+        var q;
+        this._index = index;
+        if ((q = this._queued_query) !== null) {
+            this._queued_query = null;
+            Search.query(q);
         }
     },
 
-    hasIndex: () => Search._index !== null,
+    hasIndex: function() {
+        return this._index !== null;
+    },
 
-    deferQuery: (query) => (Search._queued_query = query),
+    deferQuery: function(query) {
+        this._queued_query = query;
+    },
 
-    stopPulse: () => (Search._pulse_status = -1),
+    stopPulse: function() {
+        this._pulse_status = 0;
+    },
 
-    startPulse: () => {
-        if (Search._pulse_status >= 0) return;
+    startPulse: function() {
+        if (this._pulse_status >= 0)
+            return;
 
-        const pulse = () => {
+        function pulse() {
+            var i;
             Search._pulse_status = (Search._pulse_status + 1) % 4;
-            Search.dots.innerText = ".".repeat(Search._pulse_status);
-            if (Search._pulse_status >= 0) window.setTimeout(pulse, 500);
-        };
+            var dotString = '';
+            for (i = 0; i < Search._pulse_status; i++)
+                dotString += '.';
+            Search.dots.text(dotString);
+            if (Search._pulse_status > -1)
+                window.setTimeout(pulse, 500);
+        }
         pulse();
     },
 
     /**
      * perform a search for something (or wait until index is loaded)
      */
-    performSearch: (query) => {
+    performSearch: function(query) {
         // create the required interface elements
-        const searchText = document.createElement("h2");
-        searchText.textContent = _("Searching");
-        const searchSummary = document.createElement("p");
-        searchSummary.classList.add("search-summary");
-        searchSummary.innerText = "";
-        const searchList = document.createElement("ul");
-        searchList.classList.add("search");
-
-        const out = document.getElementById("search-results");
-        Search.title = out.appendChild(searchText);
-        Search.dots = Search.title.appendChild(document.createElement("span"));
-        Search.status = out.appendChild(searchSummary);
-        Search.output = out.appendChild(searchList);
-
-        const searchProgress = document.getElementById("search-progress");
-        // Some themes don't use the search progress node
-        if (searchProgress) {
-            searchProgress.innerText = _("Preparing search...");
-        }
-        Search.startPulse();
+        this.out = $('#search-results');
+        this.title = $('<h2>' + _('Searching') + '</h2>').appendTo(this.out);
+        this.dots = $('<span></span>').appendTo(this.title);
+        this.status = $('<p class="search-summary">&nbsp;</p>').appendTo(this.out);
+        this.output = $('<ul class="search"/>').appendTo(this.out);
+
+        $('#search-progress').text(_('Preparing search...'));
+        this.startPulse();
 
         // index already loaded, the browser was quick!
-        if (Search.hasIndex()) Search.query(query);
-        else Search.deferQuery(query);
+        if (this.hasIndex())
+            this.query(query);
+        else
+            this.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
-    query: (query) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-        const allTitles = Search._index.alltitles;
-        const indexEntries = Search._index.indexentries;
-
-        // stem the search terms and add them to the correct list
-        const stemmer = new Stemmer();
-        const searchTerms = new Set();
-        const excludedTerms = new Set();
-        const highlightTerms = new Set();
-        const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
-        splitQuery(query.trim()).forEach((queryTerm) => {
-            const queryTermLower = queryTerm.toLowerCase();
+    query: function(query) {
+        var i;
 
-            // maybe skip this "word"
-            // stopwords array is from language_data.js
-            if (
-                stopwords.indexOf(queryTermLower) !== -1 ||
-                queryTerm.match(/^\d+$/)
-            )
-                return;
+        // stem the searchterms and add them to the correct list
+        var stemmer = new Stemmer();
+        var searchterms = [];
+        var excluded = [];
+        var hlterms = [];
+        var tmp = splitQuery(query);
+        var objectterms = [];
+        for (i = 0; i < tmp.length; i++) {
+            if (tmp[i] !== "") {
+                objectterms.push(tmp[i].toLowerCase());
+            }
 
+            if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i] === "") {
+                // skip this "word"
+                continue;
+            }
             // stem the word
-            let word = stemmer.stemWord(queryTermLower);
+            var word = stemmer.stemWord(tmp[i].toLowerCase());
+            // prevent stemmer from cutting word smaller than two chars
+            if (word.length < 3 && tmp[i].length >= 3) {
+                word = tmp[i];
+            }
+            var toAppend;
             // select the correct list
-            if (word[0] === "-") excludedTerms.add(word.substr(1));
-            else {
-                searchTerms.add(word);
-                highlightTerms.add(queryTermLower);
+            if (word[0] == '-') {
+                toAppend = excluded;
+                word = word.substr(1);
+            } else {
+                toAppend = searchterms;
+                hlterms.push(tmp[i].toLowerCase());
             }
-        });
-
-        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
-            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+            // only add if not already in the list
+            if (!$u.contains(toAppend, word))
+                toAppend.push(word);
         }
+        var highlightstring = '?highlight=' + $.urlencode(hlterms.join(" "));
 
-        // console.debug("SEARCH: searching for:");
-        // console.info("required: ", [...searchTerms]);
-        // console.info("excluded: ", [...excludedTerms]);
-
-        // array of [docname, title, anchor, descr, score, filename]
-        let results = [];
-        _removeChildren(document.getElementById("search-progress"));
-
-        const queryLower = query.toLowerCase();
-        for (const [title, foundTitles] of Object.entries(allTitles)) {
-            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
-                for (const [file, id] of foundTitles) {
-                    let score = Math.round(100 * queryLower.length / title.length)
-                    results.push([
-                        docNames[file],
-                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
-                        id !== null ? "#" + id : "",
-                        null,
-                        score,
-                        filenames[file],
-                    ]);
-                }
-            }
-        }
+        // console.debug('SEARCH: searching for:');
+        // console.info('required: ', searchterms);
+        // console.info('excluded: ', excluded);
 
-        // search for explicit entries in index directives
-        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
-            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
-                for (const [file, id] of foundEntries) {
-                    let score = Math.round(100 * queryLower.length / entry.length)
-                    results.push([
-                        docNames[file],
-                        titles[file],
-                        id ? "#" + id : "",
-                        null,
-                        score,
-                        filenames[file],
-                    ]);
-                }
-            }
-        }
+        // prepare search
+        var terms = this._index.terms;
+        var titleterms = this._index.titleterms;
+
+        // array of [filename, title, anchor, descr, score]
+        var results = [];
+        $('#search-progress').empty();
 
         // lookup as object
-        objectTerms.forEach((term) =>
-            results.push(...Search.performObjectSearch(term, objectTerms))
-        );
+        for (i = 0; i < objectterms.length; i++) {
+            var others = [].concat(objectterms.slice(0, i),
+                objectterms.slice(i + 1, objectterms.length));
+            results = results.concat(this.performObjectSearch(objectterms[i], others));
+        }
 
         // lookup as search terms in fulltext
-        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
+        results = results.concat(this.performTermsSearch(searchterms, excluded, terms, titleterms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
+        if (Scorer.score) {
+            for (i = 0; i < results.length; i++)
+                results[i][4] = Scorer.score(results[i]);
+        }
 
         // now sort the results by score (in opposite order of appearance, since the
         // display function below uses pop() to retrieve items) and then
         // alphabetically
-        results.sort((a, b) => {
-            const leftScore = a[4];
-            const rightScore = b[4];
-            if (leftScore === rightScore) {
+        results.sort(function(a, b) {
+            var left = a[4];
+            var right = b[4];
+            if (left > right) {
+                return 1;
+            } else if (left < right) {
+                return -1;
+            } else {
                 // same score: sort alphabetically
-                const leftTitle = a[1].toLowerCase();
-                const rightTitle = b[1].toLowerCase();
-                if (leftTitle === rightTitle) return 0;
-                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
+                left = a[1].toLowerCase();
+                right = b[1].toLowerCase();
+                return (left > right) ? -1 : ((left < right) ? 1 : 0);
             }
-            return leftScore > rightScore ? 1 : -1;
         });
 
-        // remove duplicate search results
-        // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
-        let seen = new Set();
-        results = results.reverse().reduce((acc, result) => {
-            let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
-            if (!seen.has(resultStr)) {
-                acc.push(result);
-                seen.add(resultStr);
-            }
-            return acc;
-        }, []);
-
-        results = results.reverse();
-
         // for debugging
         //Search.lastresults = results.slice();  // a copy
-        // console.info("search results:", Search.lastresults);
+        //console.info('search results:', Search.lastresults);
 
         // print the results
-        _displayNextItem(results, results.length, searchTerms);
+        var resultCount = results.length;
+
+        function displayNextItem() {
+            // results left, load the summary and display it
+            if (results.length) {
+                var item = results.pop();
+                var listItem = $('<li style="display:none"></li>');
+                var requestUrl = "";
+                var linkUrl = "";
+                if (DOCUMENTATION_OPTIONS.BUILDER === 'dirhtml') {
+                    // dirhtml builder
+                    var dirname = item[0] + '/';
+                    if (dirname.match(/\/index\/$/)) {
+                        dirname = dirname.substring(0, dirname.length - 6);
+                    } else if (dirname == 'index/') {
+                        dirname = '';
+                    }
+                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + dirname;
+                    linkUrl = requestUrl;
+
+                } else {
+                    // normal html builders
+                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX;
+                    linkUrl = item[0] + DOCUMENTATION_OPTIONS.LINK_SUFFIX;
+                }
+                listItem.append($('<a/>').attr('href',
+                    linkUrl +
+                    highlightstring + item[2]).html(item[1]));
+                if (item[3]) {
+                    listItem.append($('<span> (' + item[3] + ')</span>'));
+                    Search.output.append(listItem);
+                    listItem.slideDown(5, function() {
+                        displayNextItem();
+                    });
+                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
+                    $.ajax({
+                        url: requestUrl,
+                        dataType: "text",
+                        complete: function(jqxhr, textstatus) {
+                            var data = jqxhr.responseText;
+                            if (data !== '' && data !== undefined) {
+                                listItem.append(Search.makeSearchSummary(data, searchterms, hlterms));
+                            }
+                            Search.output.append(listItem);
+                            listItem.slideDown(5, function() {
+                                displayNextItem();
+                            });
+                        }
+                    });
+                } else {
+                    // no source available, just display title
+                    Search.output.append(listItem);
+                    listItem.slideDown(5, function() {
+                        displayNextItem();
+                    });
+                }
+            }
+            // search finished, update title and status message
+            else {
+                Search.stopPulse();
+                Search.title.text(_('Search Results'));
+                if (!resultCount)
+                    Search.status.text(_('Your search did not match any documents. Please make sure that all words are spelled correctly and that you\'ve selected enough categories.'));
+                else
+                    Search.status.text(_('Search finished, found %s page(s) matching the search query.').replace('%s', resultCount));
+                Search.status.fadeIn(500);
+            }
+        }
+        displayNextItem();
     },
 
     /**
      * search for object names
      */
-    performObjectSearch: (object, objectTerms) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const objects = Search._index.objects;
-        const objNames = Search._index.objnames;
-        const titles = Search._index.titles;
-
-        const results = [];
-
-        const objectSearchCallback = (prefix, match) => {
-            const name = match[4]
-            const fullname = (prefix ? prefix + "." : "") + name;
-            const fullnameLower = fullname.toLowerCase();
-            if (fullnameLower.indexOf(object) < 0) return;
-
-            let score = 0;
-            const parts = fullnameLower.split(".");
-
-            // check for different match types: exact matches of full name or
-            // "last name" (i.e. last dotted part)
-            if (fullnameLower === object || parts.slice(-1)[0] === object)
-                score += Scorer.objNameMatch;
-            else if (parts.slice(-1)[0].indexOf(object) > -1)
-                score += Scorer.objPartialMatch; // matches in last name
-
-            const objName = objNames[match[1]][2];
-            const title = titles[match[0]];
-
-            // If more than one term searched for, we require other words to be
-            // found in the name/title/description
-            const otherTerms = new Set(objectTerms);
-            otherTerms.delete(object);
-            if (otherTerms.size > 0) {
-                const haystack = `${prefix} ${name} ${objName} ${title}`.toLowerCase();
-                if (
-                    [...otherTerms].some((otherTerm) => haystack.indexOf(otherTerm) < 0)
-                )
-                    return;
-            }
-
-            let anchor = match[3];
-            if (anchor === "") anchor = fullname;
-            else if (anchor === "-") anchor = objNames[match[1]][1] + "-" + fullname;
-
-            const descr = objName + _(", in ") + title;
-
-            // add custom score for some objects according to scorer
-            if (Scorer.objPrio.hasOwnProperty(match[2]))
-                score += Scorer.objPrio[match[2]];
-            else score += Scorer.objPrioDefault;
-
-            results.push([
-                docNames[match[0]],
-                fullname,
-                "#" + anchor,
-                descr,
-                score,
-                filenames[match[0]],
-            ]);
-        };
-        Object.keys(objects).forEach((prefix) =>
-            objects[prefix].forEach((array) =>
-                objectSearchCallback(prefix, array)
-            )
-        );
+    performObjectSearch: function(object, otherterms) {
+        var filenames = this._index.filenames;
+        var docnames = this._index.docnames;
+        var objects = this._index.objects;
+        var objnames = this._index.objnames;
+        var titles = this._index.titles;
+
+        var i;
+        var results = [];
+
+        for (var prefix in objects) {
+            for (var name in objects[prefix]) {
+                var fullname = (prefix ? prefix + '.' : '') + name;
+                var fullnameLower = fullname.toLowerCase()
+                if (fullnameLower.indexOf(object) > -1) {
+                    var score = 0;
+                    var parts = fullnameLower.split('.');
+                    // check for different match types: exact matches of full name or
+                    // "last name" (i.e. last dotted part)
+                    if (fullnameLower == object || parts[parts.length - 1] == object) {
+                        score += Scorer.objNameMatch;
+                        // matches in last name
+                    } else if (parts[parts.length - 1].indexOf(object) > -1) {
+                        score += Scorer.objPartialMatch;
+                    }
+                    var match = objects[prefix][name];
+                    var objname = objnames[match[1]][2];
+                    var title = titles[match[0]];
+                    // If more than one term searched for, we require other words to be
+                    // found in the name/title/description
+                    if (otherterms.length > 0) {
+                        var haystack = (prefix + ' ' + name + ' ' +
+                            objname + ' ' + title).toLowerCase();
+                        var allfound = true;
+                        for (i = 0; i < otherterms.length; i++) {
+                            if (haystack.indexOf(otherterms[i]) == -1) {
+                                allfound = false;
+                                break;
+                            }
+                        }
+                        if (!allfound) {
+                            continue;
+                        }
+                    }
+                    var descr = objname + _(', in ') + title;
+
+                    var anchor = match[3];
+                    if (anchor === '')
+                        anchor = fullname;
+                    else if (anchor == '-')
+                        anchor = objnames[match[1]][1] + '-' + fullname;
+                    // add custom score for some objects according to scorer
+                    if (Scorer.objPrio.hasOwnProperty(match[2])) {
+                        score += Scorer.objPrio[match[2]];
+                    } else {
+                        score += Scorer.objPrioDefault;
+                    }
+                    results.push([docnames[match[0]], fullname, '#' + anchor, descr, score, filenames[match[0]]]);
+                }
+            }
+        }
+
         return results;
     },
 
     /**
      * search for full-text terms in the index
      */
-    performTermsSearch: (searchTerms, excludedTerms) => {
-        // prepare search
-        const terms = Search._index.terms;
-        const titleTerms = Search._index.titleterms;
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-
-        const scoreMap = new Map();
-        const fileMap = new Map();
+    performTermsSearch: function(searchterms, excluded, terms, titleterms) {
+        var docnames = this._index.docnames;
+        var filenames = this._index.filenames;
+        var titles = this._index.titles;
+
+        var i, j, file;
+        var fileMap = {};
+        var scoreMap = {};
+        var results = [];
 
         // perform the search on the required terms
-        searchTerms.forEach((word) => {
-            const files = [];
-            const arr = [{
+        for (i = 0; i < searchterms.length; i++) {
+            var word = searchterms[i];
+            var files = [];
+            var _o = [{
                 files: terms[word],
                 score: Scorer.term
             }, {
-                files: titleTerms[word],
+                files: titleterms[word],
                 score: Scorer.title
-            }, ];
+            }];
             // add support for partial matches
             if (word.length > 2) {
-                const escapedWord = _escapeRegExp(word);
-                Object.keys(terms).forEach((term) => {
-                    if (term.match(escapedWord) && !terms[word])
-                        arr.push({
-                            files: terms[term],
+                for (var w in terms) {
+                    if (w.match(word) && !terms[word]) {
+                        _o.push({
+                            files: terms[w],
                             score: Scorer.partialTerm
-                        });
-                });
-                Object.keys(titleTerms).forEach((term) => {
-                    if (term.match(escapedWord) && !titleTerms[word])
-                        arr.push({
-                            files: titleTerms[word],
+                        })
+                    }
+                }
+                for (var w in titleterms) {
+                    if (w.match(word) && !titleterms[word]) {
+                        _o.push({
+                            files: titleterms[w],
                             score: Scorer.partialTitle
-                        });
-                });
+                        })
+                    }
+                }
             }
 
             // no match but word was a required one
-            if (arr.every((record) => record.files === undefined)) return;
-
+            if ($u.every(_o, function(o) {
+                    return o.files === undefined;
+                })) {
+                break;
+            }
             // found search word in contents
-            arr.forEach((record) => {
-                if (record.files === undefined) return;
-
-                let recordFiles = record.files;
-                if (recordFiles.length === undefined) recordFiles = [recordFiles];
-                files.push(...recordFiles);
-
-                // set score for the word in each file
-                recordFiles.forEach((file) => {
-                    if (!scoreMap.has(file)) scoreMap.set(file, {});
-                    scoreMap.get(file)[word] = record.score;
-                });
+            $u.each(_o, function(o) {
+                var _files = o.files;
+                if (_files === undefined)
+                    return
+
+                if (_files.length === undefined)
+                    _files = [_files];
+                files = files.concat(_files);
+
+                // set score for the word in each file to Scorer.term
+                for (j = 0; j < _files.length; j++) {
+                    file = _files[j];
+                    if (!(file in scoreMap))
+                        scoreMap[file] = {};
+                    scoreMap[file][word] = o.score;
+                }
             });
 
             // create the mapping
-            files.forEach((file) => {
-                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
-                    fileMap.get(file).push(word);
-                else fileMap.set(file, [word]);
-            });
-        });
+            for (j = 0; j < files.length; j++) {
+                file = files[j];
+                if (file in fileMap && fileMap[file].indexOf(word) === -1)
+                    fileMap[file].push(word);
+                else
+                    fileMap[file] = [word];
+            }
+        }
 
         // now check if the files don't contain excluded terms
-        const results = [];
-        for (const [file, wordList] of fileMap) {
-            // check if all requirements are matched
+        for (file in fileMap) {
+            var valid = true;
 
-            // as search terms with length < 3 are discarded
-            const filteredTermCount = [...searchTerms].filter(
-                (term) => term.length > 2
-            ).length;
+            // check if all requirements are matched
+            var filteredTermCount = // as search terms with length < 3 are discarded: ignore
+                searchterms.filter(function(term) {
+                    return term.length > 2
+                }).length
             if (
-                wordList.length !== searchTerms.size &&
-                wordList.length !== filteredTermCount
-            )
-                continue;
+                fileMap[file].length != searchterms.length &&
+                fileMap[file].length != filteredTermCount
+            ) continue;
 
             // ensure that none of the excluded terms is in the search result
-            if (
-                [...excludedTerms].some(
-                    (term) =>
-                    terms[term] === file ||
-                    titleTerms[term] === file ||
-                    (terms[term] || []).includes(file) ||
-                    (titleTerms[term] || []).includes(file)
-                )
-            )
-                break;
+            for (i = 0; i < excluded.length; i++) {
+                if (terms[excluded[i]] == file ||
+                    titleterms[excluded[i]] == file ||
+                    $u.contains(terms[excluded[i]] || [], file) ||
+                    $u.contains(titleterms[excluded[i]] || [], file)) {
+                    valid = false;
+                    break;
+                }
+            }
 
-            // select one (max) score for the file.
-            const score = Math.max(...wordList.map((w) => scoreMap.get(file)[w]));
-            // add result to the result list
-            results.push([
-                docNames[file],
-                titles[file],
-                "",
-                null,
-                score,
-                filenames[file],
-            ]);
+            // if we have still a valid result we can add it to the result list
+            if (valid) {
+                // select one (max) score for the file.
+                // for better ranking, we should calculate ranking by using words statistics like basic tf-idf...
+                var score = $u.max($u.map(fileMap[file], function(w) {
+                    return scoreMap[file][w]
+                }));
+                results.push([docnames[file], titles[file], '', null, score, filenames[file]]);
+            }
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words.
+     * of stemmed words, hlwords is the list of normal, unstemmed
+     * words. the first one is used to find the occurrence, the
+     * latter for highlighting it.
      */
-    makeSearchSummary: (htmlText, keywords) => {
-        const text = Search.htmlToText(htmlText);
-        if (text === "") return null;
-
-        const textLower = text.toLowerCase();
-        const actualStartPosition = [...keywords]
-            .map((k) => textLower.indexOf(k.toLowerCase()))
-            .filter((i) => i > -1)
-            .slice(-1)[0];
-        const startWithContext = Math.max(actualStartPosition - 120, 0);
-
-        const top = startWithContext === 0 ? "" : "...";
-        const tail = startWithContext + 240 < text.length ? "..." : "";
-
-        let summary = document.createElement("p");
-        summary.classList.add("context");
-        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
-
-        return summary;
-    },
+    makeSearchSummary: function(htmlText, keywords, hlwords) {
+        var text = Search.htmlToText(htmlText);
+        var textLower = text.toLowerCase();
+        var start = 0;
+        $.each(keywords, function() {
+            var i = textLower.indexOf(this.toLowerCase());
+            if (i > -1)
+                start = i;
+        });
+        start = Math.max(start - 120, 0);
+        var excerpt = ((start > 0) ? '...' : '') +
+            $.trim(text.substr(start, 240)) +
+            ((start + 240 - text.length) ? '...' : '');
+        var rv = $('<div class="context"></div>').text(excerpt);
+        $.each(hlwords, function() {
+            rv = rv.highlightText(this, 'highlighted');
+        });
+        return rv;
+    }
 };
 
-_ready(Search.init);
+$(document).ready(function() {
+    Search.init();
+});
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/genindex.html` & `Orange3-Explain-0.6.3/doc/_build/html/genindex.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  <title>Index &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
-        <script src="_static/sphinx_highlight.js"></script>
+        <script src="_static/language_data.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
@@ -54,16 +51,16 @@
           <a href="index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Index</li>
+      <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Index</li>
       <li class="wy-breadcrumbs-aside">
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
```

#### html2text {}

```diff
@@ -8,14 +8,15 @@
 [q                   ]
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
     * ICE
    Orange3_Explain
+    *  »
     * Index
 ===============================================================================
 ****** Index ******
 
 ===============================================================================
 © Copyright 2015, Biolab.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/index.html` & `Orange3-Explain-0.6.3/doc/_build/html/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to Orange3 Explain documentation! &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  <title>Welcome to Orange3 Explain documentation! &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
-        <script src="_static/sphinx_highlight.js"></script>
+        <script src="_static/language_data.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Feature Importance" href="widgets/permutation-importance.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
@@ -56,42 +53,42 @@
           <a href="#">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="#" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Welcome to Orange3 Explain documentation!</li>
+      <li><a href="#" class="icon icon-home"></a> &raquo;</li>
+      <li>Welcome to Orange3 Explain documentation!</li>
       <li class="wy-breadcrumbs-aside">
             <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="welcome-to-orange3-explain-documentation">
-<h1>Welcome to Orange3 Explain documentation!<a class="headerlink" href="#welcome-to-orange3-explain-documentation" title="Permalink to this heading"></a></h1>
+<h1>Welcome to Orange3 Explain documentation!<a class="headerlink" href="#welcome-to-orange3-explain-documentation" title="Permalink to this headline">¶</a></h1>
 <section id="widgets">
-<h2>Widgets<a class="headerlink" href="#widgets" title="Permalink to this heading"></a></h2>
+<h2>Widgets<a class="headerlink" href="#widgets" title="Permalink to this headline">¶</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="widgets/permutation-importance.html">Feature Importance</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/explain-model.html">Explain Model</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/explain-prediction.html">Explain Prediction</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/explain-predictions.html">Explain Predictions</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/ice.html">ICE</a></li>
 </ul>
 </div>
 </section>
 </section>
 <section id="indices-and-tables">
-<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
+<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this headline">¶</a></h1>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 <li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
 <li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
 </section>
```

#### html2text {}

```diff
@@ -9,26 +9,27 @@
 [q                   ]
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
     * ICE
    Orange3_Explain
+    *  »
     * Welcome to Orange3 Explain documentation!
     * View_page_source
 ===============================================================================
-****** Welcome to Orange3 Explain documentation!ï ******
-***** Widgetsï *****
+****** Welcome to Orange3 Explain documentation!Â¶ ******
+***** WidgetsÂ¶ *****
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
     * ICE
 
-****** Indices and tablesï ******
+****** Indices and tablesÂ¶ ******
     * Index
     * Module_Index
     * Search_Page
 Next
 ===============================================================================
 © Copyright 2015, Biolab.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/search.html` & `Orange3-Explain-0.6.3/doc/_build/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  <title>Search &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/custom.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
-        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
-        <script src="_static/sphinx_highlight.js"></script>
+        <script src="_static/language_data.js"></script>
     <script src="_static/js/theme.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" /> 
 </head>
 
@@ -57,16 +54,16 @@
           <a href="index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Search</li>
+      <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Search</li>
       <li class="wy-breadcrumbs-aside">
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
```

#### html2text {}

```diff
@@ -8,14 +8,15 @@
 [q                   ]
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
     * ICE
    Orange3_Explain
+    *  »
     * Search
 ===============================================================================
 Please activate JavaScript to enable the search functionality.
 
 ===============================================================================
 © Copyright 2015, Biolab.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-model.html` & `Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-model.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Explain Model &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+  <title>Explain Model &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
-        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
-        <script src="../_static/sphinx_highlight.js"></script>
+        <script src="../_static/language_data.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Explain Prediction" href="explain-prediction.html" />
     <link rel="prev" title="Feature Importance" href="permutation-importance.html" /> 
 </head>
 
@@ -44,15 +41,14 @@
 <li class="toctree-l1"><a class="reference internal" href="permutation-importance.html">Feature Importance</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Explain Model</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#example">Example</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="explain-prediction.html">Explain Prediction</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-predictions.html">Explain Predictions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="ice.html">ICE</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -60,27 +56,27 @@
           <a href="../index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Explain Model</li>
+      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Explain Model</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/explain-model.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="explain-model">
-<h1>Explain Model<a class="headerlink" href="#explain-model" title="Permalink to this heading"></a></h1>
+<h1>Explain Model<a class="headerlink" href="#explain-model" title="Permalink to this headline">¶</a></h1>
 <p>Explains a classification or regression model. Explains which features contribute the most and how they contribute toward the prediction for a specific class.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Data: dataset used to compute the explanations</p></li>
 <li><p>Model: a model which widget explains</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
@@ -95,15 +91,15 @@
 <li><p>Select number of the features shown in the plot.</p></li>
 <li><p>Show/hide the legend.</p></li>
 <li><p>Plot which shows the selected number of features that are most important for a model. For each feature, points in the graph show SHAP values (horizontal axis) for each data instance (row) in the data. SHAP value is a measure of how much each feature affect the model output. Higher SHAP value (higher deviation from the centre of the graph) means that feature value has a higher impact on the prediction for the selected class. Positive SHAP values (points right from the centre) are feature values with the impact toward the prediction for the selected class. Negative values (points left from the centre) have an impact against classification in this class. For regression, SHAP value shows how much the feature value affects the predicted value from the average prediction. Colours represent the value of each feature. Red colour represents higher feature value, while blue colour is a lower value. The colour range is defined based on all values in the dataset for a feature.</p></li>
 <li><p>Press <em>Apply</em> to commit the selection.</p></li>
 <li><p>Get help, save the plot, make the report, or observe the size of input and output data.</p></li>
 </ol>
 <section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline">¶</a></h2>
 <p>In the flowing example, we use the Explain Model widget to explain Logistic regression model. In the File widget, we open Hearth disease dataset. We connect it to Logistic regression widget, which trains the model. Explain Model widget accepts the model and data which are used to explain the model. For an explanation, we usually use the same data than for training, but it is also possible to explain the model on different data. In the Explain model widget, we set the target class on the class to 1 – it means that we observe features that contribute the most to the prediction of a patient with diagnosed heart disease.</p>
 <p>Features in the plot are ordered by their relevance to the prediction. Major vessels coloured is the most important for the prediction in class 1. Instances with higher values of this feature (red colour) have higher SHAP values which mean they contribute toward the prediction of class 1. Lower values of this attribute (blue) contribute against the prediction of this class. The second most important attribute is chest pain (categorical attribute) with value asymptomatic. The presence of this category for the patient (red colour) contributes toward the prediction of class 1, while the absence of this category contributes against class 1.</p>
 <p><img alt="../_images/Explain-Model-Example.png" src="../_images/Explain-Model-Example.png" /></p>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -9,20 +9,20 @@
 Orange3_Explain
 [q                   ]
     * Feature_Importance
     * Explain_Model
           o Example
     * Explain_Prediction
     * Explain_Predictions
-    * ICE
    Orange3_Explain
+    *  »
     * Explain Model
     * View_page_source
 ===============================================================================
-****** Explain Modelï ******
+****** Explain ModelÂ¶ ******
 Explains a classification or regression model. Explains which features
 contribute the most and how they contribute toward the prediction for a
 specific class.
 Inputs
     * Data: dataset used to compute the explanations
     * Model: a model which widget explains
 Outputs
@@ -51,15 +51,15 @@
       the feature value affects the predicted value from the average
       prediction. Colours represent the value of each feature. Red colour
       represents higher feature value, while blue colour is a lower value. The
       colour range is defined based on all values in the dataset for a feature.
    5. Press Apply to commit the selection.
    6. Get help, save the plot, make the report, or observe the size of input
       and output data.
-***** Exampleï *****
+***** ExampleÂ¶ *****
 In the flowing example, we use the Explain Model widget to explain Logistic
 regression model. In the File widget, we open Hearth disease dataset. We
 connect it to Logistic regression widget, which trains the model. Explain Model
 widget accepts the model and data which are used to explain the model. For an
 explanation, we usually use the same data than for training, but it is also
 possible to explain the model on different data. In the Explain model widget,
 we set the target class on the class to 1 â it means that we observe features
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-prediction.html` & `Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-prediction.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Explain Prediction &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+  <title>Explain Prediction &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
-        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
-        <script src="../_static/sphinx_highlight.js"></script>
+        <script src="../_static/language_data.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Explain Predictions" href="explain-predictions.html" />
     <link rel="prev" title="Explain Model" href="explain-model.html" /> 
 </head>
 
@@ -44,15 +41,14 @@
 <li class="toctree-l1"><a class="reference internal" href="permutation-importance.html">Feature Importance</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-model.html">Explain Model</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Explain Prediction</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#example">Example</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="explain-predictions.html">Explain Predictions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="ice.html">ICE</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -60,27 +56,27 @@
           <a href="../index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Explain Prediction</li>
+      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Explain Prediction</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/explain-prediction.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="explain-prediction">
-<h1>Explain Prediction<a class="headerlink" href="#explain-prediction" title="Permalink to this heading"></a></h1>
+<h1>Explain Prediction<a class="headerlink" href="#explain-prediction" title="Permalink to this headline">¶</a></h1>
 <p>Explains which features contribute the most to the prediction for a single instance based on the model and how they contribute.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Model: a model whose predictions are explained by the widget</p></li>
 <li><p>Background data: data needed to compute explanations</p></li>
 <li><p>Data: Single data instance whose prediction is explained by the widget</p></li>
 </ul>
@@ -95,15 +91,15 @@
 <li><p>Zoom in/out the plot.</p></li>
 <li><p>Observe the prediction probability for a class and base value – an average probability in the dataset.</p></li>
 <li><p>Plot which shows features that affect the prediction the most (features with longer tape length) and how they affect it. Red features increase the probability for a selected class while blue features decrease the probability. On the right from the tape, you can see the feature name and its value* for the selected instance. The length of the tape segment (and number on the tape) represent the SHAP value for feature contribution – it is how much the feature affects the probability for the selected class. Numbers in the gray boxes indicate the prediction probability for the selected class is (0.6) and the baseline probability (0.45) (the average probability in the data).</p></li>
 <li><p>Get help, save the plot, make the report, or observe the size of input and output data.</p></li>
 </ol>
 <p>* Some models (including logistic regression) extend the categorical feature to more features with the technique named <a class="reference external" href="https://en.wikipedia.org/wiki/One-hot">one-hot encoding</a>. It means each value in the feature gets a new column which has value 0 (the instance does not have this feature value) or 1 (the instance has this feature value) for each instance. In those cases categorical features will be labeled with the format <code class="docutils literal notranslate"><span class="pre">feature-name=feature-value</span> <span class="pre">=</span> <span class="pre">0/1</span></code> – e.g. <code class="docutils literal notranslate"><span class="pre">chest</span> <span class="pre">pain=asymptomatic</span> <span class="pre">=</span> <span class="pre">1</span></code>. It means that the feature chest pain has value asymptomatic. Model, in this case, made more columns for feature chest pain, one of them was asymptomatic, and it was the case for the selected data instance.</p>
 <section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline">¶</a></h2>
 <p>First, we open heart disease dataset in File widget. With the Data Sampler widget, we split the dataset on the training and test set. The training set is used to train the logistic regression model with the Logistic Regression widget. We compute predictions for the test part of the dataset (remaining data from Data Sampler) with the Predictions widget. In the Predictions widget (the left window) we select the data instance whose prediction we would like to explain – we select the third row in the data which is predicted to belong to class 1 (diagnosed heart disease).</p>
 <p>Explain Prediction widget accept three inputs. First is the model from the Logistic Regression widget, background data from the Data Sampler (we usually use model’s training data as background data), and the data instance whose prediction we want to explain with the Explain Prediction widget. In the widget we select class 1 as a target class, it means we are explaining what features and how they affect the prediction probability for the selected class 1. Numbers in the gray boxes in the plot indicate that the prediction probability for the selected class is 0.6 (border between red and yellow tape) and the baseline probability is 0.45 (the average probability in the data).</p>
 <p>Features marked red on the tape push probabilities from the baseline probability toward probability 1.0 (prediction of the selected class), and blue features push against the prediction of the selected class. Numbers on the tape are SHAP values for each feature – this is how much the feature (and its value) changes the probability toward or against the selected class. We can see that the highest impact on the prediction has the feature <em>major vessels coloured</em> with the value 2 and <em>ST by exercise</em> with the value 2.8. Two important features that push against the prediction of class 1 are <em>gender=male</em> with value 0 (which means that the patient is not male) and <em>gender=female</em> with the value 1 (patient is female - actually another feature with the same meaning that previous).<br /><img alt="../_images/Explain-Prediction-Example.png" src="../_images/Explain-Prediction-Example.png" /></p>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -9,20 +9,20 @@
 Orange3_Explain
 [q                   ]
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
           o Example
     * Explain_Predictions
-    * ICE
    Orange3_Explain
+    *  »
     * Explain Prediction
     * View_page_source
 ===============================================================================
-****** Explain Predictionï ******
+****** Explain PredictionÂ¶ ******
 Explains which features contribute the most to the prediction for a single
 instance based on the model and how they contribute.
 Inputs
     * Model: a model whose predictions are explained by the widget
     * Background data: data needed to compute explanations
     * Data: Single data instance whose prediction is explained by the widget
 Outputs
@@ -56,15 +56,15 @@
 the feature gets a new column which has value 0 (the instance does not have
 this feature value) or 1 (the instance has this feature value) for each
 instance. In those cases categorical features will be labeled with the format
 feature-name=feature-value = 0/1 â e.g. chest pain=asymptomatic = 1. It means
 that the feature chest pain has value asymptomatic. Model, in this case, made
 more columns for feature chest pain, one of them was asymptomatic, and it was
 the case for the selected data instance.
-***** Exampleï *****
+***** ExampleÂ¶ *****
 First, we open heart disease dataset in File widget. With the Data Sampler
 widget, we split the dataset on the training and test set. The training set is
 used to train the logistic regression model with the Logistic Regression
 widget. We compute predictions for the test part of the dataset (remaining data
 from Data Sampler) with the Predictions widget. In the Predictions widget (the
 left window) we select the data instance whose prediction we would like to
 explain â we select the third row in the data which is predicted to belong to
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/widgets/explain-predictions.html` & `Orange3-Explain-0.6.3/doc/_build/html/widgets/explain-predictions.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Explain Predictions &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+  <title>Explain Predictions &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
-        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
-        <script src="../_static/sphinx_highlight.js"></script>
+        <script src="../_static/language_data.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="ICE" href="ice.html" />
     <link rel="prev" title="Explain Prediction" href="explain-prediction.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
@@ -41,15 +37,14 @@
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="permutation-importance.html">Feature Importance</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-model.html">Explain Model</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-prediction.html">Explain Prediction</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Explain Predictions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="ice.html">ICE</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -57,27 +52,27 @@
           <a href="../index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Explain Predictions</li>
+      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Explain Predictions</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/explain-predictions.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="explain-predictions">
-<h1>Explain Predictions<a class="headerlink" href="#explain-predictions" title="Permalink to this heading"></a></h1>
+<h1>Explain Predictions<a class="headerlink" href="#explain-predictions" title="Permalink to this headline">¶</a></h1>
 <p>Explains which features contribute the most to the predictions for the selected instances based on the model and how they contribute.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Model: model whose predictions are explained by the widget</p></li>
 <li><p>Background data: dataset needed to compute explanations</p></li>
 <li><p>Data: dataset whose predictions are explained by the widget</p></li>
 </ul>
@@ -91,15 +86,14 @@
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="explain-prediction.html" class="btn btn-neutral float-left" title="Explain Prediction" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="ice.html" class="btn btn-neutral float-right" title="ICE" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2015, Biolab.</p>
   </div>
```

#### html2text {}

```diff
@@ -1,38 +1,37 @@
 
 
 
 
 
 
 
-
 Orange3_Explain
 [q                   ]
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
-    * ICE
    Orange3_Explain
+    *  »
     * Explain Predictions
     * View_page_source
 ===============================================================================
-****** Explain Predictionsï ******
+****** Explain PredictionsÂ¶ ******
 Explains which features contribute the most to the predictions for the selected
 instances based on the model and how they contribute.
 Inputs
     * Model: model whose predictions are explained by the widget
     * Background data: dataset needed to compute explanations
     * Data: dataset whose predictions are explained by the widget
 Outputs
     * Selected Data: instances selected from the plot
     * Data: original dataset with an additional column showing whether the
       instance is selected
     * Scores: SHAP values for each feature. Features that contribute more to
       prediction have a higher score deviation from 0.
 Explain Predictions widget explains classification or regression modelâs
 predictions for the provided data instances.
-Previous Next
+Previous
 ===============================================================================
 © Copyright 2015, Biolab.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/widgets/ice.html` & `Orange3-Explain-0.6.3/doc/_build/html/widgets/ice.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>ICE &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+  <title>ICE &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
-        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
-        <script src="../_static/sphinx_highlight.js"></script>
+        <script src="../_static/language_data.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="prev" title="Explain Predictions" href="explain-predictions.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
@@ -59,27 +56,27 @@
           <a href="../index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">ICE</li>
+      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>ICE</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/ice.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="ice">
-<h1>ICE<a class="headerlink" href="#ice" title="Permalink to this heading"></a></h1>
+<h1>ICE<a class="headerlink" href="#ice" title="Permalink to this headline">¶</a></h1>
 <p>Displays one line per instance that shows how the instance’s prediction changes when a feature changes.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Model: model</p></li>
 <li><p>Data: dataset</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
@@ -99,15 +96,15 @@
 <li><p>If <strong>Send Automatically</strong> is ticked, the output is sent automatically after any change.
 Alternatively, click <strong>Send</strong>.</p></li>
 <li><p>Get help, save the plot, make the report, set plot properties, or observe the size of input and output data.</p></li>
 <li><p>Plot shows a line for each instance in the input dataset.</p></li>
 <li><p>An interactive plot. Each line represents an instance in the dataset. To select a line, click and drag a line over it.</p></li>
 </ol>
 <section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline">¶</a></h2>
 <p>In the following example, we use the ICE widget to explain a <a class="reference external" href="https://orangedatamining.com/widget-catalog/model/randomforest/">Random Forest</a> model. In the <a class="reference external" href="https://orangedatamining.com/widget-catalog/data/file/">File</a> widget, we open the <em>housing</em> dataset. We connect it to the Random Forest widget, which trains the model. The ICE widget accepts the model and data which are used to explain the model.</p>
 <p>By selecting some arbitrary lines, the selected instances of the input dataset appear on the output of the ICE widget.</p>
 <p><img alt="../_images/ICE-example.png" src="../_images/ICE-example.png" /></p>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -10,18 +10,19 @@
     * Feature_Importance
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
     * ICE
           o Example
    Orange3_Explain
+    *  »
     * ICE
     * View_page_source
 ===============================================================================
-****** ICEï ******
+****** ICEÂ¶ ******
 Displays one line per instance that shows how the instanceâs prediction
 changes when a feature changes.
 Inputs
     * Model: model
     * Data: dataset
 Outputs
     * Selected Data: instances selected from the plot
@@ -42,15 +43,15 @@
    7. If Send Automatically is ticked, the output is sent automatically after
       any change. Alternatively, click Send.
    8. Get help, save the plot, make the report, set plot properties, or observe
       the size of input and output data.
    9. Plot shows a line for each instance in the input dataset.
   10. An interactive plot. Each line represents an instance in the dataset. To
       select a line, click and drag a line over it.
-***** Exampleï *****
+***** ExampleÂ¶ *****
 In the following example, we use the ICE widget to explain a Random_Forest
 model. In the File widget, we open the housing dataset. We connect it to the
 Random Forest widget, which trains the model. The ICE widget accepts the model
 and data which are used to explain the model.
 By selecting some arbitrary lines, the selected instances of the input dataset
 appear on the output of the ICE widget.
 [../_images/ICE-example.png]
```

### Comparing `Orange3-Explain-0.6.2/doc/_build/html/widgets/permutation-importance.html` & `Orange3-Explain-0.6.3/doc/_build/html/widgets/permutation-importance.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Feature Importance &mdash; Orange3 Explain  documentation</title>
-      <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
-      <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+  <title>Feature Importance &mdash; Orange3 Explain  documentation</title><link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
+    <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
-  
-        <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+  <script id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
-        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
-        <script src="../_static/sphinx_highlight.js"></script>
+        <script src="../_static/language_data.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Explain Model" href="explain-model.html" />
     <link rel="prev" title="Welcome to Orange3 Explain documentation!" href="../index.html" /> 
 </head>
 
@@ -44,15 +41,14 @@
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Feature Importance</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#example">Example</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="explain-model.html">Explain Model</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-prediction.html">Explain Prediction</a></li>
 <li class="toctree-l1"><a class="reference internal" href="explain-predictions.html">Explain Predictions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="ice.html">ICE</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -60,27 +56,27 @@
           <a href="../index.html">Orange3 Explain</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a></li>
-      <li class="breadcrumb-item active">Feature Importance</li>
+      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
+      <li>Feature Importance</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/permutation-importance.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="feature-importance">
-<h1>Feature Importance<a class="headerlink" href="#feature-importance" title="Permalink to this heading"></a></h1>
+<h1>Feature Importance<a class="headerlink" href="#feature-importance" title="Permalink to this headline">¶</a></h1>
 <p>Inspect model using the Permutation Feature Importance technique.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Data: dataset used to compute the explanations</p></li>
 <li><p>Model: a model which widget explains</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
@@ -96,15 +92,15 @@
 <li><p>Select the number of the features to be shown in the plot.</p></li>
 <li><p>Zoom in/out the plot.</p></li>
 <li><p>Press <em>Apply</em> to commit the selection.</p></li>
 <li><p>Plot which shows the selected number of features that are most important for a model.</p></li>
 <li><p>Get help, save the plot, make the report, set plot properties, or observe the size of input and output data.</p></li>
 </ol>
 <section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline">¶</a></h2>
 <p>In the flowing example, we use the Feature Importance widget to explain features, used in Logistic regression model. In the File widget, we open Hearth disease dataset. We connect it to Logistic regression widget, which trains the model. Feature Importance widget accepts the model and data which are used to explain the features. For an explanation, we usually use the same data than for training, but it is also possible to explain the features on different data (e.g. reference data subset).</p>
 <p>The features in the plot are ordered by their relevance (e.g. Major vessels coloured is the most important feature).</p>
 <p>By selecting some arbitrary features, a filtered input dataset appears on the output of the Feature Importance widget.</p>
 <p><img alt="../_images/Permutation-Importance-Example.png" src="../_images/Permutation-Importance-Example.png" /></p>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -9,20 +9,20 @@
 Orange3_Explain
 [q                   ]
     * Feature_Importance
           o Example
     * Explain_Model
     * Explain_Prediction
     * Explain_Predictions
-    * ICE
    Orange3_Explain
+    *  »
     * Feature Importance
     * View_page_source
 ===============================================================================
-****** Feature Importanceï ******
+****** Feature ImportanceÂ¶ ******
 Inspect model using the Permutation Feature Importance technique.
 Inputs
     * Data: dataset used to compute the explanations
     * Model: a model which widget explains
 Outputs
     * Selected data: data instances that belong to selected features in the
       plot
@@ -39,15 +39,15 @@
    3. Select the number of the features to be shown in the plot.
    4. Zoom in/out the plot.
    5. Press Apply to commit the selection.
    6. Plot which shows the selected number of features that are most important
       for a model.
    7. Get help, save the plot, make the report, set plot properties, or observe
       the size of input and output data.
-***** Exampleï *****
+***** ExampleÂ¶ *****
 In the flowing example, we use the Feature Importance widget to explain
 features, used in Logistic regression model. In the File widget, we open Hearth
 disease dataset. We connect it to Logistic regression widget, which trains the
 model. Feature Importance widget accepts the model and data which are used to
 explain the features. For an explanation, we usually use the same data than for
 training, but it is also possible to explain the features on different data
 (e.g. reference data subset).
```

### Comparing `Orange3-Explain-0.6.2/doc/conf.py` & `Orange3-Explain-0.6.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/make.bat` & `Orange3-Explain-0.6.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/explain-model.md` & `Orange3-Explain-0.6.3/doc/widgets/explain-model.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/explain-prediction.md` & `Orange3-Explain-0.6.3/doc/widgets/explain-prediction.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/explain-predictions.md` & `Orange3-Explain-0.6.3/doc/widgets/explain-predictions.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/ice.md` & `Orange3-Explain-0.6.3/doc/widgets/ice.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Explain-Model-Example.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Model-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Explain-Model.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Model.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Explain-Prediction-Example.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Prediction-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Explain-Prediction.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Explain-Prediction.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/ICE-example.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/ICE-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/ICE.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/ICE.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Permutation-Importance-Example.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Permutation-Importance-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/images/Permutation-Importance.png` & `Orange3-Explain-0.6.3/doc/_build/htmlhelp/_images/Permutation-Importance.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/doc/widgets/permutation-importance.md` & `Orange3-Explain-0.6.3/doc/widgets/permutation-importance.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/explainer.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import contextlib
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 from scipy import sparse
-
 from shap import KernelExplainer, TreeExplainer
 from shap.utils import sample, hclust_ordering
 from shap.utils._legacy import kmeans
 
 from Orange.base import Model
 from Orange.data import Table, Domain, Variable
 from Orange.util import dummy_callback, wrap_callback
@@ -91,39 +90,51 @@
         )
     # I know it is too broad but this is what TreeExplainer trows
     except Exception:
         return None, None, None
 
     # TreeExplaner cannot explain in normal time more cases than 1000
     data_sample, sample_mask = _subsample_data(transformed_data, 1000)
-    num_classes = (
-        len(model.domain.class_var.values)
-        if model.domain.class_var.is_discrete
-        else None
-    )
 
     # this method will work in batches since explaining only one attribute
     # at time the processing timed doubles comparing to batch size 10
     shap_values = []
     batch_size = 1  # currently set to 1 to minimize widget blocking
     for i in range(0, len(data_sample), batch_size):
         progress_callback(i / len(data_sample))
         batch = data_sample.X[i : i + batch_size]
         shap_values.append(explainer.shap_values(batch, check_additivity=False))
 
     shap_values = _join_shap_values(shap_values)
     base_value = explainer.expected_value
-    # when in training phase one class value was missing skl_model do not
-    # output probability for it. For other models it is handled by Orange
-    if num_classes is not None:
-        missing_d = num_classes - len(shap_values)
-        shap_values += [
-            np.zeros(shap_values[0].shape) for _ in range(missing_d)
+
+    if (
+        type(model.skl_model).__name__ in ("XGBClassifier", "XGBRFClassifier", "GradientBoostingClassifier")
+        and len(model.skl_model.classes_) == 2
+        and len(shap_values) == 1
+    ):
+        # workaround for the error in the TreeExplainer, for the binary
+        # classification the TreeExplainer returns explanations for class 1 only
+        # https://github.com/slundberg/shap/pull/1046
+        shap_values = [-shap_values[0], shap_values[0]]
+        base_value = np.array([-base_value, base_value])
+
+    # when while training one class value is missing in data but is still in
+    # variable's values skl_model do not output probability for it.
+    # Missing class cannot be explained, report zeros
+    class_ = model.domain.class_var
+    if class_.is_discrete and len(class_.values) > len(model.skl_model.classes_):
+        sklc = model.skl_model.classes_.astype(int).tolist()
+        shap_values = [
+            shap_values[sklc.index(i)] if i in sklc else np.zeros(shap_values[0].shape)
+            for i in range(len(class_.values))
         ]
-        base_value = np.hstack((base_value, np.zeros(missing_d)))
+        bv = np.zeros(len(class_.values))
+        bv[sklc] = base_value
+        base_value = bv
 
     return shap_values, sample_mask, base_value
 
 
 def _explain_other_models(
     model: Model,
     transformed_data: Table,
```

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/inspection.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/inspection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/tests/test_explainer.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/tests/test_explainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import inspect
 import unittest
 
 import numpy as np
-
+from numpy.testing import assert_array_equal
 from Orange.classification import (
     LogisticRegressionLearner,
     RandomForestLearner,
     SGDClassificationLearner,
     SVMLearner,
     TreeLearner,
     ThresholdLearner,
 )
-from Orange.data import Table, Domain
+from Orange.data import Table, Domain, ContinuousVariable
 from Orange.regression import LinearRegressionLearner, CurveFitLearner
 from Orange.tests import test_regression, test_classification
 from Orange.widgets.data import owcolor
+from Orange.modelling import GBLearner
+try:
+    from Orange.modelling import XGBLearner, XGBRFLearner
+except ImportError:
+    XGBLearner = XGBRFLearner = None
+from shap import TreeExplainer
+
 from orangecontrib.explain.explainer import (
     compute_colors,
     compute_shap_values,
     explain_predictions,
     INSTANCE_ORDERINGS,
     get_instance_ordering,
     get_shap_values_and_colors,
@@ -28,14 +35,15 @@
 
 
 class TestExplainer(unittest.TestCase):
     def setUp(self) -> None:
         self.iris = Table.from_file("iris")
         self.housing = Table.from_file("housing")[:100, -10:]
         self.titanic = Table("titanic")
+        self.hearth_disease = Table("heart_disease")
 
     def test_tree_explainer(self):
         learner = RandomForestLearner()
         model = learner(self.iris)
 
         shap_values, _, sample_mask, base_value = compute_shap_values(
             model, self.iris, self.iris
@@ -134,39 +142,116 @@
 
         self.assertEqual(len(shap_values), 3)
         self.assertTupleEqual((3,), base_value.shape)
         self.assertTrue(np.any(shap_values[0]))
         self.assertTrue(np.any(shap_values[1]))
         # missing class has all shap values 0
         self.assertFalse(np.any(shap_values[2]))
+        self.assertNotEqual(base_value[0], 0)
+        self.assertNotEqual(base_value[1], 0)
+        self.assertEqual(base_value[2], 0)
 
         # for one class SHAP returns only array (not list of arrays) -
         # must be handled
         learner = RandomForestLearner()
         model = learner(self.iris[:50])
 
         shap_values, _, _, base_value = compute_shap_values(
             model, self.iris[:100], self.iris[:100]
         )
         self.assertEqual(len(shap_values), 3)
         self.assertTupleEqual((3,), base_value.shape)
 
-        # for Logistic regression Orange handle that - test anyway
+        # for Logistic regression Orange handles that - test anyway
         learner = LogisticRegressionLearner()
         model = learner(self.iris[:100])
 
         shap_values, _, _, base_value = compute_shap_values(
             model, self.iris[:100], self.iris[:100]
         )
         self.assertEqual(len(shap_values), 3)
         self.assertTupleEqual((3,), base_value.shape)
-        self.assertNotEqual(shap_values[0].sum(), 0)
-        self.assertNotEqual(shap_values[1].sum(), 0)
+        self.assertTrue(np.any(shap_values[0]))
+        self.assertTrue(np.any(shap_values[1]))
         # missing class has all shap values 0
-        self.assertTrue(not np.any(shap_values[2].sum()))
+        self.assertFalse(np.any(shap_values[2]))
+        self.assertNotEqual(base_value[0], 0)
+        self.assertNotEqual(base_value[1], 0)
+        self.assertEqual(base_value[2], 0)
+
+        learner = RandomForestLearner()
+        data = Table.concatenate((self.iris[:50], self.iris[100:]))
+        model = learner(data)
+        shap_values, _, _, base_value = compute_shap_values(model, data, data)
+        self.assertEqual(len(shap_values), 3)
+        self.assertTupleEqual((3,), base_value.shape)
+        self.assertTrue(np.any(shap_values[0]))
+        # missing class has all shap values 0
+        self.assertFalse(np.any(shap_values[1]))
+        self.assertTrue(np.any(shap_values[2]))
+        self.assertNotEqual(base_value[0], 0)
+        self.assertEqual(base_value[1], 0)
+        self.assertNotEqual(base_value[2], 0)
+
+    @unittest.skipIf(XGBLearner is None, "Missing 'xgboost' package")
+    def test_gradient_boosting_shape(self):
+        """
+        TreeExplainer library for XGBClassifier and GradientBoostingClassifier
+        in case of binary classification outputs only explanation for
+        the class 1. Test workaround that adds explanation for class 0.
+        """
+        learner = XGBLearner()
+        model = learner(self.hearth_disease)
+        shap_values, _, _, base_value = compute_shap_values(
+            model, self.hearth_disease, self.hearth_disease
+        )
+        self.assertEqual(len(shap_values), 2)
+        self.assertEqual(len(base_value), 2)
+        assert_array_equal(-shap_values[0], shap_values[1])
+
+        learner = GBLearner()
+        model = learner(self.hearth_disease)
+        shap_values, _, _, base_value = compute_shap_values(
+            model, self.hearth_disease, self.hearth_disease
+        )
+        self.assertEqual(len(shap_values), 2)
+        self.assertEqual(len(base_value), 2)
+        assert_array_equal(-shap_values[0], shap_values[1])
+
+        learner = XGBRFLearner()
+        model = learner(self.hearth_disease)
+        shap_values, _, _, base_value = compute_shap_values(
+            model, self.hearth_disease, self.hearth_disease
+        )
+        self.assertEqual(len(shap_values), 2)
+        self.assertEqual(len(base_value), 2)
+        assert_array_equal(-shap_values[0], shap_values[1])
+
+    @unittest.skipIf(XGBLearner is None, "Missing 'xgboost' package")
+    def test_remove_workaround(self):
+        """
+        TreeExplainer for XGBClassifier and GradientBoostingClassifier
+        in case of binary classification outputs only explanation for
+        the class 1. Test if it is still the case. When test starts to fail:
+        - remove the test
+        - remove the workaround currently at line 118 from the code
+        """
+        domain = self.hearth_disease.domain
+        hd = self.hearth_disease.transform(
+            Domain(
+                [a for a in domain.attributes if isinstance(a, ContinuousVariable)],
+                class_vars=domain.class_vars,
+            ),
+        )
+        learner = XGBLearner()
+        model = learner(hd)
+        explainer = TreeExplainer(model.skl_model, data=hd.X)
+        shap_values = explainer.shap_values(hd.X[:10], check_additivity=False)
+        # # when it will be fixed the output will have shape (2,) + hs.X.shape
+        self.assertEqual(shap_values.shape, (10, hd.X.shape[1]))
 
     def test_all_classifiers(self):
         """ Test explanation for all classifiers """
         for learner in test_classification.all_learners():
             with self.subTest(learner):
                 if learner == ThresholdLearner:
                     # ThresholdLearner require binary class
```

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/tests/test_inspection.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/__init__.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainModel.svg` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainModel.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainPred.svg` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainPred.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ExplainPredictions.svg` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ExplainPredictions.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/ICE.svg` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/ICE.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/icons/PermutationImportance.svg` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/icons/PermutationImportance.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainfeaturebase.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainfeaturebase.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainmodel.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainmodel.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainprediction.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainprediction.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owexplainpredictions.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owexplainpredictions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owice.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owice.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/owpermutationimportance.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/owpermutationimportance.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainmodel.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainmodel.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainprediction.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainprediction.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owice.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owice.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py` & `Orange3-Explain-0.6.3/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.2/setup.py` & `Orange3-Explain-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path, walk
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "Orange3-Explain"
 
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 
 AUTHOR = "Bioinformatics Laboratory, FRI UL"
 AUTHOR_EMAIL = "contact@orange.biolab.si"
 
 URL = "http://orange.biolab.si/download"
 DESCRIPTION = "Orange3 add-on for explanatory AI"
 LONG_DESCRIPTION = open(
@@ -40,15 +40,15 @@
 INSTALL_REQUIRES = [
     "Orange3 >= 3.33.0",
     "orange-widget-base",
     "AnyQt",
     "numpy",
     "pyqtgraph",
     "scipy",
-    "shap ==0.40.*",  # shap makes significant changes between versions
+    "shap ==0.41.*",  # shap makes significant changes between versions
     "scikit-learn>=1.0.1",
 ]
 
 EXTRAS_REQUIRE = {
     'test': ['pytest', 'coverage'],
     'doc': ['sphinx', 'recommonmark', 'sphinx_rtd_theme'],
 }
```

