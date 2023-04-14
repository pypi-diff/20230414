# Comparing `tmp/compel-1.1.3.tar.gz` & `tmp/compel-1.1.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-_t77dw_k/compel-1.1.3.tar", last modified: Fri Apr 14 11:42:27 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-emvysva3/compel-1.1.3.dev0.tar", last modified: Fri Apr 14 08:44:46 2023, max compression
```

## Comparing `compel-1.1.3.tar` & `compel-1.1.3.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 11:42:27.000000 compel-1.1.3/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.3/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     6978 2023-04-14 11:42:27.000000 compel-1.1.3/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6400 2023-04-14 11:42:09.000000 compel-1.1.3/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-14 11:42:09.000000 compel-1.1.3/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 11:42:27.000000 compel-1.1.3/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 11:42:27.000000 compel-1.1.3/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.3/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14494 2023-04-14 11:42:09.000000 compel-1.1.3/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.3/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.3/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    24862 2023-04-14 11:42:09.000000 compel-1.1.3/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-14 08:42:01.000000 compel-1.1.3/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     6978 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 11:42:27.000000 compel-1.1.3/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 11:42:27.000000 compel-1.1.3/test/
--rw-r--r--   0 damian     (501) staff       (20)    14454 2023-04-14 11:42:09.000000 compel-1.1.3/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-14 11:42:09.000000 compel-1.1.3/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-14 08:42:01.000000 compel-1.1.3/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6400 2023-04-14 08:44:28.000000 compel-1.1.3.dev0/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-04-14 08:42:50.000000 compel-1.1.3.dev0/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.3.dev0/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14494 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.3.dev0/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    24862 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/test/
+-rw-r--r--   0 damian     (501) staff       (20)    14454 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/test/test_prompt_parser.py
```

### Comparing `compel-1.1.3/LICENSE` & `compel-1.1.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/PKG-INFO` & `compel-1.1.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.3
+Version: 1.1.3.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `compel-1.1.3/README.md` & `compel-1.1.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/pyproject.toml` & `compel-1.1.3.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.3"
+version = "1.1.3.dev0"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.3/src/compel/compel.py` & `compel-1.1.3.dev0/src/compel/compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/src/compel/conditioning_scheduler.py` & `compel-1.1.3.dev0/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/src/compel/cross_attention_control.py` & `compel-1.1.3.dev0/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/src/compel/embeddings_provider.py` & `compel-1.1.3.dev0/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/src/compel/prompt_parser.py` & `compel-1.1.3.dev0/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/src/compel.egg-info/PKG-INFO` & `compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.3
+Version: 1.1.3.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `compel-1.1.3/test/test_compel.py` & `compel-1.1.3.dev0/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/test/test_embeddings_provider.py` & `compel-1.1.3.dev0/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3/test/test_prompt_parser.py` & `compel-1.1.3.dev0/test/test_prompt_parser.py`

 * *Files identical despite different names*

