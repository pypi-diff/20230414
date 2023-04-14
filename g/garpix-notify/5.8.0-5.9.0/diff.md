# Comparing `tmp/garpix_notify-5.8.0.tar.gz` & `tmp/garpix_notify-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_notify-5.8.0.tar", last modified: Wed Jun 29 07:24:59 2022, max compression
+gzip compressed data, was "garpix_notify-5.9.0.tar", last modified: Thu Jun 30 15:44:01 2022, max compression
```

## Comparing `garpix_notify-5.8.0.tar` & `garpix_notify-5.9.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.287263 garpix_notify-5.8.0/
--rw-r--r--   0 crusat     (501) staff       (20)       78 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     8283 2022-06-29 07:24:59.287025 garpix_notify-5.8.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.266008 garpix_notify-5.8.0/garpix_notify/
--rw-r--r--   0 crusat     (501) staff       (20)       78 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     7579 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/README.md
--rw-r--r--   0 crusat     (501) staff       (20)     6205 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/README.rst
--rw-r--r--   0 crusat     (501) staff       (20)       55 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.267194 garpix_notify-5.8.0/garpix_notify/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      215 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      435 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1332 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1085 2021-08-12 15:39:06.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/smtp.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1616 2022-03-17 07:28:41.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/tasks.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     6275 2022-05-19 08:43:05.000000 garpix_notify-5.8.0/garpix_notify/__pycache__/tests.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.268282 garpix_notify-5.8.0/garpix_notify/admin/
--rw-r--r--   0 crusat     (501) staff       (20)      365 2022-05-19 08:35:29.000000 garpix_notify-5.8.0/garpix_notify/admin/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.269306 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      548 2022-05-19 08:35:33.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      552 2022-05-19 08:35:33.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/category.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1676 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      543 2021-08-12 15:25:12.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/fcm.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      526 2021-08-12 15:25:12.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/file.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      872 2021-08-12 15:25:12.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/log.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1164 2022-05-19 07:01:32.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/notify.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      878 2021-08-12 15:25:12.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/smtp.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1996 2022-05-19 08:35:33.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/template.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      974 2022-05-19 07:01:32.000000 garpix_notify-5.8.0/garpix_notify/admin/__pycache__/user_list.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      250 2022-05-19 08:35:29.000000 garpix_notify-5.8.0/garpix_notify/admin/category.py
--rw-r--r--   0 crusat     (501) staff       (20)     1615 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/admin/config.py
--rw-r--r--   0 crusat     (501) staff       (20)      229 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/admin/fcm.py
--rw-r--r--   0 crusat     (501) staff       (20)      221 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/admin/file.py
--rw-r--r--   0 crusat     (501) staff       (20)      401 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/admin/log.py
--rw-r--r--   0 crusat     (501) staff       (20)      815 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/admin/notify.py
--rw-r--r--   0 crusat     (501) staff       (20)      529 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/admin/smtp.py
--rw-r--r--   0 crusat     (501) staff       (20)     2012 2022-05-19 08:35:29.000000 garpix_notify-5.8.0/garpix_notify/admin/template.py
--rw-r--r--   0 crusat     (501) staff       (20)      617 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/admin/user_list.py
--rw-r--r--   0 crusat     (501) staff       (20)        0 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/admin/user_list_participant.py
--rw-r--r--   0 crusat     (501) staff       (20)      138 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/apps.py
--rw-r--r--   0 crusat     (501) staff       (20)      769 2021-10-29 07:00:59.000000 garpix_notify-5.8.0/garpix_notify/consumers.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.269409 garpix_notify-5.8.0/garpix_notify/management/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-02 16:04:58.000000 garpix_notify-5.8.0/garpix_notify/management/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.273005 garpix_notify-5.8.0/garpix_notify/management/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      172 2021-09-02 16:10:06.000000 garpix_notify-5.8.0/garpix_notify/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.273252 garpix_notify-5.8.0/garpix_notify/management/commands/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-02 16:05:13.000000 garpix_notify-5.8.0/garpix_notify/management/commands/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.273481 garpix_notify-5.8.0/garpix_notify/management/commands/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      181 2021-09-02 16:10:27.000000 garpix_notify-5.8.0/garpix_notify/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2210 2021-09-02 16:29:54.000000 garpix_notify-5.8.0/garpix_notify/management/commands/__pycache__/garpix_notify_telegram.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1797 2021-09-02 16:29:34.000000 garpix_notify-5.8.0/garpix_notify/management/commands/garpix_notify_telegram.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.273914 garpix_notify-5.8.0/garpix_notify/mixins/
--rw-r--r--   0 crusat     (501) staff       (20)       85 2022-05-19 14:03:26.000000 garpix_notify-5.8.0/garpix_notify/mixins/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.274332 garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      273 2022-05-19 14:04:00.000000 garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      537 2022-05-19 14:04:00.000000 garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/notify_mixin.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1973 2021-09-02 15:58:20.000000 garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/user_notify_mixin.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      105 2022-05-19 11:37:43.000000 garpix_notify-5.8.0/garpix_notify/mixins/notify_mixin.py
--rw-r--r--   0 crusat     (501) staff       (20)     1767 2021-09-02 15:58:18.000000 garpix_notify-5.8.0/garpix_notify/mixins/user_notify_mixin.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.275835 garpix_notify-5.8.0/garpix_notify/models/
--rw-r--r--   0 crusat     (501) staff       (20)      354 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/models/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.281533 garpix_notify-5.8.0/garpix_notify/models/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      622 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1004 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/category.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1618 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/choices.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     7607 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      785 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/fcm.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      975 2022-05-19 08:35:33.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/file.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1167 2022-06-01 11:52:55.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/log.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)    12855 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/notify.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3841 2022-05-19 07:01:32.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/smtp.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3941 2022-05-19 07:01:32.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/template.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1372 2022-05-19 07:01:31.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/user_list.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1771 2022-05-19 07:01:32.000000 garpix_notify-5.8.0/garpix_notify/models/__pycache__/user_list_participant.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      489 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/models/category.py
--rw-r--r--   0 crusat     (501) staff       (20)     1134 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/models/choices.py
--rw-r--r--   0 crusat     (501) staff       (20)    10254 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/models/config.py
--rw-r--r--   0 crusat     (501) staff       (20)      360 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/models/fcm.py
--rw-r--r--   0 crusat     (501) staff       (20)      478 2022-05-19 08:35:29.000000 garpix_notify-5.8.0/garpix_notify/models/file.py
--rw-r--r--   0 crusat     (501) staff       (20)      666 2022-06-01 11:46:17.000000 garpix_notify-5.8.0/garpix_notify/models/log.py
--rw-r--r--   0 crusat     (501) staff       (20)    19459 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/models/notify.py
--rw-r--r--   0 crusat     (501) staff       (20)     4286 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/models/smtp.py
--rw-r--r--   0 crusat     (501) staff       (20)     3365 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/models/template.py
--rw-r--r--   0 crusat     (501) staff       (20)      854 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/models/user_list.py
--rw-r--r--   0 crusat     (501) staff       (20)     1322 2022-05-19 07:00:29.000000 garpix_notify-5.8.0/garpix_notify/models/user_list_participant.py
--rw-r--r--   0 crusat     (501) staff       (20)      158 2021-10-29 07:00:59.000000 garpix_notify-5.8.0/garpix_notify/routing.py
--rw-r--r--   0 crusat     (501) staff       (20)     1211 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/settings.py
--rw-r--r--   0 crusat     (501) staff       (20)     1586 2022-06-29 07:24:56.000000 garpix_notify-5.8.0/garpix_notify/setup.py
--rw-r--r--   0 crusat     (501) staff       (20)      799 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/smtp.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.281682 garpix_notify-5.8.0/garpix_notify/static/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2022-04-01 16:06:35.000000 garpix_notify-5.8.0/garpix_notify/static/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.281798 garpix_notify-5.8.0/garpix_notify/static/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      168 2022-04-02 07:50:41.000000 garpix_notify-5.8.0/garpix_notify/static/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.264102 garpix_notify-5.8.0/garpix_notify/static/css/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.284143 garpix_notify-5.8.0/garpix_notify/static/css/admin/
--rw-r--r--   0 crusat     (501) staff       (20)       34 2022-04-01 16:06:35.000000 garpix_notify-5.8.0/garpix_notify/static/css/admin/garpix_notify.css
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.264201 garpix_notify-5.8.0/garpix_notify/static/js/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.284305 garpix_notify-5.8.0/garpix_notify/static/js/admin/
--rw-r--r--   0 crusat     (501) staff       (20)     2466 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/static/js/admin/garpix_notify.js
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.284592 garpix_notify-5.8.0/garpix_notify/tasks/
--rw-r--r--   0 crusat     (501) staff       (20)       21 2022-05-30 15:37:12.000000 garpix_notify-5.8.0/garpix_notify/tasks/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.284844 garpix_notify-5.8.0/garpix_notify/tasks/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      167 2022-05-19 07:01:33.000000 garpix_notify-5.8.0/garpix_notify/tasks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1674 2022-05-19 08:37:40.000000 garpix_notify-5.8.0/garpix_notify/tasks/__pycache__/tasks.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1791 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/tasks/tasks.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.284984 garpix_notify-5.8.0/garpix_notify/templates/
--rw-r--r--   0 crusat     (501) staff       (20)      258 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/templates/send_notify.html
--rw-r--r--   0 crusat     (501) staff       (20)    11259 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/tests.py
--rw-r--r--   0 crusat     (501) staff       (20)      244 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/urls.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.285885 garpix_notify-5.8.0/garpix_notify/utils/
--rw-r--r--   0 crusat     (501) staff       (20)      184 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.286783 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      401 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2771 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/call_code_cheker.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      711 2021-08-12 15:25:11.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/file.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2813 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/operators_data.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1206 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/receiving.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      624 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/send_data.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2986 2022-06-29 07:23:36.000000 garpix_notify-5.8.0/garpix_notify/utils/__pycache__/sms_checker.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3492 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/call_code_cheker.py
--rw-r--r--   0 crusat     (501) staff       (20)      489 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/utils/file.py
--rw-r--r--   0 crusat     (501) staff       (20)     4474 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/operators_data.py
--rw-r--r--   0 crusat     (501) staff       (20)     2284 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/receiving.py
--rw-r--r--   0 crusat     (501) staff       (20)      648 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/send_data.py
--rw-r--r--   0 crusat     (501) staff       (20)     5410 2022-06-29 07:21:52.000000 garpix_notify-5.8.0/garpix_notify/utils/sms_checker.py
--rw-r--r--   0 crusat     (501) staff       (20)     3945 2021-08-12 15:20:06.000000 garpix_notify-5.8.0/garpix_notify/views.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 07:24:59.266600 garpix_notify-5.8.0/garpix_notify.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     8283 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)     4482 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)      252 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       14 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/garpix_notify.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2022-06-29 07:24:59.287311 garpix_notify-5.8.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1586 2022-06-29 07:24:59.000000 garpix_notify-5.8.0/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.667487 garpix_notify-5.9.0/
+-rw-r--r--   0 crusat     (501) staff       (20)       78 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     8283 2022-06-30 15:44:01.667309 garpix_notify-5.9.0/PKG-INFO
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.650050 garpix_notify-5.9.0/garpix_notify/
+-rw-r--r--   0 crusat     (501) staff       (20)       78 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     7579 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/README.md
+-rw-r--r--   0 crusat     (501) staff       (20)     6205 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/README.rst
+-rw-r--r--   0 crusat     (501) staff       (20)       55 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.651289 garpix_notify-5.9.0/garpix_notify/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      215 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      435 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1332 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1085 2021-08-12 15:39:06.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/smtp.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1616 2022-03-17 07:28:41.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/tasks.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     6053 2022-06-29 07:28:02.000000 garpix_notify-5.9.0/garpix_notify/__pycache__/tests.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.656653 garpix_notify-5.9.0/garpix_notify/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)      365 2022-05-19 08:35:29.000000 garpix_notify-5.9.0/garpix_notify/admin/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.659553 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      548 2022-05-19 08:35:33.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      552 2022-05-19 08:35:33.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/category.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1676 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      543 2021-08-12 15:25:12.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/fcm.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      526 2021-08-12 15:25:12.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/file.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      872 2021-08-12 15:25:12.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1164 2022-05-19 07:01:32.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/notify.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      878 2021-08-12 15:25:12.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/smtp.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1996 2022-05-19 08:35:33.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      974 2022-05-19 07:01:32.000000 garpix_notify-5.9.0/garpix_notify/admin/__pycache__/user_list.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      250 2022-05-19 08:35:29.000000 garpix_notify-5.9.0/garpix_notify/admin/category.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1615 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/admin/config.py
+-rw-r--r--   0 crusat     (501) staff       (20)      229 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/admin/fcm.py
+-rw-r--r--   0 crusat     (501) staff       (20)      221 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/admin/file.py
+-rw-r--r--   0 crusat     (501) staff       (20)      401 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/admin/log.py
+-rw-r--r--   0 crusat     (501) staff       (20)      815 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/admin/notify.py
+-rw-r--r--   0 crusat     (501) staff       (20)      529 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/admin/smtp.py
+-rw-r--r--   0 crusat     (501) staff       (20)     2012 2022-05-19 08:35:29.000000 garpix_notify-5.9.0/garpix_notify/admin/template.py
+-rw-r--r--   0 crusat     (501) staff       (20)      617 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/admin/user_list.py
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/admin/user_list_participant.py
+-rw-r--r--   0 crusat     (501) staff       (20)      138 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/apps.py
+-rw-r--r--   0 crusat     (501) staff       (20)      769 2021-10-29 07:00:59.000000 garpix_notify-5.9.0/garpix_notify/consumers.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.659679 garpix_notify-5.9.0/garpix_notify/management/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-02 16:04:58.000000 garpix_notify-5.9.0/garpix_notify/management/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.659781 garpix_notify-5.9.0/garpix_notify/management/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      172 2021-09-02 16:10:06.000000 garpix_notify-5.9.0/garpix_notify/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.659991 garpix_notify-5.9.0/garpix_notify/management/commands/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-02 16:05:13.000000 garpix_notify-5.9.0/garpix_notify/management/commands/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.660220 garpix_notify-5.9.0/garpix_notify/management/commands/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      181 2021-09-02 16:10:27.000000 garpix_notify-5.9.0/garpix_notify/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2210 2021-09-02 16:29:54.000000 garpix_notify-5.9.0/garpix_notify/management/commands/__pycache__/garpix_notify_telegram.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1797 2021-09-02 16:29:34.000000 garpix_notify-5.9.0/garpix_notify/management/commands/garpix_notify_telegram.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.660575 garpix_notify-5.9.0/garpix_notify/mixins/
+-rw-r--r--   0 crusat     (501) staff       (20)       85 2022-05-19 14:03:26.000000 garpix_notify-5.9.0/garpix_notify/mixins/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.660897 garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      273 2022-05-19 14:04:00.000000 garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      537 2022-05-19 14:04:00.000000 garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/notify_mixin.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1973 2021-09-02 15:58:20.000000 garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/user_notify_mixin.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      105 2022-05-19 11:37:43.000000 garpix_notify-5.9.0/garpix_notify/mixins/notify_mixin.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1767 2021-09-02 15:58:18.000000 garpix_notify-5.9.0/garpix_notify/mixins/user_notify_mixin.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.662552 garpix_notify-5.9.0/garpix_notify/models/
+-rw-r--r--   0 crusat     (501) staff       (20)      354 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/models/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664131 garpix_notify-5.9.0/garpix_notify/models/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      622 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1004 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/category.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1618 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/choices.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     7607 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      785 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/fcm.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      975 2022-05-19 08:35:33.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/file.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1167 2022-06-01 11:52:55.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)    12855 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/notify.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     3841 2022-05-19 07:01:32.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/smtp.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     3941 2022-05-19 07:01:32.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/template.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1372 2022-05-19 07:01:31.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/user_list.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1771 2022-05-19 07:01:32.000000 garpix_notify-5.9.0/garpix_notify/models/__pycache__/user_list_participant.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      489 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/models/category.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1134 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/models/choices.py
+-rw-r--r--   0 crusat     (501) staff       (20)    10254 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/models/config.py
+-rw-r--r--   0 crusat     (501) staff       (20)      360 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/models/fcm.py
+-rw-r--r--   0 crusat     (501) staff       (20)      478 2022-05-19 08:35:29.000000 garpix_notify-5.9.0/garpix_notify/models/file.py
+-rw-r--r--   0 crusat     (501) staff       (20)      666 2022-06-01 11:46:17.000000 garpix_notify-5.9.0/garpix_notify/models/log.py
+-rw-r--r--   0 crusat     (501) staff       (20)    19459 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/models/notify.py
+-rw-r--r--   0 crusat     (501) staff       (20)     4286 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/models/smtp.py
+-rw-r--r--   0 crusat     (501) staff       (20)     3365 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/models/template.py
+-rw-r--r--   0 crusat     (501) staff       (20)      854 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/models/user_list.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1322 2022-05-19 07:00:29.000000 garpix_notify-5.9.0/garpix_notify/models/user_list_participant.py
+-rw-r--r--   0 crusat     (501) staff       (20)      158 2021-10-29 07:00:59.000000 garpix_notify-5.9.0/garpix_notify/routing.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1211 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/settings.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1585 2022-06-30 15:43:44.000000 garpix_notify-5.9.0/garpix_notify/setup.py
+-rw-r--r--   0 crusat     (501) staff       (20)      799 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/smtp.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664260 garpix_notify-5.9.0/garpix_notify/static/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2022-04-01 16:06:35.000000 garpix_notify-5.9.0/garpix_notify/static/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664369 garpix_notify-5.9.0/garpix_notify/static/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      168 2022-04-02 07:50:41.000000 garpix_notify-5.9.0/garpix_notify/static/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.648126 garpix_notify-5.9.0/garpix_notify/static/css/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664501 garpix_notify-5.9.0/garpix_notify/static/css/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)       34 2022-04-01 16:06:35.000000 garpix_notify-5.9.0/garpix_notify/static/css/admin/garpix_notify.css
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.648221 garpix_notify-5.9.0/garpix_notify/static/js/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664678 garpix_notify-5.9.0/garpix_notify/static/js/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)     2466 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/static/js/admin/garpix_notify.js
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.664966 garpix_notify-5.9.0/garpix_notify/tasks/
+-rw-r--r--   0 crusat     (501) staff       (20)       21 2022-05-30 15:37:12.000000 garpix_notify-5.9.0/garpix_notify/tasks/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.665259 garpix_notify-5.9.0/garpix_notify/tasks/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      189 2022-06-29 07:28:02.000000 garpix_notify-5.9.0/garpix_notify/tasks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1786 2022-06-29 07:28:02.000000 garpix_notify-5.9.0/garpix_notify/tasks/__pycache__/tasks.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1791 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/tasks/tasks.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.665394 garpix_notify-5.9.0/garpix_notify/templates/
+-rw-r--r--   0 crusat     (501) staff       (20)      258 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/templates/send_notify.html
+-rw-r--r--   0 crusat     (501) staff       (20)    11259 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/tests.py
+-rw-r--r--   0 crusat     (501) staff       (20)      244 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/urls.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.666283 garpix_notify-5.9.0/garpix_notify/utils/
+-rw-r--r--   0 crusat     (501) staff       (20)      184 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.667108 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      401 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2771 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/call_code_cheker.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      711 2021-08-12 15:25:11.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/file.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2813 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/operators_data.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1206 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/receiving.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      624 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/send_data.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2986 2022-06-29 07:23:36.000000 garpix_notify-5.9.0/garpix_notify/utils/__pycache__/sms_checker.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     3492 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/call_code_cheker.py
+-rw-r--r--   0 crusat     (501) staff       (20)      489 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/utils/file.py
+-rw-r--r--   0 crusat     (501) staff       (20)     4474 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/operators_data.py
+-rw-r--r--   0 crusat     (501) staff       (20)     2284 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/receiving.py
+-rw-r--r--   0 crusat     (501) staff       (20)      648 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/send_data.py
+-rw-r--r--   0 crusat     (501) staff       (20)     5410 2022-06-29 07:21:52.000000 garpix_notify-5.9.0/garpix_notify/utils/sms_checker.py
+-rw-r--r--   0 crusat     (501) staff       (20)     3945 2021-08-12 15:20:06.000000 garpix_notify-5.9.0/garpix_notify/views.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-30 15:44:01.650662 garpix_notify-5.9.0/garpix_notify.egg-info/
+-rw-r--r--   0 crusat     (501) staff       (20)     8283 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/PKG-INFO
+-rw-r--r--   0 crusat     (501) staff       (20)     4482 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/not-zip-safe
+-rw-r--r--   0 crusat     (501) staff       (20)      251 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/requires.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       14 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/garpix_notify.egg-info/top_level.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       38 2022-06-30 15:44:01.667534 garpix_notify-5.9.0/setup.cfg
+-rw-r--r--   0 crusat     (501) staff       (20)     1585 2022-06-30 15:44:01.000000 garpix_notify-5.9.0/setup.py
```

### Comparing `garpix_notify-5.8.0/PKG-INFO` & `garpix_notify-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_notify
-Version: 5.8.0
+Version: 5.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/garpixcms/garpix_notify
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `garpix_notify-5.8.0/garpix_notify/README.md` & `garpix_notify-5.9.0/garpix_notify/README.md`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/README.rst` & `garpix_notify-5.9.0/garpix_notify/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/__pycache__/settings.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/__pycache__/smtp.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/__pycache__/smtp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/__pycache__/tasks.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/__pycache__/tasks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/__pycache__/tests.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/__pycache__/tests.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May 19 08:43:02 2022 UTC, .py size: 11515 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1603 8662 fb2c 0000  U..........b.,..
+00000000: 550d 0d0a 0000 0000 90fd bb62 fb2b 0000  U..........b.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
@@ -28,366 +28,352 @@
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0300 0000 0000 0000 7334 0000 0065 005a  ........s4...e.Z
 000001d0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
 000001e0: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
 000001f0: 0564 0764 0884 005a 0687 0004 005a 0753  .d.d...Z.....Z.S
 00000200: 0029 09da 1050 7265 4275 696c 6454 6573  .)...PreBuildTes
 00000210: 7443 6173 6563 0100 0000 0000 0000 0000  tCasec..........
-00000220: 0000 0100 0000 0700 0000 0300 0000 73c8  ..............s.
+00000220: 0000 0100 0000 0700 0000 0300 0000 73ba  ..............s.
 00000230: 0000 0064 017c 005f 0064 027c 005f 0164  ...d.|._.d.|._.d
 00000240: 037c 005f 0264 0474 0364 0564 068d 0117  .|._.d.t.d.d....
 00000250: 0064 0764 0864 0964 0a64 0b9c 057c 005f  .d.d.d.d.d...|._
 00000260: 0464 0c64 0d64 0e64 0f74 056a 067c 006a  .d.d.d.d.t.j.|.j
 00000270: 0064 109c 067c 005f 0764 1174 0364 0564  .d...|._.d.t.d.d
 00000280: 068d 0117 0064 1264 139c 027c 005f 0864  .....d.d...|._.d
 00000290: 147c 005f 0964 157c 006a 0464 1619 009b  .|._.d.|.j.d....
 000002a0: 009d 0264 177c 006a 0464 1619 009b 0064  ...d.|.j.d.....d
 000002b0: 187c 006a 099b 009d 0464 197c 006a 0464  .|.j.....d.|.j.d
 000002c0: 1619 009b 0064 187c 006a 099b 009d 0474  .....d.|.j.....t
 000002d0: 056a 067c 006a 0064 1a9c 057c 005f 0a74  .j.|.j.d...|._.t
-000002e0: 0b6a 0ca0 0da1 00a0 0ea1 0001 0074 0f83  .j...........t..
-000002f0: 00a0 10a1 0001 0064 0053 0029 1b4e 7201  .......d.S.).Nr.
-00000300: 0000 00e9 0100 0000 e902 0000 005a 0a65  .............Z.e
-00000310: 6d61 696c 5f74 6573 74e9 0400 0000 a901  mail_test.......
-00000320: da06 6c65 6e67 7468 fa0f 7465 7374 4067  ..length..test@g
-00000330: 6172 7069 782e 636f 6dda 0942 6c61 426c  arpix.com..BlaBl
-00000340: 6131 3233 5a04 4976 616e 5a06 4976 616e  a123Z.IvanZ.Ivan
-00000350: 6f76 2905 da08 7573 6572 6e61 6d65 da05  ov)...username..
-00000360: 656d 6169 6cda 0870 6173 7377 6f72 64da  email..password.
-00000370: 0a66 6972 7374 5f6e 616d 65da 096c 6173  .first_name..las
-00000380: 745f 6e61 6d65 f521 0000 00d0 a2d0 b5d1  t_name.!........
-00000390: 81d1 82d0 bed0 b2d1 8bd0 b920 d182 d0b5  ........... ....
-000003a0: d0bc d0bf d0bb d0b5 d0b9 d182 f530 0000  .............0..
-000003b0: 00d0 a2d0 b5d1 81d1 82d0 bed0 b2d1 8bd0  ................
-000003c0: b920 d182 d0b5 d0bc d0bf d0bb d0b5 d0b9  . ..............
-000003d0: d182 207b 7b75 7365 722e 656d 6169 6c7d  .. {{user.email}
-000003e0: 7df5 3f00 0000 d09a d0be d0bd d182 d0b5  }.?.............
-000003f0: d0bd d182 20d1 82d0 b5d0 bad1 81d1 82d0  .... ...........
-00000400: bed0 b2d1 8bd0 b920 7b7b 7573 6572 2e65  ....... {{user.e
-00000410: 6d61 696c 7d7d 202d 207b 7b73 6f6d 6574  mail}} - {{somet
-00000420: 6578 747d 7df5 3100 0000 d09a d0be d0bd  ext}}.1.........
-00000430: d182 d0b5 d0bd d182 2048 544d 4c20 7b7b  ........ HTML {{
-00000440: 7573 6572 2e65 6d61 696c 7d7d 202d 207b  user.email}} - {
-00000450: 7b73 6f6d 6574 6578 747d 7da9 06da 0574  {sometext}}....t
-00000460: 6974 6c65 da07 7375 626a 6563 74da 0474  itle..subject..t
-00000470: 6578 74da 0468 746d 6cda 0474 7970 65da  ext..html..type.
-00000480: 0565 7665 6e74 7524 0000 00d0 9ed1 81d0  .eventu$........
-00000490: bdd0 bed0 b2d0 bdd0 b0d1 8f20 d0ba d0b0  ........... ....
-000004a0: d182 d0b5 d0b3 d0be d180 d0b8 d18f 5f7a  .............._z
-000004b0: 133c 6469 763e 7b7b 7465 7874 7d7d 3c2f  .<div>{{text}}</
-000004c0: 6469 763e 2902 721f 0000 00da 0874 656d  div>).r......tem
-000004d0: 706c 6174 657a 0762 6c61 2062 6c61 f522  platez.bla bla."
-000004e0: 0000 00d0 a2d0 b5d1 81d1 82d0 bed0 b2d1  ................
-000004f0: 8bd0 b920 d182 d0b5 d0bc d0bf d0bb d0b5  ... ............
-00000500: d0b9 d182 2072 1600 0000 f522 0000 00d0  .... r....."....
-00000510: 9ad0 bed0 bdd1 82d0 b5d0 bdd1 8220 d182  ............. ..
-00000520: d0b5 d0ba d181 d182 d0be d0b2 d18b d0b9  ................
-00000530: 20fa 0320 2d20 f514 0000 00d0 9ad0 bed0   .. - ..........
-00000540: bdd1 82d0 b5d0 bdd1 8220 4854 4d4c 20a9  ......... HTML .
-00000550: 0572 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000560: 7223 0000 0072 2400 0000 2911 da0f 5041  r#...r$...)...PA
-00000570: 5353 5f54 4553 545f 4556 454e 54da 1150  SS_TEST_EVENT..P
-00000580: 4153 535f 5445 5354 5f45 5645 4e54 5f31  ASS_TEST_EVENT_1
-00000590: da11 5041 5353 5f54 4553 545f 4556 454e  ..PASS_TEST_EVEN
-000005a0: 545f 3272 0200 0000 da09 6461 7461 5f75  T_2r......data_u
-000005b0: 7365 7272 0b00 0000 da05 454d 4149 4cda  serr......EMAIL.
-000005c0: 1364 6174 615f 7465 6d70 6c61 7465 5f65  .data_template_e
-000005d0: 6d61 696c da0d 6461 7461 5f63 6174 6567  mail..data_categ
-000005e0: 6f72 79da 0873 6f6d 6574 6578 74da 1364  ory..sometext..d
-000005f0: 6174 615f 636f 6d70 696c 6564 5f65 6d61  ata_compiled_ema
-00000600: 696c 7206 0000 00da 076f 626a 6563 7473  ilr......objects
-00000610: da03 616c 6cda 0664 656c 6574 65da 0573  ..all..delete..s
-00000620: 7570 6572 da05 7365 7455 7029 01da 0473  uper..setUp)...s
-00000630: 656c 66a9 01da 095f 5f63 6c61 7373 5f5f  elf....__class__
-00000640: a900 fa43 2f55 7365 7273 2f63 7275 7361  ...C/Users/crusa
-00000650: 742f 7072 6f6a 6563 7473 2f67 6172 7069  t/projects/garpi
-00000660: 785f 6e6f 7469 6679 2f62 6163 6b65 6e64  x_notify/backend
-00000670: 2f67 6172 7069 785f 6e6f 7469 6679 2f74  /garpix_notify/t
-00000680: 6573 7473 2e70 7972 3800 0000 1600 0000  ests.pyr8.......
-00000690: 7338 0000 0000 0206 0106 0106 030c 0102  s8..............
-000006a0: 0102 0102 0102 fb08 0902 0102 0102 0102  ................
-000006b0: 0104 0104 fa08 090c 0102 fe08 0406 020e  ................
-000006c0: 0116 0116 0104 0104 fb08 070e 017a 1650  .............z.P
-000006d0: 7265 4275 696c 6454 6573 7443 6173 652e  reBuildTestCase.
-000006e0: 7365 7455 7063 0100 0000 0000 0000 0000  setUpc..........
-000006f0: 0000 0600 0000 0500 0000 4300 0000 73c4  ..........C...s.
-00000700: 0100 0074 006a 01a0 02a1 00a0 03a1 0001  ...t.j..........
-00000710: 0074 0483 007d 017c 016a 016a 0566 007c  .t...}.|.j.j.f.|
-00000720: 006a 068e 017d 0274 076a 016a 0866 007c  .j...}.t.j.j.f.|
-00000730: 006a 098e 017d 0374 076a 016a 0a7c 036a  .j...}.t.j.j.|.j
-00000740: 0b64 018d 017d 037c 00a0 0c7c 036a 0d7c  .d...}.|...|.j.|
-00000750: 006a 0964 0219 00a1 0201 007c 00a0 0c7c  .j.d.......|...|
-00000760: 036a 0e7c 006a 0964 0319 00a1 0201 0074  .j.|.j.d.......t
-00000770: 0f6a 016a 0866 0064 047c 0369 017c 006a  .j.j.f.d.|.i.|.j
-00000780: 1097 028e 017d 0474 0f6a 016a 0a7c 046a  .....}.t.j.j.|.j
-00000790: 0b64 018d 017d 047c 00a0 0c7c 046a 0d7c  .d...}.|...|.j.|
-000007a0: 006a 1064 0219 00a1 0201 007c 00a0 0c7c  .j.d.......|...|
-000007b0: 046a 117c 006a 1064 0519 00a1 0201 007c  .j.|.j.d.......|
-000007c0: 00a0 0c7c 046a 127c 006a 1064 0619 00a1  ...|.j.|.j.d....
-000007d0: 0201 007c 00a0 0c7c 046a 137c 006a 1064  ...|...|.j.|.j.d
-000007e0: 0719 00a1 0201 007c 00a0 0c7c 046a 147c  .......|...|.j.|
-000007f0: 006a 1064 0819 00a1 0201 007c 00a0 0c7c  .j.d.......|...|
-00000800: 046a 157c 006a 1064 0919 00a1 0201 007c  .j.|.j.d.......|
-00000810: 00a0 0c7c 046a 166a 177c 036a 17a1 0201  ...|.j.j.|.j....
-00000820: 0074 006a 187c 006a 197c 006a 1a7c 0264  .t.j.|.j.|.j.|.d
-00000830: 0a9c 027c 0264 0b8d 0301 007c 00a0 0c74  ...|.d.....|...t
-00000840: 006a 01a0 02a1 00a0 1ba1 0064 0ca1 0201  .j.........d....
-00000850: 0074 006a 01a0 02a1 00a0 1ca1 007d 057c  .t.j.........}.|
-00000860: 00a0 0c7c 056a 117c 006a 1d64 0519 00a1  ...|.j.|.j.d....
-00000870: 0201 007c 00a0 0c7c 056a 127c 006a 1d64  ...|...|.j.|.j.d
-00000880: 0619 00a1 0201 007c 00a0 0c7c 056a 137c  .......|...|.j.|
-00000890: 006a 1d64 0719 00a1 0201 007c 00a0 0c7c  .j.d.......|...|
-000008a0: 056a 147c 006a 1d64 0819 00a1 0201 007c  .j.|.j.d.......|
-000008b0: 00a0 0c7c 056a 157c 006a 1d64 0919 00a1  ...|.j.|.j.d....
-000008c0: 0201 0064 0053 0029 0d4e a901 da02 706b  ...d.S.).N....pk
-000008d0: 721f 0000 0072 2500 0000 da08 6361 7465  r....r%.....cate
-000008e0: 676f 7279 7220 0000 0072 2100 0000 7222  goryr ...r!...r"
-000008f0: 0000 0072 2300 0000 7224 0000 00a9 0272  ...r#...r$.....r
-00000900: 3200 0000 da04 7573 6572 a901 7242 0000  2.....user..rB..
-00000910: 0072 0e00 0000 291e 7206 0000 0072 3400  .r....).r....r4.
-00000920: 0000 7235 0000 0072 3600 0000 7204 0000  ..r5...r6...r...
-00000930: 00da 0b63 7265 6174 655f 7573 6572 722e  ...create_userr.
-00000940: 0000 0072 0700 0000 da06 6372 6561 7465  ...r......create
-00000950: 7231 0000 00da 0367 6574 723f 0000 00da  r1.....getr?....
-00000960: 0b61 7373 6572 7445 7175 616c 721f 0000  .assertEqualr...
-00000970: 0072 2500 0000 7208 0000 0072 3000 0000  .r%...r....r0...
-00000980: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00000990: 2300 0000 7224 0000 0072 4000 0000 da02  #...r$...r@.....
-000009a0: 6964 da04 7365 6e64 722b 0000 0072 3200  id..sendr+...r2.
-000009b0: 0000 da05 636f 756e 74da 0566 6972 7374  ....count..first
-000009c0: 7233 0000 0029 0672 3900 0000 da04 5573  r3...).r9.....Us
-000009d0: 6572 7242 0000 0072 4000 0000 da0e 7465  errB...r@.....te
-000009e0: 6d70 6c61 7465 5f65 6d61 696c da06 6e6f  mplate_email..no
-000009f0: 7469 6679 723c 0000 0072 3c00 0000 723d  tifyr<...r<...r=
-00000a00: 0000 00da 1a74 6573 745f 6e6f 7469 6679  .....test_notify
-00000a10: 5f65 6d61 696c 5f70 6f73 6974 6976 653b  _email_positive;
-00000a20: 0000 0073 3a00 0000 0001 0e02 0601 1002  ...s:...........
-00000a30: 1001 1001 1401 1402 1801 1001 1401 1401  ................
-00000a40: 1401 1401 1401 1401 1202 0801 0401 02fe  ................
-00000a50: 0403 02fd 0604 1601 0e01 1401 1401 1401  ................
-00000a60: 1401 7a2b 5072 6542 7569 6c64 5465 7374  ..z+PreBuildTest
-00000a70: 4361 7365 2e74 6573 745f 6e6f 7469 6679  Case.test_notify
-00000a80: 5f65 6d61 696c 5f70 6f73 6974 6976 6563  _email_positivec
-00000a90: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
-00000aa0: 0700 0000 4300 0000 73b2 0200 0074 006a  ....C...s....t.j
-00000ab0: 01a0 02a1 00a0 03a1 0001 0064 0164 0264  ...........d.d.d
-00000ac0: 0364 0474 046a 057c 006a 0664 059c 067c  .d.t.j.|.j.d...|
-00000ad0: 005f 0764 067c 006a 0864 0719 009b 009d  ._.d.|.j.d......
-00000ae0: 0264 087c 006a 0864 0719 009b 0064 097c  .d.|.j.d.....d.|
-00000af0: 006a 099b 009d 0464 0a7c 006a 0864 0719  .j.....d.|.j.d..
-00000b00: 009b 0064 097c 006a 099b 009d 0474 046a  ...d.|.j.....t.j
-00000b10: 057c 006a 0664 0b9c 057c 005f 0a74 0b83  .|.j.d...|._.t..
-00000b20: 007d 017c 016a 016a 0c66 007c 006a 088e  .}.|.j.j.f.|.j..
-00000b30: 017d 0274 0d6a 016a 0e64 0c74 0f64 0d64  .}.t.j.j.d.t.d.d
-00000b40: 0e8d 0117 0064 0f8d 017d 0374 106a 016a  .....d...}.t.j.j
-00000b50: 0e64 1074 0f64 0d64 0e8d 0117 0064 118d  .d.t.d.d.....d..
-00000b60: 017d 047c 036a 11a0 127c 04a1 0101 0074  .}.|.j...|.....t
-00000b70: 136a 016a 0e7c 0364 1264 138d 027d 0574  .j.j.|.d.d...}.t
-00000b80: 136a 016a 0e7c 0364 148d 017d 0674 136a  .j.j.|.d...}.t.j
-00000b90: 016a 0e7c 0364 1564 138d 027d 0774 146a  .j.|.d.d...}.t.j
-00000ba0: 016a 0e66 007c 006a 158e 017d 0874 146a  .j.f.|.j...}.t.j
-00000bb0: 016a 167c 086a 1764 168d 017d 087c 00a0  .j.|.j.d...}.|..
-00000bc0: 187c 086a 197c 006a 1564 1719 00a1 0201  .|.j.|.j.d......
-00000bd0: 007c 00a0 187c 086a 1a7c 006a 1564 1819  .|...|.j.|.j.d..
-00000be0: 00a1 0201 0074 1b6a 016a 0e66 0064 197c  .....t.j.j.f.d.|
-00000bf0: 0869 017c 006a 0797 028e 017d 0974 1b6a  .i.|.j.....}.t.j
-00000c00: 016a 167c 096a 1764 168d 017d 097c 096a  .j.|.j.d...}.|.j
-00000c10: 1ca0 127c 03a1 0101 007c 09a0 1da1 0001  ...|.....|......
-00000c20: 007c 00a0 187c 096a 197c 006a 0764 1719  .|...|.j.|.j.d..
-00000c30: 00a1 0201 007c 00a0 187c 096a 1e7c 006a  .....|...|.j.|.j
-00000c40: 0764 1a19 00a1 0201 007c 00a0 187c 096a  .d.......|...|.j
-00000c50: 1f7c 006a 0764 1b19 00a1 0201 007c 00a0  .|.j.d.......|..
-00000c60: 187c 096a 207c 006a 0764 1c19 00a1 0201  .|.j |.j.d......
-00000c70: 007c 00a0 187c 096a 217c 006a 0764 1d19  .|...|.j!|.j.d..
-00000c80: 00a1 0201 007c 00a0 187c 096a 227c 006a  .....|...|.j"|.j
-00000c90: 0764 1e19 00a1 0201 007c 00a0 187c 096a  .d.......|...|.j
-00000ca0: 236a 247c 086a 24a1 0201 0074 006a 257c  #j$|.j$....t.j%|
-00000cb0: 006a 067c 006a 097c 0264 1f9c 027c 0264  .j.|.j.|.d...|.d
-00000cc0: 208d 0301 007c 00a0 1874 006a 01a0 02a1   ....|...t.j....
-00000cd0: 00a0 26a1 0064 21a1 0201 0074 006a 016a  ..&..d!....t.j.j
-00000ce0: 167c 0264 208d 017d 0a7c 00a0 187c 0a6a  .|.d ..}.|...|.j
-00000cf0: 1e7c 006a 0a64 1a19 00a1 0201 007c 00a0  .|.j.d.......|..
-00000d00: 187c 0a6a 1f7c 006a 0a64 1b19 00a1 0201  .|.j.|.j.d......
-00000d10: 007c 00a0 187c 0a6a 207c 006a 0a64 1c19  .|...|.j |.j.d..
-00000d20: 00a1 0201 007c 00a0 187c 0a6a 217c 006a  .....|...|.j!|.j
-00000d30: 0a64 1d19 00a1 0201 007c 00a0 187c 0a6a  .d.......|...|.j
-00000d40: 227c 006a 0a64 1e19 00a1 0201 007c 00a0  "|.j.d.......|..
-00000d50: 187c 0a6a 2764 22a1 0201 0064 0053 0029  .|.j'd"....d.S.)
-00000d60: 234e 721a 0000 0072 1b00 0000 721c 0000  #Nr....r....r...
-00000d70: 0072 1d00 0000 721e 0000 0072 2600 0000  .r....r....r&...
-00000d80: 7216 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
-00000d90: 2900 0000 722a 0000 005a 0975 7365 726c  )...r*...Z.userl
-00000da0: 6973 745f 7210 0000 0072 1100 0000 a901  ist_r....r......
-00000db0: 721f 0000 005a 0667 726f 7570 5f29 01da  r....Z.group_)..
-00000dc0: 046e 616d 657a 1074 6573 7432 4067 6172  .namez.test2@gar
-00000dd0: 7069 782e 636f 6d29 02da 0975 7365 725f  pix.com)...user_
-00000de0: 6c69 7374 7216 0000 00a9 0172 5200 0000  listr......rR...
-00000df0: 7a10 7465 7374 3340 6761 7270 6978 2e63  z.test3@garpix.c
-00000e00: 6f6d 723e 0000 0072 1f00 0000 7225 0000  omr>...r....r%..
-00000e10: 0072 4000 0000 7220 0000 0072 2100 0000  .r@...r ...r!...
-00000e20: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
-00000e30: 4100 0000 7243 0000 0072 0f00 0000 7213  A...rC...r....r.
-00000e40: 0000 0029 2872 0600 0000 7234 0000 0072  ...)(r....r4...r
-00000e50: 3500 0000 7236 0000 0072 0b00 0000 722f  5...r6...r....r/
-00000e60: 0000 0072 2c00 0000 5a15 6461 7461 5f74  ...r,...Z.data_t
-00000e70: 656d 706c 6174 655f 656d 6169 6c5f 3172  emplate_email_1r
-00000e80: 2e00 0000 7232 0000 005a 1564 6174 615f  ....r2...Z.data_
-00000e90: 636f 6d70 696c 6564 5f65 6d61 696c 5f31  compiled_email_1
-00000ea0: 7204 0000 0072 4400 0000 7209 0000 0072  r....rD...r....r
-00000eb0: 4500 0000 7202 0000 0072 0500 0000 da0b  E...r....r......
-00000ec0: 7573 6572 5f67 726f 7570 73da 0361 6464  user_groups..add
-00000ed0: 720a 0000 0072 0700 0000 7231 0000 0072  r....r....r1...r
-00000ee0: 4600 0000 723f 0000 0072 4700 0000 721f  F...r?...rG...r.
-00000ef0: 0000 0072 2500 0000 7208 0000 00da 0a75  ...r%...r......u
-00000f00: 7365 725f 6c69 7374 73da 0473 6176 6572  ser_lists..saver
-00000f10: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00000f20: 0000 0072 2400 0000 7240 0000 0072 4800  ...r$...r@...rH.
-00000f30: 0000 7249 0000 0072 4a00 0000 7216 0000  ..rI...rJ...r...
-00000f40: 0029 0b72 3900 0000 724c 0000 0072 4200  .).r9...rL...rB.
-00000f50: 0000 7252 0000 00da 0567 726f 7570 da16  ..rR.....group..
-00000f60: 7573 6572 5f6c 6973 745f 7061 7274 6963  user_list_partic
-00000f70: 6970 616e 7431 5a16 7573 6572 5f6c 6973  ipant1Z.user_lis
-00000f80: 745f 7061 7274 6963 6970 616e 7432 5a16  t_participant2Z.
-00000f90: 7573 6572 5f6c 6973 745f 7061 7274 6963  user_list_partic
-00000fa0: 6970 616e 7433 7240 0000 0072 4d00 0000  ipant3r@...rM...
-00000fb0: 724e 0000 0072 3c00 0000 723c 0000 0072  rN...r<...r<...r
-00000fc0: 3d00 0000 da1b 7465 7374 5f6e 6f74 6966  =.....test_notif
-00000fd0: 795f 656d 6169 6c5f 7573 6572 5f6c 6973  y_email_user_lis
-00000fe0: 745c 0000 0073 7600 0000 0001 0e02 0201  t\...sv.........
-00000ff0: 0201 0201 0201 0401 04fa 0809 0e01 1601  ................
-00001000: 1601 0401 04fb 0808 0601 1002 1801 1801  ................
-00001010: 0c02 0601 0201 02fe 0604 0601 02ff 0603  ................
-00001020: 0601 0201 02fe 0606 1001 1001 1401 1403  ................
-00001030: 1801 1001 0c01 0802 1401 1401 1401 1401  ................
-00001040: 1401 1401 1203 0801 0401 02fe 0403 02fd  ................
-00001050: 0605 1603 0e01 1401 1401 1401 1401 1401  ................
-00001060: 7a2c 5072 6542 7569 6c64 5465 7374 4361  z,PreBuildTestCa
-00001070: 7365 2e74 6573 745f 6e6f 7469 6679 5f65  se.test_notify_e
-00001080: 6d61 696c 5f75 7365 725f 6c69 7374 6301  mail_user_listc.
-00001090: 0000 0000 0000 0000 0000 0008 0000 0007  ................
-000010a0: 0000 0043 0000 0073 8e02 0000 7400 6a01  ...C...s....t.j.
-000010b0: a002 a100 a003 a100 0100 6401 6402 6403  ..........d.d.d.
-000010c0: 6404 7404 6a05 7c00 6a06 6405 9c06 7c00  d.t.j.|.j.d...|.
-000010d0: 5f07 6406 7408 6407 6408 8d01 1700 6409  _.d.t.d.d.....d.
-000010e0: 640a 640b 640c 640d 640e 9c06 7c00 5f09  d.d.d.d.d...|._.
-000010f0: 640f 7c00 6a09 6410 1900 9b00 9d02 6411  d.|.j.d.......d.
-00001100: 7c00 6a09 6410 1900 9b00 6412 7c00 6a0a  |.j.d.....d.|.j.
-00001110: 9b00 9d04 6413 7c00 6a09 6410 1900 9b00  ....d.|.j.d.....
-00001120: 6412 7c00 6a0a 9b00 9d04 7404 6a05 7c00  d.|.j.....t.j.|.
-00001130: 6a06 6414 9c05 7c00 5f0b 740c 8300 7d01  j.d...|._.t...}.
-00001140: 7c01 6a01 6a0d 6600 7c00 6a09 8e01 7d02  |.j.j.f.|.j...}.
-00001150: 740e 6a01 6a0f 6406 7408 6415 6408 8d01  t.j.j.d.t.d.d...
-00001160: 1700 6416 8d01 7d03 7410 6a01 6a0f 7c03  ..d...}.t.j.j.|.
-00001170: 6417 8d01 7d04 7411 6a01 6a0f 6600 7c00  d...}.t.j.j.f.|.
-00001180: 6a12 8e01 7d05 7411 6a01 6a13 7c05 6a14  j...}.t.j.j.|.j.
-00001190: 6418 8d01 7d05 7c00 a015 7c05 6a16 7c00  d...}.|...|.j.|.
-000011a0: 6a12 6419 1900 a102 0100 7c00 a015 7c05  j.d.......|...|.
-000011b0: 6a17 7c00 6a12 641a 1900 a102 0100 7418  j.|.j.d.......t.
-000011c0: 6a01 6a0f 6600 7c00 6a07 641b 7c05 6901  j.j.f.|.j.d.|.i.
-000011d0: 9702 8e01 7d06 7418 6a01 6a13 7c06 6a14  ....}.t.j.j.|.j.
-000011e0: 6418 8d01 7d06 7c06 6a19 a01a 7c03 a101  d...}.|.j...|...
-000011f0: 0100 7c06 a01b a100 0100 7c00 a015 7c06  ..|.......|...|.
-00001200: 6a16 7c00 6a07 6419 1900 a102 0100 7c00  j.|.j.d.......|.
-00001210: a015 7c06 6a1c 7c00 6a07 641c 1900 a102  ..|.j.|.j.d.....
-00001220: 0100 7c00 a015 7c06 6a1d 7c00 6a07 641d  ..|...|.j.|.j.d.
-00001230: 1900 a102 0100 7c00 a015 7c06 6a1e 7c00  ......|...|.j.|.
-00001240: 6a07 641e 1900 a102 0100 7c00 a015 7c06  j.d.......|...|.
-00001250: 6a1f 7c00 6a07 641f 1900 a102 0100 7c00  j.|.j.d.......|.
-00001260: a015 7c06 6a20 7c00 6a07 6420 1900 a102  ..|.j |.j.d ....
-00001270: 0100 7c00 a015 7c06 6a21 6a22 7c05 6a22  ..|...|.j!j"|.j"
-00001280: a102 0100 7400 6a23 7c00 6a06 7c00 6a0a  ....t.j#|.j.|.j.
-00001290: 7c02 6421 9c02 7c02 6422 8d03 0100 7c00  |.d!..|.d"....|.
-000012a0: a015 7400 6a01 a002 a100 a024 a100 6423  ..t.j......$..d#
-000012b0: a102 0100 7400 6a01 6a13 7c02 6422 8d01  ....t.j.j.|.d"..
-000012c0: 7d07 7c00 a015 7c07 6a1c 7c00 6a0b 641c  }.|...|.j.|.j.d.
-000012d0: 1900 a102 0100 7c00 a015 7c07 6a1d 7c00  ......|...|.j.|.
-000012e0: 6a0b 641d 1900 a102 0100 7c00 a015 7c07  j.d.......|...|.
-000012f0: 6a1e 7c00 6a0b 641e 1900 a102 0100 7c00  j.|.j.d.......|.
-00001300: a015 7c07 6a1f 7c00 6a0b 641f 1900 a102  ..|.j.|.j.d.....
-00001310: 0100 7c00 a015 7c07 6a20 7c00 6a0b 6420  ..|...|.j |.j.d 
-00001320: 1900 a102 0100 7c00 a015 7c07 6a25 6a26  ......|...|.j%j&
-00001330: 640a a102 0100 6400 5300 2924 4e72 1a00  d.....d.S.)$Nr..
-00001340: 0000 7538 0000 00d0 a2d0 b5d1 81d1 82d0  ..u8............
-00001350: bed0 b2d1 8bd0 b920 d182 d0b5 d0bc d0bf  ....... ........
-00001360: d0bb d0b5 d0b9 d182 207b 7b75 7365 722e  ........ {{user.
-00001370: 7669 6265 725f 6368 6174 5f69 647d 7d75  viber_chat_id}}u
-00001380: 4700 0000 d09a d0be d0bd d182 d0b5 d0bd  G...............
-00001390: d182 20d1 82d0 b5d0 bad1 81d1 82d0 bed0  .. .............
-000013a0: b2d1 8bd0 b920 7b7b 7573 6572 2e76 6962  ..... {{user.vib
-000013b0: 6572 5f63 6861 745f 6964 7d7d 202d 207b  er_chat_id}} - {
-000013c0: 7b73 6f6d 6574 6578 747d 7d75 3900 0000  {sometext}}u9...
-000013d0: d09a d0be d0bd d182 d0b5 d0bd d182 2048  .............. H
-000013e0: 544d 4c20 7b7b 7573 6572 2e76 6962 6572  TML {{user.viber
-000013f0: 5f63 6861 745f 6964 7d7d 202d 207b 7b73  _chat_id}} - {{s
-00001400: 6f6d 6574 6578 747d 7d72 1e00 0000 5a06  ometext}}r....Z.
-00001410: 7669 6265 725f e905 0000 0072 1100 0000  viber_.....r....
-00001420: 5a03 3131 317a 186d 3446 7361 5275 356b  Z.111z.m4FsaRu5k
-00001430: 4269 3848 7a53 4143 306c 6946 513d 3d72  Bi8HzSAC0liFQ==r
-00001440: 1400 0000 5a09 4976 616e 5669 6265 725a  ....Z.IvanViberZ
-00001450: 0b49 7661 6e6f 7656 6962 6572 2906 7215  .IvanovViber).r.
-00001460: 0000 00da 1076 6962 6572 5f73 6563 7265  .....viber_secre
-00001470: 745f 6b65 79da 0d76 6962 6572 5f63 6861  t_key..viber_cha
-00001480: 745f 6964 7217 0000 0072 1800 0000 7219  t_idr....r....r.
-00001490: 0000 0072 2600 0000 725d 0000 0072 2700  ...r&...r]...r'.
-000014a0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-000014b0: 0072 1000 0000 7250 0000 0072 5300 0000  .r....rP...rS...
-000014c0: 723e 0000 0072 1f00 0000 7225 0000 0072  r>...r....r%...r
-000014d0: 4000 0000 7220 0000 0072 2100 0000 7222  @...r ...r!...r"
-000014e0: 0000 0072 2300 0000 7224 0000 0072 4100  ...r#...r$...rA.
-000014f0: 0000 7243 0000 00e9 0300 0000 2927 7206  ..rC........)'r.
-00001500: 0000 0072 3400 0000 7235 0000 0072 3600  ...r4...r5...r6.
-00001510: 0000 720b 0000 00da 0556 4942 4552 722d  ..r......VIBERr-
-00001520: 0000 005a 1364 6174 615f 7465 6d70 6c61  ...Z.data_templa
-00001530: 7465 5f76 6962 6572 7202 0000 005a 0f64  te_viberr....Z.d
-00001540: 6174 615f 7669 6265 725f 7573 6572 7232  ata_viber_userr2
-00001550: 0000 005a 1364 6174 615f 636f 6d70 696c  ...Z.data_compil
-00001560: 6564 5f76 6962 6572 7204 0000 0072 4400  ed_viberr....rD.
-00001570: 0000 7209 0000 0072 4500 0000 720a 0000  ..r....rE...r...
-00001580: 0072 0700 0000 7231 0000 0072 4600 0000  .r....r1...rF...
-00001590: 723f 0000 0072 4700 0000 721f 0000 0072  r?...rG...r....r
-000015a0: 2500 0000 7208 0000 0072 5600 0000 7255  %...r....rV...rU
-000015b0: 0000 0072 5700 0000 7220 0000 0072 2100  ...rW...r ...r!.
-000015c0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-000015d0: 0072 4000 0000 7248 0000 0072 4900 0000  .r@...rH...rI...
-000015e0: 724a 0000 0072 4200 0000 725d 0000 0029  rJ...rB...r]...)
-000015f0: 0872 3900 0000 724c 0000 0072 4200 0000  .r9...rL...rB...
-00001600: 7252 0000 0072 5900 0000 7240 0000 005a  rR...rY...r@...Z
-00001610: 0e74 656d 706c 6174 655f 7669 6265 7272  .template_viberr
-00001620: 4e00 0000 723c 0000 0072 3c00 0000 723d  N...r<...r<...r=
-00001630: 0000 00da 1174 6573 745f 6e6f 7469 6679  .....test_notify
-00001640: 5f76 6962 6572 a600 0000 7370 0000 0000  _viber....sp....
-00001650: 010e 0202 0102 0102 0102 0104 0104 fa08  ................
-00001660: 090c 0102 0102 0102 0102 0102 fa08 090e  ................
-00001670: 0116 0116 0104 0104 fb08 0806 0110 0218  ................
-00001680: 0106 0102 ff06 0410 0110 0214 0114 0318  ................
-00001690: 0110 010c 0108 0214 0114 0114 0114 0114  ................
-000016a0: 0114 0112 0308 0104 0102 fe04 0302 fd06  ................
-000016b0: 0516 030e 0114 0114 0114 0114 0114 017a  ...............z
-000016c0: 2250 7265 4275 696c 6454 6573 7443 6173  "PreBuildTestCas
-000016d0: 652e 7465 7374 5f6e 6f74 6966 795f 7669  e.test_notify_vi
-000016e0: 6265 7229 08da 085f 5f6e 616d 655f 5fda  ber)...__name__.
-000016f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001700: 7561 6c6e 616d 655f 5f72 3800 0000 724f  ualname__r8...rO
-00001710: 0000 0072 5a00 0000 7260 0000 00da 0d5f  ...rZ...r`....._
-00001720: 5f63 6c61 7373 6365 6c6c 5f5f 723c 0000  _classcell__r<..
-00001730: 0072 3c00 0000 723a 0000 0072 3d00 0000  .r<...r:...r=...
-00001740: 720d 0000 0015 0000 0073 0800 0000 0801  r........s......
-00001750: 0c25 0821 084a 720d 0000 0029 16da 0664  .%.!.Jr....)...d
-00001760: 6a61 6e67 6fda 026f 73da 1364 6a61 6e67  jango..os..djang
-00001770: 6f2e 7574 696c 732e 6372 7970 746f 7202  o.utils.cryptor.
-00001780: 0000 00da 0875 6e69 7474 6573 7472 0300  .....unittestr..
-00001790: 0000 da13 646a 616e 676f 2e63 6f6e 7472  ....django.contr
-000017a0: 6962 2e61 7574 6872 0400 0000 da1a 646a  ib.authr......dj
-000017b0: 616e 676f 2e63 6f6e 7472 6962 2e61 7574  ango.contrib.aut
-000017c0: 682e 6d6f 6465 6c73 7205 0000 005a 1467  h.modelsr....Z.g
-000017d0: 6172 7069 785f 6e6f 7469 6679 2e6d 6f64  arpix_notify.mod
-000017e0: 656c 7372 0600 0000 7207 0000 0072 0800  elsr....r....r..
-000017f0: 0000 7209 0000 0072 0a00 0000 5a1c 6761  ..r....r....Z.ga
-00001800: 7270 6978 5f6e 6f74 6966 792e 6d6f 6465  rpix_notify.mode
-00001810: 6c73 2e63 686f 6963 6573 720b 0000 00da  ls.choicesr.....
-00001820: 0765 6e76 6972 6f6e da0a 7365 7464 6566  .environ..setdef
-00001830: 6175 6c74 da05 7365 7475 7072 0d00 0000  ault..setupr....
-00001840: 723c 0000 0072 3c00 0000 723c 0000 0072  r<...r<...r<...r
-00001850: 3d00 0000 da08 3c6d 6f64 756c 653e 0100  =.....<module>..
-00001860: 0000 731c 0000 0008 0108 020c 010c 020c  ..s.............
-00001870: 010c 020c 010c 010c 010c 010c 010c 020e  ................
-00001880: 0108 03                                  ...
+000002e0: 0b83 00a0 0ca1 0001 0064 0053 0029 1b4e  .........d.S.).N
+000002f0: 7201 0000 00e9 0100 0000 e902 0000 005a  r..............Z
+00000300: 0a65 6d61 696c 5f74 6573 74e9 0400 0000  .email_test.....
+00000310: a901 da06 6c65 6e67 7468 fa0f 7465 7374  ....length..test
+00000320: 4067 6172 7069 782e 636f 6dda 0942 6c61  @garpix.com..Bla
+00000330: 426c 6131 3233 5a04 4976 616e 5a06 4976  Bla123Z.IvanZ.Iv
+00000340: 616e 6f76 2905 da08 7573 6572 6e61 6d65  anov)...username
+00000350: da05 656d 6169 6cda 0870 6173 7377 6f72  ..email..passwor
+00000360: 64da 0a66 6972 7374 5f6e 616d 65da 096c  d..first_name..l
+00000370: 6173 745f 6e61 6d65 f521 0000 00d0 a2d0  ast_name.!......
+00000380: b5d1 81d1 82d0 bed0 b2d1 8bd0 b920 d182  ............. ..
+00000390: d0b5 d0bc d0bf d0bb d0b5 d0b9 d182 f530  ...............0
+000003a0: 0000 00d0 a2d0 b5d1 81d1 82d0 bed0 b2d1  ................
+000003b0: 8bd0 b920 d182 d0b5 d0bc d0bf d0bb d0b5  ... ............
+000003c0: d0b9 d182 207b 7b75 7365 722e 656d 6169  .... {{user.emai
+000003d0: 6c7d 7df5 3f00 0000 d09a d0be d0bd d182  l}}.?...........
+000003e0: d0b5 d0bd d182 20d1 82d0 b5d0 bad1 81d1  ...... .........
+000003f0: 82d0 bed0 b2d1 8bd0 b920 7b7b 7573 6572  ......... {{user
+00000400: 2e65 6d61 696c 7d7d 202d 207b 7b73 6f6d  .email}} - {{som
+00000410: 6574 6578 747d 7df5 3100 0000 d09a d0be  etext}}.1.......
+00000420: d0bd d182 d0b5 d0bd d182 2048 544d 4c20  .......... HTML 
+00000430: 7b7b 7573 6572 2e65 6d61 696c 7d7d 202d  {{user.email}} -
+00000440: 207b 7b73 6f6d 6574 6578 747d 7da9 06da   {{sometext}}...
+00000450: 0574 6974 6c65 da07 7375 626a 6563 74da  .title..subject.
+00000460: 0474 6578 74da 0468 746d 6cda 0474 7970  .text..html..typ
+00000470: 65da 0565 7665 6e74 7524 0000 00d0 9ed1  e..eventu$......
+00000480: 81d0 bdd0 bed0 b2d0 bdd0 b0d1 8f20 d0ba  ............. ..
+00000490: d0b0 d182 d0b5 d0b3 d0be d180 d0b8 d18f  ................
+000004a0: 5f7a 133c 6469 763e 7b7b 7465 7874 7d7d  _z.<div>{{text}}
+000004b0: 3c2f 6469 763e 2902 721f 0000 00da 0874  </div>).r......t
+000004c0: 656d 706c 6174 657a 0762 6c61 2062 6c61  emplatez.bla bla
+000004d0: f522 0000 00d0 a2d0 b5d1 81d1 82d0 bed0  ."..............
+000004e0: b2d1 8bd0 b920 d182 d0b5 d0bc d0bf d0bb  ..... ..........
+000004f0: d0b5 d0b9 d182 2072 1600 0000 f522 0000  ...... r....."..
+00000500: 00d0 9ad0 bed0 bdd1 82d0 b5d0 bdd1 8220  ............... 
+00000510: d182 d0b5 d0ba d181 d182 d0be d0b2 d18b  ................
+00000520: d0b9 20fa 0320 2d20 f514 0000 00d0 9ad0  .. .. - ........
+00000530: bed0 bdd1 82d0 b5d0 bdd1 8220 4854 4d4c  ........... HTML
+00000540: 20a9 0572 2000 0000 7221 0000 0072 2200   ..r ...r!...r".
+00000550: 0000 7223 0000 0072 2400 0000 290d da0f  ..r#...r$...)...
+00000560: 5041 5353 5f54 4553 545f 4556 454e 54da  PASS_TEST_EVENT.
+00000570: 1150 4153 535f 5445 5354 5f45 5645 4e54  .PASS_TEST_EVENT
+00000580: 5f31 da11 5041 5353 5f54 4553 545f 4556  _1..PASS_TEST_EV
+00000590: 454e 545f 3272 0200 0000 da09 6461 7461  ENT_2r......data
+000005a0: 5f75 7365 7272 0b00 0000 da05 454d 4149  _userr......EMAI
+000005b0: 4cda 1364 6174 615f 7465 6d70 6c61 7465  L..data_template
+000005c0: 5f65 6d61 696c da0d 6461 7461 5f63 6174  _email..data_cat
+000005d0: 6567 6f72 79da 0873 6f6d 6574 6578 74da  egory..sometext.
+000005e0: 1364 6174 615f 636f 6d70 696c 6564 5f65  .data_compiled_e
+000005f0: 6d61 696c da05 7375 7065 72da 0573 6574  mail..super..set
+00000600: 5570 2901 da04 7365 6c66 a901 da09 5f5f  Up)...self....__
+00000610: 636c 6173 735f 5fa9 00fa 432f 5573 6572  class__...C/User
+00000620: 732f 6372 7573 6174 2f70 726f 6a65 6374  s/crusat/project
+00000630: 732f 6761 7270 6978 5f6e 6f74 6966 792f  s/garpix_notify/
+00000640: 6261 636b 656e 642f 6761 7270 6978 5f6e  backend/garpix_n
+00000650: 6f74 6966 792f 7465 7374 732e 7079 7235  otify/tests.pyr5
+00000660: 0000 0016 0000 0073 3600 0000 0002 0601  .......s6.......
+00000670: 0601 0603 0c01 0201 0201 0201 02fb 0809  ................
+00000680: 0201 0201 0201 0201 0401 04fa 0809 0c01  ................
+00000690: 02fe 0804 0602 0e01 1601 1601 0401 04fb  ................
+000006a0: 0807 7a16 5072 6542 7569 6c64 5465 7374  ..z.PreBuildTest
+000006b0: 4361 7365 2e73 6574 5570 6301 0000 0000  Case.setUpc.....
+000006c0: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
+000006d0: 0000 0073 a201 0000 7400 8300 7d01 7c01  ...s....t...}.|.
+000006e0: 6a01 6a02 6600 7c00 6a03 8e01 7d02 7404  j.j.f.|.j...}.t.
+000006f0: 6a01 6a05 6600 7c00 6a06 8e01 7d03 7404  j.j.f.|.j...}.t.
+00000700: 6a01 6a07 7c03 6a08 6401 8d01 7d03 7c00  j.j.|.j.d...}.|.
+00000710: a009 7c03 6a0a 7c00 6a06 6402 1900 a102  ..|.j.|.j.d.....
+00000720: 0100 7c00 a009 7c03 6a0b 7c00 6a06 6403  ..|...|.j.|.j.d.
+00000730: 1900 a102 0100 740c 6a01 6a05 6600 6404  ......t.j.j.f.d.
+00000740: 7c03 6901 7c00 6a0d 9702 8e01 7d04 740c  |.i.|.j.....}.t.
+00000750: 6a01 6a07 7c04 6a08 6401 8d01 7d04 7c00  j.j.|.j.d...}.|.
+00000760: a009 7c04 6a0a 7c00 6a0d 6402 1900 a102  ..|.j.|.j.d.....
+00000770: 0100 7c00 a009 7c04 6a0e 7c00 6a0d 6405  ..|...|.j.|.j.d.
+00000780: 1900 a102 0100 7c00 a009 7c04 6a0f 7c00  ......|...|.j.|.
+00000790: 6a0d 6406 1900 a102 0100 7c00 a009 7c04  j.d.......|...|.
+000007a0: 6a10 7c00 6a0d 6407 1900 a102 0100 7c00  j.|.j.d.......|.
+000007b0: a009 7c04 6a11 7c00 6a0d 6408 1900 a102  ..|.j.|.j.d.....
+000007c0: 0100 7c00 a009 7c04 6a12 7c00 6a0d 6409  ..|...|.j.|.j.d.
+000007d0: 1900 a102 0100 7c00 a009 7c04 6a13 6a14  ......|...|.j.j.
+000007e0: 7c03 6a14 a102 0100 7415 6a16 7c00 6a17  |.j.....t.j.|.j.
+000007f0: 7c00 6a18 7c02 640a 9c02 7c02 640b 8d03  |.j.|.d...|.d...
+00000800: 7d05 7c00 a009 7c05 6a12 7c04 6a12 a102  }.|...|.j.|.j...
+00000810: 0100 7c00 a009 7c05 6a0e 7c00 6a19 6405  ..|...|.j.|.j.d.
+00000820: 1900 a102 0100 7c00 a009 7c05 6a0f 7c00  ......|...|.j.|.
+00000830: 6a19 6406 1900 a102 0100 7c00 a009 7c05  j.d.......|...|.
+00000840: 6a10 7c00 6a19 6407 1900 a102 0100 7c00  j.|.j.d.......|.
+00000850: a009 7c05 6a11 7c00 6a19 6408 1900 a102  ..|.j.|.j.d.....
+00000860: 0100 7c00 a009 7c05 6a12 7c00 6a19 6409  ..|...|.j.|.j.d.
+00000870: 1900 a102 0100 6400 5300 290c 4ea9 01da  ......d.S.).N...
+00000880: 0270 6b72 1f00 0000 7225 0000 00da 0863  .pkr....r%.....c
+00000890: 6174 6567 6f72 7972 2000 0000 7221 0000  ategoryr ...r!..
+000008a0: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+000008b0: a902 7232 0000 00da 0475 7365 72a9 0172  ..r2.....user..r
+000008c0: 3f00 0000 291a 7204 0000 00da 076f 626a  ?...).r......obj
+000008d0: 6563 7473 da0b 6372 6561 7465 5f75 7365  ects..create_use
+000008e0: 7272 2e00 0000 7207 0000 00da 0663 7265  rr....r......cre
+000008f0: 6174 6572 3100 0000 da03 6765 7472 3c00  ater1.....getr<.
+00000900: 0000 da0b 6173 7365 7274 4571 7561 6c72  ....assertEqualr
+00000910: 1f00 0000 7225 0000 0072 0800 0000 7230  ....r%...r....r0
+00000920: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00000930: 0000 7223 0000 0072 2400 0000 723d 0000  ..r#...r$...r=..
+00000940: 00da 0269 6472 0600 0000 da04 7365 6e64  ...idr......send
+00000950: 722b 0000 0072 3200 0000 7233 0000 0029  r+...r2...r3...)
+00000960: 0672 3600 0000 da04 5573 6572 723f 0000  .r6.....Userr?..
+00000970: 0072 3d00 0000 da0e 7465 6d70 6c61 7465  .r=.....template
+00000980: 5f65 6d61 696c da06 6e6f 7469 6679 7239  _email..notifyr9
+00000990: 0000 0072 3900 0000 723a 0000 00da 1a74  ...r9...r:.....t
+000009a0: 6573 745f 6e6f 7469 6679 5f65 6d61 696c  est_notify_email
+000009b0: 5f70 6f73 6974 6976 653a 0000 0073 3600  _positive:...s6.
+000009c0: 0000 0002 0601 1002 1001 1001 1401 1402  ................
+000009d0: 1801 1001 1401 1401 1401 1401 1401 1401  ................
+000009e0: 1202 0801 0401 02fe 0403 02fd 0604 1001  ................
+000009f0: 1401 1401 1401 1401 7a2b 5072 6542 7569  ........z+PreBui
+00000a00: 6c64 5465 7374 4361 7365 2e74 6573 745f  ldTestCase.test_
+00000a10: 6e6f 7469 6679 5f65 6d61 696c 5f70 6f73  notify_email_pos
+00000a20: 6974 6976 6563 0100 0000 0000 0000 0000  itivec..........
+00000a30: 0000 0b00 0000 0700 0000 4300 0000 7390  ..........C...s.
+00000a40: 0200 0064 0164 0264 0364 0474 006a 017c  ...d.d.d.d.t.j.|
+00000a50: 006a 0264 059c 067c 005f 0364 067c 006a  .j.d...|._.d.|.j
+00000a60: 0464 0719 009b 009d 0264 087c 006a 0464  .d.......d.|.j.d
+00000a70: 0719 009b 0064 097c 006a 059b 009d 0464  .....d.|.j.....d
+00000a80: 0a7c 006a 0464 0719 009b 0064 097c 006a  .|.j.d.....d.|.j
+00000a90: 059b 009d 0474 006a 017c 006a 0264 0b9c  .....t.j.|.j.d..
+00000aa0: 057c 005f 0674 0783 007d 017c 016a 086a  .|._.t...}.|.j.j
+00000ab0: 0966 007c 006a 048e 017d 0274 0a6a 086a  .f.|.j...}.t.j.j
+00000ac0: 0b64 0c74 0c64 0d64 0e8d 0117 0064 0f8d  .d.t.d.d.....d..
+00000ad0: 017d 0374 0d6a 086a 0b64 1074 0c64 0d64  .}.t.j.j.d.t.d.d
+00000ae0: 0e8d 0117 0064 118d 017d 047c 036a 0ea0  .....d...}.|.j..
+00000af0: 0f7c 04a1 0101 0074 106a 086a 0b7c 0364  .|.....t.j.j.|.d
+00000b00: 1264 138d 027d 0574 106a 086a 0b7c 0364  .d...}.t.j.j.|.d
+00000b10: 148d 017d 0674 106a 086a 0b7c 0364 1564  ...}.t.j.j.|.d.d
+00000b20: 138d 027d 0774 116a 086a 0b66 007c 006a  ...}.t.j.j.f.|.j
+00000b30: 128e 017d 0874 116a 086a 137c 086a 1464  ...}.t.j.j.|.j.d
+00000b40: 168d 017d 087c 00a0 157c 086a 167c 006a  ...}.|...|.j.|.j
+00000b50: 1264 1719 00a1 0201 007c 00a0 157c 086a  .d.......|...|.j
+00000b60: 177c 006a 1264 1819 00a1 0201 0074 186a  .|.j.d.......t.j
+00000b70: 086a 0b66 0064 197c 0869 017c 006a 0397  .j.f.d.|.i.|.j..
+00000b80: 028e 017d 0974 186a 086a 137c 096a 1464  ...}.t.j.j.|.j.d
+00000b90: 168d 017d 097c 096a 19a0 0f7c 03a1 0101  ...}.|.j...|....
+00000ba0: 007c 09a0 1aa1 0001 007c 00a0 157c 096a  .|.......|...|.j
+00000bb0: 167c 006a 0364 1719 00a1 0201 007c 00a0  .|.j.d.......|..
+00000bc0: 157c 096a 1b7c 006a 0364 1a19 00a1 0201  .|.j.|.j.d......
+00000bd0: 007c 00a0 157c 096a 1c7c 006a 0364 1b19  .|...|.j.|.j.d..
+00000be0: 00a1 0201 007c 00a0 157c 096a 1d7c 006a  .....|...|.j.|.j
+00000bf0: 0364 1c19 00a1 0201 007c 00a0 157c 096a  .d.......|...|.j
+00000c00: 1e7c 006a 0364 1d19 00a1 0201 007c 00a0  .|.j.d.......|..
+00000c10: 157c 096a 1f7c 006a 0364 1e19 00a1 0201  .|.j.|.j.d......
+00000c20: 007c 00a0 157c 096a 206a 217c 086a 21a1  .|...|.j j!|.j!.
+00000c30: 0201 0074 226a 237c 006a 027c 006a 057c  ...t"j#|.j.|.j.|
+00000c40: 0264 1f9c 027c 0264 208d 037d 0a7c 00a0  .d...|.d ..}.|..
+00000c50: 157c 0a6a 1f7c 096a 1fa1 0201 007c 00a0  .|.j.|.j.....|..
+00000c60: 157c 0a6a 1b7c 006a 0664 1a19 00a1 0201  .|.j.|.j.d......
+00000c70: 007c 00a0 157c 0a6a 1c7c 006a 0664 1b19  .|...|.j.|.j.d..
+00000c80: 00a1 0201 007c 00a0 157c 0a6a 1d7c 006a  .....|...|.j.|.j
+00000c90: 0664 1c19 00a1 0201 007c 00a0 157c 0a6a  .d.......|...|.j
+00000ca0: 1e7c 006a 0664 1d19 00a1 0201 007c 00a0  .|.j.d.......|..
+00000cb0: 157c 0a6a 1f7c 006a 0664 1e19 00a1 0201  .|.j.|.j.d......
+00000cc0: 007c 00a0 157c 0a6a 2464 21a1 0201 0064  .|...|.j$d!....d
+00000cd0: 0053 0029 224e 721a 0000 0072 1b00 0000  .S.)"Nr....r....
+00000ce0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000cf0: 2600 0000 7216 0000 0072 2700 0000 7228  &...r....r'...r(
+00000d00: 0000 0072 2900 0000 722a 0000 005a 0975  ...r)...r*...Z.u
+00000d10: 7365 726c 6973 745f 7210 0000 0072 1100  serlist_r....r..
+00000d20: 0000 a901 721f 0000 005a 0667 726f 7570  ....r....Z.group
+00000d30: 5f29 01da 046e 616d 657a 1074 6573 7432  _)...namez.test2
+00000d40: 4067 6172 7069 782e 636f 6d29 02da 0975  @garpix.com)...u
+00000d50: 7365 725f 6c69 7374 7216 0000 00a9 0172  ser_listr......r
+00000d60: 4e00 0000 7a10 7465 7374 3340 6761 7270  N...z.test3@garp
+00000d70: 6978 2e63 6f6d 723b 0000 0072 1f00 0000  ix.comr;...r....
+00000d80: 7225 0000 0072 3d00 0000 7220 0000 0072  r%...r=...r ...r
+00000d90: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
+00000da0: 0000 0072 3e00 0000 7240 0000 0072 1300  ...r>...r@...r..
+00000db0: 0000 2925 720b 0000 0072 2f00 0000 722c  ..)%r....r/...r,
+00000dc0: 0000 005a 1564 6174 615f 7465 6d70 6c61  ...Z.data_templa
+00000dd0: 7465 5f65 6d61 696c 5f31 722e 0000 0072  te_email_1r....r
+00000de0: 3200 0000 5a15 6461 7461 5f63 6f6d 7069  2...Z.data_compi
+00000df0: 6c65 645f 656d 6169 6c5f 3172 0400 0000  led_email_1r....
+00000e00: 7241 0000 0072 4200 0000 7209 0000 0072  rA...rB...r....r
+00000e10: 4300 0000 7202 0000 0072 0500 0000 da0b  C...r....r......
+00000e20: 7573 6572 5f67 726f 7570 73da 0361 6464  user_groups..add
+00000e30: 720a 0000 0072 0700 0000 7231 0000 0072  r....r....r1...r
+00000e40: 4400 0000 723c 0000 0072 4500 0000 721f  D...r<...rE...r.
+00000e50: 0000 0072 2500 0000 7208 0000 00da 0a75  ...r%...r......u
+00000e60: 7365 725f 6c69 7374 73da 0473 6176 6572  ser_lists..saver
+00000e70: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+00000e80: 0000 0072 2400 0000 723d 0000 0072 4600  ...r$...r=...rF.
+00000e90: 0000 7206 0000 0072 4700 0000 7216 0000  ..r....rG...r...
+00000ea0: 0029 0b72 3600 0000 7248 0000 0072 3f00  .).r6...rH...r?.
+00000eb0: 0000 724e 0000 00da 0567 726f 7570 da16  ..rN.....group..
+00000ec0: 7573 6572 5f6c 6973 745f 7061 7274 6963  user_list_partic
+00000ed0: 6970 616e 7431 5a16 7573 6572 5f6c 6973  ipant1Z.user_lis
+00000ee0: 745f 7061 7274 6963 6970 616e 7432 5a16  t_participant2Z.
+00000ef0: 7573 6572 5f6c 6973 745f 7061 7274 6963  user_list_partic
+00000f00: 6970 616e 7433 723d 0000 0072 4900 0000  ipant3r=...rI...
+00000f10: 724a 0000 0072 3900 0000 7239 0000 0072  rJ...r9...r9...r
+00000f20: 3a00 0000 da1b 7465 7374 5f6e 6f74 6966  :.....test_notif
+00000f30: 795f 656d 6169 6c5f 7573 6572 5f6c 6973  y_email_user_lis
+00000f40: 7459 0000 0073 7200 0000 0002 0201 0201  tY...sr.........
+00000f50: 0201 0201 0401 04fa 0809 0e01 1601 1601  ................
+00000f60: 0401 04fb 0808 0601 1002 1801 1801 0c02  ................
+00000f70: 0601 0201 02fe 0604 0601 02ff 0603 0601  ................
+00000f80: 0201 02fe 0606 1001 1001 1401 1403 1801  ................
+00000f90: 1001 0c01 0802 1401 1401 1401 1401 1401  ................
+00000fa0: 1401 1203 0801 0401 02fe 0403 02fd 0605  ................
+00000fb0: 1003 1401 1401 1401 1401 1401 7a2c 5072  ............z,Pr
+00000fc0: 6542 7569 6c64 5465 7374 4361 7365 2e74  eBuildTestCase.t
+00000fd0: 6573 745f 6e6f 7469 6679 5f65 6d61 696c  est_notify_email
+00000fe0: 5f75 7365 725f 6c69 7374 6301 0000 0000  _user_listc.....
+00000ff0: 0000 0000 0000 0008 0000 0007 0000 0043  ...............C
+00001000: 0000 0073 6c02 0000 6401 6402 6403 6404  ...sl...d.d.d.d.
+00001010: 7400 6a01 7c00 6a02 6405 9c06 7c00 5f03  t.j.|.j.d...|._.
+00001020: 6406 7404 6407 6408 8d01 1700 6409 640a  d.t.d.d.....d.d.
+00001030: 640b 640c 640d 640e 9c06 7c00 5f05 640f  d.d.d.d...|._.d.
+00001040: 7c00 6a05 6410 1900 9b00 9d02 6411 7c00  |.j.d.......d.|.
+00001050: 6a05 6410 1900 9b00 6412 7c00 6a06 9b00  j.d.....d.|.j...
+00001060: 9d04 6413 7c00 6a05 6410 1900 9b00 6412  ..d.|.j.d.....d.
+00001070: 7c00 6a06 9b00 9d04 7400 6a01 7c00 6a02  |.j.....t.j.|.j.
+00001080: 6414 9c05 7c00 5f07 7408 8300 7d01 7c01  d...|._.t...}.|.
+00001090: 6a09 6a0a 6600 7c00 6a05 8e01 7d02 740b  j.j.f.|.j...}.t.
+000010a0: 6a09 6a0c 6406 7404 6415 6408 8d01 1700  j.j.d.t.d.d.....
+000010b0: 6416 8d01 7d03 740d 6a09 6a0c 7c03 6417  d...}.t.j.j.|.d.
+000010c0: 8d01 7d04 740e 6a09 6a0c 6600 7c00 6a0f  ..}.t.j.j.f.|.j.
+000010d0: 8e01 7d05 740e 6a09 6a10 7c05 6a11 6418  ..}.t.j.j.|.j.d.
+000010e0: 8d01 7d05 7c00 a012 7c05 6a13 7c00 6a0f  ..}.|...|.j.|.j.
+000010f0: 6419 1900 a102 0100 7c00 a012 7c05 6a14  d.......|...|.j.
+00001100: 7c00 6a0f 641a 1900 a102 0100 7415 6a09  |.j.d.......t.j.
+00001110: 6a0c 6600 7c00 6a03 641b 7c05 6901 9702  j.f.|.j.d.|.i...
+00001120: 8e01 7d06 7415 6a09 6a10 7c06 6a11 6418  ..}.t.j.j.|.j.d.
+00001130: 8d01 7d06 7c06 6a16 a017 7c03 a101 0100  ..}.|.j...|.....
+00001140: 7c06 a018 a100 0100 7c00 a012 7c06 6a13  |.......|...|.j.
+00001150: 7c00 6a03 6419 1900 a102 0100 7c00 a012  |.j.d.......|...
+00001160: 7c06 6a19 7c00 6a03 641c 1900 a102 0100  |.j.|.j.d.......
+00001170: 7c00 a012 7c06 6a1a 7c00 6a03 641d 1900  |...|.j.|.j.d...
+00001180: a102 0100 7c00 a012 7c06 6a1b 7c00 6a03  ....|...|.j.|.j.
+00001190: 641e 1900 a102 0100 7c00 a012 7c06 6a1c  d.......|...|.j.
+000011a0: 7c00 6a03 641f 1900 a102 0100 7c00 a012  |.j.d.......|...
+000011b0: 7c06 6a1d 7c00 6a03 6420 1900 a102 0100  |.j.|.j.d ......
+000011c0: 7c00 a012 7c06 6a1e 6a1f 7c05 6a1f a102  |...|.j.j.|.j...
+000011d0: 0100 7420 6a21 7c00 6a02 7c00 6a06 7c02  ..t j!|.j.|.j.|.
+000011e0: 6421 9c02 7c02 6422 8d03 7d07 7c00 a012  d!..|.d"..}.|...
+000011f0: 7c07 6a1d 7c06 6a1d a102 0100 7c00 a012  |.j.|.j.....|...
+00001200: 7c07 6a19 7c00 6a07 641c 1900 a102 0100  |.j.|.j.d.......
+00001210: 7c00 a012 7c07 6a1a 7c00 6a07 641d 1900  |...|.j.|.j.d...
+00001220: a102 0100 7c00 a012 7c07 6a1b 7c00 6a07  ....|...|.j.|.j.
+00001230: 641e 1900 a102 0100 7c00 a012 7c07 6a1c  d.......|...|.j.
+00001240: 7c00 6a07 641f 1900 a102 0100 7c00 a012  |.j.d.......|...
+00001250: 7c07 6a1d 7c00 6a07 6420 1900 a102 0100  |.j.|.j.d ......
+00001260: 7c00 a012 7c07 6a22 6a23 640a a102 0100  |...|.j"j#d.....
+00001270: 6400 5300 2923 4e72 1a00 0000 7538 0000  d.S.)#Nr....u8..
+00001280: 00d0 a2d0 b5d1 81d1 82d0 bed0 b2d1 8bd0  ................
+00001290: b920 d182 d0b5 d0bc d0bf d0bb d0b5 d0b9  . ..............
+000012a0: d182 207b 7b75 7365 722e 7669 6265 725f  .. {{user.viber_
+000012b0: 6368 6174 5f69 647d 7d75 4700 0000 d09a  chat_id}}uG.....
+000012c0: d0be d0bd d182 d0b5 d0bd d182 20d1 82d0  ............ ...
+000012d0: b5d0 bad1 81d1 82d0 bed0 b2d1 8bd0 b920  ............... 
+000012e0: 7b7b 7573 6572 2e76 6962 6572 5f63 6861  {{user.viber_cha
+000012f0: 745f 6964 7d7d 202d 207b 7b73 6f6d 6574  t_id}} - {{somet
+00001300: 6578 747d 7d75 3900 0000 d09a d0be d0bd  ext}}u9.........
+00001310: d182 d0b5 d0bd d182 2048 544d 4c20 7b7b  ........ HTML {{
+00001320: 7573 6572 2e76 6962 6572 5f63 6861 745f  user.viber_chat_
+00001330: 6964 7d7d 202d 207b 7b73 6f6d 6574 6578  id}} - {{sometex
+00001340: 747d 7d72 1e00 0000 5a06 7669 6265 725f  t}}r....Z.viber_
+00001350: e905 0000 0072 1100 0000 5a03 3131 317a  .....r....Z.111z
+00001360: 186d 3446 7361 5275 356b 4269 3848 7a53  .m4FsaRu5kBi8HzS
+00001370: 4143 306c 6946 513d 3d72 1400 0000 5a09  AC0liFQ==r....Z.
+00001380: 4976 616e 5669 6265 725a 0b49 7661 6e6f  IvanViberZ.Ivano
+00001390: 7656 6962 6572 2906 7215 0000 00da 1076  vViber).r......v
+000013a0: 6962 6572 5f73 6563 7265 745f 6b65 79da  iber_secret_key.
+000013b0: 0d76 6962 6572 5f63 6861 745f 6964 7217  .viber_chat_idr.
+000013c0: 0000 0072 1800 0000 7219 0000 0072 2600  ...r....r....r&.
+000013d0: 0000 7259 0000 0072 2700 0000 7228 0000  ..rY...r'...r(..
+000013e0: 0072 2900 0000 722a 0000 0072 1000 0000  .r)...r*...r....
+000013f0: 724c 0000 0072 4f00 0000 723b 0000 0072  rL...rO...r;...r
+00001400: 1f00 0000 7225 0000 0072 3d00 0000 7220  ....r%...r=...r 
+00001410: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+00001420: 0000 7224 0000 0072 3e00 0000 7240 0000  ..r$...r>...r@..
+00001430: 0029 2472 0b00 0000 da05 5649 4245 5272  .)$r......VIBERr
+00001440: 2d00 0000 5a13 6461 7461 5f74 656d 706c  -...Z.data_templ
+00001450: 6174 655f 7669 6265 7272 0200 0000 5a0f  ate_viberr....Z.
+00001460: 6461 7461 5f76 6962 6572 5f75 7365 7272  data_viber_userr
+00001470: 3200 0000 5a13 6461 7461 5f63 6f6d 7069  2...Z.data_compi
+00001480: 6c65 645f 7669 6265 7272 0400 0000 7241  led_viberr....rA
+00001490: 0000 0072 4200 0000 7209 0000 0072 4300  ...rB...r....rC.
+000014a0: 0000 720a 0000 0072 0700 0000 7231 0000  ..r....r....r1..
+000014b0: 0072 4400 0000 723c 0000 0072 4500 0000  .rD...r<...rE...
+000014c0: 721f 0000 0072 2500 0000 7208 0000 0072  r....r%...r....r
+000014d0: 5200 0000 7251 0000 0072 5300 0000 7220  R...rQ...rS...r 
+000014e0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+000014f0: 0000 7224 0000 0072 3d00 0000 7246 0000  ..r$...r=...rF..
+00001500: 0072 0600 0000 7247 0000 0072 3f00 0000  .r....rG...r?...
+00001510: 7259 0000 0029 0872 3600 0000 7248 0000  rY...).r6...rH..
+00001520: 0072 3f00 0000 724e 0000 0072 5500 0000  .r?...rN...rU...
+00001530: 723d 0000 005a 0e74 656d 706c 6174 655f  r=...Z.template_
+00001540: 7669 6265 7272 4a00 0000 7239 0000 0072  viberrJ...r9...r
+00001550: 3900 0000 723a 0000 00da 1174 6573 745f  9...r:.....test_
+00001560: 6e6f 7469 6679 5f76 6962 6572 a100 0000  notify_viber....
+00001570: 736c 0000 0000 0202 0102 0102 0102 0104  sl..............
+00001580: 0104 fa08 090c 0102 0102 0102 0102 0102  ................
+00001590: fa08 090e 0116 0116 0104 0104 fb08 0806  ................
+000015a0: 0110 0218 0106 0102 ff06 0410 0110 0214  ................
+000015b0: 0114 0318 0110 010c 0108 0214 0114 0114  ................
+000015c0: 0114 0114 0114 0112 0308 0104 0102 fe04  ................
+000015d0: 0302 fd06 0510 0314 0114 0114 0114 0114  ................
+000015e0: 017a 2250 7265 4275 696c 6454 6573 7443  .z"PreBuildTestC
+000015f0: 6173 652e 7465 7374 5f6e 6f74 6966 795f  ase.test_notify_
+00001600: 7669 6265 7229 08da 085f 5f6e 616d 655f  viber)...__name_
+00001610: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001620: 5f71 7561 6c6e 616d 655f 5f72 3500 0000  _qualname__r5...
+00001630: 724b 0000 0072 5600 0000 725b 0000 00da  rK...rV...r[....
+00001640: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7239  .__classcell__r9
+00001650: 0000 0072 3900 0000 7237 0000 0072 3a00  ...r9...r7...r:.
+00001660: 0000 720d 0000 0015 0000 0073 0800 0000  ..r........s....
+00001670: 0801 0c24 081f 0848 720d 0000 0029 16da  ...$...Hr....)..
+00001680: 0664 6a61 6e67 6fda 026f 73da 1364 6a61  .django..os..dja
+00001690: 6e67 6f2e 7574 696c 732e 6372 7970 746f  ngo.utils.crypto
+000016a0: 7202 0000 00da 0875 6e69 7474 6573 7472  r......unittestr
+000016b0: 0300 0000 da13 646a 616e 676f 2e63 6f6e  ......django.con
+000016c0: 7472 6962 2e61 7574 6872 0400 0000 da1a  trib.authr......
+000016d0: 646a 616e 676f 2e63 6f6e 7472 6962 2e61  django.contrib.a
+000016e0: 7574 682e 6d6f 6465 6c73 7205 0000 005a  uth.modelsr....Z
+000016f0: 1467 6172 7069 785f 6e6f 7469 6679 2e6d  .garpix_notify.m
+00001700: 6f64 656c 7372 0600 0000 7207 0000 0072  odelsr....r....r
+00001710: 0800 0000 7209 0000 0072 0a00 0000 da1c  ....r....r......
+00001720: 6761 7270 6978 5f6e 6f74 6966 792e 6d6f  garpix_notify.mo
+00001730: 6465 6c73 2e63 686f 6963 6573 720b 0000  dels.choicesr...
+00001740: 00da 0765 6e76 6972 6f6e da0a 7365 7464  ...environ..setd
+00001750: 6566 6175 6c74 da05 7365 7475 7072 0d00  efault..setupr..
+00001760: 0000 7239 0000 0072 3900 0000 7239 0000  ..r9...r9...r9..
+00001770: 0072 3a00 0000 da08 3c6d 6f64 756c 653e  .r:.....<module>
+00001780: 0100 0000 731c 0000 0008 0108 020c 010c  ....s...........
+00001790: 020c 010c 020c 010c 010c 010c 010c 010c  ................
+000017a0: 020e 0108 03                             .....
```

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/__init__.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/category.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/category.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/config.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/fcm.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/fcm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/file.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/file.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/log.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/log.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/notify.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/notify.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/smtp.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/smtp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/template.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/__pycache__/user_list.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/admin/__pycache__/user_list.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/config.py` & `garpix_notify-5.9.0/garpix_notify/admin/config.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/notify.py` & `garpix_notify-5.9.0/garpix_notify/admin/notify.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/smtp.py` & `garpix_notify-5.9.0/garpix_notify/admin/smtp.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/template.py` & `garpix_notify-5.9.0/garpix_notify/admin/template.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/admin/user_list.py` & `garpix_notify-5.9.0/garpix_notify/admin/user_list.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/consumers.py` & `garpix_notify-5.9.0/garpix_notify/consumers.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/management/commands/__pycache__/garpix_notify_telegram.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/management/commands/__pycache__/garpix_notify_telegram.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/management/commands/garpix_notify_telegram.py` & `garpix_notify-5.9.0/garpix_notify/management/commands/garpix_notify_telegram.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/notify_mixin.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/notify_mixin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/mixins/__pycache__/user_notify_mixin.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/mixins/__pycache__/user_notify_mixin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/mixins/user_notify_mixin.py` & `garpix_notify-5.9.0/garpix_notify/mixins/user_notify_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/__init__.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/category.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/category.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/choices.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/choices.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/config.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/fcm.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/fcm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/file.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/file.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/log.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/log.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/notify.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/notify.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/smtp.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/smtp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/template.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/user_list.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/user_list.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/__pycache__/user_list_participant.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/models/__pycache__/user_list_participant.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/choices.py` & `garpix_notify-5.9.0/garpix_notify/models/choices.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/config.py` & `garpix_notify-5.9.0/garpix_notify/models/config.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/log.py` & `garpix_notify-5.9.0/garpix_notify/models/log.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/notify.py` & `garpix_notify-5.9.0/garpix_notify/models/notify.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/smtp.py` & `garpix_notify-5.9.0/garpix_notify/models/smtp.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/template.py` & `garpix_notify-5.9.0/garpix_notify/models/template.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/user_list.py` & `garpix_notify-5.9.0/garpix_notify/models/user_list.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/models/user_list_participant.py` & `garpix_notify-5.9.0/garpix_notify/models/user_list_participant.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/settings.py` & `garpix_notify-5.9.0/garpix_notify/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/setup.py` & `garpix_notify-5.9.0/garpix_notify/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_notify')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_notify',
-    version='5.8.0',
+    version='5.9.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_notify',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -39,12 +39,12 @@
         'django-ckeditor >= 5.6.1',
         'python-telegram-bot >= 12.6.1',
         'viberbot >= 1.0.11',
         'django-uuslug >= 1.2.0',
         'Pillow >= 8.2.0',
         'celery>=4.4.2',
         'redis >= 3.5.3',
-        'channels == 3.0.3',
-        'channels-redis == 3.3.1',
-        'asgiref == 3.2.10',
+        'channels == 3.0.4',
+        'channels-redis == 3.4.0',
+        'asgiref == 3.3.2',
     ],
 )
```

### Comparing `garpix_notify-5.8.0/garpix_notify/smtp.py` & `garpix_notify-5.9.0/garpix_notify/smtp.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/static/js/admin/garpix_notify.js` & `garpix_notify-5.9.0/garpix_notify/static/js/admin/garpix_notify.js`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/tasks/__pycache__/tasks.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/tasks/__pycache__/tasks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May 19 07:00:29 2022 UTC, .py size: 1691 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,112 @@
-00000000: 550d 0d0a 0000 0000 0deb 8562 9b06 0000  U..........b....
+00000000: 550d 0d0a 0000 0000 90fd bb62 ff06 0000  U..........b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
-00000070: 6406 6c0c 6d0d 5a0d 0100 6400 6407 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 0100 6504 6a10 6408 6409 8400  m.Z...e.j.d.d...
-00000090: 8301 5a11 6504 6a10 640a 640b 8400 8301  ..Z.e.j.d.d.....
-000000a0: 5a12 6504 6a13 6a14 a015 640c 640d 650d  Z.e.j.j...d.d.e.
-000000b0: a016 a100 6a17 640e 9c02 6901 a101 0100  ....j.d...i.....
-000000c0: 640f 6504 6a13 5f01 6410 5300 2911 e900  d.e.j._.d.S.)...
-000000d0: 0000 0029 01da 0874 696d 657a 6f6e 6529  ...)...timezone)
-000000e0: 01da 0361 7070 2901 da0d 6173 796e 635f  ...app)...async_
-000000f0: 746f 5f73 796e 6329 01da 1167 6574 5f63  to_sync)...get_c
-00000100: 6861 6e6e 656c 5f6c 6179 6572 2902 da05  hannel_layer)...
-00000110: 5354 4154 45da 0454 5950 4529 01da 0c4e  STATE..TYPE)...N
-00000120: 6f74 6966 7943 6f6e 6669 6729 01da 064e  otifyConfig)...N
-00000130: 6f74 6966 7963 0000 0000 0000 0000 0000  otifyc..........
-00000140: 0000 0200 0000 0300 0000 4300 0000 7364  ..........C...sd
-00000150: 0000 0074 006a 016a 0274 036a 0467 0164  ...t.j.j.t.j.g.d
-00000160: 018d 016a 0574 066a 0764 028d 017d 007c  ...j.t.j.d...}.|
-00000170: 00a0 08a1 0044 005d 3a7d 017c 016a 0974  .....D.]:}.|.j.t
-00000180: 036a 046b 0272 247c 016a 0a64 006b 0872  .j.k.r$|.j.d.k.r
-00000190: 487c 01a0 0ba1 0001 0071 2474 0ca0 0da1  H|.......q$t....
-000001a0: 007c 016a 0a6b 0472 247c 01a0 0ba1 0001  .|.j.k.r$|......
-000001b0: 0071 2464 0053 0029 034e 2901 5a09 7374  .q$d.S.).N).Z.st
-000001c0: 6174 655f 5f69 6e29 01da 0474 7970 6529  ate__in)...type)
-000001d0: 0e72 0900 0000 da07 6f62 6a65 6374 73da  .r......objects.
-000001e0: 0666 696c 7465 7272 0600 0000 da04 5741  .filterr......WA
-000001f0: 4954 da07 6578 636c 7564 6572 0700 0000  IT..excluder....
-00000200: da06 5359 5354 454d da08 6974 6572 6174  ..SYSTEM..iterat
-00000210: 6f72 da05 7374 6174 65da 0773 656e 645f  or..state..send_
-00000220: 6174 da05 5f73 656e 6472 0200 0000 da03  at.._sendr......
-00000230: 6e6f 7729 02da 086e 6f74 6966 6965 73da  now)...notifies.
-00000240: 066e 6f74 6966 79a9 0072 1700 0000 fa49  .notify..r.....I
-00000250: 2f55 7365 7273 2f63 7275 7361 742f 7072  /Users/crusat/pr
-00000260: 6f6a 6563 7473 2f67 6172 7069 785f 6e6f  ojects/garpix_no
-00000270: 7469 6679 2f62 6163 6b65 6e64 2f67 6172  tify/backend/gar
-00000280: 7069 785f 6e6f 7469 6679 2f74 6173 6b73  pix_notify/tasks
-00000290: 2f74 6173 6b73 2e70 79da 1273 656e 645f  /tasks.py..send_
-000002a0: 6e6f 7469 6669 6361 7469 6f6e 730b 0000  notifications...
-000002b0: 0073 1000 0000 0002 1c02 0c01 0c01 0a01  .s..............
-000002c0: 0a02 0e01 0a01 7219 0000 0063 0100 0000  ......r....c....
-000002d0: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
-000002e0: 4300 0000 73a6 0000 007a 6074 006a 016a  C...s....z`t.j.j
-000002f0: 027c 0064 018d 017d 017c 016a 0372 1e7c  .|.d...}.|.j.r.|
-00000300: 016a 037d 026e 0e64 027c 016a 046a 059b  .j.}.n.d.|.j.j..
-00000310: 009d 027d 0274 0674 0783 006a 0883 017c  ...}.t.t...j...|
-00000320: 027c 0064 037c 016a 097c 016a 0a64 049c  .|.d.|.j.|.j.d..
-00000330: 0483 0201 0074 0b6a 0c7c 015f 0d74 0ea0  .....t.j.|._.t..
-00000340: 0fa1 007c 015f 1057 006e 3804 0074 116b  ...|._.W.n8..t.k
-00000350: 0a72 9801 007d 0301 007a 1a74 0b6a 127c  .r...}...z.t.j.|
-00000360: 015f 0d7c 01a0 1374 147c 0383 01a1 0101  ._.|...t.|......
-00000370: 0057 0035 0064 007d 037e 0358 0059 006e  .W.5.d.}.~.X.Y.n
-00000380: 0258 007c 01a0 15a1 0001 0064 0053 0029  .X.|.......d.S.)
-00000390: 054e 2901 da02 706b 5a05 726f 6f6d 5f5a  .N)...pkZ.room_Z
-000003a0: 0b73 656e 645f 6e6f 7469 6679 2904 da02  .send_notify)...
-000003b0: 6964 720a 0000 00da 0565 7665 6e74 da07  idr......event..
-000003c0: 6d65 7373 6167 6529 1672 0900 0000 720b  message).r....r.
-000003d0: 0000 00da 0367 6574 da09 726f 6f6d 5f6e  .....get..room_n
-000003e0: 616d 65da 0475 7365 7272 1b00 0000 7204  ame..userr....r.
-000003f0: 0000 0072 0500 0000 5a0a 6772 6f75 705f  ...r....Z.group_
-00000400: 7365 6e64 721c 0000 00da 0468 746d 6c72  sendr......htmlr
-00000410: 0600 0000 da09 4445 4c49 5645 5245 4472  ......DELIVEREDr
-00000420: 1100 0000 7202 0000 0072 1400 0000 da07  ....r....r......
-00000430: 7365 6e74 5f61 74da 0945 7863 6570 7469  sent_at..Excepti
-00000440: 6f6e da08 5245 4a45 4354 4544 da06 746f  on..REJECTED..to
-00000450: 5f6c 6f67 da03 7374 72da 0473 6176 6529  _log..str..save)
-00000460: 045a 096e 6f74 6966 795f 706b da08 696e  .Z.notify_pk..in
-00000470: 7374 616e 6365 da0a 6772 6f75 705f 6e61  stance..group_na
-00000480: 6d65 da01 6572 1700 0000 7217 0000 0072  me..er....r....r
-00000490: 1800 0000 da19 7365 6e64 5f73 7973 7465  ......send_syste
-000004a0: 6d5f 6e6f 7469 6669 6361 7469 6f6e 7319  m_notifications.
-000004b0: 0000 0073 2800 0000 0002 0201 0e01 0601  ...s(...........
-000004c0: 0802 0e01 0a01 0202 0201 0201 0401 04fc  ................
-000004d0: 04fe 0409 0801 0e01 1001 0801 2001 0801  ............ ...
-000004e0: 722c 0000 005a 0d70 6572 696f 6469 635f  r,...Z.periodic_
-000004f0: 7461 736b 7a2c 6761 7270 6978 5f6e 6f74  taskz,garpix_not
-00000500: 6966 792e 7461 736b 732e 7461 736b 732e  ify.tasks.tasks.
-00000510: 7365 6e64 5f6e 6f74 6966 6963 6174 696f  send_notificatio
-00000520: 6e73 2902 da04 7461 736b da08 7363 6865  ns)...task..sche
-00000530: 6475 6c65 da03 5554 434e 2918 da0c 646a  dule..UTCN)...dj
-00000540: 616e 676f 2e75 7469 6c73 7202 0000 005a  ango.utilsr....Z
-00000550: 0a61 7070 2e63 656c 6572 7972 0300 0000  .app.celeryr....
-00000560: da0a 6365 6c65 7279 5f61 7070 da0c 6173  ..celery_app..as
-00000570: 6769 7265 662e 7379 6e63 7204 0000 005a  giref.syncr....Z
-00000580: 0f63 6861 6e6e 656c 732e 6c61 7965 7273  .channels.layers
-00000590: 7205 0000 005a 1c67 6172 7069 785f 6e6f  r....Z.garpix_no
-000005a0: 7469 6679 2e6d 6f64 656c 732e 6368 6f69  tify.models.choi
-000005b0: 6365 7372 0600 0000 7207 0000 005a 1b67  cesr....r....Z.g
-000005c0: 6172 7069 785f 6e6f 7469 6679 2e6d 6f64  arpix_notify.mod
-000005d0: 656c 732e 636f 6e66 6967 7208 0000 005a  els.configr....Z
-000005e0: 1b67 6172 7069 785f 6e6f 7469 6679 2e6d  .garpix_notify.m
-000005f0: 6f64 656c 732e 6e6f 7469 6679 7209 0000  odels.notifyr...
-00000600: 0072 2d00 0000 7219 0000 0072 2c00 0000  .r-...r....r,...
-00000610: da04 636f 6e66 da0d 6265 6174 5f73 6368  ..conf..beat_sch
-00000620: 6564 756c 65da 0675 7064 6174 65da 0867  edule..update..g
-00000630: 6574 5f73 6f6c 6fda 0870 6572 696f 6469  et_solo..periodi
-00000640: 6372 1700 0000 7217 0000 0072 1700 0000  cr....r....r....
-00000650: 7218 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000660: 0000 0073 2200 0000 0c01 0c01 0c01 0c02  ...s"...........
-00000670: 1001 0c01 0c03 0401 0a0d 0401 0a19 0801  ................
-00000680: 0201 0201 08fe 04ff 0606                 ..........
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6407 6c0d  m.Z.m.Z...d.d.l.
+00000080: 6d0e 5a0e 0100 6400 6408 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000090: 0100 6505 6501 6a11 8301 5a12 6512 6a13  ..e.e.j...Z.e.j.
+000000a0: 6409 640a 8400 8301 5a14 6512 6a13 640b  d.d.....Z.e.j.d.
+000000b0: 640c 8400 8301 5a15 6512 6a16 6a17 a018  d.....Z.e.j.j...
+000000c0: 640d 640e 650e a019 a100 6a1a 640f 9c02  d.d.e.....j.d...
+000000d0: 6901 a101 0100 6410 6512 6a16 5f03 6411  i.....d.e.j._.d.
+000000e0: 5300 2912 e900 0000 0029 01da 0873 6574  S.)......)...set
+000000f0: 7469 6e67 7329 01da 0874 696d 657a 6f6e  tings)...timezon
+00000100: 6529 01da 0d69 6d70 6f72 745f 7374 7269  e)...import_stri
+00000110: 6e67 2901 da0d 6173 796e 635f 746f 5f73  ng)...async_to_s
+00000120: 796e 6329 01da 1167 6574 5f63 6861 6e6e  ync)...get_chann
+00000130: 656c 5f6c 6179 6572 2902 da05 5354 4154  el_layer)...STAT
+00000140: 45da 0454 5950 4529 01da 0c4e 6f74 6966  E..TYPE)...Notif
+00000150: 7943 6f6e 6669 6729 01da 064e 6f74 6966  yConfig)...Notif
+00000160: 7963 0000 0000 0000 0000 0000 0000 0200  yc..............
+00000170: 0000 0300 0000 4300 0000 7364 0000 0074  ......C...sd...t
+00000180: 006a 016a 0274 036a 0467 0164 018d 016a  .j.j.t.j.g.d...j
+00000190: 0574 066a 0764 028d 017d 007c 00a0 08a1  .t.j.d...}.|....
+000001a0: 0044 005d 3a7d 017c 016a 0974 036a 046b  .D.]:}.|.j.t.j.k
+000001b0: 0272 247c 016a 0a64 006b 0872 487c 01a0  .r$|.j.d.k.rH|..
+000001c0: 0ba1 0001 0071 2474 0ca0 0da1 007c 016a  .....q$t.....|.j
+000001d0: 0a6b 0472 247c 01a0 0ba1 0001 0071 2464  .k.r$|.......q$d
+000001e0: 0053 0029 034e 2901 5a09 7374 6174 655f  .S.).N).Z.state_
+000001f0: 5f69 6e29 01da 0474 7970 6529 0e72 0a00  _in)...type).r..
+00000200: 0000 da07 6f62 6a65 6374 73da 0666 696c  ....objects..fil
+00000210: 7465 7272 0700 0000 da04 5741 4954 da07  terr......WAIT..
+00000220: 6578 636c 7564 6572 0800 0000 da06 5359  excluder......SY
+00000230: 5354 454d da08 6974 6572 6174 6f72 da05  STEM..iterator..
+00000240: 7374 6174 65da 0773 656e 645f 6174 da05  state..send_at..
+00000250: 5f73 656e 6472 0300 0000 da03 6e6f 7729  _sendr......now)
+00000260: 02da 086e 6f74 6966 6965 73da 066e 6f74  ...notifies..not
+00000270: 6966 79a9 0072 1800 0000 fa49 2f55 7365  ify..r.....I/Use
+00000280: 7273 2f63 7275 7361 742f 7072 6f6a 6563  rs/crusat/projec
+00000290: 7473 2f67 6172 7069 785f 6e6f 7469 6679  ts/garpix_notify
+000002a0: 2f62 6163 6b65 6e64 2f67 6172 7069 785f  /backend/garpix_
+000002b0: 6e6f 7469 6679 2f74 6173 6b73 2f74 6173  notify/tasks/tas
+000002c0: 6b73 2e70 79da 1273 656e 645f 6e6f 7469  ks.py..send_noti
+000002d0: 6669 6361 7469 6f6e 730f 0000 0073 1000  fications....s..
+000002e0: 0000 0002 1c02 0c01 0c01 0a01 0a02 0e01  ................
+000002f0: 0a01 721a 0000 0063 0100 0000 0000 0000  ..r....c........
+00000300: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
+00000310: 73a6 0000 0074 006a 016a 027c 0064 018d  s....t.j.j.|.d..
+00000320: 017d 017a 527c 016a 0372 1e7c 016a 037d  .}.zR|.j.r.|.j.}
+00000330: 026e 0e64 027c 016a 046a 059b 009d 027d  .n.d.|.j.j.....}
+00000340: 0274 0674 0783 006a 0883 017c 027c 0064  .t.t...j...|.|.d
+00000350: 037c 016a 097c 016a 0a64 049c 0483 0201  .|.j.|.j.d......
+00000360: 0074 0b6a 0c7c 015f 0d74 0ea0 0fa1 007c  .t.j.|._.t.....|
+00000370: 015f 1057 006e 3804 0074 116b 0a72 9801  ._.W.n8..t.k.r..
+00000380: 007d 0301 007a 1a74 0b6a 127c 015f 0d7c  .}...z.t.j.|._.|
+00000390: 01a0 1374 147c 0383 01a1 0101 0057 0035  ...t.|.......W.5
+000003a0: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
+000003b0: 01a0 15a1 0001 0064 0053 0029 054e 2901  .......d.S.).N).
+000003c0: da02 706b 5a05 726f 6f6d 5f5a 0b73 656e  ..pkZ.room_Z.sen
+000003d0: 645f 6e6f 7469 6679 2904 da02 6964 720b  d_notify)...idr.
+000003e0: 0000 00da 0565 7665 6e74 da07 6d65 7373  .....event..mess
+000003f0: 6167 6529 1672 0a00 0000 720c 0000 00da  age).r....r.....
+00000400: 0367 6574 da09 726f 6f6d 5f6e 616d 65da  .get..room_name.
+00000410: 0475 7365 7272 1c00 0000 7205 0000 0072  .userr....r....r
+00000420: 0600 0000 5a0a 6772 6f75 705f 7365 6e64  ....Z.group_send
+00000430: 721d 0000 00da 0468 746d 6c72 0700 0000  r......htmlr....
+00000440: da09 4445 4c49 5645 5245 4472 1200 0000  ..DELIVEREDr....
+00000450: 7203 0000 0072 1500 0000 da07 7365 6e74  r....r......sent
+00000460: 5f61 74da 0945 7863 6570 7469 6f6e da08  _at..Exception..
+00000470: 5245 4a45 4354 4544 da06 746f 5f6c 6f67  REJECTED..to_log
+00000480: da03 7374 72da 0473 6176 6529 045a 096e  ..str..save).Z.n
+00000490: 6f74 6966 795f 706b da08 696e 7374 616e  otify_pk..instan
+000004a0: 6365 da0a 6772 6f75 705f 6e61 6d65 da01  ce..group_name..
+000004b0: 6572 1800 0000 7218 0000 0072 1900 0000  er....r....r....
+000004c0: da19 7365 6e64 5f73 7973 7465 6d5f 6e6f  ..send_system_no
+000004d0: 7469 6669 6361 7469 6f6e 731d 0000 0073  tifications....s
+000004e0: 2600 0000 0002 0e01 0201 0601 0802 0e01  &...............
+000004f0: 0a01 0202 0201 0201 0401 04fc 04fe 0409  ................
+00000500: 0801 0e01 1001 0801 2001 722d 0000 005a  ........ .r-...Z
+00000510: 0d70 6572 696f 6469 635f 7461 736b 7a2c  .periodic_taskz,
+00000520: 6761 7270 6978 5f6e 6f74 6966 792e 7461  garpix_notify.ta
+00000530: 736b 732e 7461 736b 732e 7365 6e64 5f6e  sks.tasks.send_n
+00000540: 6f74 6966 6963 6174 696f 6e73 2902 da04  otifications)...
+00000550: 7461 736b da08 7363 6865 6475 6c65 da03  task..schedule..
+00000560: 5554 434e 291b da0b 646a 616e 676f 2e63  UTCN)...django.c
+00000570: 6f6e 6672 0200 0000 da0c 646a 616e 676f  onfr......django
+00000580: 2e75 7469 6c73 7203 0000 00da 1b64 6a61  .utilsr......dja
+00000590: 6e67 6f2e 7574 696c 732e 6d6f 6475 6c65  ngo.utils.module
+000005a0: 5f6c 6f61 6469 6e67 7204 0000 00da 0c61  _loadingr......a
+000005b0: 7367 6972 6566 2e73 796e 6372 0500 0000  sgiref.syncr....
+000005c0: 5a0f 6368 616e 6e65 6c73 2e6c 6179 6572  Z.channels.layer
+000005d0: 7372 0600 0000 5a1c 6761 7270 6978 5f6e  sr....Z.garpix_n
+000005e0: 6f74 6966 792e 6d6f 6465 6c73 2e63 686f  otify.models.cho
+000005f0: 6963 6573 7207 0000 0072 0800 0000 5a1b  icesr....r....Z.
+00000600: 6761 7270 6978 5f6e 6f74 6966 792e 6d6f  garpix_notify.mo
+00000610: 6465 6c73 2e63 6f6e 6669 6772 0900 0000  dels.configr....
+00000620: 5a1b 6761 7270 6978 5f6e 6f74 6966 792e  Z.garpix_notify.
+00000630: 6d6f 6465 6c73 2e6e 6f74 6966 7972 0a00  models.notifyr..
+00000640: 0000 da1d 4741 5250 4958 5f4e 4f54 4946  ....GARPIX_NOTIF
+00000650: 595f 4345 4c45 5259 5f53 4554 5449 4e47  Y_CELERY_SETTING
+00000660: 53da 0a63 656c 6572 795f 6170 7072 2e00  S..celery_appr..
+00000670: 0000 721a 0000 0072 2d00 0000 da04 636f  ..r....r-.....co
+00000680: 6e66 da0d 6265 6174 5f73 6368 6564 756c  nf..beat_schedul
+00000690: 65da 0675 7064 6174 65da 0867 6574 5f73  e..update..get_s
+000006a0: 6f6c 6fda 0870 6572 696f 6469 6372 1800  olo..periodicr..
+000006b0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000006c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000006d0: 2600 0000 0c01 0c01 0c01 0c01 0c02 1001  &...............
+000006e0: 0c01 0c03 0a03 0401 0a0d 0401 0a18 0801  ................
+000006f0: 0201 0201 08fe 04ff 0606                 ..........
```

### Comparing `garpix_notify-5.8.0/garpix_notify/tasks/tasks.py` & `garpix_notify-5.9.0/garpix_notify/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/tests.py` & `garpix_notify-5.9.0/garpix_notify/tests.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/call_code_cheker.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/call_code_cheker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/file.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/file.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/operators_data.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/operators_data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/receiving.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/receiving.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/send_data.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/send_data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/__pycache__/sms_checker.cpython-38.pyc` & `garpix_notify-5.9.0/garpix_notify/utils/__pycache__/sms_checker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/call_code_cheker.py` & `garpix_notify-5.9.0/garpix_notify/utils/call_code_cheker.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/operators_data.py` & `garpix_notify-5.9.0/garpix_notify/utils/operators_data.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/receiving.py` & `garpix_notify-5.9.0/garpix_notify/utils/receiving.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/send_data.py` & `garpix_notify-5.9.0/garpix_notify/utils/send_data.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/utils/sms_checker.py` & `garpix_notify-5.9.0/garpix_notify/utils/sms_checker.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify/views.py` & `garpix_notify-5.9.0/garpix_notify/views.py`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/garpix_notify.egg-info/PKG-INFO` & `garpix_notify-5.9.0/garpix_notify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-notify
-Version: 5.8.0
+Version: 5.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/garpixcms/garpix_notify
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `garpix_notify-5.8.0/garpix_notify.egg-info/SOURCES.txt` & `garpix_notify-5.9.0/garpix_notify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_notify-5.8.0/setup.py` & `garpix_notify-5.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_notify')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_notify',
-    version='5.8.0',
+    version='5.9.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_notify',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -39,12 +39,12 @@
         'django-ckeditor >= 5.6.1',
         'python-telegram-bot >= 12.6.1',
         'viberbot >= 1.0.11',
         'django-uuslug >= 1.2.0',
         'Pillow >= 8.2.0',
         'celery>=4.4.2',
         'redis >= 3.5.3',
-        'channels == 3.0.3',
-        'channels-redis == 3.3.1',
-        'asgiref == 3.2.10',
+        'channels == 3.0.4',
+        'channels-redis == 3.4.0',
+        'asgiref == 3.3.2',
     ],
 )
```

