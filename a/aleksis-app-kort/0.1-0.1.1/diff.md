# Comparing `tmp/aleksis_app_kort-0.1.tar.gz` & `tmp/aleksis_app_kort-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_kort-0.1.tar", max compression
+gzip compressed data, was "aleksis_app_kort-0.1.1.tar", max compression
```

## Comparing `aleksis_app_kort-0.1.tar` & `aleksis_app_kort-0.1.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      436 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/LICENCE.rst
--rw-r--r--   0        0        0      888 2022-12-04 11:35:00.665707 aleksis_app_kort-0.1/README.rst
--rw-r--r--   0        0        0      150 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/aleksis/apps/kort/__init__.py
--rw-r--r--   0        0        0      193 2022-03-10 18:37:05.158053 aleksis_app_kort-0.1/aleksis/apps/kort/admin.py
--rw-r--r--   0        0        0     7107 2022-12-04 12:04:32.510414 aleksis_app_kort-0.1/aleksis/apps/kort/api.py
--rw-r--r--   0        0        0     1449 2022-12-04 12:00:14.657517 aleksis_app_kort-0.1/aleksis/apps/kort/apps.py
--rw-r--r--   0        0        0     5311 2022-08-14 13:54:09.409675 aleksis_app_kort-0.1/aleksis/apps/kort/forms.py
--rw-r--r--   0        0        0     5713 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1/aleksis/apps/kort/frontend/index.js
--rw-r--r--   0        0        0      231 2023-03-19 14:58:24.454538 aleksis_app_kort-0.1/aleksis/apps/kort/frontend/messages/de.json
--rw-r--r--   0        0        0      228 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1/aleksis/apps/kort/frontend/messages/en.json
--rw-r--r--   0        0        0        3 2023-03-19 14:58:24.458538 aleksis_app_kort-0.1/aleksis/apps/kort/frontend/messages/ru.json
--rw-r--r--   0        0        0        3 2023-03-19 14:58:24.458538 aleksis_app_kort-0.1/aleksis/apps/kort/frontend/messages/uk.json
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/aleksis/apps/kort/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18993 2023-03-19 14:48:32.328267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13124 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24175 2023-03-19 14:48:32.316267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18909 2023-03-19 14:48:32.252267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.236267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.296267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19053 2023-03-19 14:48:32.212267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.276267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19140 2023-03-19 14:48:32.240267 aleksis_app_kort-0.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1459 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0001_initial.py
--rw-r--r--   0        0        0     2334 2021-11-30 20:07:19.626067 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0002_card_printer.py
--rw-r--r--   0        0        0     1544 2022-03-08 19:23:37.637527 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py
--rw-r--r--   0        0        0      428 2022-03-08 19:32:45.096219 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0004_alter_card_chip_number.py
--rw-r--r--   0        0        0      538 2022-03-10 16:48:40.401048 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0005_card_pdf_file.py
--rw-r--r--   0        0        0     1218 2022-03-10 19:03:08.179322 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py
--rw-r--r--   0        0        0     2418 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py
--rw-r--r--   0        0        0     1052 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py
--rw-r--r--   0        0        0      455 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0009_cardprinter_generate_number_on_server.py
--rw-r--r--   0        0        0      778 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py
--rw-r--r--   0        0        0      437 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0011_cardprinter_card_detector.py
--rw-r--r--   0        0        0     2071 2022-07-29 13:47:52.820053 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py
--rw-r--r--   0        0        0      906 2022-07-29 13:47:52.820053 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py
--rw-r--r--   0        0        0      754 2022-08-02 22:25:04.075075 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py
--rw-r--r--   0        0        0      575 2022-12-04 11:45:56.812937 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0015_migrate_scopes.py
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/aleksis/apps/kort/migrations/__init__.py
--rw-r--r--   0        0        0    11630 2022-12-04 12:00:14.781516 aleksis_app_kort-0.1/aleksis/apps/kort/models.py
--rw-r--r--   0        0        0     3515 2022-08-29 10:20:09.797130 aleksis_app_kort-0.1/aleksis/apps/kort/rules.py
--rw-r--r--   0        0        0       32 2022-09-04 10:38:46.745643 aleksis_app_kort-0.1/aleksis/apps/kort/settings.py
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1/aleksis/apps/kort/static/.keepdir
--rw-r--r--   0        0        0     5184 2022-08-04 09:05:10.177572 aleksis_app_kort-0.1/aleksis/apps/kort/tables.py
--rw-r--r--   0        0        0      634 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/tasks.py
--rw-r--r--   0        0        0     2126 2022-08-10 14:27:45.460767 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/actions.html
--rw-r--r--   0        0        0     1345 2022-03-12 21:12:55.899447 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/delete.html
--rw-r--r--   0        0        0      399 2023-01-27 18:23:26.937618 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/detail.html
--rw-r--r--   0        0        0     2307 2022-08-10 14:26:18.376009 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/detail_content.html
--rw-r--r--   0        0        0      641 2022-03-08 19:29:07.431134 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/edit.html
--rw-r--r--   0        0        0     3295 2022-08-04 09:04:47.167728 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/issue.html
--rw-r--r--   0        0        0     1177 2023-01-27 18:23:26.937618 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/list.html
--rw-r--r--   0        0        0      787 2022-08-10 14:27:45.448768 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/print_form.html
--rw-r--r--   0        0        0      292 2022-03-10 16:04:46.741747 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/short.html
--rw-r--r--   0        0        0      203 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/status.html
--rw-r--r--   0        0        0     1344 2022-08-10 14:27:45.472767 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/actions.html
--rw-r--r--   0        0        0      896 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/create.html
--rw-r--r--   0        0        0     1273 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/delete.html
--rw-r--r--   0        0        0     1291 2022-08-10 14:27:45.488766 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/detail.html
--rw-r--r--   0        0        0     1851 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/detail_content.html
--rw-r--r--   0        0        0      892 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/edit.html
--rw-r--r--   0        0        0     1276 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/instructions.html
--rw-r--r--   0        0        0      699 2022-08-10 14:27:45.456767 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/list.html
--rw-r--r--   0        0        0      115 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/short.html
--rw-r--r--   0        0        0      470 2022-08-03 17:35:59.880270 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/person_status.html
--rw-r--r--   0        0        0      385 2022-08-03 17:25:48.418519 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/picture.html
--rw-r--r--   0        0        0     1312 2022-08-10 14:27:45.480766 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/actions.html
--rw-r--r--   0        0        0      645 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/create.html
--rw-r--r--   0        0        0     1303 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/delete.html
--rw-r--r--   0        0        0     1292 2022-08-10 14:27:45.476766 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/detail.html
--rw-r--r--   0        0        0     3776 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/detail_content.html
--rw-r--r--   0        0        0      657 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/edit.html
--rw-r--r--   0        0        0      706 2022-08-10 14:27:45.468767 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/list.html
--rw-r--r--   0        0        0      317 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/short.html
--rw-r--r--   0        0        0      228 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/status.html
--rw-r--r--   0        0        0     1232 2022-07-29 13:47:52.828052 aleksis_app_kort-0.1/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html
--rw-r--r--   0        0        0      760 2022-03-11 22:36:47.959342 aleksis_app_kort-0.1/aleksis/apps/kort/templatetags/barcode.py
--rw-r--r--   0        0        0     2537 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1/aleksis/apps/kort/urls.py
--rw-r--r--   0        0        0    14858 2022-08-12 16:41:36.393225 aleksis_app_kort-0.1/aleksis/apps/kort/views.py
--rw-r--r--   0        0        0     1363 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1/pyproject.toml
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 aleksis_app_kort-0.1/setup.py
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 aleksis_app_kort-0.1/PKG-INFO
+-rw-r--r--   0        0        0      641 2023-03-20 16:04:20.798483 aleksis_app_kort-0.1.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/LICENCE.rst
+-rw-r--r--   0        0        0      888 2022-12-04 11:35:00.665707 aleksis_app_kort-0.1.1/README.rst
+-rw-r--r--   0        0        0      150 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/aleksis/apps/kort/__init__.py
+-rw-r--r--   0        0        0      193 2022-03-10 18:37:05.158053 aleksis_app_kort-0.1.1/aleksis/apps/kort/admin.py
+-rw-r--r--   0        0        0     7107 2022-12-04 12:04:32.510414 aleksis_app_kort-0.1.1/aleksis/apps/kort/api.py
+-rw-r--r--   0        0        0     1449 2022-12-04 12:00:14.657517 aleksis_app_kort-0.1.1/aleksis/apps/kort/apps.py
+-rw-r--r--   0        0        0     5311 2022-08-14 13:54:09.409675 aleksis_app_kort-0.1.1/aleksis/apps/kort/forms.py
+-rw-r--r--   0        0        0     5751 2023-03-20 15:59:14.764294 aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/index.js
+-rw-r--r--   0        0        0      231 2023-03-19 14:58:24.454538 aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/messages/de.json
+-rw-r--r--   0        0        0      228 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/messages/en.json
+-rw-r--r--   0        0        0        3 2023-03-19 14:58:24.458538 aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/messages/ru.json
+-rw-r--r--   0        0        0      295 2023-04-14 09:25:50.833116 aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/messages/uk.json
+-rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18993 2023-03-19 14:48:32.328267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13124 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24175 2023-03-19 14:48:32.316267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18909 2023-03-19 14:48:32.252267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.236267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.296267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19053 2023-03-19 14:48:32.212267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.276267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2023-03-19 20:34:24.465191 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19140 2023-03-19 14:48:32.240267 aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1459 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2334 2021-11-30 20:07:19.626067 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0002_card_printer.py
+-rw-r--r--   0        0        0     1544 2022-03-08 19:23:37.637527 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py
+-rw-r--r--   0        0        0      428 2022-03-08 19:32:45.096219 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0004_alter_card_chip_number.py
+-rw-r--r--   0        0        0      538 2022-03-10 16:48:40.401048 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0005_card_pdf_file.py
+-rw-r--r--   0        0        0     1218 2022-03-10 19:03:08.179322 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py
+-rw-r--r--   0        0        0     2418 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py
+-rw-r--r--   0        0        0     1052 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py
+-rw-r--r--   0        0        0      455 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0009_cardprinter_generate_number_on_server.py
+-rw-r--r--   0        0        0      778 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py
+-rw-r--r--   0        0        0      437 2022-05-29 10:47:02.293945 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0011_cardprinter_card_detector.py
+-rw-r--r--   0        0        0     2071 2022-07-29 13:47:52.820053 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py
+-rw-r--r--   0        0        0      906 2022-07-29 13:47:52.820053 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py
+-rw-r--r--   0        0        0      754 2022-08-02 22:25:04.075075 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py
+-rw-r--r--   0        0        0      575 2022-12-04 11:45:56.812937 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0015_migrate_scopes.py
+-rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/__init__.py
+-rw-r--r--   0        0        0    11630 2022-12-04 12:00:14.781516 aleksis_app_kort-0.1.1/aleksis/apps/kort/models.py
+-rw-r--r--   0        0        0     3515 2022-08-29 10:20:09.797130 aleksis_app_kort-0.1.1/aleksis/apps/kort/rules.py
+-rw-r--r--   0        0        0       32 2022-09-04 10:38:46.745643 aleksis_app_kort-0.1.1/aleksis/apps/kort/settings.py
+-rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.1.1/aleksis/apps/kort/static/.keepdir
+-rw-r--r--   0        0        0     5184 2022-08-04 09:05:10.177572 aleksis_app_kort-0.1.1/aleksis/apps/kort/tables.py
+-rw-r--r--   0        0        0      634 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/tasks.py
+-rw-r--r--   0        0        0     2126 2022-08-10 14:27:45.460767 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/actions.html
+-rw-r--r--   0        0        0     1345 2022-03-12 21:12:55.899447 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/delete.html
+-rw-r--r--   0        0        0      399 2023-01-27 18:23:26.937618 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/detail.html
+-rw-r--r--   0        0        0     2307 2022-08-10 14:26:18.376009 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/detail_content.html
+-rw-r--r--   0        0        0      641 2022-03-08 19:29:07.431134 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/edit.html
+-rw-r--r--   0        0        0     3295 2022-08-04 09:04:47.167728 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/issue.html
+-rw-r--r--   0        0        0     1177 2023-01-27 18:23:26.937618 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/list.html
+-rw-r--r--   0        0        0      787 2022-08-10 14:27:45.448768 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/print_form.html
+-rw-r--r--   0        0        0      292 2022-03-10 16:04:46.741747 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/short.html
+-rw-r--r--   0        0        0      203 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/status.html
+-rw-r--r--   0        0        0     1344 2022-08-10 14:27:45.472767 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/actions.html
+-rw-r--r--   0        0        0      896 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/create.html
+-rw-r--r--   0        0        0     1273 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/delete.html
+-rw-r--r--   0        0        0     1291 2022-08-10 14:27:45.488766 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/detail.html
+-rw-r--r--   0        0        0     1851 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/detail_content.html
+-rw-r--r--   0        0        0      892 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/edit.html
+-rw-r--r--   0        0        0     1276 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/instructions.html
+-rw-r--r--   0        0        0      699 2022-08-10 14:27:45.456767 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/list.html
+-rw-r--r--   0        0        0      115 2022-07-29 13:47:52.824052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/short.html
+-rw-r--r--   0        0        0      470 2022-08-03 17:35:59.880270 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/person_status.html
+-rw-r--r--   0        0        0      385 2022-08-03 17:25:48.418519 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/picture.html
+-rw-r--r--   0        0        0     1312 2022-08-10 14:27:45.480766 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/actions.html
+-rw-r--r--   0        0        0      645 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/create.html
+-rw-r--r--   0        0        0     1303 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/delete.html
+-rw-r--r--   0        0        0     1292 2022-08-10 14:27:45.476766 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/detail.html
+-rw-r--r--   0        0        0     3776 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/detail_content.html
+-rw-r--r--   0        0        0      657 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/edit.html
+-rw-r--r--   0        0        0      706 2022-08-10 14:27:45.468767 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/list.html
+-rw-r--r--   0        0        0      317 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/short.html
+-rw-r--r--   0        0        0      228 2022-05-29 10:47:02.297945 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/status.html
+-rw-r--r--   0        0        0     1232 2022-07-29 13:47:52.828052 aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html
+-rw-r--r--   0        0        0      760 2022-03-11 22:36:47.959342 aleksis_app_kort-0.1.1/aleksis/apps/kort/templatetags/barcode.py
+-rw-r--r--   0        0        0     2537 2023-03-19 14:47:27.272460 aleksis_app_kort-0.1.1/aleksis/apps/kort/urls.py
+-rw-r--r--   0        0        0    14858 2022-08-12 16:41:36.393225 aleksis_app_kort-0.1.1/aleksis/apps/kort/views.py
+-rw-r--r--   0        0        0     1365 2023-03-20 16:03:36.646693 aleksis_app_kort-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 aleksis_app_kort-0.1.1/setup.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 aleksis_app_kort-0.1.1/PKG-INFO
```

### Comparing `aleksis_app_kort-0.1/LICENCE.rst` & `aleksis_app_kort-0.1.1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/README.rst` & `aleksis_app_kort-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/api.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/api.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/apps.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/forms.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/frontend/index.js` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/frontend/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 export default {
     meta: {
         inMenu: true,
         titleKey: "kort.menu_title",
         icon: "mdi-card-account-details-outline",
+        permission: "kort.view_menu_rule",
     },
     children: [{
         path: "cards/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "kort.cards",
         meta: {
             inMenu: true,
             titleKey: "kort.card.menu_title",
             icon: "mdi-card-multiple-outline",
             permission: "kort.view_cards_rule",
         },
-
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "cards/create/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "kort.createCard",
```

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0001_initial.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0002_card_printer.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0002_card_printer.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0005_card_pdf_file.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0005_card_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/migrations/0015_migrate_scopes.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/migrations/0015_migrate_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/models.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/rules.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/tables.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/tasks.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/actions.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/delete.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/detail_content.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/edit.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/issue.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/issue.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/list.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card/print_form.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card/print_form.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/actions.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/create.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/delete.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/detail.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/detail_content.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/edit.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/instructions.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/instructions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/card_layout/list.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/card_layout/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/actions.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/create.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/delete.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/detail.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/detail_content.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/edit.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/kort/printer/list.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/kort/printer/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/templatetags/barcode.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/templatetags/barcode.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/urls.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/aleksis/apps/kort/views.py` & `aleksis_app_kort-0.1.1/aleksis/apps/kort/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.1/pyproject.toml` & `aleksis_app_kort-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Kort"
-version = "0.1"
+version = "0.1.1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Kort (manage student IDs)"
```

### Comparing `aleksis_app_kort-0.1/setup.py` & `aleksis_app_kort-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'python-barcode>=0.14.0,<0.15.0']
 
 entry_points = \
 {'aleksis.app': ['kort = aleksis.apps.kort.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-kort',
-    'version': '0.1',
+    'version': '0.1.1',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Kort (manage student IDs)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Kort (manage student IDs)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2021 Margarete Grassl <grasslma@katharineum.de>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n',
     'author': 'Margarete Grassl',
     'author_email': 'grasslma@katharineum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_kort-0.1/PKG-INFO` & `aleksis_app_kort-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-kort
-Version: 0.1
+Version: 0.1.1
 Summary: AlekSIS (School Information System) — App Kort (manage student IDs)
 Home-page: https://aleksis.org
 License: EUPL-1.2
 Author: Margarete Grassl
 Author-email: grasslma@katharineum.de
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

