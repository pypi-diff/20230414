# Comparing `tmp/NewsArticlesScraper-0.1.6.tar.gz` & `tmp/NewsArticlesScraper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.1.6.tar", last modified: Mon Mar 27 21:54:54 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.1.7.tar", last modified: Fri Apr 14 11:28:25 2023, max compression
```

## Comparing `NewsArticlesScraper-0.1.6.tar` & `NewsArticlesScraper-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 21:54:54.569907 NewsArticlesScraper-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-03-27 21:54:54.551908 NewsArticlesScraper-0.1.6/NewsArticlesScraper/
--rw-rw-rw-   0        0        0     9292 2023-03-27 21:53:15.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 21:54:54.567907 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-03-27 21:54:54.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-27 21:54:54.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 21:54:54.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-27 21:54:54.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-27 21:54:54.000000 NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-03-27 21:54:54.569406 NewsArticlesScraper-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 21:54:54.569907 NewsArticlesScraper-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-03-27 21:54:35.000000 NewsArticlesScraper-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.935897 NewsArticlesScraper-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.922397 NewsArticlesScraper-0.1.7/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0     9290 2023-04-14 11:26:33.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.934397 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-04-14 11:28:25.935397 NewsArticlesScraper-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:28:25.936397 NewsArticlesScraper-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-14 11:26:33.000000 NewsArticlesScraper-0.1.7/setup.py
```

### Comparing `NewsArticlesScraper-0.1.6/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.1.7/NewsArticlesScraper/Scrapers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     allowed_domains = ["api.queryly.com", "cnbc.com"]
     start_urls = []
     custom_settings = {
         'LOG_LEVEL': 'WARN',
         'USER_AGENT': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/22.0.1207.1 '
                       'Safari/537.1',
         'ROBOTSTXT_OBEY': False,
-        'DOWNLOAD_DELAY': 0.5,
+        'DOWNLOAD_DELAY': 6,
         # 'JOBDIR': './News/CNBCJobs',
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
```

### Comparing `NewsArticlesScraper-0.1.6/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.1.6/PKG-INFO` & `NewsArticlesScraper-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.1.6/setup.py` & `NewsArticlesScraper-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

