# Comparing `tmp/dbt-snowflake-1.5.0b4.tar.gz` & `tmp/dbt-snowflake-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.5.0b4.tar", last modified: Thu Mar 30 20:56:10 2023, max compression
+gzip compressed data, was "dbt-snowflake-1.5.0rc1.tar", last modified: Fri Apr 14 21:50:06 2023, max compression
```

## Comparing `dbt-snowflake-1.5.0b4.tar` & `dbt-snowflake-1.5.0rc1.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.673558 dbt-snowflake-1.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.665558 dbt-snowflake-1.5.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.665558 dbt-snowflake-1.5.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.665558 dbt-snowflake-1.5.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:56:10.669558 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 20:56:10.000000 dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:56:10.673558 dbt-snowflake-1.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-30 20:55:59.000000 dbt-snowflake-1.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.321372 dbt-snowflake-1.5.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.321372 dbt-snowflake-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/setup.py
```

### Comparing `dbt-snowflake-1.5.0b4/LICENSE.md` & `dbt-snowflake-1.5.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/PKG-INFO` & `dbt-snowflake-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0b4 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0rc1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.5.0b4/README.md` & `dbt-snowflake-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from dataclasses import dataclass
 from typing import Mapping, Any, Optional, List, Union, Dict
 
 import agate
 
-from dbt.adapters.base.impl import AdapterConfig
+from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport  # type: ignore
 from dbt.adapters.base.meta import available
 from dbt.adapters.sql import SQLAdapter  # type: ignore
 from dbt.adapters.sql.impl import (
     LIST_SCHEMAS_MACRO_NAME,
     LIST_RELATIONS_MACRO_NAME,
 )
+
 from dbt.adapters.snowflake import SnowflakeConnectionManager
 from dbt.adapters.snowflake import SnowflakeRelation
 from dbt.adapters.snowflake import SnowflakeColumn
 from dbt.contracts.graph.manifest import Manifest
+from dbt.contracts.graph.nodes import ConstraintType
 from dbt.exceptions import CompilationError, DbtDatabaseError, DbtRuntimeError
 from dbt.utils import filter_null_values
 
 
 @dataclass
 class SnowflakeConfig(AdapterConfig):
     transient: Optional[bool] = None
@@ -34,14 +36,22 @@
 class SnowflakeAdapter(SQLAdapter):
     Relation = SnowflakeRelation
     Column = SnowflakeColumn
     ConnectionManager = SnowflakeConnectionManager
 
     AdapterSpecificConfigs = SnowflakeConfig
 
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.not_null: ConstraintSupport.ENFORCED,
+        ConstraintType.unique: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.primary_key: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.NOT_ENFORCED,
+    }
+
     @classmethod
     def date_function(cls):
         return "CURRENT_TIMESTAMP()"
 
     @classmethod
     def _catalog_filter_table(cls, table: agate.Table, manifest: Manifest) -> agate.Table:
         # On snowflake, users can set QUOTED_IDENTIFIERS_IGNORE_CASE, so force
```

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           temporary
         {%- elif transient -%}
           transient
         {%- endif %} table {{ relation }}
         {%- set contract_config = config.get('contract') -%}
         {%- if contract_config.enforced -%}
           {{ get_assert_columns_equivalent(sql) }}
-          {{ get_columns_spec_ddl() }}
+          {{ get_table_columns_and_constraints() }}
           {% set compiled_code = get_select_subquery(compiled_code) %}
         {% endif %}
         {% if copy_grants and not temporary -%} copy grants {%- endif %} as
         (
           {%- if cluster_by_string is not none -%}
             select * from (
               {{ compiled_code }}
```

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0b4 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0rc1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.5.0b4/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 dbt/include/snowflake/macros/materializations/snapshot.sql
 dbt/include/snowflake/macros/materializations/table.sql
 dbt/include/snowflake/macros/materializations/test.sql
 dbt/include/snowflake/macros/materializations/view.sql
 dbt/include/snowflake/macros/utils/array_construct.sql
 dbt/include/snowflake/macros/utils/bool_or.sql
 dbt/include/snowflake/macros/utils/escape_single_quotes.sql
-dbt/include/snowflake/macros/utils/get_columns_spec_ddl.sql
 dbt/include/snowflake/macros/utils/right.sql
 dbt/include/snowflake/macros/utils/safe_cast.sql
 dbt/include/snowflake/macros/utils/timestamps.sql
 dbt_snowflake.egg-info/PKG-INFO
 dbt_snowflake.egg-info/SOURCES.txt
 dbt_snowflake.egg-info/dependency_links.txt
 dbt_snowflake.egg-info/not-zip-safe
```

### Comparing `dbt-snowflake-1.5.0b4/setup.py` & `dbt-snowflake-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-snowflake"
-package_version = "1.5.0b4"
+package_version = "1.5.0rc1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

