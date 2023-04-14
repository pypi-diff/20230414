# Comparing `tmp/sqlfluff-templater-dbt-2.0.3.tar.gz` & `tmp/sqlfluff-templater-dbt-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-qfd6f743/sqlfluff-templater-dbt-2.0.3.tar", last modified: Wed Apr  5 17:27:00 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-mxbzpp0x/sqlfluff-templater-dbt-2.0.4.tar", last modified: Fri Apr 14 09:56:01 2023, max compression
```

## Comparing `sqlfluff-templater-dbt-2.0.3.tar` & `sqlfluff-templater-dbt-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-05 17:26:45.000000 sqlfluff-templater-dbt-2.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-05 17:26:45.000000 sqlfluff-templater-dbt-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-05 17:26:45.000000 sqlfluff-templater-dbt-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-05 17:26:45.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-05 17:26:45.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 17:27:00.000000 sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:55:48.000000 sqlfluff-templater-dbt-2.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 09:55:48.000000 sqlfluff-templater-dbt-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 09:55:48.000000 sqlfluff-templater-dbt-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-14 09:55:48.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-14 09:55:48.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 09:56:01.000000 sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-2.0.3/LICENSE.md` & `sqlfluff-templater-dbt-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.0.3/PKG-INFO` & `sqlfluff-templater-dbt-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.0.3
+Version: 2.0.4
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-templater-dbt-2.0.3/setup.cfg` & `sqlfluff-templater-dbt-2.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 2.0.3
+version = 2.0.4
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -61,15 +61,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	sqlfluff==2.0.3
+	sqlfluff==2.0.4
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt/templater.py` & `sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt/templater.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.0.3/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff-templater-dbt-2.0.4/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.0.3
+Version: 2.0.4
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

