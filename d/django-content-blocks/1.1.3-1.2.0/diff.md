# Comparing `tmp/django-content-blocks-1.1.3.tar.gz` & `tmp/django-content-blocks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.1.3.tar", last modified: Tue Apr  4 14:29:26 2023, max compression
+gzip compressed data, was "django-content-blocks-1.2.0.tar", last modified: Fri Apr 14 13:30:05 2023, max compression
```

## Comparing `django-content-blocks-1.1.3.tar` & `django-content-blocks-1.2.0.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.361163 django-content-blocks-1.1.3/
--rw-r--r--   0 quantra    (501) staff       (20)     1075 2023-03-16 15:50:21.000000 django-content-blocks-1.1.3/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)      146 2023-03-07 15:39:03.000000 django-content-blocks-1.1.3/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     3458 2023-04-04 14:29:26.361282 django-content-blocks-1.1.3/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     2001 2023-03-20 13:07:58.000000 django-content-blocks-1.1.3/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.322813 django-content-blocks-1.1.3/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.1.3/content_blocks/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3047 2023-03-01 13:20:40.000000 django-content-blocks-1.1.3/content_blocks/abstract_models.py
--rw-r--r--   0 quantra    (501) staff       (20)    10457 2023-03-07 16:00:12.000000 django-content-blocks-1.1.3/content_blocks/admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     4041 2023-03-08 14:20:23.000000 django-content-blocks-1.1.3/content_blocks/admin_forms.py
--rw-r--r--   0 quantra    (501) staff       (20)     1601 2023-02-23 15:19:48.000000 django-content-blocks-1.1.3/content_blocks/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)      158 2023-01-05 16:14:15.000000 django-content-blocks-1.1.3/content_blocks/cache.py
--rw-r--r--   0 quantra    (501) staff       (20)     1654 2023-03-10 11:51:54.000000 django-content-blocks-1.1.3/content_blocks/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)     1929 2023-03-07 15:39:03.000000 django-content-blocks-1.1.3/content_blocks/fields.py
--rw-r--r--   0 quantra    (501) staff       (20)     7501 2023-04-04 14:24:55.000000 django-content-blocks-1.1.3/content_blocks/forms.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.323699 django-content-blocks-1.1.3/content_blocks/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.1.3/content_blocks/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.325337 django-content-blocks-1.1.3/content_blocks/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.1.3/content_blocks/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      459 2023-02-27 23:55:14.000000 django-content-blocks-1.1.3/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 quantra    (501) staff       (20)      461 2023-02-27 23:57:07.000000 django-content-blocks-1.1.3/content_blocks/management/commands/update_content_blocks_cache.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.326620 django-content-blocks-1.1.3/content_blocks/migrations/
--rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.1.3/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.1.3/content_blocks/migrations/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    22599 2023-04-04 12:39:54.000000 django-content-blocks-1.1.3/content_blocks/models.py
--rw-r--r--   0 quantra    (501) staff       (20)      410 2023-02-28 12:22:17.000000 django-content-blocks-1.1.3/content_blocks/permissions.py
--rw-r--r--   0 quantra    (501) staff       (20)     4874 2023-02-28 19:46:26.000000 django-content-blocks-1.1.3/content_blocks/signals.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.305254 django-content-blocks-1.1.3/content_blocks/static/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.326831 django-content-blocks-1.1.3/content_blocks/static/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.328660 django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      722 2023-02-17 13:42:24.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 quantra    (501) staff       (20)     9336 2023-03-09 18:25:40.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.329037 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 19:46:37.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.332177 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 18:56:30.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)    80823 2023-01-30 19:05:04.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      753 2023-03-04 01:20:32.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 quantra    (501) staff       (20)      572 2023-01-30 19:05:04.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.334105 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-01-30 19:05:04.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-01-30 19:05:04.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.335912 django-content-blocks-1.1.3/content_blocks/static/content_blocks/iframeresizer/
--rw-rw-r--   0 quantra    (501) staff       (20)    34813 2021-04-26 11:15:23.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-rw-r--   0 quantra    (501) staff       (20)    37781 2021-04-26 11:15:23.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.336787 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 quantra    (501) staff       (20)    17094 2022-09-08 20:48:29.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 quantra    (501) staff       (20)    22564 2022-09-08 20:48:29.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.338027 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 quantra    (501) staff       (20)    30801 2022-09-08 20:48:29.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 quantra    (501) staff       (20)   255079 2022-09-08 20:48:29.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.340800 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/
--rw-r--r--   0 quantra    (501) staff       (20)     1892 2023-03-07 15:33:44.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 quantra    (501) staff       (20)     1065 2023-02-06 13:17:16.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 quantra    (501) staff       (20)    22492 2023-03-10 11:51:54.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 quantra    (501) staff       (20)     2213 2023-03-07 15:42:59.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 quantra    (501) staff       (20)     2303 2023-02-28 22:47:03.000000 django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.341729 django-content-blocks-1.1.3/content_blocks/templates/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.1.3/content_blocks/templates/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      136 2023-01-03 19:48:12.000000 django-content-blocks-1.1.3/content_blocks/templates/base.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.343502 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      307 2023-04-02 17:26:54.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 quantra    (501) staff       (20)      457 2023-03-03 16:05:10.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.345708 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 quantra    (501) staff       (20)     2042 2023-02-28 22:49:36.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 quantra    (501) staff       (20)     3012 2023-03-10 11:51:54.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 quantra    (501) staff       (20)     5232 2023-03-04 01:02:33.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 quantra    (501) staff       (20)      442 2023-02-25 02:17:35.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 quantra    (501) staff       (20)     5461 2023-02-28 23:38:02.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.347419 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 quantra    (501) staff       (20)      190 2023-02-23 13:56:34.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.348399 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 quantra    (501) staff       (20)      150 2023-02-23 13:56:28.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 quantra    (501) staff       (20)      516 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.351513 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 quantra    (501) staff       (20)      145 2023-02-23 13:56:16.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 quantra    (501) staff       (20)      477 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 quantra    (501) staff       (20)      299 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 quantra    (501) staff       (20)      412 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 quantra    (501) staff       (20)      545 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 quantra    (501) staff       (20)      566 2023-02-27 19:02:42.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 quantra    (501) staff       (20)      224 2023-02-23 13:56:43.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.353035 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 quantra    (501) staff       (20)      536 2023-02-23 13:54:11.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 quantra    (501) staff       (20)      605 2023-02-23 13:54:23.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 quantra    (501) staff       (20)      214 2023-02-24 02:12:55.000000 django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.355367 django-content-blocks-1.1.3/content_blocks/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.1.3/content_blocks/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.1.3/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     1126 2023-04-03 10:01:32.000000 django-content-blocks-1.1.3/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 quantra    (501) staff       (20)      699 2023-01-05 14:16:33.000000 django-content-blocks-1.1.3/content_blocks/urls.py
--rw-r--r--   0 quantra    (501) staff       (20)     9871 2023-04-04 12:41:48.000000 django-content-blocks-1.1.3/content_blocks/views.py
--rw-r--r--   0 quantra    (501) staff       (20)     1622 2023-02-24 14:43:18.000000 django-content-blocks-1.1.3/content_blocks/widgets.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-04 14:29:26.361008 django-content-blocks-1.1.3/django_content_blocks.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     3458 2023-04-04 14:29:26.000000 django-content-blocks-1.1.3/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     4184 2023-04-04 14:29:26.000000 django-content-blocks-1.1.3/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-04-04 14:29:26.000000 django-content-blocks-1.1.3/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       55 2023-04-04 14:29:26.000000 django-content-blocks-1.1.3/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       23 2023-04-04 14:29:26.000000 django-content-blocks-1.1.3/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 quantra    (501) staff       (20)       88 2023-03-02 00:40:47.000000 django-content-blocks-1.1.3/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-04-04 14:29:26.365387 django-content-blocks-1.1.3/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.1.3/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.257772 django-content-blocks-1.2.0/
+-rw-r--r--   0 quantra    (501) staff       (20)     1075 2023-03-16 15:50:21.000000 django-content-blocks-1.2.0/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)      146 2023-03-07 15:39:03.000000 django-content-blocks-1.2.0/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     3497 2023-04-14 13:30:05.257863 django-content-blocks-1.2.0/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     2001 2023-03-20 13:07:58.000000 django-content-blocks-1.2.0/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.153315 django-content-blocks-1.2.0/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.2.0/content_blocks/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3047 2023-03-01 13:20:40.000000 django-content-blocks-1.2.0/content_blocks/abstract_models.py
+-rw-r--r--   0 quantra    (501) staff       (20)    10457 2023-03-07 16:00:12.000000 django-content-blocks-1.2.0/content_blocks/admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     4008 2023-04-13 17:44:10.000000 django-content-blocks-1.2.0/content_blocks/admin_forms.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1601 2023-02-23 15:19:48.000000 django-content-blocks-1.2.0/content_blocks/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)      158 2023-01-05 16:14:15.000000 django-content-blocks-1.2.0/content_blocks/cache.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1654 2023-03-10 11:51:54.000000 django-content-blocks-1.2.0/content_blocks/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1686 2023-04-13 17:44:10.000000 django-content-blocks-1.2.0/content_blocks/fields.py
+-rw-r--r--   0 quantra    (501) staff       (20)     7501 2023-04-04 14:24:55.000000 django-content-blocks-1.2.0/content_blocks/forms.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.154590 django-content-blocks-1.2.0/content_blocks/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.2.0/content_blocks/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.156278 django-content-blocks-1.2.0/content_blocks/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.2.0/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      459 2023-02-27 23:55:14.000000 django-content-blocks-1.2.0/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 quantra    (501) staff       (20)      461 2023-02-27 23:57:07.000000 django-content-blocks-1.2.0/content_blocks/management/commands/update_content_blocks_cache.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.158108 django-content-blocks-1.2.0/content_blocks/migrations/
+-rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.2.0/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.2.0/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.2.0/content_blocks/migrations/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    22332 2023-04-14 12:49:12.000000 django-content-blocks-1.2.0/content_blocks/models.py
+-rw-r--r--   0 quantra    (501) staff       (20)      410 2023-02-28 12:22:17.000000 django-content-blocks-1.2.0/content_blocks/permissions.py
+-rw-r--r--   0 quantra    (501) staff       (20)     4874 2023-02-28 19:46:26.000000 django-content-blocks-1.2.0/content_blocks/signals.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.129799 django-content-blocks-1.2.0/content_blocks/static/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.160387 django-content-blocks-1.2.0/content_blocks/static/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.161709 django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      722 2023-02-17 13:42:24.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 quantra    (501) staff       (20)     9706 2023-04-14 13:22:29.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.164378 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 19:46:37.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.180228 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 18:56:30.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)    80823 2023-01-30 19:05:04.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      753 2023-03-04 01:20:32.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 quantra    (501) staff       (20)      572 2023-01-30 19:05:04.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.189738 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-01-30 19:05:04.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-01-30 19:05:04.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.202595 django-content-blocks-1.2.0/content_blocks/static/content_blocks/iframeresizer/
+-rw-rw-r--   0 quantra    (501) staff       (20)    34813 2021-04-26 11:15:23.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-rw-r--   0 quantra    (501) staff       (20)    37781 2021-04-26 11:15:23.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.203493 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 quantra    (501) staff       (20)    17094 2022-09-08 20:48:29.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 quantra    (501) staff       (20)    22564 2022-09-08 20:48:29.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.204356 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 quantra    (501) staff       (20)    30801 2022-09-08 20:48:29.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)   255079 2022-09-08 20:48:29.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.206927 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 quantra    (501) staff       (20)     1892 2023-03-07 15:33:44.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 quantra    (501) staff       (20)     1065 2023-02-06 13:17:16.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 quantra    (501) staff       (20)    22492 2023-03-10 11:51:54.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2213 2023-03-07 15:42:59.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2303 2023-02-28 22:47:03.000000 django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.213294 django-content-blocks-1.2.0/content_blocks/templates/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.2.0/content_blocks/templates/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      136 2023-01-03 19:48:12.000000 django-content-blocks-1.2.0/content_blocks/templates/base.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.217805 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      307 2023-04-02 17:26:54.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 quantra    (501) staff       (20)      457 2023-03-03 16:05:10.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.220283 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 quantra    (501) staff       (20)     2042 2023-02-28 22:49:36.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)     3012 2023-03-10 11:51:54.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)     5308 2023-04-14 13:22:41.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 quantra    (501) staff       (20)      442 2023-02-25 02:17:35.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 quantra    (501) staff       (20)     5461 2023-02-28 23:38:02.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.223365 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 quantra    (501) staff       (20)      190 2023-02-23 13:56:34.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.226421 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 quantra    (501) staff       (20)      150 2023-02-23 13:56:28.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)      516 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.241101 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 quantra    (501) staff       (20)      145 2023-02-23 13:56:16.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)      477 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      299 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 quantra    (501) staff       (20)      412 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      545 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 quantra    (501) staff       (20)      566 2023-02-27 19:02:42.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 quantra    (501) staff       (20)      224 2023-02-23 13:56:43.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.244733 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 quantra    (501) staff       (20)      536 2023-02-23 13:54:11.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 quantra    (501) staff       (20)      605 2023-02-23 13:54:23.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 quantra    (501) staff       (20)      214 2023-02-24 02:12:55.000000 django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.246258 django-content-blocks-1.2.0/content_blocks/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.2.0/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.2.0/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1351 2023-04-14 12:49:12.000000 django-content-blocks-1.2.0/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 quantra    (501) staff       (20)      699 2023-01-05 14:16:33.000000 django-content-blocks-1.2.0/content_blocks/urls.py
+-rw-r--r--   0 quantra    (501) staff       (20)     9667 2023-04-14 10:35:29.000000 django-content-blocks-1.2.0/content_blocks/views.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.2.0/content_blocks/widgets.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 13:30:05.257571 django-content-blocks-1.2.0/django_content_blocks.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     3497 2023-04-14 13:30:05.000000 django-content-blocks-1.2.0/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     4256 2023-04-14 13:30:05.000000 django-content-blocks-1.2.0/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-04-14 13:30:05.000000 django-content-blocks-1.2.0/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       55 2023-04-14 13:30:05.000000 django-content-blocks-1.2.0/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       23 2023-04-14 13:30:05.000000 django-content-blocks-1.2.0/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       88 2023-03-02 00:40:47.000000 django-content-blocks-1.2.0/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1945 2023-04-14 13:30:05.260417 django-content-blocks-1.2.0/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.2.0/setup.py
```

### Comparing `django-content-blocks-1.1.3/LICENSE` & `django-content-blocks-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/PKG-INFO` & `django-content-blocks-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.1.3
+Version: 1.2.0
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
 Keywords: django,django-content-blocks,django content blocks,django content,django dynamic content,django content manager,django cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-content-blocks-1.1.3/README.rst` & `django-content-blocks-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/abstract_models.py` & `django-content-blocks-1.2.0/content_blocks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/admin.py` & `django-content-blocks-1.2.0/content_blocks/admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/admin_forms.py` & `django-content-blocks-1.2.0/content_blocks/admin_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 
 from django import forms
 
-from content_blocks.fields import ChoicesWidget
 from content_blocks.models import (
     ContentBlock,
     ContentBlockField,
     ContentBlockFields,
     ContentBlockTemplate,
     ContentBlockTemplateField,
 )
-from content_blocks.widgets import TemplateFilenameAutocompleteWidget
+from content_blocks.widgets import ChoicesWidget, TemplateFilenameAutocompleteWidget
 
 REQUIRED_ERROR_MSG = "This field is required"
 
 
 class ContentBlockTemplateAdminForm(forms.ModelForm):
     class Meta:
         model = ContentBlockTemplate
```

### Comparing `django-content-blocks-1.1.3/content_blocks/apps.py` & `django-content-blocks-1.2.0/content_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/conf.py` & `django-content-blocks-1.2.0/content_blocks/conf.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/fields.py` & `django-content-blocks-1.2.0/content_blocks/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,17 +63,7 @@
     attr_class = FieldVideo
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validators.append(
             FileExtensionValidator(allowed_extensions=["mp4", "webm", "ogg"])
         )
-
-
-# todo move this to widgets.py
-class ChoicesWidget(forms.HiddenInput):
-    template_name = "content_blocks/widgets/choices.html"
-
-    @property
-    def is_hidden(self):
-        # Show the label in the admin change page.
-        return False
```

### Comparing `django-content-blocks-1.1.3/content_blocks/forms.py` & `django-content-blocks-1.2.0/content_blocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.2.0/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/models.py` & `django-content-blocks-1.2.0/content_blocks/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,40 +40,26 @@
     from django_cleanup.cleanup import cleanup_ignore
 else:
     # noop shim for when django_cleanup isn't installed
     def cleanup_ignore(cls):  # pragma: no cover (covered in settings specific tests)
         return cls
 
 
-class ContentBlockFields:
-    # todo replace this with models.TextChoices
+class ContentBlockFields(models.TextChoices):
     TEXT_FIELD = "TextField"
     CONTENT_FIELD = "ContentField"
     IMAGE_FIELD = "ImageField"
     NESTED_FIELD = "NestedField"
     CHECKBOX_FIELD = "CheckboxField"
     CHOICE_FIELD = "ChoiceField"
     MODEL_CHOICE_FIELD = "ModelChoiceField"
     FILE_FIELD = "FileField"
     VIDEO_FIELD = "VideoField"
     EMBEDDED_VIDEO_FIELD = "EmbeddedVideoField"
 
-    CHOICES = (
-        (TEXT_FIELD, "Text Field"),
-        (CONTENT_FIELD, "Content Field"),
-        (IMAGE_FIELD, "Image Field"),
-        (VIDEO_FIELD, "Video Field"),
-        (FILE_FIELD, "File Field"),
-        (EMBEDDED_VIDEO_FIELD, "Embedded Video Field"),
-        (NESTED_FIELD, "Nested Field"),
-        (MODEL_CHOICE_FIELD, "Model Choice Field"),
-        (CHOICE_FIELD, "Choice Field"),
-        (CHECKBOX_FIELD, "Checkbox Field"),
-    )
-
 
 class ContentBlockFieldManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().select_related("template_field")
 
 
 def get_storage(field_type):
@@ -121,16 +107,15 @@
         "content_blocks.ContentBlock",
         on_delete=models.CASCADE,
         related_name="content_block_fields",
     )
 
     # duplicate from template_field here because it can't be changed on template field and seems impossible to have
     # select_related working in the __init__
-    # todo fix the maxlength here 32 is more like it
-    field_type = models.CharField(max_length=256)
+    field_type = models.CharField(max_length=32)
 
     text = models.CharField(max_length=256, blank=True)
     content = models.TextField(blank=True)
     checkbox = models.BooleanField(blank=True, default=False)
     image = SVGAndImageField(
         upload_to="content-blocks/images", blank=True, storage=image_storage
     )
@@ -150,46 +135,68 @@
     model_choice = GenericForeignKey(
         "model_choice_content_type", "model_choice_object_id"
     )
 
     template_name = "content_blocks/partials/fields/default.html"
     preview_template_name = None
 
+    class Meta:
+        ordering = ["template_field__position"]
+
     def __init__(self, *args, **kwargs):
+        """
+        Polymorph to the appropriate subclass proxy model.
+        """
         super().__init__(*args, **kwargs)
 
-        # todo remove this try
-        try:
-            for _class in ContentBlockField.__subclasses__():
-                if self.field_type == _class.__name__:
-                    self.__class__ = _class
-                    break
-        except:  # pragma: no cover # noqa
-            logger.error("Polymorphism failed")  # pragma: no cover
+        for _class in ContentBlockField.__subclasses__():
+            if self.field_type == _class.__name__:
+                self.__class__ = _class
+                break
 
-    class Meta:
-        ordering = ["template_field__position"]
+    def __init_subclass__(subcls):
+        """
+        Wrap all subclass form_field.__get__ methods with form_field_wrapper
+        """
+        super.__init_subclass__()
+
+        new_property = property(
+            ContentBlockField.form_field_wrapper(subcls.form_field.__get__),
+            subcls.form_field.__set__,
+        )
+        setattr(
+            subcls,
+            "form_field",
+            new_property,
+        )
+
+    @staticmethod
+    def form_field_wrapper(form_field):
+        """
+        Wraps the form_field.__get__ method and adds common attributes to all fields.
+        :param form_field: the form_field.__get__ method we are wrapping
+        """
+
+        def wrapper(self):
+            field = form_field(self)
+            if field is not None:
+                field.cb_field = self
+
+            return field
+
+        return wrapper
 
     @property
     def form_field(self):
         """
         To be overridden. Will return a form.Field class if the field is to be shown on the form.
         This method should return _form_field() with the desired forms.Field.
         """
         raise NotImplementedError  # pragma: no cover
 
-    def _form_field(self, field):
-        """
-        Adds content_block_field attribute to field
-        :return:
-        """
-        # todo can this be replace with a decorator?
-        field.cb_field = self
-        return field
-
     @property
     def context_value(self):
         raise NotImplementedError  # pragma: no cover
 
     def save_value(self, value):
         raise NotImplementedError  # pragma: no cover
 
@@ -217,21 +224,19 @@
     def form_field(self):
         widget = (
             forms.Textarea
             if settings.CONTENT_BLOCKS_TEXTFIELD_TEXTAREA
             else forms.TextInput
         )
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.CharField(
-                initial=self.text,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=widget,
-            )
+        return forms.CharField(
+            initial=self.text,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=widget,
         )
 
 
 class ContentField(ContentBlockField):
     class Meta:
         proxy = True
 
@@ -245,21 +250,19 @@
         self.content = value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.CharField(
-                initial=self.content,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=forms.Textarea(),
-            )
+        return forms.CharField(
+            initial=self.content,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=forms.Textarea(),
         )
 
 
 class CheckboxField(ContentBlockField):
     template_name = "content_blocks/partials/fields/checkbox.html"
 
     class Meta:
@@ -273,20 +276,18 @@
         self.checkbox = value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.BooleanField(
-                initial=self.checkbox,
-                required=False,
-                help_text=self.template_field.help_text,
-            )
+        return forms.BooleanField(
+            initial=self.checkbox,
+            required=False,
+            help_text=self.template_field.help_text,
         )
 
 
 @cleanup_ignore
 class ImageField(ContentBlockField):
     preview_template_name = "content_blocks/partials/fields/previews/image.html"
 
@@ -301,21 +302,19 @@
         self.image = None if value is False else value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            SVGAndImageFieldFormField(
-                initial=self.image,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=FileWidget(),
-            )
+        return SVGAndImageFieldFormField(
+            initial=self.image,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=FileWidget(),
         )
 
 
 @cleanup_ignore
 class FileField(ContentBlockField):
     class Meta:
         proxy = True
@@ -328,21 +327,19 @@
         self.file = None if value is False else value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.FileField(
-                initial=self.file,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=FileWidget(),
-            )
+        return forms.FileField(
+            initial=self.file,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=FileWidget(),
         )
 
 
 @cleanup_ignore
 class VideoField(ContentBlockField):
     preview_template_name = "content_blocks/partials/fields/previews/video.html"
 
@@ -357,21 +354,19 @@
         self.video = None if value is False else value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.FileField(
-                initial=self.video,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=FileWidget(),
-            )
+        return forms.FileField(
+            initial=self.video,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=FileWidget(),
         )
 
 
 class EmbeddedVideoField(ContentBlockField):
     preview_template_name = (
         "content_blocks/partials/fields/previews/embedded_video.html"
     )
@@ -387,20 +382,18 @@
         self.embedded_video = value
         self.save()
         return value
 
     @property
     def form_field(self):
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.CharField(
-                initial=self.embedded_video,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-            )
+        return forms.CharField(
+            initial=self.embedded_video,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
         )
 
 
 class ChoiceField(ContentBlockField):
     class Meta:
         proxy = True
 
@@ -413,41 +406,37 @@
         self.save()
         return value
 
     @property
     def form_field(self):
         choices = [[None, "-" * 9]] + json.loads(self.template_field.choices)
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.CharField(
-                initial=self.choice,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-                widget=forms.Select(choices=choices),
-            )
+        return forms.CharField(
+            initial=self.choice,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
+            widget=forms.Select(choices=choices),
         )
 
 
 class ModelChoiceField(ContentBlockField):
     class Meta:
         proxy = True
 
     @property
     def form_field(self):
         # self.model_choice_content_type must be set or this will raise an error.
         model = self.model_choice_content_type.model_class()
         queryset = model.objects.all()
         # noinspection PyTypeChecker
-        return self._form_field(
-            forms.ModelChoiceField(
-                queryset,
-                initial=self.model_choice,
-                required=self.template_field.required,
-                help_text=self.template_field.help_text,
-            )
+        return forms.ModelChoiceField(
+            queryset,
+            initial=self.model_choice,
+            required=self.template_field.required,
+            help_text=self.template_field.help_text,
         )
 
     @property
     def context_value(self):
         return self.model_choice
 
     def save_value(self, value):
@@ -470,15 +459,15 @@
         return None
 
     @property
     def context_value(self):
         """
         :return: Nested content blocks which we can then call render or access context on.
         """
-        return self.content_blocks.visible()
+        return self.content_blocks.nested()
 
 
 class ContentBlockManager(VisibleManager):
     def get_queryset(self):
         return (
             super()
             .get_queryset()
@@ -498,14 +487,21 @@
         """
         Visible drafts only. Exclude those which haven't been saved via the editor yet (empties).
         Can be used in page previews.
         :return:
         """
         return super().visible().filter(draft=True, saved=True)
 
+    def nested(self):
+        """
+        Used in the context for NestedField objects. Visible but with unsaved excluded.
+        :return:
+        """
+        return super().visible().filter(draft=False, saved=True)
+
     def published(self):
         """
         All published including visible=False.
         Used by the publishing/reset mechanism.
         :return:
         """
         return self.get_queryset().filter(draft=False)
@@ -536,16 +532,15 @@
         ContentBlockField,
         on_delete=models.CASCADE,
         related_name="content_blocks",
         blank=True,
         null=True,
     )
 
-    # todo max_length=64
-    css_class = models.CharField(max_length=256, blank=True)
+    css_class = models.CharField(max_length=64, blank=True)
 
     draft = models.BooleanField(blank=True, default=False)
 
     saved = models.BooleanField(blank=True, default=False)
 
     context_name = "content_block"
     cache_prefix = "content_block"
@@ -589,34 +584,40 @@
         """
         Return dictionary of template context for this content block
         """
         context = {key: field.context_value for key, field in self.fields.items()}
         context["css_class"] = self.css_class
         return context
 
-    def render(self, request=None):
+    def render(self, context=None, request=None):
         """
         Render html for this block and cache
         """
         if not self.can_render:
             return ""
 
+        context = context or {}
+        request = request or context.get("request")
+
+        context[self.context_name] = self.context
+        context["request"] = request
+
         cache_enabled = (
             not self.content_block_template.no_cache
             and not settings.CONTENT_BLOCKS_DISABLE_CACHE
         )
 
         html = None
         if cache_enabled:
             html = cache.get(self.cache_key)
 
         if html is None:
             html = render_to_string(
                 self.template,
-                {self.context_name: self.context, "request": request},
+                context,
                 request=request,
             )
 
             if cache_enabled:
                 cache.set(self.cache_key, html)
 
         return html
@@ -688,34 +689,31 @@
 
     content_block_template = models.ForeignKey(
         ContentBlockTemplate,
         on_delete=models.CASCADE,
         related_name="content_block_template_fields",
     )
 
-    # todo max_length=32
-    field_type = models.CharField(max_length=256, choices=ContentBlockFields.CHOICES)
+    field_type = models.CharField(max_length=32, choices=ContentBlockFields.choices)
 
-    # todo max_length=64
     key = models.SlugField(
-        max_length=256,
+        max_length=64,
         validators=[
             RegexValidator(
                 "[a-z0-9_]+", "Lowercase letters, numbers and underscores only."
             )
         ],
         help_text="Must be unique to this content block template. Lowercase letters, numbers and underscores only.",
     )
 
     help_text = models.TextField(blank=True)
     required = models.BooleanField(blank=True, default=False)
 
-    # todo max_length=64
     css_class = models.CharField(
-        max_length=256,
+        max_length=64,
         blank=True,
         help_text="Set a custom CSS class for this field in the editor.",
     )
 
     # Only used if field_type == NestedField
     nested_templates = models.ManyToManyField(
         "content_blocks.ContentBlockTemplate",
```

### Comparing `django-content-blocks-1.1.3/content_blocks/signals.py` & `django-content-blocks-1.2.0/content_blocks/signals.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/content_block_template_admin.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/content_block_template_admin.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/css/content_blocks.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/css/content_blocks.css`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,37 @@
 	padding: 20px 0 0 0;
 }
 
 .root-wrapper-controls.controls {
 	padding-top:0;
 }
 
+@media (prefers-color-scheme: light) {
+	.wrapper-controls button {
+		color: var(--link-fg);
+	}
+}
+html[data-theme="light"] .wrapper-controls button {
+	color: var(--link-fg);
+}
+
+/*
+-------------------------------------
+NESTED TITLE
+-------------------------------------
+*/
+
+h4.nested-title {
+	/*float:left;*/
+	position: absolute;
+	bottom:0;
+	left:0;
+	padding-bottom:0;
+}
+
 /*
 -------------------------------------
 TITLE BAR
 -------------------------------------
 */
 
 .title-bar {
```

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.2.0/content_blocks/static/content_blocks/js/popup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/.DS_Store` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/base.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,19 @@
         </div>
 
         <div class="cb-form-wrapper" id="cb_form_wrapper_{{ content_block.id }}">
             {% include 'content_blocks/editor/content_block_form.html' %}
         </div>
 
         <div class="expander expander_{{ content_block.id }}">
-			{#	Nested fields #}
+            {#	Nested fields #}
             {% for field in content_block.nested_fields.values %}
                 <div class="controls wrapper-controls">
+                    <h4 class="nested-title">{{ field.key }}</h4>
+
                     <button tabindex="-1" class="collapse-all" data-target="#nested_blocks_{{ field.id }}">
                         <i class="fa-solid fa-light fa-chevrons-up"></i>
                     </button>
                     <button tabindex="-1" class="expand-all" data-target="#nested_blocks_{{ field.id }}">
                         <i class="fa-solid fa-light fa-chevrons-down"></i>
                     </button>
                 </div>
```

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/fields/default.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/fields/default.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/loader.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/loader.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/partials/popup.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/partials/popup.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/choices.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/choices.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.2.0/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.2.0/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.2.0/content_blocks/templatetags/content_blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,9 +32,19 @@
 def render_content_block(context, content_block):
     """
     Allows rendering of content blocks with request context.  Content blocks should have no_cache=True in this case.
     :param context:
     :param content_block:
     :return:
     """
-    # todo test, docs
-    return content_block.render(request=context.get("request"))
+
+    # Because our context might have RequestContext already in it flatten ourselves
+    context_dict = {}
+    for d in context.dicts:
+        try:
+            d = d.flatten()
+        except AttributeError:
+            pass
+
+        context_dict.update(d)
+
+    return content_block.render(context=context_dict)
```

### Comparing `django-content-blocks-1.1.3/content_blocks/urls.py` & `django-content-blocks-1.2.0/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.1.3/content_blocks/views.py` & `django-content-blocks-1.2.0/content_blocks/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,14 @@
     }
 
     params.update(kwargs)
 
     LogEntry.objects.log_action(**params)
 
 
-def render_with_admin_context(request, template, context, model_admin):
-    context.update(**model_admin.admin_site.each_context(request))
-    return render(request, template, context)
-
-
 @staff_member_required
 @ensure_csrf_cookie
 def content_block_editor(request, object_id, model_admin=None):
     """
     Show the content block editor.
     """
     parent = get_object_or_404(model_admin.model, id=object_id)
@@ -71,29 +66,27 @@
     )
     import_content_blocks_form = ImportContentBlocksForm(parent=parent)
 
     status_message = settings.CONTENT_BLOCKS_DEFAULT_STATUS_MESSAGE
     if callable(status_message):
         status_message = status_message()
 
-    return render_with_admin_context(
-        request,
-        "content_blocks/editor/editor.html",
-        {
-            "import_content_blocks_form": import_content_blocks_form,
-            "new_content_block_form": new_content_block_form,
-            "parent": parent,
-            "publish_form": publish_form,
-            "discard_form": discard_changes_form,
-            "return_url": return_url,
-            "opts": parent._meta,
-            "status_message": status_message,
-        },
-        model_admin,
-    )
+    context = {
+        "import_content_blocks_form": import_content_blocks_form,
+        "new_content_block_form": new_content_block_form,
+        "parent": parent,
+        "publish_form": publish_form,
+        "discard_form": discard_changes_form,
+        "return_url": return_url,
+        "opts": parent._meta,
+        "status_message": status_message,
+    }
+    context.update(**model_admin.admin_site.each_context(request))
+
+    return render(request, "content_blocks/editor/editor.html", context)
 
 
 def content_block_create_base(request, form, parent, log_name="content block"):
     """
     Ajax view for creating new top level and nested content blocks depending on the form passed.
     Returns html form for the new content block.
     """
```

### Comparing `django-content-blocks-1.1.3/content_blocks/widgets.py` & `django-content-blocks-1.2.0/content_blocks/widgets.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,7 +47,16 @@
         return f"{slugify(self.template_dir)}__suggestions"
 
     def get_context(self, *args):
         context = super().get_context(*args)
         context["widget"]["data_list_id"] = self.data_list_id
         context["widget"]["template_list"] = self.template_list
         return context
+
+
+class ChoicesWidget(forms.HiddenInput):
+    template_name = "content_blocks/widgets/choices.html"
+
+    @property
+    def is_hidden(self):
+        # Show the label in the admin change page.
+        return False
```

### Comparing `django-content-blocks-1.1.3/django_content_blocks.egg-info/PKG-INFO` & `django-content-blocks-1.2.0/django_content_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.1.3
+Version: 1.2.0
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
 Keywords: django,django-content-blocks,django content blocks,django content,django dynamic content,django content manager,django cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-content-blocks-1.1.3/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.2.0/django_content_blocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 content_blocks/views.py
 content_blocks/widgets.py
 content_blocks/management/__init__.py
 content_blocks/management/commands/__init__.py
 content_blocks/management/commands/clear_content_blocks_cache.py
 content_blocks/management/commands/update_content_blocks_cache.py
 content_blocks/migrations/0001_initial.py
+content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
 content_blocks/migrations/__init__.py
 content_blocks/static/content_blocks/.DS_Store
 content_blocks/static/content_blocks/css/.DS_Store
 content_blocks/static/content_blocks/css/content_block_template_admin.css
 content_blocks/static/content_blocks/css/content_blocks.css
 content_blocks/static/content_blocks/fontawesome/.DS_Store
 content_blocks/static/content_blocks/fontawesome/css/.DS_Store
```

### Comparing `django-content-blocks-1.1.3/setup.cfg` & `django-content-blocks-1.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [metadata]
 name = django-content-blocks
-version = 1.1.3
+version = 1.2.0
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
```

