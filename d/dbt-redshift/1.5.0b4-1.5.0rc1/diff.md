# Comparing `tmp/dbt-redshift-1.5.0b4.tar.gz` & `tmp/dbt-redshift-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.5.0b4.tar", last modified: Thu Mar 30 19:33:17 2023, max compression
+gzip compressed data, was "dbt-redshift-1.5.0rc1.tar", last modified: Fri Apr 14 21:19:22 2023, max compression
```

## Comparing `dbt-redshift-1.5.0b4.tar` & `dbt-redshift-1.5.0rc1.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.793351 dbt-redshift-1.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-30 19:33:17.793351 dbt-redshift-1.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.785350 dbt-redshift-1.5.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.785350 dbt-redshift-1.5.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.789350 dbt-redshift-1.5.0b4/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.785350 dbt-redshift-1.5.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.789350 dbt-redshift-1.5.0b4/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.789350 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.789350 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.789350 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.793351 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:33:17.793351 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 19:33:17.000000 dbt-redshift-1.5.0b4/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 19:33:17.793351 dbt-redshift-1.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-30 19:33:01.000000 dbt-redshift-1.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.484236 dbt-redshift-1.5.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.484236 dbt-redshift-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/setup.py
```

### Comparing `dbt-redshift-1.5.0b4/LICENSE.md` & `dbt-redshift-1.5.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/PKG-INFO` & `dbt-redshift-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0b4 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.5.0b4/README.md` & `dbt-redshift-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,26 +174,32 @@
         sql = f"select pg_terminate_backend({pid})"
         _, cursor = self.add_query(sql)
         res = cursor.fetchone()
         logger.debug(f"Cancel query '{connection.name}': {res}")
 
     @classmethod
     def get_response(cls, cursor: redshift_connector.Cursor) -> AdapterResponse:
+        # redshift_connector.Cursor doesn't have a status message attribute but
+        # this function is only used for successful run, so we can just return a dummy
         rows = cursor.rowcount
-        message = f"cursor.rowcount = {rows}"
+        message = "SUCCESS"
         return AdapterResponse(_message=message, rows_affected=rows)
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
         except redshift_connector.DatabaseError as e:
-            logger.debug(f"Redshift error: {str(e)}")
+            try:
+                err_msg = e.args[0]["M"]  # this is a type redshift sets, so we must use these keys
+            except Exception:
+                err_msg = str(e).strip()
+            logger.debug(f"Redshift error: {err_msg}")
             self.rollback_if_open()
-            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
+            raise dbt.exceptions.DbtDatabaseError(err_msg) from e
 
         except Exception as e:
             logger.debug("Error running SQL: {}", sql)
             logger.debug("Rolling back transaction.")
             self.rollback_if_open()
             # Raise DBT native exceptions as is.
             if isinstance(e, dbt.exceptions.DbtRuntimeError):
```

### Comparing `dbt-redshift-1.5.0b4/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/impl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from dataclasses import dataclass
 from typing import Optional, Set, Any, Dict, Type
 from collections import namedtuple
 
 from dbt.adapters.base import PythonJobHelper
-from dbt.adapters.base.impl import AdapterConfig
+from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.base.meta import available
 from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.graph.nodes import ConstraintType
 from dbt.events import AdapterLogger
+
 import dbt.exceptions
 
 from dbt.adapters.redshift import RedshiftConnectionManager, RedshiftRelation, RedshiftColumn
 
-
 logger = AdapterLogger("Redshift")
 
 
 GET_RELATIONS_MACRO_NAME = "redshift__get_relations"
 
 
 @dataclass
@@ -32,14 +33,22 @@
     Relation = RedshiftRelation
     ConnectionManager = RedshiftConnectionManager
     connections: RedshiftConnectionManager
     Column = RedshiftColumn  # type: ignore
 
     AdapterSpecificConfigs = RedshiftConfig  # type: ignore
 
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
         return "getdate()"
 
     def drop_relation(self, relation):
         """
         In Redshift, DROP TABLE ... CASCADE should not be used
```

### Comparing `dbt-redshift-1.5.0b4/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   {{ sql_header if sql_header is not none }}
 
   {%- set contract_config = config.get('contract') -%}
   {%- if contract_config.enforced -%}
 
   create {% if temporary -%}temporary{%- endif %} table
     {{ relation.include(database=(not temporary), schema=(not temporary)) }}
-    {{ get_columns_spec_ddl() }}
+    {{ get_table_columns_and_constraints() }}
     {{ get_assert_columns_equivalent(sql) }}
     {%- set sql = get_select_subquery(sql) %}
     {% if backup == false -%}backup no{%- endif %}
     {{ dist(_dist) }}
     {{ sort(_sort_type, _sort) }}
   ;
```

### Comparing `dbt-redshift-1.5.0b4/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.5.0rc1/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0b4/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0b4 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.5.0b4/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 dbt/include/redshift/macros/materializations/snapshot_merge.sql
 dbt/include/redshift/macros/utils/array_append.sql
 dbt/include/redshift/macros/utils/array_concat.sql
 dbt/include/redshift/macros/utils/array_construct.sql
 dbt/include/redshift/macros/utils/cast_bool_to_text.sql
 dbt/include/redshift/macros/utils/dateadd.sql
 dbt/include/redshift/macros/utils/datediff.sql
-dbt/include/redshift/macros/utils/get_columns_spec_ddl.sql
 dbt/include/redshift/macros/utils/last_day.sql
 dbt/include/redshift/macros/utils/length.sql
 dbt/include/redshift/macros/utils/listagg.sql
 dbt/include/redshift/macros/utils/split_part.sql
 dbt_redshift.egg-info/PKG-INFO
 dbt_redshift.egg-info/SOURCES.txt
 dbt_redshift.egg-info/dependency_links.txt
```

### Comparing `dbt-redshift-1.5.0b4/setup.py` & `dbt-redshift-1.5.0rc1/setup.py`

 * *Files identical despite different names*

