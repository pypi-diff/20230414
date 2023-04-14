# Comparing `tmp/phpdoc-trans-0.0.4.tar.gz` & `tmp/phpdoc-trans-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpdoc-trans-0.0.4.tar", last modified: Fri Apr 14 09:58:05 2023, max compression
+gzip compressed data, was "phpdoc-trans-0.0.5.tar", last modified: Fri Apr 14 10:10:00 2023, max compression
```

## Comparing `phpdoc-trans-0.0.4.tar` & `phpdoc-trans-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/phpdoc_trans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:00.201129 phpdoc-trans-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 10:10:00.197129 phpdoc-trans-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:00.197129 phpdoc-trans-0.0.5/phpdoc_trans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/phpdoc_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/phpdoc_trans/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/phpdoc_trans/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:00.197129 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 10:10:00.000000 phpdoc-trans-0.0.5/phpdoc_trans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:10:00.201129 phpdoc-trans-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 10:09:50.000000 phpdoc-trans-0.0.5/setup.py
```

### Comparing `phpdoc-trans-0.0.4/LICENSE` & `phpdoc-trans-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.4/PKG-INFO` & `phpdoc-trans-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdoc-trans
-Version: 0.0.4
+Version: 0.0.5
 Summary: PHP doc transaction tool
 Home-page: https://github.com/AtlanticF/phpdoc-openai-trans
 Author: meifeng.song
 Author-email: atlanticfeng@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phpdoc-trans-0.0.4/README.md` & `phpdoc-trans-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.4/phpdoc_trans/main.py` & `phpdoc-trans-0.0.5/phpdoc_trans/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 @click.command()
 @click.argument('doc', type=click.File('rb'))
 @click.option('--lang', default='zh', help='Language to translate')
 @click.option('--model', default='text-davinci-003', help='Model ID')
 @click.option('--max-tokens', default=100, help='Maximum number of tokens to generate')
 @click.option('--temperature', default=0.3, help='Sampling temperature')
+@click.version_option()
 def main(doc, lang, model, max_tokens, temperature):
     '''Load phpdoc file and translate it.'''
     # check api key
     api_key = os.getenv("OPENAI_API_KEY")
     if api_key is None:
         click.echo(
             "No API key provided. You can set the environment variable OPENAI_API_KEY=<API-KEY>")
```

### Comparing `phpdoc-trans-0.0.4/phpdoc_trans/spinner.py` & `phpdoc-trans-0.0.5/phpdoc_trans/spinner.py`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.4/phpdoc_trans.egg-info/PKG-INFO` & `phpdoc-trans-0.0.5/phpdoc_trans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdoc-trans
-Version: 0.0.4
+Version: 0.0.5
 Summary: PHP doc transaction tool
 Home-page: https://github.com/AtlanticF/phpdoc-openai-trans
 Author: meifeng.song
 Author-email: atlanticfeng@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phpdoc-trans-0.0.4/setup.py` & `phpdoc-trans-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", encoding="utf8") as f_r:
         _long_description = f_r.read()
 except FileNotFoundError:
     _long_description = ""
 
 setup(
     name='phpdoc-trans',
-    version='0.0.4',
+    version='0.0.5',
     packages=['phpdoc_trans'],
     install_requires=[
         'click',
         'openai',
         'bs4',
         'progress'
     ],
```

