# Comparing `tmp/wagtailstreamforms-4.0.2.tar.gz` & `tmp/wagtailstreamforms-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailstreamforms-4.0.2.tar", last modified: Fri Apr 14 09:06:32 2023, max compression
+gzip compressed data, was "wagtailstreamforms-4.0.3.tar", last modified: Fri Apr 14 12:52:04 2023, max compression
```

## Comparing `wagtailstreamforms-4.0.2.tar` & `wagtailstreamforms-4.0.3.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/prunesubmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0002_form_site.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/models/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/streamfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/advanced_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/form_block.html
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/index_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/list_submissions.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/non_existent_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/form_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.547336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/streamforms_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.555336 wagtailstreamforms-4.0.2/wagtailstreamforms/views/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-14 09:06:28.000000 wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:06:32.551336 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 09:06:32.000000 wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.126981 wagtailstreamforms-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 12:52:04.126981 wagtailstreamforms-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 12:52:04.126981 wagtailstreamforms-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/management/commands/prunesubmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/0002_form_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/0003_alter_form_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/models/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/models/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/streamfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/advanced_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/confirm_copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/form_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/index_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/list_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/non_existent_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/partials/form_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.114981 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/wagtailadmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.122981 wagtailstreamforms-4.0.3/wagtailstreamforms/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/templatetags/streamforms_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.126981 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.126981 wagtailstreamforms-4.0.3/wagtailstreamforms/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/views/advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/views/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/views/submission_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/views/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/wagtailstreamforms_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-14 12:52:01.000000 wagtailstreamforms-4.0.3/wagtailstreamforms/wagtailstreamforms_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.118981 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-14 12:52:03.000000 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-14 12:52:04.000000 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:03.000000 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-14 12:52:03.000000 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 12:52:03.000000 wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/top_level.txt
```

### Comparing `wagtailstreamforms-4.0.2/LICENSE` & `wagtailstreamforms-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/PKG-INFO` & `wagtailstreamforms-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.2
+Version: 4.0.3
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.2/README.rst` & `wagtailstreamforms-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/setup.py` & `wagtailstreamforms-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/blocks.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from wagtailstreamforms.wagtail_hooks import WagtailStreamFormsChooser
 
 
 class InfoBlock(blocks.CharBlock):
     def render_form(self, value, prefix="", errors=None):
         field = self.field
         shown_value = value if value else field.help_text
-        return mark_safe(
-            '<div style="margin-top:5px;padding:0.9em 1.2em;">%s</div>' % shown_value
-        )
+        return mark_safe('<div style="margin-top:5px;padding:0.9em 1.2em;">%s</div>' % shown_value)
 
 
 class FormChooserBlock(blocks.ChooserBlock):
     @cached_property
     def target_model(self):
         return Form
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/conf.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/conf.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/fields.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,15 @@
         defaults = {
             "form_class": HookMultiSelectFormField,
             "choices": self.get_choices_default(),
         }
         defaults.update(kwargs)
         return super().formfield(**defaults)
 
-    def from_db_value(
-        self, value, expression, connection, context=None, *args, **kwargs
-    ):
+    def from_db_value(self, value, expression, connection, context=None, *args, **kwargs):
         if value is None or value == "":
             return []
         return value.split(",")
 
     def to_python(self, value):
         if not value or value == "":
             return []
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/forms.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 
         for field in self.fields:
             field_type = field.get("type")
             field_value = field.get("value")
 
             # check we have the field
             if field_type not in registered_fields:
-                raise AttributeError(
-                    "Could not find a registered field of type %s" % field_type
-                )
+                raise AttributeError("Could not find a registered field of type %s" % field_type)
 
             # get the field
             registered_cls = registered_fields[field_type]()
             field_name = registered_cls.get_formfield_name(field_value)
             field_cls = registered_cls.get_formfield(field_value)
             formfields[field_name] = field_cls
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/hooks.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/es/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.3/wagtailstreamforms/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.3/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.3/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/management/commands/prunesubmissions.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/management/commands/prunesubmissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     def add_arguments(self, parser):
         parser.add_argument("days_to_keep", type=int)
 
     def get_queryset(self, date):
         return FormSubmission.objects.filter(submit_time__lt=date)
 
     def handle(self, *args, **options):
-        keep_from_date = datetime.today().date() - timedelta(
-            days=options["days_to_keep"]
-        )
+        keep_from_date = datetime.today().date() - timedelta(days=options["days_to_keep"])
 
         queryset = self.get_queryset(keep_from_date)
 
         count = queryset.count()
         queryset.delete()
 
         msg = "Successfully deleted %s form submissions prior to %s" % (
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0001_initial.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/migrations/0002_form_site.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/migrations/0002_form_site.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/models/__init__.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/models/file.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/models/file.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/models/form.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/models/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,30 +55,26 @@
             "An optional success message to show when the form has been successfully submitted"
         ),
     )
     error_message = models.CharField(
         _("Error message"),
         blank=True,
         max_length=255,
-        help_text=_(
-            "An optional error message to show when the form has validation errors"
-        ),
+        help_text=_("An optional error message to show when the form has validation errors"),
     )
     post_redirect_page = models.ForeignKey(
         "wagtailcore.Page",
         verbose_name=_("Post redirect page"),
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name="+",
         help_text=_("The page to redirect to after a successful submission"),
     )
-    process_form_submission_hooks = HookSelectField(
-        verbose_name=_("Submission hooks"), blank=True
-    )
+    process_form_submission_hooks = HookSelectField(verbose_name=_("Submission hooks"), blank=True)
 
     objects = FormQuerySet.as_manager()
 
     settings_panels = [
         FieldPanel("title", classname="full"),
         FieldPanel("slug"),
         FieldPanel("template_name"),
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/models/submission.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/models/submission.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/streamfield.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/streamfield.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/advanced_settings.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/advanced_settings.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_copy.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/confirm_copy.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/confirm_delete.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/index_submissions.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/list_submissions.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/templatetags/streamforms_tags.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/templatetags/streamforms_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,13 @@
         form = Form.objects.get(slug=slug)
 
         block = WagtailFormBlock()
 
         # the context is a RequestContext, we need to turn it into a dict or
         # the blocks in wagtail will start to fail with dict(context)
         return block.render(
-            block.to_python(
-                {"form": form.pk, "form_action": action, "form_reference": reference}
-            ),
+            block.to_python({"form": form.pk, "form_action": action, "form_reference": reference}),
             context.flatten(),
         )
 
     except Form.DoesNotExist:
         return mark_safe("")
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/urls.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/utils/apps.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/utils/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/utils/loading.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/utils/loading.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/views/advanced_settings.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/views/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/views/copy.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/views/copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,15 @@
         context = self.get_context_data(object=self.object)
         context["form"] = form
 
         return self.render_to_response(context)
 
     def get(self, request, *args, **kwargs):
         context = self.get_context_data(object=self.object)
-        context["form"] = CopyForm(
-            initial={"title": self.object.title, "slug": self.object.slug}
-        )
+        context["form"] = CopyForm(initial={"title": self.object.title, "slug": self.object.slug})
 
         return self.render_to_response(context)
 
     def post(self, request, *args, **kwargs):
         return self.copy(request, *args, **kwargs)
 
     def create_success_message(self, copied):
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_delete.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/views/submission_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     @property
     def permission_helper(self):
         return PermissionHelper(model=self.model)
 
     def dispatch(self, request, *args, **kwargs):
         self.object = self.get_object()
-        if not self.permission_helper.user_can_delete_obj(
-            self.request.user, self.object
-        ):
+        if not self.permission_helper.user_can_delete_obj(self.request.user, self.object):
             raise PermissionDenied
         return super().dispatch(request, *args, **kwargs)
 
     def get_object(self, queryset=None):
         obj = super().get_object(queryset)
         return obj
 
@@ -68,10 +66,8 @@
                 "%(count)d submissions have been deleted.",
                 count,
             )
             % {"count": count},
         )
 
     def get_success_url(self):
-        return reverse(
-            "wagtailstreamforms:streamforms_submissions", kwargs={"pk": self.object.pk}
-        )
+        return reverse("wagtailstreamforms:streamforms_submissions", kwargs={"pk": self.object.pk})
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/views/submission_list.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/views/submission_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,15 @@
 
         # populate data rows from paginator
         data_rows = []
         for s in context["page_obj"]:
             form_data = s.get_data()
             form_files = s.files.all()
             data_row = [form_data.get(name) for name, label in data_fields]
-            data_rows.append(
-                {"model_id": s.id, "fields": data_row, "files": form_files}
-            )
+            data_rows.append({"model_id": s.id, "fields": data_row, "files": form_files})
 
         context.update(
             {
                 "filter_form": self.filter_form,
                 "data_rows": data_rows,
                 "data_headings": data_headings,
                 "has_delete_permission": self.permission_helper.user_can_delete_obj(
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtail_hooks.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/wagtail_hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 SettingsModel = get_advanced_settings_model()
 
 
 class FormURLHelper(AdminURLHelper):
     def get_action_url(self, action, *args, **kwargs):
         if action in ["advanced", "copy", "submissions"]:
-            return reverse(
-                "wagtailstreamforms:streamforms_%s" % action, args=args, kwargs=kwargs
-            )
+            return reverse("wagtailstreamforms:streamforms_%s" % action, args=args, kwargs=kwargs)
 
         return super().get_action_url(action, *args, **kwargs)
 
 
 class FormButtonHelper(ButtonHelper):
     def button(self, pk, action, label, title, classnames_add, classnames_exclude):
         cn = self.finalise_classname(classnames_add, classnames_exclude)
@@ -44,29 +42,23 @@
             "label": label,
             "classname": cn,
             "title": title,
         }
 
         return button
 
-    def get_buttons_for_obj(
-        self, obj, exclude=None, classnames_add=None, classnames_exclude=None
-    ):
-        buttons = super().get_buttons_for_obj(
-            obj, exclude, classnames_add, classnames_exclude
-        )
+    def get_buttons_for_obj(self, obj, exclude=None, classnames_add=None, classnames_exclude=None):
+        buttons = super().get_buttons_for_obj(obj, exclude, classnames_add, classnames_exclude)
         pk = getattr(obj, self.opts.pk.attname)
         ph = self.permission_helper
         usr = self.request.user
 
         # if there is a form settings model defined
         # users that either create or edit forms should be able edit advanced settings
-        if SettingsModel and (
-            ph.user_can_create(usr) or ph.user_can_edit_obj(usr, obj)
-        ):
+        if SettingsModel and (ph.user_can_create(usr) or ph.user_can_edit_obj(usr, obj)):
             buttons.append(
                 self.button(
                     pk,
                     "advanced",
                     _("Advanced"),
                     _("Advanced settings"),
                     classnames_add,
@@ -169,19 +161,15 @@
         list_filter = self.list_filter
         for fn in form_hooks.get_hooks("construct_form_list_filter"):
             list_filter = fn(list_filter, request)
         return list_filter
 
     def latest_submission(self, obj):
         submission_class = obj.get_submission_class()
-        return (
-            submission_class._default_manager.filter(form=obj)
-            .latest("submit_time")
-            .submit_time
-        )
+        return submission_class._default_manager.filter(form=obj).latest("submit_time").submit_time
 
     latest_submission.short_description = _("Latest submission")
 
     def saved_submissions(self, obj):
         submission_class = obj.get_submission_class()
         return submission_class._default_manager.filter(form=obj).count()
 
@@ -203,43 +191,37 @@
     if not get_setting("ENABLE_FORM_PROCESSING"):
         return
 
     if request.method == "POST":
         form_def = get_form_instance_from_request(request)
 
         if form_def:
-            form = form_def.get_form(
-                request.POST, request.FILES, page=page, user=request.user
-            )
+            form = form_def.get_form(request.POST, request.FILES, page=page, user=request.user)
             context = page.get_context(request, *args, **kwargs)
 
             if form.is_valid():
                 # process the form submission
                 form_def.process_form_submission(form)
 
                 # create success message
                 if form_def.success_message:
-                    messages.success(
-                        request, form_def.success_message, fail_silently=True
-                    )
+                    messages.success(request, form_def.success_message, fail_silently=True)
 
                 # redirect to the page defined in the form
                 # or the current page as a fallback - this will avoid refreshing
                 # and submitting again
                 redirect_page = form_def.post_redirect_page or page
 
                 return redirect(redirect_page.get_url(request), context=context)
 
             else:
                 # update the context with the invalid form and serve the page
                 context.update(
                     {
-                        "invalid_stream_form_reference": form.data.get(
-                            "form_reference"
-                        ),
+                        "invalid_stream_form_reference": form.data.get("form_reference"),
                         "invalid_stream_form": form,
                     }
                 )
 
                 # create error message
                 if form_def.error_message:
                     messages.error(request, form_def.error_message, fail_silently=True)
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_fields.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/wagtailstreamforms_fields.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms/wagtailstreamforms_hooks.py` & `wagtailstreamforms-4.0.3/wagtailstreamforms/wagtailstreamforms_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,8 @@
         form_data=json.dumps(submission_data, cls=FormSubmissionSerializer),
         form=instance,
     )
 
     # save the form files
     for field in form.files:
         for file in form.files.getlist(field):
-            FormSubmissionFile.objects.create(
-                submission=submission, field=field, file=file
-            )
+            FormSubmissionFile.objects.create(submission=submission, field=field, file=file)
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/PKG-INFO` & `wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 4.0.2
+Version: 4.0.3
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
```

### Comparing `wagtailstreamforms-4.0.2/wagtailstreamforms.egg-info/SOURCES.txt` & `wagtailstreamforms-4.0.3/wagtailstreamforms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 wagtailstreamforms/__init__.py
 wagtailstreamforms/blocks.py
 wagtailstreamforms/conf.py
 wagtailstreamforms/fields.py
 wagtailstreamforms/forms.py
@@ -27,14 +28,15 @@
 wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
 wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
 wagtailstreamforms/management/__init__.py
 wagtailstreamforms/management/commands/__init__.py
 wagtailstreamforms/management/commands/prunesubmissions.py
 wagtailstreamforms/migrations/0001_initial.py
 wagtailstreamforms/migrations/0002_form_site.py
+wagtailstreamforms/migrations/0003_alter_form_fields.py
 wagtailstreamforms/migrations/__init__.py
 wagtailstreamforms/models/__init__.py
 wagtailstreamforms/models/abstract.py
 wagtailstreamforms/models/file.py
 wagtailstreamforms/models/form.py
 wagtailstreamforms/models/submission.py
 wagtailstreamforms/templates/streamforms/advanced_settings.html
```

