# Comparing `tmp/django-silly-auth-1.0.4.tar.gz` & `tmp/django-silly-auth-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.4.tar", last modified: Wed Apr 12 17:32:44 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.5.tar", last modified: Fri Apr 14 16:45:24 2023, max compression
```

## Comparing `django-silly-auth-1.0.4.tar` & `django-silly-auth-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.4/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      981 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.869113 django-silly-auth-1.0.4/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4859 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10584 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.861112 django-silly-auth-1.0.4/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10598 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.861112 django-silly-auth-1.0.4/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10108 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    15877 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5953 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.877113 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5003 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-11 18:51:15.000000 django-silly-auth-1.0.4/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6476 2023-04-12 17:32:02.000000 django-silly-auth-1.0.4/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13685 2023-04-11 19:05:08.000000 django-silly-auth-1.0.4/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.4/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-12 17:32:44.873113 django-silly-auth-1.0.4/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2294 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-12 17:32:44.000000 django-silly-auth-1.0.4/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-12 17:32:44.881113 django-silly-auth-1.0.4/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.4/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.5/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1620 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1010 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5631 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10574 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.897895 django-silly-auth-1.0.5/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10588 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.897895 django-silly-auth-1.0.5/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10088 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    15857 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6096 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4478 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_single_page.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/django_silly_auth/tests/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/tests/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3790 2023-04-14 16:20:53.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3971 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_classic_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1051 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4924 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3254 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-14 13:53:37.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      445 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6472 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13683 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1771 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/views/try_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1620 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2464 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2227 2023-04-14 16:45:16.000000 django-silly-auth-1.0.5/setup.py
```

### Comparing `django-silly-auth-1.0.4/LICENSE.md` & `django-silly-auth-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/PKG-INFO` & `django-silly-auth-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.4
+Version: 1.0.5
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -39,10 +39,11 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.4/README.md` & `django-silly-auth-1.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/config.py` & `django-silly-auth-1.0.5/django_silly_auth/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class SillyAuthError(Exception):
     pass
 
 
 SILLY_AUTH_SETTINGS = {
     # Quick settings
-    "AUTO_SET": 'TEST',  # 'CLASSIC', 'SPA', 'SILLY or 'TEST'
+    "AUTO_SET": 'TRY',  # 'CLASSIC', 'SPA', 'TRY', 'SILLY' or 'TEST'
     "DSA_PREFIX": 'auth/',  # only the CLASSIC_INDEX view has a blank prefix, it's the entry point in a classic site.
 
     # Secondary settings
     "SITE_NAME": None,  # str used in templates if provided
     "DELETE_UNCONFIRMED_TIME": 24.0,  # hours after what an unconfirmed account is deleted, O to set off
 
     # Classic settings
@@ -35,17 +35,18 @@
 
     # DRF settings
     "USE_DRF": False,  # False for only classic django views
     "CONFIRMATION_METHOD": 'GET',  # 'GET' or 'POST'
     "ALLOW_CREATE_USER_ENDPOINT": True,  # activate this endpoint
     "ALLOW_MY_INFOS_ENDPOINT": True,  # activate this endpoint
     "ALLOW_DELETE_ME_ENDPOINT": True,  # activate this endpoint
+    "USER_INFOS_EXCLUDE": ['password', 'id'],  # fields to exclude from the user infos
 
     # pure SPA only:
-    "SPA_EMAIL_LOGIN_LINK": "http://your spa adress/",  # + <jwt_token>",
+    "SPA_EMAIL_LOGIN_LINK": "http://your spa address/",  # + <jwt_token>",
 
 
     # Silly settings
     "USE_SILLY": False,
     "SILLY_LINK_TO_SPA": None,  # link used in templates to get back to your SPA
 
     # emails settings
@@ -53,32 +54,32 @@
     "EMAIL_VALID_TIME": 1200,  # seconds
     "EMAIL_CONFIRM_ACCOUNT_TEMPLATE":
         "silly_auth/emails/confirm_email.txt",
     "EMAIL_RESET_PASSWORD_TEMPLATE":  # email template
         "silly_auth/emails/request_password_reset.txt",
 
     # For development,
-    "TEST_TEMPLATES": False,  # for dev only,  opens 2 "_test/" endpoint
+    "TRY_TEMPLATES": False,  # for dev only,  opens 2 "_test/" endpoint
     "VERBOSE": False,  # prints to terminal : imports
 }
 
 
 # Overwrite SILLY_AUTH_SETTINGS with datas from settings.SILLY_AUTH
 
 try:
     settings.SILLY_AUTH
     is_set = True
 except AttributeError:
     is_set = False
 
 if is_set and "AUTO_SET" in settings.SILLY_AUTH:
     auto_set = settings.SILLY_AUTH['AUTO_SET']
-    if auto_set not in ['CLASSIC', 'SPA', 'SILLY', 'TEST']:
+    if auto_set not in ['CLASSIC', 'SPA', 'SILLY', 'TRY', 'TEST']:
         raise SillyAuthError(
-            "AUTO_SET must be 'CLASSIC', 'SPA', 'SILLY or 'TEST'")
+            "AUTO_SET must be 'CLASSIC', 'SPA', 'SILLY', 'TRY' or 'TEST'")
 else:
     auto_set = SILLY_AUTH_SETTINGS["AUTO_SET"]
 
 match auto_set:
     case "CLASSIC":
         SILLY_AUTH_SETTINGS["USE_DRF"] = False
         SILLY_AUTH_SETTINGS["USE_CLASSIC"] = True
@@ -91,22 +92,35 @@
 
     case "SILLY":
         SILLY_AUTH_SETTINGS["USE_DRF"] = True
         SILLY_AUTH_SETTINGS["USE_CLASSIC"] = False
         SILLY_AUTH_SETTINGS["CONFIRMATION_METHOD"] = 'GET'
         SILLY_AUTH_SETTINGS["USE_SILLY"] = True
 
-    case "TEST":
+    case "TRY":
         SILLY_AUTH_SETTINGS["USE_DRF"] = False
         SILLY_AUTH_SETTINGS["USE_CLASSIC"] = True
         SILLY_AUTH_SETTINGS["CONFIRMATION_METHOD"] = 'GET'
-        SILLY_AUTH_SETTINGS["BASE_TEMPLATE"] = "silly_auth/_test/_base.html"
-        SILLY_AUTH_SETTINGS["TEST_TEMPLATES"] = True
+        SILLY_AUTH_SETTINGS["BASE_TEMPLATE"] = "silly_auth/_try/_base.html"
+        SILLY_AUTH_SETTINGS["TRY_TEMPLATES"] = True
         SILLY_AUTH_SETTINGS["VERBOSE"] = True
 
+    case "TEST":
+        SILLY_AUTH_SETTINGS["USE_DRF"] = True
+        SILLY_AUTH_SETTINGS["ALLOW_CREATE_USER_ENDPOINT"] = True,
+        SILLY_AUTH_SETTINGS["ALLOW_MY_INFOS_ENDPOINT"] = True,
+        SILLY_AUTH_SETTINGS["ALLOW_DELETE_ME_ENDPOINT"] = True,
+        SILLY_AUTH_SETTINGS["USE_CLASSIC"] = True
+        SILLY_AUTH_SETTINGS["USE_CLASSIC_INDEX"] = True,
+        SILLY_AUTH_SETTINGS["USE_CLASSIC_ACCOUNT"] = True,
+        SILLY_AUTH_SETTINGS["USE_SILLY"] = True
+        SILLY_AUTH_SETTINGS["CONFIRMATION_METHOD"] = 'GET'
+        SILLY_AUTH_SETTINGS["BASE_TEMPLATE"] = "silly_auth/_try/_base.html"
+        SILLY_AUTH_SETTINGS["EMAIL_TERMINAL_PRINT"] = False
+
 if is_set:
     for key in settings.SILLY_AUTH:
         if key not in SILLY_AUTH_SETTINGS:
             raise SillyAuthError(f"Unexpected key in settings.SILLY_AUTH: '{key}'")
         SILLY_AUTH_SETTINGS[key] = settings.SILLY_AUTH[key]
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/forms.py` & `django-silly-auth-1.0.5/django_silly_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/locale/django.pot` & `django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# django-silly-auth translation file
+# Copyright (C) 2023 Vincent Fabre
+# This file is distributed under the same license as the django-silly-auth package.
+# Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-12 19:04+0200\n"
+"POT-Creation-Date: 2023-04-14 18:23+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -43,15 +43,15 @@
 msgid "Confirm password"
 msgstr ""
 
 #: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:50 serializers.py:189
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr ""
@@ -62,15 +62,15 @@
 msgstr ""
 
 #: forms.py:132
 #, python-format
 msgid "'%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:164 serializers.py:73
+#: forms.py:164 serializers.py:79
 msgid "The passwords you entered do not match."
 msgstr ""
 
 #: forms.py:170
 msgid "New username"
 msgstr ""
 
@@ -103,98 +103,98 @@
 msgid "Username must contain only letters, digits and ./+/-/_ characters."
 msgstr ""
 
 #: mixins.py:45
 msgid "email address"
 msgstr ""
 
-#: serializers.py:99
+#: serializers.py:105
 msgid "This email is already associated with an existing account."
 msgstr ""
 
-#: serializers.py:120 serializers.py:148
+#: serializers.py:126 serializers.py:154
 msgid "Email not found"
 msgstr ""
 
-#: serializers.py:123 serializers.py:153
+#: serializers.py:129 serializers.py:159
 msgid "User not found"
 msgstr ""
 
-#: serializers.py:161
+#: serializers.py:167
 msgid "The given token does not match the user"
 msgstr ""
 
-#: serializers.py:163
+#: serializers.py:169
 msgid "jwt token invalid or expired"
 msgstr ""
 
-#: serializers.py:180
+#: serializers.py:186
 msgid "This username is already associated with an existing account."
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:29
+#: templates/silly_auth/_try/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:34
+#: templates/silly_auth/_try/_base.html:34
 #: templates/silly_auth/classic/account.html:9
 msgid "Account"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:40
+#: templates/silly_auth/_try/_base.html:40
 msgid "More"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:45
+#: templates/silly_auth/_try/_base.html:45
 msgid "Documentation"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:48
+#: templates/silly_auth/_try/_base.html:48
 msgid "Buy me a coffee"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:51
+#: templates/silly_auth/_try/_base.html:51
 msgid "Contact"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:55
+#: templates/silly_auth/_try/_base.html:55
 msgid "Report an issue"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:67
+#: templates/silly_auth/_try/_base.html:67
 msgid "Log out"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:71
+#: templates/silly_auth/_try/_base.html:71
 #: templates/silly_auth/classic/signup.html:5
 msgid "Sign up"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:74
+#: templates/silly_auth/_try/_base.html:74
 msgid "Log in"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:85
-msgid "Test single page"
+#: templates/silly_auth/_try/_base.html:85
+msgid "Single page"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:86
-msgid "Test Users page"
+#: templates/silly_auth/_try/_base.html:86
+msgid "Users page"
 msgstr ""
 
-#: templates/silly_auth/_test/_test.html:8
+#: templates/silly_auth/_try/_single_page.html:8
 msgid "Test template"
 msgstr ""
 
-#: templates/silly_auth/_test/_test.html:10
+#: templates/silly_auth/_try/_single_page.html:10
 msgid "Simple test here"
 msgstr ""
 
-#: templates/silly_auth/_test/_users.html:7
+#: templates/silly_auth/_try/_users.html:7
 msgid "Test users"
 msgstr ""
 
 #: templates/silly_auth/classic/account.html:12
 msgid "id:"
 msgstr ""
 
@@ -347,23 +347,23 @@
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
-#: views/api_views_if_drf.py:40
+#: views/api_views_if_drf.py:41
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:48 views/classics.py:362
+#: views/api_views_if_drf.py:49 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
-#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:53 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr ""
 
 #: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr ""
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.0.5/django_silly_auth/locale/django.pot`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# django-silly-auth translation file
-# Copyright (C) 2023 Vincent Fabre
-# This file is distributed under the same license as the django-silly-auth package.
-# Vincent Fabre <peigne.plume@gmail.com>, 2023.
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-12 19:04+0200\n"
+"POT-Creation-Date: 2023-04-14 18:23+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -43,15 +43,15 @@
 msgid "Confirm password"
 msgstr ""
 
 #: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:50 serializers.py:189
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr ""
@@ -62,15 +62,15 @@
 msgstr ""
 
 #: forms.py:132
 #, python-format
 msgid "'%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:164 serializers.py:73
+#: forms.py:164 serializers.py:79
 msgid "The passwords you entered do not match."
 msgstr ""
 
 #: forms.py:170
 msgid "New username"
 msgstr ""
 
@@ -103,98 +103,98 @@
 msgid "Username must contain only letters, digits and ./+/-/_ characters."
 msgstr ""
 
 #: mixins.py:45
 msgid "email address"
 msgstr ""
 
-#: serializers.py:99
+#: serializers.py:105
 msgid "This email is already associated with an existing account."
 msgstr ""
 
-#: serializers.py:120 serializers.py:148
+#: serializers.py:126 serializers.py:154
 msgid "Email not found"
 msgstr ""
 
-#: serializers.py:123 serializers.py:153
+#: serializers.py:129 serializers.py:159
 msgid "User not found"
 msgstr ""
 
-#: serializers.py:161
+#: serializers.py:167
 msgid "The given token does not match the user"
 msgstr ""
 
-#: serializers.py:163
+#: serializers.py:169
 msgid "jwt token invalid or expired"
 msgstr ""
 
-#: serializers.py:180
+#: serializers.py:186
 msgid "This username is already associated with an existing account."
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:29
+#: templates/silly_auth/_try/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:34
+#: templates/silly_auth/_try/_base.html:34
 #: templates/silly_auth/classic/account.html:9
 msgid "Account"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:40
+#: templates/silly_auth/_try/_base.html:40
 msgid "More"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:45
+#: templates/silly_auth/_try/_base.html:45
 msgid "Documentation"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:48
+#: templates/silly_auth/_try/_base.html:48
 msgid "Buy me a coffee"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:51
+#: templates/silly_auth/_try/_base.html:51
 msgid "Contact"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:55
+#: templates/silly_auth/_try/_base.html:55
 msgid "Report an issue"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:67
+#: templates/silly_auth/_try/_base.html:67
 msgid "Log out"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:71
+#: templates/silly_auth/_try/_base.html:71
 #: templates/silly_auth/classic/signup.html:5
 msgid "Sign up"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:74
+#: templates/silly_auth/_try/_base.html:74
 msgid "Log in"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:85
-msgid "Test single page"
+#: templates/silly_auth/_try/_base.html:85
+msgid "Single page"
 msgstr ""
 
-#: templates/silly_auth/_test/_base.html:86
-msgid "Test Users page"
+#: templates/silly_auth/_try/_base.html:86
+msgid "Users page"
 msgstr ""
 
-#: templates/silly_auth/_test/_test.html:8
+#: templates/silly_auth/_try/_single_page.html:8
 msgid "Test template"
 msgstr ""
 
-#: templates/silly_auth/_test/_test.html:10
+#: templates/silly_auth/_try/_single_page.html:10
 msgid "Simple test here"
 msgstr ""
 
-#: templates/silly_auth/_test/_users.html:7
+#: templates/silly_auth/_try/_users.html:7
 msgid "Test users"
 msgstr ""
 
 #: templates/silly_auth/classic/account.html:12
 msgid "id:"
 msgstr ""
 
@@ -347,23 +347,23 @@
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
-#: views/api_views_if_drf.py:40
+#: views/api_views_if_drf.py:41
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:48 views/classics.py:362
+#: views/api_views_if_drf.py:49 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
-#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:53 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr ""
 
 #: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr ""
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-12 19:06+0200\n"
+"PO-Revision-Date: 2023-04-14 18:24+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -262,19 +262,16 @@
 
 msgid "Sign up"
 msgstr "S'enregistrer"
 
 msgid "Simple test here"
 msgstr "Simple test ici"
 
-msgid "Test Users page"
-msgstr "Test page utilisateurs"
-
-msgid "Test single page"
-msgstr "Test page unique"
+msgid "Single page"
+msgstr "Page simple"
 
 msgid "Test template"
 msgstr "Template de test"
 
 msgid "Test users"
 msgstr "Test utilisateurs"
 
@@ -311,14 +308,17 @@
 
 msgid "Username or email"
 msgstr "Nom d'utilisateur ou email"
 
 msgid "Username successfully changed."
 msgstr "Nom d'utilisateur changé avec succès."
 
+msgid "Users page"
+msgstr "Page utilisateurs"
+
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 "Vous avez été connecté via un email de confirmation. Réinitialisez votre mot "
 "de passe si besoin."
 
 msgid ""
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the django-silly-auth package.
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-12 19:04+0200\n"
-"PO-Revision-Date: 2023-04-12 19:06+0200\n"
+"POT-Creation-Date: 2023-04-14 18:23+0200\n"
+"PO-Revision-Date: 2023-04-14 18:24+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -44,15 +44,15 @@
 msgid "Confirm password"
 msgstr "Confirmez le mot de passe"
 
 #: forms.py:88
 msgid "different than password"
 msgstr "mots de passe différents"
 
-#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44 serializers.py:183
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:50 serializers.py:189
 msgid "A username cannot include the symbol '@'."
 msgstr "Un nom d'utilisateur ne peut pas inclure '@'."
 
 #: forms.py:99 forms.py:186
 #, python-format
 msgid "'%(username)s' is already taken by someone else."
 msgstr "'%(username)s' est déjà utilisé par quelqu'un."
@@ -63,15 +63,15 @@
 msgstr "'%(email)s' déjà utilisé par quelqu'un."
 
 #: forms.py:132
 #, python-format
 msgid "'%(credential)s' unknown or unconfirmed"
 msgstr "'%(credential)s' inconnu ou non confirmé"
 
-#: forms.py:164 serializers.py:73
+#: forms.py:164 serializers.py:79
 msgid "The passwords you entered do not match."
 msgstr "Les mots de passe saisis ne correspondent pas."
 
 #: forms.py:170
 msgid "New username"
 msgstr "Nouveau nom d'utilisateur"
 
@@ -105,98 +105,98 @@
 msgstr ""
 "Un nom d'utilisateur ne doit contenir que des lettres, nombres, ou +/-/_/."
 
 #: mixins.py:45
 msgid "email address"
 msgstr "adresse email"
 
-#: serializers.py:99
+#: serializers.py:105
 msgid "This email is already associated with an existing account."
 msgstr "Cet email est déjà associé à un compte existant."
 
-#: serializers.py:120 serializers.py:148
+#: serializers.py:126 serializers.py:154
 msgid "Email not found"
 msgstr "Email inconnu"
 
-#: serializers.py:123 serializers.py:153
+#: serializers.py:129 serializers.py:159
 msgid "User not found"
 msgstr "Utilisateur inconnu"
 
-#: serializers.py:161
+#: serializers.py:167
 msgid "The given token does not match the user"
 msgstr "Le token fourni ne correspond pas à l'utilisateur"
 
-#: serializers.py:163
+#: serializers.py:169
 msgid "jwt token invalid or expired"
 msgstr "le token jwt est invalide ou expiré"
 
-#: serializers.py:180
+#: serializers.py:186
 msgid "This username is already associated with an existing account."
 msgstr "Ce nom d'utilisateur est déjà associé à un compte existant."
 
-#: templates/silly_auth/_test/_base.html:29
+#: templates/silly_auth/_try/_base.html:29
 #: templates/silly_auth/classic/index.html:9
 msgid "Home"
 msgstr "Accueil"
 
-#: templates/silly_auth/_test/_base.html:34
+#: templates/silly_auth/_try/_base.html:34
 #: templates/silly_auth/classic/account.html:9
 msgid "Account"
 msgstr "Compte"
 
-#: templates/silly_auth/_test/_base.html:40
+#: templates/silly_auth/_try/_base.html:40
 msgid "More"
 msgstr "Plus"
 
-#: templates/silly_auth/_test/_base.html:45
+#: templates/silly_auth/_try/_base.html:45
 msgid "Documentation"
 msgstr "Documentation"
 
-#: templates/silly_auth/_test/_base.html:48
+#: templates/silly_auth/_try/_base.html:48
 msgid "Buy me a coffee"
 msgstr "Offrez-moi un café"
 
-#: templates/silly_auth/_test/_base.html:51
+#: templates/silly_auth/_try/_base.html:51
 msgid "Contact"
 msgstr "Contact"
 
-#: templates/silly_auth/_test/_base.html:55
+#: templates/silly_auth/_try/_base.html:55
 msgid "Report an issue"
 msgstr "Signaler un problème"
 
-#: templates/silly_auth/_test/_base.html:67
+#: templates/silly_auth/_try/_base.html:67
 msgid "Log out"
 msgstr "Déconnexion"
 
-#: templates/silly_auth/_test/_base.html:71
+#: templates/silly_auth/_try/_base.html:71
 #: templates/silly_auth/classic/signup.html:5
 msgid "Sign up"
 msgstr "S'enregistrer"
 
-#: templates/silly_auth/_test/_base.html:74
+#: templates/silly_auth/_try/_base.html:74
 msgid "Log in"
 msgstr "Connexion"
 
-#: templates/silly_auth/_test/_base.html:85
-msgid "Test single page"
-msgstr "Test page unique"
-
-#: templates/silly_auth/_test/_base.html:86
-msgid "Test Users page"
-msgstr "Test page utilisateurs"
+#: templates/silly_auth/_try/_base.html:85
+msgid "Single page"
+msgstr "Page simple"
+
+#: templates/silly_auth/_try/_base.html:86
+msgid "Users page"
+msgstr "Page utilisateurs"
 
-#: templates/silly_auth/_test/_test.html:8
+#: templates/silly_auth/_try/_single_page.html:8
 msgid "Test template"
 msgstr "Template de test"
 
-#: templates/silly_auth/_test/_test.html:10
+#: templates/silly_auth/_try/_single_page.html:10
 msgid "Simple test here"
 msgstr "Simple test ici"
 
-#: templates/silly_auth/_test/_users.html:7
+#: templates/silly_auth/_try/_users.html:7
 msgid "Test users"
 msgstr "Test utilisateurs"
 
 #: templates/silly_auth/classic/account.html:12
 msgid "id:"
 msgstr "id:"
 
@@ -382,23 +382,23 @@
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 "Connexion par email de confirmation, changez votre mot de passe si besoin."
 
-#: views/api_views_if_drf.py:40
+#: views/api_views_if_drf.py:41
 msgid "no credential provided"
 msgstr "aucun identifiant fourni"
 
-#: views/api_views_if_drf.py:48 views/classics.py:362
+#: views/api_views_if_drf.py:49 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr "Votre compte est déjà confirmé."
 
-#: views/api_views_if_drf.py:52 views/api_views_if_drf.py:82
+#: views/api_views_if_drf.py:53 views/api_views_if_drf.py:82
 msgid "Email sent for password reset"
 msgstr "Email envoyé pour réinitialisation du mot de passe"
 
 #: views/api_views_if_drf.py:64
 msgid "Logged out."
 msgstr "Déconnexion."
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/mixins.py` & `django-silly-auth-1.0.5/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/serializers.py` & `django-silly-auth-1.0.5/django_silly_auth/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.serializers")
 
 User = get_user_model()
 
 
+class UserInfosSerializer(serializers.ModelSerializer):
+    class Meta:
+        model = User
+        exclude = [*conf["USER_INFOS_EXCLUDE"]]
+
+
 class GetAllUsersSerializer(serializers.ModelSerializer):
     class Meta:
         model = User
         fields = '__all__'
 
 
 class CreateUserSerializer(serializers.ModelSerializer):
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_base.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   <body class="has-navbar-fixed-top">
   <section class="section">
     <div class="container">
 
       <nav class="navbar is-fixed-top pl-2 pr-2" role="navigation" aria-label="main navigation">
         <div class="navbar-brand">
           <a class="navbar-item" href="https://github.com/byoso/django_silly_auth" target="_blank">
-            <h1 class="title">DSA test - base template</h1>
+            <h1 class="title">Django Silly Auth</h1>
           </a>
           <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
             <span aria-hidden="true"></span>
             <span aria-hidden="true"></span>
             <span aria-hidden="true"></span>
           </a>
         </div>
@@ -78,16 +78,16 @@
             </div>
           </div>
 
         </div>
       </nav>
       <nav>
 
-        <a href="{% url 'test_templates_view' %}">  {% translate 'Test single page' %}</a>
-        <a href="{% url 'test_users_view' %}"> :: {% translate 'Test Users page' %}</a>
+        <a href="{% url 'try_templates_view' %}">  {% translate 'Single page' %}</a>
+        <a href="{% url 'try_users_view' %}"> :: {% translate 'Users page' %}</a>
 
       </nav>
 
       {% if messages %}
 
         {% for message in messages %}
           <div class="notification is-{{ message.tags }}">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 {% load i18n %}
 
-******_DSA_test_-_base_template_******
+******_Django_Silly_Auth_******
 
 {%_translate_'Home'_%} {% if user.is_authenticated %} {%_translate_'Account'_%}
 {% endif%}
 {% translate 'More' %}
 {%_translate_'Documentation'_%} {%_translate_'Buy_me_a_coffee'_%} {%_translate
 'Contact'_%}
 ===============================================================================
 {%_translate_'Report_an_issue'_%}
 {% if user.is_authenticated %} {%_translate_'Log_out'_%} {% else %} {%
 translate_'Sign_up'_%} {%_translate_'Log_in'_%} {% endif %}
-  {%_translate_'Test_single_page'_%} ::_{%_translate_'Test_Users_page'_%}  {%
-if messages %} {% for message in messages %}
+  {%_translate_'Single_page'_%} ::_{%_translate_'Users_page'_%}  {% if messages
+%} {% for message in messages %}
  {{ message }}
 {% endfor %} {% endif %} {% block content %} {% endblock content %}
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/urls.py` & `django-silly-auth-1.0.5/django_silly_auth/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,23 @@
 from django.db.models.signals import pre_save
 from django.dispatch import receiver
 from django.contrib.auth import get_user_model
 
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
 from django_silly_auth.views import (
     api_views,
-    test_views,
+    try_views,
     silly_views,
     classics)
 
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.urls")
     if conf["USE_DRF"]:
-        print("=== DSA login_with_auth_token FROM django_silly_auth.views.api_custom_login")
-
-if conf["USE_DRF"]:
-    from django_silly_auth.views.api_custom_login import (
-        LoginWithAuthToken,
-        LoginWithJWTToken,
-    )
+        print("=== DSA LoginWithAuthToken FROM django_silly_auth.views.api_custom_login")
 
 prefix = conf["DSA_PREFIX"]
 User = get_user_model()
 
 
 # Signal interceptor to make sure that superusers are always active
 @receiver(pre_save, sender=User)
@@ -35,53 +29,53 @@
 
 
 urlpatterns = []
 
 # DRF routes
 if conf["USE_DRF"]:
     urlpatterns += [
-        path(f'{prefix}token/login/', LoginWithAuthToken.as_view(), name="login_with_auth_token"),
-        path(f'{prefix}token/logout/', api_views.logout_api_view, name="logout_api_view"),
+        path(f'{prefix}token/login/', api_views.LoginWithAuthToken.as_view(), name="token_login"),
+        path(f'{prefix}token/logout/', api_views.token_logout, name="token_logout"),
         path(
             f'{prefix}password/request_reset/',
-            api_views.request_password_reset,
-            name='request_password_reset'
+            api_views.password_request_reset,
+            name='password_request_reset'
         ),
         path(
             f'{prefix}email/confirm_email/resend/',
-            api_views.resend_email_confirmation,
-            name="resend_email_confirmation"
+            api_views.email_confirm_email_resend,
+            name="email_confirm_email_resend"
         ),
         path(
             f'{prefix}password/change/',
-            api_views.change_password,
-            name='change_password'
+            api_views.password_change,
+            name='password_change'
         ),
         path(
             f'{prefix}username/change/',
-            api_views.change_username,
-            name='change_username'
+            api_views.username_change,
+            name='username_change'
         ),
         path(
             f'{prefix}email/request_change/',
-            api_views.change_email_request,
-            name='change_email_request'
+            api_views.email_request_change,
+            name='email_request_change'
         ),
         ]
 
     if conf["ALLOW_DELETE_ME_ENDPOINT"]:
         urlpatterns += [
-            path(f'{prefix}users/delete_me/', api_views.delete_me, name='delete_me'),
+            path(f'{prefix}users/delete_me/', api_views.users_delete_me, name='users_delete_me'),
         ]
 
     if conf["ALLOW_CREATE_USER_ENDPOINT"]:
         urlpatterns += [path(f'{prefix}users/', api_views.UserView.as_view(), name="users")]
 
     if conf['ALLOW_MY_INFOS_ENDPOINT']:
-        urlpatterns += [path(f'{prefix}users/my_infos/', api_views.my_infos, name="my_infos")]
+        urlpatterns += [path(f'{prefix}users/my_infos/', api_views.users_my_infos, name="users_my_infos")]
 
 # Classic routes
 
 if conf["USE_CLASSIC"]:
     urlpatterns += [
         path(f'{prefix}classic_login/', classics.login_view, name='classic_login'),
         path(f'{prefix}classic_logout/', classics.logout_view, name='classic_logout'),
@@ -112,26 +106,26 @@
         path(f'{prefix}classic_reset_password/<token>', classics.reset_password, name='classic_reset_password'),
         path(f'{prefix}classic_request_password_reset/', classics.request_password_reset, name='classic_request_password_reset'),
     ]
     if conf["USE_SILLY"]:
         urlpatterns += [
             path(
                 f'{prefix}dsa_confirm_email/<token>',
-                silly_views.silly_confirm_email,
-                name='silly_confirm_email'),
+                silly_views.dsa_confirm_email,
+                name='dsa_confirm_email'),
             path(
                 f'{prefix}dsa_password_reset_done',
-                silly_views.silly_password_reset_done,
-                name='silly_password_reset_done'),
+                silly_views.dsa_password_reset_done,
+                name='dsa_password_reset_done'),
         ]
 
-if conf['CONFIRMATION_METHOD'] == 'POST':
+if conf['CONFIRMATION_METHOD'] == 'POST' or conf['AUTO_SET'] == 'TEST':
     urlpatterns += [
-        path(f'{prefix}login_with_jwt/', LoginWithJWTToken.as_view(), name="login_with_jwt_token"),
+        path(f'{prefix}login_with_jwt/', api_views.LoginWithJWTToken.as_view(), name="login_with_jwt"),
     ]
 
-# testing routes
-if conf["TEST_TEMPLATES"]:
+# trying routes
+if conf["TRY_TEMPLATES"] or conf['AUTO_SET'] == 'TEST':
     urlpatterns += [
-        path(f'{prefix}_test/', test_views.test_templates_view, name="test_templates_view"),
-        path(f'{prefix}_test_users/', test_views.test_users_view, name="test_users_view"),
+        path(f'{prefix}_try/', try_views.try_templates_view, name="try_templates_view"),
+        path(f'{prefix}_try_users/', try_views.try_users_view, name="try_users_view"),
         ]
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/utils.py` & `django-silly-auth-1.0.5/django_silly_auth/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def send_confirm_email(request, user, new_email=False):
     token = user.get_jwt_token(expires_in=conf["EMAIL_VALID_TIME"])
     domain = request.build_absolute_uri('/')[:-1]
     # if new_email:
     if conf["USE_SILLY"]:
-        link = domain + reverse('silly_confirm_email', args=[token])
+        link = domain + reverse('dsa_confirm_email', args=[token])
     elif conf["CONFIRMATION_METHOD"] == 'GET':
         link = domain + reverse('classic_confirm_email', args=[token])
     if conf["CONFIRMATION_METHOD"] == 'POST':
         link = conf['SPA_EMAIL_LOGIN_LINK'] + f"{token}"
     context = {
         'user': user,
         'link': link,
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.5/django_silly_auth/views/api_custom_login.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.4/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.5/django_silly_auth/views/api_views_if_drf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from rest_framework.decorators import api_view, permission_classes
 from rest_framework.permissions import AllowAny, IsAuthenticated
 from rest_framework.exceptions import (
     ValidationError,
     )
 
 from django_silly_auth.serializers import (
+    UserInfosSerializer,
     GetAllUsersSerializer,
     CreateUserSerializer,
     PasswordsSerializer,
     EmailSerializer,
     UsernameSerializer,
     )
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
@@ -29,15 +30,15 @@
 
 User = get_user_model()
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([AllowAny])
-def resend_email_confirmation(request):
+def email_confirm_email_resend(request):
     """Resends an email to the user to confirm his account"""
     credential = request.data.get('credential')
     if not credential:
         msg = _("no credential provided")
         raise ValidationError({"error": msg}, code='authorization')
     if "@" in credential:
         user = User.objects.filter(email=credential).first()
@@ -53,25 +54,24 @@
     msg = "Invalid credential"
     raise ValidationError({"error": msg}, code='authorization')
 
 
 @transaction.atomic
 @api_view(['GET'])
 @permission_classes([IsAuthenticated])
-def logout_api_view(request):
+def token_logout(request):
     """Destroys the auth token"""
-    print("=== DSA LOGOUT API VIEW")
     request.user.auth_token.delete()
     return Response({'success': _('Logged out.')})
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([AllowAny])
-def request_password_reset(request):
+def password_request_reset(request):
     """Sends an email to the user with a link to reset their password"""
     credential = request.data.get('credential')
     if not credential:
         msg = _("No credentials were provided")
         raise ValidationError({"error": msg}, code='authorization')
     if "@" in credential:
         user = User.objects.filter(email=credential).first()
@@ -122,15 +122,15 @@
             msg = serializer.errors
             raise ValidationError({"error": msg}, code='authorization')
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([IsAuthenticated])
-def change_password(request):
+def password_change(request):
     """Changes the user's password"""
     serializer = PasswordsSerializer(data=request.data)
     if serializer.is_valid():
         user = request.user
         password = request.data.get('password')
         user.set_password(password)
         user.save()
@@ -138,15 +138,15 @@
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([IsAuthenticated])
-def change_email_request(request):
+def email_request_change(request):
     user = request.user
     serializer = EmailSerializer(data=request.data)
     if serializer.is_valid():
         new_email = request.data.get('email')
         user.new_email = new_email
         user.save()
         send_confirm_email(request, user, new_email=True)
@@ -161,34 +161,34 @@
     raise ValidationError({"error": msg}, code='authorization')
 
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([IsAuthenticated])
-def change_username(request):
+def username_change(request):
     """Changes the user's username"""
     serializer = UsernameSerializer(data=request.data)
     if serializer.is_valid():
         user = request.user
         username = request.data.get('username')
         user.username = username
         user.save()
         return Response({'success': _('Username successfully changed.')})
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
 
 
 @api_view(['GET'])
 @permission_classes([IsAuthenticated])
-def my_infos(request):
+def users_my_infos(request):
     """Returns the user's infos"""
-    serializer = GetAllUsersSerializer(request.user)
+    serializer = UserInfosSerializer(request.user)
     return Response(serializer.data)
 
 @api_view(['DELETE'])
 @permission_classes([IsAuthenticated])
-def delete_me(request):
+def users_delete_me(request):
     """Deletes the user's account"""
     request.user.auth_token.delete()
     request.user.delete()
     return Response({'success': _('Account successfully deleted.')})
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.5/django_silly_auth/views/classics.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 
     if request.method == 'POST':
         form = ResetPasswordForm(request.POST)
         if form.is_valid():
             user.set_password(form.cleaned_data['password'])
             user.save()
             if conf["USE_SILLY"]:
-                return redirect('silly_password_reset_done')
+                return redirect('dsa_password_reset_done')
             login(request, user)
             messages.add_message(
                 request, messages.SUCCESS,
                 message=_("Your password has been successfully reset. Please log in."),
                 extra_tags="success"
             )
             return redirect('classic_index')
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.5/django_silly_auth/views/silly_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.views.classics")
 
 User = get_user_model()
 
 
 @transaction.atomic
-def silly_confirm_email(request, token):
+def dsa_confirm_email(request, token):
     user = User.verify_jwt_token(token)
     if user is None:
         msg = _("Token invalid or expired"),
         tag = "danger"
     if user is not None and user.is_active:
         if not user.is_confirmed:
             user.is_confirmed = True
@@ -42,15 +42,15 @@
         "tag": tag,
         "link": conf["SILLY_LINK_TO_SPA"],
         "site_name": conf["SITE_NAME"],
     }
     return render(request, 'silly_auth/silly/silly_confirm_email.html', context)
 
 
-def silly_password_reset_done(request):
+def dsa_password_reset_done(request):
     msg = _("Your password has been successfully reset.")
     context = {
         "base_template": conf["BASE_TEMPLATE"],
         "message": msg,
         "tag": "success",
         "link": conf["SILLY_LINK_TO_SPA"],
         "site_name": conf["SITE_NAME"],
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.5/django_silly_auth/views/try_views.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 """
 
 
 User = get_user_model()
 
 
 @transaction.atomic
-def test_templates_view(request):
+def try_templates_view(request):
     users = User.objects.all()
     context = {
         "users": users,
         "title": "dsa render test",
         "base_template": conf["BASE_TEMPLATE"],
     }
-    return render(request, "silly_auth/_test/_test.html", context)
+    return render(request, "silly_auth/_try/_single_page.html", context)
 
 
 @transaction.atomic
-def test_users_view(request):
+def try_users_view(request):
     users = User.objects.all()
     context = {
         "users": users,
         "title": "dsa render test",
         "base_template": conf["BASE_TEMPLATE"],
     }
-    return render(request, "silly_auth/_test/_users.html", context)
+    return render(request, "silly_auth/_try/_users.html", context)
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.5/django_silly_auth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.4
+Version: 1.0.5
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -39,10 +39,11 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.4/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.5/django_silly_auth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 django_silly_auth/locale/en/LC_MESSAGES/django.mo
 django_silly_auth/locale/en/LC_MESSAGES/django.po
 django_silly_auth/locale/fr/LC_MESSAGES/django.mo
 django_silly_auth/locale/fr/LC_MESSAGES/django.po
 django_silly_auth/templates/__init__.py
 django_silly_auth/templates/silly_auth/__init__.py
 django_silly_auth/templates/silly_auth/_base.html
-django_silly_auth/templates/silly_auth/_test/__init__.py
-django_silly_auth/templates/silly_auth/_test/_base.html
-django_silly_auth/templates/silly_auth/_test/_test.html
-django_silly_auth/templates/silly_auth/_test/_users.html
+django_silly_auth/templates/silly_auth/_try/__init__.py
+django_silly_auth/templates/silly_auth/_try/_base.html
+django_silly_auth/templates/silly_auth/_try/_single_page.html
+django_silly_auth/templates/silly_auth/_try/_users.html
 django_silly_auth/templates/silly_auth/classic/__init__.py
 django_silly_auth/templates/silly_auth/classic/account.html
 django_silly_auth/templates/silly_auth/classic/change_email.html
 django_silly_auth/templates/silly_auth/classic/change_username.html
 django_silly_auth/templates/silly_auth/classic/index.html
 django_silly_auth/templates/silly_auth/classic/login.html
 django_silly_auth/templates/silly_auth/classic/request_password_reset.html
@@ -36,14 +36,18 @@
 django_silly_auth/templates/silly_auth/classic/reset_password.html
 django_silly_auth/templates/silly_auth/classic/signup.html
 django_silly_auth/templates/silly_auth/emails/__init__.py
 django_silly_auth/templates/silly_auth/emails/confirm_email.txt
 django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
 django_silly_auth/templates/silly_auth/silly/__init__.py
 django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+django_silly_auth/tests/__init__.py
+django_silly_auth/tests/test_api_views.py
+django_silly_auth/tests/test_classic_views.py
+django_silly_auth/tests/test_silly_views.py
 django_silly_auth/views/__init__.py
 django_silly_auth/views/api_custom_login.py
 django_silly_auth/views/api_views.py
 django_silly_auth/views/api_views_if_drf.py
 django_silly_auth/views/classics.py
 django_silly_auth/views/silly_views.py
-django_silly_auth/views/test_views.py
+django_silly_auth/views/try_views.py
```

### Comparing `django-silly-auth-1.0.4/setup.py` & `django-silly-auth-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,25 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
     ],
     packages=[
         "django_silly_auth",
         "django_silly_auth.templates",
         "django_silly_auth.templates.silly_auth",
-        "django_silly_auth.templates.silly_auth._test",
+        "django_silly_auth.templates.silly_auth._try",
         "django_silly_auth.templates.silly_auth.classic",
         "django_silly_auth.templates.silly_auth.emails",
         "django_silly_auth.templates.silly_auth.silly",
         "django_silly_auth.views",
         "django_silly_auth.locale",
         "django_silly_auth.locale.fr",
         "django_silly_auth.locale.fr.LC_MESSAGES",
         "django_silly_auth.locale.en",
         "django_silly_auth.locale.en.LC_MESSAGES",
+        "django_silly_auth.tests",
         ],
     # include_package_data=True,
     package_data={'': ['*.txt', '*.html', '*.po', '*.mo', '*.pot']},
     python_requires='>=3.7',
     install_requires=[
         "pyjwt >= 2.6.0",
     ],
```

