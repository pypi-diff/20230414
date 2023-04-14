# Comparing `tmp/comwares-0.1.4.tar.gz` & `tmp/comwares-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/comwares-0.1.4.tar", last modified: Thu Apr 13 18:36:35 2023, max compression
+gzip compressed data, was "dist/comwares-0.1.5.tar", last modified: Fri Apr 14 08:59:26 2023, max compression
```

## Comparing `comwares-0.1.4.tar` & `comwares-0.1.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.520939 comwares-0.1.4/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:36:35.520358 comwares-0.1.4/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.4/README.md
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.485500 comwares-0.1.4/comwares/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      219 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.490157 comwares-0.1.4/comwares/captcha/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.4/comwares/captcha/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3942 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/captcha/captcha_dev.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1440 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/captcha/icredit_captcha.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.4/comwares/captcha/slider.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.495625 comwares-0.1.4/comwares/commons/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.4/comwares/commons/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/commons/logger.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/md5.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/path_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.4/comwares/commons/sorting.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.4/comwares/commons/string_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/time_funcs.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.496753 comwares-0.1.4/comwares/crawler/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.4/comwares/crawler/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/crawler/user_agents.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.500622 comwares-0.1.4/comwares/data/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.4/comwares/data/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/data/loaders.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/data/mongo_to_pg.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.4/comwares/data/pandas_utils.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/data/pg_utils.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.503050 comwares-0.1.4/comwares/decorators/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.4/comwares/decorators/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.4/comwares/decorators/batchify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.4/comwares/decorators/time.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.505889 comwares-0.1.4/comwares/e-mail/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/e-mail/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.4/comwares/e-mail/check.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/e-mail/exmail.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.4/comwares/e-mail/send.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.508669 comwares-0.1.4/comwares/google/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/auth.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3199 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/google/gdrive.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/sheets.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      861 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/google/values.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.510347 comwares-0.1.4/comwares/image/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.4/comwares/image/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/image/io.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.4/comwares/image/visualize.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.512593 comwares-0.1.4/comwares/pdf/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.4/comwares/pdf/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.4/comwares/pdf/b64_transfer.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.4/comwares/pdf/pdf_analyzer.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.515188 comwares-0.1.4/comwares/tencent/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/tencent/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 comwares-0.1.4/comwares/tencent/cos.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.4/comwares/tencent/sms.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.4/comwares/tencent/translate.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.516317 comwares-0.1.4/comwares/traffic/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.4/comwares/traffic/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.4/comwares/traffic/alexacn.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.517251 comwares-0.1.4/comwares/video/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.4/comwares/video/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.4/comwares/video/snap.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.519588 comwares-0.1.4/comwares/webhooks/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.4/comwares/webhooks/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.4/comwares/webhooks/chanify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.4/comwares/webhooks/feishu.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.4/comwares/webhooks/work_weixin.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.487539 comwares-0.1.4/comwares.egg-info/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1540 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/SOURCES.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/dependency_links.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/requires.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        9 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/top_level.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-13 18:36:35.521044 comwares-0.1.4/setup.cfg
--rw-r--r--   0 kevinzhu   (501) staff       (20)      897 2023-04-13 18:36:05.000000 comwares-0.1.4/setup.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.943061 comwares-0.1.5/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-14 08:59:26.942245 comwares-0.1.5/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.5/README.md
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.912693 comwares-0.1.5/comwares/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:58:27.000000 comwares-0.1.5/comwares/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.916308 comwares-0.1.5/comwares/captcha/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.5/comwares/captcha/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3942 2023-04-13 17:21:15.000000 comwares-0.1.5/comwares/captcha/captcha_dev.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1440 2023-04-13 17:21:15.000000 comwares-0.1.5/comwares/captcha/icredit_captcha.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.5/comwares/captcha/slider.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.920835 comwares-0.1.5/comwares/commons/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.5/comwares/commons/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/commons/logger.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.5/comwares/commons/md5.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.5/comwares/commons/path_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.5/comwares/commons/sorting.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.5/comwares/commons/string_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.5/comwares/commons/time_funcs.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.921831 comwares-0.1.5/comwares/crawler/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.5/comwares/crawler/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/crawler/user_agents.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.924841 comwares-0.1.5/comwares/data/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.5/comwares/data/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/data/loaders.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.5/comwares/data/mongo_to_pg.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.5/comwares/data/pandas_utils.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.5/comwares/data/pg_utils.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.926408 comwares-0.1.5/comwares/decorators/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.5/comwares/decorators/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.5/comwares/decorators/batchify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.5/comwares/decorators/time.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.928497 comwares-0.1.5/comwares/e-mail/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/e-mail/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.5/comwares/e-mail/check.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.5/comwares/e-mail/exmail.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.5/comwares/e-mail/send.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.931273 comwares-0.1.5/comwares/google/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/google/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/google/auth.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3199 2023-04-13 17:21:15.000000 comwares-0.1.5/comwares/google/gdrive.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/google/sheets.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      861 2023-04-13 17:21:15.000000 comwares-0.1.5/comwares/google/values.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.932687 comwares-0.1.5/comwares/image/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.5/comwares/image/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.5/comwares/image/io.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.5/comwares/image/visualize.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.934327 comwares-0.1.5/comwares/pdf/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.5/comwares/pdf/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.5/comwares/pdf/b64_transfer.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.5/comwares/pdf/pdf_analyzer.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.937120 comwares-0.1.5/comwares/tencent/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.5/comwares/tencent/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 comwares-0.1.5/comwares/tencent/cos.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.5/comwares/tencent/sms.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.5/comwares/tencent/translate.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.937887 comwares-0.1.5/comwares/traffic/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.5/comwares/traffic/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.5/comwares/traffic/alexacn.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.938695 comwares-0.1.5/comwares/video/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.5/comwares/video/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.5/comwares/video/snap.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.941106 comwares-0.1.5/comwares/webhooks/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.5/comwares/webhooks/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.5/comwares/webhooks/chanify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.5/comwares/webhooks/feishu.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.5/comwares/webhooks/work_weixin.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-14 08:59:26.914384 comwares-0.1.5/comwares.egg-info/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-14 08:59:26.000000 comwares-0.1.5/comwares.egg-info/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1540 2023-04-14 08:59:26.000000 comwares-0.1.5/comwares.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-14 08:59:26.000000 comwares-0.1.5/comwares.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-14 08:59:26.000000 comwares-0.1.5/comwares.egg-info/requires.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        9 2023-04-14 08:59:26.000000 comwares-0.1.5/comwares.egg-info/top_level.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-14 08:59:26.943259 comwares-0.1.5/setup.cfg
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      897 2023-04-14 08:59:23.000000 comwares-0.1.5/setup.py
```

### Comparing `comwares-0.1.4/comwares/captcha/captcha_dev.py` & `comwares-0.1.5/comwares/captcha/captcha_dev.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/captcha/icredit_captcha.py` & `comwares-0.1.5/comwares/captcha/icredit_captcha.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/captcha/slider.py` & `comwares-0.1.5/comwares/captcha/slider.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/commons/logger.py` & `comwares-0.1.5/comwares/commons/logger.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/commons/path_funcs.py` & `comwares-0.1.5/comwares/commons/path_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/commons/time_funcs.py` & `comwares-0.1.5/comwares/commons/time_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/data/mongo_to_pg.py` & `comwares-0.1.5/comwares/data/mongo_to_pg.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/data/pandas_utils.py` & `comwares-0.1.5/comwares/data/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/data/pg_utils.py` & `comwares-0.1.5/comwares/data/pg_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/decorators/batchify.py` & `comwares-0.1.5/comwares/decorators/batchify.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/decorators/time.py` & `comwares-0.1.5/comwares/decorators/time.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/e-mail/check.py` & `comwares-0.1.5/comwares/e-mail/check.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/e-mail/exmail.py` & `comwares-0.1.5/comwares/e-mail/exmail.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/e-mail/send.py` & `comwares-0.1.5/comwares/e-mail/send.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/google/auth.py` & `comwares-0.1.5/comwares/google/auth.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/google/gdrive.py` & `comwares-0.1.5/comwares/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/google/values.py` & `comwares-0.1.5/comwares/google/values.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/image/io.py` & `comwares-0.1.5/comwares/image/io.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/pdf/b64_transfer.py` & `comwares-0.1.5/comwares/pdf/b64_transfer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/pdf/pdf_analyzer.py` & `comwares-0.1.5/comwares/pdf/pdf_analyzer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/tencent/cos.py` & `comwares-0.1.5/comwares/tencent/cos.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/tencent/sms.py` & `comwares-0.1.5/comwares/tencent/sms.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/tencent/translate.py` & `comwares-0.1.5/comwares/tencent/translate.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/traffic/alexacn.py` & `comwares-0.1.5/comwares/traffic/alexacn.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/video/snap.py` & `comwares-0.1.5/comwares/video/snap.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/webhooks/feishu.py` & `comwares-0.1.5/comwares/webhooks/feishu.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares/webhooks/work_weixin.py` & `comwares-0.1.5/comwares/webhooks/work_weixin.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/comwares.egg-info/SOURCES.txt` & `comwares-0.1.5/comwares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comwares-0.1.4/setup.py` & `comwares-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="comwares",
-    version="0.1.4",
+    version="0.1.5",
     author="Kevin Zhu",
     description="This project provides middlewares for a startup company.",
     packages=find_packages(),
     install_requires=[
         'tencentcloud_sdk_python',
         'cos_python_sdk_v5',
         'ffmpeg',
```

