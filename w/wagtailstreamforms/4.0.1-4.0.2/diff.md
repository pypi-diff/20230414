# Comparing `tmp/wagtailstreamforms-4.0.1.tar.gz` & `tmp/wagtailstreamforms-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailstreamforms-4.0.1.tar", last modified: Thu Apr 13 14:27:52 2023, max compression
+gzip compressed data, was "wagtailstreamforms-4.0.2.tar", last modified: Fri Apr 14 09:06:32 2023, max compression
```

## Comparing `wagtailstreamforms-4.0.1.tar` & `wagtailstreamforms-4.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 14:27:52.654876 wagtailstreamforms-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.638875 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/prunesubmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0002_form_site.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/streamfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/advanced_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/form_block.html
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/index_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/list_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/non_existent_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/form_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/streamforms_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/views/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/prunesubmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0002_form_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/streamfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/advanced_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/form_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/index_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/list_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/non_existent_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/form_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/streamforms_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/top_level.txt
```

### Comparing `wagtailstreamforms-4.0.1/LICENSE` & `wagtailstreamforms-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/PKG-INFO` & `wagtailstreamforms-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.1
+Version: 4.0.2
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.1/README.rst` & `wagtailstreamforms-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/setup.py` & `wagtailstreamforms-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/blocks.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/conf.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/conf.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/fields.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/forms.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/hooks.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/prunesubmissions.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/prunesubmissions.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0001_initial.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0002_form_site.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0002_form_site.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/models/__init__.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/models/file.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/models/file.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/models/form.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/models/form.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/models/submission.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/models/submission.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/streamfield.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/streamfield.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,9 @@
     @property
     def dependencies(self):
         return self._dependencies
 
 
 class FormFieldsStreamField(StreamField):
     def __init__(self, block_types, use_json_field=None, **kwargs):
-        super().__init__(block_types, **kwargs)
+        super().__init__(block_types, use_json_field=use_json_field, **kwargs)
         self.stream_block = FormFieldStreamBlock(block_types, required=not self.blank)
```

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/advanced_settings.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/advanced_settings.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_copy.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_copy.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_delete.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/index_submissions.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/list_submissions.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/streamforms_tags.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/streamforms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/urls.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/utils/apps.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/utils/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/utils/loading.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/utils/loading.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/views/advanced_settings.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/views/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/views/copy.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/views/copy.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_delete.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_delete.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_list.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_list.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtail_hooks.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_fields.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_fields.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_hooks.py` & `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/PKG-INFO` & `wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.1
+Version: 4.0.2
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/SOURCES.txt` & `wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

