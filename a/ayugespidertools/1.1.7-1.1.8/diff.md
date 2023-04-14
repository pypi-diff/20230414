# Comparing `tmp/ayugespidertools-1.1.7.tar.gz` & `tmp/ayugespidertools-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-1.1.7.tar", max compression
+gzip compressed data, was "ayugespidertools-1.1.8.tar", max compression
```

## Comparing `ayugespidertools-1.1.7.tar` & `ayugespidertools-1.1.8.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/LICENSE
--rw-r--r--   0        0        0    12951 2023-04-10 09:42:27.000000 ayugespidertools-1.1.7/README.md
--rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyuRequest.py
--rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyugeCrawlSpider.py
--rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyugeSpider.py
--rw-r--r--   0        0        0     8185 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/DownloaderMiddlewares.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.7/ayugespidertools/FormatData.py
--rw-r--r--   0        0        0     9527 2023-03-30 01:53:24.000000 ayugespidertools-1.1.7/ayugespidertools/ImgOperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.7/ayugespidertools/Items.py
--rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/Middlewares.py
--rw-r--r--   0        0        0     8545 2023-04-11 06:06:53.000000 ayugespidertools-1.1.7/ayugespidertools/MongoClient.py
--rw-r--r--   0        0        0     1150 2023-04-04 01:32:28.000000 ayugespidertools-1.1.7/ayugespidertools/MysqlClient.py
--rw-r--r--   0        0        0     5480 2023-03-17 03:03:53.000000 ayugespidertools-1.1.7/ayugespidertools/Oss.py
--rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/Pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/ProcessManager.py
--rw-r--r--   0        0        0     2409 2023-04-06 07:08:21.000000 ayugespidertools-1.1.7/ayugespidertools/RPA.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/RunJs.py
--rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/VerificationCode.py
--rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.7/ayugespidertools/__init__.py
--rw-r--r--   0        0        0     7227 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0     7109 2023-03-29 02:02:32.428686 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2947 2023-03-29 02:02:32.473687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1158 2023-03-29 02:02:32.506687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.7/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4072 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      626 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0     3095 2023-03-30 03:16:54.000000 ayugespidertools-1.1.7/ayugespidertools/common/Encryption.py
--rw-r--r--   0        0        0     6458 2023-04-11 06:00:18.000000 ayugespidertools-1.1.7/ayugespidertools/common/Expend.py
--rw-r--r--   0        0        0     3832 2023-04-11 07:28:36.000000 ayugespidertools-1.1.7/ayugespidertools/common/MongoDBPipe.py
--rw-r--r--   0        0        0    11894 2023-04-11 06:29:34.000000 ayugespidertools-1.1.7/ayugespidertools/common/MultiPlexing.py
--rw-r--r--   0        0        0    12983 2023-04-11 07:26:18.000000 ayugespidertools-1.1.7/ayugespidertools/common/MysqlErrorHandle.py
--rw-r--r--   0        0        0    32543 2023-04-11 07:27:48.000000 ayugespidertools-1.1.7/ayugespidertools/common/Params.py
--rw-r--r--   0        0        0     4264 2023-04-11 07:33:08.000000 ayugespidertools-1.1.7/ayugespidertools/common/SpiderDBConf.py
--rw-r--r--   0        0        0     3726 2023-04-11 07:35:01.000000 ayugespidertools-1.1.7/ayugespidertools/common/SqlFormat.py
--rw-r--r--   0        0        0     1421 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/common/TypeVars.py
--rw-r--r--   0        0        0    11146 2023-04-11 07:54:51.000000 ayugespidertools-1.1.7/ayugespidertools/common/Utils.py
--rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/common/YiDunGap.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0      455 2023-03-15 08:01:04.000000 ayugespidertools-1.1.7/ayugespidertools/config.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11139 2023-04-11 07:45:49.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-10 09:37:46.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13257 2023-04-11 03:04:29.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     2823 2023-04-11 02:54:07.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     2086 2023-04-10 07:23:47.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3899 2023-04-11 03:05:04.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-10 01:20:43.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     6119 2023-04-04 17:02:00.663859 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      777 2023-03-29 02:02:30.564685 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
--rw-r--r--   0        0        0      450 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      630 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
--rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4604 2023-03-15 09:36:02.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5953 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     3073 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    14673 1970-01-01 00:00:00.000000 ayugespidertools-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/LICENSE
+-rw-r--r--   0        0        0    13472 2023-04-14 08:11:10.000000 ayugespidertools-1.1.8/README.md
+-rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyuRequest.py
+-rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyugeCrawlSpider.py
+-rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyugeSpider.py
+-rw-r--r--   0        0        0     8257 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/DownloaderMiddlewares.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.8/ayugespidertools/FormatData.py
+-rw-r--r--   0        0        0     7681 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/ImgOperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.8/ayugespidertools/Items.py
+-rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/Middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/MongoClient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/MysqlClient.py
+-rw-r--r--   0        0        0     5475 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/Oss.py
+-rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/Pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/ProcessManager.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/RPA.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/RunJs.py
+-rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/VerificationCode.py
+-rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.8/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0     7227 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0     7109 2023-03-29 02:02:32.428686 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2947 2023-03-29 02:02:32.473687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1158 2023-03-29 02:02:32.506687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.8/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4072 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      626 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0     3704 2023-04-14 07:32:45.000000 ayugespidertools-1.1.8/ayugespidertools/common/Encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-14 08:08:19.000000 ayugespidertools-1.1.8/ayugespidertools/common/Expend.py
+-rw-r--r--   0        0        0     3832 2023-04-11 07:28:36.000000 ayugespidertools-1.1.8/ayugespidertools/common/MongoDBPipe.py
+-rw-r--r--   0        0        0    11869 2023-04-14 06:07:52.000000 ayugespidertools-1.1.8/ayugespidertools/common/MultiPlexing.py
+-rw-r--r--   0        0        0    13474 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/common/MysqlErrorHandle.py
+-rw-r--r--   0        0        0    32577 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/common/Params.py
+-rw-r--r--   0        0        0     4264 2023-04-11 07:33:08.000000 ayugespidertools-1.1.8/ayugespidertools/common/SpiderDBConf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-1.1.8/ayugespidertools/common/SqlFormat.py
+-rw-r--r--   0        0        0     1421 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/common/TypeVars.py
+-rw-r--r--   0        0        0    11610 2023-04-13 08:18:25.000000 ayugespidertools-1.1.8/ayugespidertools/common/Utils.py
+-rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/common/YiDunGap.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-1.1.8/ayugespidertools/config.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11208 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-12 02:07:09.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13312 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     2823 2023-04-11 02:54:07.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3899 2023-04-11 03:05:04.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-10 01:20:43.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-13 07:18:00.730130 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-13 07:18:02.706131 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      630 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
+-rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4647 2023-04-14 08:26:26.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5953 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     3094 2023-04-12 09:55:12.000000 ayugespidertools-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    15149 1970-01-01 00:00:00.000000 ayugespidertools-1.1.8/PKG-INFO
```

### Comparing `ayugespidertools-1.1.7/LICENSE` & `ayugespidertools-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/README.md` & `ayugespidertools-1.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -156,43 +156,42 @@
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
 
 比如你可能需要更新依赖库中 `pymongo` 为新版本 `x.x.x`，那只需 `poetry install` 安装现有依赖后，再 `poetry add pymongo@x.x.x` 安装目标版本（尽量不要使用 `poetry update pymongo`），确定测试正常了即可 `poetry build` 打包使用。
 
 ## TodoList
 
 - [x] `scrapy` 的扩展功能场景
-  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [ ] ~~`selenium`: 性能没有 `pyppeteer` 强~~
-    - [x] `pyppeteer`: `Gerapy-pyppeteer` 库已经实现此功能
     - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
-    - [ ] ~~`splash`: 继承 `splash` 渲染 `js` 的功能~~
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
   - [ ] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
 - [x] 常用开发场景
   - [x] `sql` 语句拼接，只是简单场景，后续优化。已给出优化方向，参考库等信息。
   - [x] `mongoDB` 语句拼接
   - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
-  - [ ] 字体反爬还原方法
+  - [x] 字体反爬还原方法
+    - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
+      - [x] 可以直接在字体文件 `xml` 中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
+      - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`，后再通过各种方式识别。
   - [x] `html` 格式转 `markdown` 格式
   - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等等等
   - [x] 添加常用的图片验证码中的处理方法
     - [x] 滑块缺口距离的识别方法（多种实现方式）
     - [x] 根据滑块距离生成轨迹数组的方法
     - [x] 识别点选验证码位置及点击顺序，识别结果不太好，待优化
     - [x] 图片乱序混淆的还原方法示例
 
-注：
+**注：**
 
-- 不再开发结合 `selenium` 扩展的功能，推荐使用 `scrapy-playwright`，`Gerapy-pyppeteer` 等其它库；
-- 不再开发结合 `splash` 的功能，如果使用 `splash http api` 的话，在 `scrapy` ，本库或自写脚本中都比较容易扩展。如果要使用 `lua` `api` 等复杂的功能那还是推荐 `scrapy-splash` 这类的扩展库。
+1. 由于 `scrapy` 扩展库的开源项目众多，在使用本库的基础上扩展它们，与使用 `scrapy` 时扩展它们的用法一致，所以不再开发一些其它工具已经拥有且稳定的功能，但也会尽量开发一些常用且通用的方法来提升效率。
+2. 字体反爬部分不会给出详细解决示例，不管是使用 `fontforge`，`fontTools` 或 `ocr` 等工具，已经脱离本库的范围了，我会给出部分依赖的方法，但不会添加以上工具库的依赖了，而导致本库依赖过于杂糅。而且，若要实现高可用的字体映射也比较简单，请自行实现，可能会考虑新开 `pypi` 库来实现此部分。
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/DownloaderMiddlewares.py` & `ayugespidertools-1.1.8/ayugespidertools/DownloaderMiddlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import urllib.parse
 
 import aiohttp
 from scrapy.http import HtmlResponse
 
 from ayugespidertools.common.MultiPlexing import ReuseOperation
 from ayugespidertools.common.Params import Param
 from ayugespidertools.common.Utils import ToolsForAyu
@@ -71,17 +70,18 @@
         使用 aiohttp 来 process spider
         """
         aiohttp_meta = request.meta.get("aiohttp_args", {})
         assert isinstance(aiohttp_meta, dict), "aiohttp_args 参数的格式不是 dict，请查看！"
 
         # set proxy
 
+        # todo: 此部分中的 domain 参数暂时不使用，后续考虑是否需要
         # set cookies domain 参数
-        parse_result = urllib.parse.urlsplit(request.url)
-        domain = parse_result.hostname
+        # parse_result = urllib.parse.urlsplit(request.url)
+        # domain = parse_result.hostname
 
         # _timeout = self.download_timeout
         # if aiohttp_meta.get('timeout') is not None:
         #     _timeout = aiohttp_meta.get('timeout')
 
         spider.slog.debug(f"crawling {request.url}")
         html_content = None
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/FormatData.py` & `ayugespidertools-1.1.8/ayugespidertools/FormatData.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/ImgOperation.py` & `ayugespidertools-1.1.8/ayugespidertools/ImgOperation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional, Union
 
 import cv2
-import requests
 from PIL import Image
 
 from ayugespidertools.common.Encryption import EncryptOperation
 from ayugespidertools.common.MultiPlexing import ReuseOperation
 
 __all__ = [
     "Picture",
@@ -14,56 +13,14 @@
 
 class Picture(object):
     """
     对验证码图片的一些操作
     """
 
     @classmethod
-    def get_captcha(cls, url: str, img_path: str) -> None:
-        """
-        下载完美滑块的图片，并将缺口图和滑块在一起的图片切割
-        Args:
-            url: 完美滑块的滑块图片链接
-            img_path: 图片保存路径
-
-        Returns:
-            None
-        """
-        session = requests.Session()
-        session.headers = {
-            "authority": "captchas-1251008858.file.myqcloud.com",
-            "pragma": "no-cache",
-            "cache-control": "no-cache",
-            "sec-ch-ua": '" Not;A Brand";v="99", "Google Chrome";v="91", "Chromium";v="91"',
-            "sec-ch-ua-mobile": "?0",
-            "upgrade-insecure-requests": "1",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36",
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "sec-fetch-site": "none",
-            "sec-fetch-mode": "navigate",
-            "sec-fetch-user": "?1",
-            "sec-fetch-dest": "document",
-            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
-        }
-        text = session.get(url).content
-        with open(f"{img_path}/captcha.png", "wb") as f:
-            f.write(text)
-
-        # 新建空白图片
-        # captcha = Image.new('RGB', (50, 120))
-        # 实例化原始图片 Image 对象
-        img = Image.open(f"{img_path}/captcha.png")
-
-        # 切割滑块验证码图片，将背景图和滑块图分开
-        # (left, upper, right, lower)
-        captcha = img.crop((260, 0, 325, 120 - 4))
-        captcha = captcha.convert("RGBA")
-        captcha.save(f"{img_path}/captcha_slide.png")
-
-    @classmethod
     def convert_index_to_offset(cls, index):
         """
         获取每张小图的偏移量
         Args:
             index: 当前小块图片
 
         Returns:
@@ -142,25 +99,25 @@
         Args:
             slide_data: 完美滑块重组所需的数组
 
         Returns:
             true_pic_list: 真实图片的顺序坐标
         """
         c = 260
-        d = 120
-        l = 20
-        s = 9
-        a = 61
+        # d = 120
+        _l = 20
+        # s = 9
+        # a = 61
         true_pic_list = []
         for curr_data in slide_data:
             curr_position_list = []
-            if curr_data < l:
-                curr_position_list.extend((int(c / l * curr_data), 0))
+            if curr_data < _l:
+                curr_position_list.extend((int(c / _l * curr_data), 0))
             else:
-                curr_position_list.extend((int(c / l * (curr_data % l)), 60))
+                curr_position_list.extend((int(c / _l * (curr_data % _l)), 60))
             true_pic_list.append(curr_position_list)
         return true_pic_list
 
     @classmethod
     def find_pic(cls, target, template):
         """
         找出图像中最佳匹配位置
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/Items.py` & `ayugespidertools-1.1.8/ayugespidertools/Items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/Middlewares.py` & `ayugespidertools-1.1.8/ayugespidertools/Middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/MongoClient.py` & `ayugespidertools-1.1.8/ayugespidertools/MongoClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional
 
-from gridfs import *
+from gridfs import GridFS
 from pymongo import MongoClient
 
 __all__ = [
     "MongoDbBase",
 ]
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/MysqlClient.py` & `ayugespidertools-1.1.8/ayugespidertools/MysqlClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional
+from typing import Literal
 
 import pymysql
 
 __all__ = [
     "MysqlOrm",
 ]
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/Oss.py` & `ayugespidertools-1.1.8/ayugespidertools/Oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             ).content
 
         try:
             self.bucket.put_object(
                 f"{self.operateDoc}/{input_file_name}.{file_format}",
                 put_bytes_or_url,
             )
-        except Exception as e:
+        except Exception:
             return False, ""
         return True, input_file_name
 
     def enumer_file_by_pre(
         self, prefix: str, count_by_type: Union[Param.Str_Lstr, Param.NoneType] = None
     ) -> list:
         """
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/Pipelines.py` & `ayugespidertools-1.1.8/ayugespidertools/Pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/RPA.py` & `ayugespidertools-1.1.8/ayugespidertools/RPA.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
                 # logger.info("quit process success")
                 cls.quit_process(
                     process_name="curr_process", sudo_pwd="自行替换 sudo root 的密码"
                 )
 
             # 当最新四行日志中未出现 scrapy 统计，则为正常状态，并清空日志
             elif block_times == 0:
-                clean_log = subprocess.getstatusoutput(f"> {fn}")
+                subprocess.getstatusoutput(f"> {fn}")
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/RunJs.py` & `ayugespidertools-1.1.8/ayugespidertools/RunJs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/VerificationCode.py` & `ayugespidertools-1.1.8/ayugespidertools/VerificationCode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/startproject.py` & `ayugespidertools-1.1.8/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/commands/version.py` & `ayugespidertools-1.1.8/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/Encryption.py` & `ayugespidertools-1.1.8/ayugespidertools/common/Encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import hashlib
+import re
 from typing import Union
 
 import mmh3
 from Crypto.Cipher import PKCS1_v1_5 as Cipher_pkcsl_v1_5
 from Crypto.PublicKey import RSA
 
 __all__ = [
@@ -94,7 +95,23 @@
 
         Returns:
             1). mmh3 hash128 后的结果
         """
         o = mmh3.hash128(encode_data)
         hash128_encoded = hex(((o & 0xFFFFFFFFFFFFFFFF) << 64) + (o >> 64))
         return hash128_encoded[2:]
+
+    @staticmethod
+    def uni_to_chr(uni: str) -> str:
+        """
+        将 Unicode 码位表示的字符串转换正常的字符，用于获取字体映射时使用
+        Args:
+            uni: 需要转换的 unicode 字符串，
+                如：006A，但它可能是非标准的，可能需要去掉前面的 0x 或 uni。
+
+        Returns:
+            1). 转换后的字符
+        """
+        _uni = re.sub(r"^(0x|U\+|uni)", "", uni)
+        unicode_value = int(_uni, 16)
+        # 使用 chr() 函数将整数值转换为字符
+        return chr(unicode_value)
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/Expend.py` & `ayugespidertools-1.1.8/ayugespidertools/common/Expend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-import datetime
-
-import pymysql
-from retrying import retry
-
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import MysqlConfig
-from ayugespidertools.config import logger
-
-__all__ = [
-    "MysqlPipeEnhanceMixin",
-]
-
-
-class MysqlPipeEnhanceMixin(object):
-    """
-    用于扩展 pipelines 中的功能，作为 Mixin 使用，不要对其实例化和单独使用等
-    """
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def _connect(
-        self,
-        mysql_conf: MysqlConfig,
-    ) -> pymysql.connections.Connection:
-        """
-        链接数据库操作：
-            1.如果链接正常，则返回链接句柄；
-            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
-        Args:
-            mysql_conf: pymysql 链接所需的参数
-
-        Returns:
-            1).pymysql.connections.Connection, 链接句柄
-        """
-        try:
-            conn = pymysql.connect(
-                user=mysql_conf.user,
-                password=mysql_conf.password,
-                host=mysql_conf.host,
-                port=mysql_conf.port,
-                database=mysql_conf.database,
-                charset=mysql_conf.charset,
-            )
-        except Exception as e:
-            logger.warning(f"目标数据库：{mysql_conf.database} 不存在，尝试创建中...")
-            if "1049" in str(e):
-                # 如果连接目标数据库报不存在的错误时，先创建出此目标数据库
-                ReuseOperation.create_database(mysql_conf)
-        else:
-            # 连接没有问题就直接返回连接对象
-            return conn
-        # 出现数据库不存在问题后，在创建数据库 create_database 后，再次返回连接对象
-        return pymysql.connect(
-            user=mysql_conf.user,
-            password=mysql_conf.password,
-            host=mysql_conf.host,
-            port=mysql_conf.port,
-            database=mysql_conf.database,
-            charset=mysql_conf.charset,
-        )
-
-    def _get_sql_by_item(self, table: str, item: dict) -> str:
-        """
-        根据处理后的 item 生成 sql 插入语句
-        Args:
-            table: 数据库表名
-            item: 处理后的 item
-
-        Returns:
-            1). sql 插入语句
-        """
-        keys = f"""`{"`, `".join(item.keys())}`"""
-        values = ", ".join(["%s"] * len(item))
-        update = ",".join([f" `{key}` = %s" for key in item])
-        return f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-
-    def _get_log_by_spider(self, spider, crawl_time):
-        """
-        获取 spider 的运行日志情况
-        Args:
-            spider: scrapy spider
-            crawl_time: 爬取时间
-
-        Returns:
-            log_info: 日志信息
-        """
-        mysql_conf = spider.mysql_conf
-        text = {}
-        stats = spider.stats.get_stats()
-        error_reason = ""
-        for k, v in stats.items():
-            if isinstance(v, datetime.datetime):
-                text[k.replace("/", "_")] = (v + datetime.timedelta(hours=8)).strftime(
-                    "%Y-%m-%d %H:%M:%S"
-                )
-            else:
-                if all(
-                    [
-                        "response_status_count" in k,
-                        k != "downloader/response_status_count/200",
-                    ]
-                ):
-                    status_code = k.split("/")[-1] if len(k.split("/")) > 0 else ""
-                    if status_code.startswith("4"):
-                        if status_code == "429":
-                            error_reason += f"{status_code}错误：代理超过使用频率限制"
-                        else:
-                            error_reason += f"{status_code}错误：网页失效/无此网页/网站拒绝访问"
-                    elif status_code.startswith("5"):
-                        error_reason += f"{status_code}错误：网站服务器处理出错"
-                    elif status_code != "":
-                        error_reason += f"{status_code}:待人工排查原因"
-                elif "exception_type_count" in k:
-                    error_name = k.split("/")[-1]
-                    if "Timeout" in error_name:
-                        error_reason += f"{error_name}:网站响应超时错误 "
-                    elif "ConnectionDone" in error_name:
-                        error_reason += f"{error_name}:网站与脚本连接断开 "
-                    else:
-                        # "ResponseNeverReceived" or "ResponseFailed"
-                        error_reason += f"{error_name}:网站无响应 "
-                text[k.replace("/", "_")] = v
-
-        log_info = {
-            "database": mysql_conf["database"],
-            # 脚本名称
-            "spider_name": spider.name,
-            # uid
-            "uid": f'{mysql_conf["database"]}|{spider.name}',
-            # 请求次数统计
-            "request_counts": text.get("downloader_request_count", 0),
-            # 接收次数统计
-            "received_count": text.get("response_received_count", 0),
-            # 采集数据量
-            "item_counts": text.get("item_scraped_count", 0),
-            # info 数据统计
-            "info_count": text.get("log_count_INFO", 0),
-            # 警告数据统计
-            "warning_count": text.get("log_count_WARNING", 0),
-            # 错误数据统计
-            "error_count": text.get("log_count_ERROR", 0),
-            # 开始时间
-            "start_time": text.get("start_time"),
-            # 结束时间
-            "finish_time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-            # 花费时间
-            "spend_minutes": round(
-                (
-                    datetime.datetime.now()
-                    - stats.get("start_time")
-                    - datetime.timedelta(hours=8)
-                ).seconds
-                / 60,
-                2,
-            ),
-            "crawl_time": crawl_time,
-        }
-
-        # 错误原因
-        if text.get("log_count_ERROR", 0):
-            log_info["log_count_ERROR"] = error_reason or "请人工排查错误原因！"
-
-        else:
-            log_info["log_count_ERROR"] = ""
-        return log_info
+import datetime
+
+import pymysql
+from retrying import retry
+
+from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.Params import Param
+from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.config import logger
+
+__all__ = [
+    "MysqlPipeEnhanceMixin",
+]
+
+
+class MysqlPipeEnhanceMixin(object):
+    """
+    用于扩展 pipelines 中的功能，作为 Mixin 使用，不要对其实例化和单独使用等
+    """
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def _connect(
+        self,
+        mysql_conf: MysqlConfig,
+    ) -> pymysql.connections.Connection:
+        """
+        链接数据库操作：
+            1.如果链接正常，则返回链接句柄；
+            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
+        Args:
+            mysql_conf: pymysql 链接所需的参数
+
+        Returns:
+            1).pymysql.connections.Connection, 链接句柄
+        """
+        try:
+            conn = pymysql.connect(
+                user=mysql_conf.user,
+                password=mysql_conf.password,
+                host=mysql_conf.host,
+                port=mysql_conf.port,
+                database=mysql_conf.database,
+                charset=mysql_conf.charset,
+            )
+        except Exception as e:
+            logger.warning(f"目标数据库：{mysql_conf.database} 不存在，尝试创建中...")
+            if "1049" in str(e):
+                # 如果连接目标数据库报不存在的错误时，先创建出此目标数据库
+                ReuseOperation.create_database(mysql_conf)
+        else:
+            # 连接没有问题就直接返回连接对象
+            return conn
+        # 出现数据库不存在问题后，在创建数据库 create_database 后，再次返回连接对象
+        return pymysql.connect(
+            user=mysql_conf.user,
+            password=mysql_conf.password,
+            host=mysql_conf.host,
+            port=mysql_conf.port,
+            database=mysql_conf.database,
+            charset=mysql_conf.charset,
+        )
+
+    def _get_sql_by_item(self, table: str, item: dict) -> str:
+        """
+        根据处理后的 item 生成 sql 插入语句
+        Args:
+            table: 数据库表名
+            item: 处理后的 item
+
+        Returns:
+            1). sql 插入语句
+        """
+        keys = f"""`{"`, `".join(item.keys())}`"""
+        values = ", ".join(["%s"] * len(item))
+        update = ",".join([f" `{key}` = %s" for key in item])
+        return f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
+
+    def _get_log_by_spider(self, spider, crawl_time):
+        """
+        获取 spider 的运行日志情况
+        Args:
+            spider: scrapy spider
+            crawl_time: 爬取时间
+
+        Returns:
+            log_info: 日志信息
+        """
+        mysql_conf = spider.mysql_conf
+        text = {}
+        stats = spider.stats.get_stats()
+        error_reason = ""
+        for k, v in stats.items():
+            if isinstance(v, datetime.datetime):
+                text[k.replace("/", "_")] = (v + datetime.timedelta(hours=8)).strftime(
+                    "%Y-%m-%d %H:%M:%S"
+                )
+            else:
+                if all(
+                    [
+                        "response_status_count" in k,
+                        k != "downloader/response_status_count/200",
+                    ]
+                ):
+                    status_code = k.split("/")[-1] if len(k.split("/")) > 0 else ""
+                    if status_code.startswith("4"):
+                        if status_code == "429":
+                            error_reason += f"{status_code}错误：代理超过使用频率限制"
+                        else:
+                            error_reason += f"{status_code}错误：网页失效/无此网页/网站拒绝访问"
+                    elif status_code.startswith("5"):
+                        error_reason += f"{status_code}错误：网站服务器处理出错"
+                    elif status_code != "":
+                        error_reason += f"{status_code}:待人工排查原因"
+                elif "exception_type_count" in k:
+                    error_name = k.split("/")[-1]
+                    if "Timeout" in error_name:
+                        error_reason += f"{error_name}:网站响应超时错误 "
+                    elif "ConnectionDone" in error_name:
+                        error_reason += f"{error_name}:网站与脚本连接断开 "
+                    else:
+                        # "ResponseNeverReceived" or "ResponseFailed"
+                        error_reason += f"{error_name}:网站无响应 "
+                text[k.replace("/", "_")] = v
+
+        log_info = {
+            "database": mysql_conf.database,
+            # 脚本名称
+            "spider_name": spider.name,
+            # uid
+            "uid": f"{mysql_conf.database}|{spider.name}",
+            # 请求次数统计
+            "request_counts": text.get("downloader_request_count", 0),
+            # 接收次数统计
+            "received_count": text.get("response_received_count", 0),
+            # 采集数据量
+            "item_counts": text.get("item_scraped_count", 0),
+            # info 数据统计
+            "info_count": text.get("log_count_INFO", 0),
+            # 警告数据统计
+            "warning_count": text.get("log_count_WARNING", 0),
+            # 错误数据统计
+            "error_count": text.get("log_count_ERROR", 0),
+            # 开始时间
+            "start_time": text.get("start_time"),
+            # 结束时间
+            "finish_time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            # 花费时间
+            "spend_minutes": round(
+                (
+                    datetime.datetime.now()
+                    - stats.get("start_time")
+                    - datetime.timedelta(hours=8)
+                ).seconds
+                / 60,
+                2,
+            ),
+            "crawl_time": crawl_time,
+        }
+
+        # 错误原因
+        if text.get("log_count_ERROR", 0):
+            log_info["log_count_ERROR"] = error_reason or "请人工排查错误原因！"
+
+        else:
+            log_info["log_count_ERROR"] = ""
+        return log_info
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/MongoDBPipe.py` & `ayugespidertools-1.1.8/ayugespidertools/common/MongoDBPipe.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/MultiPlexing.py` & `ayugespidertools-1.1.8/ayugespidertools/common/MultiPlexing.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,24 +62,22 @@
         if file_name_list := pattern.findall(file_url):
             return file_name_list[0]
         return ""
 
     @staticmethod
     def get_files_from_path(path: str) -> list:
         """
-        获取 path 文件夹下的所有文件
+        获取 path 文件夹下的所有文件，而且输出以 path 为根目录的相对路径
         Args:
             path: 需要判断的文件夹路径
 
         Returns:
             file_list: path 文件夹下的文件列表
         """
-        # 得到文件夹下的所有文件名称
-        files = os.listdir(path)
-        return [file for file in files if not os.path.isdir(path + "\\" + file)]
+        return [f.path for f in os.scandir(path) if f.is_file()]
 
     @staticmethod
     def get_bytes_by_file(file_path: str) -> bytes:
         """
         获取媒体文件的 bytes 内容
         Args:
             file_path: 对应文件的路径
@@ -297,15 +295,15 @@
             1）.是否为 json 格式
         """
         if not isinstance(judge_str, str):
             return False
 
         try:
             json.loads(judge_str)
-        except Exception as e:
+        except Exception:
             return False
         else:
             return True
 
     @staticmethod
     def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
         """
@@ -334,15 +332,15 @@
             1). 转化 dict 格式后的 body
         """
         return {
             x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
         }
 
     @staticmethod
-    def get_array_dimension(array: list) -> int:
+    def get_array_dimension(array: Union[frozenset, list, set, tuple]) -> int:
         """
         获取 array 的维度
         Args:
             array: 数组
 
         Returns:
             1).层级数
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/Params.py` & `ayugespidertools-1.1.8/ayugespidertools/common/Params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import platform
 import random
 from typing import List, TypeVar
 
+import pymongo
+import pymysql
+
 from ayugespidertools.Items import MongoDataItem, MysqlDataItem, ScrapyClassicItem
 
 __all__ = [
     "Param",
 ]
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/SpiderDBConf.py` & `ayugespidertools-1.1.8/ayugespidertools/common/SpiderDBConf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/SqlFormat.py` & `ayugespidertools-1.1.8/ayugespidertools/common/SqlFormat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/TypeVars.py` & `ayugespidertools-1.1.8/ayugespidertools/common/TypeVars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/Utils.py` & `ayugespidertools-1.1.8/ayugespidertools/common/Utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,29 @@
         Returns:
             conf_value: consul 的 group 下 key_values 的详细信息
         """
         url_params = urlparse(url).query
 
         curr_consul_headers = copy.deepcopy(Param.consul_headers)
         curr_consul_headers["X-Consul-Token"] = token
-        r = requests.get(url, headers=curr_consul_headers, verify=False)
+        try:
+            r = requests.get(
+                url,
+                headers=curr_consul_headers,
+                verify=False,
+                timeout=(
+                    Param.requests_req_timeout,
+                    Param.requests_res_timeout,
+                ),
+            )
+        except (
+            requests.exceptions.ConnectionError,
+            requests.exceptions.ConnectTimeout,
+        ) as e:
+            raise ValueError("请求 consul 超时，请检查 consul 是否正常运行!") from e
         # 判断是否返回的 raw 原始数据
         if "raw" in url_params:
             return r.text
         return EncryptOperation.base64_decode(decode_data=r.json()[0]["Value"])
 
     @classmethod
     def get_conf_by_consul(
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/common/YiDunGap.py` & `ayugespidertools-1.1.8/ayugespidertools/common/YiDunGap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,19 @@
         s = cls(wwx_robot_key=crawler.settings.get("WWXRobot_key", None))
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         crawler.signals.connect(s.spider_closed, signal=signals.spider_closed)
         return s
 
     @retry(stop_max_attempt_number=Param.retry_num)
     def get_proxy_ip(self, size, isdict: Optional[bool] = None):
-        proxy_url = f"http://dps.kdlapi.com/api/getdps?orderid={self.simidaili_conf['orderid']}&num={size}&signature={self.simidaili_conf['signature']}&format=json"
+        proxy_url = (
+            "http://dps.kdlapi.com/api/getdps"
+            f"?orderid={self.simidaili_conf['orderid']}&num={size}"
+            f"&signature={self.simidaili_conf['signature']}&format=json"
+        )
         if self.important_error:
             raise ValueError("ip 获取方式有误，请重构私密代理中间件获取 ip 的模块！")
 
         try:
             r = requests.get(proxy_url).json()
         except Exception as e:
             raise ValueError("快代理请求获取 ip 无响应，请检查是否能够正常访问快代理或者 nacos 的配置是否以及失效！") from e
@@ -65,15 +69,15 @@
 
                     if isdict:
                         self.proxy_list = iplist
                     else:
                         return iplist
                 else:
                     raise ValueError("ip 获取方式有误，请重构私密代理中间件获取 ip 的模块！")
-            except:
+            except Exception:
                 self.important_error = True
                 traceback.print_exc()
                 raise ValueError("ip 获取方式有误，请重构私密代理中间件获取ip的模块！")
 
         elif msg := r.get("msg"):
             self.WWX.send_text(f"私密代理特级警报：私密代理出现错误，错误原因是: {msg}")
             raise ValueError(f"获取私密ip失败，原因是：{msg}")
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,336 +1,331 @@
-import datetime
-import warnings
-from typing import Optional, Type
-
-import pymysql
-from retrying import retry
-
-from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.MysqlErrorHandle import Synchronize, deal_mysql_err
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import MysqlConfig, TableEnumTypeVar
-from ayugespidertools.common.Utils import ToolsForAyu
-
-# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
-warnings.filterwarnings(
-    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
-)
-
-__all__ = [
-    "AyuMysqlPipeline",
-]
-
-
-class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
-    """
-    Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
-    """
-
-    def __init__(
-        self,
-        table_prefix: str,
-        table_enum: Type[TableEnumTypeVar],
-        env: str,
-        record_log_to_mysql: Optional[bool] = False,
-    ) -> None:
-        """
-        初始化 Mysql 链接所需要的信息
-        Args:
-            table_prefix: 数据库表前缀
-            table_enum: 数据表的枚举信息
-            env: 当前程序部署环境名
-            record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
-        """
-        self.table_prefix = table_prefix
-        self.table_enum = table_enum
-        self.env = env
-        self.record_log_to_mysql = record_log_to_mysql
-        # 排序规则，用于创建数据库时使用
-        self.collate = None
-        self.mysql_conf: Optional[MysqlConfig] = None
-        self.conn = None
-        self.slog = None
-        self.cursor = None
-        self.crawl_time = datetime.date.today()
-
-    @classmethod
-    def from_crawler(cls, crawler):
-        return cls(
-            # 数据库表前缀
-            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
-            # 数据库表枚举是否开启
-            table_enum=crawler.settings.get("DATA_ENUM"),
-            # 获取部署的环境
-            env=crawler.settings.get("ENV"),
-            # 当 record_log_to_mysql 为 True 时，会记录运行情况
-            record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
-        )
-
-    def open_spider(self, spider):
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
-        self.conn = self._connect(self.mysql_conf)
-        self.cursor = self.conn.cursor()
-
-    def get_table_name(self, table: str) -> str:
-        """
-        组合完整的数据库表
-        Args:
-            table: 数据表的后缀
-
-        Returns:
-            1). 拼接成完整的数据表的值
-        """
-        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
-        full_table_name = f"{self.table_prefix}{table}"
-
-        # 最终的数据表名不能含有空格
-        assert (
-            " " not in full_table_name
-        ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
-        return full_table_name
-
-    def get_new_item(self, item):
-        """
-        重新整合 item
-        Args:
-            item: scrapy yield 的 item 信息
-
-        Returns:
-            1). 整合后的 item
-        """
-        new_item = {}
-        notes_dic = {}
-        # 如果是 ayugespidertools.Items 中的各个自封装类型时
-        # alldata 可以认为是关键字，需要判断其是否存在，且是否为 dict。
-        # 若其存在且为 dict，则默认其为 Items 中的 alldata 数据类型而非单一字段值
-        insert_data = item.get("alldata")
-        if all([insert_data, isinstance(insert_data, dict)]):
-            judge_item = next(iter(insert_data.values()))
-            # 是 namedtuple 类型
-            if ReuseOperation.is_namedtuple_instance(judge_item):
-                for key, value in insert_data.items():
-                    new_item[key] = value.key_value
-                    notes_dic[key] = value.notes
-            # 是双层 dict 格式
-            elif isinstance(judge_item, dict):
-                for key, value in insert_data.items():
-                    new_item[key] = value.get("key_value", "")
-                    notes_dic[key] = value["notes"]
-            # 其它默认为单层 dict 格式
-            else:
-                for key, value in insert_data.items():
-                    new_item[key] = value
-                    notes_dic[key] = key
-
-        # 兼容旧写法，直接 dict 格式的 item 即可
-        else:
-            # 将存入表的无关字段给去掉
-            save_data_item = ReuseOperation.get_items_except_keys(
-                dict_conf=item, key_list=["table", "item_mode"]
-            )
-            for key, value in save_data_item.items():
-                new_item[key] = value
-                notes_dic[key] = key
-
-        return {"new_item": new_item, "notes_dic": notes_dic}
-
-    def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "Mysql":
-            self.insert_item(
-                self.get_new_item(item_dict), self.get_table_name(item_dict["table"])
-            )
-        return item
-
-    def insert_item(self, item_o, table):
-        """
-        通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
-        Args:
-            item_o: item
-            table: 数据库表名
-
-        Returns:
-            None
-        """
-        if not (new_item := item_o.get("new_item")):
-            return
-
-        note_dic = item_o.get("notes_dic")
-        sql = self._get_sql_by_item(table=table, item=new_item)
-
-        try:
-            if self.cursor.execute(sql, tuple(new_item.values()) * 2):
-                self.conn.commit()
-
-        except Exception as e:
-            self.slog.warning(f":{e}")
-            self.slog.warning(f"Item:{new_item}  Table: {table}")
-            self.conn.rollback()
-            deal_mysql_err(
-                Synchronize(),
-                err_msg=str(e),
-                conn=self.conn,
-                cursor=self.cursor,
-                charset=self.mysql_conf.charset,
-                collate=self.collate,
-                database=self.mysql_conf.database,
-                table=table,
-                table_prefix=self.table_prefix,
-                table_enum=self.table_enum,
-                note_dic=note_dic,
-            )
-            return self.insert_item(item_o, table)
-
-    def close_spider(self, spider):
-        # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
-        if self.record_log_to_mysql:
-            log_info = self._get_log_by_spider(
-                spider=spider, crawl_time=self.crawl_time
-            )
-
-            # 运行脚本统计信息
-            self.insert_script_statistics(log_info)
-            self.table_collection_statistics(
-                spider_name=spider.name,
-                database=spider.mysql_conf.database,
-                crawl_time=self.crawl_time,
-            )
-
-        if self.conn:
-            self.conn.close()
-
-    def table_collection_statistics(
-        self, spider_name: str, database: str, crawl_time: datetime.date
-    ):
-        """
-        统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
-        Args:
-            spider_name: 爬虫脚本名称
-            database: 数据库，保存程序采集记录保存的数据库
-            crawl_time: 采集时间，程序运行时间
-
-        Returns:
-            None
-        """
-        sql = f"""
-        select concat(
-            'select "',
-            TABLE_NAME,
-            '", count(id) as num , crawl_time from ',
-            TABLE_SCHEMA,
-            '.',
-            TABLE_NAME,
-                ' where crawl_time = "{crawl_time}"'
-        ) from information_schema.tables
-        where TABLE_SCHEMA='{database}' and TABLE_NAME in (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
-        """
-        self.cursor.execute(sql)
-        results = self.cursor.fetchall()
-        if sql_list := [row[0] for row in results]:
-            sql_all = " union all ".join(sql_list)
-            self.cursor.execute(sql_all)
-            results = self.cursor.fetchall()
-
-            for row in results:
-                table_statistics = {
-                    "spider_name": spider_name,
-                    "database": database,
-                    "table_name": row[0],
-                    "number": row[1],
-                    "crawl_time": str((row[2] or crawl_time)),
-                }
-                self.insert_table_statistics(table_statistics)
-
-    def insert_table_statistics(
-        self, data: dict, table: str = "table_collection_statistics"
-    ):
-        """
-        插入统计数据到表中
-        Args:
-            data: 需要统计的入库信息
-            table: 存储表的名称
-
-        Returns:
-            None
-        """
-        self.cursor.execute(
-            f"""
-            CREATE TABLE IF NOT EXISTS `{table}` (
-            `id` int(11) NOT NULL AUTO_INCREMENT,
-            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',            
-            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
-            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',            
-            PRIMARY KEY (`id`) USING BTREE
-            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
-            """
-        )
-
-        keys = f"""`{"`, `".join(data.keys())}`"""
-        values = ", ".join(["%s"] * len(data))
-        update = ",".join([f" `{key}` = %s" for key in data])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-        try:
-            if self.cursor.execute(sql, tuple(data.values()) * 2):
-                self.conn.commit()
-        except Exception as e:
-            self.conn.rollback()
-            self.slog.warning(f":{e}")
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def insert_script_statistics(
-        self, data: dict, table: str = "script_collection_statistics"
-    ):
-        """
-        存储运行脚本的统计信息
-        Args:
-            data: 需要插入的 log 信息
-            table: 存储表的名称
-
-        Returns:
-            None
-        """
-        self.cursor.execute(
-            f"""
-            CREATE TABLE IF NOT EXISTS `{table}` (
-            `id` int(11) NOT NULL AUTO_INCREMENT,
-            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
-            `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
-            `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
-            `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
-            `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
-            `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
-            `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
-            `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
-            `start_time` datetime NOT NULL COMMENT '开始时间',
-            `finish_time` datetime NOT NULL COMMENT '结束时间',
-            `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
-            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-            `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
-            PRIMARY KEY (`id`) USING BTREE
-            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
-            """
-        )
-
-        keys = f"""`{"`, `".join(data.keys())}`"""
-        values = ", ".join(["%s"] * len(data))
-        update = ",".join([f" `{key}` = %s" for key in data])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-        try:
-            if self.cursor.execute(sql, tuple(data.values()) * 2):
-                self.conn.commit()
-        except Exception as e:
-            self.conn.rollback()
-            self.slog.warning(f":{e}")
+import datetime
+import warnings
+from typing import Optional, Tuple, Type
+
+import pymysql
+from retrying import retry
+
+from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.MysqlErrorHandle import Synchronize, deal_mysql_err
+from ayugespidertools.common.Params import Param
+from ayugespidertools.common.TypeVars import MysqlConfig, TableEnumTypeVar
+from ayugespidertools.common.Utils import ToolsForAyu
+
+# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
+warnings.filterwarnings(
+    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
+)
+
+__all__ = [
+    "AyuMysqlPipeline",
+]
+
+
+class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
+    """
+    Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
+    """
+
+    def __init__(
+        self,
+        table_prefix: str,
+        table_enum: Type[TableEnumTypeVar],
+        env: str,
+        record_log_to_mysql: Optional[bool] = False,
+    ) -> None:
+        """
+        初始化 Mysql 链接所需要的信息
+        Args:
+            table_prefix: 数据库表前缀
+            table_enum: 数据表的枚举信息
+            env: 当前程序部署环境名
+            record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
+        """
+        self.table_prefix = table_prefix
+        self.table_enum = table_enum
+        self.env = env
+        self.record_log_to_mysql = record_log_to_mysql
+        # 排序规则，用于创建数据库时使用
+        self.collate = None
+        self.mysql_conf: Optional[MysqlConfig] = None
+        self.conn = None
+        self.slog = None
+        self.cursor = None
+        self.crawl_time = datetime.date.today()
+
+    @classmethod
+    def from_crawler(cls, crawler):
+        return cls(
+            # 数据库表前缀
+            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
+            # 数据库表枚举是否开启
+            table_enum=crawler.settings.get("DATA_ENUM"),
+            # 获取部署的环境
+            env=crawler.settings.get("ENV"),
+            # 当 record_log_to_mysql 为 True 时，会记录运行情况
+            record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
+        )
+
+    def open_spider(self, spider):
+        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
+        self.conn = self._connect(self.mysql_conf)
+        self.cursor = self.conn.cursor()
+
+    def get_table_name(self, table: str) -> str:
+        """
+        组合完整的数据库表
+        Args:
+            table: 数据表的后缀
+
+        Returns:
+            1). 拼接成完整的数据表的值
+        """
+        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
+        full_table_name = f"{self.table_prefix}{table}"
+
+        # 最终的数据表名不能含有空格
+        assert (
+            " " not in full_table_name
+        ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
+        return full_table_name
+
+    def get_new_item(self, item):
+        """
+        重新整合 item
+        Args:
+            item: scrapy yield 的 item 信息
+
+        Returns:
+            1). 整合后的 item
+        """
+        new_item = {}
+        notes_dic = {}
+        # 如果是 ayugespidertools.Items 中的各个自封装类型时
+        # alldata 可以认为是关键字，需要判断其是否存在，且是否为 dict。
+        # 若其存在且为 dict，则默认其为 Items 中的 alldata 数据类型而非单一字段值
+        insert_data = item.get("alldata")
+        if all([insert_data, isinstance(insert_data, dict)]):
+            judge_item = next(iter(insert_data.values()))
+            # 是 namedtuple 类型
+            if ReuseOperation.is_namedtuple_instance(judge_item):
+                for key, value in insert_data.items():
+                    new_item[key] = value.key_value
+                    notes_dic[key] = value.notes
+            # 是双层 dict 格式
+            elif isinstance(judge_item, dict):
+                for key, value in insert_data.items():
+                    new_item[key] = value.get("key_value", "")
+                    notes_dic[key] = value["notes"]
+            # 其它默认为单层 dict 格式
+            else:
+                for key, value in insert_data.items():
+                    new_item[key] = value
+                    notes_dic[key] = key
+
+        # 兼容旧写法，直接 dict 格式的 item 即可
+        else:
+            # 将存入表的无关字段给去掉
+            save_data_item = ReuseOperation.get_items_except_keys(
+                dict_conf=item, key_list=["table", "item_mode"]
+            )
+            for key, value in save_data_item.items():
+                new_item[key] = value
+                notes_dic[key] = key
+
+        return {"new_item": new_item, "notes_dic": notes_dic}
+
+    def process_item(self, item, spider):
+        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        # 先查看存储场景是否匹配
+        if item_dict["item_mode"] == "Mysql":
+            self.insert_item(
+                self.get_new_item(item_dict), self.get_table_name(item_dict["table"])
+            )
+        return item
+
+    def insert_item(self, item_o, table):
+        """
+        通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
+        Args:
+            item_o: item
+            table: 数据库表名
+
+        Returns:
+            None
+        """
+        if not (new_item := item_o.get("new_item")):
+            return
+
+        note_dic = item_o.get("notes_dic")
+        sql = self._get_sql_by_item(table=table, item=new_item)
+
+        try:
+            if self.cursor.execute(sql, tuple(new_item.values()) * 2):
+                self.conn.commit()
+
+        except Exception as e:
+            self.slog.warning(f":{e}")
+            self.slog.warning(f"Item:{new_item}  Table: {table}")
+            self.conn.rollback()
+            deal_mysql_err(
+                Synchronize(),
+                err_msg=str(e),
+                conn=self.conn,
+                cursor=self.cursor,
+                charset=self.mysql_conf.charset,
+                collate=self.collate,
+                database=self.mysql_conf.database,
+                table=table,
+                table_prefix=self.table_prefix,
+                table_enum=self.table_enum,
+                note_dic=note_dic,
+            )
+            return self.insert_item(item_o, table)
+
+    def close_spider(self, spider):
+        # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
+        if self.record_log_to_mysql:
+            log_info = self._get_log_by_spider(
+                spider=spider, crawl_time=self.crawl_time
+            )
+
+            # 运行脚本统计信息
+            self.insert_script_statistics(log_info)
+            self.table_collection_statistics(
+                spider_name=spider.name,
+                database=spider.mysql_conf.database,
+                crawl_time=self.crawl_time,
+            )
+
+        if self.conn:
+            self.conn.close()
+
+    def table_collection_statistics(
+        self, spider_name: str, database: str, crawl_time: datetime.date
+    ):
+        """
+        统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
+        Args:
+            spider_name: 爬虫脚本名称
+            database: 数据库，保存程序采集记录保存的数据库
+            crawl_time: 采集时间，程序运行时间
+
+        Returns:
+            None
+        """
+        sql = f"""
+        select concat(
+        'select "', TABLE_NAME, '", count(id) as num , crawl_time from ', TABLE_SCHEMA, '.', TABLE_NAME,
+        ' where crawl_time = "{crawl_time}"') from information_schema.tables
+        where TABLE_SCHEMA='{database}' and TABLE_NAME in
+        (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
+        """
+        self.cursor.execute(sql)
+        results = self.cursor.fetchall()
+        if sql_list := [row[0] for row in results]:
+            sql_all = " union all ".join(sql_list)
+            self.cursor.execute(sql_all)
+            results = self.cursor.fetchall()
+
+            for row in results:
+                table_statistics = {
+                    "spider_name": spider_name,
+                    "database": database,
+                    "table_name": row[0],
+                    "number": row[1],
+                    "crawl_time": str((row[2] or crawl_time)),
+                }
+                self.insert_table_statistics(table_statistics)
+
+    def insert_table_statistics(
+        self, data: dict, table: str = "table_collection_statistics"
+    ):
+        """
+        插入统计数据到表中
+        Args:
+            data: 需要统计的入库信息
+            table: 存储表的名称
+
+        Returns:
+            None
+        """
+        create_table_sql = f"""
+        CREATE TABLE IF NOT EXISTS `{table}` (
+            `id` int(11) NOT NULL AUTO_INCREMENT,
+            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
+            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
+            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',
+            PRIMARY KEY (`id`) USING BTREE
+        ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
+        """
+        self.cursor.execute(create_table_sql)
+
+        sql = self._get_sql_by_item(table=table, item=data)
+        self._log_record(sql=sql, data=tuple(data.values()) * 2)
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def insert_script_statistics(
+        self, data: dict, table: str = "script_collection_statistics"
+    ):
+        """
+        存储运行脚本的统计信息
+        Args:
+            data: 需要插入的 log 信息
+            table: 存储表的名称
+
+        Returns:
+            None
+        """
+        self.cursor.execute(
+            f"""
+            CREATE TABLE IF NOT EXISTS `{table}` (
+                `id` int(11) NOT NULL AUTO_INCREMENT,
+                `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+                `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
+                `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
+                `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
+                `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
+                `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
+                `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
+                `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
+                `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
+                `start_time` datetime NOT NULL COMMENT '开始时间',
+                `finish_time` datetime NOT NULL COMMENT '结束时间',
+                `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
+                `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+                `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
+                PRIMARY KEY (`id`) USING BTREE
+                ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
+            """
+        )
+
+        sql = self._get_sql_by_item(table=table, item=data)
+        self._log_record(sql=sql, data=tuple(data.values()) * 2)
+
+    def _log_record(self, sql: str, data: Tuple) -> None:
+        """
+        执行日志记录的 sql 语句
+        Args:
+            sql: sql 语句
+            data: sql 语句中的参数
+
+        Returns:
+            None
+        """
+        try:
+            if self.cursor.execute(sql, data):
+                self.conn.commit()
+        except Exception as e:
+            self.conn.rollback()
+            self.slog.warning(f":{e}")
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import dataclasses
 import datetime
 
-from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
 from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.scraper.pipelines import AyuMysqlPipeline
 
 __all__ = [
     "AyuStatisticsMysqlPipeline",
 ]
 
 
-class AyuStatisticsMysqlPipeline(MysqlPipeEnhanceMixin):
+class AyuStatisticsMysqlPipeline(AyuMysqlPipeline):
     """
     Mysql 存储且记录脚本运行状态的简单示例
     """
 
     # TODO: 此方法暂用于测试
     def __init__(self, env):
         self.env = env
@@ -43,23 +43,16 @@
             data_item: scrapy item
             table: 存储至 mysql 的表名
 
         Returns:
             None
         """
         data = dataclasses.asdict(data_item)
-        keys = f"""`{"`, `".join(data.keys())}`"""
-        values = ", ".join(["%s"] * len(data))
-        update = ",".join([f" `{key}` = %s" for key in data])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-        try:
-            if self.cursor.execute(sql, tuple(data.values()) * 2):
-                self.conn.commit()
-        except Exception as e:
-            self.slog.warning(f":{e}")
+        sql = self._get_sql_by_item(table=table, item=data)
+        self._log_record(sql=sql, data=tuple(data.values()) * 2)
 
     def close_spider(self, spider):
         log_info = self._get_log_by_spider(spider=spider, crawl_time=self.crawl_time)
         self.insert(log_info, "script_collection_statistics")
 
         if self.conn:
             self.conn.close()
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Feb 10 19:57:28 2023 UTC, .py size: 450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-00000000: 550d 0d0a 0000 0000 a8a1 e663 c201 0000  U..........c....
+00000000: 550d 0d0a 0000 0000 ff7f 3664 ba01 0000  U.........6d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 6403 6701 5a05  d.l.m.Z...d.g.Z.
-00000050: 4700 6404 6403 8400 6403 6504 6501 8304  G.d.d...d.e.e...
-00000060: 5a06 6405 5300 2906 e900 0000 0029 02da  Z.d.S.)......)..
-00000070: 0b43 7261 776c 5370 6964 6572 da06 5370  .CrawlSpider..Sp
-00000080: 6964 6572 2901 da09 4179 7553 7069 6465  ider)...AyuSpide
-00000090: 72da 0e41 7975 4372 6177 6c53 7069 6465  r..AyuCrawlSpide
-000000a0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-000000b0: 0000 0200 0000 4000 0000 7318 0000 0065  ......@...s....e
-000000c0: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-000000d0: 005a 0464 0453 0029 0572 0500 0000 755a  .Z.d.S.).r....uZ
-000000e0: 0000 000a 2020 2020 e588 9de5 a78b 2041  ....    ...... A
-000000f0: 7975 5370 6964 6572 20e9 858d e7bd aeef  yuSpider .......
-00000100: bc8c e4b9 9fe5 889d e5a7 8be5 8c96 2043  .............. C
-00000110: 7261 776c 5370 6964 6572 20e7 9a84 2073  rawlSpider ... s
-00000120: 7069 6465 7220 e58a a0e5 bcba e789 88e6  pider ..........
-00000130: 9cac e985 8de7 bdae 0a20 2020 2063 0100  .........    c..
-00000140: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000150: 0000 4f00 0000 7328 0000 0074 006a 017c  ..O...s(...t.j.|
-00000160: 0066 017c 019e 027c 028e 0101 0074 026a  .f.|...|.....t.j
-00000170: 017c 0066 017c 019e 027c 028e 0101 0064  .|.f.|...|.....d
-00000180: 0053 0029 014e 2903 7204 0000 00da 085f  .S.).N).r......_
-00000190: 5f69 6e69 745f 5f72 0200 0000 2903 da04  _init__r....)...
-000001a0: 7365 6c66 da04 6172 6773 da06 6b77 6172  self..args..kwar
-000001b0: 6773 a900 720a 0000 00fa 472f 726f 6f74  gs..r.....G/root
-000001c0: 2f6d 7970 726f 6a2f 4179 7567 6553 7069  /myproj/AyugeSpi
-000001d0: 6465 7254 6f6f 6c73 2f61 7975 6765 7370  derTools/ayugesp
-000001e0: 6964 6572 746f 6f6c 732f 7363 7261 7065  idertools/scrape
-000001f0: 722f 7370 6964 6572 732f 6372 6177 6c2e  r/spiders/crawl.
-00000200: 7079 7206 0000 000f 0000 0073 0400 0000  pyr........s....
-00000210: 0001 1201 7a17 4179 7543 7261 776c 5370  ....z.AyuCrawlSp
-00000220: 6964 6572 2e5f 5f69 6e69 745f 5f4e 2905  ider.__init__N).
-00000230: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000240: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000250: 6d65 5f5f da07 5f5f 646f 635f 5f72 0600  me__..__doc__r..
-00000260: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000270: 0072 0b00 0000 7205 0000 000a 0000 0073  .r....r........s
-00000280: 0400 0000 0801 0404 4e29 07da 0e73 6372  ........N)...scr
-00000290: 6170 792e 7370 6964 6572 7372 0200 0000  apy.spidersr....
-000002a0: 7203 0000 00da 2061 7975 6765 7370 6964  r..... ayugespid
-000002b0: 6572 746f 6f6c 732e 7363 7261 7065 722e  ertools.scraper.
-000002c0: 7370 6964 6572 7372 0400 0000 da07 5f5f  spidersr......__
-000002d0: 616c 6c5f 5f72 0500 0000 720a 0000 0072  all__r....r....r
-000002e0: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-000002f0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000300: 0010 020c 0302 ff04 05                   .........
+00000020: 0005 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 0100 6403 6701 5a04 4700 6404  m.Z...d.g.Z.G.d.
+00000050: 6403 8400 6403 6503 6501 8304 5a05 6405  d...d.e.e...Z.d.
+00000060: 5300 2906 e900 0000 0029 01da 0b43 7261  S.)......)...Cra
+00000070: 776c 5370 6964 6572 2901 da09 4179 7553  wlSpider)...AyuS
+00000080: 7069 6465 72da 0e41 7975 4372 6177 6c53  pider..AyuCrawlS
+00000090: 7069 6465 7263 0000 0000 0000 0000 0000  piderc..........
+000000a0: 0000 0000 0000 0200 0000 4000 0000 7318  ..........@...s.
+000000b0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000000c0: 0264 0384 005a 0464 0453 0029 0572 0400  .d...Z.d.S.).r..
+000000d0: 0000 755a 0000 000a 2020 2020 e588 9de5  ..uZ....    ....
+000000e0: a78b 2041 7975 5370 6964 6572 20e9 858d  .. AyuSpider ...
+000000f0: e7bd aeef bc8c e4b9 9fe5 889d e5a7 8be5  ................
+00000100: 8c96 2043 7261 776c 5370 6964 6572 20e7  .. CrawlSpider .
+00000110: 9a84 2073 7069 6465 7220 e58a a0e5 bcba  .. spider ......
+00000120: e789 88e6 9cac e985 8de7 bdae 0a20 2020  .............   
+00000130: 2063 0100 0000 0000 0000 0000 0000 0300   c..............
+00000140: 0000 0300 0000 4f00 0000 7328 0000 0074  ......O...s(...t
+00000150: 006a 017c 0066 017c 019e 027c 028e 0101  .j.|.f.|...|....
+00000160: 0074 026a 017c 0066 017c 019e 027c 028e  .t.j.|.f.|...|..
+00000170: 0101 0064 0053 0029 014e 2903 7203 0000  ...d.S.).N).r...
+00000180: 00da 085f 5f69 6e69 745f 5f72 0200 0000  ...__init__r....
+00000190: 2903 da04 7365 6c66 da04 6172 6773 da06  )...self..args..
+000001a0: 6b77 6172 6773 a900 7209 0000 00fa 472f  kwargs..r.....G/
+000001b0: 726f 6f74 2f6d 7970 726f 6a2f 4179 7567  root/myproj/Ayug
+000001c0: 6553 7069 6465 7254 6f6f 6c73 2f61 7975  eSpiderTools/ayu
+000001d0: 6765 7370 6964 6572 746f 6f6c 732f 7363  gespidertools/sc
+000001e0: 7261 7065 722f 7370 6964 6572 732f 6372  raper/spiders/cr
+000001f0: 6177 6c2e 7079 7205 0000 000f 0000 0073  awl.pyr........s
+00000200: 0400 0000 0001 1201 7a17 4179 7543 7261  ........z.AyuCra
+00000210: 776c 5370 6964 6572 2e5f 5f69 6e69 745f  wlSpider.__init_
+00000220: 5f4e 2905 da08 5f5f 6e61 6d65 5f5f da0a  _N)...__name__..
+00000230: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000240: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000250: 5f72 0500 0000 7209 0000 0072 0900 0000  _r....r....r....
+00000260: 7209 0000 0072 0a00 0000 7204 0000 000a  r....r....r.....
+00000270: 0000 0073 0400 0000 0801 0404 4e29 06da  ...s........N)..
+00000280: 0e73 6372 6170 792e 7370 6964 6572 7372  .scrapy.spidersr
+00000290: 0200 0000 da20 6179 7567 6573 7069 6465  ..... ayugespide
+000002a0: 7274 6f6f 6c73 2e73 6372 6170 6572 2e73  rtools.scraper.s
+000002b0: 7069 6465 7273 7203 0000 00da 075f 5f61  pidersr......__a
+000002c0: 6c6c 5f5f 7204 0000 0072 0900 0000 7209  ll__r....r....r.
+000002d0: 0000 0072 0900 0000 720a 0000 00da 083c  ...r....r......<
+000002e0: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
+000002f0: 0c02 0c03 02ff 0405                      ........
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc` & `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-1.1.8/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     ),
     "Endpoint": config_parser.get("ALI_OSS", "Endpoint", fallback=None),
     "examplebucket": config_parser.get("ALI_OSS", "Examplebucket", fallback=None),
     "operateDoc": config_parser.get("ALI_OSS", "OperateDoc", fallback=None),
 }
 
 # 日志管理
+LOG_LEVEL = env.str("LOG_LEVEL", "ERROR")
 LOG_FILE = f"{LOG_DIR}/$project_name.log"
 logger.add(
     env.str("LOG_ERROR_FILE", f"{LOG_DIR}/error.log"),
     level="ERROR",
     rotation="1 week",
     retention="7 days",
     enqueue=True,
```

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/ayugespidertools/utils/cmdline.py` & `ayugespidertools-1.1.8/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.7/pyproject.toml` & `ayugespidertools-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "1.1.7"
+version = "1.1.8"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
 keywords = ["crawler", "scraping", "twisted", "aiohttp", "asyncio", "scrapy", "aiomysql", "mmh3"]
 homepage = "https://www.ayuge.top/mkdocs-material/"
 include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 opencv-python = "^4.6.0.66"
 PyMySQL = "^1.0.2"
 environs = "^9.5.0"
 loguru = "^0.6.0"
 numpy = "1.24.2"
 PyExecJS = "^1.5.1"
 requests = "^2.28.1"
@@ -48,14 +48,15 @@
 pytest = "^7.1.3"
 black = "^23.1.0"
 isort = "^5.12.0"
 sphinx-rtd-theme = "^1.2.0"
 recommonmark = "^0.7.1"
 coverage = "^7.2.2"
 tox = "^4.4.8"
+flake8 = "^6.0.0"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple"
 
 [tool.pytest.ini_options]
 xfail_strict = true
```

### Comparing `ayugespidertools-1.1.7/PKG-INFO` & `ayugespidertools-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 1.1.7
+Version: 1.1.8
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: DBUtils (>=3.0.2,<4.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
@@ -201,44 +200,43 @@
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
 
 比如你可能需要更新依赖库中 `pymongo` 为新版本 `x.x.x`，那只需 `poetry install` 安装现有依赖后，再 `poetry add pymongo@x.x.x` 安装目标版本（尽量不要使用 `poetry update pymongo`），确定测试正常了即可 `poetry build` 打包使用。
 
 ## TodoList
 
 - [x] `scrapy` 的扩展功能场景
-  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [ ] ~~`selenium`: 性能没有 `pyppeteer` 强~~
-    - [x] `pyppeteer`: `Gerapy-pyppeteer` 库已经实现此功能
     - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
-    - [ ] ~~`splash`: 继承 `splash` 渲染 `js` 的功能~~
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
   - [ ] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
 - [x] 常用开发场景
   - [x] `sql` 语句拼接，只是简单场景，后续优化。已给出优化方向，参考库等信息。
   - [x] `mongoDB` 语句拼接
   - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
-  - [ ] 字体反爬还原方法
+  - [x] 字体反爬还原方法
+    - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
+      - [x] 可以直接在字体文件 `xml` 中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
+      - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`，后再通过各种方式识别。
   - [x] `html` 格式转 `markdown` 格式
   - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等等等
   - [x] 添加常用的图片验证码中的处理方法
     - [x] 滑块缺口距离的识别方法（多种实现方式）
     - [x] 根据滑块距离生成轨迹数组的方法
     - [x] 识别点选验证码位置及点击顺序，识别结果不太好，待优化
     - [x] 图片乱序混淆的还原方法示例
 
-注：
+**注：**
 
-- 不再开发结合 `selenium` 扩展的功能，推荐使用 `scrapy-playwright`，`Gerapy-pyppeteer` 等其它库；
-- 不再开发结合 `splash` 的功能，如果使用 `splash http api` 的话，在 `scrapy` ，本库或自写脚本中都比较容易扩展。如果要使用 `lua` `api` 等复杂的功能那还是推荐 `scrapy-splash` 这类的扩展库。
+1. 由于 `scrapy` 扩展库的开源项目众多，在使用本库的基础上扩展它们，与使用 `scrapy` 时扩展它们的用法一致，所以不再开发一些其它工具已经拥有且稳定的功能，但也会尽量开发一些常用且通用的方法来提升效率。
+2. 字体反爬部分不会给出详细解决示例，不管是使用 `fontforge`，`fontTools` 或 `ocr` 等工具，已经脱离本库的范围了，我会给出部分依赖的方法，但不会添加以上工具库的依赖了，而导致本库依赖过于杂糅。而且，若要实现高可用的字体映射也比较简单，请自行实现，可能会考虑新开 `pypi` 库来实现此部分。
```

