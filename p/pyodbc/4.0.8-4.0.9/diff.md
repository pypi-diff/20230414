# Comparing `tmp/pyodbc-4.0.8.tar.gz` & `tmp/pyodbc-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyodbc-4.0.8.tar", last modified: Fri Feb 17 23:15:56 2017, max compression
+gzip compressed data, was "dist/pyodbc-4.0.9.tar", last modified: Sun Feb 19 00:03:27 2017, max compression
```

## Comparing `pyodbc-4.0.8.tar` & `pyodbc-4.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-17 23:15:56.000000 pyodbc-4.0.8/
--rw-r--r--   0 mkleehammer   (501) staff       (20)      868 2016-11-28 20:51:34.000000 pyodbc-4.0.8/LICENSE.txt
--rw-r--r--   0 mkleehammer   (501) staff       (20)      177 2016-11-28 20:51:34.000000 pyodbc-4.0.8/MANIFEST.in
--rw-r--r--   0 mkleehammer   (501) staff       (20)      857 2017-02-17 23:15:56.000000 pyodbc-4.0.8/PKG-INFO
-drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-17 23:15:56.000000 pyodbc-4.0.8/pyodbc.egg-info/
--rw-r--r--   0 mkleehammer   (501) staff       (20)        1 2017-02-17 23:15:56.000000 pyodbc-4.0.8/pyodbc.egg-info/dependency_links.txt
--rw-r--r--   0 mkleehammer   (501) staff       (20)      857 2017-02-17 23:15:56.000000 pyodbc-4.0.8/pyodbc.egg-info/PKG-INFO
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1232 2017-02-17 23:15:56.000000 pyodbc-4.0.8/pyodbc.egg-info/SOURCES.txt
--rw-r--r--   0 mkleehammer   (501) staff       (20)        7 2017-02-17 23:15:56.000000 pyodbc-4.0.8/pyodbc.egg-info/top_level.txt
--rw-r--r--   0 mkleehammer   (501) staff       (20)      385 2016-11-29 03:06:28.000000 pyodbc-4.0.8/README.md
--rw-r--r--   0 mkleehammer   (501) staff       (20)      347 2017-02-17 23:15:56.000000 pyodbc-4.0.8/setup.cfg
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    10259 2017-02-16 21:48:30.000000 pyodbc-4.0.8/setup.py
-drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-17 23:15:56.000000 pyodbc-4.0.8/src/
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1970 2016-11-28 20:51:34.000000 pyodbc-4.0.8/src/buffer.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     2182 2016-11-28 20:51:34.000000 pyodbc-4.0.8/src/buffer.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     6552 2017-02-17 23:01:09.000000 pyodbc-4.0.8/src/cnxninfo.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1886 2017-01-19 20:15:35.000000 pyodbc-4.0.8/src/cnxninfo.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)    45097 2017-02-16 21:44:28.000000 pyodbc-4.0.8/src/connection.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4902 2017-02-11 03:36:18.000000 pyodbc-4.0.8/src/connection.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)    74489 2017-02-16 21:48:52.000000 pyodbc-4.0.8/src/cursor.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     5880 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/cursor.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)      710 2017-02-11 02:59:28.000000 pyodbc-4.0.8/src/dbspecific.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     8950 2016-11-29 03:06:28.000000 pyodbc-4.0.8/src/errors.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     2521 2016-11-28 20:51:34.000000 pyodbc-4.0.8/src/errors.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)    23327 2017-02-17 21:52:28.000000 pyodbc-4.0.8/src/getdata.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)      411 2017-02-11 03:36:18.000000 pyodbc-4.0.8/src/getdata.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)    28689 2017-02-17 23:10:07.000000 pyodbc-4.0.8/src/params.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)      240 2016-11-28 20:51:34.000000 pyodbc-4.0.8/src/params.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4047 2017-01-19 20:15:35.000000 pyodbc-4.0.8/src/pyodbc.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)      957 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/pyodbccompat.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4625 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/pyodbccompat.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4977 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/pyodbcdbg.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)    39087 2017-02-11 03:49:36.000000 pyodbc-4.0.8/src/pyodbcmodule.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1922 2017-02-11 03:36:18.000000 pyodbc-4.0.8/src/pyodbcmodule.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)      386 2016-11-28 20:51:34.000000 pyodbc-4.0.8/src/resource.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)    17167 2017-01-20 19:04:17.000000 pyodbc-4.0.8/src/row.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1594 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/row.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     2651 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/sqlwchar.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4127 2017-02-11 03:36:18.000000 pyodbc-4.0.8/src/textenc.cpp
--rw-r--r--   0 mkleehammer   (501) staff       (20)     2295 2017-02-16 21:34:41.000000 pyodbc-4.0.8/src/textenc.h
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1593 2016-12-30 15:36:36.000000 pyodbc-4.0.8/src/wrapper.h
-drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-17 23:15:56.000000 pyodbc-4.0.8/tests2/
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    22760 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/accesstests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    31431 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/dbapi20.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)     1406 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/dbapitests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)   311296 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/empty.accdb
--rw-r--r--   0 mkleehammer   (501) staff       (20)   188416 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/empty.mdb
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)     4592 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/exceltests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    46182 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/freetdstests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    46546 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/informixtests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    25855 2016-12-30 15:36:36.000000 pyodbc-4.0.8/tests2/mysqltests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    19373 2017-01-13 23:42:32.000000 pyodbc-4.0.8/tests2/pgtests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     2048 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/sqlite.db
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    28150 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/sqlitetests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    55848 2017-01-13 23:22:32.000000 pyodbc-4.0.8/tests2/sqlservertests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)     1084 2016-12-30 15:36:36.000000 pyodbc-4.0.8/tests2/test.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)    17920 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/test.xls
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)      819 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests2/testbase.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)     3954 2016-12-30 15:36:36.000000 pyodbc-4.0.8/tests2/testutils.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4531 2017-01-19 20:16:37.000000 pyodbc-4.0.8/tests2/testutils.pyc
-drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-17 23:15:56.000000 pyodbc-4.0.8/tests3/
--rw-r--r--   0 mkleehammer   (501) staff       (20)    21519 2017-02-17 23:01:09.000000 pyodbc-4.0.8/tests3/accesstests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)    31431 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/dbapi20.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     1406 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/dbapitests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     4592 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/exceltests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)    46014 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/informixtests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    25955 2017-02-17 23:01:09.000000 pyodbc-4.0.8/tests3/mysqltests.py
--rwxr-xr-x   0 mkleehammer   (501) staff       (20)    18767 2017-02-17 23:01:09.000000 pyodbc-4.0.8/tests3/pgtests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)    25949 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/sqlitetests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)    49221 2017-02-11 03:36:18.000000 pyodbc-4.0.8/tests3/sqlservertests.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)      333 2017-02-16 21:50:15.000000 pyodbc-4.0.8/tests3/test.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)      819 2016-11-28 20:51:34.000000 pyodbc-4.0.8/tests3/testbase.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     3756 2016-12-30 15:36:36.000000 pyodbc-4.0.8/tests3/testutils.py
--rw-r--r--   0 mkleehammer   (501) staff       (20)     3985 2016-12-01 23:14:54.000000 pyodbc-4.0.8/tests3/testutils.pyc
+drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-19 00:03:27.000000 pyodbc-4.0.9/
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      868 2016-11-28 20:51:34.000000 pyodbc-4.0.9/LICENSE.txt
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      177 2016-11-28 20:51:34.000000 pyodbc-4.0.9/MANIFEST.in
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      857 2017-02-19 00:03:27.000000 pyodbc-4.0.9/PKG-INFO
+drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-19 00:03:27.000000 pyodbc-4.0.9/pyodbc.egg-info/
+-rw-r--r--   0 mkleehammer   (501) staff       (20)        1 2017-02-19 00:03:27.000000 pyodbc-4.0.9/pyodbc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      857 2017-02-19 00:03:27.000000 pyodbc-4.0.9/pyodbc.egg-info/PKG-INFO
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1232 2017-02-19 00:03:27.000000 pyodbc-4.0.9/pyodbc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkleehammer   (501) staff       (20)        7 2017-02-19 00:03:27.000000 pyodbc-4.0.9/pyodbc.egg-info/top_level.txt
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      574 2017-02-18 17:08:23.000000 pyodbc-4.0.9/README.md
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      347 2017-02-19 00:03:27.000000 pyodbc-4.0.9/setup.cfg
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    10259 2017-02-16 21:48:30.000000 pyodbc-4.0.9/setup.py
+drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-19 00:03:27.000000 pyodbc-4.0.9/src/
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1970 2016-11-28 20:51:34.000000 pyodbc-4.0.9/src/buffer.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2182 2016-11-28 20:51:34.000000 pyodbc-4.0.9/src/buffer.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     6552 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/cnxninfo.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1886 2017-01-19 20:15:35.000000 pyodbc-4.0.9/src/cnxninfo.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    45097 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/connection.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4902 2017-02-18 22:48:22.000000 pyodbc-4.0.9/src/connection.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    74489 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/cursor.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     5880 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/cursor.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1244 2017-02-19 00:02:39.000000 pyodbc-4.0.9/src/dbspecific.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     8950 2016-11-29 03:06:28.000000 pyodbc-4.0.9/src/errors.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2521 2016-11-28 20:51:34.000000 pyodbc-4.0.9/src/errors.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    24649 2017-02-19 00:02:39.000000 pyodbc-4.0.9/src/getdata.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      411 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/getdata.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    29421 2017-02-19 00:02:39.000000 pyodbc-4.0.9/src/params.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      240 2016-11-28 20:51:34.000000 pyodbc-4.0.9/src/params.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4047 2017-01-19 20:15:35.000000 pyodbc-4.0.9/src/pyodbc.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      957 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/pyodbccompat.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4625 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/pyodbccompat.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4977 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/pyodbcdbg.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    39577 2017-02-19 00:02:39.000000 pyodbc-4.0.9/src/pyodbcmodule.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2066 2017-02-19 00:02:39.000000 pyodbc-4.0.9/src/pyodbcmodule.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      386 2016-11-28 20:51:34.000000 pyodbc-4.0.9/src/resource.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    17167 2017-01-20 19:04:17.000000 pyodbc-4.0.9/src/row.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1594 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/row.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2651 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/sqlwchar.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4127 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/textenc.cpp
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2295 2017-02-18 17:08:23.000000 pyodbc-4.0.9/src/textenc.h
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1593 2016-12-30 15:36:36.000000 pyodbc-4.0.9/src/wrapper.h
+drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-19 00:03:27.000000 pyodbc-4.0.9/tests2/
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    22760 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/accesstests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    31431 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/dbapi20.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)     1406 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/dbapitests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)   311296 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/empty.accdb
+-rw-r--r--   0 mkleehammer   (501) staff       (20)   188416 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/empty.mdb
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)     4592 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/exceltests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    46182 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/freetdstests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    46546 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/informixtests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    25855 2016-12-30 15:36:36.000000 pyodbc-4.0.9/tests2/mysqltests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    19373 2017-01-13 23:42:32.000000 pyodbc-4.0.9/tests2/pgtests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     2048 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/sqlite.db
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    28150 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/sqlitetests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    56531 2017-02-19 00:02:39.000000 pyodbc-4.0.9/tests2/sqlservertests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)     1084 2016-12-30 15:36:36.000000 pyodbc-4.0.9/tests2/test.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    17920 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/test.xls
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)      819 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests2/testbase.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)     3954 2016-12-30 15:36:36.000000 pyodbc-4.0.9/tests2/testutils.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4531 2017-01-19 20:16:37.000000 pyodbc-4.0.9/tests2/testutils.pyc
+drwxr-xr-x   0 mkleehammer   (501) staff       (20)        0 2017-02-19 00:03:27.000000 pyodbc-4.0.9/tests3/
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    21519 2017-02-18 17:08:23.000000 pyodbc-4.0.9/tests3/accesstests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    31431 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/dbapi20.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     1406 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/dbapitests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     4592 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/exceltests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    46014 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/informixtests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    25955 2017-02-18 17:08:23.000000 pyodbc-4.0.9/tests3/mysqltests.py
+-rwxr-xr-x   0 mkleehammer   (501) staff       (20)    18767 2017-02-18 17:08:23.000000 pyodbc-4.0.9/tests3/pgtests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    25949 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/sqlitetests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)    49899 2017-02-19 00:02:39.000000 pyodbc-4.0.9/tests3/sqlservertests.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      333 2017-02-16 21:50:15.000000 pyodbc-4.0.9/tests3/test.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)      819 2016-11-28 20:51:34.000000 pyodbc-4.0.9/tests3/testbase.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     3756 2016-12-30 15:36:36.000000 pyodbc-4.0.9/tests3/testutils.py
+-rw-r--r--   0 mkleehammer   (501) staff       (20)     3985 2016-12-01 23:14:54.000000 pyodbc-4.0.9/tests3/testutils.pyc
```

### Comparing `pyodbc-4.0.8/LICENSE.txt` & `pyodbc-4.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/PKG-INFO` & `pyodbc-4.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyodbc
-Version: 4.0.8
+Version: 4.0.9
 Summary: DB API Module for ODBC
 Home-page: https://github.com/mkleehammer/pyodbc
 Author: Michael Kleehammer
 Author-email: michael@kleehammer.com
 License: MIT
 Description: A Python DB API 2 module for ODBC. This project provides an up-to-date, convenient interface to ODBC using native data types like datetime and decimal.
 Platform: UNKNOWN
```

### Comparing `pyodbc-4.0.8/pyodbc.egg-info/PKG-INFO` & `pyodbc-4.0.9/pyodbc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyodbc
-Version: 4.0.8
+Version: 4.0.9
 Summary: DB API Module for ODBC
 Home-page: https://github.com/mkleehammer/pyodbc
 Author: Michael Kleehammer
 Author-email: michael@kleehammer.com
 License: MIT
 Description: A Python DB API 2 module for ODBC. This project provides an up-to-date, convenient interface to ODBC using native data types like datetime and decimal.
 Platform: UNKNOWN
```

### Comparing `pyodbc-4.0.8/pyodbc.egg-info/SOURCES.txt` & `pyodbc-4.0.9/pyodbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/setup.py` & `pyodbc-4.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/buffer.cpp` & `pyodbc-4.0.9/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/buffer.h` & `pyodbc-4.0.9/src/buffer.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/cnxninfo.cpp` & `pyodbc-4.0.9/src/cnxninfo.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/cnxninfo.h` & `pyodbc-4.0.9/src/cnxninfo.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/connection.cpp` & `pyodbc-4.0.9/src/connection.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/connection.h` & `pyodbc-4.0.9/src/connection.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/cursor.cpp` & `pyodbc-4.0.9/src/cursor.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/cursor.h` & `pyodbc-4.0.9/src/cursor.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/errors.cpp` & `pyodbc-4.0.9/src/errors.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/errors.h` & `pyodbc-4.0.9/src/errors.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/getdata.cpp` & `pyodbc-4.0.9/src/getdata.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -568,14 +568,41 @@
     if (cbFetched == SQL_NULL_DATA)
         Py_RETURN_NONE;
 
     int micros = (int)(value.fraction / 1000); // nanos --> micros
     return PyTime_FromTime(value.hour, value.minute, value.second, micros);
 }
 
+static PyObject* GetUUID(Cursor* cur, Py_ssize_t iCol)
+{
+    // REVIEW: Since GUID is a fixed size, do we need to pass the size or cbFetched?
+
+    PYSQLGUID guid;
+    SQLLEN cbFetched = 0;
+    SQLRETURN ret;
+    Py_BEGIN_ALLOW_THREADS
+    ret = SQLGetData(cur->hstmt, (SQLUSMALLINT)(iCol+1), SQL_GUID, &guid, sizeof(guid), &cbFetched);
+    Py_END_ALLOW_THREADS
+
+    if (!SQL_SUCCEEDED(ret))
+        return RaiseErrorFromHandle("SQLGetData", cur->cnxn->hdbc, cur->hstmt);
+
+    if (cbFetched == SQL_NULL_DATA)
+        Py_RETURN_NONE;
+
+#if PY_MAJOR_VERSION >= 3
+    const char* szFmt = "(yyy#)";
+#else
+    const char* szFmt = "(sss#)";
+#endif
+    Object args = Py_BuildValue(szFmt, NULL, NULL, &guid, (int)sizeof(guid));
+    if (!args)
+        return 0;
+    return PyObject_CallObject(uuid_type, args.Get());
+}
 
 static PyObject* GetDataTimestamp(Cursor* cur, Py_ssize_t iCol)
 {
     TIMESTAMP_STRUCT value;
 
     SQLLEN cbFetched = 0;
     SQLRETURN ret;
@@ -638,25 +665,42 @@
     PyObject* pytype = 0;
 
     switch (type)
     {
     case SQL_CHAR:
     case SQL_VARCHAR:
     case SQL_LONGVARCHAR:
-    case SQL_GUID:
 #if PY_MAJOR_VERSION < 3
         if (cur->cnxn->str_enc.ctype == SQL_C_CHAR)
             pytype = (PyObject*)&PyString_Type;
         else
             pytype = (PyObject*)&PyUnicode_Type;
 #else
         pytype = (PyObject*)&PyUnicode_Type;
 #endif
         break;
 
+    case SQL_GUID:
+        if (UseNativeUUID())
+        {
+            pytype = uuid_type;
+        }
+        else
+        {
+#if PY_MAJOR_VERSION < 3
+            if (cur->cnxn->str_enc.ctype == SQL_C_CHAR)
+                pytype = (PyObject*)&PyString_Type;
+            else
+                pytype = (PyObject*)&PyUnicode_Type;
+#else
+            pytype = (PyObject*)&PyUnicode_Type;
+#endif
+        }
+        break;
+
     case SQL_WCHAR:
     case SQL_WVARCHAR:
     case SQL_WLONGVARCHAR:
     case SQL_SS_XML:
         pytype = (PyObject*)&PyUnicode_Type;
         break;
 
@@ -734,18 +778,23 @@
     case SQL_WVARCHAR:
     case SQL_WLONGVARCHAR:
         return GetText(cur, iCol);
 
     case SQL_CHAR:
     case SQL_VARCHAR:
     case SQL_LONGVARCHAR:
-    case SQL_GUID:
     case SQL_SS_XML:
         return GetText(cur, iCol);
 
+    case SQL_GUID:
+        if (UseNativeUUID())
+            return GetUUID(cur, iCol);
+        return GetText(cur, iCol);
+        break;
+
     case SQL_BINARY:
     case SQL_VARBINARY:
     case SQL_LONGVARBINARY:
         return GetBinary(cur, iCol);
 
     case SQL_DECIMAL:
     case SQL_NUMERIC:
```

### Comparing `pyodbc-4.0.8/src/params.cpp` & `pyodbc-4.0.9/src/params.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,36 @@
     }
 
     I(pch == 0 || (int)(strlen(pch) + 1) == len);
 
     return pch;
 }
 
+static bool GetUUIDInfo(Cursor* cur, Py_ssize_t index, PyObject* param, ParamInfo& info)
+{
+    info.ValueType = SQL_C_GUID;
+    info.ParameterType = SQL_GUID;
+    info.ColumnSize = 16;
+
+    info.allocated = true;
+    info.ParameterValuePtr = pyodbc_malloc(sizeof(SQLGUID));
+    if (!info.ParameterValuePtr)
+    {
+        PyErr_NoMemory();
+        return false;
+    }
+
+    // Do we need to use "bytes" on a big endian machine?
+    Object b(PyObject_GetAttrString(param, "bytes_le"));
+    if (!b)
+        return false;
+    memcpy(info.ParameterValuePtr, PyBytes_AS_STRING(b.Get()), sizeof(SQLGUID));
+    return true;
+}
+
 static bool GetDecimalInfo(Cursor* cur, Py_ssize_t index, PyObject* param, ParamInfo& info)
 {
     // The NUMERIC structure never works right with SQL Server and probably a lot of other drivers.  We'll bind as a
     // string.  Unfortunately, the Decimal class doesn't seem to have a way to force it to return a string without
     // exponents, so we'll have to build it ourselves.
 
     Object t = PyObject_CallMethod(param, "as_tuple", 0);
@@ -586,14 +608,17 @@
 
     if (PyFloat_Check(param))
         return GetFloatInfo(cur, index, param, info);
 
     if (PyDecimal_Check(param))
         return GetDecimalInfo(cur, index, param, info);
 
+    if (uuid_type && PyObject_IsInstance(param, uuid_type))
+        return GetUUIDInfo(cur, index, param, info);
+
 #if PY_VERSION_HEX >= 0x02060000
     if (PyByteArray_Check(param))
         return GetByteArrayInfo(cur, index, param, info);
 #endif
 
 #if PY_MAJOR_VERSION < 3
     if (PyInt_Check(param))
```

### Comparing `pyodbc-4.0.8/src/pyodbc.h` & `pyodbc-4.0.9/src/pyodbc.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/pyodbccompat.cpp` & `pyodbc-4.0.9/src/pyodbccompat.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/pyodbccompat.h` & `pyodbc-4.0.9/src/pyodbccompat.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/pyodbcdbg.cpp` & `pyodbc-4.0.9/src/pyodbcdbg.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/pyodbcmodule.cpp` & `pyodbc-4.0.9/src/pyodbcmodule.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 // Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 // documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 // rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 // permit persons to whom the Software is furnished to do so.
 //
 // THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 // WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
@@ -124,19 +123,30 @@
                 "Exception raised in case a method or database API was used which is not\n"
                 "supported by the database, e.g. requesting a .rollback() on a connection that\n"
                 "does not support transaction or has transactions turned off.")
 };
 
 
 PyObject* decimal_type;
+PyObject* uuid_type;
+
+bool UseNativeUUID()
+{
+    PyObject* o = PyObject_GetAttrString(pModule, "native_uuid");
+    // If this fails for some reason, we'll assume false and allow the exception to pop up later.
+    bool b = o && PyObject_IsTrue(o);
+    Py_XDECREF(o);
+    return b;
+}
 
 HENV henv = SQL_NULL_HANDLE;
 
 Py_UNICODE chDecimal = '.';
 
+
 // Initialize the global decimal character and thousands separator character, used when parsing decimal
 // objects.
 //
 static void init_locale_info()
 {
     Object module = PyImport_ImportModule("locale");
     if (!module)
@@ -178,33 +188,45 @@
     Cursor_init();
     if (!CnxnInfo_init())
         return false;
     GetData_init();
     if (!Params_init())
         return false;
 
-    PyObject* decimalmod = PyImport_ImportModule("cdecimal");
-    if (!decimalmod)
+    Object mod(PyImport_ImportModule("cdecimal"));
+    if (!mod)
     {
-        // Clear the error from the failed import of cdecimal.
         PyErr_Clear();
-        decimalmod = PyImport_ImportModule("decimal");
-        if (!decimalmod) {
+        mod.Attach(PyImport_ImportModule("decimal"));
+        if (!mod)
+        {
             PyErr_SetString(PyExc_RuntimeError, "Unable to import cdecimal or decimal");
             return false;
         }
     }
 
-    decimal_type = PyObject_GetAttrString(decimalmod, "Decimal");
-    Py_DECREF(decimalmod);
-
-    if (decimal_type == 0)
+    Object dec(PyObject_GetAttrString(mod, "Decimal"));
+    if (!dec)
+    {
         PyErr_SetString(PyExc_RuntimeError, "Unable to import decimal.Decimal.");
+        return false;
+    }
+
+    mod = PyImport_ImportModule("uuid");
+    if (!mod)
+        return false;
+
+    Object uuid(PyObject_GetAttrString(mod, "UUID"));
+    if (!uuid)
+        return false;
 
-    return decimal_type != 0;
+    decimal_type = dec.Detach();
+    uuid_type    = uuid.Detach();
+
+    return true;
 }
 
 
 static bool AllocateEnv()
 {
     PyObject* pooling = PyObject_GetAttrString(pModule, "pooling");
     bool bPooling = pooling == Py_True;
@@ -1027,14 +1049,16 @@
     PyModule_AddIntConstant(module, "threadsafety", 1);
     PyModule_AddStringConstant(module, "apilevel", "2.0");
     PyModule_AddStringConstant(module, "paramstyle", "qmark");
     PyModule_AddObject(module, "pooling", Py_True);
     Py_INCREF(Py_True);
     PyModule_AddObject(module, "lowercase", Py_False);
     Py_INCREF(Py_False);
+    PyModule_AddObject(module, "native_uuid", Py_False);
+    Py_INCREF(Py_False);
 
     PyModule_AddObject(module, "Connection", (PyObject*)&ConnectionType);
     Py_INCREF((PyObject*)&ConnectionType);
     PyModule_AddObject(module, "Cursor", (PyObject*)&CursorType);
     Py_INCREF((PyObject*)&CursorType);
     PyModule_AddObject(module, "Row", (PyObject*)&RowType);
     Py_INCREF((PyObject*)&RowType);
@@ -1152,8 +1176,7 @@
         buffer[offset++] = (Py_UNICODE)';';
     }
 
     I(offset == length);
 
     return result;
 }
-
```

### Comparing `pyodbc-4.0.8/src/pyodbcmodule.h` & `pyodbc-4.0.9/src/pyodbcmodule.h`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 extern PyObject* IntegrityError;
 extern PyObject* DataError;
 extern PyObject* NotSupportedError;
 
 extern PyObject* null_binary;
 
 extern PyObject* decimal_type;
+extern PyObject* uuid_type;
 
 inline bool PyDecimal_Check(PyObject* p)
 {
     return Py_TYPE(p) == (_typeobject*)decimal_type;
 }
 extern HENV henv;
 
@@ -49,8 +50,11 @@
 inline bool lowercase()
 {
     return PyObject_GetAttrString(pModule, "lowercase") == Py_True;
 }
 
 extern Py_UNICODE chDecimal;
 
+bool UseNativeUUID();
+// Returns True if pyodbc.native_uuid is true, meaning uuid.UUID objects should be returned.
+
 #endif // _PYPGMODULE_H
```

### Comparing `pyodbc-4.0.8/src/row.cpp` & `pyodbc-4.0.9/src/row.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/row.h` & `pyodbc-4.0.9/src/row.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/sqlwchar.h` & `pyodbc-4.0.9/src/sqlwchar.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/textenc.cpp` & `pyodbc-4.0.9/src/textenc.cpp`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/textenc.h` & `pyodbc-4.0.9/src/textenc.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/src/wrapper.h` & `pyodbc-4.0.9/src/wrapper.h`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/accesstests.py` & `pyodbc-4.0.9/tests2/accesstests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/dbapi20.py` & `pyodbc-4.0.9/tests2/dbapi20.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/dbapitests.py` & `pyodbc-4.0.9/tests2/dbapitests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/empty.accdb` & `pyodbc-4.0.9/tests2/empty.accdb`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/empty.mdb` & `pyodbc-4.0.9/tests2/empty.mdb`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/exceltests.py` & `pyodbc-4.0.9/tests2/exceltests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/freetdstests.py` & `pyodbc-4.0.9/tests2/freetdstests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/informixtests.py` & `pyodbc-4.0.9/tests2/informixtests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/mysqltests.py` & `pyodbc-4.0.9/tests2/mysqltests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/pgtests.py` & `pyodbc-4.0.9/tests2/pgtests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/sqlite.db` & `pyodbc-4.0.9/tests2/sqlite.db`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/sqlitetests.py` & `pyodbc-4.0.9/tests2/sqlitetests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/sqlservertests.py` & `pyodbc-4.0.9/tests2/sqlservertests.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 is installed:
 
   2000: DRIVER={SQL Server}
   2005: DRIVER={SQL Server}
   2008: DRIVER={SQL Server Native Client 10.0}
 """
 
-import sys, os, re
+import sys, os, re, uuid
 import unittest
 from decimal import Decimal
 from datetime import datetime, date, time
 from os.path import join, getsize, dirname, abspath
 from testutils import *
 
 _TESTSTR = '0123456789-abcdefghijklmnopqrstuvwxyz-'
@@ -158,20 +158,36 @@
         self.assert_(isinstance(value, int))
 
     def test_noscan(self):
         self.assertEqual(self.cursor.noscan, False)
         self.cursor.noscan = True
         self.assertEqual(self.cursor.noscan, True)
 
-    def test_guid(self):
-        self.cursor.execute("create table t1(g1 uniqueidentifier)")
-        self.cursor.execute("insert into t1 values (newid())")
-        v = self.cursor.execute("select * from t1").fetchone()[0]
-        self.assertEqual(type(v), unicode)
-        self.assertEqual(len(v), 36)
+    def test_nonnative_uuid(self):
+        # The default is False meaning we should return a string.  Note that
+        # SQL Server seems to always return uppercase.
+        value = uuid.uuid4()
+        self.cursor.execute("create table t1(n uniqueidentifier)")
+        self.cursor.execute("insert into t1 values (?)", value)
+
+        pyodbc.native_uuid = False
+        result = self.cursor.execute("select n from t1").fetchval()
+        self.assertEqual(type(result), unicode)
+        self.assertEqual(result, unicode(value).upper())
+
+    def test_native_uuid(self):
+        # When true, we should return a uuid.UUID object.
+        value = uuid.uuid4()
+        self.cursor.execute("create table t1(n uniqueidentifier)")
+        self.cursor.execute("insert into t1 values (?)", value)
+
+        pyodbc.native_uuid = True
+        result = self.cursor.execute("select n from t1").fetchval()
+        self.assertIsInstance(result, uuid.UUID)
+        self.assertEqual(value, result)
 
     def test_nextset(self):
         self.cursor.execute("create table t1(i int)")
         for i in range(4):
             self.cursor.execute("insert into t1(i) values(?)", i)
 
         self.cursor.execute("select i from t1 where i < 2 order by i; select i from t1 where i >= 2 order by i")
```

### Comparing `pyodbc-4.0.8/tests2/test.py` & `pyodbc-4.0.9/tests2/test.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/test.xls` & `pyodbc-4.0.9/tests2/test.xls`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/testbase.py` & `pyodbc-4.0.9/tests2/testbase.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/testutils.py` & `pyodbc-4.0.9/tests2/testutils.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests2/testutils.pyc` & `pyodbc-4.0.9/tests2/testutils.pyc`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/accesstests.py` & `pyodbc-4.0.9/tests3/accesstests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/dbapi20.py` & `pyodbc-4.0.9/tests3/dbapi20.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/dbapitests.py` & `pyodbc-4.0.9/tests3/dbapitests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/exceltests.py` & `pyodbc-4.0.9/tests3/exceltests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/informixtests.py` & `pyodbc-4.0.9/tests3/informixtests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/mysqltests.py` & `pyodbc-4.0.9/tests3/mysqltests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/pgtests.py` & `pyodbc-4.0.9/tests3/pgtests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/sqlitetests.py` & `pyodbc-4.0.9/tests3/sqlitetests.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/sqlservertests.py` & `pyodbc-4.0.9/tests3/sqlservertests.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 is installed:
 
   2000: DRIVER={SQL Server}
   2005: DRIVER={SQL Server}
   2008: DRIVER={SQL Server Native Client 10.0}
 """
 
-import sys, os, re
+import sys, os, re, uuid
 import unittest
 from decimal import Decimal
 from datetime import datetime, date, time
 from os.path import join, getsize, dirname, abspath
 from testutils import *
 
 _TESTSTR = '0123456789-abcdefghijklmnopqrstuvwxyz-'
@@ -153,20 +153,36 @@
         self.assert_(isinstance(value, int))
 
     def test_noscan(self):
         self.assertEqual(self.cursor.noscan, False)
         self.cursor.noscan = True
         self.assertEqual(self.cursor.noscan, True)
 
-    def test_guid(self):
-        self.cursor.execute("create table t1(g1 uniqueidentifier)")
-        self.cursor.execute("insert into t1 values (newid())")
-        v = self.cursor.execute("select * from t1").fetchone()[0]
-        self.assertEqual(type(v), str)
-        self.assertEqual(len(v), 36)
+    def test_nonnative_uuid(self):
+        # The default is False meaning we should return a string.  Note that
+        # SQL Server seems to always return uppercase.
+        value = uuid.uuid4()
+        self.cursor.execute("create table t1(n uniqueidentifier)")
+        self.cursor.execute("insert into t1 values (?)", value)
+
+        pyodbc.native_uuid = False
+        result = self.cursor.execute("select n from t1").fetchval()
+        self.assertEqual(type(result), str)
+        self.assertEqual(result, str(value).upper())
+
+    def test_native_uuid(self):
+        # When true, we should return a uuid.UUID object.
+        value = uuid.uuid4()
+        self.cursor.execute("create table t1(n uniqueidentifier)")
+        self.cursor.execute("insert into t1 values (?)", value)
+
+        pyodbc.native_uuid = True
+        result = self.cursor.execute("select n from t1").fetchval()
+        self.assertIsInstance(result, uuid.UUID)
+        self.assertEqual(value, result)
 
     def test_nextset(self):
         self.cursor.execute("create table t1(i int)")
         for i in range(4):
             self.cursor.execute("insert into t1(i) values(?)", i)
 
         self.cursor.execute("select i from t1 where i < 2 order by i; select i from t1 where i >= 2 order by i")
@@ -629,15 +645,14 @@
     def test_negative_float(self):
         value = -200
         self.cursor.execute("create table t1(n float)")
         self.cursor.execute("insert into t1 values (?)", value)
         result  = self.cursor.execute("select n from t1").fetchone()[0]
         self.assertEqual(value, result)
 
-
     #
     # stored procedures
     #
 
     # def test_callproc(self):
     #     "callproc with a simple input-only stored procedure"
     #     pass
```

### Comparing `pyodbc-4.0.8/tests3/testbase.py` & `pyodbc-4.0.9/tests3/testbase.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/testutils.py` & `pyodbc-4.0.9/tests3/testutils.py`

 * *Files identical despite different names*

### Comparing `pyodbc-4.0.8/tests3/testutils.pyc` & `pyodbc-4.0.9/tests3/testutils.pyc`

 * *Files identical despite different names*

