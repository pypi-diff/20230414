# Comparing `tmp/django-attachments-1.9.tar.gz` & `tmp/django-attachments-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-attachments-1.9.tar", last modified: Thu Apr 29 13:10:34 2021, max compression
+gzip compressed data, was "django-attachments-1.9.1.tar", last modified: Fri Apr 30 13:53:31 2021, max compression
```

## Comparing `django-attachments-1.9.tar` & `django-attachments-1.9.1.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.565703 django-attachments-1.9/
--rw-rw-r--   0 senko     (1001) senko     (1002)     3610 2021-04-29 13:09:54.000000 django-attachments-1.9/CHANGELOG.rst
--rw-rw-r--   0 senko     (1001) senko     (1002)     1542 2021-04-27 20:12:56.000000 django-attachments-1.9/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1002)      205 2021-04-27 20:12:56.000000 django-attachments-1.9/MANIFEST.in
--rw-rw-r--   0 senko     (1001) senko     (1002)    13761 2021-04-29 13:10:34.565703 django-attachments-1.9/PKG-INFO
--rw-rw-r--   0 senko     (1001) senko     (1002)      401 2021-04-27 20:12:56.000000 django-attachments-1.9/Pipfile
--rw-rw-r--   0 senko     (1001) senko     (1002)    13241 2021-04-27 20:12:56.000000 django-attachments-1.9/Pipfile.lock
--rw-rw-r--   0 senko     (1001) senko     (1002)     6380 2021-04-27 20:12:56.000000 django-attachments-1.9/README.rst
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.558702 django-attachments-1.9/attachments/
--rw-rw-r--   0 senko     (1001) senko     (1002)       58 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      243 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      283 2021-04-29 13:09:54.000000 django-attachments-1.9/attachments/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     1152 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/forms.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/
--rw-rw-r--   0 senko     (1001) senko     (1002)      309 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/README.transifex
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/da/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/da/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1266 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/de/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/de/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1207 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/el/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/el/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1402 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/en/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/en/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1209 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/es_AR/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/es_AR/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1210 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/es_AR/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/fi/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1250 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/fr/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1252 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.556702 django-attachments-1.9/attachments/locale/it/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/it/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1762 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.557702 django-attachments-1.9/attachments/locale/pt_BR/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1215 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.557702 django-attachments-1.9/attachments/locale/ru/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.559702 django-attachments-1.9/attachments/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1836 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.560702 django-attachments-1.9/attachments/management/
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/management/__init__.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.560702 django-attachments-1.9/attachments/management/commands/
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/management/commands/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     1491 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/management/commands/delete_stale_attachments.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.560702 django-attachments-1.9/attachments/migrations/
--rw-rw-r--   0 senko     (1001) senko     (1002)     1459 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      561 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/0002_auto_20180104_1247.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      384 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/0003_auto_20190722_1216.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      723 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/0004_db_index.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      353 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/0005_object_id_charfield.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      454 2021-04-29 09:00:40.000000 django-attachments-1.9/attachments/migrations/0007_auto_20210429_0400.py
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/migrations/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     3047 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/models.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.557702 django-attachments-1.9/attachments/templates/
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.561702 django-attachments-1.9/attachments/templates/attachments/
--rw-rw-r--   0 senko     (1001) senko     (1002)      119 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templates/attachments/add.html
--rw-rw-r--   0 senko     (1001) senko     (1002)      347 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templates/attachments/add_form.html
--rw-rw-r--   0 senko     (1001) senko     (1002)       33 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templates/attachments/base.html
--rw-rw-r--   0 senko     (1001) senko     (1002)      151 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templates/attachments/delete_link.html
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.562703 django-attachments-1.9/attachments/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     2390 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/templatetags/attachments_tags.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.563702 django-attachments-1.9/attachments/tests/
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     2277 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/base.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      562 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/test_integrity.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     2837 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/test_template.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     8567 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/test_views.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.563702 django-attachments-1.9/attachments/tests/testapp/
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      228 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/admin.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.564702 django-attachments-1.9/attachments/tests/testapp/migrations/
--rw-rw-r--   0 senko     (1001) senko     (1002)      491 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      393 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/migrations/0002_auto_20180104_1247.py
--rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/migrations/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      215 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/models.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     1859 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/settings.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.564702 django-attachments-1.9/attachments/tests/testapp/templates/
--rw-rw-r--   0 senko     (1001) senko     (1002)      372 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/templates/testmodel_detail.html
--rw-rw-r--   0 senko     (1001) senko     (1002)      629 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/tests/testapp/urls.py
--rw-rw-r--   0 senko     (1001) senko     (1002)      467 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/urls.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     2362 2021-04-27 20:12:56.000000 django-attachments-1.9/attachments/views.py
-drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-29 13:10:34.564702 django-attachments-1.9/django_attachments.egg-info/
--rw-rw-r--   0 senko     (1001) senko     (1002)    13761 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/PKG-INFO
--rw-rw-r--   0 senko     (1001) senko     (1002)     2259 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/SOURCES.txt
--rw-rw-r--   0 senko     (1001) senko     (1002)        1 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/dependency_links.txt
--rw-rw-r--   0 senko     (1001) senko     (1002)        1 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/not-zip-safe
--rw-rw-r--   0 senko     (1001) senko     (1002)       76 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/requires.txt
--rw-rw-r--   0 senko     (1001) senko     (1002)       12 2021-04-29 13:10:34.000000 django-attachments-1.9/django_attachments.egg-info/top_level.txt
--rw-rw-r--   0 senko     (1001) senko     (1002)     1683 2021-04-29 13:10:34.565703 django-attachments-1.9/setup.cfg
--rw-rw-r--   0 senko     (1001) senko     (1002)       59 2021-04-27 20:12:56.000000 django-attachments-1.9/setup.py
--rw-rw-r--   0 senko     (1001) senko     (1002)     1174 2021-04-29 09:34:10.000000 django-attachments-1.9/tox.ini
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.418493 django-attachments-1.9.1/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     3768 2021-04-30 13:52:08.000000 django-attachments-1.9.1/CHANGELOG.rst
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1542 2021-04-27 20:12:56.000000 django-attachments-1.9.1/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1002)      205 2021-04-27 20:12:56.000000 django-attachments-1.9.1/MANIFEST.in
+-rw-rw-r--   0 senko     (1001) senko     (1002)    13969 2021-04-30 13:53:31.418493 django-attachments-1.9.1/PKG-INFO
+-rw-rw-r--   0 senko     (1001) senko     (1002)      401 2021-04-27 20:12:56.000000 django-attachments-1.9.1/Pipfile
+-rw-rw-r--   0 senko     (1001) senko     (1002)    13241 2021-04-27 20:12:56.000000 django-attachments-1.9.1/Pipfile.lock
+-rw-rw-r--   0 senko     (1001) senko     (1002)     6380 2021-04-27 20:12:56.000000 django-attachments-1.9.1/README.rst
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.414493 django-attachments-1.9.1/attachments/
+-rw-rw-r--   0 senko     (1001) senko     (1002)       58 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      243 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      283 2021-04-29 13:09:54.000000 django-attachments-1.9.1/attachments/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1152 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/forms.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.414493 django-attachments-1.9.1/attachments/locale/
+-rw-rw-r--   0 senko     (1001) senko     (1002)      309 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/README.transifex
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/da/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.414493 django-attachments-1.9.1/attachments/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1266 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/de/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.414493 django-attachments-1.9.1/attachments/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1207 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/el/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1402 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/en/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1209 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/es_AR/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/es_AR/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1210 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/es_AR/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/fi/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1250 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/fr/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1252 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/it/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1762 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/pt_BR/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1215 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.412493 django-attachments-1.9.1/attachments/locale/ru/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1836 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/management/
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/management/__init__.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.415493 django-attachments-1.9.1/attachments/management/commands/
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/management/commands/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1491 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/management/commands/delete_stale_attachments.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.416493 django-attachments-1.9.1/attachments/migrations/
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1459 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      561 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/0002_auto_20180104_1247.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      384 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/0003_auto_20190722_1216.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      723 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/0004_db_index.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      353 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/0005_object_id_charfield.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/migrations/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     3047 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/models.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.413493 django-attachments-1.9.1/attachments/templates/
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.416493 django-attachments-1.9.1/attachments/templates/attachments/
+-rw-rw-r--   0 senko     (1001) senko     (1002)      119 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templates/attachments/add.html
+-rw-rw-r--   0 senko     (1001) senko     (1002)      347 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templates/attachments/add_form.html
+-rw-rw-r--   0 senko     (1001) senko     (1002)       33 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templates/attachments/base.html
+-rw-rw-r--   0 senko     (1001) senko     (1002)      151 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templates/attachments/delete_link.html
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.416493 django-attachments-1.9.1/attachments/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     2390 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/templatetags/attachments_tags.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.417493 django-attachments-1.9.1/attachments/tests/
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     2277 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/base.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      562 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/test_integrity.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     2837 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/test_template.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     8567 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/test_views.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.417493 django-attachments-1.9.1/attachments/tests/testapp/
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      228 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/admin.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.417493 django-attachments-1.9.1/attachments/tests/testapp/migrations/
+-rw-rw-r--   0 senko     (1001) senko     (1002)      491 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      393 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/migrations/0002_auto_20180104_1247.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)        0 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      215 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/models.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1859 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/settings.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.417493 django-attachments-1.9.1/attachments/tests/testapp/templates/
+-rw-rw-r--   0 senko     (1001) senko     (1002)      372 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/templates/testmodel_detail.html
+-rw-rw-r--   0 senko     (1001) senko     (1002)      629 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/tests/testapp/urls.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)      467 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/urls.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     2362 2021-04-27 20:12:56.000000 django-attachments-1.9.1/attachments/views.py
+drwxrwxr-x   0 senko     (1001) senko     (1002)        0 2021-04-30 13:53:31.418493 django-attachments-1.9.1/django_attachments.egg-info/
+-rw-rw-r--   0 senko     (1001) senko     (1002)    13969 2021-04-30 13:53:31.000000 django-attachments-1.9.1/django_attachments.egg-info/PKG-INFO
+-rw-rw-r--   0 senko     (1001) senko     (1002)     2209 2021-04-30 13:53:31.000000 django-attachments-1.9.1/django_attachments.egg-info/SOURCES.txt
+-rw-rw-r--   0 senko     (1001) senko     (1002)        1 2021-04-30 13:53:31.000000 django-attachments-1.9.1/django_attachments.egg-info/dependency_links.txt
+-rw-rw-r--   0 senko     (1001) senko     (1002)        1 2021-04-29 13:10:34.000000 django-attachments-1.9.1/django_attachments.egg-info/not-zip-safe
+-rw-rw-r--   0 senko     (1001) senko     (1002)       76 2021-04-30 13:53:31.000000 django-attachments-1.9.1/django_attachments.egg-info/requires.txt
+-rw-rw-r--   0 senko     (1001) senko     (1002)       12 2021-04-30 13:53:31.000000 django-attachments-1.9.1/django_attachments.egg-info/top_level.txt
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1685 2021-04-30 13:53:31.418493 django-attachments-1.9.1/setup.cfg
+-rw-rw-r--   0 senko     (1001) senko     (1002)       59 2021-04-27 20:12:56.000000 django-attachments-1.9.1/setup.py
+-rw-rw-r--   0 senko     (1001) senko     (1002)     1174 2021-04-29 09:34:10.000000 django-attachments-1.9.1/tox.ini
```

### Comparing `django-attachments-1.9/CHANGELOG.rst` & `django-attachments-1.9.1/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 Changelog:
 ==========
 
-v1.9 (2021-04-29)
------------------
+v1.9.1 (2021-04-30)
+-------------------
+
+- Rebuild the previous version but don't ship a left-over migration file
+
+
+v1.9 (2021-04-29) -- removed from PyPI
+--------------------------------------
 
 - Configure PK explicitly to AutoField for Django 3.2+, see
   https://docs.djangoproject.com/en/3.2/releases/3.2/#customizing-type-of-auto-created-primary-keys
 - Start testing with Django 3.2
 - Fix typo in README (Jesaja Everling)
 - Enable syntax highlighting in README (Basil S)
```

### Comparing `django-attachments-1.9/LICENSE` & `django-attachments-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/PKG-INFO` & `django-attachments-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-attachments
-Version: 1.9
+Version: 1.9.1
 Summary: django-attachments is generic Django application to attach Files (Attachments) to any model.
 Home-page: https://github.com/bartTC/django-attachments
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Description: .. image:: https://badge.fury.io/py/django-attachments.svg
             :target: https://badge.fury.io/py/django-attachments
@@ -228,16 +228,22 @@
             {% endfor %}
             </ul>
             {% endif %}
         
         Changelog:
         ==========
         
-        v1.9 (2021-04-29)
-        -----------------
+        v1.9.1 (2021-04-30)
+        -------------------
+        
+        - Rebuild the previous version but don't ship a left-over migration file
+        
+        
+        v1.9 (2021-04-29) -- removed from PyPI
+        --------------------------------------
         
         - Configure PK explicitly to AutoField for Django 3.2+, see
           https://docs.djangoproject.com/en/3.2/releases/3.2/#customizing-type-of-auto-created-primary-keys
         - Start testing with Django 3.2
         - Fix typo in README (Jesaja Everling)
         - Enable syntax highlighting in README (Basil S)
```

### Comparing `django-attachments-1.9/Pipfile.lock` & `django-attachments-1.9.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/README.rst` & `django-attachments-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/forms.py` & `django-attachments-1.9.1/attachments/forms.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/da/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/de/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/el/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/en/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/es_AR/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/fi/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/fr/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/it/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/pt_BR/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/locale/ru/LC_MESSAGES/django.po` & `django-attachments-1.9.1/attachments/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/management/commands/delete_stale_attachments.py` & `django-attachments-1.9.1/attachments/management/commands/delete_stale_attachments.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/migrations/0001_initial.py` & `django-attachments-1.9.1/attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/migrations/0002_auto_20180104_1247.py` & `django-attachments-1.9.1/attachments/migrations/0002_auto_20180104_1247.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/migrations/0004_db_index.py` & `django-attachments-1.9.1/attachments/migrations/0004_db_index.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/models.py` & `django-attachments-1.9.1/attachments/models.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/templatetags/attachments_tags.py` & `django-attachments-1.9.1/attachments/templatetags/attachments_tags.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/base.py` & `django-attachments-1.9.1/attachments/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/test_integrity.py` & `django-attachments-1.9.1/attachments/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/test_template.py` & `django-attachments-1.9.1/attachments/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/test_views.py` & `django-attachments-1.9.1/attachments/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/testapp/settings.py` & `django-attachments-1.9.1/attachments/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/tests/testapp/urls.py` & `django-attachments-1.9.1/attachments/tests/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/attachments/views.py` & `django-attachments-1.9.1/attachments/views.py`

 * *Files identical despite different names*

### Comparing `django-attachments-1.9/django_attachments.egg-info/PKG-INFO` & `django-attachments-1.9.1/django_attachments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-attachments
-Version: 1.9
+Version: 1.9.1
 Summary: django-attachments is generic Django application to attach Files (Attachments) to any model.
 Home-page: https://github.com/bartTC/django-attachments
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Description: .. image:: https://badge.fury.io/py/django-attachments.svg
             :target: https://badge.fury.io/py/django-attachments
@@ -228,16 +228,22 @@
             {% endfor %}
             </ul>
             {% endif %}
         
         Changelog:
         ==========
         
-        v1.9 (2021-04-29)
-        -----------------
+        v1.9.1 (2021-04-30)
+        -------------------
+        
+        - Rebuild the previous version but don't ship a left-over migration file
+        
+        
+        v1.9 (2021-04-29) -- removed from PyPI
+        --------------------------------------
         
         - Configure PK explicitly to AutoField for Django 3.2+, see
           https://docs.djangoproject.com/en/3.2/releases/3.2/#customizing-type-of-auto-created-primary-keys
         - Start testing with Django 3.2
         - Fix typo in README (Jesaja Everling)
         - Enable syntax highlighting in README (Basil S)
```

### Comparing `django-attachments-1.9/django_attachments.egg-info/SOURCES.txt` & `django-attachments-1.9.1/django_attachments.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 attachments/management/commands/__init__.py
 attachments/management/commands/delete_stale_attachments.py
 attachments/migrations/0001_initial.py
 attachments/migrations/0002_auto_20180104_1247.py
 attachments/migrations/0003_auto_20190722_1216.py
 attachments/migrations/0004_db_index.py
 attachments/migrations/0005_object_id_charfield.py
-attachments/migrations/0007_auto_20210429_0400.py
 attachments/migrations/__init__.py
 attachments/templates/attachments/add.html
 attachments/templates/attachments/add_form.html
 attachments/templates/attachments/base.html
 attachments/templates/attachments/delete_link.html
 attachments/templatetags/__init__.py
 attachments/templatetags/attachments_tags.py
```

### Comparing `django-attachments-1.9/setup.cfg` & `django-attachments-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-attachments
-version = 1.9
+version = 1.9.1
 description = django-attachments is generic Django application to attach Files (Attachments) to any model.
 long_description = file: README.rst, CHANGELOG.rst
 author = Martin Mahner
 author_email = martin@mahner.org
 url = https://github.com/bartTC/django-attachments
 keywords = django, attachments, files, upload
 license = MIT
```

### Comparing `django-attachments-1.9/tox.ini` & `django-attachments-1.9.1/tox.ini`

 * *Files identical despite different names*

