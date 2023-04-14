# Comparing `tmp/dbt-postgres-1.5.0b5.tar.gz` & `tmp/dbt-postgres-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-postgres-1.5.0b5.tar", last modified: Thu Mar 30 16:56:48 2023, max compression
+gzip compressed data, was "dbt-postgres-1.5.0rc1.tar", last modified: Fri Apr 14 00:23:12 2023, max compression
```

## Comparing `dbt-postgres-1.5.0b5.tar` & `dbt-postgres-1.5.0rc1.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/adapters/postgres/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/include/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.833909 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/dbt/include/postgres/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 16:56:48.000000 dbt-postgres-1.5.0b5/dbt_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:56:48.837909 dbt-postgres-1.5.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-30 16:56:37.000000 dbt-postgres-1.5.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/adapters/postgres/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/include/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.463280 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/dbt/include/postgres/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 00:23:12.000000 dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:23:12.467280 dbt-postgres-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-14 00:23:01.000000 dbt-postgres-1.5.0rc1/setup.py
```

### Comparing `dbt-postgres-1.5.0b5/PKG-INFO` & `dbt-postgres-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.5.0b5
+Version: 1.5.0rc1
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.5.0b5 Summary: The postgres
-adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
-labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.5.0rc1 Summary: The
+postgres adapter plugin for dbt (data build tool) Home-page: https://
+github.com/dbt-labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
+:: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-postgres The `dbt-postgres` package contains all of
```

### Comparing `dbt-postgres-1.5.0b5/README.md` & `dbt-postgres-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/adapters/postgres/__init__.py` & `dbt-postgres-1.5.0rc1/dbt/adapters/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/adapters/postgres/connections.py` & `dbt-postgres-1.5.0rc1/dbt/adapters/postgres/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/adapters/postgres/impl.py` & `dbt-postgres-1.5.0rc1/dbt/adapters/postgres/impl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 from dataclasses import dataclass
 from typing import Optional, Set, List, Any
 from dbt.adapters.base.meta import available
-from dbt.adapters.base.impl import AdapterConfig
+from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.postgres import PostgresConnectionManager
 from dbt.adapters.postgres.column import PostgresColumn
 from dbt.adapters.postgres import PostgresRelation
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
+from dbt.contracts.graph.nodes import ConstraintType
 from dbt.exceptions import (
     CrossDbReferenceProhibitedError,
     IndexConfigNotDictError,
     IndexConfigError,
     DbtRuntimeError,
     UnexpectedDbReferenceError,
 )
@@ -60,14 +61,22 @@
 class PostgresAdapter(SQLAdapter):
     Relation = PostgresRelation
     ConnectionManager = PostgresConnectionManager
     Column = PostgresColumn
 
     AdapterSpecificConfigs = PostgresConfig
 
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.ENFORCED,
+        ConstraintType.not_null: ConstraintSupport.ENFORCED,
+        ConstraintType.unique: ConstraintSupport.ENFORCED,
+        ConstraintType.primary_key: ConstraintSupport.ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
+    }
+
     @classmethod
     def date_function(cls):
         return "now()"
 
     @available
     def verify_database(self, database):
         if database.startswith('"'):
```

### Comparing `dbt-postgres-1.5.0b5/dbt/adapters/postgres/relation.py` & `dbt-postgres-1.5.0rc1/dbt/adapters/postgres/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/adapters.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     temporary
   {%- elif unlogged -%}
     unlogged
   {%- endif %} table {{ relation }}
   {% set contract_config = config.get('contract') %}
   {% if contract_config.enforced %}
     {{ get_assert_columns_equivalent(sql) }}
-    {{ get_columns_spec_ddl() }} ;
+    {{ get_table_columns_and_constraints() }} ;
     insert into {{ relation }} {{ get_column_names() }}
     {%- set sql = get_select_subquery(sql) %}
   {% else %}
     as
   {% endif %}
   (
     {{ sql }}
```

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/catalog.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/relations.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/timestamps.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/datediff.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt/include/postgres/macros/utils/listagg.sql` & `dbt-postgres-1.5.0rc1/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.5.0b5/dbt_postgres.egg-info/PKG-INFO` & `dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.5.0b5
+Version: 1.5.0rc1
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.5.0b5 Summary: The postgres
-adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
-labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.5.0rc1 Summary: The
+postgres adapter plugin for dbt (data build tool) Home-page: https://
+github.com/dbt-labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
+:: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-postgres The `dbt-postgres` package contains all of
```

### Comparing `dbt-postgres-1.5.0b5/dbt_postgres.egg-info/SOURCES.txt` & `dbt-postgres-1.5.0rc1/dbt_postgres.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 dbt/include/postgres/sample_profiles.yml
 dbt/include/postgres/macros/adapters.sql
 dbt/include/postgres/macros/catalog.sql
 dbt/include/postgres/macros/relations.sql
 dbt/include/postgres/macros/timestamps.sql
 dbt/include/postgres/macros/materializations/incremental_strategies.sql
 dbt/include/postgres/macros/materializations/snapshot_merge.sql
+dbt/include/postgres/macros/materializations/materialized_view/create.sql
+dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
 dbt/include/postgres/macros/utils/any_value.sql
 dbt/include/postgres/macros/utils/columns_spec_ddl.sql
 dbt/include/postgres/macros/utils/dateadd.sql
 dbt/include/postgres/macros/utils/datediff.sql
 dbt/include/postgres/macros/utils/last_day.sql
 dbt/include/postgres/macros/utils/listagg.sql
 dbt/include/postgres/macros/utils/split_part.sql
```

### Comparing `dbt-postgres-1.5.0b5/setup.py` & `dbt-postgres-1.5.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # default to psycopg2-binary for all OSes/versions
     print(PSYCOPG2_MESSAGE)
     return "psycopg2-binary"
 
 
 package_name = "dbt-postgres"
-package_version = "1.5.0b5"
+package_version = "1.5.0rc1"
 description = """The postgres adapter plugin for dbt (data build tool)"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 DBT_PSYCOPG2_NAME = _dbt_psycopg2_name()
```

