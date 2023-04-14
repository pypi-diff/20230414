# Comparing `tmp/astronomer-starship-0.3.4.tar.gz` & `tmp/astronomer-starship-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer-starship-0.3.4.tar", last modified: Wed Apr 12 15:12:20 2023, max compression
+gzip compressed data, was "astronomer-starship-0.3.5.tar", last modified: Fri Apr 14 13:38:10 2023, max compression
```

## Comparing `astronomer-starship-0.3.4.tar` & `astronomer-starship-0.3.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.185887 astronomer-starship-0.3.4/aeroscope/plugins/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/astronomer_starship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/astrohub_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.193888 astronomer-starship-0.3.4/starship/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/idiomorph.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/tippy.js
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/tail-spin.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.185887 astronomer-starship-0.3.4/starship/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.193888 astronomer-starship-0.3.4/starship/templates/starship/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/starship/templates/starship/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/dag_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/github_loop.html
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_pool_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/tabs_loading.html
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select_loading.html
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/token_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/user_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/dags.html
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/env.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/migration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/pools.html
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/variables.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/astronomer_starship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/astrohub_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/idiomorph.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/tippy.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/tail-spin.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/starship/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/templates/starship/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/starship/templates/starship/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/user_label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/dags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/env.html
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/pools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/variables.html
```

### Comparing `astronomer-starship-0.3.4/PKG-INFO` & `astronomer-starship-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astronomer-starship
-Version: 0.3.4
+Version: 0.3.5
 Summary: Migrations to Astro Cloud
 Home-page: UNKNOWN
 Author: ade@astronomer.io
 License: UNKNOWN
 Description: Astronomer Starship Plugin
         ==========================
```

### Comparing `astronomer-starship-0.3.4/README.rst` & `astronomer-starship-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/aeroscope/operators.py` & `astronomer-starship-0.3.5/aeroscope/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/aeroscope/plugins/__init__.py` & `astronomer-starship-0.3.5/aeroscope/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/main.html` & `astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/main.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/aeroscope/util.py` & `astronomer-starship-0.3.5/aeroscope/util.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/astronomer_starship.egg-info/PKG-INFO` & `astronomer-starship-0.3.5/astronomer_starship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astronomer-starship
-Version: 0.3.4
+Version: 0.3.5
 Summary: Migrations to Astro Cloud
 Home-page: UNKNOWN
 Author: ade@astronomer.io
 License: UNKNOWN
 Description: Astronomer Starship Plugin
         ==========================
```

### Comparing `astronomer-starship-0.3.4/astronomer_starship.egg-info/SOURCES.txt` & `astronomer-starship-0.3.5/astronomer_starship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/setup.cfg` & `astronomer-starship-0.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = astronomer-starship
-version = 0.3.4
+version = 0.3.5
 description = Migrations to Astro Cloud
 author = ade@astronomer.io
 long_description = file: README.rst
 
 [options]
 include_package_data = True
 python_requires = >=3.7, <4
```

### Comparing `astronomer-starship-0.3.4/starship/main.py` & `astronomer-starship-0.3.5/starship/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,14 +267,17 @@
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
     @expose("/label_test_connection/<string:deployment>/<string:conn_id>")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONNECTION)])
     def label_test_connection(self, conn_id: str, deployment: str):
+        if not os.getenv("ENABLE_CONN_TEST"):
+            return "🟡"
+
         deployment_url = self.get_deployment_url(deployment)
 
         local_connections = {
             conn.conn_id: conn for conn in self.local_client.get_connections()
         }
 
         rv = requests.post(
```

### Comparing `astronomer-starship-0.3.4/starship/services/astrohub_client.py` & `astronomer-starship-0.3.5/starship/services/astrohub_client.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/services/local_client.py` & `astronomer-starship-0.3.5/starship/services/local_client.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/static/js/htmx.min.js` & `astronomer-starship-0.3.5/starship/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/static/js/idiomorph.min.js` & `astronomer-starship-0.3.5/starship/static/js/idiomorph.min.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/static/js/popper.js` & `astronomer-starship-0.3.5/starship/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/static/js/tippy.js` & `astronomer-starship-0.3.5/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/static/tail-spin.svg` & `astronomer-starship-0.3.5/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/dag_row.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/dag_row.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/migrate_connection_button.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/tabs.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/tabs.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/tabs_loading.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/tabs_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select_loading.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/components/token_modal.html` & `astronomer-starship-0.3.5/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/connections.html` & `astronomer-starship-0.3.5/starship/templates/starship/connections.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/dags.html` & `astronomer-starship-0.3.5/starship/templates/starship/dags.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/env.html` & `astronomer-starship-0.3.5/starship/templates/starship/env.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/main.html` & `astronomer-starship-0.3.5/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/migration.html` & `astronomer-starship-0.3.5/starship/templates/starship/migration.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/pools.html` & `astronomer-starship-0.3.5/starship/templates/starship/pools.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.4/starship/templates/starship/variables.html` & `astronomer-starship-0.3.5/starship/templates/starship/variables.html`

 * *Files identical despite different names*

