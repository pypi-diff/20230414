# Comparing `tmp/diengine-connect-0.0.1.tar.gz` & `tmp/diengine-connect-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diengine-connect-0.0.1.tar", last modified: Fri Apr 14 12:36:25 2023, max compression
+gzip compressed data, was "diengine-connect-0.1.7.tar", last modified: Thu Apr 13 02:38:50 2023, max compression
```

## Comparing `diengine-connect-0.0.1.tar` & `diengine-connect-0.1.7.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.324076 diengine-connect-0.0.1/
--rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/LICENSE
--rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-14 12:36:25.323909 diengine-connect-0.0.1/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)      315 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/README.md
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.311950 diengine-connect-0.0.1/diengine_connect/
--rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-04-14 12:36:19.000000 diengine-connect-0.0.1/diengine_connect/VERSION
--rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.313227 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/
--rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.315539 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4792 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)    13591 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.317139 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1599 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7513 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3512 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.317564 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-04-14 11:40:07.000000 diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/sql/preparer.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.317911 diengine-connect-0.0.1/diengine_connect/cc_superset/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/cc_superset/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1228 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/cc_superset/datatypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8404 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/cc_superset/engine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1989 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/common.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.319527 diengine-connect-0.0.1/diengine_connect/datatypes/
--rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)    14636 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/base.py
--rw-r--r--   0 xushihao   (501) staff       (20)     9238 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/container.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2558 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/format.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4649 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/network.py
--rw-r--r--   0 xushihao   (501) staff       (20)    11148 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/numeric.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2352 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/registry.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3725 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/special.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5932 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/string.py
--rw-r--r--   0 xushihao   (501) staff       (20)     8402 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/datatypes/temporal.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.320025 diengine-connect-0.0.1/diengine_connect/dbapi/
--rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/dbapi/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/dbapi/connection.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/dbapi/cursor.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.323524 diengine-connect-0.0.1/diengine_connect/driver/
--rw-r--r--   0 xushihao   (501) staff       (20)     6674 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/buffer.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6057 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/common.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/compression.py
--rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/constants.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/context.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1316 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/ctypes.py
--rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/dataconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)      823 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/ddl.py
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/diengine.py
--rw-r--r--   0 xushihao   (501) staff       (20)     2842 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/exceptions.py
--rw-r--r--   0 xushihao   (501) staff       (20)     7194 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/extras.py
--rw-r--r--   0 xushihao   (501) staff       (20)    18878 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/httpclient.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6476 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/httputil.py
--rw-r--r--   0 xushihao   (501) staff       (20)     6980 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/insert.py
--rw-r--r--   0 xushihao   (501) staff       (20)      732 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/models.py
--rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/npconv.py
--rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/npquery.py
--rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/options.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5718 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/parser.py
--rw-r--r--   0 xushihao   (501) staff       (20)    19957 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/query.py
--rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/tools.py
--rw-r--r--   0 xushihao   (501) staff       (20)     5385 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/transform.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-04-14 10:13:07.000000 diengine-connect-0.0.1/diengine_connect/driver/types.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.323678 diengine-connect-0.0.1/diengine_connect/driverc/
--rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/driverc/__init__.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/entry_points.py
--rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/diengine_connect/json_impl.py
-drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-14 12:36:25.312793 diengine-connect-0.0.1/diengine_connect.egg-info/
--rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/PKG-INFO
--rw-r--r--   0 xushihao   (501) staff       (20)     2520 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/SOURCES.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/dependency_links.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/entry_points.txt
--rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/not-zip-safe
--rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/requires.txt
--rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-04-14 12:36:25.000000 diengine-connect-0.0.1/diengine_connect.egg-info/top_level.txt
--rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/pyproject.toml
--rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-04-14 12:36:25.324127 diengine-connect-0.0.1/setup.cfg
--rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-04-14 09:22:42.000000 diengine-connect-0.0.1/setup.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212683 diengine-connect-0.1.7/
+-rw-r--r--   0 xushihao   (501) staff       (20)    11389 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/LICENSE
+-rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-13 02:38:50.212551 diengine-connect-0.1.7/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)      315 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/README.md
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.204287 diengine-connect-0.1.7/diengine_connect/
+-rw-r--r--   0 xushihao   (501) staff       (20)        5 2023-04-13 02:38:28.000000 diengine-connect-0.1.7/diengine_connect/VERSION
+-rw-r--r--   0 xushihao   (501) staff       (20)      261 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.205608 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/
+-rw-r--r--   0 xushihao   (501) staff       (20)      200 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206116 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)       57 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4792 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    13591 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206484 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1599 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7513 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3512 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2435 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.206860 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 xushihao   (501) staff       (20)      458 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      884 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      281 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/preparer.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.207197 diengine-connect-0.1.7/diengine_connect/cc_superset/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1228 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/datatypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8404 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/cc_superset/engine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1989 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/common.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.208631 diengine-connect-0.1.7/diengine_connect/datatypes/
+-rw-r--r--   0 xushihao   (501) staff       (20)      297 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    14636 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/base.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     9238 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/container.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2558 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/format.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4649 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/network.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    11148 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/numeric.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2352 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/registry.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3725 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/special.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5932 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/string.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     8402 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/datatypes/temporal.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.209002 diengine-connect-0.1.7/diengine_connect/dbapi/
+-rw-r--r--   0 xushihao   (501) staff       (20)      880 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1525 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/connection.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4462 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/dbapi/cursor.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212275 diengine-connect-0.1.7/diengine_connect/driver/
+-rw-r--r--   0 xushihao   (501) staff       (20)     6674 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4379 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/buffer.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    34700 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/client.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6057 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/common.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1756 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/compression.py
+-rw-r--r--   0 xushihao   (501) staff       (20)       80 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/constants.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2410 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/context.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1316 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/ctypes.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     3466 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/dataconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      823 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/ddl.py
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/diengine.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     2842 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/exceptions.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     7194 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/extras.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    18878 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/httpclient.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6476 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/httputil.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     6980 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/insert.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      732 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/models.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      312 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/npconv.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     4232 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/npquery.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      682 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/options.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5718 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/parser.py
+-rw-r--r--   0 xushihao   (501) staff       (20)    19957 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/query.py
+-rw-r--r--   0 xushihao   (501) staff       (20)      799 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/tools.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     5385 2023-04-13 02:27:50.000000 diengine-connect-0.1.7/diengine_connect/driver/transform.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1011 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driver/types.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.212399 diengine-connect-0.1.7/diengine_connect/driverc/
+-rw-r--r--   0 xushihao   (501) staff       (20)        0 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/driverc/__init__.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1294 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/entry_points.py
+-rw-r--r--   0 xushihao   (501) staff       (20)     1306 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/diengine_connect/json_impl.py
+drwxr-xr-x   0 xushihao   (501) staff       (20)        0 2023-04-13 02:38:50.205120 diengine-connect-0.1.7/diengine_connect.egg-info/
+-rw-r--r--   0 xushihao   (501) staff       (20)     1336 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/PKG-INFO
+-rw-r--r--   0 xushihao   (501) staff       (20)     2554 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      263 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/entry_points.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)        1 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/not-zip-safe
+-rw-r--r--   0 xushihao   (501) staff       (20)      179 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/requires.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)       17 2023-04-13 02:38:50.000000 diengine-connect-0.1.7/diengine_connect.egg-info/top_level.txt
+-rw-r--r--   0 xushihao   (501) staff       (20)      192 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/pyproject.toml
+-rw-r--r--   0 xushihao   (501) staff       (20)       38 2023-04-13 02:38:50.212731 diengine-connect-0.1.7/setup.cfg
+-rw-r--r--   0 xushihao   (501) staff       (20)     3152 2023-04-13 02:23:12.000000 diengine-connect-0.1.7/setup.py
```

### Comparing `diengine-connect-0.0.1/LICENSE` & `diengine-connect-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/PKG-INFO` & `diengine-connect-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.0.1
+Version: 0.1.7
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
         A suite of Python packages for connecting Python to ClickHouse:
```

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/base.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/custom.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/ddl/tableengine.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/dialect.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/inspector.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `diengine-connect-0.1.7/diengine_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_superset/datatypes.py` & `diengine-connect-0.1.7/diengine_connect/cc_superset/datatypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/cc_superset/engine.py` & `diengine-connect-0.1.7/diengine_connect/cc_superset/engine.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/common.py` & `diengine-connect-0.1.7/diengine_connect/common.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/base.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/container.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/format.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/network.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/numeric.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/registry.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/special.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/string.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/datatypes/temporal.py` & `diengine-connect-0.1.7/diengine_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/dbapi/__init__.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/dbapi/connection.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/dbapi/cursor.py` & `diengine-connect-0.1.7/diengine_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/__init__.py` & `diengine-connect-0.1.7/diengine_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/buffer.py` & `diengine-connect-0.1.7/diengine_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/common.py` & `diengine-connect-0.1.7/diengine_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/compression.py` & `diengine-connect-0.1.7/diengine_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/context.py` & `diengine-connect-0.1.7/diengine_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/ctypes.py` & `diengine-connect-0.1.7/diengine_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/dataconv.py` & `diengine-connect-0.1.7/diengine_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/ddl.py` & `diengine-connect-0.1.7/diengine_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/exceptions.py` & `diengine-connect-0.1.7/diengine_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/extras.py` & `diengine-connect-0.1.7/diengine_connect/driver/extras.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/httpclient.py` & `diengine-connect-0.1.7/diengine_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/httputil.py` & `diengine-connect-0.1.7/diengine_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/insert.py` & `diengine-connect-0.1.7/diengine_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/models.py` & `diengine-connect-0.1.7/diengine_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/npquery.py` & `diengine-connect-0.1.7/diengine_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/options.py` & `diengine-connect-0.1.7/diengine_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/parser.py` & `diengine-connect-0.1.7/diengine_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/query.py` & `diengine-connect-0.1.7/diengine_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/tools.py` & `diengine-connect-0.1.7/diengine_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/transform.py` & `diengine-connect-0.1.7/diengine_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/driver/types.py` & `diengine-connect-0.1.7/diengine_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/entry_points.py` & `diengine-connect-0.1.7/diengine_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect/json_impl.py` & `diengine-connect-0.1.7/diengine_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `diengine-connect-0.0.1/diengine_connect.egg-info/PKG-INFO` & `diengine-connect-0.1.7/diengine_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diengine-connect
-Version: 0.0.1
+Version: 0.1.7
 Summary: Diengine core driver, SqlAlchemy, and Superset libraries
 Home-page: UNKNOWN
 Author: diengine Inc.
 License: Apache License 2.0
 Description: ## Diengine Connect
         
         A suite of Python packages for connecting Python to ClickHouse:
```

### Comparing `diengine-connect-0.0.1/diengine_connect.egg-info/SOURCES.txt` & `diengine-connect-0.1.7/diengine_connect.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 diengine_connect/datatypes/string.py
 diengine_connect/datatypes/temporal.py
 diengine_connect/dbapi/__init__.py
 diengine_connect/dbapi/connection.py
 diengine_connect/dbapi/cursor.py
 diengine_connect/driver/__init__.py
 diengine_connect/driver/buffer.py
+diengine_connect/driver/client.py
 diengine_connect/driver/common.py
 diengine_connect/driver/compression.py
 diengine_connect/driver/constants.py
 diengine_connect/driver/context.py
 diengine_connect/driver/ctypes.py
 diengine_connect/driver/dataconv.py
 diengine_connect/driver/ddl.py
```

### Comparing `diengine-connect-0.0.1/setup.py` & `diengine-connect-0.1.7/setup.py`

 * *Files identical despite different names*

