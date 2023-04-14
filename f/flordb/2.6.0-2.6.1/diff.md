# Comparing `tmp/flordb-2.6.0.tar.gz` & `tmp/flordb-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.6.0.tar", last modified: Thu Mar 23 13:20:02 2023, max compression
+gzip compressed data, was "flordb-2.6.1.tar", last modified: Fri Apr 14 18:09:39 2023, max compression
```

## Comparing `flordb-2.6.0.tar` & `flordb-2.6.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.936062 flordb-2.6.0/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.0/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-03-23 13:20:02.935956 flordb-2.6.0/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.0/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.928197 flordb-2.6.0/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      206 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     5339 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.928690 flordb-2.6.0/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.929559 flordb-2.6.0/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.929716 flordb-2.6.0/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.930184 flordb-2.6.0/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.931279 flordb-2.6.0/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.931988 flordb-2.6.0/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.932617 flordb-2.6.0/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1742 2023-03-20 19:44:52.000000 flordb-2.6.0/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.933373 flordb-2.6.0/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)      897 2023-03-20 19:44:52.000000 flordb-2.6.0/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1318 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.0/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.934191 flordb-2.6.0/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     7921 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3658 2023-03-15 23:49:42.000000 flordb-2.6.0/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8773 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.934543 flordb-2.6.0/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.0/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2382 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3148 2023-03-23 13:19:05.000000 flordb-2.6.0/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.935258 flordb-2.6.0/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.0/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.0/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.0/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3767 2023-03-12 17:55:36.000000 flordb-2.6.0/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.0/flor/state.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-03-23 13:20:02.935824 flordb-2.6.0/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-03-23 13:20:02.000000 flordb-2.6.0/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1622 2023-03-23 13:20:02.000000 flordb-2.6.0/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-03-23 13:20:02.000000 flordb-2.6.0/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       61 2023-03-23 13:20:02.000000 flordb-2.6.0/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-03-23 13:20:02.000000 flordb-2.6.0/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-03-23 13:20:02.936094 flordb-2.6.0/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      841 2023-03-23 13:19:23.000000 flordb-2.6.0/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.536112 flordb-2.6.1/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.1/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-04-14 18:09:39.536006 flordb-2.6.1/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.1/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.528533 flordb-2.6.1/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      246 2023-04-04 22:53:53.000000 flordb-2.6.1/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     5339 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.528991 flordb-2.6.1/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.529984 flordb-2.6.1/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.530106 flordb-2.6.1/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.530479 flordb-2.6.1/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.531432 flordb-2.6.1/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.532243 flordb-2.6.1/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.532843 flordb-2.6.1/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.1/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.533558 flordb-2.6.1/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      897 2023-03-20 19:44:52.000000 flordb-2.6.1/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1318 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.1/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.534454 flordb-2.6.1/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7921 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3658 2023-03-15 23:49:42.000000 flordb-2.6.1/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8773 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.534787 flordb-2.6.1/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2382 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3148 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.535378 flordb-2.6.1/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.1/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.1/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.535865 flordb-2.6.1/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1636 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-04-14 18:09:39.536144 flordb-2.6.1/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-04-14 18:09:20.000000 flordb-2.6.1/setup.py
```

### Comparing `flordb-2.6.0/LICENSE` & `flordb-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/PKG-INFO` & `flordb-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.0
+Version: 2.6.1
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.0/README.md` & `flordb-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/constants.py` & `flordb-2.6.1/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/flags.py` & `flordb-2.6.1/flor/flags.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/__init__.py` & `flordb-2.6.1/flor/hlast/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gtpropagate.py` & `flordb-2.6.1/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/__init__.py` & `flordb-2.6.1/flor/hlast/gumtree/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/adapter.py` & `flordb-2.6.1/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/idmap.py` & `flordb-2.6.1/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/priorityq.py` & `flordb-2.6.1/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/python.py` & `flordb-2.6.1/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/test.py` & `flordb-2.6.1/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/gumtree/tree.py` & `flordb-2.6.1/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/hlast/visitors.py` & `flordb-2.6.1/flor/hlast/visitors.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/iterator.py` & `flordb-2.6.1/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/__init__.py` & `flordb-2.6.1/flor/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/__init__.py` & `flordb-2.6.1/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/abstract.py` & `flordb-2.6.1/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/data/abstract.py` & `flordb-2.6.1/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/data/dataframe.py` & `flordb-2.6.1/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/data/reference.py` & `flordb-2.6.1/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.6.1/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/data/value.py` & `flordb-2.6.1/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/metadata/bracket.py` & `flordb-2.6.1/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/entry/metadata/eof.py` & `flordb-2.6.1/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/tree/block.py` & `flordb-2.6.1/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/tree/group.py` & `flordb-2.6.1/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/tree/tree.py` & `flordb-2.6.1/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/journal/tree/window.py` & `flordb-2.6.1/flor/journal/tree/window.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/kits.py` & `flordb-2.6.1/flor/kits.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,13 +43,21 @@
                     yield each
                     State.seconds["EPOCHS"].append(time() - start_time)
             else:
                 assert State.loop_nesting_level > 1
                 # Nested loop
                 if SkipBlock.step_into(name, probed):
                     assert State.step is not None
-                    for each in iter8r:
-                        State.step += 1
-                        yield each
-                SkipBlock.end(*MTK.chckpts)
+                    try:
+                        while True:
+                            each = next(iter8r)
+                            State.step += 1
+                            yield each
+                    except StopIteration:
+                        pass
+                    finally:
+                        SkipBlock.end(*MTK.chckpts)
+                else:
+                    SkipBlock.end(*MTK.chckpts)
+
         finally:
             State.loop_nesting_level -= 1
```

### Comparing `flordb-2.6.0/flor/logger/__init__.py` & `flordb-2.6.1/flor/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/logger/checkpoint_logger.py` & `flordb-2.6.1/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/logger/exp_json.py` & `flordb-2.6.1/flor/logger/exp_json.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/logger/future.py` & `flordb-2.6.1/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/logger/log_records.py` & `flordb-2.6.1/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/query/__init__.py` & `flordb-2.6.1/flor/query/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/query/database.py` & `flordb-2.6.1/flor/query/database.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/query/engine.py` & `flordb-2.6.1/flor/query/engine.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/query/pivot.py` & `flordb-2.6.1/flor/query/pivot.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/query/unpack.py` & `flordb-2.6.1/flor/query/unpack.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/shelf/cwd_shelf.py` & `flordb-2.6.1/flor/shelf/cwd_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/shelf/home_shelf.py` & `flordb-2.6.1/flor/shelf/home_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/skipblock/abstract.py` & `flordb-2.6.1/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/skipblock/readblock.py` & `flordb-2.6.1/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flor/skipblock/writeblock.py` & `flordb-2.6.1/flor/skipblock/writeblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         # Must align successor checkpoints for periodic checkpointing
         if block.force_mat:
             return True
 
         # First consider atomic case (always/never)
         ratio = block_group.materialization_time / block_group.computation_time
-        threshold = min(1 / (1 + WriteBlock.scaling_factor), flags.EPSILON)
+        threshold = min(1 / (1 + WriteBlock.scaling_factor), flags.EPSILON)  # type: ignore
         if ratio < threshold:
             return True
 
         # Then account for parallelism speedup
         if block.parent is None:
             threshold *= block_group.executions_count / (
                 block_group.materializations_count + 1
@@ -97,10 +97,10 @@
         return DataVal(lbracket.sk, lbracket.gk, arg)
     elif isinstance(arg, pd.DataFrame):
         return DataFrame(lbracket.sk, lbracket.gk, arg)
     else:
         if hasattr(arg, "state_dict"):
             try:
                 return Torch(lbracket.sk, lbracket.gk, arg.state_dict())  # type: ignore
-            except:
-                pass
+            except Exception as e:
+                print("for debugging", e)
         return DataRef(lbracket.sk, lbracket.gk, arg)
```

### Comparing `flordb-2.6.0/flor/state.py` & `flordb-2.6.1/flor/state.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.0/flordb.egg-info/PKG-INFO` & `flordb-2.6.1/flordb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.0
+Version: 2.6.1
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.0/flordb.egg-info/SOURCES.txt` & `flordb-2.6.1/flordb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 flor/__init__.py
 flor/constants.py
 flor/flags.py
 flor/iterator.py
 flor/kits.py
 flor/state.py
+flor/utils.py
 flor/hlast/__init__.py
 flor/hlast/gtpropagate.py
 flor/hlast/visitors.py
 flor/hlast/gumtree/__init__.py
 flor/hlast/gumtree/adapter.py
 flor/hlast/gumtree/idmap.py
 flor/hlast/gumtree/priorityq.py
```

### Comparing `flordb-2.6.0/setup.py` & `flordb-2.6.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.6.0",
+    version="2.6.1",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
     install_requires=[
         "GitPython",
         "cloudpickle",
         "astunparse",
         "pandas",
         "bidict==0.21.3",
         "apted",
+        "matplotlib",
+        "scikit-learn",
+        "numpy",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
```

