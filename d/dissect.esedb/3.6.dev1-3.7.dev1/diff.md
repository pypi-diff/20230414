# Comparing `tmp/dissect.esedb-3.6.dev1.tar.gz` & `tmp/dissect.esedb-3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.esedb-3.6.dev1.tar", last modified: Thu Mar 16 13:02:55 2023, max compression
+gzip compressed data, was "dissect.esedb-3.7.dev1.tar", last modified: Fri Apr 14 11:34:08 2023, max compression
```

## Comparing `dissect.esedb-3.6.dev1.tar` & `dissect.esedb-3.7.dev1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.122067 dissect.esedb-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-16 13:02:55.122067 dissect.esedb-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.106066 dissect.esedb-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.114066 dissect.esedb-3.6.dev1/dissect/esedb/
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/c_esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/cursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3357 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/lcmapstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17144 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/record.py
--rw-r--r--   0 runner    (1001) docker     (123)   819383 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/sorting_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.114066 dissect.esedb-3.6.dev1/dissect/esedb/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/tools/impacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/tools/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/dissect/esedb/tools/ual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.110067 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-16 13:02:55.000000 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-16 13:02:55.000000 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:02:55.000000 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:02:55.000000 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:02:55.000000 dissect.esedb-3.6.dev1/dissect.esedb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-16 13:02:43.000000 dissect.esedb-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:02:55.122067 dissect.esedb-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.118067 dissect.esedb-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:55.122067 dissect.esedb-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    56705 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/Current.mdb.gz
--rw-r--r--   0 runner    (1001) docker     (123)    52655 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/SRUDB.dat.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)     9771 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/basic.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)     9913 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/binary.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/default.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    12993 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/index.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)  2009304 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/large.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/multi.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)    11790 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/data/text.edb.gz
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/test_esedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/test_sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tests/test_ual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:02:39.000000 dissect.esedb-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.868126 dissect.esedb-3.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-14 11:34:08.868126 dissect.esedb-3.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.852126 dissect.esedb-3.7.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.860127 dissect.esedb-3.7.dev1/dissect/esedb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/c_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/cursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3357 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/lcmapstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17144 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)   819383 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/sorting_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.864127 dissect.esedb-3.7.dev1/dissect/esedb/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/tools/impacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/tools/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/dissect/esedb/tools/ual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.856126 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-14 11:34:08.000000 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 11:34:08.000000 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:34:08.000000 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 11:34:08.000000 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 11:34:08.000000 dissect.esedb-3.7.dev1/dissect.esedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 11:33:59.000000 dissect.esedb-3.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:34:08.872127 dissect.esedb-3.7.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.864127 dissect.esedb-3.7.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.868126 dissect.esedb-3.7.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    56705 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/Current.mdb.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    52655 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/SRUDB.dat.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9771 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/basic.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9913 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/binary.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/default.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12993 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/index.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2009304 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/large.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/multi.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11790 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/data/text.edb.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/test_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/test_sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tests/test_ual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-14 11:33:55.000000 dissect.esedb-3.7.dev1/tox.ini
```

### Comparing `dissect.esedb-3.6.dev1/LICENSE` & `dissect.esedb-3.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/PKG-INFO` & `dissect.esedb-3.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.esedb
-Version: 3.6.dev1
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
 Project-URL: repository, https://github.com/fox-it/dissect.esedb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.esedb-3.6.dev1/README.md` & `dissect.esedb-3.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/c_esedb.py` & `dissect.esedb-3.7.dev1/dissect/esedb/c_esedb.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     BYTE        fTimeIsUTC:1;
     BYTE        bMillisecondsLow:7;
 
     BYTE        fReserved:1;                        // fOSSnapshot
     BYTE        bMillisecondsHigh:3;
     BYTE        fUnused:4;
-}
+};
 
 struct LGPOS {
     USHORT      ib;                                 // must be the last so that lgpos can
     USHORT      isec;                               // index of disksec starting logsec
     LONG        lGeneration;                        // generation of logsec
 };
```

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/compression.py` & `dissect.esedb-3.7.dev1/dissect/esedb/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/cursor.py` & `dissect.esedb-3.7.dev1/dissect/esedb/cursor.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/esedb.py` & `dissect.esedb-3.7.dev1/dissect/esedb/esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/index.py` & `dissect.esedb-3.7.dev1/dissect/esedb/index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/lcmapstring.py` & `dissect.esedb-3.7.dev1/dissect/esedb/lcmapstring.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/page.py` & `dissect.esedb-3.7.dev1/dissect/esedb/page.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/record.py` & `dissect.esedb-3.7.dev1/dissect/esedb/record.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/sorting_table.py` & `dissect.esedb-3.7.dev1/dissect/esedb/sorting_table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/table.py` & `dissect.esedb-3.7.dev1/dissect/esedb/table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/tools/impacket.py` & `dissect.esedb-3.7.dev1/dissect/esedb/tools/impacket.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/tools/sru.py` & `dissect.esedb-3.7.dev1/dissect/esedb/tools/sru.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect/esedb/tools/ual.py` & `dissect.esedb-3.7.dev1/dissect/esedb/tools/ual.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/dissect.esedb.egg-info/PKG-INFO` & `dissect.esedb-3.7.dev1/dissect.esedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.esedb
-Version: 3.6.dev1
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
 Project-URL: repository, https://github.com/fox-it/dissect.esedb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.esedb-3.6.dev1/dissect.esedb.egg-info/SOURCES.txt` & `dissect.esedb-3.7.dev1/dissect.esedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/pyproject.toml` & `dissect.esedb-3.7.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/conftest.py` & `dissect.esedb-3.7.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/Current.mdb.gz` & `dissect.esedb-3.7.dev1/tests/data/Current.mdb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/SRUDB.dat.gz` & `dissect.esedb-3.7.dev1/tests/data/SRUDB.dat.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/basic.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/basic.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/binary.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/binary.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/default.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/default.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/index.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/index.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/large.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/large.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/multi.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/multi.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/data/text.edb.gz` & `dissect.esedb-3.7.dev1/tests/data/text.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/test_esedb.py` & `dissect.esedb-3.7.dev1/tests/test_esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tests/test_index.py` & `dissect.esedb-3.7.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.6.dev1/tox.ini` & `dissect.esedb-3.7.dev1/tox.ini`

 * *Files identical despite different names*

