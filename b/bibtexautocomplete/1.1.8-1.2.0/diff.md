# Comparing `tmp/bibtexautocomplete-1.1.8.tar.gz` & `tmp/bibtexautocomplete-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtexautocomplete-1.1.8.tar", last modified: Mon Feb 27 10:22:07 2023, max compression
+gzip compressed data, was "bibtexautocomplete-1.2.0.tar", last modified: Fri Apr 14 13:05:45 2023, max compression
```

## Comparing `bibtexautocomplete-1.1.8.tar` & `bibtexautocomplete-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1070 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/LICENSE
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    12117 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    10872 2023-02-08 11:34:03.000000 bibtexautocomplete-1.1.8/README.md
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.457530 bibtexautocomplete-1.1.8/bibtexautocomplete/
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.457530 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      649 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3905 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/arxiv.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4323 2022-12-23 09:28:35.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/crossref.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2290 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/dblp.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3570 2023-02-27 10:14:37.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/doi.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2840 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/researchr.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3593 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/unpaywall.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      184 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       67 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/__main__.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.457530 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2341 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/author.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     6834 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/entry.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2565 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/io.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2352 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/matching.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     5990 2023-02-27 10:15:05.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/normalize.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/bibtexautocomplete/core/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      121 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    12837 2023-02-27 09:43:01.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/autocomplete.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1005 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/data_dump.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3453 2023-02-26 23:39:11.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/main.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     9252 2023-01-06 12:18:21.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/parser.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2240 2023-02-27 09:46:40.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/core/threads.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3779 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/abstract_base.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1731 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/condition_mixin.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     9208 2023-02-27 10:14:59.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/https.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1115 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/lookups.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4626 2022-12-23 09:27:29.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/multiple_mixin.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3510 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/search_mixin.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2710 2023-02-27 09:04:25.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/ansi.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1391 2023-02-27 10:21:16.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/constants.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     7755 2023-02-27 09:42:38.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/logger.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2497 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/only_exclude.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3860 2022-10-31 11:49:39.000000 bibtexautocomplete-1.1.8/bibtexautocomplete/utils/safe_json.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-02-27 10:22:07.457530 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    12117 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1539 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/SOURCES.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/dependency_links.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       55 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/entry_points.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      126 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/requires.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       19 2023-02-27 10:22:07.000000 bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/top_level.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      395 2023-02-27 10:22:07.461530 bibtexautocomplete-1.1.8/setup.cfg
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2298 2023-02-03 08:49:32.000000 bibtexautocomplete-1.1.8/setup.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.893211 bibtexautocomplete-1.2.0/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1070 2023-02-27 13:14:39.000000 bibtexautocomplete-1.2.0/LICENSE
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    13083 2023-04-14 13:05:45.893211 bibtexautocomplete-1.2.0/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    11838 2023-04-14 12:48:13.000000 bibtexautocomplete-1.2.0/README.md
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.889211 bibtexautocomplete-1.2.0/bibtexautocomplete/
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.889211 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      757 2023-03-22 15:20:57.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3905 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/arxiv.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4321 2023-03-21 12:32:23.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/crossref.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2595 2023-03-06 19:04:10.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/dblp.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3631 2023-03-21 12:41:29.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/doi.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2845 2023-03-21 12:37:16.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/researchr.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5938 2023-03-22 15:26:15.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/semantic_scholar.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3493 2023-03-21 12:41:42.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/unpaywall.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      184 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       67 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/__main__.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.889211 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2341 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/author.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     6834 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/entry.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2565 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/io.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2352 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/matching.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4626 2023-03-06 18:52:33.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/normalize.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.889211 bibtexautocomplete-1.2.0/bibtexautocomplete/core/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      121 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    13345 2023-03-21 11:58:52.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/autocomplete.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1005 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/data_dump.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4116 2023-04-14 12:50:29.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/main.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     9679 2023-04-14 12:51:14.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/parser.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2240 2023-02-27 09:46:40.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/core/threads.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.893211 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3779 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/abstract_base.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1731 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/condition_mixin.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     9435 2023-03-21 12:36:31.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/https.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1115 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/lookups.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4697 2023-03-21 13:36:00.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/multiple_mixin.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3464 2023-03-06 18:56:15.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/search_mixin.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.893211 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2710 2023-02-27 09:04:25.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/ansi.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1528 2023-04-14 13:04:06.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/constants.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      719 2023-04-14 12:44:02.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/functions.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     7780 2023-03-21 12:31:57.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/logger.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2497 2023-04-14 12:41:44.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/only_exclude.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3860 2022-10-31 11:49:39.000000 bibtexautocomplete-1.2.0/bibtexautocomplete/utils/safe_json.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-04-14 13:05:45.889211 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    13083 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1621 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       55 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/entry_points.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      126 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/requires.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       19 2023-04-14 13:05:45.000000 bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/top_level.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      395 2023-04-14 13:05:45.893211 bibtexautocomplete-1.2.0/setup.cfg
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2298 2023-02-03 08:49:32.000000 bibtexautocomplete-1.2.0/setup.py
```

### Comparing `bibtexautocomplete-1.1.8/LICENSE` & `bibtexautocomplete-1.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Dorian Lesbre
+Copyright (c) 2023 Dorian Lesbre
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bibtexautocomplete-1.1.8/PKG-INFO` & `bibtexautocomplete-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtexautocomplete
-Version: 1.1.8
+Version: 1.2.0
 Summary: Module to complete bibtex files by polling online databases
 Home-page: https://github.com/dlesbre/bibtex-autocomplete
 Author: Dorian Lesbre
 Author-email: dorian.lesbre@gmail.com
 License: MIT
 Keywords: bibtex biblatex latex autocomplete btac
 Platform: any
@@ -27,21 +27,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: dev
 License-File: LICENSE
 
-<!-- LTeX: language=en -->
-
 # Bibtex Autocomplete
 
 [![PyPI version][version-shield]][pypi-link]
 [![PyPI pyversions][pyversion-shield]][pypi-link]
-[![License][license-shield]](./LICENSE)
+[![License][license-shield]](https://choosealicense.com/licenses/mit/)
 [![PyPI status][status-shield]][pypi-link]
 [![Downloads][download-shield]](https://pepy.tech/project/bibtexautocomplete)
 
 [![Maintenance][maintain-shield]][commit-link]
 [![Commit][commit-shield]][commit-link]
 [![actions][pipeline-shield]][pipeline-link]
 [![issues][issues-shield]][issues-link]
@@ -71,14 +69,15 @@
 bibliographies. It is inspired and expanding on the solution provided by
 [thando](https://tex.stackexchange.com/users/182467/thando) in this
 [TeX stack exchange post](https://tex.stackexchange.com/questions/6810/automatically-adding-doi-fields-to-a-hand-made-bibliography).
 
 It attempts to complete a BibTeX file by querying the following domains:
 - [www.crossref.org](https://www.crossref.org/)
 - [arxiv.org](https://arxiv.org/)
+- [semanticscholar.org](https://www.semanticscholar.org/)
 - [dlbp.org](https://dlbp.org)
 - [researchr.org](https://researchr.org/)
 - [unpaywall.org](https://unpaywall.org/)
 
 Big thanks to all of them for allowing open, easy and well-documented access to
 their databases.
 
@@ -86,14 +85,17 @@
 
 - [Demo](#demo)
 - [Quick overview](#quick-overview)
 - [Installation](#installation)
   - [Dependencies](#dependencies)
 - [Usage](#usage)
 - [Command line arguments](#command-line-arguments)
+  - [Query filtering](#query-filtering)
+  - [Output formatting](#output-formatting)
+  - [Optional flags](#optional-flags)
 
 ## Demo
 
 ![demo.svg](https://raw.githubusercontent.com/dlesbre/bibtex-autocomplete/2d1a01f5ec94c8af9c2f3c1a810eca51bb4cce74/imgs/demo.svg)
 
 ## Quick overview
 
@@ -123,19 +125,21 @@
   adding data from another similar-ish entry to your entry. If you find any such
   false positive please report them using the [issue
   tracker](https://github.com/dlesbre/bibtex-autocomplete/issues).
 
 **How are entries completed?**
 
 Once responses from all websites have been found, the script will add fields
-from website with the following priority : crossref > arxiv > dblp > researchr >
-unpaywall.
+from website with the following priority :
+
+crossref > arxiv > semantic scholar > dblp > researchr > unpaywall.
 
 So if both crossref's and dblp's response contain a publisher, the one from
-crossref will be used.
+crossref will be used. This order can be changed using the `-q --only-query`
+option (see [query filtering](#query-filtering)).
 
 The script will not overwrite any user given non-empty fields, unless the
 `-f/--force-overwrite` flag is given. If you want to check what fields are
 added, you can use `-v/--verbose` to have them printed to stdout (with
 source information), or `-p/--prefix` to have the new fields be prefixed with
 `BTAC` in the output file.
 
@@ -158,72 +162,89 @@
 ```
 
 ### Dependencies
 
 This package has two dependencies (automatically installed by pip) :
 
 - [bibtexparser](https://bibtexparser.readthedocs.io/)
-- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 2.4.0) for the fancy progress bar
+- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 3.0.0) for the fancy progress bar
 
 ## Usage
 
 The command line tool can be used as follows:
 ```console
 btac [--flags] <input_files>
 ```
 
 **Examples :**
 
 - `btac my/db.bib` : reads from `./my/db.bib`, writes to `./my/db.btac.bib`
 - `btac -i db.bib` : reads from `db.bib` and overwrites it (inplace flag)
-- `btac db1.bib db2.bib -o out1.bib -o out2.bib` reads multiple files and write
-  their outputs to `out1.bib` and `out2.bib` respectively.
+- `btac db1.bib db2.bib db3.bib -o out1.bib -o out2.bib` reads `db1.bib`,
+  `db2.bib` and `db3.bib`, and write their outputs to `out1.bib`, `out2.bib`
+  and `db3.btac.bib` respectively.
 - `btac folder` : reads from all files ending with `.bib` in folder. Excludes
   `.btac.bib` files unless they are the only `.bib` files present. Writes to
   `folder/file.btac.bib` unless inplace flag is set.
 - `btac` with no inputs is same as `btac .`
+- `btac -v ...` verbose mode, pretty prints all new fields when done
 
 **Note:** the [parser](https://pypi.org/project/bibtexparser/) doesn't preserve
 format information, so this script will reformat your files. Some formatting
 options (see below) are provided.
 
 **Slow responses:** I found that crossref responds significantly slower than the
 other websites. It often takes longer than the 20s timeout.
 - You can increase timeout with `btac ... -t 60` (60s) or `btac ... -t -1` (no timeout)
 - You can disable crossref queries with `btac ... -Q crossref`
 
 ## Command line arguments
 
-**Optional arguments:**
-
 - `-o --output <file.bib>`
 
   Write output to given file. Can be used multiple times when also giving
   multiple inputs. Maps inputs to outputs in order. If there are extra inputs,
   uses default name (`old_name.btac.bib`). Ignored in inplace (`-i`) mode.
 
+### Query filtering
+
 - `-q --only-query <site>` or `-Q --dont-query <site>`
 
   Restrict which websites to query from. `<site>` must be one of: `crossref`,
-  `dblp`, `arxiv`, `researchr`, `unpaywall`. These arguments can be used
+  `arxiv`, `s2`, `dblp`, `researchr`, `unpaywall`. These arguments can be used
   multiple times, for example to only query crossref and dblp use `-q crossref
-  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv`
+  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv -Q s2`
+
+  Additionally, you can use `-q` to change the completion priority.
+  So `-q unpaywall -q researchr -q dblp -q s2 -q arxiv -q crossref` reverses the
+  default order.
 
 - `-e --only-entry <id>` or `-E --exclude-entry <id>`
 
   Restrict which entries should be autocomplete. `<id>` is the entry ID used in
   your BibTeX file (e.g. `@inproceedings{<id> ... }`). These arguments can also
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
-**Output formatting:**
+- `-m --mark` and `-M --ignore-mark`
+
+  This is useful to avoid repeated queries if you want to run `btac` many times
+  on the same (large) file.
+
+  By default, `btac` ignores any entry with a `BTACqueried` field. `--ignore-mark`
+  overrides this behavior.
+
+  When `--mark` is set, `btac` adds a `BTACqueried = {yyyy-mm-dd}` field to each entry
+  it queries.
+
+### Output formatting
 
 Unfortunately [bibtexparser](https://pypi.org/project/bibtexparser/) doesn't
 preserve format information, so this script will reformat your BibTeX file. Here
 are a few options you can use to control the output format:
 
 - `--fa --align-values` pad field names to align all values
 
@@ -245,15 +266,16 @@
   ```
 
 - `--fl --no-trailing-comma` don't add the last trailing comma
 - `--fi --indent <space>` space used for indentation, default is a tab.
   Can be specified as a number (number of spaces) or a string with spaces
   and `_`, `t`, and `n` characters to mark space, tabs and newlines.
 
-**Flags:**
+### Optional flags
+
 - `-i --inplace` Modify input files inplace, ignores any specified output files
 - `-p --prefix` Write new fields with a prefix. The script will add `BTACtitle =
   ...` instead of `title = ...` in the bib file. This can be combined with `-f`
   to safely show info for already present fields.
 
   Note that this can overwrite existing fields starting with `BTACxxxx`, even
   without the `-f` option.
```

### Comparing `bibtexautocomplete-1.1.8/README.md` & `bibtexautocomplete-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-<!-- LTeX: language=en -->
-
 # Bibtex Autocomplete
 
 [![PyPI version][version-shield]][pypi-link]
 [![PyPI pyversions][pyversion-shield]][pypi-link]
-[![License][license-shield]](./LICENSE)
+[![License][license-shield]](https://choosealicense.com/licenses/mit/)
 [![PyPI status][status-shield]][pypi-link]
 [![Downloads][download-shield]](https://pepy.tech/project/bibtexautocomplete)
 
 [![Maintenance][maintain-shield]][commit-link]
 [![Commit][commit-shield]][commit-link]
 [![actions][pipeline-shield]][pipeline-link]
 [![issues][issues-shield]][issues-link]
@@ -38,14 +36,15 @@
 bibliographies. It is inspired and expanding on the solution provided by
 [thando](https://tex.stackexchange.com/users/182467/thando) in this
 [TeX stack exchange post](https://tex.stackexchange.com/questions/6810/automatically-adding-doi-fields-to-a-hand-made-bibliography).
 
 It attempts to complete a BibTeX file by querying the following domains:
 - [www.crossref.org](https://www.crossref.org/)
 - [arxiv.org](https://arxiv.org/)
+- [semanticscholar.org](https://www.semanticscholar.org/)
 - [dlbp.org](https://dlbp.org)
 - [researchr.org](https://researchr.org/)
 - [unpaywall.org](https://unpaywall.org/)
 
 Big thanks to all of them for allowing open, easy and well-documented access to
 their databases.
 
@@ -53,14 +52,17 @@
 
 - [Demo](#demo)
 - [Quick overview](#quick-overview)
 - [Installation](#installation)
   - [Dependencies](#dependencies)
 - [Usage](#usage)
 - [Command line arguments](#command-line-arguments)
+  - [Query filtering](#query-filtering)
+  - [Output formatting](#output-formatting)
+  - [Optional flags](#optional-flags)
 
 ## Demo
 
 ![demo.svg](https://raw.githubusercontent.com/dlesbre/bibtex-autocomplete/2d1a01f5ec94c8af9c2f3c1a810eca51bb4cce74/imgs/demo.svg)
 
 ## Quick overview
 
@@ -90,19 +92,21 @@
   adding data from another similar-ish entry to your entry. If you find any such
   false positive please report them using the [issue
   tracker](https://github.com/dlesbre/bibtex-autocomplete/issues).
 
 **How are entries completed?**
 
 Once responses from all websites have been found, the script will add fields
-from website with the following priority : crossref > arxiv > dblp > researchr >
-unpaywall.
+from website with the following priority :
+
+crossref > arxiv > semantic scholar > dblp > researchr > unpaywall.
 
 So if both crossref's and dblp's response contain a publisher, the one from
-crossref will be used.
+crossref will be used. This order can be changed using the `-q --only-query`
+option (see [query filtering](#query-filtering)).
 
 The script will not overwrite any user given non-empty fields, unless the
 `-f/--force-overwrite` flag is given. If you want to check what fields are
 added, you can use `-v/--verbose` to have them printed to stdout (with
 source information), or `-p/--prefix` to have the new fields be prefixed with
 `BTAC` in the output file.
 
@@ -125,72 +129,89 @@
 ```
 
 ### Dependencies
 
 This package has two dependencies (automatically installed by pip) :
 
 - [bibtexparser](https://bibtexparser.readthedocs.io/)
-- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 2.4.0) for the fancy progress bar
+- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 3.0.0) for the fancy progress bar
 
 ## Usage
 
 The command line tool can be used as follows:
 ```console
 btac [--flags] <input_files>
 ```
 
 **Examples :**
 
 - `btac my/db.bib` : reads from `./my/db.bib`, writes to `./my/db.btac.bib`
 - `btac -i db.bib` : reads from `db.bib` and overwrites it (inplace flag)
-- `btac db1.bib db2.bib -o out1.bib -o out2.bib` reads multiple files and write
-  their outputs to `out1.bib` and `out2.bib` respectively.
+- `btac db1.bib db2.bib db3.bib -o out1.bib -o out2.bib` reads `db1.bib`,
+  `db2.bib` and `db3.bib`, and write their outputs to `out1.bib`, `out2.bib`
+  and `db3.btac.bib` respectively.
 - `btac folder` : reads from all files ending with `.bib` in folder. Excludes
   `.btac.bib` files unless they are the only `.bib` files present. Writes to
   `folder/file.btac.bib` unless inplace flag is set.
 - `btac` with no inputs is same as `btac .`
+- `btac -v ...` verbose mode, pretty prints all new fields when done
 
 **Note:** the [parser](https://pypi.org/project/bibtexparser/) doesn't preserve
 format information, so this script will reformat your files. Some formatting
 options (see below) are provided.
 
 **Slow responses:** I found that crossref responds significantly slower than the
 other websites. It often takes longer than the 20s timeout.
 - You can increase timeout with `btac ... -t 60` (60s) or `btac ... -t -1` (no timeout)
 - You can disable crossref queries with `btac ... -Q crossref`
 
 ## Command line arguments
 
-**Optional arguments:**
-
 - `-o --output <file.bib>`
 
   Write output to given file. Can be used multiple times when also giving
   multiple inputs. Maps inputs to outputs in order. If there are extra inputs,
   uses default name (`old_name.btac.bib`). Ignored in inplace (`-i`) mode.
 
+### Query filtering
+
 - `-q --only-query <site>` or `-Q --dont-query <site>`
 
   Restrict which websites to query from. `<site>` must be one of: `crossref`,
-  `dblp`, `arxiv`, `researchr`, `unpaywall`. These arguments can be used
+  `arxiv`, `s2`, `dblp`, `researchr`, `unpaywall`. These arguments can be used
   multiple times, for example to only query crossref and dblp use `-q crossref
-  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv`
+  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv -Q s2`
+
+  Additionally, you can use `-q` to change the completion priority.
+  So `-q unpaywall -q researchr -q dblp -q s2 -q arxiv -q crossref` reverses the
+  default order.
 
 - `-e --only-entry <id>` or `-E --exclude-entry <id>`
 
   Restrict which entries should be autocomplete. `<id>` is the entry ID used in
   your BibTeX file (e.g. `@inproceedings{<id> ... }`). These arguments can also
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
-**Output formatting:**
+- `-m --mark` and `-M --ignore-mark`
+
+  This is useful to avoid repeated queries if you want to run `btac` many times
+  on the same (large) file.
+
+  By default, `btac` ignores any entry with a `BTACqueried` field. `--ignore-mark`
+  overrides this behavior.
+
+  When `--mark` is set, `btac` adds a `BTACqueried = {yyyy-mm-dd}` field to each entry
+  it queries.
+
+### Output formatting
 
 Unfortunately [bibtexparser](https://pypi.org/project/bibtexparser/) doesn't
 preserve format information, so this script will reformat your BibTeX file. Here
 are a few options you can use to control the output format:
 
 - `--fa --align-values` pad field names to align all values
 
@@ -212,15 +233,16 @@
   ```
 
 - `--fl --no-trailing-comma` don't add the last trailing comma
 - `--fi --indent <space>` space used for indentation, default is a tab.
   Can be specified as a number (number of spaces) or a string with spaces
   and `_`, `t`, and `n` characters to mark space, tabs and newlines.
 
-**Flags:**
+### Optional flags
+
 - `-i --inplace` Modify input files inplace, ignores any specified output files
 - `-p --prefix` Write new fields with a prefix. The script will add `BTACtitle =
   ...` instead of `title = ...` in the bib file. This can be combined with `-f`
   to safely show info for already present fields.
 
   Note that this can overwrite existing fields starting with `BTACxxxx`, even
   without the `-f` option.
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/__init__.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from typing import List
 
 from ..lookups.abstract_base import LookupType
 from .arxiv import ArxivLookup
 from .crossref import CrossrefLookup
 from .dblp import DBLPLookup
 from .researchr import ResearchrLookup
+from .semantic_scholar import SemanticScholarLookup
 from .unpaywall import UnpaywallLookup
 
 # List of lookup to use, in the order they will be used
 LOOKUPS: List[LookupType] = [
     CrossrefLookup,
     ArxivLookup,
+    SemanticScholarLookup,
     DBLPLookup,
     ResearchrLookup,
     UnpaywallLookup,
 ]
 LOOKUP_NAMES = [cls.name for cls in LOOKUPS]
 
 __all__ = (
     "LookupType",
     "LOOKUPS",
     "LOOKUP_NAMES",
     "CrossrefLookup",
+    "SemanticScholarLookup",
     "ArxivLookup",
     "DBLPLookup",
     "ResearchrLookup",
     "UnpaywallLookup",
 )
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/arxiv.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/arxiv.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/crossref.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/crossref.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..lookups.lookups import JSON_DAT_Lookup
 from ..utils.constants import QUERY_MAX_RESULTS
 from ..utils.safe_json import SafeJSON
 
 
 class CrossrefLookup(JSON_DAT_Lookup):
     """Lookup info on https://www.crossref.org
-    Uses the crossref REST API, documentated here:
+    Uses the crossref REST API, documented here:
     https://api.crossref.org/swagger-ui/index.html
 
     example URLs:
     DOI mode:
     https://api.crossref.org/works/10.1109/tro.2004.829459
     Author + title:
     https://api.crossref.org/works?rows=3&query.title=Reactive+Path+Deformation+for+Nonholonomic+Mobile+Robots&query.author=Lamiraux
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/dblp.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/dblp.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,22 @@
 
     @staticmethod
     def get_authors(info: SafeJSON) -> List[Author]:
         """Return a bibtex formatted list of authors"""
         authors = info["authors"]["author"]
         formatted = []
         for author in authors.iter_list():
-            aut = Author.from_name(author["text"].to_str())
+            name = author["text"].to_str()
+            if name is None:
+                continue
+            # Some DBLP authors have a 4-digit disambiguation number
+            # Added to their names..., ex : "Ralf Jung 0002"
+            if len(name) > 4 and name[-4:].isnumeric():
+                name = name[:-4].strip()
+            aut = Author.from_name(name)
             if aut is not None:
                 formatted.append(aut)
         return formatted
 
     def get_value(self, result: SafeJSON) -> BibtexEntry:
         info = result["info"]
         values = BibtexEntry()
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/doi.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/doi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Queries to https://doi.org/<doi>
 used to check that dois are valid
 """
 
 from typing import Optional
-from urllib.parse import quote, urlencode
+from urllib.parse import quote
 
 from ..bibtex.normalize import normalize_doi, normalize_str_weak, normalize_url
 from ..lookups.abstract_base import Data
 from ..lookups.condition_mixin import ConditionMixin
 from ..lookups.https import HTTPSRateCapedLookup, RedirectFollower
 from ..utils.logger import logger
 from ..utils.safe_json import SafeJSON
@@ -58,15 +58,15 @@
     silent_fail = True
 
     params = {"type": "URL"}
     domain = "doi.org"
     path = "/api/handles/"
 
     not_available_checks = [
-        "not available",
+        "doi not available",
         "not found",
     ]
 
     doi: str
 
     def __init__(self, input: str) -> None:
         self.input = input
@@ -75,16 +75,16 @@
         """Checks that a doi is valid"""
         doi = normalize_doi(self.input)
         if doi is not None:
             self.doi = doi
             return True
         return False
 
-    def get_path(self) -> str:
-        return self.path + quote(self.doi) + "?" + urlencode(self.params)
+    def get_base_path(self) -> str:
+        return self.path + quote(self.doi)
 
     def process_data(self, data: Data) -> Optional[bool]:
         if data.code != 200:
             return None
         json = SafeJSON.from_bytes(data.data)
         if json["responseCode"].to_int() != 1:
             return None
@@ -103,14 +103,15 @@
                 info = checker.response.headers
                 if info.get_content_maintype() != "text":
                     return True
                 # Some websites, namely springer, don't send 404 for invalid DOIs...
                 # See: https://link.springer.com/deleted
                 try:
                     text = normalize_str_weak(final.data.decode())
+                    for elem in self.not_available_checks:
+                        if elem in text:
+                            logger.debug("INVALID TEXT IN RESPONSE PAGE " + elem)
+                            return False
                 except UnicodeDecodeError:
                     logger.warn("Can't decode text content from URL {}".format(url))
-                for elem in self.not_available_checks:
-                    if elem in text:
-                        return False
                 return True
         return False
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/researchr.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/researchr.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
 
     name = "researchr"
 
     domain = "researchr.org"
     path = "/api/search/publication/"
 
-    def get_path(self) -> str:
+    def get_base_path(self) -> str:
         search = ""
         if self.author is not None:
             search += self.author + " "
         if self.title is not None:
             search += self.title + " "
         return self.path + quote_plus(search.strip())
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/APIs/unpaywall.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/APIs/unpaywall.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Lookup info from https://unpaywall.org/
 """
 
 from typing import Dict, Iterable, List, Optional
-from urllib.parse import urlencode
 
 from ..bibtex.author import Author
 from ..bibtex.entry import BibtexEntry, FieldNames
 from ..lookups.lookups import JSON_DT_Lookup
 from ..utils.constants import EMAIL
 from ..utils.safe_json import SafeJSON
 
@@ -40,20 +39,19 @@
         base = super().get_params()
         if self.doi is None:
             if self.title is None:
                 raise ValueError("query with no title or doi")
             base["query"] = self.title
         return base
 
-    def get_path(self) -> str:
+    def get_base_path(self) -> str:
         base = self.path
-        params = "?" + urlencode(self.get_params())
         if self.doi is not None:
-            return base + self.doi + params
-        return base + "search/" + params
+            return base + self.doi
+        return base + "search/"
 
     def get_results(self, data: bytes) -> Optional[Iterable[SafeJSON]]:
         json = SafeJSON.from_bytes(data)
         if self.doi is not None:
             # doi based search, single result if any
             return [json]
         return json["results"].iter_list()
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/author.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/author.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/entry.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/entry.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/io.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/io.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/matching.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/matching.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/bibtex/normalize.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/bibtex/normalize.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Functions used to normalize bibtex fields
 """
 
 import unicodedata
 from datetime import date
-from re import compile, search, sub
-from typing import Dict, List, Optional, Tuple
-from urllib.parse import parse_qsl, urlencode, urlsplit
+from re import search, sub
+from typing import Dict, Optional, Tuple
+from urllib.parse import parse_qsl, urlencode, urljoin, urlsplit
 
 from ..utils.constants import EntryType
+from ..utils.logger import logger
 
 
 def make_plain(value: Optional[str]) -> Optional[str]:
     """Returns a plain version of the field (remove redundant braces)
     returns None if the field is None or empty string"""
     if value is not None:
         plain = value.replace("{", "").replace("}", "").strip()
@@ -70,129 +71,14 @@
             prev_space = False
         elif not prev_space:
             res += " "
             prev_space = True
     return res.lower().strip()
 
 
-# 100 most common english words, from Wikipedia
-COMMON_WORDS = [
-    "the",
-    "be",
-    "to",
-    "of",
-    "and",
-    "a",
-    "in",
-    "that",
-    "have",
-    "i",
-    "it",
-    "for",
-    "not",
-    "on",
-    "with",
-    "he",
-    "as",
-    "you",
-    "do",
-    "at",
-    "this",
-    "but",
-    "his",
-    "by",
-    "from",
-    "they",
-    "we",
-    "say",
-    "her",
-    "she",
-    "or",
-    "an",
-    "will",
-    "my",
-    "one",
-    "all",
-    "would",
-    "there",
-    "their",
-    "what",
-    "so",
-    "up",
-    "out",
-    "if",
-    "about",
-    "who",
-    "get",
-    "which",
-    "go",
-    "me",
-    "when",
-    "make",
-    "can",
-    "like",
-    "time",
-    "no",
-    "just",
-    "him",
-    "know",
-    "take",
-    "people",
-    "into",
-    "year",
-    "your",
-    "good",
-    "some",
-    "could",
-    "them",
-    "see",
-    "other",
-    "than",
-    "then",
-    "now",
-    "look",
-    "only",
-    "come",
-    "its",
-    "over",
-    "think",
-    "also",
-    "back",
-    "after",
-    "use",
-    "two",
-    "how",
-    "our",
-    "work",
-    "first",
-    "well",
-    "way",
-    "even",
-    "new",
-    "want",
-    "because",
-    "any",
-    "these",
-    "give",
-    "day",
-    "most",
-    "us",
-]
-
-
-def keywords(title: str) -> List[str]:
-    """Returns only the best keywords in the given title"""
-    title = normalize_str(title)
-    words = []
-    for word in title.split(" "):
-        if word not in COMMON_WORDS:
-            words.append(word)
-    return words
-
-
 DOI_REGEX = r"(10\.\d{4,5}\/[\S]+[^;,.\s])$"
 
 
 def normalize_doi(doi_or_url: Optional[str]) -> Optional[str]:
     """Returns doi to canonical form (i.e. removing url)"""
     if doi_or_url is not None:
         match = search(DOI_REGEX, doi_or_url)
@@ -269,29 +155,27 @@
     months.update(get_locale_months())
     norm = normalize_str(month)
     if norm in months:
         return str(months[norm])
     return month
 
 
-URL_REGEX = compile(
-    "((http|https)://)(www.)?"
-    + "[a-zA-Z0-9@:%._\\+~#?&//=]"
-    + "{2,256}\\.[a-z]"
-    + "{2,6}\\b([-a-zA-Z0-9@:%"
-    + "._\\+~#?&//=]*)"
-)
-
-
-def normalize_url(url: str) -> Optional[Tuple[str, str]]:
+def normalize_url(
+    url: str, previous: Optional[str] = None
+) -> Optional[Tuple[str, str]]:
     """Splits and url into domain/path
     Returns none if url is not valid"""
-    if not search(URL_REGEX, url):
-        return None
+    url_copy = url
+    if previous is not None:
+        # resolve relative URLs
+        url = urljoin(previous, url)
     split = urlsplit(url)
-    if split.netloc == "":
+    if split.netloc == "" or split.scheme == "":
+        logger.debug(f"INVALID URL: {url_copy}, FROM {previous}")
         return None
     domain = split.netloc
     path = split.path
     if split.query != "":
         path += "?" + urlencode(parse_qsl(split.query))
+    if split.fragment != "":
+        path += "#" + split.fragment
     return domain, path
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/core/autocomplete.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/core/autocomplete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Bibtexautocomplete
 main class used to manage calls to different lookups
 """
 
+from datetime import datetime
 from functools import reduce
 from json import dump as json_dump
 from pathlib import Path
 from threading import Condition
 from typing import (
     Callable,
     Container,
@@ -23,15 +24,21 @@
 from bibtexparser.bibdatabase import BibDatabase
 
 from ..APIs.doi import DOICheck, URLCheck
 from ..bibtex.entry import BibtexEntry, FieldNames
 from ..bibtex.io import file_read, file_write, get_entries
 from ..bibtex.normalize import has_field
 from ..lookups.abstract_base import LookupType
-from ..utils.constants import BULLET, FIELD_PREFIX, MAX_THREAD_NB, EntryType
+from ..utils.constants import (
+    BULLET,
+    FIELD_PREFIX,
+    MARKED_FIELD,
+    MAX_THREAD_NB,
+    EntryType,
+)
 from ..utils.logger import VERBOSE_INFO, logger
 from ..utils.only_exclude import OnlyExclude
 from .data_dump import DataDump
 from .threads import LookupThread
 
 T = TypeVar("T")
 Q = TypeVar("Q")
@@ -55,14 +62,16 @@
 
     bibdatabases: List[BibDatabase]
     lookups: List[LookupType]
     fields: Container[str]
     entries: OnlyExclude[str]
     force_overwrite: bool
     prefix: str
+    mark: bool
+    filter: Callable[[EntryType], bool]
     dumps: List[DataDump]
 
     changed_fields: int
     changed_entries: int
 
     # Ordered list of (entry, changes) where
     # changes is a list of (field, new_value, source)
@@ -71,31 +80,40 @@
     def __init__(
         self,
         bibdatabases: List[BibDatabase],
         lookups: Iterable[LookupType],
         fields: Container[str],
         entries: OnlyExclude[str],
         force_overwrite: bool,
+        mark: bool = False,
+        ignore_mark: bool = False,
         prefix: bool = False,
     ):
         self.bibdatabases = bibdatabases
         self.lookups = list(lookups)
         self.fields = fields
         self.entries = entries
         self.force_overwrite = force_overwrite
         self.changed_entries = 0
         self.changed_fields = 0
         self.changes = []
         self.dumps = []
         self.prefix = FIELD_PREFIX if prefix else ""
+        self.mark = mark
+        if ignore_mark:
+            self.filter = lambda x: x["ID"] in self.entries
+        else:
+            self.filter = (
+                lambda x: x["ID"] in self.entries and MARKED_FIELD.lower() not in x
+            )
 
     def __iter__(self) -> Iterator[EntryType]:
         """Iterate through entries"""
         for db in self.bibdatabases:
-            yield from filter(lambda x: x["ID"] in self.entries, get_entries(db))
+            yield from filter(self.filter, get_entries(db))
 
     @memoize
     def count_entries(self) -> int:
         """count the number of entries"""
         # Its official, functional programming has infected me...
         return reduce(lambda x, _y: x + 1, self, 0)
 
@@ -202,14 +220,16 @@
             self.changes.append((entry["ID"], changes))
         logger.verbose_info(
             BULLET + "{StBold}{entry}{StBoldOff} {nb} new fields",
             entry=entry["ID"].ljust(self.get_id_padding()),
             nb=len(changes),
         )
         self.dumps.append(dump)
+        if self.mark:
+            entry[MARKED_FIELD] = datetime.today().strftime("%Y-%m-%d")
 
     def combine(self, entry: EntryType, new_info: BibtexEntry) -> Dict[str, str]:
         """Adds the information in info to entry.
         Does not overwrite unless self.force_overwrite is True
         only acts on fields contained in self.fields"""
         changes: Dict[str, str] = {}
         for field, value in new_info:
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/core/data_dump.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/core/data_dump.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/core/main.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/core/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 from ..APIs import LOOKUP_NAMES, LOOKUPS
 from ..bibtex.io import writer
 from ..lookups.condition_mixin import FieldConditionMixin
 from ..lookups.https import HTTPSLookup
 from ..utils.ansi import ANSICodes, ansi_format
 from ..utils.constants import (
     CONNECTION_TIMEOUT,
+    FIELD_PREFIX,
     LICENSE,
+    MARKED_FIELD,
     SCRIPT_NAME,
     URL,
     VERSION_DATE,
     VERSION_STR,
 )
+from ..utils.functions import list_sort_using, list_unduplicate
 from ..utils.logger import logger
 from ..utils.only_exclude import OnlyExclude
 from .autocomplete import BibtexAutocomplete
 from .parser import (
     HELP_TEXT,
     flatten,
     get_bibfiles,
@@ -47,14 +50,16 @@
                 TIMEOUT=CONNECTION_TIMEOUT,
                 VERSION=VERSION_STR,
                 VERSION_DATE=VERSION_DATE,
                 LOOKUPS=LOOKUP_NAMES,
                 NAME=SCRIPT_NAME,
                 URL=URL,
                 LICENSE=LICENSE,
+                MARKEDFIELD=MARKED_FIELD,
+                PREFIX=FIELD_PREFIX,
             )
         )
         return
     if args.version:
         print(
             "{NAME} version {VERSION} ({VERSION_DATE})".format(
                 NAME=SCRIPT_NAME, VERSION=VERSION_STR, VERSION_DATE=VERSION_DATE
@@ -86,24 +91,39 @@
     HTTPSLookup.connection_timeout = args.timeout if args.timeout > 0.0 else None
     HTTPSLookup.ignore_ssl = args.ignore_ssl
     lookups = (
         OnlyExclude[str]
         .from_nonempty(args.only_query, args.dont_query)
         .filter(LOOKUPS, lambda x: x.name)
     )
+    if args.only_query != []:
+        # remove duplicate from list
+        args.only_query, dups = list_unduplicate(args.only_query)
+        if dups:
+            # Print set without leading and ending brace
+            logger.warn("Duplicate '-q' arguments ignored: {set}", set=str(dups)[1:-1])
+        lookups = list_sort_using(lookups, args.only_query, lambda x: x.name)
+
     fields = OnlyExclude[str].from_nonempty(args.only_complete, args.dont_complete)
     entries = OnlyExclude[str].from_nonempty(args.only_entry, args.exclude_entry)
 
     FieldConditionMixin.fields_to_complete = set(
         fields.filter(FieldConditionMixin.fields_to_complete, lambda x: x)
     )
 
     databases = BibtexAutocomplete.read(args.input)
     completer = BibtexAutocomplete(
-        databases, lookups, fields, entries, args.force_overwrite, args.prefix
+        databases,
+        lookups,
+        fields,
+        entries,
+        args.force_overwrite,
+        mark=args.mark,
+        ignore_mark=args.ignore_mark,
+        prefix=args.prefix,
     )
     completer.print_filters()
     try:
         completer.autocomplete(args.verbose < 0)
         completer.print_changes()
         if args.dump_data is not None:
             completer.write_dumps(args.dump_data)
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/core/parser.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/core/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,16 +131,21 @@
 parser.add_argument("--comma-first", "--fc", action="store_true")
 parser.add_argument("--no-trailing-comma", "--fl", action="store_false")
 parser.add_argument("--indent", "--fi", default="\t")
 
 parser.add_argument("--force-overwrite", "-f", action="store_true")
 parser.add_argument("--prefix", "-p", action="store_true")
 parser.add_argument("--inplace", "-i", action="store_true")
+
+parser.add_argument("--mark", "-m", action="store_true")
+parser.add_argument("--ignore-mark", "-M", action="store_true")
+
 parser.add_argument("--timeout", "-t", type=float, default=CONNECTION_TIMEOUT)
 parser.add_argument("--verbose", "-v", action="count", default=0)
+
 parser.add_argument("--silent", "-s", action="store_true")
 parser.add_argument("--no-color", "-n", action="store_true")
 parser.add_argument("--ignore-ssl", "-S", action="store_true")
 
 parser.add_argument("--version", action="store_true")
 parser.add_argument("--help", "-h", action="store_true")
 
@@ -171,15 +176,16 @@
   {StBold}{FgYellow}{NAME}{Reset}                    same as 'btac .'
 
 {StBold}Optional arguments:{Reset} can all be used multiple times
   {FgYellow}-o --output{Reset} {FgGreen}<file.bib>{Reset}      Write output to given file
         With multiple input/outputs they are mapped in appearance order
         Extra inputs use default output name <filename>.btac.bib
 
-  {FgYellow}-q --only-query{Reset} {FgGreen}<website>{Reset}   Only query the given sites
+  {FgYellow}-q --only-query{Reset} {FgGreen}<website>{Reset}   Only query the given sites,
+        also change completion priority.
   {FgYellow}-Q --dont-query{Reset} {FgGreen}<website>{Reset}   Don't query the given sites
         Website must be one of: {LOOKUPS}
 
   {FgYellow}-e --only-entry{Reset}    {FgGreen}<id>{Reset}     Only perform lookup these entries
   {FgYellow}-E --exclude-entry{Reset} {FgGreen}<id>{Reset}     Don't perform lookup these entries
         ID is the identifier in bibtex (e.g. @inproceedings{{<id> ... }})
 
@@ -197,18 +203,22 @@
 
 {StBold}Flags:{Reset}
   {FgYellow}-i --inplace{Reset}          Modify input files inplace
         ignores any specified output files
   {FgYellow}-f --force-overwrite{Reset}  Overwrite already present fields
         The default is to overwrite a field if it is empty or absent
   {FgYellow}-p --prefix{Reset}           Write new fields with a prefix
-        eg: will write "BTACtitle = ..." instead of "title = ..." in the bib file.
+        eg: will write "{PREFIX}title = ..." instead of "title = ..." in the bib file.
         Can overwrite existing fields starting with BTACxxxx, even without the -f option.
         Can be combined with -f to safely show info for already present fields.
 
+  {FgYellow}-m --mark{Reset}             Add a "{MARKEDFIELD}" field to queried entries.
+        Entries with such a field are not queried in subsequent calls to btac
+  {FgYellow}-M --ignore-mark{Reset}      Also query entries with a "{MARKEDFIELD}" field
+
   {FgYellow}-t --timeout{Reset} {FgGreen}<float>{Reset}  set timeout on request, default: {TIMEOUT} s
         Set to -1 for no timeout.
   {FgYellow}-S --ignore-ssl{Reset}       Ignore SSL verification when performing queries
 
   {FgYellow}-d --dump-data{Reset} {FgGreen}<file.json>{Reset} writes all data from matching entries to
         the given file in JSON format, so data from multiple sources can be compared
   {FgYellow}-O --no-output{Reset}        Don't write any output files (except the --dump-data file)
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/core/threads.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/core/threads.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/abstract_base.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/abstract_base.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/condition_mixin.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/condition_mixin.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/https.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/https.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,27 @@
     def get_host(self) -> str:
         """Return the host header
         override this if not using self.host or self.domain"""
         if self.host is not None:
             return self.host
         return self.get_domain()
 
+    def get_base_path(self) -> str:
+        """Return the base path (without parameter)
+        default to simply using self.path"""
+        return self.path
+
     def get_path(self) -> str:
         """Return the path to connect to
         override this if not using self.path"""
         params = self.get_params()
+        path = self.get_base_path()
         if params:
-            return self.path + "?" + urlencode(params, safe=self.safe)
-        return self.path
+            return path + "?" + urlencode(params, safe=self.safe)
+        return path
 
     def get_params(self) -> Dict[str, str]:
         """Url parameters, can use self.entry to set them
         override this if not using self.path"""
         return self.params
 
     def get_body(self) -> Optional[Any]:
@@ -150,15 +156,15 @@
             delay = round(time() - start, 3)
             self._last_query_info = {
                 "url": url,
                 "response-time": delay,
                 "response-status": self.response.status,
             }
             logger.debug(
-                "response: {status}{reason} in {delay}s",
+                "response {status}{reason} in {delay}s",
                 status=self.response.status,
                 reason=" " + self.response.reason if self.response.reason else "",
                 delay=delay,
             )
             logger.very_verbose_debug(
                 "response headers: {headers}", headers=self.response.headers
             )
@@ -212,26 +218,26 @@
     Only works with fixed attributes for domain/path/query..."""
 
     max_depth = 10
     depth = 0
 
     def get_data(self) -> Optional[Data]:
         data = super().get_data()
-        while data is not None and data.code in [301, 302, 303]:
+        while data is not None and data.code in [301, 302, 303, 307]:
             if self.response is None:
                 return data
             location = self.response.getheader("Location")
             if location is None:
                 return data
             self.depth += 1
             logger.debug("Redirect {depth} to : {url}", depth=self.depth, url=location)
             if self.depth >= self.max_depth:
                 logger.warn("Redirection depth exceeded")
                 return None
-            split = normalize_url(location)
+            split = normalize_url(location, "https://" + self.domain + self.path)
             if split is None:
                 return data
             self.domain = split[0]
             self.path = split[1]
             data = super().get_data()
         return data
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/lookups.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/lookups.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/multiple_mixin.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/multiple_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     Performs parent queries if any
     then perform a single query if self.title is set
     """
 
     title: Optional[str] = None
 
     def iter_queries(self) -> Iterator[None]:
-        self.title = self.entry.title
+        self.title = (
+            None if self.entry.title is None else normalize_str(self.entry.title)
+        )
         # Perform parent queries with title set
         for x in super().iter_queries():
             yield x
         if self.title is not None:
             yield None
 
 
@@ -131,14 +133,14 @@
     - if authors, with all authors, with title (if any)
     - if authors, with each author individually, with title (if any)
     - if title, with title (if any)"""
 
     pass
 
 
-class DTQueryMixin(TitleAuthorQueryMixin, DOIQueryMixin):
+class DTQueryMixin(TitleQueryMixin, DOIQueryMixin):
     """DOI - Title Mixin
     queries in order:
     - if doi, with doi, with title (if any)
     - if title, with title (if any)"""
 
     pass
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/lookups/search_mixin.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/lookups/search_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         """
         Assign a score between ENTRY_NO_MATCH and ENTRY_CERTAIN_MATCH (included)
         representing how likely the given entries matches our search term
         - entry:BibtexEntry is self.get_value(res)
         - res:result is also passed in case get_value forgets some data.
         """
         raise NotImplementedError("should be overridden in child class")
-        return match_score(self.entry, entry)
 
     def process_data(self, data: Data) -> Optional[BibtexEntry]:
         """Iterate through results until one matches"""
         if data.code not in self.ok_codes:
             logger.warn(
                 "response: {FgYellow}{status}{reason}{Reset} in {delay}s",
                 status=data.code,
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/utils/ansi.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/utils/constants.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/utils/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 AUTHOR = "Dorian Lesbre"
 URL = "https://github.com/dlesbre/bibtex-autocomplete"
 ISSUES_URL = URL + "/issues"
 LICENSE = "MIT"
 DESCRIPTION = "Module to complete bibtex files by polling online databases"
 
 VERSION_MAJOR = 1
-VERSION_MINOR = 1
-VERSION_PATCH = 8
+VERSION_MINOR = 2
+VERSION_PATCH = 0
 
-VERSION_DATE = "2023-02-27"
+VERSION_DATE = "2023-04-14"
 
 VERSION = (VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH)
 VERSION_STR = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_PATCH}"
 
 EMAIL = "dorian.lesbre" + chr(64) + "gmail.com"
 
 # Minimum delay between queries to same host, to avoid surcharging server
@@ -41,9 +41,13 @@
 # Most APIs allow to limit the number of results returned for a search query
 # This allows for smaller data transfers
 QUERY_MAX_RESULTS = 10
 
 # Prefix added to fields with -p / --prefix option
 FIELD_PREFIX = "BTAC"
 
+# Field used to mark entries, the value is mostly irrelevant
+# As only field presence is tested
+MARKED_FIELD = FIELD_PREFIX + "queried"
+
 # Bullet printed to the screen when printing a list
 BULLET = "{FgBlue}{StBold}*{Reset} "
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/utils/logger.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 DEFAULT_LEVEL = logging.INFO
 
 
 def prefix_indent(prefix: str, message: str) -> str:
     """Adds a prefix to the first line of message
     Indents all subsequent lines with spaces to be aligned to prefix"""
     len = ansiless_len(prefix)
-    return prefix + message.replace("\n", "\n" + " " * len)
+    return ansi_format(prefix) + message.replace("\n", "\n" + " " * len)
 
 
 class Logger:
 
     logger: logging.Logger
 
     def __init__(self, logger_name: str) -> None:
@@ -65,18 +65,18 @@
         self.logger.setLevel(DEFAULT_LEVEL)
 
     @staticmethod
     def add_thread_info(message: str) -> str:
         """Add thread name to message if not in main thread"""
         current = current_thread()
         if current is not main_thread():
-            info = ansi_format("[{FgBlue}" + current.name + "{Reset}] ")
+            info = "[{FgBlue}" + current.name + "{Reset}] "
             entry_name = current.entry_name if hasattr(current, "entry_name") else None
             if isinstance(entry_name, str):
-                info += entry_name + ": "
+                info += "{StUnderline}" + entry_name + ":{Reset} "
             message = prefix_indent(info, message)
         return message
 
     def to_logger(self, level: int, message: str, *args: Any, **kwargs: Any) -> None:
         """Formats a message (with given args and ansi colors)
         and sends it to the logger with the given level"""
         message = self.add_thread_info(ansi_format(message, *args, **kwargs))
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/utils/only_exclude.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/utils/only_exclude.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete/utils/safe_json.py` & `bibtexautocomplete-1.2.0/bibtexautocomplete/utils/safe_json.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/PKG-INFO` & `bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtexautocomplete
-Version: 1.1.8
+Version: 1.2.0
 Summary: Module to complete bibtex files by polling online databases
 Home-page: https://github.com/dlesbre/bibtex-autocomplete
 Author: Dorian Lesbre
 Author-email: dorian.lesbre@gmail.com
 License: MIT
 Keywords: bibtex biblatex latex autocomplete btac
 Platform: any
@@ -27,21 +27,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: dev
 License-File: LICENSE
 
-<!-- LTeX: language=en -->
-
 # Bibtex Autocomplete
 
 [![PyPI version][version-shield]][pypi-link]
 [![PyPI pyversions][pyversion-shield]][pypi-link]
-[![License][license-shield]](./LICENSE)
+[![License][license-shield]](https://choosealicense.com/licenses/mit/)
 [![PyPI status][status-shield]][pypi-link]
 [![Downloads][download-shield]](https://pepy.tech/project/bibtexautocomplete)
 
 [![Maintenance][maintain-shield]][commit-link]
 [![Commit][commit-shield]][commit-link]
 [![actions][pipeline-shield]][pipeline-link]
 [![issues][issues-shield]][issues-link]
@@ -71,14 +69,15 @@
 bibliographies. It is inspired and expanding on the solution provided by
 [thando](https://tex.stackexchange.com/users/182467/thando) in this
 [TeX stack exchange post](https://tex.stackexchange.com/questions/6810/automatically-adding-doi-fields-to-a-hand-made-bibliography).
 
 It attempts to complete a BibTeX file by querying the following domains:
 - [www.crossref.org](https://www.crossref.org/)
 - [arxiv.org](https://arxiv.org/)
+- [semanticscholar.org](https://www.semanticscholar.org/)
 - [dlbp.org](https://dlbp.org)
 - [researchr.org](https://researchr.org/)
 - [unpaywall.org](https://unpaywall.org/)
 
 Big thanks to all of them for allowing open, easy and well-documented access to
 their databases.
 
@@ -86,14 +85,17 @@
 
 - [Demo](#demo)
 - [Quick overview](#quick-overview)
 - [Installation](#installation)
   - [Dependencies](#dependencies)
 - [Usage](#usage)
 - [Command line arguments](#command-line-arguments)
+  - [Query filtering](#query-filtering)
+  - [Output formatting](#output-formatting)
+  - [Optional flags](#optional-flags)
 
 ## Demo
 
 ![demo.svg](https://raw.githubusercontent.com/dlesbre/bibtex-autocomplete/2d1a01f5ec94c8af9c2f3c1a810eca51bb4cce74/imgs/demo.svg)
 
 ## Quick overview
 
@@ -123,19 +125,21 @@
   adding data from another similar-ish entry to your entry. If you find any such
   false positive please report them using the [issue
   tracker](https://github.com/dlesbre/bibtex-autocomplete/issues).
 
 **How are entries completed?**
 
 Once responses from all websites have been found, the script will add fields
-from website with the following priority : crossref > arxiv > dblp > researchr >
-unpaywall.
+from website with the following priority :
+
+crossref > arxiv > semantic scholar > dblp > researchr > unpaywall.
 
 So if both crossref's and dblp's response contain a publisher, the one from
-crossref will be used.
+crossref will be used. This order can be changed using the `-q --only-query`
+option (see [query filtering](#query-filtering)).
 
 The script will not overwrite any user given non-empty fields, unless the
 `-f/--force-overwrite` flag is given. If you want to check what fields are
 added, you can use `-v/--verbose` to have them printed to stdout (with
 source information), or `-p/--prefix` to have the new fields be prefixed with
 `BTAC` in the output file.
 
@@ -158,72 +162,89 @@
 ```
 
 ### Dependencies
 
 This package has two dependencies (automatically installed by pip) :
 
 - [bibtexparser](https://bibtexparser.readthedocs.io/)
-- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 2.4.0) for the fancy progress bar
+- [alive_progress](https://github.com/rsalmei/alive-progress) (>= 3.0.0) for the fancy progress bar
 
 ## Usage
 
 The command line tool can be used as follows:
 ```console
 btac [--flags] <input_files>
 ```
 
 **Examples :**
 
 - `btac my/db.bib` : reads from `./my/db.bib`, writes to `./my/db.btac.bib`
 - `btac -i db.bib` : reads from `db.bib` and overwrites it (inplace flag)
-- `btac db1.bib db2.bib -o out1.bib -o out2.bib` reads multiple files and write
-  their outputs to `out1.bib` and `out2.bib` respectively.
+- `btac db1.bib db2.bib db3.bib -o out1.bib -o out2.bib` reads `db1.bib`,
+  `db2.bib` and `db3.bib`, and write their outputs to `out1.bib`, `out2.bib`
+  and `db3.btac.bib` respectively.
 - `btac folder` : reads from all files ending with `.bib` in folder. Excludes
   `.btac.bib` files unless they are the only `.bib` files present. Writes to
   `folder/file.btac.bib` unless inplace flag is set.
 - `btac` with no inputs is same as `btac .`
+- `btac -v ...` verbose mode, pretty prints all new fields when done
 
 **Note:** the [parser](https://pypi.org/project/bibtexparser/) doesn't preserve
 format information, so this script will reformat your files. Some formatting
 options (see below) are provided.
 
 **Slow responses:** I found that crossref responds significantly slower than the
 other websites. It often takes longer than the 20s timeout.
 - You can increase timeout with `btac ... -t 60` (60s) or `btac ... -t -1` (no timeout)
 - You can disable crossref queries with `btac ... -Q crossref`
 
 ## Command line arguments
 
-**Optional arguments:**
-
 - `-o --output <file.bib>`
 
   Write output to given file. Can be used multiple times when also giving
   multiple inputs. Maps inputs to outputs in order. If there are extra inputs,
   uses default name (`old_name.btac.bib`). Ignored in inplace (`-i`) mode.
 
+### Query filtering
+
 - `-q --only-query <site>` or `-Q --dont-query <site>`
 
   Restrict which websites to query from. `<site>` must be one of: `crossref`,
-  `dblp`, `arxiv`, `researchr`, `unpaywall`. These arguments can be used
+  `arxiv`, `s2`, `dblp`, `researchr`, `unpaywall`. These arguments can be used
   multiple times, for example to only query crossref and dblp use `-q crossref
-  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv`
+  -q dblp` or `-Q researchr -Q unpaywall -Q arxiv -Q s2`
+
+  Additionally, you can use `-q` to change the completion priority.
+  So `-q unpaywall -q researchr -q dblp -q s2 -q arxiv -q crossref` reverses the
+  default order.
 
 - `-e --only-entry <id>` or `-E --exclude-entry <id>`
 
   Restrict which entries should be autocomplete. `<id>` is the entry ID used in
   your BibTeX file (e.g. `@inproceedings{<id> ... }`). These arguments can also
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
-**Output formatting:**
+- `-m --mark` and `-M --ignore-mark`
+
+  This is useful to avoid repeated queries if you want to run `btac` many times
+  on the same (large) file.
+
+  By default, `btac` ignores any entry with a `BTACqueried` field. `--ignore-mark`
+  overrides this behavior.
+
+  When `--mark` is set, `btac` adds a `BTACqueried = {yyyy-mm-dd}` field to each entry
+  it queries.
+
+### Output formatting
 
 Unfortunately [bibtexparser](https://pypi.org/project/bibtexparser/) doesn't
 preserve format information, so this script will reformat your BibTeX file. Here
 are a few options you can use to control the output format:
 
 - `--fa --align-values` pad field names to align all values
 
@@ -245,15 +266,16 @@
   ```
 
 - `--fl --no-trailing-comma` don't add the last trailing comma
 - `--fi --indent <space>` space used for indentation, default is a tab.
   Can be specified as a number (number of spaces) or a string with spaces
   and `_`, `t`, and `n` characters to mark space, tabs and newlines.
 
-**Flags:**
+### Optional flags
+
 - `-i --inplace` Modify input files inplace, ignores any specified output files
 - `-p --prefix` Write new fields with a prefix. The script will add `BTACtitle =
   ...` instead of `title = ...` in the bib file. This can be combined with `-f`
   to safely show info for already present fields.
 
   Note that this can overwrite existing fields starting with `BTACxxxx`, even
   without the `-f` option.
```

### Comparing `bibtexautocomplete-1.1.8/bibtexautocomplete.egg-info/SOURCES.txt` & `bibtexautocomplete-1.2.0/bibtexautocomplete.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 bibtexautocomplete.egg-info/top_level.txt
 bibtexautocomplete/APIs/__init__.py
 bibtexautocomplete/APIs/arxiv.py
 bibtexautocomplete/APIs/crossref.py
 bibtexautocomplete/APIs/dblp.py
 bibtexautocomplete/APIs/doi.py
 bibtexautocomplete/APIs/researchr.py
+bibtexautocomplete/APIs/semantic_scholar.py
 bibtexautocomplete/APIs/unpaywall.py
 bibtexautocomplete/bibtex/__init__.py
 bibtexautocomplete/bibtex/author.py
 bibtexautocomplete/bibtex/entry.py
 bibtexautocomplete/bibtex/io.py
 bibtexautocomplete/bibtex/matching.py
 bibtexautocomplete/bibtex/normalize.py
@@ -35,10 +36,11 @@
 bibtexautocomplete/lookups/https.py
 bibtexautocomplete/lookups/lookups.py
 bibtexautocomplete/lookups/multiple_mixin.py
 bibtexautocomplete/lookups/search_mixin.py
 bibtexautocomplete/utils/__init__.py
 bibtexautocomplete/utils/ansi.py
 bibtexautocomplete/utils/constants.py
+bibtexautocomplete/utils/functions.py
 bibtexautocomplete/utils/logger.py
 bibtexautocomplete/utils/only_exclude.py
 bibtexautocomplete/utils/safe_json.py
```

### Comparing `bibtexautocomplete-1.1.8/setup.py` & `bibtexautocomplete-1.2.0/setup.py`

 * *Files identical despite different names*

