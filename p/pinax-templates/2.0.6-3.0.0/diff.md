# Comparing `tmp/pinax-templates-2.0.6.tar.gz` & `tmp/pinax-templates-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinax-templates-2.0.6.tar", last modified: Thu Feb 20 21:31:27 2020, max compression
+gzip compressed data, was "pinax-templates-3.0.0.tar", last modified: Fri Apr 14 16:22:54 2023, max compression
```

## Comparing `pinax-templates-2.0.6.tar` & `pinax-templates-3.0.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/
--rw-r--r--   0 paltman    (501) staff       (20)     3413 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/PKG-INFO
--rw-r--r--   0 paltman    (501) staff       (20)     1101 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/LICENSE
--rw-r--r--   0 paltman    (501) staff       (20)       53 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/AUTHORS
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/
--rw-r--r--   0 paltman    (501) staff       (20)     3413 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/PKG-INFO
--rw-r--r--   0 paltman    (501) staff       (20)        1 2020-02-20 21:16:30.000000 pinax-templates-2.0.6/pinax_templates.egg-info/not-zip-safe
--rw-r--r--   0 paltman    (501) staff       (20)     6307 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/SOURCES.txt
--rw-r--r--   0 paltman    (501) staff       (20)       42 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/requires.txt
--rw-r--r--   0 paltman    (501) staff       (20)        6 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/top_level.txt
--rw-r--r--   0 paltman    (501) staff       (20)        1 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax_templates.egg-info/dependency_links.txt
--rw-r--r--   0 paltman    (501) staff       (20)      139 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/MANIFEST.in
--rw-r--r--   0 paltman    (501) staff       (20)     5888 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/README.md
--rw-r--r--   0 paltman    (501) staff       (20)     3477 2020-02-20 21:31:04.000000 pinax-templates-2.0.6/setup.py
--rw-r--r--   0 paltman    (501) staff       (20)      114 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/setup.cfg
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/
--rw-r--r--   0 paltman    (501) staff       (20)       83 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/__init__.py
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/ja/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/ja/LC_MESSAGES/
--rw-r--r--   0 paltman    (501) staff       (20)     8014 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 paltman    (501) staff       (20)    12476 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/zh_CN/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 paltman    (501) staff       (20)     5728 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 paltman    (501) staff       (20)     9168 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/de/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/de/LC_MESSAGES/
--rw-r--r--   0 paltman    (501) staff       (20)     9303 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 paltman    (501) staff       (20)    17326 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/fr/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/locale/fr/LC_MESSAGES/
--rw-r--r--   0 paltman    (501) staff       (20)     7918 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 paltman    (501) staff       (20)    12579 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/tests/
--rw-r--r--   0 paltman    (501) staff       (20)        0 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/tests/models.py
--rw-r--r--   0 paltman    (501) staff       (20)        0 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/tests/__init__.py
--rw-r--r--   0 paltman    (501) staff       (20)     1219 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/tests/settings.py
--rw-r--r--   0 paltman    (501) staff       (20)       93 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/tests/tests.py
--rw-r--r--   0 paltman    (501) staff       (20)       18 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/tests/urls.py
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/management/
--rw-r--r--   0 paltman    (501) staff       (20)        0 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/management/__init__.py
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/management/commands/
--rw-r--r--   0 paltman    (501) staff       (20)        0 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/management/commands/__init__.py
--rw-r--r--   0 paltman    (501) staff       (20)     1117 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/management/commands/copy_templates.py
--rw-r--r--   0 paltman    (501) staff       (20)      149 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/__init__.py
--rw-r--r--   0 paltman    (501) staff       (20)      241 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/apps.py
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pagination/
--rw-r--r--   0 paltman    (501) staff       (20)     1746 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pagination/_pagination.html
--rw-r--r--   0 paltman    (501) staff       (20)     2909 2020-02-20 21:15:21.000000 pinax-templates-2.0.6/pinax/templates/templates/base.html
--rw-r--r--   0 paltman    (501) staff       (20)      132 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/site_base.html
--rw-r--r--   0 paltman    (501) staff       (20)      404 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/500.html
--rw-r--r--   0 paltman    (501) staff       (20)      326 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/404.html
--rw-r--r--   0 paltman    (501) staff       (20)     1034 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/_account_bar.html
--rw-r--r--   0 paltman    (501) staff       (20)      133 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/_nav.html
--rw-r--r--   0 paltman    (501) staff       (20)      227 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/_messages.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/account/
--rw-r--r--   0 paltman    (501) staff       (20)      596 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/signup_closed.html
--rw-r--r--   0 paltman    (501) staff       (20)     1274 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/base.html
--rw-r--r--   0 paltman    (501) staff       (20)      437 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email_confirmed.html
--rw-r--r--   0 paltman    (501) staff       (20)      511 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/password_reset_token_fail.html
--rw-r--r--   0 paltman    (501) staff       (20)      692 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email_confirm.html
--rw-r--r--   0 paltman    (501) staff       (20)     1018 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/password_reset.html
--rw-r--r--   0 paltman    (501) staff       (20)      627 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/password_reset_token.html
--rw-r--r--   0 paltman    (501) staff       (20)     1345 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/login.html
--rw-r--r--   0 paltman    (501) staff       (20)     1125 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/password_reset_sent.html
--rw-r--r--   0 paltman    (501) staff       (20)      503 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/settings.html
--rw-r--r--   0 paltman    (501) staff       (20)      687 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email_confirmation_sent.html
--rw-r--r--   0 paltman    (501) staff       (20)      567 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/logout.html
--rw-r--r--   0 paltman    (501) staff       (20)      692 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/delete.html
--rw-r--r--   0 paltman    (501) staff       (20)      550 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/password_change.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/
--rw-r--r--   0 paltman    (501) staff       (20)      109 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/invite_user_subject.txt
--rw-r--r--   0 paltman    (501) staff       (20)       63 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/password_change_subject.txt
--rw-r--r--   0 paltman    (501) staff       (20)      343 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/password_reset.txt
--rw-r--r--   0 paltman    (501) staff       (20)      162 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/password_change.txt
--rw-r--r--   0 paltman    (501) staff       (20)      296 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 paltman    (501) staff       (20)      115 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/password_reset_subject.txt
--rw-r--r--   0 paltman    (501) staff       (20)      124 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 paltman    (501) staff       (20)      144 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/email/invite_user.txt
--rw-r--r--   0 paltman    (501) staff       (20)     1159 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/account/signup.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/calendars/
--rw-r--r--   0 paltman    (501) staff       (20)     1511 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/calendars/calendar.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/
--rw-r--r--   0 paltman    (501) staff       (20)       83 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/base.html
--rw-r--r--   0 paltman    (501) staff       (20)      580 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/message_create.html
--rw-r--r--   0 paltman    (501) staff       (20)     1241 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/thread_detail.html
--rw-r--r--   0 paltman    (501) staff       (20)     1192 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/inbox.html
--rw-r--r--   0 paltman    (501) staff       (20)      814 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/thread_confirm_delete.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/likes/
--rw-r--r--   0 paltman    (501) staff       (20)      371 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/likes/_widget_brief.html
--rw-r--r--   0 paltman    (501) staff       (20)      221 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/likes/_like.html
--rw-r--r--   0 paltman    (501) staff       (20)      462 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/likes/_widget.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/waitinglist/
--rw-r--r--   0 paltman    (501) staff       (20)      442 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/waitinglist/_list_signup.html
--rw-r--r--   0 paltman    (501) staff       (20)       86 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/waitinglist/_success.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/
--rw-r--r--   0 paltman    (501) staff       (20)      266 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_detail.html
--rw-r--r--   0 paltman    (501) staff       (20)      804 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_confirm_delete.html
--rw-r--r--   0 paltman    (501) staff       (20)       82 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/base.html
--rw-r--r--   0 paltman    (501) staff       (20)     1463 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_list.html
--rw-r--r--   0 paltman    (501) staff       (20)      971 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_form.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/
--rw-r--r--   0 paltman    (501) staff       (20)      829 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_list.html
--rw-r--r--   0 paltman    (501) staff       (20)      588 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/dateline_stale.html
--rw-r--r--   0 paltman    (501) staff       (20)      540 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/dateline.html
--rw-r--r--   0 paltman    (501) staff       (20)     2106 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_post.html
--rw-r--r--   0 paltman    (501) staff       (20)     3579 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_base.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/
--rw-r--r--   0 paltman    (501) staff       (20)      259 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/_status.html
--rw-r--r--   0 paltman    (501) staff       (20)     4150 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_detail.html
--rw-r--r--   0 paltman    (501) staff       (20)      609 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_create.html
--rw-r--r--   0 paltman    (501) staff       (20)      180 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/_members.html
--rw-r--r--   0 paltman    (501) staff       (20)     1118 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_list.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/
--rw-r--r--   0 paltman    (501) staff       (20)     1054 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_share.html
--rw-r--r--   0 paltman    (501) staff       (20)     1002 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_confirm_delete.html
--rw-r--r--   0 paltman    (501) staff       (20)      435 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_detail.html
--rw-r--r--   0 paltman    (501) staff       (20)      325 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/index.html
--rw-r--r--   0 paltman    (501) staff       (20)       85 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/base.html
--rw-r--r--   0 paltman    (501) staff       (20)      908 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/document_confirm_delete.html
--rw-r--r--   0 paltman    (501) staff       (20)     1095 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/document_create.html
--rw-r--r--   0 paltman    (501) staff       (20)      577 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/_breadcrumbs.html
--rw-r--r--   0 paltman    (501) staff       (20)     3001 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/_member_table.html
--rw-r--r--   0 paltman    (501) staff       (20)      718 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_create.html
--rw-r--r--   0 paltman    (501) staff       (20)      503 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/document_detail.html
--rw-r--r--   0 paltman    (501) staff       (20)      320 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/_usage.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/
--rw-r--r--   0 paltman    (501) staff       (20)       97 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/base.html
--rw-r--r--   0 paltman    (501) staff       (20)      101 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/short.txt
--rw-r--r--   0 paltman    (501) staff       (20)      102 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/full.txt
--rw-r--r--   0 paltman    (501) staff       (20)      313 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/email_body.txt
--rw-r--r--   0 paltman    (501) staff       (20)       84 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/email_subject.txt
--rw-r--r--   0 paltman    (501) staff       (20)     1882 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/notice_settings.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/
--rw-r--r--   0 paltman    (501) staff       (20)      904 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_create.html
--rw-r--r--   0 paltman    (501) staff       (20)       52 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_create.html
--rw-r--r--   0 paltman    (501) staff       (20)     1492 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_list.html
--rw-r--r--   0 paltman    (501) staff       (20)     1570 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_list.html
--rw-r--r--   0 paltman    (501) staff       (20)      102 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/base.html
--rw-r--r--   0 paltman    (501) staff       (20)     1155 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_update.html
--rw-r--r--   0 paltman    (501) staff       (20)       52 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_update.html
--rw-r--r--   0 paltman    (501) staff       (20)     1338 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_form.html
--rw-r--r--   0 paltman    (501) staff       (20)      359 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/invoice_list.html
--rw-r--r--   0 paltman    (501) staff       (20)      690 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_delete.html
--rw-r--r--   0 paltman    (501) staff       (20)      899 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_delete.html
--rw-r--r--   0 paltman    (501) staff       (20)       73 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/_stripe_js.html
--rw-r--r--   0 paltman    (501) staff       (20)      706 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/_invoice_table.html
-drwxr-xr-x   0 paltman    (501) staff       (20)        0 2020-02-20 21:31:27.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/
--rw-r--r--   0 paltman    (501) staff       (20)      631 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/_invited.html
--rw-r--r--   0 paltman    (501) staff       (20)      170 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/_invites_remaining.html
--rw-r--r--   0 paltman    (501) staff       (20)      708 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/_invite_form.html
--rw-r--r--   0 paltman    (501) staff       (20)      273 2020-02-20 21:14:49.000000 pinax-templates-2.0.6/pinax/templates/templates/subnav_base.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.593168 pinax-templates-3.0.0/
+-rw-r--r--   0 chris      (502) staff       (20)       53 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/AUTHORS
+-rw-r--r--   0 chris      (502) staff       (20)     1101 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/LICENSE
+-rw-r--r--   0 chris      (502) staff       (20)      139 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/MANIFEST.in
+-rw-r--r--   0 chris      (502) staff       (20)     2922 2023-04-14 16:22:54.593279 pinax-templates-3.0.0/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     5888 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/README.md
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.544764 pinax-templates-3.0.0/pinax/
+-rw-r--r--   0 chris      (502) staff       (20)       83 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.545606 pinax-templates-3.0.0/pinax/templates/
+-rw-r--r--   0 chris      (502) staff       (20)      149 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)      240 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/apps.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.538905 pinax-templates-3.0.0/pinax/templates/locale/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.538250 pinax-templates-3.0.0/pinax/templates/locale/de/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.546483 pinax-templates-3.0.0/pinax/templates/locale/de/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     9303 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris      (502) staff       (20)    17326 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.538535 pinax-templates-3.0.0/pinax/templates/locale/fr/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.547406 pinax-templates-3.0.0/pinax/templates/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     7918 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris      (502) staff       (20)    12579 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.538770 pinax-templates-3.0.0/pinax/templates/locale/ja/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.548128 pinax-templates-3.0.0/pinax/templates/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     8014 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris      (502) staff       (20)    12476 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.538998 pinax-templates-3.0.0/pinax/templates/locale/zh_CN/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.549447 pinax-templates-3.0.0/pinax/templates/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     5728 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris      (502) staff       (20)     9168 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.549932 pinax-templates-3.0.0/pinax/templates/management/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/management/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.550438 pinax-templates-3.0.0/pinax/templates/management/commands/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/management/commands/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     1117 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/management/commands/copy_templates.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.553745 pinax-templates-3.0.0/pinax/templates/templates/
+-rw-r--r--   0 chris      (502) staff       (20)      326 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/404.html
+-rw-r--r--   0 chris      (502) staff       (20)      404 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/500.html
+-rw-r--r--   0 chris      (502) staff       (20)     1034 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/_account_bar.html
+-rw-r--r--   0 chris      (502) staff       (20)      227 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/_messages.html
+-rw-r--r--   0 chris      (502) staff       (20)      133 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/_nav.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.561541 pinax-templates-3.0.0/pinax/templates/templates/account/
+-rw-r--r--   0 chris      (502) staff       (20)     1274 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/base.html
+-rw-r--r--   0 chris      (502) staff       (20)      692 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/delete.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.564797 pinax-templates-3.0.0/pinax/templates/templates/account/email/
+-rw-r--r--   0 chris      (502) staff       (20)      296 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 chris      (502) staff       (20)      124 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 chris      (502) staff       (20)      144 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/invite_user.txt
+-rw-r--r--   0 chris      (502) staff       (20)      109 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/invite_user_subject.txt
+-rw-r--r--   0 chris      (502) staff       (20)      162 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/password_change.txt
+-rw-r--r--   0 chris      (502) staff       (20)       63 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/password_change_subject.txt
+-rw-r--r--   0 chris      (502) staff       (20)      343 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/password_reset.txt
+-rw-r--r--   0 chris      (502) staff       (20)      115 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email/password_reset_subject.txt
+-rw-r--r--   0 chris      (502) staff       (20)      692 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email_confirm.html
+-rw-r--r--   0 chris      (502) staff       (20)      687 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email_confirmation_sent.html
+-rw-r--r--   0 chris      (502) staff       (20)      437 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/email_confirmed.html
+-rw-r--r--   0 chris      (502) staff       (20)     1345 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/login.html
+-rw-r--r--   0 chris      (502) staff       (20)      567 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/logout.html
+-rw-r--r--   0 chris      (502) staff       (20)      550 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/password_change.html
+-rw-r--r--   0 chris      (502) staff       (20)     1018 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/password_reset.html
+-rw-r--r--   0 chris      (502) staff       (20)     1125 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/password_reset_sent.html
+-rw-r--r--   0 chris      (502) staff       (20)      627 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/password_reset_token.html
+-rw-r--r--   0 chris      (502) staff       (20)      511 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/password_reset_token_fail.html
+-rw-r--r--   0 chris      (502) staff       (20)      503 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/settings.html
+-rw-r--r--   0 chris      (502) staff       (20)     1159 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/signup.html
+-rw-r--r--   0 chris      (502) staff       (20)      596 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/account/signup_closed.html
+-rw-r--r--   0 chris      (502) staff       (20)     2909 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/base.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.565240 pinax-templates-3.0.0/pinax/templates/templates/pagination/
+-rw-r--r--   0 chris      (502) staff       (20)     1746 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pagination/_pagination.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.541583 pinax-templates-3.0.0/pinax/templates/templates/pinax/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.567164 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/
+-rw-r--r--   0 chris      (502) staff       (20)      804 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_confirm_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)      266 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_detail.html
+-rw-r--r--   0 chris      (502) staff       (20)      971 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_form.html
+-rw-r--r--   0 chris      (502) staff       (20)     1463 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_list.html
+-rw-r--r--   0 chris      (502) staff       (20)       82 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/base.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.569188 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/
+-rw-r--r--   0 chris      (502) staff       (20)     3579 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_base.html
+-rw-r--r--   0 chris      (502) staff       (20)      829 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_list.html
+-rw-r--r--   0 chris      (502) staff       (20)     2106 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_post.html
+-rw-r--r--   0 chris      (502) staff       (20)      540 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/dateline.html
+-rw-r--r--   0 chris      (502) staff       (20)      588 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/dateline_stale.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.569577 pinax-templates-3.0.0/pinax/templates/templates/pinax/calendars/
+-rw-r--r--   0 chris      (502) staff       (20)     1511 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/calendars/calendar.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.571490 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/
+-rw-r--r--   0 chris      (502) staff       (20)      180 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/_members.html
+-rw-r--r--   0 chris      (502) staff       (20)      259 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/_status.html
+-rw-r--r--   0 chris      (502) staff       (20)      609 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_create.html
+-rw-r--r--   0 chris      (502) staff       (20)     4150 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_detail.html
+-rw-r--r--   0 chris      (502) staff       (20)     1118 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_list.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.576505 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/
+-rw-r--r--   0 chris      (502) staff       (20)      577 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/_breadcrumbs.html
+-rw-r--r--   0 chris      (502) staff       (20)     3001 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/_member_table.html
+-rw-r--r--   0 chris      (502) staff       (20)      320 2023-04-14 16:12:29.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/_usage.html
+-rw-r--r--   0 chris      (502) staff       (20)       85 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/base.html
+-rw-r--r--   0 chris      (502) staff       (20)      908 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/document_confirm_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)     1095 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/document_create.html
+-rw-r--r--   0 chris      (502) staff       (20)      503 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/document_detail.html
+-rw-r--r--   0 chris      (502) staff       (20)     1002 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_confirm_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)      718 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_create.html
+-rw-r--r--   0 chris      (502) staff       (20)      435 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_detail.html
+-rw-r--r--   0 chris      (502) staff       (20)     1054 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_share.html
+-rw-r--r--   0 chris      (502) staff       (20)      325 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/index.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.577659 pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/
+-rw-r--r--   0 chris      (502) staff       (20)      708 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/_invite_form.html
+-rw-r--r--   0 chris      (502) staff       (20)      631 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/_invited.html
+-rw-r--r--   0 chris      (502) staff       (20)      170 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/_invites_remaining.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.578838 pinax-templates-3.0.0/pinax/templates/templates/pinax/likes/
+-rw-r--r--   0 chris      (502) staff       (20)      221 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/likes/_like.html
+-rw-r--r--   0 chris      (502) staff       (20)      462 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/likes/_widget.html
+-rw-r--r--   0 chris      (502) staff       (20)      371 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/likes/_widget_brief.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.581202 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/
+-rw-r--r--   0 chris      (502) staff       (20)       83 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/base.html
+-rw-r--r--   0 chris      (502) staff       (20)     1192 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/inbox.html
+-rw-r--r--   0 chris      (502) staff       (20)      580 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/message_create.html
+-rw-r--r--   0 chris      (502) staff       (20)      814 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/thread_confirm_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)     1241 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/thread_detail.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.583595 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/
+-rw-r--r--   0 chris      (502) staff       (20)       97 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/base.html
+-rw-r--r--   0 chris      (502) staff       (20)      313 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/email_body.txt
+-rw-r--r--   0 chris      (502) staff       (20)       84 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/email_subject.txt
+-rw-r--r--   0 chris      (502) staff       (20)      102 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/full.txt
+-rw-r--r--   0 chris      (502) staff       (20)     1882 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/notice_settings.html
+-rw-r--r--   0 chris      (502) staff       (20)      101 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/short.txt
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.588508 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/
+-rw-r--r--   0 chris      (502) staff       (20)      706 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/_invoice_table.html
+-rw-r--r--   0 chris      (502) staff       (20)       73 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/_stripe_js.html
+-rw-r--r--   0 chris      (502) staff       (20)      102 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/base.html
+-rw-r--r--   0 chris      (502) staff       (20)      359 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/invoice_list.html
+-rw-r--r--   0 chris      (502) staff       (20)      904 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_create.html
+-rw-r--r--   0 chris      (502) staff       (20)      899 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)     1492 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_list.html
+-rw-r--r--   0 chris      (502) staff       (20)     1155 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_update.html
+-rw-r--r--   0 chris      (502) staff       (20)       52 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_create.html
+-rw-r--r--   0 chris      (502) staff       (20)      690 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_delete.html
+-rw-r--r--   0 chris      (502) staff       (20)     1338 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_form.html
+-rw-r--r--   0 chris      (502) staff       (20)     1570 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_list.html
+-rw-r--r--   0 chris      (502) staff       (20)       52 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_update.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.589249 pinax-templates-3.0.0/pinax/templates/templates/pinax/waitinglist/
+-rw-r--r--   0 chris      (502) staff       (20)      442 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/waitinglist/_list_signup.html
+-rw-r--r--   0 chris      (502) staff       (20)       86 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/pinax/waitinglist/_success.html
+-rw-r--r--   0 chris      (502) staff       (20)      132 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/site_base.html
+-rw-r--r--   0 chris      (502) staff       (20)      273 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/templates/subnav_base.html
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.590870 pinax-templates-3.0.0/pinax/templates/tests/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/tests/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/tests/models.py
+-rw-r--r--   0 chris      (502) staff       (20)     1219 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/tests/settings.py
+-rw-r--r--   0 chris      (502) staff       (20)       93 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/tests/tests.py
+-rw-r--r--   0 chris      (502) staff       (20)       18 2023-04-14 16:12:30.000000 pinax-templates-3.0.0/pinax/templates/tests/urls.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 16:22:54.592934 pinax-templates-3.0.0/pinax_templates.egg-info/
+-rw-r--r--   0 chris      (502) staff       (20)     2922 2023-04-14 16:22:54.000000 pinax-templates-3.0.0/pinax_templates.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     6307 2023-04-14 16:22:54.000000 pinax-templates-3.0.0/pinax_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-14 16:22:54.000000 pinax-templates-3.0.0/pinax_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-14 16:17:04.000000 pinax-templates-3.0.0/pinax_templates.egg-info/not-zip-safe
+-rw-r--r--   0 chris      (502) staff       (20)       41 2023-04-14 16:22:54.000000 pinax-templates-3.0.0/pinax_templates.egg-info/requires.txt
+-rw-r--r--   0 chris      (502) staff       (20)        6 2023-04-14 16:22:54.000000 pinax-templates-3.0.0/pinax_templates.egg-info/top_level.txt
+-rw-r--r--   0 chris      (502) staff       (20)      114 2023-04-14 16:22:54.593703 pinax-templates-3.0.0/setup.cfg
+-rw-r--r--   0 chris      (502) staff       (20)     3429 2023-04-14 16:22:42.000000 pinax-templates-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pinax-templates-2.0.6/PKG-INFO` & `pinax-templates-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pinax-templates
-Version: 2.0.6
+Version: 3.0.0
 Summary: semantic templates for pinax apps
 Home-page: http://github.com/pinax/pinax-templates/
 Author: Pinax Team
 Author-email: team@pinaxprojects.com
 License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-templates.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        ===============
-        Pinax Templates
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-templates.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-templates.svg
-            :target: https://circleci.com/gh/pinax/pinax-templates
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-templates.svg
-            :target: https://codecov.io/gh/pinax/pinax-templates
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/pulls?q=is%3Apr+is%3Aclosed
-        
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        
-        ``pinax-templates`` provides semantically-correct templates for use with Pinax apps.
-        
-        
-        Supported Pinax Apps
-        --------------------
-        
-        * django-user-accounts
-        * pinax-announcements
-        * pinax-blog
-        * pinax-cohorts
-        * pinax-documents
-        * pinax-invitations
-        * pinax-likes
-        * pinax-notifications
-        * pinax-strip
-        
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+-----+
-        | Django / Python | 2.7 | 3.4 | 3.5 | 3.6 |
-        +=================+=====+=====+=====+=====+
-        |  1.11           |  *  |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+-----+
-        |  2.0            |     |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+-----+
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-templates.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+===============
+Pinax Templates
+===============
+
+.. image:: https://img.shields.io/pypi/v/pinax-templates.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-templates.svg
+    :target: https://circleci.com/gh/pinax/pinax-templates
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-templates.svg
+    :target: https://codecov.io/gh/pinax/pinax-templates
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/pulls?q=is%3Apr+is%3Aclosed
+
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+
+``pinax-templates`` provides semantically-correct templates for use with Pinax apps.
+
+
+Supported Pinax Apps
+--------------------
+
+* django-user-accounts
+* pinax-announcements
+* pinax-blog
+* pinax-cohorts
+* pinax-documents
+* pinax-invitations
+* pinax-likes
+* pinax-notifications
+* pinax-strip
+
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+-----+
+| Django / Python | 3.2 | 3.5 | 3.6 | 4.2 |
++=================+=====+=====+=====+=====+
+|  3.2            |  *  |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
+|  4.2            |     |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
```

### Comparing `pinax-templates-2.0.6/LICENSE` & `pinax-templates-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax_templates.egg-info/PKG-INFO` & `pinax-templates-3.0.0/pinax_templates.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pinax-templates
-Version: 2.0.6
+Version: 3.0.0
 Summary: semantic templates for pinax apps
 Home-page: http://github.com/pinax/pinax-templates/
 Author: Pinax Team
 Author-email: team@pinaxprojects.com
 License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-templates.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        ===============
-        Pinax Templates
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-templates.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-templates.svg
-            :target: https://circleci.com/gh/pinax/pinax-templates
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-templates.svg
-            :target: https://codecov.io/gh/pinax/pinax-templates
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-templates.svg
-            :target: https://github.com/pinax/pinax-templates/pulls?q=is%3Apr+is%3Aclosed
-        
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://pypi.python.org/pypi/pinax-templates/
-        
-        
-        ``pinax-templates`` provides semantically-correct templates for use with Pinax apps.
-        
-        
-        Supported Pinax Apps
-        --------------------
-        
-        * django-user-accounts
-        * pinax-announcements
-        * pinax-blog
-        * pinax-cohorts
-        * pinax-documents
-        * pinax-invitations
-        * pinax-likes
-        * pinax-notifications
-        * pinax-strip
-        
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+-----+
-        | Django / Python | 2.7 | 3.4 | 3.5 | 3.6 |
-        +=================+=====+=====+=====+=====+
-        |  1.11           |  *  |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+-----+
-        |  2.0            |     |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+-----+
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-templates.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+===============
+Pinax Templates
+===============
+
+.. image:: https://img.shields.io/pypi/v/pinax-templates.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-templates.svg
+    :target: https://circleci.com/gh/pinax/pinax-templates
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-templates.svg
+    :target: https://codecov.io/gh/pinax/pinax-templates
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-templates.svg
+    :target: https://github.com/pinax/pinax-templates/pulls?q=is%3Apr+is%3Aclosed
+
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://pypi.python.org/pypi/pinax-templates/
+
+
+``pinax-templates`` provides semantically-correct templates for use with Pinax apps.
+
+
+Supported Pinax Apps
+--------------------
+
+* django-user-accounts
+* pinax-announcements
+* pinax-blog
+* pinax-cohorts
+* pinax-documents
+* pinax-invitations
+* pinax-likes
+* pinax-notifications
+* pinax-strip
+
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+-----+
+| Django / Python | 3.2 | 3.5 | 3.6 | 4.2 |
++=================+=====+=====+=====+=====+
+|  3.2            |  *  |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
+|  4.2            |     |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
```

### Comparing `pinax-templates-2.0.6/pinax_templates.egg-info/SOURCES.txt` & `pinax-templates-3.0.0/pinax_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/README.md` & `pinax-templates-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/setup.py` & `pinax-templates-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from setuptools import find_packages, setup
 
-VERSION = "2.0.6"
+VERSION = "3.0.0"
 LONG_DESCRIPTION = """
 .. image:: http://pinaxproject.com/pinax-design/patches/pinax-templates.svg
     :target: https://pypi.python.org/pypi/pinax-templates/
 
 ===============
 Pinax Templates
 ===============
@@ -53,19 +53,19 @@
 * pinax-strip
 
 
 Supported Django and Python Versions
 ------------------------------------
 
 +-----------------+-----+-----+-----+-----+
-| Django / Python | 2.7 | 3.4 | 3.5 | 3.6 |
+| Django / Python | 3.2 | 3.5 | 3.6 | 4.2 |
 +=================+=====+=====+=====+=====+
-|  1.11           |  *  |  *  |  *  |  *  |
+|  3.2            |  *  |  *  |  *  |  *  |
 +-----------------+-----+-----+-----+-----+
-|  2.0            |     |  *  |  *  |  *  |
+|  4.2            |     |  *  |  *  |  *  |
 +-----------------+-----+-----+-----+-----+
 """
 
 
 # Publish Helper.
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist bdist_wheel upload')
@@ -83,30 +83,29 @@
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.0',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=[
-        "django>=1.11",
+        "django>=3.2",
         "django-bootstrap-form>=3.0.0"
     ],
     tests_require=[
     ],
     test_suite="runtests.runtests",
     zip_safe=False
 )
```

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/ja/LC_MESSAGES/django.mo` & `pinax-templates-3.0.0/pinax/templates/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/ja/LC_MESSAGES/django.po` & `pinax-templates-3.0.0/pinax/templates/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/zh_CN/LC_MESSAGES/django.mo` & `pinax-templates-3.0.0/pinax/templates/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/zh_CN/LC_MESSAGES/django.po` & `pinax-templates-3.0.0/pinax/templates/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/de/LC_MESSAGES/django.mo` & `pinax-templates-3.0.0/pinax/templates/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/de/LC_MESSAGES/django.po` & `pinax-templates-3.0.0/pinax/templates/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/fr/LC_MESSAGES/django.mo` & `pinax-templates-3.0.0/pinax/templates/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/locale/fr/LC_MESSAGES/django.po` & `pinax-templates-3.0.0/pinax/templates/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/tests/settings.py` & `pinax-templates-3.0.0/pinax/templates/tests/settings.py`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/management/commands/copy_templates.py` & `pinax-templates-3.0.0/pinax/templates/management/commands/copy_templates.py`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pagination/_pagination.html` & `pinax-templates-3.0.0/pinax/templates/templates/pagination/_pagination.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/base.html` & `pinax-templates-3.0.0/pinax/templates/templates/base.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/_account_bar.html` & `pinax-templates-3.0.0/pinax/templates/templates/_account_bar.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/signup_closed.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/base.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/email_confirm.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/password_reset.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/password_reset_token.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/password_reset_token.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/login.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/password_reset_sent.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/password_reset_sent.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/email_confirmation_sent.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/email_confirmation_sent.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/logout.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/password_change.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/account/signup.html` & `pinax-templates-3.0.0/pinax/templates/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/calendars/calendar.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/calendars/calendar.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/message_create.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/message_create.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/thread_detail.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/thread_detail.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/inbox.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/inbox.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/messages/thread_confirm_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/messages/thread_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_confirm_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_list.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_list.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/announcements/announcement_form.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/announcements/announcement_form.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_list.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_list.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/dateline_stale.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/dateline_stale.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/dateline.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/dateline.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_post.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_post.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/blog/blog_base.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/blog/blog_base.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_detail.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_detail.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_create.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_create.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/cohorts/cohort_list.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/cohorts/cohort_list.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_share.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_share.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_confirm_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/document_confirm_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/document_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/document_create.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/document_create.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/_breadcrumbs.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/_breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/_member_table.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/_member_table.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/documents/folder_create.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/documents/folder_create.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/notifications/notice_settings.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/notifications/notice_settings.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_create.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_create.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_list.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_list.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_list.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_list.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_update.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_update.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_form.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_form.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/subscription_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/subscription_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/paymentmethod_delete.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/paymentmethod_delete.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/stripe/_invoice_table.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/stripe/_invoice_table.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/_invited.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/_invited.html`

 * *Files identical despite different names*

### Comparing `pinax-templates-2.0.6/pinax/templates/templates/pinax/invitations/_invite_form.html` & `pinax-templates-3.0.0/pinax/templates/templates/pinax/invitations/_invite_form.html`

 * *Files identical despite different names*

