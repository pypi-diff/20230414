# Comparing `tmp/wc-django-notifications-0.1.2.tar.gz` & `tmp/wc-django-notifications-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-notifications-0.1.2.tar", last modified: Wed Oct  5 10:20:58 2022, max compression
+gzip compressed data, was "wc-django-notifications-0.1.3.tar", last modified: Fri Apr 14 09:03:50 2023, max compression
```

## Comparing `wc-django-notifications-0.1.2.tar` & `wc-django-notifications-0.1.3.tar`

### file list

```diff
@@ -1,385 +1,386 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.804104 wc-django-notifications-0.1.2/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      297 2022-10-05 10:15:49.000000 wc-django-notifications-0.1.2/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-09-28 09:10:10.000000 wc-django-notifications-0.1.2/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-10-05 10:04:05.000000 wc-django-notifications-0.1.2/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-10-05 10:04:34.000000 wc-django-notifications-0.1.2/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9530 2022-10-05 10:20:58.804104 wc-django-notifications-0.1.2/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     8593 2022-10-05 10:02:16.000000 wc-django-notifications-0.1.2/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2022-10-05 10:20:58.804104 wc-django-notifications-0.1.2/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1842 2022-10-04 14:33:21.000000 wc-django-notifications-0.1.2/setup.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-10-03 15:15:47.000000 wc-django-notifications-0.1.2/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9530 2022-10-05 10:20:58.000000 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9612 2022-10-05 10:20:58.000000 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2022-10-05 10:20:58.000000 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      288 2022-10-05 10:20:58.000000 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2022-10-05 10:20:58.000000 wc-django-notifications-0.1.2/wc_django_notifications.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2022-10-05 10:20:54.000000 wc-django-notifications-0.1.2/wcd_notifications/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1141 2022-10-05 10:19:30.000000 wc-django-notifications-0.1.2/wcd_notifications/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-10-04 10:41:02.000000 wc-django-notifications-0.1.2/wcd_notifications/apps.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2022-10-05 08:30:05.000000 wc-django-notifications-0.1.2/wcd_notifications/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-09-29 11:02:58.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-10-05 10:14:22.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-10-05 10:15:11.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7064 2022-10-05 06:55:03.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/filters.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5209 2022-10-05 09:05:01.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4250 2022-10-05 08:26:24.000000 wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/views.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-09-28 11:52:34.000000 wc-django-notifications-0.1.2/wcd_notifications/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.772104 wc-django-notifications-0.1.2/wcd_notifications/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.772104 wc-django-notifications-0.1.2/wcd_notifications/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3446 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.772104 wc-django-notifications-0.1.2/wcd_notifications/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ast/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.772104 wc-django-notifications-0.1.2/wcd_notifications/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/az/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/az/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.772104 wc-django-notifications-0.1.2/wcd_notifications/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/be/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3504 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/be/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/br/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3663 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/br/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3443 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3408 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.788104 wc-django-notifications-0.1.2/wcd_notifications/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3401 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3424 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/gl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3435 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ia/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ig/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/io/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/io/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/is/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3382 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/is/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.776104 wc-django-notifications-0.1.2/wcd_notifications/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.792104 wc-django-notifications-0.1.2/wcd_notifications/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3497 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3398 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3390 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3314 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/pl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3512 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.796104 wc-django-notifications-0.1.2/wcd_notifications/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3404 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ru/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3504 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3438 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/uk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3591 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.780104 wc-django-notifications-0.1.2/wcd_notifications/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.784104 wc-django-notifications-0.1.2/wcd_notifications/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-10-05 10:03:15.000000 wc-django-notifications-0.1.2/wcd_notifications/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.800104 wc-django-notifications-0.1.2/wcd_notifications/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5496 2022-10-03 12:56:24.000000 wc-django-notifications-0.1.2/wcd_notifications/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-09-29 10:39:29.000000 wc-django-notifications-0.1.2/wcd_notifications/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.804104 wc-django-notifications-0.1.2/wcd_notifications/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-10-03 12:07:52.000000 wc-django-notifications-0.1.2/wcd_notifications/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9289 2022-10-05 10:01:34.000000 wc-django-notifications-0.1.2/wcd_notifications/models/notifications.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1785 2022-10-04 10:21:13.000000 wc-django-notifications-0.1.2/wcd_notifications/models/stats.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-10-05 10:20:58.804104 wc-django-notifications-0.1.2/wcd_notifications/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-28 09:10:10.000000 wc-django-notifications-0.1.2/wcd_notifications/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4371 2022-10-05 09:45:37.000000 wc-django-notifications-0.1.2/wcd_notifications/services/manager.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2113 2022-10-05 10:02:50.000000 wc-django-notifications-0.1.2/wcd_notifications/services/notifier.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      231 2022-10-05 08:25:03.000000 wc-django-notifications-0.1.2/wcd_notifications/signals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      453 2022-10-05 09:09:31.000000 wc-django-notifications-0.1.2/wcd_notifications/subscriptions.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3927 2022-10-04 09:11:57.000000 wc-django-notifications-0.1.2/wcd_notifications/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      347 2023-04-14 09:03:30.000000 wc-django-notifications-0.1.3/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9580 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     8593 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1842 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/setup.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9580 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9640 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      288 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-04-14 09:02:22.000000 wc-django-notifications-0.1.3/wcd_notifications/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1141 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.1.3/wcd_notifications/compat.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7064 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/filters.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5209 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/serializers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4250 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/views.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3446 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3504 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3663 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3443 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3408 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4397 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3401 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3424 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3435 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3382 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3497 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3398 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3390 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3314 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3512 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3404 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4541 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3438 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4628 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.1.3/wcd_notifications/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9322 2023-04-14 08:13:46.000000 wc-django-notifications-0.1.3/wcd_notifications/models/notifications.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1801 2023-04-14 08:43:15.000000 wc-django-notifications-0.1.3/wcd_notifications/models/stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4371 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/manager.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2113 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/notifier.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      231 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/signals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      453 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/subscriptions.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3927 2023-04-14 08:34:36.000000 wc-django-notifications-0.1.3/wcd_notifications/utils.py
```

### Comparing `wc-django-notifications-0.1.2/LICENSE` & `wc-django-notifications-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/Makefile` & `wc-django-notifications-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/PKG-INFO` & `wc-django-notifications-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -299,11 +299,15 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.3]
+### Fixed
+- Django 2.2 compatibility.
+
 ## [0.1.1]
 Initial version.
```

### Comparing `wc-django-notifications-0.1.2/README.md` & `wc-django-notifications-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/setup.py` & `wc-django-notifications-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/tox.ini` & `wc-django-notifications-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wc_django_notifications.egg-info/PKG-INFO` & `wc-django-notifications-0.1.3/wc_django_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -299,11 +299,15 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.3]
+### Fixed
+- Django 2.2 compatibility.
+
 ## [0.1.1]
 Initial version.
```

### Comparing `wc-django-notifications-0.1.2/wc_django_notifications.egg-info/SOURCES.txt` & `wc-django-notifications-0.1.3/wc_django_notifications.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 wc_django_notifications.egg-info/SOURCES.txt
 wc_django_notifications.egg-info/dependency_links.txt
 wc_django_notifications.egg-info/requires.txt
 wc_django_notifications.egg-info/top_level.txt
 wcd_notifications/__init__.py
 wcd_notifications/admin.py
 wcd_notifications/apps.py
+wcd_notifications/compat.py
 wcd_notifications/conf.py
 wcd_notifications/exceptions.py
 wcd_notifications/signals.py
 wcd_notifications/subscriptions.py
 wcd_notifications/utils.py
 wcd_notifications/contrib/__init__.py
 wcd_notifications/contrib/drf/__init__.py
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/admin.py` & `wc-django-notifications-0.1.3/wcd_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/conf.py` & `wc-django-notifications-0.1.3/wcd_notifications/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/filters.py` & `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/filters.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/serializers.py` & `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/contrib/drf/views.py` & `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/views.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/af/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ar/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ast/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/az/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/be/LC_MESSAGES/django.mo` & `wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/be/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/bg/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/bn/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/br/LC_MESSAGES/django.mo` & `wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/br/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/bs/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ca/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/cs/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/cy/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/da/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/de/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/dsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/el/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/en/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/eo/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/es/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/et/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/eu/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/fa/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/fi/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/fr/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/fy/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ga/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/gd/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/gl/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/he/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/hi/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/hr/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/hsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/hu/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/hy/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ia/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/id/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ig/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/io/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/is/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/it/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ja/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ka/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/kab/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/kk/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/km/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/kn/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ko/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ky/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/lb/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/lt/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/lv/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/mk/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ml/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/mn/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/mr/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ms/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/my/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/nb/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ne/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/nl/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/nn/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/os/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/pa/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/pl/LC_MESSAGES/django.mo` & `wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/pl/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/pt/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ro/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ru/LC_MESSAGES/django.mo` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ru/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
+"%100==4 ? 2 : 3);\n"
 #: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sk/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sl/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 #: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sq/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sr/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sv/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/sw/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ta/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/te/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/tg/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/th/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/tk/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/tr/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/tt/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/udm/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/uk/LC_MESSAGES/django.mo` & `wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/uk/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 #: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/ur/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -4,135 +4,144 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-02-10 15:02+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
+"%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: packages/wc-django-notifications/wcd_notifications/apps.py:10
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
-#: wcd_notifications/contrib/drf/filters.py:81
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
-#: wcd_notifications/contrib/drf/filters.py:82
-#: wcd_notifications/contrib/drf/filters.py:116
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:82
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:116
 msgctxt "wcd_notifications"
 msgid "No such content type exists."
 msgstr ""
 
-#: wcd_notifications/contrib/drf/serializers.py:120
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:35
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:115
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:131
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:137
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:34
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:141
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:38
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:148
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:152
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:159
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:163
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:170
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:174
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:181
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:185
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:190
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:23
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:25
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:43
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:47
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/locale/uz/LC_MESSAGES/django.po` & `wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.po`

 * *Files 27% similar despite different names*

```diff
@@ -4,135 +4,145 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-02-10 15:02+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+
+#: packages/wc-django-notifications/wcd_notifications/apps.py:10
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
-#: wcd_notifications/contrib/drf/filters.py:81
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
-#: wcd_notifications/contrib/drf/filters.py:82
-#: wcd_notifications/contrib/drf/filters.py:116
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:82
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:116
 msgctxt "wcd_notifications"
 msgid "No such content type exists."
 msgstr ""
 
-#: wcd_notifications/contrib/drf/serializers.py:120
+#: packages/wc-django-notifications/wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:35
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:115
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:131
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:137
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:34
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:141
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:38
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:148
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:152
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:159
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:163
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:170
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:174
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:181
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:185
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:190
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:23
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:25
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:43
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: packages/wc-django-notifications/wcd_notifications/models/stats.py:47
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/migrations/0001_initial.py` & `wc-django-notifications-0.1.3/wcd_notifications/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import django.contrib.postgres.fields
 import django.contrib.postgres.indexes
 import django.contrib.postgres.operations
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 
+from wcd_notifications.compat import JSONField
+
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         ('contenttypes', '0002_remove_content_type_name'),
@@ -19,16 +21,16 @@
     operations = [
         django.contrib.postgres.operations.CreateExtension('intarray'),
         migrations.CreateModel(
             name='Stats',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('recipient_object_id', models.CharField(max_length=255, verbose_name='Recipient: Id')),
-                ('flags', models.JSONField(blank=True, default=dict, verbose_name='Flags stats')),
-                ('total', models.PositiveBigIntegerField(default=0, verbose_name='Total')),
+                ('flags', JSONField(blank=True, default=dict, verbose_name='Flags stats')),
+                ('total', models.BigIntegerField(default=0, verbose_name='Total')),
                 ('recipient_content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='stats_recipient', to='contenttypes.contenttype', verbose_name='Recipient: Content type')),
             ],
             options={
                 'verbose_name': 'Notification stats',
                 'verbose_name_plural': 'List of notifications stats',
                 'ordering': ('-pk',),
             },
@@ -39,15 +41,15 @@
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('recipient_object_id', models.CharField(max_length=255, verbose_name='Recipient: Id')),
                 ('actor_object_id', models.CharField(blank=True, max_length=255, null=True, verbose_name='Actor: Id')),
                 ('action_object_id', models.CharField(blank=True, max_length=255, null=True, verbose_name='Action: Id')),
                 ('target_object_id', models.CharField(blank=True, max_length=255, null=True, verbose_name='Target: Id')),
                 ('flags', django.contrib.postgres.fields.ArrayField(base_field=models.PositiveIntegerField(), size=None, verbose_name='Flags')),
                 ('message', models.TextField(verbose_name='Message')),
-                ('data', models.JSONField(blank=True, default=dict, verbose_name='Data')),
+                ('data', JSONField(blank=True, default=dict, verbose_name='Data')),
                 ('sended_at', models.DateTimeField(db_index=True, default=django.utils.timezone.now)),
                 ('created_at', models.DateTimeField(db_index=True, default=django.utils.timezone.now)),
                 ('ordering_field', models.BigIntegerField(db_index=True, editable=False)),
                 ('action_content_type', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='notification_action', to='contenttypes.contenttype', verbose_name='Action: Content type')),
                 ('actor_content_type', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='notification_actor', to='contenttypes.contenttype', verbose_name='Actor: Content type')),
                 ('parent', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='children', to='wcd_notifications.notification', verbose_name='Parent notification')),
                 ('recipient_content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='notification_recipient', to='contenttypes.contenttype', verbose_name='Recipient: Content type')),
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/models/notifications.py` & `wc-django-notifications-0.1.3/wcd_notifications/models/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.utils import timezone
 from django.utils.translation import pgettext_lazy
 from django.db import models
 from django.contrib.postgres.indexes import GinIndex, BTreeIndex
 from px_pipeline import Filter
 
 from ..utils import Registry, make_generic_Q, to_intarray, ModelDef
+from ..compat import IntegerChoices, JSONField
 
 
 __all__ = (
     'Readability',
     'NotificationQuerySet', 'Notification',
     'make_generic_Q',
     'prepare_ordering',
@@ -27,15 +28,15 @@
 
 
 class FlagStats(TypedDict):
     recipient: RecipientDef
     stats: Dict[int, int]
 
 
-class Readability(models.IntegerChoices):
+class Readability(IntegerChoices):
     UNREAD = READABILITY_BASE_NUMBER + 2, pgettext_lazy('wcd_notifications', 'Unread')
     READ = READABILITY_BASE_NUMBER + 6, pgettext_lazy('wcd_notifications', 'Read')
 
 
 class FlagsRegistry(Registry):
     def add(self, choices: Type[Enum]):
         for item in choices:
@@ -182,15 +183,15 @@
         null=False, blank=True, default=list,
     )
     message = models.TextField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Message'),
         null=False, blank=False,
     )
 
-    data = models.JSONField(
+    data = JSONField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Data'),
         blank=True, null=False, default=dict,
     )
     sended_at = models.DateTimeField(default=timezone.now, db_index=True)
     created_at = models.DateTimeField(default=timezone.now, db_index=True)
     ordering_field = models.BigIntegerField(db_index=True, editable=False)
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/models/stats.py` & `wc-django-notifications-0.1.3/wcd_notifications/models/stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import pgettext_lazy
 from django.db import models
 from django.contrib.postgres.indexes import BTreeIndex
 
 from ..utils import make_generic_Q, ModelDef
+from ..compat import JSONField
 
 
 __all__ = 'StatsQuerySet', 'Stats',
 
 
 class StatsQuerySet(models.QuerySet):
     def recipients(self, recipients: Sequence[ModelDef]):
@@ -35,18 +36,18 @@
         related_name='stats_recipient', on_delete=models.CASCADE,
     )
     recipient_object_id = models.CharField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Recipient: Id'),
         max_length=255, null=False, blank=False,
     )
     recipient = GenericForeignKey('recipient_content_type', 'recipient_object_id')
-    flags = models.JSONField(
+    flags = JSONField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Flags stats'),
         blank=True, null=False, default=dict,
     )
-    total = models.PositiveBigIntegerField(
+    total = models.BigIntegerField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Total'),
         default=0,
     )
 
     def __str__(self):
         return str(self.pk)
```

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/services/manager.py` & `wc-django-notifications-0.1.3/wcd_notifications/services/manager.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/services/notifier.py` & `wc-django-notifications-0.1.3/wcd_notifications/services/notifier.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.2/wcd_notifications/utils.py` & `wc-django-notifications-0.1.3/wcd_notifications/utils.py`

 * *Files identical despite different names*

