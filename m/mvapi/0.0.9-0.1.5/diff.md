# Comparing `tmp/mvapi-0.0.9.tar.gz` & `tmp/mvapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mvapi-0.0.9.tar", last modified: Tue Aug 16 17:36:22 2022, max compression
+gzip compressed data, was "mvapi-0.1.5.tar", last modified: Fri Apr 14 19:42:43 2023, max compression
```

## Comparing `mvapi-0.0.9.tar` & `mvapi-0.1.5.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:22.000000 mvapi-0.0.9/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      275 2022-08-16 17:36:22.000000 mvapi-0.0.9/PKG-INFO
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        8 2020-08-25 10:59:54.000000 mvapi-0.0.9/README.md
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/settings/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      807 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/settings/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     2387 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/settings/default_settings.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)       18 2022-08-16 17:33:13.000000 mvapi-0.0.9/mvapi/version.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/web/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        0 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/web/models/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1460 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/models/user.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      437 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/models/session.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        0 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/models/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/web/libs/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1885 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/jsonwebtoken.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     2953 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/misc.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     6700 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/appfactory.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        0 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      138 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/logger.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)       44 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/extensions.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      542 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/exceptions.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      882 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/libs/decorators.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/web/serializers/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      588 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/serializers/user.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      687 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/serializers/session.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      886 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/serializers/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     3494 2022-08-15 22:08:10.000000 mvapi-0.0.9/mvapi/web/serializers/items.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     4484 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/serializers/base.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      686 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/urls.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:22.000000 mvapi-0.0.9/mvapi/web/views/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1401 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/views/sessions.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      731 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/views/users.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      838 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/views/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     5453 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/web/views/api.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)    12618 2022-08-16 16:19:00.000000 mvapi-0.0.9/mvapi/web/views/base.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)       56 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/models/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     7370 2022-08-16 16:01:55.000000 mvapi-0.0.9/mvapi/models/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        0 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/project/
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/project/web/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      345 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/web/run.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      128 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/web/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      452 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/project/user/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      694 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/user/create_user.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      211 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/user/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      725 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/user/update_user.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      324 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/run_temp_script.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/project/migration/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      338 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      789 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/upgrade.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      415 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/utils.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1649 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/revision.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      860 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/downgrade.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      495 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/project/migration/init.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/cli/mvapi/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      112 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/mvapi/init_project.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      187 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/cli/mvapi/__init__.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/libs/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1144 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/misc.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      856 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/run.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     2069 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/error.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      538 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/database.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        0 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/__init__.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      227 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/logger.py
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      240 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/libs/exceptions.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi/templates/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     5727 2022-08-14 17:55:44.000000 mvapi-0.0.9/mvapi/templates/error.tmpl
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1068 2022-08-14 17:55:44.000000 mvapi-0.0.9/setup.py
-drwxr-xr-x   0 mvetoshkin   (501) staff       (20)        0 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      275 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/PKG-INFO
--rw-r--r--   0 mvetoshkin   (501) staff       (20)     1678 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/SOURCES.txt
--rw-r--r--   0 mvetoshkin   (501) staff       (20)       38 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/entry_points.txt
--rw-r--r--   0 mvetoshkin   (501) staff       (20)      249 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/requires.txt
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        6 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/top_level.txt
--rw-r--r--   0 mvetoshkin   (501) staff       (20)        1 2022-08-16 17:36:21.000000 mvapi-0.0.9/mvapi.egg-info/dependency_links.txt
--rw-r--r--   0 mvetoshkin   (501) staff       (20)       38 2022-08-16 17:36:22.000000 mvapi-0.0.9/setup.cfg
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.796499 mvapi-0.1.5/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)    35149 2022-08-14 17:55:44.000000 mvapi-0.1.5/COPYING
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      305 2023-04-14 19:42:43.796499 mvapi-0.1.5/PKG-INFO
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        8 2020-08-25 10:59:54.000000 mvapi-0.1.5/README.md
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.776494 mvapi-0.1.5/mvapi/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)       56 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/__init__.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        0 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/__init__.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/mvapi/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      187 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/mvapi/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      112 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/mvapi/init_project.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/project/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      452 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/__init__.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/project/migration/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      338 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      860 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/downgrade.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      495 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/init.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1649 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/revision.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      789 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/upgrade.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      415 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/migration/utils.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      324 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/run_temp_script.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/project/user/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      211 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/user/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      694 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/user/create_user.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      725 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/user/update_user.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi/cli/project/web/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      128 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/web/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      345 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/cli/project/web/run.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.784496 mvapi-0.1.5/mvapi/libs/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        0 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/libs/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1565 2023-02-22 17:59:05.000000 mvapi-0.1.5/mvapi/libs/database.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     2069 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/libs/error.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      240 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/libs/exceptions.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      227 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/libs/logger.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1144 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/libs/misc.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1082 2023-01-30 21:53:23.000000 mvapi-0.1.5/mvapi/libs/run.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.784496 mvapi-0.1.5/mvapi/models/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     7370 2022-08-16 16:01:55.000000 mvapi-0.1.5/mvapi/models/__init__.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.788497 mvapi-0.1.5/mvapi/settings/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      807 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/settings/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     2591 2022-09-13 21:38:06.000000 mvapi-0.1.5/mvapi/settings/default_settings.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.788497 mvapi-0.1.5/mvapi/templates/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     5727 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/templates/error.tmpl
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)       18 2023-04-10 21:12:40.000000 mvapi-0.1.5/mvapi/version.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.788497 mvapi-0.1.5/mvapi/web/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        0 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/__init__.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.792498 mvapi-0.1.5/mvapi/web/libs/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        0 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     5774 2023-04-10 21:12:24.000000 mvapi-0.1.5/mvapi/web/libs/appfactory.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      882 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/decorators.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      542 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/exceptions.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)       44 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/extensions.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1885 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/jsonwebtoken.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      138 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/logger.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     2953 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/libs/misc.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.792498 mvapi-0.1.5/mvapi/web/models/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        0 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/models/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      437 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/models/session.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1460 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/models/user.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.792498 mvapi-0.1.5/mvapi/web/serializers/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      886 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/serializers/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     4484 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/serializers/base.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     3494 2022-08-15 22:08:10.000000 mvapi-0.1.5/mvapi/web/serializers/items.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      687 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/serializers/session.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      588 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/serializers/user.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      686 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/urls.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.796499 mvapi-0.1.5/mvapi/web/views/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      838 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/views/__init__.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     5453 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/views/api.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)    12618 2022-08-16 16:19:00.000000 mvapi-0.1.5/mvapi/web/views/base.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1401 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/views/sessions.py
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      731 2022-08-14 17:55:44.000000 mvapi-0.1.5/mvapi/web/views/users.py
+drwxr-xr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-04-14 19:42:43.780495 mvapi-0.1.5/mvapi.egg-info/
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      305 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1686 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        1 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)       38 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)      262 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/requires.txt
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)        6 2023-04-14 19:42:43.000000 mvapi-0.1.5/mvapi.egg-info/top_level.txt
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)       38 2023-04-14 19:42:43.796499 mvapi-0.1.5/setup.cfg
+-rw-r--r--   0 mikhail   (1000) mikhail   (1000)     1147 2022-09-05 16:47:49.000000 mvapi-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mvapi-0.0.9/mvapi/settings/__init__.py` & `mvapi-0.1.5/mvapi/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/settings/default_settings.py` & `mvapi-0.1.5/mvapi/settings/default_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,70 +21,78 @@
     SYSLOG = False
     TEMPLATE_LOADERS = {}
     VIEWS = []
 
     # noinspection PyPep8Naming
     @property
     def LOGGING(self):
-        config = {
-            'version': 1,
-            'disable_existing_loggers': False,
-            'formatters': {
-                'standard': {
-                    'format': '%(asctime)s %(name)s %(levelname)s: %(message)s'
-                }
-            },
-            'handlers': {
-                'console': {
-                    'formatter': 'standard',
-                    'class': 'logging.StreamHandler'
-                }
-            },
-            'loggers': {
-                '': {
-                    'handlers': ['console'],
-                    'level': 'DEBUG' if self.DEBUG else 'INFO'
-                }
-            }
-        }
-
         if self.SYSLOG:
             if self.SYSLOG is not True:
                 syslog_addr = self.SYSLOG
             else:
                 if sys.platform == 'darwin':
                     syslog_addr = '/var/run/syslog'
                 elif sys.platform == 'linux':
                     syslog_addr = '/dev/log'
                 else:
                     syslog_addr = ('localhost', 514)
 
-            config['formatters']['syslog'] = {
-                'format': '%(name)s: %(message)s'
+            formatters = {
+                'syslog': {
+                    'format': '%(name)s: %(message)s'
+                }
+            }
+
+            handlers = {
+                'syslog': {
+                    'formatter': 'syslog',
+                    'class': 'logging.handlers.SysLogHandler',
+                    'address': syslog_addr
+                }
             }
 
-            config['handlers']['syslog'] = {
-                'formatter': 'syslog',
-                'class': 'logging.handlers.SysLogHandler',
-                'level': 'INFO',
-                'address': syslog_addr
+            root_logger_handlers = ['syslog']
+
+        else:
+            formatters = {
+                'standard': {
+                    'format': '%(asctime)s %(name)s %(levelname)s: %(message)s'
+                }
             }
 
-            root_logger = config['loggers']['']
-            root_logger['handlers'].append('syslog')
+            handlers = {
+                'console': {
+                    'formatter': 'standard',
+                    'class': 'logging.StreamHandler'
+                }
+            }
+
+            root_logger_handlers = ['console']
 
-        return config
+        return {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'formatters': formatters,
+            'handlers': handlers,
+            'loggers': {
+                self.ROOT_LOGGER_NAME: {
+                    'handlers': root_logger_handlers,
+                    'level': 'DEBUG' if self.DEBUG else 'INFO',
+                    'propagate': False
+                }
+            }
+        }
 
     # noinspection PyPep8Naming
     @property
     def SQLALCHEMY_DATABASE_URI(self):
         return self.DB_URI
 
     # noinspection PyPep8Naming
     @property
     def ROOT_LOGGER_NAME(self):
         return self.APP_NAME
 
-    def __getattr__(self, item):
-        if item in os.environ:
-            return os.environ[item]
-        raise KeyError
+    def __getattribute__(self, name):
+        if name in os.environ:
+            return os.environ[name]
+        return super(DefaultSettings, self).__getattribute__(name)
```

### Comparing `mvapi-0.0.9/mvapi/web/models/user.py` & `mvapi-0.1.5/mvapi/web/models/user.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/libs/jsonwebtoken.py` & `mvapi-0.1.5/mvapi/web/libs/jsonwebtoken.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/libs/misc.py` & `mvapi-0.1.5/mvapi/web/libs/misc.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/libs/appfactory.py` & `mvapi-0.1.5/mvapi/web/libs/appfactory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import importlib
 import json
 import time
 
 from flask import Flask, g, request
-from sqlalchemy import event
-from sqlalchemy.engine.base import Engine
 from werkzeug.exceptions import HTTPException
 
 from mvapi.libs.database import db
 from mvapi.libs.error import save_error
 from mvapi.libs.exceptions import ModelKeyError, NotFoundError
 from mvapi.libs.misc import import_object
 from mvapi.settings import settings
@@ -179,32 +177,16 @@
 
         try:
             token_type, access_token = header.split(' ')
         except ValueError:
             raise BadRequestError('Wrong authorization header')
 
         if token_type.lower() != 'bearer':
-            raise BadRequestError('Wrong authorization token type')
+            return None
 
         try:
             jwt = JSONWebToken()
             g.current_user = jwt.get_user(access_token)
         except (NotFoundError, JWTError):
             return None
 
-    if settings.DEBUG_SQL:
-        # noinspection PyUnusedLocal
-        @event.listens_for(Engine, 'before_cursor_execute')
-        def before_cursor_execute(conn, cursor, statement, parameters, context,
-                                  executemany):
-            conn.info.setdefault('query_start_time', []).append(time.time())
-            logger.debug(f'Start Query: {statement}. '
-                         f'With parameters: {parameters}')
-
-        # noinspection PyUnusedLocal
-        @event.listens_for(Engine, 'after_cursor_execute')
-        def after_cursor_execute(conn, cursor, statement, parameters, context,
-                                 executemany):
-            total = time.time() - conn.info['query_start_time'].pop(-1)
-            logger.debug(f'Query Complete. Total Time: {str(total)}\n')
-
     return app
```

### Comparing `mvapi-0.0.9/mvapi/web/libs/exceptions.py` & `mvapi-0.1.5/mvapi/web/libs/exceptions.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/libs/decorators.py` & `mvapi-0.1.5/mvapi/web/libs/decorators.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/serializers/user.py` & `mvapi-0.1.5/mvapi/web/serializers/user.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/serializers/session.py` & `mvapi-0.1.5/mvapi/web/serializers/session.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/serializers/__init__.py` & `mvapi-0.1.5/mvapi/web/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/serializers/items.py` & `mvapi-0.1.5/mvapi/web/serializers/items.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/serializers/base.py` & `mvapi-0.1.5/mvapi/web/serializers/base.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/urls.py` & `mvapi-0.1.5/mvapi/web/urls.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/views/sessions.py` & `mvapi-0.1.5/mvapi/web/views/sessions.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/views/users.py` & `mvapi-0.1.5/mvapi/web/views/users.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/views/__init__.py` & `mvapi-0.1.5/mvapi/web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/views/api.py` & `mvapi-0.1.5/mvapi/web/views/api.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/web/views/base.py` & `mvapi-0.1.5/mvapi/web/views/base.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/models/__init__.py` & `mvapi-0.1.5/mvapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/cli/project/user/create_user.py` & `mvapi-0.1.5/mvapi/cli/project/user/create_user.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/cli/project/user/update_user.py` & `mvapi-0.1.5/mvapi/cli/project/user/update_user.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/cli/project/migration/upgrade.py` & `mvapi-0.1.5/mvapi/cli/project/migration/upgrade.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/cli/project/migration/revision.py` & `mvapi-0.1.5/mvapi/cli/project/migration/revision.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/cli/project/migration/downgrade.py` & `mvapi-0.1.5/mvapi/cli/project/migration/downgrade.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/libs/misc.py` & `mvapi-0.1.5/mvapi/libs/misc.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/libs/error.py` & `mvapi-0.1.5/mvapi/libs/error.py`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/mvapi/templates/error.tmpl` & `mvapi-0.1.5/mvapi/templates/error.tmpl`

 * *Files identical despite different names*

### Comparing `mvapi-0.0.9/setup.py` & `mvapi-0.1.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 
 with open('./mvapi/version.py') as file:
     version = re.search(r'version = \'(.*?)\'', file.read()).group(1)
 
 setup(
     name='mvapi',
     version=version,
-    author='Mikhail Vetoshkin',
-    author_email='mikhail@vetoshkin.dev',
     description='Skeleton for a JSON API project',
+    license='GNU General Public License v3 (GPLv3)',
     url='https://git.vetoshkin.dev/mvapi/',
+    author='Mikhail Vetoshkin',
+    author_email='mikhail@vetoshkin.dev',
     packages=find_packages(),
     package_data={
         '': ['templates/*']
     },
     entry_points={
         'console_scripts': [
             'mvapi = mvapi:main'
         ]
     },
     install_requires=[
         'alembic == 1.7.5',
         'bcrypt == 3.2.0',
+        'blinker == 1.5',
         'click == 8.0.3',
         'flask == 2.0.2',
         'flask-cors == 3.0.10',
         'inflect == 5.4.0',
         'jinja2 == 3.0.3',
         'psycopg2 == 2.9.3',
         'pyjwt == 2.3.0',
```

### Comparing `mvapi-0.0.9/mvapi.egg-info/SOURCES.txt` & `mvapi-0.1.5/mvapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYING
 README.md
 setup.py
 mvapi/__init__.py
 mvapi/version.py
 mvapi.egg-info/PKG-INFO
 mvapi.egg-info/SOURCES.txt
 mvapi.egg-info/dependency_links.txt
```

