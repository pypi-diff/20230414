# Comparing `tmp/django-statusboard-0.9.2.tar.gz` & `tmp/django-statusboard-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-statusboard-0.9.2.tar", last modified: Tue May 19 06:44:37 2020, max compression
+gzip compressed data, was "dist/django-statusboard-0.9.3.tar", last modified: Tue May 19 07:03:17 2020, max compression
```

## Comparing `django-statusboard-0.9.2.tar` & `django-statusboard-0.9.3.tar`

### file list

```diff
@@ -1,116 +1,120 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18046 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      281 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     7132 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4304 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7132 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4589 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/django_statusboard.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/
--rw-rw-r--   0 travis    (2000) travis    (2000)      868 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1192 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2509 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/forms.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/locale/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/locale/it/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/locale/it/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6461 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)    10698 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1436 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0002_incident.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0003_auto_20170121_2030.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1748 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0003_auto_20170125_0604.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0004_incident_occurred.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0005_merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0006_maintenance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4248 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0007_auto_20170213_1114.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0008_servicegroup_collapse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      562 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0009_auto_20170217_0749.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0009_servicegroup_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0010_auto_20170217_0835.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4466 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0011_auto_20170217_1120.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0012_auto_20170217_1322.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0013_auto_20170220_1444.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0014_incident_closed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0014_merge_20170222_2054.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0015_close_previously_fixed_incidents.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0015_merge_20170222_2058.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0016_auto_20170223_1005.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0016_service_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0017_auto_20170223_1428.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0018_merge_20170223_1429.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0019_auto_20170223_1503.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/0020_auto_20170223_1651.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9115 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/serializers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2157 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/settings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/statusboard/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25682 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap-theme.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    23411 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap-theme.min.css
--rw-rw-r--   0 travis    (2000) travis    (2000)   145933 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap.css
--rw-rw-r--   0 travis    (2000) travis    (2000)   121457 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap.min.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     1457 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/css/statusboard.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-default.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-major.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-operational.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-partial.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-performance.ico
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20127 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 travis    (2000) travis    (2000)   108738 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)    45404 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 travis    (2000) travis    (2000)    23424 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 travis    (2000) travis    (2000)    18028 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/static/statusboard/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)    75484 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/js/bootstrap.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    39680 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/js/bootstrap.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    86709 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/js/jquery-3.1.1.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      484 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/static/statusboard/js/npm.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4718 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/base.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/archive_month.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/archive_month_empty.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/archive_paginate_snippet.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      669 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/confirm_delete.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/create.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/edit.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1693 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/incident/list_snippet.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1856 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1891 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/login.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/
--rw-rw-r--   0 travis    (2000) travis    (2000)      678 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/confirm_delete.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/create.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/edit.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      427 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/note.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/raw_data_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/raw_data_form_errors.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      666 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/service/confirm_delete.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/service/create.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      281 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/service/edit.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/service/form.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/
--rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/confirm_delete.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/create.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/edit.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4557 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/list_snippet.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 06:44:37.000000 django-statusboard-0.9.2/statusboard/templatetags/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templatetags/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2176 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/templatetags/statusboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8804 2020-05-19 06:43:58.000000 django-statusboard-0.9.2/statusboard/views.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18046 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7132 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4304 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7132 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4821 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/django_statusboard.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      868 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1192 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/admin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2509 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/forms.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/locale/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/locale/it/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6461 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10698 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1436 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0002_incident.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0003_auto_20170121_2030.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1748 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0003_auto_20170125_0604.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      510 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0004_incident_occurred.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      345 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0005_merge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0006_maintenance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4248 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0007_auto_20170213_1114.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0008_servicegroup_collapse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      562 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0009_auto_20170217_0749.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0009_servicegroup_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0010_auto_20170217_0835.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4466 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0011_auto_20170217_1120.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0012_auto_20170217_1322.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0013_auto_20170220_1444.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0014_incident_closed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0014_merge_20170222_2054.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0015_close_previously_fixed_incidents.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0015_merge_20170222_2058.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0016_auto_20170223_1005.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0016_service_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0017_auto_20170223_1428.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0018_merge_20170223_1429.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0019_auto_20170223_1503.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      486 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/0020_auto_20170223_1651.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9115 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2157 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/settings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/statusboard/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25682 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48005 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23411 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.min.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75600 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.min.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)   145933 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)   390887 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)   121457 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.min.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)   540434 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.min.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1457 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/css/statusboard.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-default.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-major.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-operational.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-partial.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-performance.ico
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20127 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108738 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45404 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23424 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18028 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/static/statusboard/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75484 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/js/bootstrap.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39680 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/js/bootstrap.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86709 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/js/jquery-3.1.1.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      484 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/static/statusboard/js/npm.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4718 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/base.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      483 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/archive_month.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      211 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/archive_month_empty.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      681 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/archive_paginate_snippet.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      669 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/confirm_delete.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/create.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/edit.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1693 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/incident/list_snippet.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1856 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1891 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/login.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      678 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/confirm_delete.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/create.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/edit.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      427 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/note.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/raw_data_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/raw_data_form_errors.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/service/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      666 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/service/confirm_delete.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/service/create.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      281 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/service/edit.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/service/form.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/confirm_delete.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/create.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/edit.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4557 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/list_snippet.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-19 07:03:17.000000 django-statusboard-0.9.3/statusboard/templatetags/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templatetags/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2176 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/templatetags/statusboard.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8804 2020-05-19 07:02:35.000000 django-statusboard-0.9.3/statusboard/views.py
```

### Comparing `django-statusboard-0.9.2/LICENSE` & `django-statusboard-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/PKG-INFO` & `django-statusboard-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-statusboard
-Version: 0.9.2
+Version: 0.9.3
 Summary: Django app to show system status
 Home-page: http://github.com/edigiacomo/django-statusboard
 Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc
 License: GPLv2+
 Description: statusboard
         ===========
```

### Comparing `django-statusboard-0.9.2/README.md` & `django-statusboard-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/django_statusboard.egg-info/PKG-INFO` & `django-statusboard-0.9.3/django_statusboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-statusboard
-Version: 0.9.2
+Version: 0.9.3
 Summary: Django app to show system status
 Home-page: http://github.com/edigiacomo/django-statusboard
 Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc
 License: GPLv2+
 Description: statusboard
         ===========
```

### Comparing `django-statusboard-0.9.2/django_statusboard.egg-info/SOURCES.txt` & `django-statusboard-0.9.3/django_statusboard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,21 @@
 statusboard/migrations/0016_service_position.py
 statusboard/migrations/0017_auto_20170223_1428.py
 statusboard/migrations/0018_merge_20170223_1429.py
 statusboard/migrations/0019_auto_20170223_1503.py
 statusboard/migrations/0020_auto_20170223_1651.py
 statusboard/migrations/__init__.py
 statusboard/static/statusboard/css/bootstrap-theme.css
+statusboard/static/statusboard/css/bootstrap-theme.css.map
 statusboard/static/statusboard/css/bootstrap-theme.min.css
+statusboard/static/statusboard/css/bootstrap-theme.min.css.map
 statusboard/static/statusboard/css/bootstrap.css
+statusboard/static/statusboard/css/bootstrap.css.map
 statusboard/static/statusboard/css/bootstrap.min.css
+statusboard/static/statusboard/css/bootstrap.min.css.map
 statusboard/static/statusboard/css/statusboard.css
 statusboard/static/statusboard/favicons/statusboard-icon-default.ico
 statusboard/static/statusboard/favicons/statusboard-icon-major.ico
 statusboard/static/statusboard/favicons/statusboard-icon-operational.ico
 statusboard/static/statusboard/favicons/statusboard-icon-partial.ico
 statusboard/static/statusboard/favicons/statusboard-icon-performance.ico
 statusboard/static/statusboard/fonts/glyphicons-halflings-regular.eot
```

### Comparing `django-statusboard-0.9.2/setup.py` & `django-statusboard-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/__init__.py` & `django-statusboard-0.9.3/statusboard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __title__ = 'Django status board'
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 __author__ = 'Emanuele Di Giacomo'
 __license__ = 'GPLv2+'
 __copyright__ = 'Copyright 2017 Emanuele Di Giacomo'
```

### Comparing `django-statusboard-0.9.2/statusboard/admin.py` & `django-statusboard-0.9.3/statusboard/admin.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/apps.py` & `django-statusboard-0.9.3/statusboard/apps.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/forms.py` & `django-statusboard-0.9.3/statusboard/forms.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/locale/it/LC_MESSAGES/django.mo` & `django-statusboard-0.9.3/statusboard/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/locale/it/LC_MESSAGES/django.po` & `django-statusboard-0.9.3/statusboard/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0001_initial.py` & `django-statusboard-0.9.3/statusboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0002_incident.py` & `django-statusboard-0.9.3/statusboard/migrations/0002_incident.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0003_auto_20170121_2030.py` & `django-statusboard-0.9.3/statusboard/migrations/0003_auto_20170121_2030.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0003_auto_20170125_0604.py` & `django-statusboard-0.9.3/statusboard/migrations/0003_auto_20170125_0604.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0006_maintenance.py` & `django-statusboard-0.9.3/statusboard/migrations/0006_maintenance.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0007_auto_20170213_1114.py` & `django-statusboard-0.9.3/statusboard/migrations/0007_auto_20170213_1114.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0009_auto_20170217_0749.py` & `django-statusboard-0.9.3/statusboard/migrations/0009_auto_20170217_0749.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0010_auto_20170217_0835.py` & `django-statusboard-0.9.3/statusboard/migrations/0010_auto_20170217_0835.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0011_auto_20170217_1120.py` & `django-statusboard-0.9.3/statusboard/migrations/0011_auto_20170217_1120.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0012_auto_20170217_1322.py` & `django-statusboard-0.9.3/statusboard/migrations/0012_auto_20170217_1322.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0013_auto_20170220_1444.py` & `django-statusboard-0.9.3/statusboard/migrations/0013_auto_20170220_1444.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0015_close_previously_fixed_incidents.py` & `django-statusboard-0.9.3/statusboard/migrations/0015_close_previously_fixed_incidents.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0016_auto_20170223_1005.py` & `django-statusboard-0.9.3/statusboard/migrations/0016_auto_20170223_1005.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0017_auto_20170223_1428.py` & `django-statusboard-0.9.3/statusboard/migrations/0017_auto_20170223_1428.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/migrations/0019_auto_20170223_1503.py` & `django-statusboard-0.9.3/statusboard/migrations/0019_auto_20170223_1503.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/models.py` & `django-statusboard-0.9.3/statusboard/models.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/serializers.py` & `django-statusboard-0.9.3/statusboard/serializers.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/settings.py` & `django-statusboard-0.9.3/statusboard/settings.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap-theme.css` & `django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap-theme.min.css` & `django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap.css` & `django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/css/bootstrap.min.css` & `django-statusboard-0.9.3/statusboard/static/statusboard/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/css/statusboard.css` & `django-statusboard-0.9.3/statusboard/static/statusboard/css/statusboard.css`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-default.ico` & `django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-default.ico`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-major.ico` & `django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-major.ico`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-operational.ico` & `django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-operational.ico`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-partial.ico` & `django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-partial.ico`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/favicons/statusboard-icon-performance.ico` & `django-statusboard-0.9.3/statusboard/static/statusboard/favicons/statusboard-icon-performance.ico`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.eot` & `django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.svg` & `django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.ttf` & `django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff` & `django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff2` & `django-statusboard-0.9.3/statusboard/static/statusboard/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/js/bootstrap.js` & `django-statusboard-0.9.3/statusboard/static/statusboard/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/js/bootstrap.min.js` & `django-statusboard-0.9.3/statusboard/static/statusboard/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/static/statusboard/js/jquery-3.1.1.min.js` & `django-statusboard-0.9.3/statusboard/static/statusboard/js/jquery-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/base.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/base.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/incident/archive_paginate_snippet.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/incident/archive_paginate_snippet.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/incident/confirm_delete.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/incident/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/incident/form.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/incident/form.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/incident/list_snippet.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/incident/list_snippet.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/index.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/index.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/login.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/login.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/maintenance/confirm_delete.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/maintenance/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/raw_data_form.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/raw_data_form.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/service/confirm_delete.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/service/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/confirm_delete.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templates/statusboard/servicegroup/list_snippet.html` & `django-statusboard-0.9.3/statusboard/templates/statusboard/servicegroup/list_snippet.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/templatetags/statusboard.py` & `django-statusboard-0.9.3/statusboard/templatetags/statusboard.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/urls.py` & `django-statusboard-0.9.3/statusboard/urls.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-0.9.2/statusboard/views.py` & `django-statusboard-0.9.3/statusboard/views.py`

 * *Files identical despite different names*

