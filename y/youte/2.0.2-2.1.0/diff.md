# Comparing `tmp/youte-2.0.2.tar.gz` & `tmp/youte-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youte-2.0.2.tar", last modified: Fri Mar 31 05:44:13 2023, max compression
+gzip compressed data, was "youte-2.1.0.tar", last modified: Fri Apr 14 06:04:13 2023, max compression
```

## Comparing `youte-2.0.2.tar` & `youte-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.303827 youte-2.0.2/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.0.2/.gitignore
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.0.2/.readthedocs.yaml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1856 2023-03-31 05:07:05.000000 youte-2.0.2/CHANGELOG.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.0.2/LICENCE
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14626 2023-03-31 05:44:13.303827 youte-2.0.2/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14088 2023-03-16 07:04:20.000000 youte-2.0.2/README.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.295827 youte-2.0.2/docs/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    13044 2023-03-17 00:42:11.000000 youte-2.0.2/docs/documentation.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.299827 youte-2.0.2/docs/images/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.0.2/docs/images/youte-logo-black-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.0.2/docs/images/youte-logo-white-transparent-1x.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.0.2/docs/images/youte-logo-white-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.0.2/docs/images/youte_save_progress.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.0.2/docs/images/youte_search_results.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.0.2/docs/images/youte_search_results_pretty.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3297 2023-02-16 01:17:30.000000 youte-2.0.2/docs/index.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.0.2/docs/reference.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.303827 youte-2.0.2/docs/stylesheets/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.0.2/docs/stylesheets/extra.css
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.0.2/docs/tutorial.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-03-16 23:52:53.000000 youte-2.0.2/mkdocs.yml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.0.2/noxfile.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      130 2023-03-31 04:32:32.000000 youte-2.0.2/pyproject.toml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.0.2/requirements-mkdocs.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      986 2023-03-31 05:44:13.303827 youte-2.0.2/setup.cfg
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1153 2023-03-31 04:45:59.000000 youte-2.0.2/setup.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.295827 youte-2.0.2/src/
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.303827 youte-2.0.2/src/youte/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2022-06-06 05:58:14.000000 youte-2.0.2/src/youte/__init__.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      994 2023-03-16 07:04:20.000000 youte-2.0.2/src/youte/_typing.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    30588 2023-03-31 02:05:35.000000 youte-2.0.2/src/youte/cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    24891 2023-03-17 07:16:53.000000 youte-2.0.2/src/youte/collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1073 2023-03-16 07:04:20.000000 youte-2.0.2/src/youte/common.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.0.2/src/youte/config.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      453 2023-03-16 07:04:20.000000 youte-2.0.2/src/youte/exceptions.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    13006 2023-03-31 02:06:15.000000 youte-2.0.2/src/youte/parser.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2880 2023-03-31 02:05:35.000000 youte-2.0.2/src/youte/resources.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     5866 2023-03-31 02:05:35.000000 youte-2.0.2/src/youte/table_mappings.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.0.2/src/youte/utilities.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.303827 youte-2.0.2/src/youte.egg-info/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14626 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1019 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/SOURCES.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/dependency_links.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/entry_points.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       95 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/requires.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-03-31 05:44:13.000000 youte-2.0.2/src/youte.egg-info/top_level.txt
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-03-31 05:44:13.303827 youte-2.0.2/tests/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     8118 2023-03-16 07:04:20.000000 youte-2.0.2/tests/test_cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3210 2023-03-16 07:04:20.000000 youte-2.0.2/tests/test_collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      559 2023-03-31 02:07:39.000000 youte-2.0.2/tests/test_database.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2622 2023-03-28 04:07:35.000000 youte-2.0.2/tests/test_parser.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.119552 youte-2.1.0/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.1.0/.gitignore
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.1.0/.readthedocs.yaml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    18508 2023-04-14 05:35:56.000000 youte-2.1.0/CHANGELOG.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.1.0/LICENCE
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16080 2023-04-14 06:04:13.119552 youte-2.1.0/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    15542 2023-04-14 05:35:56.000000 youte-2.1.0/README.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.111552 youte-2.1.0/docs/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14689 2023-04-14 05:35:56.000000 youte-2.1.0/docs/documentation.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/docs/images/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-black-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-white-transparent-1x.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.1.0/docs/images/youte-logo-white-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.1.0/docs/images/youte_save_progress.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.1.0/docs/images/youte_search_results.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.1.0/docs/images/youte_search_results_pretty.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3297 2023-02-16 01:17:30.000000 youte-2.1.0/docs/index.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.1.0/docs/reference.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/docs/stylesheets/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.1.0/docs/stylesheets/extra.css
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.1.0/docs/tutorial.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-03-16 23:52:53.000000 youte-2.1.0/mkdocs.yml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.1.0/noxfile.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.1.0/pyproject.toml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.1.0/requirements-mkdocs.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2023-04-14 06:04:13.119552 youte-2.1.0/setup.cfg
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1255 2023-04-14 05:35:56.000000 youte-2.1.0/setup.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.111552 youte-2.1.0/src/
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/src/youte/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2022-06-06 05:58:14.000000 youte-2.1.0/src/youte/__init__.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/_logging.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      994 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/_typing.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    35928 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    26225 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1073 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/common.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/config.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/database.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      499 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/exceptions.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14406 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/parser.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3080 2023-04-14 05:35:56.000000 youte-2.1.0/src/youte/resources.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.1.0/src/youte/utilities.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.115552 youte-2.1.0/src/youte.egg-info/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16080 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1034 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/SOURCES.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/dependency_links.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/entry_points.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/requires.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-04-14 06:04:13.000000 youte-2.1.0/src/youte.egg-info/top_level.txt
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-04-14 06:04:13.119552 youte-2.1.0/tests/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2820 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_archive.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     8231 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3210 2023-03-16 07:04:20.000000 youte-2.1.0/tests/test_collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2555 2023-04-14 05:35:56.000000 youte-2.1.0/tests/test_parser.py
```

### Comparing `youte-2.0.2/.gitignore` & `youte-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/LICENCE` & `youte-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/PKG-INFO` & `youte-2.1.0/docs/documentation.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,119 +1,102 @@
-Metadata-Version: 2.1
-Name: youte
-Version: 2.0.2
-Summary: Command-line tool to collect video metadata and comments from Youtube API
-Home-page: https://github.com/QUT-Digital-Observatory/youte
-Author: Digital Observatory
-Author-email: digitalobservatory@qut.edu.au
-Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# youte 2.0
-
-A command line utility to get YouTube video metadata and comments from YouTube Data API.
+---
+title: "youte documentation"
+---
 
 ## Changes from youte 1.3.0
 
-Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
+Several major changes are made in youte 2.x. To better correspond with YouTube API endpoints and avoid confusion:
 
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
+- `youte hydrate` is now broken down to `youte videos` and `youte channels`, 
 - `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`.
-- `youte get-related` is now `youte related-to`.
+- `youte most-popular` is now `youte chart`
+- `youte get-related` is now `youte related-to`
 
 Furthermore:
 
 - Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
 - All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
-- You can now tidy data into a CSV or a flat JSON array.
-
-Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
-```bash
+```shell
 python -m pip install youte
-```  
+```
 
-## YouTube API key  
+## YouTube API key
 
 To get data from YouTube API, you will need a YouTube API key. Follow YouTube [instructions](https://developers.google.com/youtube/v3/getting-started) to obtain a YouTube API key if you do not already have one.
 
-## Configure API key (recommended)
+## config
 
-You can save your API key in the youte config file for reuse. To do so, run:
+### Store your API key
 
-```bash  
-youte config add-key
-```  
+While API key can be passed straight to youte commands, you can save your API key in a youte config file for reuse. To do so, run:
 
-The interactive prompt will ask you to input your API key and name it. The name is used to identify the key, and can be anything you choose.
+```shell
+youte config add-key
+```
 
-The prompt will also ask if you want to set the given key as default.
+In the interactive prompt, enter your API key and give it a name. The name is used to identify the key, and can be anything you choose.
 
-When running queries, if no API key or name is specified, `youte` will automatically use the default key.
+You can also choose to set the key as default. When running queries, if no API key or name is specified, `youte` will automatically use the default key.
 
-### Manually set a key as default  
+### See the list of all keys
 
-If you want to manually set an existing key as a default, run:  
+To see the list of all keys and their names stored in the config, run:
 
-```bash  
-youte config set-default <name-of-existing-key>
+```shell
+youte config list-keys
 ```
 
-Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
+The default key, if there is one, will have an asterisk next to it.
 
-#### See the list of all keys  
+### Manually set a key as default
 
-To see the list of all keys, run:  
+If you want to manually set an existing key as a default, run:
 
-```bash  
-youte config list-keys
-```  
+```shell
+youte config set-default <name-of-existing-key>
+```
 
-The default key, if there is one, will have an asterisk next to it.
+Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
 
-#### Remove a key
+### Remove a key
 
 To remove a stored key, run:
 
-```bash
+```shell
 youte config remove <name-of-key>
 ```
 
-#### About the config file  
+### About the config file
 
-youte's config file is stored in a central place whose exact location depends on the running operating system:  
+youte's config file is stored in a central place whose exact location depends on the running operating system:
 
-- Linux/Unix: ~/.config/youte/   
+- Linux/Unix: ~/.config/youte/
 - Mac OS X: ~/Library/Application Support/youte/
-- Windows: C:\Users\\\<user>\\AppData\Roaming\youte
+- Windows: C:\Users\\\<user>\\AppData\\Roaming\\youte
 
 ## search
 
 Searching can be as simple as:
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file.json>
 # OR
 youte search <search-terms> --key <API-key> -o <name-of-file.json>
 ```
 
 If you have a default key set up using `youte config`, then there is no need to specify an API key using `--key`.
 
-This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
+This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal to avoid clogging it up. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
 
 In the search terms, you can also use the Boolean NOT (-) and OR (|) operators to exclude videos or to find videos that match one of several search terms. If the terms contain spaces, the entire search term value has to be wrapped in quotes.
 
-Use the flag `--pretty` to pretty format the JSON output.
+Prettify JSON results by using the flag `--pretty`:
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file> --pretty
 ```
 
 ### Limit pages returned
 
@@ -123,15 +106,15 @@
 youte search <search-terms> --max-pages 5
 # OR
 youte search <search-terms> -m 5
 ```
 
 ### Tidy data
 
-Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
+Raw JSONs from YouTube API contain query metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
@@ -193,17 +176,17 @@
 youte search <search-terms> --limit 5 --type playlist,video
 ```
 
 #### Restrict by language and region
 
 The `--lang` returns results most relevant to a language. Not all results will be in the specified language: results in other languages will still be returned if they are highly relevant to the search query term. To specify the language, use [ISO 639-1 two letter code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes), except that you should use the values `zh-Hans` for simplified Chinese and `zh-Hant` for traditional Chinese.
 
-The `--region` returns results viewable in a region. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2). Note that this option does *not* filter videos uploaded in that region, but rather videos that can be _viewed_ in that region.
+The `--region` returns results viewable in a region. It does *not* filter videos uploaded in that region only. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, and hence should be used with care.
+The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, hence should be used with care.
 
 -  `--location` takes in 2 values - the latitude/longitude coordinates that represent the centre of the area
 -  `--radius` specifies the maximum distance that the location associated with a video can be from that point for the video to still be included in the search results. It must be a number followed by a unit. Valid units are `m`, `km`, `ft`, and `mi`. For example, `1500m`, `5km`, `10000ft`, and `0.75mi`.
 
 Both `--location` and `--radius` have to be specified if they are to be used, otherwise an API error will be thrown.
 
 ### Sort results
@@ -251,45 +234,55 @@
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
 ```shell
 youte comments <id>... --by-video-id --outfile <file.json>
-#OR
+# OR
 youte comments <id>... -v --outfile <file.json>
 ```
 
 To retrieve comments on channels, specify channel ids and pass the `--by-channel-id` or `-c` flag.
 
-```bash
+```shell
 youte comments <id>... --by-channel-id --outfile <file.json>
-OR
+# OR
 youte comments <id>... -c --outfile <file.json>
 ```
 
 If neither of the flags are specified, `youte comments` will assume the ids are thread ids and retrieve the full metadata for those threads.
 
-You can search within the threads and filter threads that match the search terms, by using the `--query` or `-q` option.
+You can search within the threads and filter threads matching the search terms, by using the `--query` or `-q` option.
 
-```bash
+```shell
 youte comments <ids>... -v --outfile <file.json> -q "search term"
 ```
 
 ## replies
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
+## chart
+
+`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
+
+For example:
+
+```shell
+youte chart <region-code> -o <file.json>
+```
+
 ## related-to
 
-`related-to` retrieves videos related to a video.
+`youte related-to` retrieves a list of videos related to a video.
 
 ```shell
 youte related-to <video-ids>... -o <file.json>
 ```
 
 If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
 
@@ -301,43 +294,42 @@
                                   [default: none]
   --region TEXT                   Specify region the videos can be viewed in
                                   (ISO 3166-1 alpha-2 country code)
   --lang TEXT                     Return results most relevant to a language
                                   (ISO 639-1 two-letter code)
 ```
 
-## chart
-
-`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
+## full-archive
 
-For example:
+A new feature added in `youte` 2.1.0 is the ability to run a full archive workflow in one command. `youte full-archive` runs `youte search`, then retrieving video and channel metadata for the search results, as well as getting comments and replies for those videos as well. All data are then tidied and stored in multiple tables in an SQLite database. 
 
 ```shell
-youte chart <region-code> -o <file.json>
+youte full-archive <query> [options] -o <name-of-database-file>
 ```
 
+The search options are identical to `youte search`. Name of the file given to `-o` has to have SQLite extension (i.e. `.db` or `.sqlite`).
+
+Below are the list of tables and the corresponding YouTube resource that they contain:
+
+- `search_result`: search results from `youte search`
+- `video`: videos
+- `channel`: channels
+- `commment`: comment threads and replies
+
+Warning: since `full-archive` will potentially run a large number of queries, it's important to ensure you have enough API quota. You can select which resources to retrieve by using the `--select` option. `--select` takes one or a comma-separated list of YouTube resource types, namely `video`, `channel`, `thread`, and `reply`. Note that if you select `reply`, `thread` also has to be selected. This is because comment thread replies are retrieved using thread IDs, thus collecting comment threads is a must before getting replies. Because of that, if you want to archive the replies, both 'thread' and 'reply' will have to be specified.
+
 ## dehydrate
 
 `dehydrate` extracts the IDs from a JSON file returned from YouTube API.
 
 ```shell
 youte dehydrate <file-name.json>
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
-## YouTube API Quota system and youte handling of quota 
-
-Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
-
-For example:  
-
-- search endpoint costs 100 units per request  
-- video, channel, commentThread, and comment endpoints each costs 1 unit per request  
-
-Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
-
-At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
+## Debugging
 
+The `--verbosity` option, available for most `youte` commands, allows you to turn on debugging messages of the program. Simply specify `--verbosity DEBUG` to turn this mode on.
```

### Comparing `youte-2.0.2/README.md` & `youte-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -297,14 +297,33 @@
 
 For example:
 
 ```shell
 youte chart <region-code> -o <file.json>
 ```
 
+## full-archive
+
+A new feature added in `youte` 2.1.0 is the ability to run a full archive workflow in one command. `youte full-archive` runs `youte search`, then retrieving video and channel metadata for the search results, as well as getting comments and replies for those videos as well. All data are then tidied and stored in multiple tables in an SQLite database. 
+
+```shell
+youte full-archive <query> [options] -o <name-of-database-file>
+```
+
+The search options are identical to `youte search`. Name of the file given to `-o` has to have SQLite extension (i.e. `.db` or `.sqlite`).
+
+Below are the list of tables and the corresponding YouTube resource that they contain:
+
+- `search_result`: search results from `youte search`
+- `video`: videos
+- `channel`: channels
+- `commment`: comment threads and replies
+
+Warning: since `full-archive` will potentially run a large number of queries, it's important to ensure you have enough API quota. You can select which resources to retrieve by using the `--select` option. `--select` takes one or a comma-separated list of YouTube resource types, namely `video`, `channel`, `thread`, and `reply`. Note that if you select `reply`, `thread` also has to be selected. This is because comment thread replies are retrieved using thread IDs, thus collecting comment threads is a must before getting replies. Because of that, if you want to archive the replies, both 'thread' and 'reply' will have to be specified.
+
 ## dehydrate
 
 `dehydrate` extracts the IDs from a JSON file returned from YouTube API.
 
 ```shell
 youte dehydrate <file-name.json>
 ```
```

### Comparing `youte-2.0.2/docs/documentation.md` & `youte-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,119 @@
----
-title: "youte documentation"
----
+Metadata-Version: 2.1
+Name: youte
+Version: 2.1.0
+Summary: Command-line tool to collect video metadata and comments from Youtube API
+Home-page: https://github.com/QUT-Digital-Observatory/youte
+Author: Digital Observatory
+Author-email: digitalobservatory@qut.edu.au
+Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# youte 2.0
+
+A command line utility to get YouTube video metadata and comments from YouTube Data API.
 
 ## Changes from youte 1.3.0
 
-Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion:
+Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
 
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`, 
+- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
 - `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`
-- `youte get-related` is now `youte related-to`
+- `youte most-popular` is now `youte chart`.
+- `youte get-related` is now `youte related-to`.
 
 Furthermore:
 
 - Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
 - All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
+- You can now tidy data into a CSV or a flat JSON array.
+
+Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
-```shell
+```bash
 python -m pip install youte
-```
+```  
 
-## YouTube API key
+## YouTube API key  
 
 To get data from YouTube API, you will need a YouTube API key. Follow YouTube [instructions](https://developers.google.com/youtube/v3/getting-started) to obtain a YouTube API key if you do not already have one.
 
-## config
+## Configure API key (recommended)
 
-### Store your API key
+You can save your API key in the youte config file for reuse. To do so, run:
 
-While API key can be passed straight to youte commands, you can save your API key in a youte config file for reuse. To do so, run:
-
-```shell
+```bash  
 youte config add-key
-```
+```  
 
-In the interactive prompt, enter your API key and give it a name. The name is used to identify the key, and can be anything you choose.
+The interactive prompt will ask you to input your API key and name it. The name is used to identify the key, and can be anything you choose.
 
-You can also choose to set the key as default. When running queries, if no API key or name is specified, `youte` will automatically use the default key.
+The prompt will also ask if you want to set the given key as default.
 
-### See the list of all keys
+When running queries, if no API key or name is specified, `youte` will automatically use the default key.
 
-To see the list of all keys and their names stored in the config, run:
+### Manually set a key as default  
 
-```shell
-youte config list-keys
+If you want to manually set an existing key as a default, run:  
+
+```bash  
+youte config set-default <name-of-existing-key>
 ```
 
-The default key, if there is one, will have an asterisk next to it.
+Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
 
-### Manually set a key as default
+#### See the list of all keys  
 
-If you want to manually set an existing key as a default, run:
+To see the list of all keys, run:  
 
-```shell
-youte config set-default <name-of-existing-key>
-```
+```bash  
+youte config list-keys
+```  
 
-Note that what is passed to this command is the _name_ of the API key, not the API key itself. It follows that the API key has to be first added to the config file using `youte config add-key`. If you use a name that has not been added to the config file, an error will be raised.
+The default key, if there is one, will have an asterisk next to it.
 
-### Remove a key
+#### Remove a key
 
 To remove a stored key, run:
 
-```shell
+```bash
 youte config remove <name-of-key>
 ```
 
-### About the config file
+#### About the config file  
 
-youte's config file is stored in a central place whose exact location depends on the running operating system:
+youte's config file is stored in a central place whose exact location depends on the running operating system:  
 
-- Linux/Unix: ~/.config/youte/
+- Linux/Unix: ~/.config/youte/   
 - Mac OS X: ~/Library/Application Support/youte/
-- Windows: C:\Users\\\<user>\\AppData\\Roaming\\youte
+- Windows: C:\Users\\\<user>\\AppData\Roaming\youte
 
 ## search
 
 Searching can be as simple as:
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file.json>
 # OR
 youte search <search-terms> --key <API-key> -o <name-of-file.json>
 ```
 
 If you have a default key set up using `youte config`, then there is no need to specify an API key using `--key`.
 
-This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal to avoid clogging it up. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
+This will return the maximum number of results pages (around 12-13) matching the search terms and store them in a JSON file. Unlike version 1.3, youte 2.0 does not print results to the terminal. Instead, `--outfile` is now a required option. <search-terms> and `--outfile` must be specified. 
 
 In the search terms, you can also use the Boolean NOT (-) and OR (|) operators to exclude videos or to find videos that match one of several search terms. If the terms contain spaces, the entire search term value has to be wrapped in quotes.
 
-Prettify JSON results by using the flag `--pretty`:
+Use the flag `--pretty` to pretty format the JSON output.
 
 ```bash
 youte search <search-terms> --key <API-key> --outfile <name-of-file> --pretty
 ```
 
 ### Limit pages returned
 
@@ -106,15 +123,15 @@
 youte search <search-terms> --max-pages 5
 # OR
 youte search <search-terms> -m 5
 ```
 
 ### Tidy data
 
-Raw JSONs from YouTube API contain query metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
+Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
@@ -176,17 +193,17 @@
 youte search <search-terms> --limit 5 --type playlist,video
 ```
 
 #### Restrict by language and region
 
 The `--lang` returns results most relevant to a language. Not all results will be in the specified language: results in other languages will still be returned if they are highly relevant to the search query term. To specify the language, use [ISO 639-1 two letter code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes), except that you should use the values `zh-Hans` for simplified Chinese and `zh-Hant` for traditional Chinese.
 
-The `--region` returns results viewable in a region. It does *not* filter videos uploaded in that region only. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+The `--region` returns results viewable in a region. To specify the region, use [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2). Note that this option does *not* filter videos uploaded in that region, but rather videos that can be _viewed_ in that region.
 
-The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, hence should be used with care.
+The `--location` and `--radius` options define a circular geographic area to filter videos that specify, in their metadata, a location within this area. This is *not* a robust and reliable way to geolocate YouTube videos, and hence should be used with care.
 
 -  `--location` takes in 2 values - the latitude/longitude coordinates that represent the centre of the area
 -  `--radius` specifies the maximum distance that the location associated with a video can be from that point for the video to still be included in the search results. It must be a number followed by a unit. Valid units are `m`, `km`, `ft`, and `mi`. For example, `1500m`, `5km`, `10000ft`, and `0.75mi`.
 
 Both `--location` and `--radius` have to be specified if they are to be used, otherwise an API error will be thrown.
 
 ### Sort results
@@ -234,55 +251,45 @@
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
 ```shell
 youte comments <id>... --by-video-id --outfile <file.json>
-# OR
+#OR
 youte comments <id>... -v --outfile <file.json>
 ```
 
 To retrieve comments on channels, specify channel ids and pass the `--by-channel-id` or `-c` flag.
 
-```shell
+```bash
 youte comments <id>... --by-channel-id --outfile <file.json>
-# OR
+OR
 youte comments <id>... -c --outfile <file.json>
 ```
 
 If neither of the flags are specified, `youte comments` will assume the ids are thread ids and retrieve the full metadata for those threads.
 
-You can search within the threads and filter threads matching the search terms, by using the `--query` or `-q` option.
+You can search within the threads and filter threads that match the search terms, by using the `--query` or `-q` option.
 
-```shell
+```bash
 youte comments <ids>... -v --outfile <file.json> -q "search term"
 ```
 
 ## replies
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
-## chart
-
-`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
-
-For example:
-
-```shell
-youte chart <region-code> -o <file.json>
-```
-
 ## related-to
 
-`youte related-to` retrieves a list of videos related to a video.
+`related-to` retrieves videos related to a video.
 
 ```shell
 youte related-to <video-ids>... -o <file.json>
 ```
 
 If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
 
@@ -294,20 +301,62 @@
                                   [default: none]
   --region TEXT                   Specify region the videos can be viewed in
                                   (ISO 3166-1 alpha-2 country code)
   --lang TEXT                     Return results most relevant to a language
                                   (ISO 639-1 two-letter code)
 ```
 
+## chart
+
+`youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
+
+For example:
+
+```shell
+youte chart <region-code> -o <file.json>
+```
+
+## full-archive
+
+A new feature added in `youte` 2.1.0 is the ability to run a full archive workflow in one command. `youte full-archive` runs `youte search`, then retrieving video and channel metadata for the search results, as well as getting comments and replies for those videos as well. All data are then tidied and stored in multiple tables in an SQLite database. 
+
+```shell
+youte full-archive <query> [options] -o <name-of-database-file>
+```
+
+The search options are identical to `youte search`. Name of the file given to `-o` has to have SQLite extension (i.e. `.db` or `.sqlite`).
+
+Below are the list of tables and the corresponding YouTube resource that they contain:
+
+- `search_result`: search results from `youte search`
+- `video`: videos
+- `channel`: channels
+- `commment`: comment threads and replies
+
+Warning: since `full-archive` will potentially run a large number of queries, it's important to ensure you have enough API quota. You can select which resources to retrieve by using the `--select` option. `--select` takes one or a comma-separated list of YouTube resource types, namely `video`, `channel`, `thread`, and `reply`. Note that if you select `reply`, `thread` also has to be selected. This is because comment thread replies are retrieved using thread IDs, thus collecting comment threads is a must before getting replies. Because of that, if you want to archive the replies, both 'thread' and 'reply' will have to be specified.
+
 ## dehydrate
 
 `dehydrate` extracts the IDs from a JSON file returned from YouTube API.
 
 ```shell
 youte dehydrate <file-name.json>
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
+## YouTube API Quota system and youte handling of quota 
+
+Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
+
+For example:  
+
+- search endpoint costs 100 units per request  
+- video, channel, commentThread, and comment endpoints each costs 1 unit per request  
+
+Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
+
+At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
+
```

### Comparing `youte-2.0.2/docs/images/youte-logo-black-transparent.png` & `youte-2.1.0/docs/images/youte-logo-black-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/images/youte-logo-white-transparent-1x.png` & `youte-2.1.0/docs/images/youte-logo-white-transparent-1x.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/images/youte-logo-white-transparent.png` & `youte-2.1.0/docs/images/youte-logo-white-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/images/youte_save_progress.png` & `youte-2.1.0/docs/images/youte_save_progress.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/images/youte_search_results.png` & `youte-2.1.0/docs/images/youte_search_results.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/images/youte_search_results_pretty.png` & `youte-2.1.0/docs/images/youte_search_results_pretty.png`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/index.md` & `youte-2.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/docs/tutorial.md` & `youte-2.1.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/mkdocs.yml` & `youte-2.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/requirements-mkdocs.txt` & `youte-2.1.0/requirements-mkdocs.txt`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/setup.cfg` & `youte-2.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 python_requires = >=3.8
 install_requires = 
 	click >= 8.0.3
 	requests >= 2.27.1
 	python-dateutil >= 2.8.2
 	configobj >= 5.0.6
 	typing_extensions >= 4.5.0
+	SQLAlchemy >= 2.0.7
+	pydantic >= 1.10.7
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts =
```

### Comparing `youte-2.0.2/setup.py` & `youte-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "2.0.2"
+__version__ = "2.1.0"
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setup(
         name="youte",
@@ -26,11 +26,14 @@
         packages=find_packages(where="src"),
         install_requires=[
             "click >= 8.0.3",
             "requests >= 2.27.1",
             "python-dateutil >= 2.8.2",
             "configobj >= 5.0.6",
             "typing_extensions >= 4.5.0",
+            "SQLAlchemy >= 2.0.7",
+            "pydantic >= 1.10.7",
+            "click_log >= 0.4.0"
         ],
         python_requires=">=3.8",
         entry_points={"console_scripts": ["youte=youte.cli:youte"]},
     )
```

### Comparing `youte-2.0.2/src/youte/_typing.py` & `youte-2.1.0/src/youte/_typing.py`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/src/youte/cli.py` & `youte-2.1.0/src/youte/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,94 +4,156 @@
 """
 from __future__ import annotations
 
 import logging
 import sys
 from json.decoder import JSONDecodeError
 from pathlib import Path
-from typing import IO, Literal
+from typing import IO, Callable, Literal
 
 import click
+import click_log
 
+import youte.database as database
 import youte.parser as parser
+from youte._logging import MultiFormatter
 from youte.collector import Youte
 from youte.config import YouteConfig
 from youte.exceptions import ValueAlreadyExists
 from youte.utilities import export_file, retrieve_ids_from_file, validate_date_string
 
 # Logging
+
 logger = logging.getLogger()
-logger.setLevel(logging.INFO)
+logging.getLogger("sqlalchemy.engine").setLevel(logging.WARNING)
 
 console_handler = logging.StreamHandler()
-console_handler.setLevel(logging.INFO)
-console_formatter = logging.Formatter("%(levelname)s: %(message)s")
-console_handler.setFormatter(console_formatter)
+console_handler.setFormatter(MultiFormatter())
+
 logger.addHandler(console_handler)
 
+API_KEY_OPTIONS = [
+    click.option("--name", help="Specify an API key name added to youte config"),
+    click.option("--key", help="Specify a YouTube API key"),
+]
+
+OUTPUT_OPTIONS = [
+    click.option(
+        "-o",
+        "--outfile",
+        type=click.Path(),
+        help="Name of json file to store results to",
+        required=True,
+    ),
+    click.option(
+        "--output-format",
+        default="json",
+        type=click.Choice(["json", "jsonl"]),
+        help="Format of the output file",
+        show_default=True,
+    ),
+    click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON"),
+]
+
+TIDY_OPTIONS = [
+    click.option("--tidy-to", type=click.Path(), help="Parse data and export to file"),
+    click.option(
+        "--format",
+        "format_",
+        type=click.Choice(["json", "csv"]),
+        default="csv",
+        help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
+        show_default=True,
+    ),
+]
+
+
+def api_key_options(func) -> Callable:
+    """Decorator to include api key options for querying commands"""
+    for option in reversed(API_KEY_OPTIONS):
+        func = option(func)
+    return func
+
 
-# file_handler = logging.FileHandler("youte.log")
-# file_handler.setLevel(logging.INFO)
-# file_formatter = logging.Formatter(
-#     "%(asctime)s - %(module)s: %(message)s (%(levelname)s)"
-# )
-# file_handler.setFormatter(file_formatter)
-#
-# logger.addHandler(file_handler)
+def output_options(func) -> Callable:
+    """Decorator to include output options"""
+    for option in reversed(OUTPUT_OPTIONS):
+        func = option(func)
+    return func
+
+
+def tidy_options(func) -> Callable:
+    """Decorator to include tidy option"""
+    for option in reversed(TIDY_OPTIONS):
+        func = option(func)
+    return func
 
 
 def _validate_date(ctx, param, value):
     if value:
         if validate_date_string(value):
             return value
         else:
             raise click.BadParameter("Date not in correct format (YYYY-MM-DD)")
 
 
+def _validate_select_values(ctx, param, value: str) -> str:
+    accept_types: tuple = ("video", "channel", "thread", "reply")
+    value_as_list: list = value.split(",")
+    for v in value_as_list:
+        if v not in accept_types:
+            raise click.BadParameter(
+                f"Contains '{v}'. Accepted values are {accept_types}"
+            )
+    return value
+
+
+def _check_file_overwrite(ctx, param, value: str) -> Path:
+    value = Path(value)
+    if value.exists():
+        try:
+            if click.confirm(
+                f"'{value}' already exists. Keep writing to this file?", abort=True
+            ):
+                return value
+        except click.Abort:
+            click.secho(
+                "Rerun this command and choose a different filename.", fg="green"
+            )
+            raise click.Abort
+
+
 # CLI argument set up:
 @click.group()
 @click.version_option()
 def youte():
     """
     Utility to collect and tidy YouTube meta-data and comments via YouTube API.
     Run `youte --help` to get started.
     """
     pass
 
 
 @youte.command()
 @click.argument("query")
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of json file to store results to",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option(
     "--from", "from_", help="Start date (YYYY-MM-DD)", callback=_validate_date
 )
 @click.option("--to", help="End date (YYYY-MM-DD)", callback=_validate_date)
 @click.option(
     "--type",
     "type_",
     default="video",
     help="Type of resource to search for",
     show_default=True,
+    callback=_validate_select_values,
 )
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
 @click.option(
     "--order",
     type=click.Choice(
         ["date", "rating", "relevance", "title", "videoCount", "viewCount"],
         case_sensitive=False,
     ),
     help="Sort results",
@@ -182,23 +244,15 @@
 )
 @click.option(
     "--max-pages",
     "-m",
     type=click.INT,
     help="Maximum number of result pages to retrieve",
 )
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def search(
     query: str,
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     from_: str,
     to: str,
@@ -272,29 +326,17 @@
             parser.parse_searches(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_searches(results).to_json(tidy_to)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of json file to store results to",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option("-f", "--file-path", help="Use IDs from file", default=None)
 @click.option(
     "--order",
     type=click.Choice(["time", "relevance"]),
     default="time",
     show_default=True,
     help="Specify how comment threads are sorted",
@@ -324,25 +366,15 @@
 )
 @click.option(
     "-v",
     "--by-video-id",
     help="Get all comments for one or a list of videos",
     is_flag=True,
 )
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def comments(
     items: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     order: Literal["time", "relevance"],
     text_format: Literal["html", "plainText"],
@@ -379,19 +411,19 @@
     yob = Youte(api_key=api_key)
 
     vid_ids: list[str] | None = None
     channel_ids: list[str] | None = None
     comment_ids: list[str] | None = None
 
     if by_video_id:
-        vid_ids = _get_ids(items, file_path)
+        vid_ids = _read_ids(items, file_path)
     elif by_channel_id:
-        channel_ids = _get_ids(items, file_path)
+        channel_ids = _read_ids(items, file_path)
     else:
-        comment_ids = _get_ids(items, file_path)
+        comment_ids = _read_ids(items, file_path)
 
     results = [
         result
         for result in yob.get_comment_threads(
             video_ids=vid_ids,
             related_channel_ids=channel_ids,
             comment_ids=comment_ids,
@@ -411,29 +443,17 @@
             parser.parse_comments(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_comments(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of json file to store results to",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option("-f", "--file-path", help="Use IDs from file", default=None)
 @click.option(
     "--text-format",
     type=click.Choice(["html", "plainText"]),
     default="html",
     show_default=True,
     help="Specify the text format of the returned data",
@@ -441,25 +461,15 @@
 @click.option(
     "--max-results",
     type=click.IntRange(0, 100),
     help="Maximum number of results returned per page",
     default=100,
     show_default=True,
 )
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def replies(
     items: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     text_format: Literal["html", "plainText"],
     name: str,
@@ -475,15 +485,15 @@
 
     You can use ids stored in a text file by using --file-path <FILENAME>. The file
     has to contain a line-separated list of ids, with no header.
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
-    ids = _get_ids(items, file_path)
+    ids = _read_ids(items, file_path)
 
     results = [
         result
         for result in yob.get_thread_replies(
             thread_ids=ids, text_format=text_format, max_results=max_results
         )
     ]
@@ -497,48 +507,26 @@
             parser.parse_comments(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_comments(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of json file to store results to",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option("-f", "--file-path", help="Get IDs from file", default=None)
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
 )
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def videos(
     items: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     file_path: Path,
     name: str,
@@ -555,15 +543,15 @@
 
     You can use ids stored in a text file by using --file-path <FILENAME>. The file
     has to contain a line-separated list of ids, with no header.
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
-    ids = _get_ids(string=items, file=file_path)
+    ids = _read_ids(string=items, file=file_path)
 
     results = [
         result for result in yob.get_video_metadata(ids, max_results=max_results)
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
@@ -574,48 +562,26 @@
             parser.parse_videos(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_videos(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of json file to store results to",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option("-f", "--file-path", help="Get IDs from file", default=None)
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
 )
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def channels(
     items: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     file_path: Path,
     name: str,
@@ -632,15 +598,15 @@
 
     You can use ids stored in a text file by using --file-path <FILENAME>. The file
     has to contain a line-separated list of ids, with no header.
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
-    ids = _get_ids(string=items, file=file_path)
+    ids = _read_ids(string=items, file=file_path)
 
     results = [
         result for result in yob.get_channel_metadata(ids=ids, max_results=max_results)
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
@@ -651,33 +617,21 @@
             parser.parse_channels(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_channels(results).to_json(tidy_to, pretty=pretty)
 
 
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
+@output_options
+@tidy_options
+@api_key_options
 @click.option(
     "-f", "--file-path", type=click.Path(), help="Get IDs from file", default=None
 )
 @click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of JSON file to store output",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
-@click.option(
     "--safe-search",
     type=click.Choice(["none", "moderate", "strict"], case_sensitive=False),
     help="Include or exclude restricted content",
     default="none",
     show_default=True,
 )
 @click.option(
@@ -685,38 +639,28 @@
     type=click.STRING,
     help="Specify region the videos can be viewed in (ISO 3166-1 alpha-2 country code)",
 )
 @click.option(
     "--lang",
     help="Return results most relevant to a language (ISO 639-1 two-letter code)",
 )
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
 )
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json', 'jsonl', or 'csv'",
-    show_default=True,
-)
 @click.option(
     "--max-pages",
     "-m",
     type=click.INT,
     help="Maximum number of result pages to retrieve",
 )
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def related_to(
     items: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     safe_search: Literal["none", "moderate", "strict"],
     region: str,
@@ -736,15 +680,15 @@
     videos separately.
 
     ITEMS: ID(s) of videos as provided by YouTube
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
-    ids = _get_ids(string=items, file=file_path)
+    ids = _read_ids(string=items, file=file_path)
 
     results = [
         result
         for result in yob.get_related_videos(
             video_ids=ids,
             region=region,
             relevance_language=lang,
@@ -763,51 +707,29 @@
             parser.parse_searches(results).to_csv(tidy_to)
         elif format_ == "json":
             parser.parse_searches(results).to_json(tidy_to)
 
 
 @youte.command()
 @click.argument("region_code", default="us")
-@click.option(
-    "-o",
-    "--outfile",
-    type=click.Path(),
-    help="Name of JSON file to store output",
-    required=True,
-)
-@click.option(
-    "--output-format",
-    default="json",
-    type=click.Choice(["json", "jsonl"]),
-    help="Format of the output file",
-    show_default=True,
-)
-@click.option("--pretty", "-p", is_flag=True, help="Pretty print JSON")
+@output_options
+@tidy_options
+@api_key_options
 @click.option(
     "--video-category",
     help="Video category ID for which the most popular videos should be retrieved",
 )
-@click.option("--name", help="Specify an API key name added to youte config")
-@click.option("--key", help="Specify a YouTube API key")
 @click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
 )
-@click.option("--tidy-to", type=click.Path(), help="Parse data and export to file")
-@click.option(
-    "--format",
-    "format_",
-    type=click.Choice(["json", "csv"]),
-    default="csv",
-    help="Format data is parsed into. Can be 'json' or 'csv'",
-    show_default=True,
-)
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def chart(
     region_code: str,
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     video_category: str,
     name: str,
@@ -848,14 +770,15 @@
 
 
 @youte.command()
 @click.argument("infile", type=click.Path())
 @click.option(
     "-o", "--output", type=click.File(mode="w"), help="Output text file to store IDs in"
 )
+@click_log.simple_verbosity_option(logger, "--verbosity")
 def dehydrate(infile: Path, output: IO) -> None:
     """Extract an ID list from a file of YouTube resources
 
     This will take in a raw JSON or JSONL output file from YouTube Data API and extract
     the item ids from it. The extracted ids are printed in the terminal or can be piped
     into a text file.
 
@@ -868,14 +791,255 @@
         for id_ in ids:
             click.echo(id_, file=output)
     except JSONDecodeError:
         logging.exception("Error occurred")
         raise click.BadParameter("File is not JSON or there is formatting error")
 
 
+@youte.command()
+@click.argument("query")
+@click.option(
+    "--select",
+    help="Comma separated string specifying which resources to get",
+    default="video,channel,thread,reply",
+    callback=_validate_select_values,
+    show_default=True,
+)
+@click.option(
+    "--out-db",
+    "-o",
+    help="Name of SQLite database to store output (must have .db ending)",
+    type=click.Path(),
+    callback=_check_file_overwrite,
+)
+@api_key_options
+@click.option(
+    "--from", "from_", help="Start date (YYYY-MM-DD)", callback=_validate_date
+)
+@click.option("--to", help="End date (YYYY-MM-DD)", callback=_validate_date)
+@click.option(
+    "--type",
+    "type_",
+    default="video",
+    help="Type of resource to search for",
+    show_default=True,
+    callback=_validate_select_values,
+)
+@click.option(
+    "--order",
+    type=click.Choice(
+        ["date", "rating", "relevance", "title", "videoCount", "viewCount"],
+        case_sensitive=False,
+    ),
+    help="Sort results",
+    show_default=True,
+    default="date",
+)
+@click.option(
+    "--safe-search",
+    type=click.Choice(["none", "moderate", "strict"], case_sensitive=False),
+    help="Include or exclude restricted content",
+    default="none",
+    show_default=True,
+)
+@click.option(
+    "--lang",
+    help="Return results most relevant to a language (ISO 639-1 two-letter code)",
+)
+@click.option(
+    "--region",
+    default="US",
+    help="Return videos viewable in the specified country (ISO 3166-1 alpha-2 code)",
+    show_default=True,
+)
+@click.option(
+    "--video-duration",
+    type=click.Choice(["any", "long", "medium", "short"]),
+    help="Include videos of a certain duration",
+)
+@click.option(
+    "--channel-type",
+    type=click.Choice(["any", "show"]),
+    help="Restrict search to a particular type of channel",
+)
+@click.option(
+    "--video-type",
+    type=click.Choice(["any", "episode", "movie"]),
+    help="Search a particular type of videos",
+)
+@click.option(
+    "--caption",
+    type=click.Choice(["any", "closedCaption", "none"]),
+    help="Filter videos based on if they have captions",
+)
+@click.option(
+    "--definition",
+    "--video-definition",
+    "video_definition",
+    type=click.Choice(["any", "high", "standard"]),
+    help="Include videos by definition",
+)
+@click.option(
+    "--dimension",
+    "--video-dimension",
+    "video_dimension",
+    type=click.Choice(["any", "2d", "3d"]),
+    help="Search 2D or 3D videos",
+)
+@click.option(
+    "--embeddable",
+    "--video-embeddable",
+    "video_embeddable",
+    type=click.Choice(["any", "true"]),
+    help="Search only embeddable videos",
+)
+@click.option(
+    "--license",
+    "--video-license",
+    "video_license",
+    type=click.Choice(["any", "creativeCommon", "youtube"]),
+    help="Include videos with a certain license",
+)
+@click.option(
+    "--location",
+    nargs=2,
+    type=click.FLOAT,
+    help="Lat and long coordinates to restrict search to. --radius must be specified",
+)
+@click.option(
+    "--radius",
+    help="Define the geographic area to restrict search. Must be a number with a unit",
+)
+@click.option(
+    "--max-results",
+    type=click.IntRange(0, 50),
+    help="Maximum number of results returned per page",
+    default=50,
+    show_default=True,
+)
+@click.option(
+    "--max-pages",
+    "-m",
+    type=click.INT,
+    help="Maximum number of result pages to retrieve",
+)
+@click_log.simple_verbosity_option(logger, "--verbosity")
+def full_archive(
+    query: str,
+    select: str,
+    key: str,
+    name: str,
+    out_db: str | Path,
+    from_: str,
+    to: str,
+    order: Literal["date", "rating", "relevance", "title", "videoCount", "viewCount"],
+    video_duration: Literal["any", "long", "medium", "short"],
+    lang: str,
+    region: str,
+    type_: str,
+    channel_type: Literal["any", "show"],
+    video_type: Literal["any", "episode", "movie"],
+    caption: Literal["any", "closedCaption", "none"],
+    video_definition: Literal["any", "high", "standard"],
+    video_dimension: Literal["any", "2d", "3d"],
+    video_embeddable: Literal["any", "true"],
+    video_license: Literal["any", "creativeCommon", "youtube"],
+    safe_search: Literal["none", "moderate", "strict"],
+    location: tuple[float],
+    radius: str,
+    max_pages: int,
+    max_results: int,
+) -> None:
+    """Run full archive workflow
+
+    Extract all related metadata of videos found from a search. This command combines
+    `youte search`, `youte videos`, `youte channels`, `youte comments` and
+    `youte replies` in one clean workflow. Data are cleaned and stored in an SQlite
+    database.
+
+    As this command attempts to archive all YouTube resources, it might take some time
+    to finish. Make sure you have enough quota before running.
+
+    A useful option is `--select`, where you specify which resource types to
+    archive. It can be one or a comma-separated list containing 'video', 'channel',
+    'thread', and 'reply'. Comment thread replies are retrieved using thread IDs,
+    thus collecting comment threads is a must before getting replies. Because of that,
+    if you want to archive the replies, both 'thread' and 'reply' will have to be
+    specified.
+    """
+
+    _check_compatibility(select)
+
+    api_key = key if key else _get_api_key(name=name)
+    yob = Youte(api_key=api_key)
+
+    results = [
+        result
+        for result in yob.search(
+            query=query,
+            type_=type_,
+            start_time=from_,
+            end_time=to,
+            order=order,
+            safe_search=safe_search,
+            language=lang,
+            region=region,
+            video_duration=video_duration,
+            video_type=video_type,
+            caption=caption,
+            video_definition=video_definition,
+            video_embeddable=video_embeddable,
+            location=location,
+            location_radius=radius,
+            video_dimension=video_dimension,
+            max_pages_retrieved=max_pages,
+            max_result=max_results,
+            video_license=video_license,
+            channel_type=channel_type,
+        )
+    ]
+
+    searches = parser.parse_searches(results)
+
+    engine = database.set_up_database(out_db)
+    database.populate_searches(engine, [searches])
+
+    video_ids = [s.id for s in searches.items]
+    channel_ids = [s.channel_id for s in searches.items]
+
+    if "video" in select:
+        click.echo("Retrieving video metadata")
+        click.echo(f"{len(video_ids)} videos being retrieved")
+        results = [result for result in yob.get_video_metadata(video_ids)]
+        _videos = parser.parse_videos(results)
+        database.populate_videos(engine, [_videos])
+
+    if "channel" in select:
+        click.echo("Retrieving channel metadata")
+        click.echo(f"{len(channel_ids)} channels being retrieved")
+        results = [result for result in yob.get_channel_metadata(channel_ids)]
+        _channels = parser.parse_channels(results)
+        database.populate_channels(engine, [_channels])
+
+    if "thread" in select:
+        click.echo("Retrieving comment threads")
+        results = [r for r in yob.get_comment_threads(video_ids)]
+        _comments = parser.parse_comments(results)
+
+        database.populate_comments(engine, [_comments])
+
+        if "reply" in select:
+            thread_ids = [c.id for c in _comments.items if c.total_reply_count > 0]
+            results = [r for r in yob.get_thread_replies(thread_ids)]
+            _replies = parser.parse_comments(results)
+            database.populate_comments(engine, [_replies])
+
+    click.secho(f"ARCHIVING COMPLETED! Data is stored in {out_db}", fg="green")
+
+
 @youte.group()
 def config():
     """
     Set up API keys to access data from YouTube API
     """
 
 
@@ -986,30 +1150,30 @@
 
 
 def _set_up_config(filename=_get_config_path()) -> YouteConfig:
     config_file = YouteConfig(filename=filename)
     return config_file
 
 
-def _get_ids(string: list[str] = None, file: str | Path = None) -> list[str]:
+def _read_ids(string: list[str] = None, file: str | Path = None) -> list[str]:
     if not (string or file):
         raise click.BadParameter("No ids are specified.")
     if string:
         ids = list(string)
     if file:
         with open(file, mode="r") as f:
             ids = [row.rstrip() for row in f.readlines()]
     return ids
 
 
 def _get_api_key(name=None, filename="config"):
     """Get API key from config file.
     If no name is given, use default API key
     """
-    logger.info("Getting API key from config file.")
+    logging.info("Getting API key from config file.")
     config_file_path = Path(click.get_app_dir("youte")).joinpath(filename)
     config_obj = YouteConfig(filename=str(config_file_path))
 
     if name:
         try:
             api_key = config_obj[name]["key"]
         except KeyError:
@@ -1036,7 +1200,19 @@
                 bold=True,
             )
             sys.exit(1)
         else:
             api_key = config_obj[default_check[0]]["key"]
 
     return api_key
+
+
+def _check_compatibility(value: str) -> str:
+    """Helper function to check that 'thread' and 'reply' must be used together
+    in `youte full-archive`
+    """
+    if "reply" in value and "thread" not in value:
+        raise click.BadOptionUsage(
+            option_name="--select",
+            message=f"Is '{value}'. 'thread' has to be specified with 'reply'",
+        )
+    return value
```

### Comparing `youte-2.0.2/src/youte/collector.py` & `youte-2.1.0/src/youte/collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
-import json
 import logging
 import random
 from datetime import datetime, timedelta
 from typing import Iterator, Literal, Optional
 
 import requests
 from dateutil import tz
 
 from youte._typing import APIResponse, SearchOrder
-from youte.exceptions import APIError, InvalidRequest
+from youte.exceptions import APIError, CommentsDisabled, InvalidRequest
 from youte.utilities import create_utc_datetime_string
 
 logger = logging.getLogger(__name__)
 
 
 class Youte:
     def __init__(self, api_key: str):
@@ -128,16 +127,16 @@
             "videoDimension": video_dimension,
             "videoEmbeddable": video_embeddable,
             "videoLicense": video_license,
             "videoType": video_type,
             "relevanceLanguage": language,
             "regionCode": region,
         }
-
-        yield from _paginate_search_results(
+        logger.debug(f"Search query: {params}")
+        yield from _paginate_results(
             url=url, max_pages_retrieved=max_pages_retrieved, **params
         )
 
     def get_video_metadata(
         self,
         ids: list[str],
         part: Optional[list[str]] = None,
@@ -180,30 +179,32 @@
             "maxResults": max_results,
             "key": self.api_key,
         }
 
         if not isinstance(ids, list):
             raise TypeError("ids must be a list")
 
-        ids = list(set(ids))
+        ids: list[str] = list(set(ids))
+
+        total_batches: int = int(len(ids) / 50)
 
         while ids:
             if len(ids) <= 50:
                 ids_string = ",".join(ids)
                 ids = []
             else:
-                total_batches = int(len(ids) / 50)
-                logger.info(f"{total_batches} pages remaining")
                 batch = random.sample(ids, k=50)
                 ids_string = ",".join(batch)
                 for elm in batch:
                     ids.remove(elm)
-
             params["id"] = ids_string
-            yield from _paginate_search_results(url=url, **params)
+            logger.info(f"Retrieving video metadata: {total_batches} batches left")
+            logger.debug(f"Retrieving metadata for videos: {params['id']}")
+            total_batches -= 1
+            yield from _paginate_results(url=url, **params)
 
     def get_channel_metadata(
         self,
         ids: list[str],
         part: Optional[list[str]] = None,
         max_results: int = 50,
     ) -> Iterator[APIResponse]:
@@ -246,29 +247,32 @@
             "maxResults": max_results,
             "key": self.api_key,
         }
 
         if ids and not isinstance(ids, list):
             raise TypeError("ids and username must be a list")
 
+        total_batches: int = int(len(ids) / 50)  # logging purpose only
+
         while ids:
             ids = list(set(ids))
             if len(ids) <= 50:
                 ids_string = ",".join(ids)
                 ids = []
             else:
-                total_batches = int(len(ids) / 50)
-                logger.info(f"{total_batches} pages remaining")
                 batch = random.sample(ids, k=50)
                 ids_string = ",".join(batch)
                 for elm in batch:
                     ids.remove(elm)
 
             params["id"] = ids_string
-            yield from _paginate_search_results(url=url, **params)
+            logger.info(f"Retrieving channel metadata: {total_batches} pages remaining")
+            logger.debug(f"Retrieving metadata for channels: {params['id']}")
+            total_batches -= 1
+            yield from _paginate_results(url=url, **params)
 
     def get_comment_threads(
         self,
         video_ids: Optional[list[str]] = None,
         related_channel_ids: Optional[list[str]] = None,
         comment_ids: Optional[list[str]] = None,
         order: Literal["time", "relevance"] = "time",
@@ -332,50 +336,64 @@
         url: str = r"https://www.googleapis.com/youtube/v3/commentThreads"
         params: dict[str, str | int] = {
             "part": "snippet",
             "textFormat": text_format,
             "key": self.api_key,
         }
 
+        i: int = 1  # logging purpose only
+
         if video_ids:
             params["order"] = order
             params["maxResults"] = max_results
             if search_terms:
                 params["searchTerms"] = search_terms
             for video_id in video_ids:
                 params["videoId"] = video_id
-                yield from _paginate_search_results(url=url, **params)
+                logger.info(
+                    f"{i}/{len(video_ids)}: Retrieving comments for video {video_id}"
+                )
+                logger.debug(f"Query {url}: {params}")
+                i += 1
+                yield from _paginate_results(url=url, **params)
 
         if related_channel_ids:
             params["order"] = order
             params["maxResults"] = max_results
             if search_terms:
                 params["searchTerms"] = search_terms
             for channel_id in related_channel_ids:
                 params["allThreadsRelatedToChannelId"] = channel_id
-                yield from _paginate_search_results(url=url, **params)
+                logger.info(
+                    f"{i}/{len(related_channel_ids)}: "
+                    f"Retrieving comments for channel {channel_id}"
+                )
+                logger.debug(f"Query {url}: {params}")
+                i += 1
+                yield from _paginate_results(url=url, **params)
 
         if comment_ids:
-            url: str = r"https://www.googleapis.com/youtube/v3/commentThreads"
-
             comment_ids = list(set(comment_ids))
+            total_batches = int(len(comment_ids) / 50)  # logging purpose only
+
             while comment_ids:
                 if len(comment_ids) <= 50:
                     ids_string = ",".join(comment_ids)
                     comment_ids = []
                 else:
-                    total_batches = int(len(comment_ids) / 50)
-                    logger.info(f"{total_batches} pages remaining")
                     batch = random.sample(comment_ids, k=50)
                     ids_string = ",".join(batch)
                     for elm in batch:
                         comment_ids.remove(elm)
 
                 params["id"] = ids_string
-                yield from _paginate_search_results(url=url, **params)
+                logger.info(f"Retrieving comments: {total_batches} pages remaining")
+                logger.debug(f"Retrieving comments: {params['id']}")
+                total_batches -= 1
+                yield from _paginate_results(url=url, **params)
 
     def get_thread_replies(
         self,
         thread_ids: list[str],
         text_format: Literal["html", "plainText"] = "html",
         max_results: int = 100,
     ) -> Iterator[APIResponse]:
@@ -407,17 +425,23 @@
             "key": self.api_key,
         }
 
         if thread_ids and not isinstance(thread_ids, list):
             raise TypeError("thread_ids must be a list")
 
         thread_ids = list(set(thread_ids))
+        i: int = 1  # logging purpose only
         for thread_id in thread_ids:
             params["parentId"] = thread_id
-            yield from _paginate_search_results(url=url, **params)
+            logger.info(
+                f"{i}/{len(thread_ids)}: Retrieving replies for thread {thread_id}"
+            )
+            logger.debug(f"Query {url}: {params}")
+            i += 1
+            yield from _paginate_results(url=url, **params)
 
     def get_most_popular(
         self,
         region_code: str = "us",
         video_category_id: Optional[str] = None,
         max_results: int = 100,
         part: list[str] = None,
@@ -455,16 +479,17 @@
             "part": part,
             "maxResults": max_results,
             "key": self.api_key,
             "chart": "mostPopular",
             "regionCode": region_code,
             "videoCategoryId": video_category_id,
         }
+        logger.debug(f"Query {url}: {params}")
 
-        yield from _paginate_search_results(url=url, **params)
+        yield from _paginate_results(url=url, **params)
 
     def get_related_videos(
         self,
         video_ids: list[str],
         region: Optional[str] = None,
         relevance_language: Optional[str] = None,
         safe_search: Literal["none", "moderate", "strict"] = "none",
@@ -509,78 +534,82 @@
             "regionCode": region,
             "relevanceLanguage": relevance_language,
             "safeSearch": safe_search,
             "key": self.api_key,
             "type": "video",
         }
 
+        i: int = 1  # logging purpose only
+
         for video_id in video_ids:
             params["relatedToVideoId"] = video_id
-            for result in _paginate_search_results(
+            logger.info(f"{i}/{len(video_ids)} Getting videos related to {video_id}")
+            logger.debug(f"Query {url}: {params}")
+            for result in _paginate_results(
                 url=url, max_pages_retrieved=max_pages_retrieved, **params
             ):
-                result["related_to_video_id"] = video_id  # type: ignore
+                result["related_to_video_id"] = video_id
                 yield result
 
 
-def _paginate_search_results(
+def _paginate_results(
     url: str, max_pages_retrieved: Optional[int] = None, **kwargs
 ) -> Iterator[APIResponse]:
     page: int = 0
     logger.info(f"Getting page {page + 1}")
-    r = _request(url=url, params=kwargs)
-    page += 1
-    response = _add_meta(r.json(), collection_time=datetime.now())
-    yield response
-
-    while "nextPageToken" in r.json():
-        if max_pages_retrieved and page >= max_pages_retrieved:
-            logger.info("Max pages reached")
-            break
-        else:
-            logger.info(f"Getting page {page + 1}")
-            next_page_token = r.json()["nextPageToken"]
-            kwargs["pageToken"] = next_page_token
-            r = _request(url=url, params=kwargs)
-            page += 1
-            response = _add_meta(r.json(), collection_time=datetime.now())
-            yield response
+
+    try:
+        r = _request(url=url, params=kwargs)
+        page += 1
+        response = _add_meta(r.json(), collection_time=datetime.now())
+        yield response
+
+        while "nextPageToken" in r.json():
+            if max_pages_retrieved and page >= max_pages_retrieved:
+                logger.info("Max pages reached")
+                break
+            else:
+                logger.info(f"Getting page {page + 1}")
+                next_page_token = r.json()["nextPageToken"]
+                kwargs["pageToken"] = next_page_token
+                r = _request(url=url, params=kwargs)
+                page += 1
+                response = _add_meta(r.json(), collection_time=datetime.now())
+                yield response
+    except CommentsDisabled:
+        logger.warning("Comments are disabled.")
 
 
 def _add_meta(response: APIResponse, **kwargs) -> APIResponse:
     for key in kwargs:
         response[key] = kwargs[key]
 
     return response
 
 
 def _request(url: str, params: dict[str, str | int]) -> requests.Response:
     response = requests.get(url, params=params)
-    logger.debug(f"Getting {response.url}")
-    logger.info(f"Status code: {response.status_code}")
+    logger.debug(f"Getting {response.url}: {response.status_code}")
 
     if response.status_code in [403, 400, 404]:
         try:
             errors = response.json()
         except requests.exceptions.JSONDecodeError:
             raise InvalidRequest("Check url and endpoint.")
 
-        logger.error(f"Error {response.status_code}: {response.url}")
-        logger.error(json.dumps(errors))
-
         for error in errors["error"]["errors"]:
-            # ignore if comment is disabled
             if error["reason"] == "commentsDisabled":
-                logger.warning(error["reason"])
+                raise CommentsDisabled(error["reason"])
             elif "quotaExceeded" in error["reason"]:
                 until_reset = _get_reset_remaining(datetime.now(tz=tz.UTC))
                 raise APIError(
                     f"{error['reason']}\n{until_reset} seconds til quota reset time"
                 )
             else:
+                logger.error(f"Error {response.status_code}: {response.url}")
                 raise APIError(error["message"])
 
     return response
 
 
 def _get_reset_remaining(current: datetime) -> int:
     next_reset = datetime.now(tz=tz.gettz("US/Pacific")) + timedelta(days=1)
```

### Comparing `youte-2.0.2/src/youte/common.py` & `youte-2.1.0/src/youte/common.py`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/src/youte/config.py` & `youte-2.1.0/src/youte/config.py`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/src/youte/parser.py` & `youte-2.1.0/src/youte/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
 import html
+import logging
 from datetime import datetime
 from typing import Iterable, Iterator, Optional
 
+from pydantic import ValidationError
+
 from youte._typing import SearchResult, StandardResult, VideoChannelResult
 from youte.resources import (
     Channel,
     Channels,
     Comment,
     Comments,
     Search,
     Searches,
     Video,
     Videos,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def parse_search(data: SearchResult) -> Searches:
     """Parse a single page of search results from Youte.search() into a list
     of Search objects. These Search objects are like dictionaries with keys
     representing attributes of the search results.
 
     Args:
@@ -43,14 +48,15 @@
 
     Returns:
         A list of Search objects.
     """
     searches: list[Search] = []
     for each in data:
         for search in _parse_search(each):
+            logger.debug(f"Parsing search item {search.id}: {search.title}")
             searches.append(search)
     return Searches(items=searches)
 
 
 def parse_video(data: VideoChannelResult) -> Videos:
     """Parse a single page of results from Youte.get_video_metadata() or
     Youte.get_most_popular() into a list of Video objects. These Video objects are
@@ -80,14 +86,15 @@
 
     Returns:
         A Videos object containing a list of Video objects.
     """
     videos: list[Video] = []
     for each in data:
         for video in _parse_video(each):
+            logger.debug(f"Parsing video {video.id}: {video.title}")
             videos.append(video)
     return Videos(items=videos)
 
 
 def parse_channel(data: VideoChannelResult) -> Channels:
     """Parse a single page of results from Youte.get_channel_metadata() into a list of
     Channel objects. These Channel objects are like dictionaries with keys representing
@@ -115,14 +122,15 @@
 
     Returns:
         A Channels object containing a list of Channel objects.
     """
     channels: list[Channel] = []
     for each in data:
         for channel in _parse_channel(each):
+            logger.debug(f"Parsing channel {channel.id}: {channel.title}")
             channels.append(channel)
     return Channels(items=channels)
 
 
 def parse_comment(data: StandardResult) -> Comments:
     """Parse a single page of results from Youte.get_comment_thread() or
      Youte.get_thread_replies() into a list of Comments objects. These Comment objects
@@ -152,14 +160,15 @@
 
     Returns:
         A Comments object containing a list of Comment objects.
     """
     cmts: list[Comment] = []
     for each in data:
         for cmt in _parse_comment(each):
+            logger.debug(f"Parsing comment {cmt.id}")
             cmts.append(cmt)
     return Comments(items=cmts)
 
 
 def _parse_search(input_: SearchResult) -> Iterator[Search]:
     if "searchListResponse" not in input_["kind"]:
         raise ValueError(
@@ -171,27 +180,28 @@
     for item in items:
         snippet = item["snippet"]
 
         for elem in item["id"]:
             if "id" in elem or "Id" in elem:
                 id_: str = item["id"][elem]
 
+        # noinspection PyArgumentList
         search = Search(
             kind=item["id"]["kind"],
             id=id_,
             description=snippet["description"],
             published_at=_parse_rfc3339(snippet["publishedAt"]),
             title=html.unescape(snippet["title"]),
             thumbnail_url=snippet["thumbnails"]["high"]["url"],
             thumbnail_height=snippet["thumbnails"]["high"]["height"],
             thumbnail_width=snippet["thumbnails"]["high"]["width"],
-            channel_title=snippet["channelTitle"],
+            channel_title=snippet.get("channelTitle"),
             live_broadcast_content=snippet["liveBroadcastContent"],
+            channel_id=snippet["channelId"],
         )
-
         yield search
 
 
 def _parse_video(input_: VideoChannelResult) -> Iterator[Video]:
     if "videoListResponse" not in input_["kind"]:
         raise ValueError(
             f"Object passed to input is {input_['kind']} not a videoListResponse"
@@ -205,14 +215,15 @@
         status = item["status"]
         statistics = item["statistics"]
         topic_details = item.get("topicDetails")
         live_stream = (
             item["liveStreamingDetails"] if "liveStreamingDetails" in item else {}
         )
 
+        # noinspection PyArgumentList
         search = Video(
             kind=item["kind"],
             id=item["id"],
             description=snippet["description"],
             published_at=_parse_rfc3339(snippet["publishedAt"]),
             title=snippet["title"],
             thumbnail_url=snippet["thumbnails"]["high"]["url"],
@@ -240,21 +251,32 @@
             made_for_kids=status["madeForKids"],
             view_count=statistics.get("viewCount"),
             like_count=statistics.get("likeCount"),
             comment_count=statistics.get("commentCount"),
             topic_categories=topic_details["topicCategories"]
             if topic_details
             else None,
-            live_streaming_start_actual=live_stream.get("actualStartTime"),
-            live_streaming_end_actual=live_stream.get("actualEndTime"),
-            live_streaming_start_scheduled=live_stream.get("scheduledStartTime"),
-            live_streaming_end_scheduled=live_stream.get("scheduledEndTime"),
-            live_streaming_concurrent_viewers=live_stream.get("concurrentViewers"),
+            live_streaming_start_actual=_parse_rfc3339(live_stream["actualStartTime"])
+            if "actualStartTime" in live_stream
+            else None,
+            live_streaming_end_actual=_parse_rfc3339(live_stream["actualEndTime"])
+            if "actualEndTime" in live_stream
+            else None,
+            live_streaming_start_scheduled=_parse_rfc3339(
+                live_stream["scheduledStartTime"]
+            )
+            if "scheduledStartTime" in live_stream
+            else None,
+            live_streaming_end_scheduled=_parse_rfc3339(live_stream["scheduledEndTime"])
+            if "scheduledEndTime" in live_stream
+            else None,
+            live_streaming_concurrent_viewers=int(live_stream["concurrentViewers"])
+            if "concurrentViewers" in live_stream
+            else None,
         )
-
         yield search
 
 
 def _parse_channel(input_: VideoChannelResult) -> Iterator[Channel]:
     if "channelListResponse" not in input_["kind"]:
         raise ValueError("Object passed to input is not a channelListResponse")
 
@@ -263,41 +285,46 @@
     for item in items:
         snippet = item["snippet"]
         status = item["status"]
         statistics = item["statistics"]
         topic_details = item.get("topicDetails")
         branding = item["brandingSettings"]
 
-        channel = Channel(
-            kind=item["kind"],
-            id=item["id"],
-            title=snippet["title"],
-            description=snippet["description"],
-            custom_url=snippet["customUrl"],
-            published_at=_parse_rfc3339(snippet["publishedAt"]),
-            thumbnail_url=snippet["thumbnails"]["high"]["url"],
-            thumbnail_height=snippet["thumbnails"]["high"]["height"],
-            thumbnail_width=snippet["thumbnails"]["high"]["width"],
-            default_language=snippet.get("defaultLanguage"),
-            localized_title=snippet["localized"]["title"],
-            localized_description=snippet["localized"]["description"],
-            country=branding["channel"].get("country"),
-            view_count=statistics["viewCount"],
-            subscriber_count=statistics["subscriberCount"],
-            video_count=statistics["videoCount"],
-            hidden_subscriber_count=statistics["hiddenSubscriberCount"],
-            topic_categories=topic_details["topicCategories"]
-            if topic_details
-            else None,
-            privacy_status=status["privacyStatus"],
-            is_linked=status["isLinked"],
-            made_for_kids=status.get("madeForKids"),
-            branding_keywords=branding["channel"].get("keywords"),
-            moderated_comments=branding["channel"].get("moderatedComments"),
-        )
+        try:
+            # noinspection PyArgumentList
+            channel = Channel(
+                kind=item["kind"],
+                id=item["id"],
+                title=snippet["title"],
+                description=snippet["description"],
+                custom_url=snippet["customUrl"],
+                published_at=_parse_rfc3339(snippet["publishedAt"]),
+                thumbnail_url=snippet["thumbnails"]["high"]["url"],
+                thumbnail_height=snippet["thumbnails"]["high"]["height"],
+                thumbnail_width=snippet["thumbnails"]["high"]["width"],
+                default_language=snippet.get("defaultLanguage"),
+                localized_title=snippet["localized"]["title"],
+                localized_description=snippet["localized"]["description"],
+                country=branding["channel"].get("country"),
+                view_count=statistics["viewCount"],
+                subscriber_count=statistics["subscriberCount"],
+                video_count=statistics["videoCount"],
+                hidden_subscriber_count=statistics["hiddenSubscriberCount"],
+                topic_categories=topic_details["topicCategories"]
+                if topic_details
+                else None,
+                privacy_status=status["privacyStatus"],
+                is_linked=status["isLinked"],
+                made_for_kids=status.get("madeForKids"),
+                branding_keywords=_list(branding["channel"].get("keywords")),
+                moderated_comments=branding["channel"].get("moderatedComments"),
+            )
+        except ValidationError:
+            print(branding["channel"].get("keywords"))
+            raise ValidationError
 
         yield channel
 
 
 def _parse_comment(input_: StandardResult) -> Iterable[Comment]:
     if "comment" not in input_["kind"]:
         raise ValueError("Object passed to input is not a comment")
@@ -312,21 +339,23 @@
             snippet = item["snippet"]["topLevelComment"]["snippet"]
             can_reply = item["snippet"]["canReply"]
             total_reply_count = item["snippet"]["totalReplyCount"]
             is_public = item["snippet"]["isPublic"]
         else:
             snippet = item["snippet"]
 
+        # noinspection PyArgumentList
         comment = Comment(
             id=item["id"],
-            channel_id=snippet.get("channelId"),
-            video_id=snippet["videoId"],
+            video_id=snippet.get("videoId"),
             author_display_name=snippet["authorDisplayName"],
             author_profile_image_url=snippet["authorProfileImageUrl"],
-            author_channel_id=snippet["authorChannelId"]["value"],
+            author_channel_id=snippet["authorChannelId"]["value"]
+            if "authorChannelId" in snippet
+            else None,
             author_channel_url=snippet["authorChannelUrl"],
             text_display=snippet["textDisplay"],
             text_original=snippet["textOriginal"],
             parent_id=snippet.get("parentId"),
             can_rate=snippet["canRate"],
             viewer_rating=snippet["viewerRating"],
             like_count=snippet["likeCount"],
@@ -343,7 +372,14 @@
     """Parser function for RFC3339 datetime string returned from YouTube.
     fromisoformat() does not work with this format, except in Python 3.11
     """
     try:
         return datetime.strptime(string, "%Y-%m-%dT%H:%M:%S.%f%z")
     except ValueError:
         return datetime.strptime(string, "%Y-%m-%dT%H:%M:%S%z")
+
+
+def _list(string: str | None) -> list | None:
+    if string:
+        return string.split(" ")
+    else:
+        return string
```

### Comparing `youte-2.0.2/src/youte/resources.py` & `youte-2.1.0/src/youte/resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
 from datetime import datetime
 from typing import List, Literal, Optional
 
+from pydantic.dataclasses import dataclass
+
 from youte.common import Resources
 
 
 @dataclass
 class Search:
     kind: str
     id: str
     published_at: datetime
     title: str
     description: str
+    channel_id: str
     thumbnail_url: str
     thumbnail_width: int
     thumbnail_height: int
     channel_title: str
     live_broadcast_content: str
 
 
@@ -34,35 +36,35 @@
     channel_id: str
     title: str
     description: str
     thumbnail_url: str
     thumbnail_width: int
     thumbnail_height: int
     channel_title: str
-    tags: List[str]
+    tags: Optional[List[str]]
     category_id: str
     localized_title: str
     localized_description: str
-    default_language: str
-    default_audio_language: str
+    default_language: Optional[str]
+    default_audio_language: Optional[str]
     duration: str
     dimension: str
     definition: Literal["hd", "sd"]
     caption: bool
     licensed_content: bool
     projection: Literal["360", "rectangular"]
     upload_status: str
     privacy_status: Literal["private", "public", "unlisted"]
     license: Literal["creativeCommon", "youtube"]
     embeddable: bool
     public_stats_viewable: bool
     made_for_kids: bool
     view_count: int
-    like_count: int
-    comment_count: int
+    like_count: Optional[int]
+    comment_count: Optional[int]
     topic_categories: Optional[List[str]]
     live_streaming_start_actual: Optional[datetime]
     live_streaming_end_actual: Optional[datetime]
     live_streaming_start_scheduled: Optional[datetime]
     live_streaming_end_scheduled: Optional[datetime]
     live_streaming_concurrent_viewers: Optional[int]
 
@@ -74,58 +76,57 @@
 
 @dataclass
 class Channel:
     kind: str
     id: str
     title: str
     description: str
-    custom_url: str
+    custom_url: Optional[str]
     published_at: datetime
     thumbnail_url: str
     thumbnail_height: int
     thumbnail_width: int
-    default_language: str
+    default_language: Optional[str]
     localized_title: str
     localized_description: str
-    country: str
-    view_count: int
-    subscriber_count: int
+    country: Optional[str]
+    view_count: Optional[str]
+    subscriber_count: Optional[str]
     hidden_subscriber_count: bool
     video_count: int
-    topic_categories: List[str]
+    topic_categories: Optional[List[str]]
     privacy_status: Literal["private", "public", "unlisted"]
     is_linked: bool
-    made_for_kids: bool
-    branding_keywords: List[str]
-    moderated_comments: bool
+    made_for_kids: Optional[bool]
+    branding_keywords: Optional[List[str]]
+    moderated_comments: Optional[bool]
 
 
 @dataclass
 class Channels(Resources):
     items: List[Channel]
 
 
 @dataclass
 class Comment:
     id: str
-    channel_id: str
-    video_id: str
-    parent_id: str
-    can_reply: bool
-    total_reply_count: int
-    is_public: bool
+    video_id: Optional[str]
+    parent_id: Optional[str]
+    can_reply: Optional[bool]
+    total_reply_count: Optional[int]
+    is_public: Optional[bool]
     author_display_name: str
     author_profile_image_url: str
     author_channel_url: str
     author_channel_id: str
     text_display: str
     text_original: str
     can_rate: bool
     viewer_rating: Literal["like", "none"]
-    like_count: str
+    like_count: int
     published_at: datetime
     updated_at: datetime
 
 
 @dataclass
 class Comments(Resources):
     items: List[Comment]
```

### Comparing `youte-2.0.2/src/youte/utilities.py` & `youte-2.1.0/src/youte/utilities.py`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/src/youte.egg-info/PKG-INFO` & `youte-2.1.0/src/youte.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.0.2
+Version: 2.1.0
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -311,14 +311,33 @@
 
 For example:
 
 ```shell
 youte chart <region-code> -o <file.json>
 ```
 
+## full-archive
+
+A new feature added in `youte` 2.1.0 is the ability to run a full archive workflow in one command. `youte full-archive` runs `youte search`, then retrieving video and channel metadata for the search results, as well as getting comments and replies for those videos as well. All data are then tidied and stored in multiple tables in an SQLite database. 
+
+```shell
+youte full-archive <query> [options] -o <name-of-database-file>
+```
+
+The search options are identical to `youte search`. Name of the file given to `-o` has to have SQLite extension (i.e. `.db` or `.sqlite`).
+
+Below are the list of tables and the corresponding YouTube resource that they contain:
+
+- `search_result`: search results from `youte search`
+- `video`: videos
+- `channel`: channels
+- `commment`: comment threads and replies
+
+Warning: since `full-archive` will potentially run a large number of queries, it's important to ensure you have enough API quota. You can select which resources to retrieve by using the `--select` option. `--select` takes one or a comma-separated list of YouTube resource types, namely `video`, `channel`, `thread`, and `reply`. Note that if you select `reply`, `thread` also has to be selected. This is because comment thread replies are retrieved using thread IDs, thus collecting comment threads is a must before getting replies. Because of that, if you want to archive the replies, both 'thread' and 'reply' will have to be specified.
+
 ## dehydrate
 
 `dehydrate` extracts the IDs from a JSON file returned from YouTube API.
 
 ```shell
 youte dehydrate <file-name.json>
 ```
```

### Comparing `youte-2.0.2/src/youte.egg-info/SOURCES.txt` & `youte-2.1.0/src/youte.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 docs/images/youte-logo-white-transparent-1x.png
 docs/images/youte-logo-white-transparent.png
 docs/images/youte_save_progress.png
 docs/images/youte_search_results.png
 docs/images/youte_search_results_pretty.png
 docs/stylesheets/extra.css
 src/youte/__init__.py
+src/youte/_logging.py
 src/youte/_typing.py
 src/youte/cli.py
 src/youte/collector.py
 src/youte/common.py
 src/youte/config.py
+src/youte/database.py
 src/youte/exceptions.py
 src/youte/parser.py
 src/youte/resources.py
-src/youte/table_mappings.py
 src/youte/utilities.py
 src/youte.egg-info/PKG-INFO
 src/youte.egg-info/SOURCES.txt
 src/youte.egg-info/dependency_links.txt
 src/youte.egg-info/entry_points.txt
 src/youte.egg-info/requires.txt
 src/youte.egg-info/top_level.txt
+tests/test_archive.py
 tests/test_cli.py
 tests/test_collector.py
-tests/test_database.py
 tests/test_parser.py
```

### Comparing `youte-2.0.2/tests/test_cli.py` & `youte-2.1.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,23 @@
 
 # TEST channels COMMAND
 
 
 def test_cli_channels(runner, outfile_json):
     results = runner.invoke(
         youte,
-        ["channels", "-f", Path("tests") / "channel_ids.csv", "-o", outfile_json],
+        [
+            "channels",
+            "-f",
+            Path("tests") / "channel_ids.csv",
+            "-o",
+            outfile_json,
+            "--key",
+            API_KEY,
+        ],
     )
     assert results.exit_code == 0
 
     with open(outfile_json, "r") as file:
         r: list[dict] = json.loads(file.read())
         assert len(r[0]["items"]) >= 10
```

### Comparing `youte-2.0.2/tests/test_collector.py` & `youte-2.1.0/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `youte-2.0.2/tests/test_parser.py` & `youte-2.1.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
 
 def test_tidy_video_multiple(yob):
     videos = [
         video for video in yob.get_video_metadata(ids=["qFagsLxu2Xs", "4MQyV7Wluhs"])
     ]
     tidied = parse_videos(videos)  # type: ignore
-    tidied.to_json("test_tidy.json", pretty=True)
-    tidied.to_csv("test_tidy.csv")
+    print(tidied)
     assert isinstance(tidied, Videos)
 
 
 def test_tidy_channel_one(yob):
     ids = ["UC_NN7u1HKTQR6vurmS9iQ1A", "UCMhRG26kBpMp3GAZv5Iv7sw"]
     channels = [ch for ch in yob.get_channel_metadata(ids=ids)]
     tidied = parse_channel(channels[0])  # type: ignore
```

