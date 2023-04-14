# Comparing `tmp/cyberdrop-dl-4.1.1.tar.gz` & `tmp/cyberdrop-dl-4.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.1.tar", last modified: Mon Apr  3 15:23:17 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.11.tar", last modified: Fri Apr 14 16:01:16 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.1.tar` & `cyberdrop-dl-4.1.11.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.464253 cyberdrop-dl-4.1.1/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.468253 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.468253 cyberdrop-dl-4.1.1/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:23:17.464253 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 15:23:17.000000 cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-03 15:23:17.472253 cyberdrop-dl-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:23:08.000000 cyberdrop-dl-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.959603 cyberdrop-dl-4.1.11/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.963603 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.963603 cyberdrop-dl-4.1.11/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.959603 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/setup.py
```

### Comparing `cyberdrop-dl-4.1.1/LICENSE` & `cyberdrop-dl-4.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/PKG-INFO` & `cyberdrop-dl-4.1.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.1
+Version: 4.1.11
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.1 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.11 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.1/README.md` & `cyberdrop-dl-4.1.11/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
+from typing import TYPE_CHECKING
 
 import rich
-from yarl import URL
 
 from cyberdrop_dl.base_functions.error_classes import NoExtensionFailure
 
+if TYPE_CHECKING:
+    from yarl import URL
+
+
 FILE_FORMATS = {
     'Images': {
         '.jpg', '.jpeg', '.png', '.gif',
         '.gifv', '.webp', '.jpe', '.svg',
         '.jfif', '.tif', '.tiff', '.jif',
     },
     'Videos': {
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 config_default = {
     "Apply_Config": False,
     "Configuration": {
         "Authentication": {
+            "gofile_api_key": "",
             "pixeldrain_api_key": "",
             "simpcity_username": "",
             "simpcity_password": "",
             "socialmediagirls_username": "",
             "socialmediagirls_password": "",
             "xbunker_username": "",
             "xbunker_password": "",
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
-from typing import ClassVar, List, Tuple, Optional
+from typing import TYPE_CHECKING, ClassVar, List, Tuple
 
-from yarl import URL
+if TYPE_CHECKING:
+    from yarl import URL
 
 
 @dataclass
 class MediaItem:
     url: URL
     referer: URL
     complete: bool
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import ssl
 from http import HTTPStatus
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import aiofiles
 import aiohttp
 import certifi
 from bs4 import BeautifulSoup
-from rich.progress import TaskID
 from tqdm import tqdm
 from yarl import URL
 
 from ..base_functions.base_functions import adjust, logger
-from ..base_functions.data_classes import MediaItem
 from ..base_functions.error_classes import DownloadFailure, InvalidContentTypeFailure
 from ..downloader.downloader_utils import CustomHTTPStatus
 from ..downloader.progress_definitions import file_progress
 from .rate_limiting import AsyncRateLimiter, throttle
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from rich.progress import TaskID
+
+    from ..base_functions.data_classes import MediaItem
+
 
 class Client:
     """Creates a 'client' that can be referenced by scraping or download sessions"""
     def __init__(self, ratelimit: int, throttle: int, secure: bool, connect_timeout: int):
         self.connect_timeout = connect_timeout
         self.ratelimit = ratelimit
         self.throttle = throttle
         self.simultaneous_session_limit = asyncio.Semaphore(50)
-        self.user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0'
+        self.user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/112.0'
         self.verify_ssl = secure
         self.ssl_context = ssl.create_default_context(cafile=certifi.where()) if secure else False
         self.cookies = aiohttp.CookieJar(quote_cookie=False)
 
 
 class ScrapeSession:
     """AIOHTTP operations for scraping"""
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,24 +71,31 @@
         return domain_obj
 
     async def handle_profile(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler for erome profiles, sends albums to handle_album"""
         domain_obj = DomainItem("erome", {})
         try:
             soup = await session.get_BS4(url)
-            title = soup.select_one('h1[class="username"]').get_text()
+            title = url.name
             if title is None:
                 title = url.name
             elif self.include_id:
                 title = title + " - " + url.name
             title = await make_title_safe(title)
 
             for album in soup.select("a[class=album-link]"):
-                url = URL(album.get('href'))
-                await domain_obj.extend(await self.handle_album(session, url))
+                album_url = URL(album.get('href'))
+                await domain_obj.extend(await self.handle_album(session, album_url))
             await domain_obj.append_title(title)
+
+            next_page = soup.select_one('a[rel="next"]')
+            if next_page:
+                next_page = next_page.get("href").split("page=")[-1]
+                next_page = url.with_query(f"page={next_page}")
+                await domain_obj.extend(await self.handle_profile(session, next_page))
+
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,23 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
         self.api_address = URL("https://api.gofile.io")
         self.token = None
 
-    async def get_token(self, session: ScrapeSession):
+    async def get_token(self, session: ScrapeSession, api_token=None):
         """Creates an anon gofile account to use."""
         if self.token:
             return
 
+        if api_token:
+            self.token = api_token
+            return
+
         try:
             json_obj = await session.get_json(self.api_address / "createAccount")
             if json_obj["status"] == "ok":
                 self.token = json_obj["data"]["token"]
                 await self.set_cookie(session)
             else:
                 raise
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         return domain_obj
 
     async def get_user(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
         """Gets posts for a user profile"""
         try:
             model = url.name + " (NSFW.XXX)"
             for page in itertools.count(1):
-                page_url = URL(f"https://nsfw.xxx/page/{page}?nsfw[]=0&types[]=image&types[]=video&types[]=gallery&slider=1&jsload=1&user={url.name}")
+                model_name = url.path.split("/")
+                model_name = list(filter(None, model_name))[-1]
+                page_url = URL(f"https://nsfw.xxx/page/{page}?nsfw[]=0&types[]=image&types[]=video&types[]=gallery&slider=1&jsload=1&user={model_name}")
                 page_soup = await session.get_BS4(page_url)
 
                 posts = page_soup.select('div[class="sh-section__image grid-item"] a[class=slider_init_href]')
                 posts.extend(page_soup.select('div[class="sh-video__player"] a[class=slider_init_href]'))
                 posts.extend(page_soup.select('div[class="sh-section__images row"] div a'))
 
                 if not posts:
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from __future__ import annotations
 
 import asyncio
 import re
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import aiofiles
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import (
     get_filename_and_ext,
     log,
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import CascadeItem, MediaItem
 from ..base_functions.error_classes import FailedLoginFailure, NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 async def write_last_post_file(file: Path, url: str):
     """Writes the last post url from a thread to the specified file"""
     async with aiofiles.open(file, mode='a') as f:
         await f.write(url + '\n')
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 import itertools
 import logging
 from http import HTTPStatus
 from random import gauss
+from typing import TYPE_CHECKING
 
 import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
-from rich.progress import TaskID
 
 from cyberdrop_dl.base_functions.base_functions import (
     adjust,
     clear,
     log,
     logger,
 )
-from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, FileLock, ForumItem, MediaItem
+from cyberdrop_dl.base_functions.data_classes import (
+    AlbumItem,
+    CascadeItem,
+    DomainItem,
+    FileLock,
+    ForumItem,
+    MediaItem,
+)
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper, get_db_path
 from cyberdrop_dl.client.client import Client, DownloadSession
 
 from .downloader_utils import (
     CustomHTTPStatus,
     allowed_filetype,
@@ -38,14 +45,17 @@
     file_progress,
     forum_progress,
     get_cascade_table,
     get_forum_table,
     overall_file_progress,
 )
 
+if TYPE_CHECKING:
+    from rich.progress import TaskID
+
 
 class Files:
     """Class that keeps track of completed, skipped and failed files"""
 
     def __init__(self, total_files: int):
         self.completed_files_task_id = overall_file_progress.add_task("[green]Completed", total=total_files)
         self.completed_files = 0
@@ -255,15 +265,16 @@
                     logger.debug("We ran into a 400 level error: %s", str(e.code))
                     await log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
-                if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
+                if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == HTTPStatus.BAD_GATEWAY \
+                        or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
                     await log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         await gfycat_session.exit_handler()
 
     async def GoFile(self, url, title=None):
         gofile_session = ScrapeSession(self.client)
         if not self.gofile_crawler:
             self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
         async with self.gofile_semaphore:
-            await self.gofile_crawler.get_token(session=gofile_session)
+            await self.gofile_crawler.get_token(session=gofile_session, api_token=self.args['Authentication']['gofile_api_key'])
         async with self.gofile_limiter:
             domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
         await self._handle_domain_additions("gofile", domain_obj, title)
         await gofile_session.exit_handler()
 
     async def HGameCG(self, url, title=None):
         hgamecg_session = ScrapeSession(self.client)
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.1
+Version: 4.1.11
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.1 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.11 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.1/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.1/setup.cfg` & `cyberdrop-dl-4.1.11/setup.cfg`

 * *Files identical despite different names*

