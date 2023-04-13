# Comparing `tmp/pytrends-4.9.1.tar.gz` & `tmp/pytrends-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrends-4.9.1.tar", last modified: Sat Apr  8 07:30:25 2023, max compression
+gzip compressed data, was "pytrends-4.9.2.tar", last modified: Thu Apr 13 23:16:38 2023, max compression
```

## Comparing `pytrends-4.9.1.tar` & `pytrends-4.9.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.699724 pytrends-4.9.1/
--rw-r--r--   0 elazzarin   (502) staff       (20)       77 2023-01-11 17:32:54.000000 pytrends-4.9.1/.gitattributes
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.689103 pytrends-4.9.1/.github/
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.691440 pytrends-4.9.1/.github/workflows/
--rw-r--r--   0 elazzarin   (502) staff       (20)     1388 2023-01-11 17:32:54.000000 pytrends-4.9.1/.github/workflows/python-package.yml
--rw-r--r--   0 elazzarin   (502) staff       (20)     2090 2022-02-02 01:32:22.000000 pytrends-4.9.1/.gitignore
--rw-r--r--   0 elazzarin   (502) staff       (20)     7264 2023-01-11 17:32:54.000000 pytrends-4.9.1/CONTRIBUTING.md
--rw-r--r--   0 elazzarin   (502) staff       (20)      559 2022-02-02 01:32:22.000000 pytrends-4.9.1/LICENSE
--rw-r--r--   0 elazzarin   (502) staff       (20)       34 2022-02-02 01:32:22.000000 pytrends-4.9.1/MANIFEST.in
--rw-r--r--   0 elazzarin   (502) staff       (20)    13165 2023-04-08 07:30:25.699484 pytrends-4.9.1/PKG-INFO
--rw-r--r--   0 elazzarin   (502) staff       (20)    12402 2023-01-11 17:32:54.000000 pytrends-4.9.1/README.md
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.691597 pytrends-4.9.1/examples/
--rw-r--r--   0 elazzarin   (502) staff       (20)     1572 2023-01-11 17:32:54.000000 pytrends-4.9.1/examples/example.py
--rw-r--r--   0 elazzarin   (502) staff       (20)     1368 2023-04-08 07:24:42.000000 pytrends-4.9.1/pyproject.toml
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.692303 pytrends-4.9.1/pytrends/
--rw-r--r--   0 elazzarin   (502) staff       (20)        0 2022-02-02 01:32:22.000000 pytrends-4.9.1/pytrends/__init__.py
--rw-r--r--   0 elazzarin   (502) staff       (20)     5308 2022-11-05 17:37:32.000000 pytrends-4.9.1/pytrends/dailydata.py
--rw-r--r--   0 elazzarin   (502) staff       (20)      581 2023-01-11 17:32:54.000000 pytrends-4.9.1/pytrends/exceptions.py
--rw-r--r--   0 elazzarin   (502) staff       (20)    24723 2023-04-08 07:24:23.000000 pytrends-4.9.1/pytrends/request.py
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.693079 pytrends-4.9.1/pytrends.egg-info/
--rw-r--r--   0 elazzarin   (502) staff       (20)    13165 2023-04-08 07:30:25.000000 pytrends-4.9.1/pytrends.egg-info/PKG-INFO
--rw-r--r--   0 elazzarin   (502) staff       (20)     2019 2023-04-08 07:30:25.000000 pytrends-4.9.1/pytrends.egg-info/SOURCES.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)        1 2023-04-08 07:30:25.000000 pytrends-4.9.1/pytrends.egg-info/dependency_links.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)       32 2023-04-08 07:30:25.000000 pytrends-4.9.1/pytrends.egg-info/requires.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)        9 2023-04-08 07:30:25.000000 pytrends-4.9.1/pytrends.egg-info/top_level.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)       52 2023-01-11 17:32:54.000000 pytrends-4.9.1/requirements-dev.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)       32 2023-01-11 17:32:54.000000 pytrends-4.9.1/requirements.txt
--rw-r--r--   0 elazzarin   (502) staff       (20)       38 2023-04-08 07:30:25.699786 pytrends-4.9.1/setup.cfg
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.693490 pytrends-4.9.1/tests/
--rw-r--r--   0 elazzarin   (502) staff       (20)        0 2023-01-11 17:32:54.000000 pytrends-4.9.1/tests/__init__.py
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.689693 pytrends-4.9.1/tests/cassettes/
-drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-08 07:30:25.699142 pytrends-4.9.1/tests/cassettes/test_request/
--rw-r--r--   0 elazzarin   (502) staff       (20)    66971 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_build_payload.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    61989 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_initial_data.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    76625 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_by_region_city_resolution.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    73920 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_by_region_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    61989 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_bad_gprop.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    69735 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_froogle.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    69729 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_images.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    69729 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_news.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    69713 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    76526 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_partial.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    69735 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_interest_over_time_youtube.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    65027 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_multirange_interest_over_time_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    65008 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_multirange_interest_over_time_same_keyword_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)   284163 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_realtime_trending_searches_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    74341 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_queries_result_keys.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    74361 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_queries_result_rising.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    74357 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_queries_result_top.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    70162 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_topics_result_keys.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    70162 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_topics_result_rising.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    70154 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_related_topics_result_top.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    63925 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_suggestions_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    66999 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_tokens.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    67287 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_top_charts_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)    91913 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/cassettes/test_request/test_trending_searches_ok.yaml
--rw-r--r--   0 elazzarin   (502) staff       (20)      249 2023-01-11 17:32:54.000000 pytrends-4.9.1/tests/conftest.py
--rw-r--r--   0 elazzarin   (502) staff       (20)    23105 2023-04-08 07:21:58.000000 pytrends-4.9.1/tests/test_request.py
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.407653 pytrends-4.9.2/
+-rw-r--r--   0 elazzarin   (502) staff       (20)       77 2023-01-11 17:32:54.000000 pytrends-4.9.2/.gitattributes
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.394736 pytrends-4.9.2/.github/
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.397631 pytrends-4.9.2/.github/workflows/
+-rw-r--r--   0 elazzarin   (502) staff       (20)     1388 2023-01-11 17:32:54.000000 pytrends-4.9.2/.github/workflows/python-package.yml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     2090 2022-02-02 01:32:22.000000 pytrends-4.9.2/.gitignore
+-rw-r--r--   0 elazzarin   (502) staff       (20)     7264 2023-01-11 17:32:54.000000 pytrends-4.9.2/CONTRIBUTING.md
+-rw-r--r--   0 elazzarin   (502) staff       (20)      559 2022-02-02 01:32:22.000000 pytrends-4.9.2/LICENSE
+-rw-r--r--   0 elazzarin   (502) staff       (20)       34 2022-02-02 01:32:22.000000 pytrends-4.9.2/MANIFEST.in
+-rw-r--r--   0 elazzarin   (502) staff       (20)    13165 2023-04-13 23:16:38.407353 pytrends-4.9.2/PKG-INFO
+-rw-r--r--   0 elazzarin   (502) staff       (20)    12402 2023-01-11 17:32:54.000000 pytrends-4.9.2/README.md
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.398060 pytrends-4.9.2/examples/
+-rw-r--r--   0 elazzarin   (502) staff       (20)     1572 2023-01-11 17:32:54.000000 pytrends-4.9.2/examples/example.py
+-rw-r--r--   0 elazzarin   (502) staff       (20)     1368 2023-04-13 23:12:49.000000 pytrends-4.9.2/pyproject.toml
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.399019 pytrends-4.9.2/pytrends/
+-rw-r--r--   0 elazzarin   (502) staff       (20)        0 2022-02-02 01:32:22.000000 pytrends-4.9.2/pytrends/__init__.py
+-rw-r--r--   0 elazzarin   (502) staff       (20)     5308 2022-11-05 17:37:32.000000 pytrends-4.9.2/pytrends/dailydata.py
+-rw-r--r--   0 elazzarin   (502) staff       (20)      581 2023-01-11 17:32:54.000000 pytrends-4.9.2/pytrends/exceptions.py
+-rw-r--r--   0 elazzarin   (502) staff       (20)    24740 2023-04-13 23:13:06.000000 pytrends-4.9.2/pytrends/request.py
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.399812 pytrends-4.9.2/pytrends.egg-info/
+-rw-r--r--   0 elazzarin   (502) staff       (20)    13165 2023-04-13 23:16:38.000000 pytrends-4.9.2/pytrends.egg-info/PKG-INFO
+-rw-r--r--   0 elazzarin   (502) staff       (20)     2019 2023-04-13 23:16:38.000000 pytrends-4.9.2/pytrends.egg-info/SOURCES.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)        1 2023-04-13 23:16:38.000000 pytrends-4.9.2/pytrends.egg-info/dependency_links.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)       32 2023-04-13 23:16:38.000000 pytrends-4.9.2/pytrends.egg-info/requires.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)        9 2023-04-13 23:16:38.000000 pytrends-4.9.2/pytrends.egg-info/top_level.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)       52 2023-01-11 17:32:54.000000 pytrends-4.9.2/requirements-dev.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)       32 2023-01-11 17:32:54.000000 pytrends-4.9.2/requirements.txt
+-rw-r--r--   0 elazzarin   (502) staff       (20)       38 2023-04-13 23:16:38.407709 pytrends-4.9.2/setup.cfg
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.400410 pytrends-4.9.2/tests/
+-rw-r--r--   0 elazzarin   (502) staff       (20)        0 2023-01-11 17:32:54.000000 pytrends-4.9.2/tests/__init__.py
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.395517 pytrends-4.9.2/tests/cassettes/
+drwxr-xr-x   0 elazzarin   (502) staff       (20)        0 2023-04-13 23:16:38.406899 pytrends-4.9.2/tests/cassettes/test_request/
+-rw-r--r--   0 elazzarin   (502) staff       (20)     7722 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_build_payload.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     2813 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_initial_data.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    17082 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_by_region_city_resolution.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    14543 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_by_region_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     2817 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_bad_gprop.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10354 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_froogle.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10336 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_images.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10352 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_news.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10336 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    17056 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_partial.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10338 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_interest_over_time_youtube.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10459 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_multirange_interest_over_time_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10436 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_multirange_interest_over_time_same_keyword_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)   177571 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_realtime_trending_searches_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    14864 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_queries_result_keys.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    14864 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_queries_result_rising.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    14877 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_queries_result_top.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10728 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_topics_result_keys.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10724 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_topics_result_rising.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    10720 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_related_topics_result_top.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     4641 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_suggestions_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     7721 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_tokens.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)     7995 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_top_charts_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)    34740 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/cassettes/test_request/test_trending_searches_ok.yaml
+-rw-r--r--   0 elazzarin   (502) staff       (20)      249 2023-01-11 17:32:54.000000 pytrends-4.9.2/tests/conftest.py
+-rw-r--r--   0 elazzarin   (502) staff       (20)    22899 2023-04-08 22:49:57.000000 pytrends-4.9.2/tests/test_request.py
```

### Comparing `pytrends-4.9.1/.github/workflows/python-package.yml` & `pytrends-4.9.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/.gitignore` & `pytrends-4.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/CONTRIBUTING.md` & `pytrends-4.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/LICENSE` & `pytrends-4.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/PKG-INFO` & `pytrends-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrends
-Version: 4.9.1
+Version: 4.9.2
 Summary: Pseudo API for Google Trends
 Author: John Hogue, Burton DeWilde
 Author-email: dreyco676@gmail.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/dreyco676/pytrends
 Keywords: google trends api search
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrends-4.9.1/README.md` & `pytrends-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/examples/example.py` & `pytrends-4.9.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/pyproject.toml` & `pytrends-4.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrends"
-version = "4.9.1"
+version = "4.9.2"
 description = "Pseudo API for Google Trends"
 urls = {homepage = "https://github.com/dreyco676/pytrends"}
 requires-python = ">=3.7"
 authors = [
     {name = "John Hogue"},
     {name = "Burton DeWilde"},
     {email = "dreyco676@gmail.com"}
```

### Comparing `pytrends-4.9.1/pytrends/dailydata.py` & `pytrends-4.9.2/pytrends/dailydata.py`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/pytrends/exceptions.py` & `pytrends-4.9.2/pytrends/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/pytrends/request.py` & `pytrends-4.9.2/pytrends/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,28 +69,28 @@
         Gets google cookie (used for each and every proxy; once on init otherwise)
         Removes proxy from the list on proxy error
         """
         while True:
             if "proxies" in self.requests_args:
                 try:
                     return dict(filter(lambda i: i[0] == 'NID', requests.get(
-                        f'{BASE_TRENDS_URL}/?geo={self.hl[-2:]}',
+                        f'{BASE_TRENDS_URL}/explore/?geo={self.hl[-2:]}',
                         timeout=self.timeout,
                         **self.requests_args
                     ).cookies.items()))
                 except:
                     continue
             else:
                 if len(self.proxies) > 0:
                     proxy = {'https': self.proxies[self.proxy_index]}
                 else:
                     proxy = ''
                 try:
                     return dict(filter(lambda i: i[0] == 'NID', requests.get(
-                        f'{BASE_TRENDS_URL}/?geo={self.hl[-2:]}',
+                        f'{BASE_TRENDS_URL}/explore/?geo={self.hl[-2:]}',
                         timeout=self.timeout,
                         proxies=proxy,
                         **self.requests_args
                     ).cookies.items()))
                 except requests.exceptions.ProxyError:
                     print('Proxy error. Changing IP')
                     if len(self.proxies) > 1:
@@ -190,15 +190,15 @@
         return
 
     def _tokens(self):
         """Makes request to Google to get API tokens for interest over time, interest by region and related queries"""
         # make the request and parse the returned json
         widget_dicts = self._get_data(
             url=TrendReq.GENERAL_URL,
-            method=TrendReq.GET_METHOD,
+            method=TrendReq.POST_METHOD,
             params=self.token_payload,
             trim_chars=4,
         )['widgets']
         # order of the json matters...
         first_region_token = True
         # clear self.related_queries_widget_list and self.related_topics_widget_list
         # of old keywords'widgets
@@ -476,15 +476,15 @@
             method=TrendReq.GET_METHOD
         )[pn]
         result_df = pd.DataFrame(req_json)
         return result_df
 
     def today_searches(self, pn='US'):
         """Request data from Google Daily Trends section and returns a dataframe"""
-        forms = {'ns': 15, 'geo': pn, 'tz': '-180', 'hl': 'en-US'}
+        forms = {'ns': 15, 'geo': pn, 'tz': '-180', 'hl': self.hl}
         req_json = self._get_data(
             url=TrendReq.TODAY_SEARCHES_URL,
             method=TrendReq.GET_METHOD,
             trim_chars=5,
             params=forms,
             **self.requests_args
         )['default']['trendingSearchesDays'][0]['trendingSearches']
@@ -509,15 +509,15 @@
 
         # rs : don't know what is does but it's max value is never more than the ri_value based on emperical evidence
         # max value of ri supported is 200, based on emperical evidence
         rs_value = 200
         if count < rs_value:
             rs_value = count-1
 
-        forms = {'ns': 15, 'geo': pn, 'tz': '300', 'hl': 'en-US', 'cat': cat, 'fi' : '0', 'fs' : '0', 'ri' : ri_value, 'rs' : rs_value, 'sort' : 0}
+        forms = {'ns': 15, 'geo': pn, 'tz': '300', 'hl': self.hl, 'cat': cat, 'fi' : '0', 'fs' : '0', 'ri' : ri_value, 'rs' : rs_value, 'sort' : 0}
         req_json = self._get_data(
             url=TrendReq.REALTIME_TRENDING_SEARCHES_URL,
             method=TrendReq.GET_METHOD,
             trim_chars=5,
             params=forms
         )['storySummaries']['trendingStories']
```

### Comparing `pytrends-4.9.1/pytrends.egg-info/PKG-INFO` & `pytrends-4.9.2/pytrends.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrends
-Version: 4.9.1
+Version: 4.9.2
 Summary: Pseudo API for Google Trends
 Author: John Hogue, Burton DeWilde
 Author-email: dreyco676@gmail.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/dreyco676/pytrends
 Keywords: google trends api search
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrends-4.9.1/pytrends.egg-info/SOURCES.txt` & `pytrends-4.9.2/pytrends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrends-4.9.1/tests/test_request.py` & `pytrends-4.9.2/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 @pytest.mark.vcr
 def test_interest_over_time_ok():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe='2021-01-01 2021-01-05')
     df_result = pytrend.interest_over_time()
     df_expected = build_interest_over_time_df({
-        'pizza': [100, 84, 78, 50, 52],
+        'pizza': [100, 83, 78, 49, 50],
         'bagel': [2, 2, 2, 1, 1]
     }, dates=['2021-01-01', '2021-01-02', '2021-01-03', '2021-01-04', '2021-01-05'])
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_interest_over_time_images():
@@ -185,47 +185,47 @@
     pytrend.build_payload(
         kw_list=['pizza', 'bagel'],
         gprop='images',
         timeframe='2021-01-01 2021-01-05'
     )
     df_result = pytrend.interest_over_time()
     df_expected = build_interest_over_time_df({
-        'pizza': [83, 100, 89, 93, 93],
-        'bagel': [2, 2, 4, 4, 4]
+        'pizza': [85, 100, 93, 93, 93],
+        'bagel': [3, 2, 9, 4, 4]
     }, dates=['2021-01-01', '2021-01-02', '2021-01-03', '2021-01-04', '2021-01-05'])
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_interest_over_time_news():
     pytrend = TrendReq()
     pytrend.build_payload(
         kw_list=['pizza', 'bagel'],
         gprop='news',
         timeframe='2021-01-01 2021-01-05'
     )
     df_result = pytrend.interest_over_time()
     df_expected = build_interest_over_time_df({
-        'pizza': [100, 51, 76, 44, 49],
-        'bagel': [0, 0, 0, 0, 15]
+        'pizza': [100, 67, 78, 32, 75],
+        'bagel': [0, 0, 0, 20, 0]
     }, dates=['2021-01-01', '2021-01-02', '2021-01-03', '2021-01-04', '2021-01-05'])
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_interest_over_time_youtube():
     pytrend = TrendReq()
     pytrend.build_payload(
         kw_list=['pizza', 'bagel'],
         gprop='youtube',
         timeframe='2021-01-01 2021-01-05'
     )
     df_result = pytrend.interest_over_time()
     df_expected = build_interest_over_time_df({
-        'pizza': [88, 100, 99, 90, 93],
+        'pizza': [88, 100, 100, 92, 95],
         'bagel': [1, 1, 1, 2, 1]
     }, dates=['2021-01-01', '2021-01-02', '2021-01-03', '2021-01-04', '2021-01-05'])
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_interest_over_time_froogle():
@@ -233,85 +233,88 @@
     pytrend.build_payload(
         kw_list=['pizza', 'bagel'],
         gprop='froogle',
         timeframe='2021-01-01 2021-01-05'
     )
     df_result = pytrend.interest_over_time()
     df_expected = build_interest_over_time_df({
-        'pizza': [100, 100, 88, 61, 91],
-        'bagel': [7, 0, 4, 0, 0]
+        'pizza': [94, 99, 94, 62, 100],
+        'bagel': [0, 0, 0, 0, 8]
     }, dates=['2021-01-01', '2021-01-02', '2021-01-03', '2021-01-04', '2021-01-05'])
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_interest_over_time_bad_gprop():
     pytrend = TrendReq()
     expected_message = re.compile(r'^gprop must be.+$')
     with pytest.raises(ValueError, match=expected_message):
         pytrend.build_payload(kw_list=['pizza', 'bagel'], gprop=' ')
 
+
 @pytest.mark.vcr
 def test_multirange_interest_over_time_ok():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe=['2021-01-01 2021-01-05', '2021-01-06 2021-01-10'])
     df_result = pytrend.multirange_interest_over_time()
 
     expected_result = ExpectedResult(
         length=6,
         df_head=pd.DataFrame({
             '[0] pizza date': ['Average', 'Jan 1, 2021', 'Jan 2, 2021'],
-            '[0] pizza value': [74, 100, 85],
+            '[0] pizza value': [72, 100, 83],
             '[1] bagel date': ['Average', 'Jan 6, 2021', 'Jan 7, 2021'],
             '[1] bagel value': [1, 1, 1]
         }),
         df_tail=pd.DataFrame({
             '[0] pizza date': ['Jan 3, 2021', 'Jan 4, 2021', 'Jan 5, 2021'],
-            '[0] pizza value': [82, 50, 51],
+            '[0] pizza value': [78, 49, 50],
             '[1] bagel date': ['Jan 8, 2021', 'Jan 9, 2021', 'Jan 10, 2021'],
             '[1] bagel value': [1, 2, 2]
-        }, index=pd.Index([3, 4, 5]))    
+        }, index=pd.Index([3, 4, 5]))
     )
     expected_result.assert_equals(df_result)
 
+
 @pytest.mark.vcr
 def test_multirange_interest_over_time_same_keyword_ok():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza', 'pizza'], timeframe=['2021-01-01 2021-01-05', '2021-01-06 2021-01-10'])
     df_result = pytrend.multirange_interest_over_time()
 
     expected_result = ExpectedResult(
         length=6,
         df_head=pd.DataFrame({
             '[0] pizza date': ['Average', 'Jan 1, 2021', 'Jan 2, 2021'],
-            '[0] pizza value': [74, 100, 85],
+            '[0] pizza value': [72, 100, 83],
             '[1] pizza date': ['Average', 'Jan 6, 2021', 'Jan 7, 2021'],
-            '[1] pizza value': [68, 53, 53]
+            '[1] pizza value': [68, 52, 52]
         }),
         df_tail=pd.DataFrame({
             '[0] pizza date': ['Jan 3, 2021', 'Jan 4, 2021', 'Jan 5, 2021'],
-            '[0] pizza value': [82, 50, 51],
+            '[0] pizza value': [78, 49, 50],
             '[1] pizza date': ['Jan 8, 2021', 'Jan 9, 2021', 'Jan 10, 2021'],
-            '[1] pizza value': [70, 88, 76]
-        }, index=pd.Index([3, 4, 5]))    
+            '[1] pizza value': [70, 89, 74]
+        }, index=pd.Index([3, 4, 5]))
     )
     expected_result.assert_equals(df_result)
 
+
 @pytest.mark.vcr
 def test_interest_by_region_ok():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.interest_by_region()
     # Both head and tail have all 0's in both values, sort the result to test more meaningful values
     df_result = df_result.sort_values(by=['bagel', 'pizza', 'geoName'], ascending=False)
     expected_result = ExpectedResult(
         length=250,
         df_head=pd.DataFrame({
-            'pizza': [93, 94, 96],
-            'bagel': [7, 6, 4],
+            'pizza': [92, 94, 96],
+            'bagel': [8, 6, 4],
         }, index=pd.Index(['Singapore', 'Hong Kong', 'Taiwan'], name='geoName')),
         df_tail=pd.DataFrame({
             'pizza': [0, 0, 0],
             'bagel': [0, 0, 0],
         }, index=pd.Index(['Algeria', 'Albania', 'Afghanistan'], name='geoName'))
     )
     expected_result.assert_equals(df_result)
@@ -323,21 +326,21 @@
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.interest_by_region(resolution='CITY')
     # Both head and tail have all 0's in both values, sort the result to test more meaningful values
     df_result = df_result.sort_values(by=['bagel', 'pizza', 'geoName'], ascending=False)
     expected_result = ExpectedResult(
         length=200,
         df_head=pd.DataFrame({
-            'pizza': [95, 96, 96],
-            'bagel': [5, 4, 4],
-        }, index=pd.Index(['Grafton', 'Melbourne', 'Boston'], name='geoName')),
+            'pizza': [97, 97, 98],
+            'bagel': [3, 3, 2],
+        }, index=pd.Index(['Charlotte', 'Altamonte Springs', 'Portland'], name='geoName')),
         df_tail=pd.DataFrame({
             'pizza': [0, 0, 0],
             'bagel': [0, 0, 0],
-        }, index=pd.Index(['Andover', 'Anchorage', 'Allen'], name='geoName'))
+        }, index=pd.Index(['Albany', 'Aix-en-Provence', 'Aalborg'], name='geoName'))
     )
     expected_result.assert_equals(df_result)
 
 
 # FIXME: With more than one term the result is always an empty dict.
 # In the web we can get related topics using ['Torvalds', 'Dijkstra'] but not here, something's wrong.
 @pytest.mark.vcr
@@ -354,62 +357,62 @@
 
 @pytest.mark.vcr
 def test_related_topics_result_top():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.related_topics()['pizza']['top']
     expected_result = ExpectedResult(
-        length=22,
+        length=21,
         df_head=pd.DataFrame({
-            'value': [100, 24, 13],
-            'formattedValue': ['100', '24', '13'],
+            'value': [100, 23, 12],
+            'formattedValue': ['100', '23', '12'],
             'hasData': [True, True, True],
             'link': [
                 '/trends/explore?q=/m/0663v&date=2021-01-01+2021-12-31',
                 '/trends/explore?q=/m/09cfq&date=2021-01-01+2021-12-31',
                 '/trends/explore?q=/m/03clwm&date=2021-01-01+2021-12-31'
             ],
             'topic_mid': ['/m/0663v', '/m/09cfq', '/m/03clwm'],
-            'topic_title': ['Pizza', 'Pizza Hut', "Domino's Pizza"],
-            'topic_type': ['Dish', 'Restaurant company', 'Restaurant company'],
+            'topic_title': ['Pizza', 'Pizza Hut', "Domino's"],
+            'topic_type': ['Dish', 'Restaurant chain', 'Restaurant chain'],
         }),
         df_tail=pd.DataFrame({
             'value': [0, 0, 0],
             'formattedValue': ['<1', '<1', '<1'],
             'hasData': [True, True, True],
             'link': [
-                '/trends/explore?q=/g/11g6qhxwmd&date=2021-01-01+2021-12-31',
                 '/trends/explore?q=/g/11b7c9w1y6&date=2021-01-01+2021-12-31',
                 '/trends/explore?q=/m/09nghg&date=2021-01-01+2021-12-31',
+                '/trends/explore?q=/m/0gwh_4&date=2021-01-01+2021-12-31',
             ],
-            'topic_mid': ['/g/11g6qhxwmd', '/g/11b7c9w1y6', '/m/09nghg'],
-            'topic_title': ['Ooni', "Roman's Pizza", 'Sam Goody'],
-            'topic_type': ['Topic', 'Topic', 'Retail company']
-        }, index=pd.Index([19, 20, 21]))
+            'topic_mid': ['/g/11b7c9w1y6', '/m/09nghg', '/m/0gwh_4'],
+            'topic_title': ["Roman's Pizza", 'Sam Goody', 'Detroit-style pizza'],
+            'topic_type': ['Topic', 'Retail company', 'Food']
+        }, index=pd.Index([18, 19, 20]))
     )
     expected_result.assert_equals(df_result)
 
 
 @pytest.mark.vcr
 def test_related_topics_result_rising():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.related_topics()['pizza']['rising']
     df_expected = pd.DataFrame({
-        'value': [12100, 160, 80, 80],
-        'formattedValue': ['Breakout', '+160%', '+80%', '+80%'],
+        'value': [12600, 160, 80, 70],
+        'formattedValue': ['Breakout', '+160%', '+80%', '+70%'],
         'link': [
             '/trends/explore?q=/m/09nghg&date=2021-01-01+2021-12-31',
             '/trends/explore?q=/m/0gwh_4&date=2021-01-01+2021-12-31',
+            '/trends/explore?q=/g/11g6qhxwmd&date=2021-01-01+2021-12-31',
             '/trends/explore?q=/m/02hvyj&date=2021-01-01+2021-12-31',
-            '/trends/explore?q=/g/11g6qhxwmd&date=2021-01-01+2021-12-31'
         ],
-        'topic_mid': ['/m/09nghg', '/m/0gwh_4', '/m/02hvyj', '/g/11g6qhxwmd'],
-        'topic_title': ['Sam Goody', 'Detroit-style pizza', 'Mystic Pizza', 'Ooni'],
-        'topic_type': ['Retail company', 'Food', '1988 film', 'Topic'],
+        'topic_mid': ['/m/09nghg', '/m/0gwh_4', '/g/11g6qhxwmd', '/m/02hvyj'],
+        'topic_title': ['Sam Goody', 'Detroit-style pizza', 'Ooni', 'Mystic Pizza'],
+        'topic_type': ['Retail company', 'Food', 'Topic', '1988 film'],
     })
     assert_frame_equal(df_result, df_expected)
 
 
 @pytest.mark.vcr
 def test_related_queries_result_keys():
     pytrend = TrendReq()
@@ -428,82 +431,82 @@
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.related_queries()
 
     expected_pizza = ExpectedResult(
         length=25,
         df_head=pd.DataFrame({
             'query': ['pizza hut', 'pizza near me', 'pizza pizza near me'],
-            'value': [100, 67, 65],
+            'value': [100, 68, 65],
         }),
         df_tail=pd.DataFrame({
-            'query': ['pizza papa johns', 'little caesars', 'boston pizza'],
+            'query': ['pizza little caesars', 'cheese pizza', 'new york pizza'],
             'value': [5, 5, 5],
         }, index=pd.Index([22, 23, 24]))
     )
     expected_pizza.assert_equals(df_result['pizza']['top'])
 
     expected_bagel = ExpectedResult(
         length=25,
         df_head=pd.DataFrame({
-            'query': ['the bagel', 'bagel me', 'bagel near me'],
-            'value': [100, 92, 85],
+            'query': ['the bagel', 'bagel me', 'everything bagel'],
+            'value': [100, 97, 92],
         }),
         df_tail=pd.DataFrame({
-            'query': ['manhattan bagel', 'bagel sandwich', 'what a bagel'],
-            'value': [21, 21, 20],
+            'query': ['what a bagel', 'bagel sandwich', 'coffee meets bagel'],
+            'value': [22, 22, 22],
         }, index=pd.Index([22, 23, 24]))
     )
     expected_bagel.assert_equals(df_result['bagel']['top'])
 
 
 @pytest.mark.vcr
 def test_related_queries_result_rising():
     pytrend = TrendReq()
     pytrend.build_payload(kw_list=['pizza', 'bagel'], timeframe='2021-01-01 2021-12-31')
     df_result = pytrend.related_queries()
 
     expected_pizza = ExpectedResult(
-        length=13,
+        length=11,
         df_head=pd.DataFrame({
             'query': ['licorice pizza', 'history of pizza', 'stoned pizza'],
-            'value': [9100, 400, 300],
+            'value': [8550, 400, 300],
         }),
         df_tail=pd.DataFrame({
-            'query': ['mountain mike pizza', 'pizza raul', 'pizza cosy'],
-            'value': [50, 50, 50],
-        }, index=pd.Index([10, 11, 12]))
+            'query': ['incredible pizza', 'mountain mike pizza', 'angels pizza'],
+            'value': [60, 50, 40],
+        }, index=pd.Index([8, 9, 10]))
     )
     expected_pizza.assert_equals(df_result['pizza']['rising'])
 
     expected_bagel = ExpectedResult(
-        length=19,
+        length=18,
         df_head=pd.DataFrame({
             'query': ['rover bagel', 'kettlemans bagel', 'bagel karen'],
-            'value': [450, 250, 190],
+            'value': [350, 250, 180],
         }),
         df_tail=pd.DataFrame({
-            'query': ['bagel street deli', 'best bagel near me', 'bloomington bagel company'],
-            'value': [40, 40, 40],
-        }, index=pd.Index([16, 17, 18]))
+            'query': ['bagel street deli', 'best bagel near me', 'the bagel nook'],
+            'value': [50, 50, 40],
+        }, index=pd.Index([15, 16, 17]))
     )
     expected_bagel.assert_equals(df_result['bagel']['rising'])
 
 
 @pytest.mark.vcr
 def test_trending_searches_ok():
     pytrend = TrendReq()
     # trending_searches doesn't need to call build_payload.
     df_result = pytrend.trending_searches()
     # NOTE: This expected result needs to be rebuilt from scratch every time the cassette is rewritten.
     # They're time-dependent.
     expected_result = ExpectedResult(
         length=20,
-        df_head=pd.DataFrame({0: ['Kevin Conroy', 'Gallagher', 'Student loan forgiveness']}),
+        df_head=pd.DataFrame({0: ['Chabelo', 'Jonathan Majors', 'Benavidez vs Plant']}),
         df_tail=pd.DataFrame(
-            {0: ['Nick Cannon', 'CPI', 'Daytona Beach']},
+            {0: ['Gonzaga', 'Reese Witherspoon', 'France vs Netherlands']},
             index=pd.Index([17, 18, 19])
         )
     )
     expected_result.assert_equals(df_result)
 
 
 @pytest.mark.vcr
@@ -514,50 +517,49 @@
     # NOTE: This expected result needs to be rebuilt from scratch every time the cassette is rewritten.
     # They're time-dependent.
     # NOTE: The result returned by this function is a monster.
     # Strings of almost 200 characters, lists of strings, lists of lists of strings...
     # Rebuilding a full 3-head-tail result from scratch is a chore, with a single record for head
     # and tail is more than enough.
     expected_result = ExpectedResult(
-        length=122,
+        length=111,
         head_tail_length=1,
         df_head=pd.DataFrame({
             'title': [
-                ("Gonzaga Bulldogs men's basketball, "
-                 "Michigan State Spartans men's basketball, "
-                 'College basketball, '
-                 'Armed Forces Classic, '
-                 'Michigan State Spartans football')
+                ('Caleb Plant, '
+                 'Boxing, Canelo Álvarez, '
+                 'David Benavidez, '
+                 'Anthony Dirrell')
             ],
             'entityNames': [
                 [
-                    "Gonzaga Bulldogs men's basketball",
-                    "Michigan State Spartans men's basketball",
-                    'College basketball',
-                    'Armed Forces Classic',
-                    'Michigan State Spartans football',
-                ],
+                    'Caleb Plant',
+                    'Boxing',
+                    'Canelo Álvarez',
+                    'David Benavidez',
+                    'Anthony Dirrell',
+                ]
             ]
         }),
         df_tail=pd.DataFrame({
             'title': [
-                ('Wake Forest University, '
-                 'Georgia Bulldogs football, '
-                 'Atlantic Coast Conference, '
-                 'College basketball')
+                ('Ron DeSantis, '
+                 'Casey DeSantis, '
+                 'Republican Party, '
+                 'Christina DeSantis')
             ],
             'entityNames': [
                 [
-                    'Wake Forest University',
-                    'Georgia Bulldogs football',
-                    'Atlantic Coast Conference',
-                    'College basketball'
-                ],
+                    'Ron DeSantis',
+                    'Casey DeSantis',
+                    'Republican Party',
+                    'Christina DeSantis',
+                ]
             ]
-        }, index=pd.Index([121]))
+        }, index=pd.Index([110]))
     )
     expected_result.assert_equals(df_result)
 
 
 @pytest.mark.vcr
 def test_top_charts_ok():
     pytrend = TrendReq()
@@ -585,17 +587,17 @@
 def test_suggestions_ok():
     pytrend = TrendReq()
     # suggestions doesn't need to call build_payload.
     result = pytrend.suggestions(keyword='pizza')
     expected = [
         {'mid': '/m/0663v', 'title': 'Pizza', 'type': 'Dish'},
         {'mid': '/g/11k19hmrkk', 'title': 'Licorice Pizza', 'type': '2021 film'},
+        {'mid': '/m/0rg8s1t', 'title': 'Dominos Pizza', 'type': 'Topic'},
         {'mid': '/m/0dfxdnc', 'title': 'Pizza dough', 'type': 'Food'},
         {'mid': '/g/11hdxfw7c0', 'title': 'history of pizza', 'type': 'Food'},
-        {'mid': '/g/11fl7dydwb', 'title': 'Pizza Oven', 'type': 'Topic'},
     ]
     assert result == expected
 
 
 @pytest.mark.vcr
 def test_interest_over_time_partial():
     # NOTE: This test may fails if regenerate the cassette on Mondays because the last week will not be partial
@@ -604,15 +606,15 @@
     df_result = pytrend.interest_over_time()
     s_last_row = df_result.iloc[-1]
     assert s_last_row.isPartial is np.bool_(True)
 
 
 def test_request_args_passing(mocked_responses):
     mocked_responses.add(
-        url=f'{BASE_TRENDS_URL}/?geo=US',
+        url=f'{BASE_TRENDS_URL}/explore/?geo=US',
         method='GET',
         match=[responses.matchers.header_matcher({'User-Agent': 'pytrends'})]
     )
     mocked_responses.add(
         url=TrendReq.TRENDING_SEARCHES_URL,
         method='GET',
         match=[responses.matchers.header_matcher({'User-Agent': 'pytrends'})],
```

