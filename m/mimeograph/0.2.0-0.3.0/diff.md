# Comparing `tmp/mimeograph-0.2.0.tar.gz` & `tmp/mimeograph-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.2.0.tar", last modified: Mon Apr  3 07:15:30 2023, max compression
+gzip compressed data, was "mimeograph-0.3.0.tar", last modified: Fri Apr 14 08:40:45 2023, max compression
```

## Comparing `mimeograph-0.2.0.tar` & `mimeograph-0.3.0.tar`

### file list

```diff
@@ -1,56 +1,70 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.2.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       69 2023-03-31 04:40:40.000000 mimeograph-0.2.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    22796 2023-04-03 07:15:30.211394 mimeograph-0.2.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    20839 2023-04-03 07:14:05.000000 mimeograph-0.2.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1422 2023-04-03 07:15:03.000000 mimeograph-0.2.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-03 07:15:30.215394 mimeograph-0.2.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.207394 mimeograph-0.2.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.207394 mimeograph-0.2.0/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-03 07:15:03.000000 mimeograph-0.2.0/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8915 2023-04-03 07:15:03.000000 mimeograph-0.2.0/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.207394 mimeograph-0.2.0/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-03-13 09:26:49.000000 mimeograph-0.2.0/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11294 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-03-27 15:10:13.000000 mimeograph-0.2.0/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-03-20 11:29:27.000000 mimeograph-0.2.0/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      881 2023-03-20 11:29:27.000000 mimeograph-0.2.0/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-03-11 12:33:58.000000 mimeograph-0.2.0/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)      109 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1316 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      649 2023-04-03 07:14:05.000000 mimeograph-0.2.0/src/mimeo/exceptions.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      165 2023-03-27 15:10:04.000000 mimeograph-0.2.0/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      282 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/generators/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1043 2023-03-16 10:25:03.000000 mimeograph-0.2.0/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      528 2023-03-16 07:24:20.000000 mimeograph-0.2.0/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12108 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/generators/generator_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5016 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/logging/filters.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)      455 2023-03-31 04:40:40.000000 mimeograph-0.2.0/src/mimeo/utils.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22796 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1278 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       91 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-03 07:15:30.000000 mimeograph-0.2.0/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-03 07:15:30.211394 mimeograph-0.2.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    29774 2023-04-03 07:14:05.000000 mimeograph-0.2.0/tests/test_mimeo_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1687 2023-03-14 09:58:56.000000 mimeograph-0.2.0/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      462 2023-03-31 04:40:40.000000 mimeograph-0.2.0/tests/test_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.3.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       69 2023-03-31 04:40:40.000000 mimeograph-0.3.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20178 2023-04-14 08:40:45.788154 mimeograph-0.3.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18221 2023-04-14 08:35:34.000000 mimeograph-0.3.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1422 2023-04-14 08:40:13.000000 mimeograph-0.3.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 08:40:45.788154 mimeograph-0.3.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.780153 mimeograph-0.3.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-14 08:40:13.000000 mimeograph-0.3.0/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9013 2023-04-14 08:40:13.000000 mimeograph-0.3.0/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-03-13 09:26:49.000000 mimeograph-0.3.0/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11602 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-03-27 15:10:13.000000 mimeograph-0.3.0/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-04 09:02:56.000000 mimeograph-0.3.0/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      881 2023-03-20 11:29:27.000000 mimeograph-0.3.0/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-03-11 12:33:58.000000 mimeograph-0.3.0/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/annotations.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4098 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      109 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      125 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1316 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      649 2023-04-03 07:14:05.000000 mimeograph-0.3.0/src/mimeo/exceptions.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5745 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      455 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      301 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6899 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6555 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/renderer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20178 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1596 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       91 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29774 2023-04-03 07:14:05.000000 mimeograph-0.3.0/tests/test_mimeo_cli.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 08:35:34.000000 mimeograph-0.3.0/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      462 2023-04-14 08:35:34.000000 mimeograph-0.3.0/tests/test_utils.py
```

### Comparing `mimeograph-0.2.0/LICENSE` & `mimeograph-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/pyproject.toml` & `mimeograph-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.2.0"
+version = "0.3.0"
 description = "Generate data based on a simple template"
 readme = "README.md"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -32,15 +32,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "build", "twine", "isort", "pytest", "pytest-cov", "responses"]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mimeograph-0.2.0/src/mimeo/__main__.py` & `mimeograph-0.3.0/src/mimeo/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 from argparse import ArgumentParser
 from os import path
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
+from mimeo.context import MimeoContextManager
 from mimeo.exceptions import EnvironmentNotFound, EnvironmentsFileNotFound
 from mimeo.logging import setup_logging
 
 setup_logging()
 logger = logging.getLogger(__name__)
 
 DEFAULT_ENVS_FILE_PATH = "mimeo.envs.json"
@@ -20,15 +21,15 @@
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template")
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.2.0")
+            version="%(prog)s v0.3.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configurations")
 
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
@@ -144,15 +145,16 @@
     elif args.fine:
         logging.getLogger("mimeo").setLevel(logging.FINE)
 
     logger.info("Starting Mimeo job")
     for path in args.paths:
         logger.info(f"Data generation from Mimeo Config: {path}")
         mimeo_config = get_config(path, args)
-        Mimeograph(mimeo_config).produce()
+        with MimeoContextManager(mimeo_config):
+            Mimeograph(mimeo_config).produce()
 
 
 def get_config(config_path, args):
     with open(config_path) as config_file:
         config = json.load(config_file)
         if args.http_env is not None:
             envs_file = args.http_envs_file if args.http_envs_file is not None else DEFAULT_ENVS_FILE_PATH
```

### Comparing `mimeograph-0.2.0/src/mimeo/config/mimeo_config.py` & `mimeograph-0.3.0/src/mimeo/config/mimeo_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     VARS_KEY = "vars"
     TEMPLATES_KEY = "_templates_"
     TEMPLATES_COUNT_KEY = "count"
     TEMPLATES_MODEL_KEY = "model"
     MODEL_CONTEXT_KEY = "context"
     MODEL_ATTRIBUTES_KEY = "_attrs"
     MODEL_VALUE_KEY = "_value"
+    MODEL_MIMEO_UTIL_KEY = "_mimeo_util"
+    MODEL_MIMEO_UTIL_NAME_KEY = "_name"
 
     SUPPORTED_OUTPUT_FORMATS = ("xml",)
 
     def __init__(self, config: dict):
         super().__init__(config)
         self.output_format = MimeoConfig.__get_output_format(config)
         self.output_details = MimeoOutputDetails(self.output_format, config.get(self.OUTPUT_DETAILS_KEY, {}))
@@ -78,28 +80,32 @@
         variables = config.get(MimeoConfig.VARS_KEY, {})
         if not isinstance(variables, dict):
             raise InvalidVars(f"vars property does not store an object: {variables}")
         for var, val in variables.items():
             if not re.match(r"^[A-Z][A-Z_0-9]*$", var):
                 raise InvalidVars(f"Provided var [{var}] is invalid "
                                   "(you can use upper-cased name with underscore and digits, starting with a letter)!")
-            if isinstance(val, list) or isinstance(val, dict):
-                raise InvalidVars(f"Provided var [{var}] is invalid (you can use ony atomic values)!")
+            if isinstance(val, list) or (isinstance(val, dict) and not MimeoConfig.__is_mimeo_util_object(val)):
+                raise InvalidVars(f"Provided var [{var}] is invalid (you can use ony atomic values and Mimeo Utils)!")
         return variables
 
     @staticmethod
     def __get_templates(config):
         templates = config.get(MimeoConfig.TEMPLATES_KEY)
         if templates is None:
             raise IncorrectMimeoConfig(f"No templates in the Mimeo Config: {config}")
         elif not isinstance(templates, list):
             raise IncorrectMimeoConfig(f"_templates_ property does not store an array: {config}")
         else:
             return (MimeoTemplate(template) for template in config.get(MimeoConfig.TEMPLATES_KEY))
 
+    @staticmethod
+    def __is_mimeo_util_object(obj: dict):
+        return isinstance(obj, dict) and len(obj) == 1 and MimeoConfig.MODEL_MIMEO_UTIL_KEY in obj
+
 
 class MimeoOutputDetails(MimeoDTO):
 
     FILE_DIRECTION = "file"
     STD_OUT_DIRECTION = "stdout"
     HTTP_DIRECTION = "http"
```

### Comparing `mimeograph-0.2.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.3.0/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.3.0/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.3.0/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/database/cities.py` & `mimeograph-0.3.0/src/mimeo/database/cities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas
 
-from mimeo import utils
+from mimeo import tools
 from mimeo.database.exc import InvalidIndex
 
 
 class City:
 
     def __init__(self, identifier: str, name: str, name_ascii: str, country: str):
         self.id = int(identifier)
@@ -59,9 +59,9 @@
             cls.__CITIES = [City(row.ID, row.CITY, row.CITY_ASCII, row.COUNTRY)
                             for row in cls.__get_cities_df().itertuples()]
         return cls.__CITIES
 
     @classmethod
     def __get_cities_df(cls) -> pandas.DataFrame:
         if cls.__CITIES_DF is None:
-            cls.__CITIES_DF = pandas.read_csv(utils.get_resource(CitiesDB.__CITIES_DB))
+            cls.__CITIES_DF = pandas.read_csv(tools.get_resource(CitiesDB.__CITIES_DB))
         return cls.__CITIES_DF
```

### Comparing `mimeograph-0.2.0/src/mimeo/database/countries.py` & `mimeograph-0.3.0/src/mimeo/database/countries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas
 
-from mimeo import utils
+from mimeo import tools
 from mimeo.database.exc import InvalidIndex
 
 
 class Country:
 
     def __init__(self, iso_3: str, iso_2: str, name: str):
         self.iso_3 = iso_3
@@ -58,9 +58,9 @@
             cls.__COUNTRIES = [Country(row.ISO_3, row.ISO_2, row.NAME)
                                for row in cls.__get_countries_df().itertuples()]
         return cls.__COUNTRIES
 
     @classmethod
     def __get_countries_df(cls) -> pandas.DataFrame:
         if cls.__COUNTRIES_DF is None:
-            cls.__COUNTRIES_DF = pandas.read_csv(utils.get_resource(CountriesDB.__COUNTRIES_DB))
+            cls.__COUNTRIES_DF = pandas.read_csv(tools.get_resource(CountriesDB.__COUNTRIES_DB))
         return cls.__COUNTRIES_DF
```

### Comparing `mimeograph-0.2.0/src/mimeo/database/mimeo_db.py` & `mimeograph-0.3.0/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/exceptions.py` & `mimeograph-0.3.0/src/mimeo/exceptions.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/generators/generator.py` & `mimeograph-0.3.0/src/mimeo/generators/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import xml.etree.ElementTree as ElemTree
 from abc import ABCMeta, abstractmethod
 from typing import Any, Iterator, Union
 
-from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
-from mimeo.generators import GeneratorUtils
+from mimeo.config.mimeo_config import MimeoTemplate
 
 
 class Generator(metaclass=ABCMeta):
 
     __GENERATOR_UTILS_CALL = "GeneratorUtils.get_for_context('{}').{}"
 
     @classmethod
     def __subclasshook__(cls, subclass):
         return (hasattr(subclass, 'generate') and
                 callable(subclass.generate) and
                 hasattr(subclass, 'stringify') and
                 callable(subclass.stringify) or
                 NotImplemented)
 
-    def __init__(self, mimeo_config: MimeoConfig):
-        GeneratorUtils.setup(mimeo_config)
-
     @abstractmethod
     def generate(self,
                  templates: Union[list, Iterator[MimeoTemplate]],
                  parent: Any = None) -> Iterator[ElemTree.Element]:
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `mimeograph-0.2.0/src/mimeo/generators/generator_factory.py` & `mimeograph-0.3.0/src/mimeo/generators/generator_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from mimeo.config.mimeo_config import MimeoConfig, UnsupportedOutputFormat
-from mimeo.generators import Generator, GeneratorUtils, XMLGenerator
+from mimeo.generators import Generator, XMLGenerator
 
 
 class GeneratorFactory:
 
     XML = "xml"
 
     @staticmethod
```

### Comparing `mimeograph-0.2.0/src/mimeo/generators/xml_generator.py` & `mimeograph-0.3.0/src/mimeo/generators/xml_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import logging
 import xml.etree.ElementTree as ElemTree
-from typing import Iterator, Union
+from typing import Iterator, List, Union
 from xml.dom import minidom
 
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
-from mimeo.generators import Generator, GeneratorUtils
+from mimeo.context import MimeoContext
+from mimeo.context.annotations import (mimeo_clear_iterations,
+                                       mimeo_context_switch,
+                                       mimeo_next_iteration, mimeo_context)
+from mimeo.generators import Generator
+from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
 class XMLGenerator(Generator):
 
     def __init__(self, mimeo_config: MimeoConfig):
-        super().__init__(mimeo_config)
+        super().__init__()
         self.__indent = mimeo_config.indent
         self.__xml_declaration = mimeo_config.xml_declaration
-        self.__current_template = None
 
-    def generate(self, templates: Union[list, Iterator[MimeoTemplate]], parent: ElemTree.Element = None) -> Iterator[ElemTree.Element]:
+    @classmethod
+    def generate(cls, templates: Union[list, Iterator[MimeoTemplate]], parent: ElemTree.Element = None) -> Iterator[ElemTree.Element]:
         for template in templates:
-            logger.debug(f"Reading template [{template}]")
-            self.__current_template = template
-            utils = GeneratorUtils.get_for_context(template.model.context_name)
-            utils.reset()
-            for i in iter(range(template.count)):
-                utils.setup_iteration(i + 1)
-                yield self.__to_xml(parent,
-                                    template.model.root_name,
-                                    template.model.root_data)
+            for copy in cls._process_single_template(template, parent):
+                yield copy
 
     def stringify(self, root, mimeo_config):
         if self.__indent is None or self.__indent == 0:
             return ElemTree.tostring(root,
                                      encoding="utf-8",
                                      method="xml",
                                      xml_declaration=self.__xml_declaration).decode('ascii')
@@ -39,61 +37,83 @@
             xml_string = ElemTree.tostring(root)
             xml_minidom = minidom.parseString(xml_string)
             if self.__xml_declaration:
                 return xml_minidom.toprettyxml(indent=" " * self.__indent, encoding="utf-8").decode('ascii')
             else:
                 return xml_minidom.childNodes[0].toprettyxml(indent=" " * self.__indent, encoding="utf-8").decode('ascii')
 
-    def __to_xml(self, parent, element_tag, element_value, attributes: dict = None):
+    @classmethod
+    @mimeo_context_switch
+    @mimeo_clear_iterations
+    def _process_single_template(cls, template: MimeoTemplate, parent: ElemTree.Element = None) -> List[ElemTree.Element]:
+        logger.debug(f"Reading template [{template}]")
+        copies = [cls._process_single_copy(template, parent) for _ in iter(range(template.count))]
+        return copies
+
+    @classmethod
+    @mimeo_next_iteration
+    def _process_single_copy(cls, template: MimeoTemplate, parent: ElemTree.Element = None):
+        return cls._process_node(parent, template.model.root_name, template.model.root_data)
+
+    @classmethod
+    @mimeo_context
+    def _process_node(cls, parent, element_tag, element_value, attributes: dict = None, context: MimeoContext = None):
         logger.fine(f"Rendering element - "
                     f"parent [{parent if parent is None else parent.tag}], "
                     f"element_tag [{element_tag}], "
                     f"element_value [{element_value}], "
                     f"attributes [{attributes}]")
         attributes = attributes if attributes is not None else {}
         if element_tag == MimeoConfig.TEMPLATES_KEY:
             templates = (MimeoTemplate(template) for template in element_value)
-            curr_template = self.__current_template
-            for _ in self.generate(templates, parent):
+            for _ in cls.generate(templates, parent):
                 pass
-            self.__current_template = curr_template
         else:
-            is_special_field = GeneratorUtils.is_special_field(element_tag)
+            is_special_field = MimeoRenderer.is_special_field(element_tag)
             if is_special_field:
-                special_field = element_tag
-                element_tag = GeneratorUtils.get_special_field_name(element_tag)
+                element_tag = MimeoRenderer.get_special_field_name(element_tag)
 
-            element = ElemTree.Element(element_tag, attrib=attributes) if parent is None else ElemTree.SubElement(
-                parent, element_tag, attrib=attributes)
-            if isinstance(element_value, dict):
+            element = cls._create_xml_element(parent, element_tag, attributes)
+
+            if isinstance(element_value, dict) and not MimeoRenderer.is_parametrized_mimeo_util(element_value):
                 if MimeoConfig.MODEL_ATTRIBUTES_KEY in element_value:
                     element_value_copy = dict(element_value)
                     attrs = element_value_copy.pop(MimeoConfig.MODEL_ATTRIBUTES_KEY)
                     value = element_value_copy.get(MimeoConfig.MODEL_VALUE_KEY, element_value_copy)
                     if parent is not None:
                         parent.remove(element)
-                        self.__to_xml(parent, element_tag, value, attrs)
+                        cls._process_node(parent, element_tag, value, attrs)
                     else:
-                        return self.__to_xml(parent, element_tag, value, attrs)
+                        return cls._process_node(parent, element_tag, value, attrs)
                 else:
                     for child_tag, child_value in element_value.items():
-                        self.__to_xml(element, child_tag, child_value)
+                        cls._process_node(element, child_tag, child_value)
             elif isinstance(element_value, list):
                 has_only_atomic_values = all(not isinstance(child, (list, dict)) for child in element_value)
                 if has_only_atomic_values:
                     parent.remove(element)
                     for child in element_value:
-                        self.__to_xml(parent, element_tag, child)
+                        cls._process_node(parent, element_tag, child)
                 else:
                     for child in element_value:
                         grand_child_tag = next(iter(child))
                         grand_child_data = child[grand_child_tag]
-                        self.__to_xml(element, grand_child_tag, grand_child_data)
+                        cls._process_node(element, grand_child_tag, grand_child_data)
             else:
-                element.text = GeneratorUtils.render_value(self.__current_template.model.context_name, element_value)
+                value = MimeoRenderer.render(element_value)
                 if is_special_field:
-                    utils = GeneratorUtils.get_for_context(self.__current_template.model.context_name)
-                    utils.provide(special_field, element.text)
+                    context.curr_iteration().add_special_field(element_tag,
+                                                                                                 value)
+
+                value_str = str(value)
+                element.text = value_str.lower() if isinstance(value, bool) else value_str
                 logger.fine(f"Rendered value [{element.text}]")
 
             if parent is None:
                 return element
+
+    @classmethod
+    def _create_xml_element(cls, parent, element_tag, attributes):
+        if parent is None:
+            return ElemTree.Element(element_tag, attrib=attributes)
+        else:
+            return ElemTree.SubElement(parent, element_tag, attrib=attributes)
```

### Comparing `mimeograph-0.2.0/src/mimeo/mimeo.py` & `mimeograph-0.3.0/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/resources/cities.csv` & `mimeograph-0.3.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/resources/countries.csv` & `mimeograph-0.3.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeo/resources/logging.yaml` & `mimeograph-0.3.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.3.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,40 +2,51 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/mimeo/__init__.py
 src/mimeo/__main__.py
 src/mimeo/exceptions.py
 src/mimeo/mimeo.py
-src/mimeo/utils.py
+src/mimeo/tools.py
 src/mimeo/config/__init__.py
 src/mimeo/config/mimeo_config.py
 src/mimeo/consumers/__init__.py
 src/mimeo/consumers/consumer.py
 src/mimeo/consumers/consumer_factory.py
 src/mimeo/consumers/file_consumer.py
 src/mimeo/consumers/http_consumer.py
 src/mimeo/consumers/raw_consumer.py
+src/mimeo/context/__init__.py
+src/mimeo/context/annotations.py
+src/mimeo/context/exc.py
+src/mimeo/context/mimeo_context.py
+src/mimeo/context/mimeo_context_manager.py
+src/mimeo/context/mimeo_iteration.py
 src/mimeo/database/__init__.py
 src/mimeo/database/cities.py
 src/mimeo/database/countries.py
 src/mimeo/database/exc.py
 src/mimeo/database/mimeo_db.py
 src/mimeo/generators/__init__.py
-src/mimeo/generators/exc.py
 src/mimeo/generators/generator.py
 src/mimeo/generators/generator_factory.py
-src/mimeo/generators/generator_utils.py
 src/mimeo/generators/xml_generator.py
 src/mimeo/logging/__init__.py
 src/mimeo/logging/filters.py
+src/mimeo/meta/__init__.py
+src/mimeo/meta/alive.py
+src/mimeo/meta/exc.py
 src/mimeo/resources/__init__.py
 src/mimeo/resources/cities.csv
 src/mimeo/resources/countries.csv
 src/mimeo/resources/logging.yaml
+src/mimeo/utils/__init__.py
+src/mimeo/utils/exc.py
+src/mimeo/utils/mimeo_utils.py
+src/mimeo/utils/renderer.py
 src/mimeograph.egg-info/PKG-INFO
 src/mimeograph.egg-info/SOURCES.txt
 src/mimeograph.egg-info/dependency_links.txt
 src/mimeograph.egg-info/entry_points.txt
 src/mimeograph.egg-info/requires.txt
 src/mimeograph.egg-info/top_level.txt
 tests/test_mimeo_cli.py
```

### Comparing `mimeograph-0.2.0/tests/test_mimeo_cli.py` & `mimeograph-0.3.0/tests/test_mimeo_cli.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.2.0/tests/test_mimeograph.py` & `mimeograph-0.3.0/tests/test_mimeograph.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from os import path
 
 import pytest
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
+from mimeo.context import MimeoContextManager
 
 
 @pytest.fixture(autouse=True)
 def teardown():
     yield
     # Teardown
     shutil.rmtree("test_mimeograph-dir")
@@ -35,27 +36,28 @@
                         "ChildNode3": True
                     }
                 }
             }
         ]
     }
     mimeo_config = MimeoConfig(config)
-    mimeo = Mimeograph(mimeo_config)
+    with MimeoContextManager(mimeo_config):
+        mimeo = Mimeograph(mimeo_config)
 
-    assert not path.exists("test_mimeograph-dir")
-    mimeo.produce()
-    assert path.exists("test_mimeograph-dir")
-    for i in range(1, 11):
-        file_path = f"test_mimeograph-dir/output-{i}.xml"
-        assert path.exists(file_path)
-
-        with open(file_path, "r") as file_content:
-            assert file_content.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
-            assert file_content.readline() == '<SomeEntity>\n'
-            assert file_content.readline() == '    <ChildNode1>1</ChildNode1>\n'
-            assert file_content.readline() == '    <ChildNode2>value-2</ChildNode2>\n'
-            assert file_content.readline() == '    <ChildNode3>true</ChildNode3>\n'
-            assert file_content.readline() == '</SomeEntity>\n'
+        assert not path.exists("test_mimeograph-dir")
+        mimeo.produce()
+        assert path.exists("test_mimeograph-dir")
+        for i in range(1, 11):
+            file_path = f"test_mimeograph-dir/output-{i}.xml"
+            assert path.exists(file_path)
+
+            with open(file_path, "r") as file_content:
+                assert file_content.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
+                assert file_content.readline() == '<SomeEntity>\n'
+                assert file_content.readline() == '    <ChildNode1>1</ChildNode1>\n'
+                assert file_content.readline() == '    <ChildNode2>value-2</ChildNode2>\n'
+                assert file_content.readline() == '    <ChildNode3>true</ChildNode3>\n'
+                assert file_content.readline() == '</SomeEntity>\n'
```

