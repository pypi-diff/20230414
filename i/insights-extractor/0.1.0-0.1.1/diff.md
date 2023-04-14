# Comparing `tmp/insights-extractor-0.1.0.tar.gz` & `tmp/insights-extractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insights-extractor-0.1.0.tar", last modified: Fri Apr 14 03:57:25 2023, max compression
+gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-pq31s1ul/insights-extractor-0.1.1.tar", last modified: Fri Apr 14 04:09:28 2023, max compression
```

## Comparing `insights-extractor-0.1.0.tar` & `insights-extractor-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.802265 insights-extractor-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.765231 insights-extractor-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.773239 insights-extractor-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     1125 2023-04-14 03:47:48.000000 insights-extractor-0.1.0/.github/workflows/python-publish.yml
--rw-rw-rw-   0        0        0      116 2023-04-14 03:01:18.000000 insights-extractor-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1091 2023-04-11 15:46:05.000000 insights-extractor-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3931 2023-04-14 03:57:25.802265 insights-extractor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3071 2023-04-13 23:25:38.000000 insights-extractor-0.1.0/README.md
--rw-rw-rw-   0        0        0     1251 2023-04-14 03:57:10.000000 insights-extractor-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 03:57:25.802265 insights-extractor-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.769235 insights-extractor-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.773239 insights-extractor-0.1.0/src/extractlib/
--rw-rw-rw-   0        0        0        0 2023-04-13 13:38:44.000000 insights-extractor-0.1.0/src/extractlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.775241 insights-extractor-0.1.0/src/extractlib/classification/
--rw-rw-rw-   0        0        0        0 2023-04-07 20:06:52.000000 insights-extractor-0.1.0/src/extractlib/classification/__init__.py
--rw-rw-rw-   0        0        0     2285 2023-04-11 18:22:01.000000 insights-extractor-0.1.0/src/extractlib/classification/prep_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.776242 insights-extractor-0.1.0/src/extractlib/classification/utils/
--rw-rw-rw-   0        0        0        0 2023-04-07 20:06:52.000000 insights-extractor-0.1.0/src/extractlib/classification/utils/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-04-11 18:23:26.000000 insights-extractor-0.1.0/src/extractlib/classification/utils/keywords.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.780244 insights-extractor-0.1.0/src/extractlib/document/
--rw-rw-rw-   0        0        0        0 2023-04-07 20:06:52.000000 insights-extractor-0.1.0/src/extractlib/document/__init__.py
--rw-rw-rw-   0        0        0     5127 2023-04-13 21:08:56.000000 insights-extractor-0.1.0/src/extractlib/document/page.py
--rw-rw-rw-   0        0        0     5887 2023-04-13 14:05:03.000000 insights-extractor-0.1.0/src/extractlib/document/process.py
--rw-rw-rw-   0        0        0     4999 2023-04-13 23:12:05.000000 insights-extractor-0.1.0/src/extractlib/document/table.py
--rw-rw-rw-   0        0        0     2136 2023-04-11 18:23:41.000000 insights-extractor-0.1.0/src/extractlib/document/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.780244 insights-extractor-0.1.0/src/extractlib/exceptions/
--rw-rw-rw-   0        0        0      102 2023-04-11 17:20:15.000000 insights-extractor-0.1.0/src/extractlib/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.782247 insights-extractor-0.1.0/src/extractlib/models/
--rw-rw-rw-   0        0        0        0 2023-04-08 04:47:51.000000 insights-extractor-0.1.0/src/extractlib/models/__init__.py
--rw-rw-rw-   0        0        0      446 2023-04-13 21:26:35.000000 insights-extractor-0.1.0/src/extractlib/models/table.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.782247 insights-extractor-0.1.0/src/extractlib/ner/
--rw-rw-rw-   0        0        0      955 2023-04-10 14:39:05.000000 insights-extractor-0.1.0/src/extractlib/ner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.785249 insights-extractor-0.1.0/src/extractlib/nlp/
--rw-rw-rw-   0        0        0       67 2023-04-06 20:39:10.000000 insights-extractor-0.1.0/src/extractlib/nlp/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-04-07 21:26:58.000000 insights-extractor-0.1.0/src/extractlib/nlp/pre_process.py
--rw-rw-rw-   0        0        0      496 2023-04-07 20:09:22.000000 insights-extractor-0.1.0/src/extractlib/nlp/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.786250 insights-extractor-0.1.0/src/extractlib/settings/
--rw-rw-rw-   0        0        0      328 2023-04-13 23:17:45.000000 insights-extractor-0.1.0/src/extractlib/settings/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-04-13 14:13:37.000000 insights-extractor-0.1.0/src/extractlib/settings/config.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.788252 insights-extractor-0.1.0/src/extractlib/utils/
--rw-rw-rw-   0        0        0     4025 2023-04-11 18:26:52.000000 insights-extractor-0.1.0/src/extractlib/utils/json_utils.py
--rw-rw-rw-   0        0        0      418 2023-03-13 23:47:28.000000 insights-extractor-0.1.0/src/extractlib/utils/temp_dir.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.800263 insights-extractor-0.1.0/src/insights_extractor.egg-info/
--rw-rw-rw-   0        0        0     3931 2023-04-14 03:57:25.000000 insights-extractor-0.1.0/src/insights_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-04-14 03:57:25.000000 insights-extractor-0.1.0/src/insights_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 03:57:25.000000 insights-extractor-0.1.0/src/insights_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-14 03:57:25.000000 insights-extractor-0.1.0/src/insights_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 03:57:25.000000 insights-extractor-0.1.0/src/insights_extractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 03:57:25.801264 insights-extractor-0.1.0/src/requirements/
--rw-rw-rw-   0        0        0       91 2023-04-11 18:48:22.000000 insights-extractor-0.1.0/src/requirements/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/dist/insights-extractor-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/dist/insights_extractor-0.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/prep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/stopwords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/settings/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/utils/temp_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/requirements/requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `insights-extractor-0.1.0/LICENSE` & `insights-extractor-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `insights-extractor-0.1.0/PKG-INFO` & `insights-extractor-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,115 @@
-Metadata-Version: 2.1
-Name: insights-extractor
-Version: 0.1.0
-Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
-Author-email: Trae Moore <trae.dev@gmail.com>
-Project-URL: Homepage, https://github.com/traemoore/insightextractor
-Project-URL: Tests, https://github.com/traemoore/insightextractor-test
-Project-URL: Bug Tracker, https://github.com/traemoore/insightextractor/issues
-Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Extractlib
-
-This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
-
-
-## python dependency overview
-### Python Dependency Install
-<pre>pip install nltk==3.8.1 PyMuPDF==1.21.1 camelot-py==0.11.0 opencv-python==4.7.0.72 ghostscript==0.7</pre>
-
-## manually install supporting binaries
-
-### camelot dependencies
-- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
-
-#### Ubuntu
-<pre>$ apt install ghostscript python3-tk</pre>
-
-#### MacOS
-<pre>$ brew install ghostscript tcl-tk</pre>
-
-## windows dependency installations
-- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
-- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
- 
-# Configuration
-- configuration file should be placed in the root of the project and named 'extractlib.config.json'
-
-## Example 'extractlib.config.json' File
-### this file should be located in the root of your project
-<pre>
-{
-  "std_out_logging": true,
-  "supported_file_types": [".pdf"],
-  "invalid_content_regexs": ["X{2,}"],
-  "stop_words": [
-    "na",
-    "dependent",
-    "address",
-    "plans",
-    "network",
-    "nonnetwork",
-    "additional",
-    "covered"
-  ],
-  "keywords": {
-    "dental": 5,
-    "vision": 5,    
-    "life": 5,
-    "disability": 5
-  },
-  "keyword_synonyms": {
-    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
-    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
-    "life": [
-      "accident",
-      "critical",
-      "illness",
-      "accidental",
-      "dismember",
-      "AD&D"
-    ],
-    "disability": []
-  },
-  "word_min_length": 3
-}
-</pre>
-
-# access config variables
-<pre>
-from extractlib.settings import config
-
-print(json.dump(config.config_raw, indent=4))
-</pre>
-# Example implementation
-<pre>
-from extractlib.document.process import process_document
-import json
-
-def main(file: str):
-    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
-    # Save the HTML content to a temporary file
-    with open('temp.json', 'w') as f:
-        json.dump(result, f, indent=4)
-
-
-if __name__ == '__main__':
-
-    # get working directory
-    import os
-    target_dir = os.path.dirname(os.path.abspath(__file__))
-    main(f'{target_dir}/_testdata/PDF.pdf')
-</pre>
+Metadata-Version: 2.1
+Name: insights-extractor
+Version: 0.1.1
+Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
+Author-email: Trae Moore <trae.dev@gmail.com>
+Project-URL: Homepage, https://github.com/traemoore/insights-extractor
+Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
+Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
+Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Extractlib
+
+This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
+
+
+## Dependency Overview
+### Python Dependency Install
+This project leverages packages 
+<pre>
+nltk == 3.8.1 
+PyMuPDF == 1.21.1 
+camelot-py == 0.11.0 
+opencv-python == 4.7.0.72 
+ghostscript == 0.7
+</pre>
+
+## manually install supporting binaries
+
+### camelot dependencies
+- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
+
+#### Ubuntu
+<pre>$ apt install ghostscript python3-tk</pre>
+
+#### MacOS
+<pre>$ brew install ghostscript tcl-tk</pre>
+
+## windows dependency installations
+- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
+- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
+ 
+# Configuration
+- configuration file should be placed in the root of the project and named 'extractlib.config.json'
+
+## Example 'extractlib.config.json' File
+### this file should be located in the root of your project
+<pre>
+{
+  "std_out_logging": true,
+  "supported_file_types": [".pdf"],
+  "invalid_content_regexs": ["X{2,}"],
+  "stop_words": [
+    "na",
+    "dependent",
+    "address",
+    "plans",
+    "network",
+    "nonnetwork",
+    "additional",
+    "covered"
+  ],
+  "keywords": {
+    "dental": 5,
+    "vision": 5,    
+    "life": 5,
+    "disability": 5
+  },
+  "keyword_synonyms": {
+    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
+    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
+    "life": [
+      "accident",
+      "critical",
+      "illness",
+      "accidental",
+      "dismember",
+      "AD&D"
+    ],
+    "disability": []
+  },
+  "word_min_length": 3
+}
+</pre>
+
+# access config variables
+<pre>
+from extractlib.settings import config
+
+print(json.dump(config.config_raw, indent=4))
+</pre>
+# Example implementation
+<pre>
+from extractlib.document.process import process_document
+import json
+
+def main(file: str):
+    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
+    # Save the HTML content to a temporary file
+    with open('temp.json', 'w') as f:
+        json.dump(result, f, indent=4)
+
+
+if __name__ == '__main__':
+
+    # get working directory
+    import os
+    target_dir = os.path.dirname(os.path.abspath(__file__))
+    main(f'{target_dir}/_testdata/PDF.pdf')
+</pre>
```

### Comparing `insights-extractor-0.1.0/README.md` & `insights-extractor-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,99 @@
-# Extractlib
-
-This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
-
-
-## python dependency overview
-### Python Dependency Install
-<pre>pip install nltk==3.8.1 PyMuPDF==1.21.1 camelot-py==0.11.0 opencv-python==4.7.0.72 ghostscript==0.7</pre>
-
-## manually install supporting binaries
-
-### camelot dependencies
-- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
-
-#### Ubuntu
-<pre>$ apt install ghostscript python3-tk</pre>
-
-#### MacOS
-<pre>$ brew install ghostscript tcl-tk</pre>
-
-## windows dependency installations
-- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
-- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
- 
-# Configuration
-- configuration file should be placed in the root of the project and named 'extractlib.config.json'
-
-## Example 'extractlib.config.json' File
-### this file should be located in the root of your project
-<pre>
-{
-  "std_out_logging": true,
-  "supported_file_types": [".pdf"],
-  "invalid_content_regexs": ["X{2,}"],
-  "stop_words": [
-    "na",
-    "dependent",
-    "address",
-    "plans",
-    "network",
-    "nonnetwork",
-    "additional",
-    "covered"
-  ],
-  "keywords": {
-    "dental": 5,
-    "vision": 5,    
-    "life": 5,
-    "disability": 5
-  },
-  "keyword_synonyms": {
-    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
-    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
-    "life": [
-      "accident",
-      "critical",
-      "illness",
-      "accidental",
-      "dismember",
-      "AD&D"
-    ],
-    "disability": []
-  },
-  "word_min_length": 3
-}
-</pre>
-
-# access config variables
-<pre>
-from extractlib.settings import config
-
-print(json.dump(config.config_raw, indent=4))
-</pre>
-# Example implementation
-<pre>
-from extractlib.document.process import process_document
-import json
-
-def main(file: str):
-    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
-    # Save the HTML content to a temporary file
-    with open('temp.json', 'w') as f:
-        json.dump(result, f, indent=4)
-
-
-if __name__ == '__main__':
-
-    # get working directory
-    import os
-    target_dir = os.path.dirname(os.path.abspath(__file__))
-    main(f'{target_dir}/_testdata/PDF.pdf')
+# Extractlib
+
+This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
+
+
+## Dependency Overview
+### Python Dependency Install
+This project leverages packages 
+<pre>
+nltk == 3.8.1 
+PyMuPDF == 1.21.1 
+camelot-py == 0.11.0 
+opencv-python == 4.7.0.72 
+ghostscript == 0.7
+</pre>
+
+## manually install supporting binaries
+
+### camelot dependencies
+- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
+
+#### Ubuntu
+<pre>$ apt install ghostscript python3-tk</pre>
+
+#### MacOS
+<pre>$ brew install ghostscript tcl-tk</pre>
+
+## windows dependency installations
+- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
+- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
+ 
+# Configuration
+- configuration file should be placed in the root of the project and named 'extractlib.config.json'
+
+## Example 'extractlib.config.json' File
+### this file should be located in the root of your project
+<pre>
+{
+  "std_out_logging": true,
+  "supported_file_types": [".pdf"],
+  "invalid_content_regexs": ["X{2,}"],
+  "stop_words": [
+    "na",
+    "dependent",
+    "address",
+    "plans",
+    "network",
+    "nonnetwork",
+    "additional",
+    "covered"
+  ],
+  "keywords": {
+    "dental": 5,
+    "vision": 5,    
+    "life": 5,
+    "disability": 5
+  },
+  "keyword_synonyms": {
+    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
+    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
+    "life": [
+      "accident",
+      "critical",
+      "illness",
+      "accidental",
+      "dismember",
+      "AD&D"
+    ],
+    "disability": []
+  },
+  "word_min_length": 3
+}
+</pre>
+
+# access config variables
+<pre>
+from extractlib.settings import config
+
+print(json.dump(config.config_raw, indent=4))
+</pre>
+# Example implementation
+<pre>
+from extractlib.document.process import process_document
+import json
+
+def main(file: str):
+    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
+    # Save the HTML content to a temporary file
+    with open('temp.json', 'w') as f:
+        json.dump(result, f, indent=4)
+
+
+if __name__ == '__main__':
+
+    # get working directory
+    import os
+    target_dir = os.path.dirname(os.path.abspath(__file__))
+    main(f'{target_dir}/_testdata/PDF.pdf')
 </pre>
```

### Comparing `insights-extractor-0.1.0/pyproject.toml` & `insights-extractor-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[project]
-dependencies = [
-  "nltk == 3.8.1; python_version >= '3.7'",
-  "PyMuPDF == 1.21.1; python_version >= '3.7'",
-  "camelot-py == 0.11.0; python_version >= '3.6'",
-  "opencv-python == 4.7.0.72; python_version >= '3.6'",
-  "ghostscript == 0.7; python_version >= '3.6'"
-]
-name = "insights-extractor"
-version = "0.1.0"
-authors = [
-  { name="Trae Moore", email="trae.dev@gmail.com" },
-]
-description = "Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities."
-readme = "README.md"
-requires-python = ">=3.7"
-keywords = ["nltk", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/traemoore/insightextractor"
-"Tests" =  "https://github.com/traemoore/insightextractor-test"
-"Bug Tracker" = "https://github.com/traemoore/insightextractor/issues"
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[project]
+dependencies = [
+  "nltk == 3.8.1; python_version >= '3.7'",
+  "PyMuPDF == 1.21.1; python_version >= '3.7'",
+  "camelot-py == 0.11.0; python_version >= '3.6'",
+  "opencv-python == 4.7.0.72; python_version >= '3.6'",
+  "ghostscript == 0.7; python_version >= '3.6'"
+]
+name = "insights-extractor"
+version = "0.1.1"
+authors = [
+  { name="Trae Moore", email="trae.dev@gmail.com" },
+]
+description = "Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities."
+readme = "README.md"
+requires-python = ">=3.7"
+keywords = ["nltk", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/traemoore/insights-extractor"
+"Tests" =  "https://github.com/traemoore/insights-extractor-test"
+"Bug Tracker" = "https://github.com/traemoore/insights-extractor/issues"
```

### Comparing `insights-extractor-0.1.0/src/extractlib/classification/prep_utils.py` & `insights-extractor-0.1.1/src/extractlib/classification/prep_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import re
-import string
-from collections import Counter
-from nltk.tokenize import word_tokenize
-from ..nlp.stopwords import get_words
-
-from settings import config
-
-def calculate_keyword_frequencies(content, keywords={}, keyword_synonyms={} , regex_list=[], stop_words=[]):
-    """
-    Calculate the frequency of occurrence for each keyword in the given content.
-
-    Args:
-        content (str): The text content to analyze.
-        keywords (dict): A dictionary containing the keywords to search for and their corresponding weights (default={}).
-        keyword_synonyms (dict): A dictionary containing synonyms for each keyword (default={}).
-        regex_list (list): A list of regular expressions to remove from the content (default=[]).
-        stop_words (list): A list of stop words to remove from the content (default=[]).
-
-    Returns:
-        list: A list of tuples containing the keyword and its frequency of occurrence in the content, sorted by frequency in descending order.
-    """
-    try:
-        keywords.update(config.keywords) 
-        stop_words.extend(list(set(get_words(config.stop_words))))
-        
-        for regex in regex_list:
-            content = re.sub(regex, '', content)
-
-        # Remove punctuation
-        content = content.translate(str.maketrans('', '', string.punctuation))
-
-        # Tokenize the data column into words
-        words = word_tokenize(content)
-        words = [word for word in words if word.lower() not in stop_words]
-        
-        # Count the frequency of each word
-        word_counts = Counter(words)
-
-        # Apply classification keyword weights
-        results = {}
-        for word, freq in word_counts.items():
-            if len(word) <= config.min_word_length:
-                continue
-
-            for keyword, synonyms in keyword_synonyms.items():
-                if word in synonyms:
-                    results[keyword] = freq * keywords[keyword]
-                else:
-                    results[word] = freq * keywords[word] if word in keywords else freq
-
-        sorted_results = sorted(results.items(), key=lambda x: x[1], reverse=True)
-
-        return sorted_results
-    except Exception as e:
-        print(f'Error processing: {e}')
+import re
+import string
+from collections import Counter
+from nltk.tokenize import word_tokenize
+from ..nlp.stopwords import get_words
+
+from settings import config
+
+def calculate_keyword_frequencies(content, keywords={}, keyword_synonyms={} , regex_list=[], stop_words=[]):
+    """
+    Calculate the frequency of occurrence for each keyword in the given content.
+
+    Args:
+        content (str): The text content to analyze.
+        keywords (dict): A dictionary containing the keywords to search for and their corresponding weights (default={}).
+        keyword_synonyms (dict): A dictionary containing synonyms for each keyword (default={}).
+        regex_list (list): A list of regular expressions to remove from the content (default=[]).
+        stop_words (list): A list of stop words to remove from the content (default=[]).
+
+    Returns:
+        list: A list of tuples containing the keyword and its frequency of occurrence in the content, sorted by frequency in descending order.
+    """
+    try:
+        keywords.update(config.keywords) 
+        stop_words.extend(list(set(get_words(config.stop_words))))
+        
+        for regex in regex_list:
+            content = re.sub(regex, '', content)
+
+        # Remove punctuation
+        content = content.translate(str.maketrans('', '', string.punctuation))
+
+        # Tokenize the data column into words
+        words = word_tokenize(content)
+        words = [word for word in words if word.lower() not in stop_words]
+        
+        # Count the frequency of each word
+        word_counts = Counter(words)
+
+        # Apply classification keyword weights
+        results = {}
+        for word, freq in word_counts.items():
+            if len(word) <= config.min_word_length:
+                continue
+
+            for keyword, synonyms in keyword_synonyms.items():
+                if word in synonyms:
+                    results[keyword] = freq * keywords[keyword]
+                else:
+                    results[word] = freq * keywords[word] if word in keywords else freq
+
+        sorted_results = sorted(results.items(), key=lambda x: x[1], reverse=True)
+
+        return sorted_results
+    except Exception as e:
+        print(f'Error processing: {e}')
         raise e
```

### Comparing `insights-extractor-0.1.0/src/extractlib/document/page.py` & `insights-extractor-0.1.1/src/extractlib/document/page.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import camelot
-import fitz
-import base64
-
-def get_images(filename):
-    """
-    Extract images from a PDF page.
-
-    Args:
-        filename (str): The path to the PDF file.
-
-    Returns:
-        list: A list of dictionaries containing the extracted images.
-    """
-
-    images_json = []
-
-    # Open the PDF document
-    with fitz.open(filename) as doc:
-        page = doc[0]
-        image_info_list = page.get_image_info()
-        images = page.get_images(full=True)
-
-        # Iterate through the extracted images and their rectangles
-        for i, image in enumerate(images):
-            target_image = None
-            
-            target_image = image_info_list[i]
-            # target_image = [img for img in image_info_list if img['cs-name'] == image[5]][0]
-
-            # Get the image binary data
-            img_base64 = doc.extract_image(image[0])['image']
-
-            # Convert the image binary data to a base64 encoded string
-            img_base64_str = base64.b64encode(img_base64).decode('utf-8')
-
-            # Create a dictionary containing the image metadata
-            image_data = {
-                "xref": image[0],
-                "width": target_image['width'],
-                "height": target_image['height'],
-                "colorspace": target_image['colorspace'],
-                "bpc": target_image['bpc'],
-                "image": img_base64_str,
-                "bbox": target_image['bbox'],
-                "transform": target_image['transform'],
-            }
-
-            # Add the image metadata dictionary to the images_json list
-            images_json.append(image_data)
-    return images_json
-
-def extract_tables(file):
-    """
-    Extract tables from a PDF file using Camelot.
-    
-    Returns: a list of camelot.core.TableList objects
-    """
-    tables = camelot.read_pdf(file, flavor='lattice', pages='1')
-    return tables
-
-
-def extract_lines(filename, tables):
-    """
-    Extract lines of text from a PDF page and remove lines contained in tables.
-
-    Args:
-        filename (str): The path to the PDF file.
-        tables (list): A list of table objects representing tables on the page.
-
-    Returns:
-        list: A list of dictionaries containing the extracted lines.
-    """
-
-    # Create an empty list to store the extracted lines
-    page_lines = []
-
-    # Open the PDF document
-    with fitz.open(filename) as doc:
-        # Get the first page of the document
-        page = doc[0]
-
-        # Get the page height and width
-        page_height = page.mediabox.height
-        page_width = page.mediabox.width
-        
-        # Get the text blocks on the page
-        blocks = page.get_text('dict')
-        
-        # collect all lines into a set
-        table_lines = []
-
-        # Remove lines contained in tables
-        for block in blocks['blocks']:
-            if 'lines' in block:
-                for line in block['lines']:
-                    # Get the bounding box for the line
-                    x1, y1, x2, y2 = line['bbox']
-
-                    # Normalize the line bounding box to the page
-                    line['bbox'] = (x1, page_height-y2, x2, page_height-y1)
-
-                    table_idx = _in_table(line, tables)
-                    # Check if the line is contained in a table
-                    collection = page_lines if not table_idx else table_lines
-                    
-                    data = {
-                        'text': line['spans'][0]['text'],
-                        'valid': True,
-                        'bbox': line['bbox'],
-                        'font': {
-                            'size': line['spans'][0]['size'],
-                            'family': line['spans'][0]['font'],
-                            'color': line['spans'][0]['color']
-                        },
-                    }
-                    
-                    # Add the table index to the line if it is contained in a table
-                    if table_idx:
-                        data['table'] = table_idx - 1
-
-                    # Add the line to the list of extracted lines
-                    collection.append(data)
-
-    
-
-    # Sort the lines by y-coordinate and then x-coordinate
-    sorted_page_elements = sorted(page_lines, key=lambda line: (-line['bbox'][3], line['bbox'][0]))
-    # Sort the table_lines by y-coordinate (top to bottom) and then x-coordinate (left to right)
-    #sorted_table_lines = sorted(table_lines, key=lambda line: (-line['bbox'][1], line['bbox'][0]))
-
-    # Return the sorted lines
-    return sorted_page_elements, table_lines
-
-
-def _in_table(line, tables):
-    """
-    Check if a line is contained in a table.
-
-    Args:
-        line (dict): A dictionary containing the line data.
-        tables (list): A list of table objects representing tables on the page.
-
-    Returns:
-        bool: True if the line is contained in a table, False otherwise.
-    """
-    for table in tables:
-        if table.contains(line):
-            return table.order
+import camelot
+import fitz
+import base64
+
+def get_images(filename):
+    """
+    Extract images from a PDF page.
+
+    Args:
+        filename (str): The path to the PDF file.
+
+    Returns:
+        list: A list of dictionaries containing the extracted images.
+    """
+
+    images_json = []
+
+    # Open the PDF document
+    with fitz.open(filename) as doc:
+        page = doc[0]
+        image_info_list = page.get_image_info()
+        images = page.get_images(full=True)
+
+        # Iterate through the extracted images and their rectangles
+        for i, image in enumerate(images):
+            target_image = None
+            
+            target_image = image_info_list[i]
+            # target_image = [img for img in image_info_list if img['cs-name'] == image[5]][0]
+
+            # Get the image binary data
+            img_base64 = doc.extract_image(image[0])['image']
+
+            # Convert the image binary data to a base64 encoded string
+            img_base64_str = base64.b64encode(img_base64).decode('utf-8')
+
+            # Create a dictionary containing the image metadata
+            image_data = {
+                "xref": image[0],
+                "width": target_image['width'],
+                "height": target_image['height'],
+                "colorspace": target_image['colorspace'],
+                "bpc": target_image['bpc'],
+                "image": img_base64_str,
+                "bbox": target_image['bbox'],
+                "transform": target_image['transform'],
+            }
+
+            # Add the image metadata dictionary to the images_json list
+            images_json.append(image_data)
+    return images_json
+
+def extract_tables(file):
+    """
+    Extract tables from a PDF file using Camelot.
+    
+    Returns: a list of camelot.core.TableList objects
+    """
+    tables = camelot.read_pdf(file, flavor='lattice', pages='1')
+    return tables
+
+
+def extract_lines(filename, tables):
+    """
+    Extract lines of text from a PDF page and remove lines contained in tables.
+
+    Args:
+        filename (str): The path to the PDF file.
+        tables (list): A list of table objects representing tables on the page.
+
+    Returns:
+        list: A list of dictionaries containing the extracted lines.
+    """
+
+    # Create an empty list to store the extracted lines
+    page_lines = []
+
+    # Open the PDF document
+    with fitz.open(filename) as doc:
+        # Get the first page of the document
+        page = doc[0]
+
+        # Get the page height and width
+        page_height = page.mediabox.height
+        page_width = page.mediabox.width
+        
+        # Get the text blocks on the page
+        blocks = page.get_text('dict')
+        
+        # collect all lines into a set
+        table_lines = []
+
+        # Remove lines contained in tables
+        for block in blocks['blocks']:
+            if 'lines' in block:
+                for line in block['lines']:
+                    # Get the bounding box for the line
+                    x1, y1, x2, y2 = line['bbox']
+
+                    # Normalize the line bounding box to the page
+                    line['bbox'] = (x1, page_height-y2, x2, page_height-y1)
+
+                    table_idx = _in_table(line, tables)
+                    # Check if the line is contained in a table
+                    collection = page_lines if not table_idx else table_lines
+                    
+                    data = {
+                        'text': line['spans'][0]['text'],
+                        'valid': True,
+                        'bbox': line['bbox'],
+                        'font': {
+                            'size': line['spans'][0]['size'],
+                            'family': line['spans'][0]['font'],
+                            'color': line['spans'][0]['color']
+                        },
+                    }
+                    
+                    # Add the table index to the line if it is contained in a table
+                    if table_idx:
+                        data['table'] = table_idx - 1
+
+                    # Add the line to the list of extracted lines
+                    collection.append(data)
+
+    
+
+    # Sort the lines by y-coordinate and then x-coordinate
+    sorted_page_elements = sorted(page_lines, key=lambda line: (-line['bbox'][3], line['bbox'][0]))
+    # Sort the table_lines by y-coordinate (top to bottom) and then x-coordinate (left to right)
+    #sorted_table_lines = sorted(table_lines, key=lambda line: (-line['bbox'][1], line['bbox'][0]))
+
+    # Return the sorted lines
+    return sorted_page_elements, table_lines
+
+
+def _in_table(line, tables):
+    """
+    Check if a line is contained in a table.
+
+    Args:
+        line (dict): A dictionary containing the line data.
+        tables (list): A list of table objects representing tables on the page.
+
+    Returns:
+        bool: True if the line is contained in a table, False otherwise.
+    """
+    for table in tables:
+        if table.contains(line):
+            return table.order
     return None
```

### Comparing `insights-extractor-0.1.0/src/extractlib/document/process.py` & `insights-extractor-0.1.1/src/extractlib/document/process.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import json
-import shutil
-import os
-from concurrent.futures import ThreadPoolExecutor
-
-from .utils import split_document_pages
-from .page import extract_lines, extract_tables, get_images
-from .table import corrilate_table_data, get_table_data
-from .utils import split_document_pages
-from ..models.table import Table
-from ..settings import config
-from ..utils.json_utils import cleanse_and_tag_json_structure
-from ..exceptions import DocumentProcessingError, PageProcessingError
-
-
-def process_document(file: str, exclude_pages=None, use_multithreading=False,  split_pages_output_dir=None, delete_split_pages=True):
-    """
-    Process a document by splitting it into pages and processing each page individually.
-
-    Args:
-        file (str): The path to the input document file.
-        pages (list): A list of page numbers to exclude (non-zero based index). If None, all pages are processed (default=None).
-        use_multithreading (bool): Whether to use multi-threading to process the pages (default=False).
-        split_pages_output_dir (str): The path to the directory where extracted pages should be saved (default=None).
-        delete_split_pages (bool): Whether to delete the split pages after processing (default=True).
-
-    Returns:
-        dict: A dictionary containing the processed data for each page. The dictionary has the following keys:
-            - 'pages': A list of dictionaries containing the processed data for each page. Each dictionary has the following keys:
-                - 'page': An integer identifying the page number.
-                - 'content': A dictionary containing the extracted content for the page.
-
-    Raises: DocumentProcessingError if an error occurs while processing the document.
-    """
-    result = {
-        'document_name': os.path.basename(file),
-        'excluded_pages': exclude_pages if exclude_pages is not None else None,
-        'pages': []
-    }
-
-    try:
-        # Split the input document into individual pages
-        target_dir, files = split_document_pages(
-            file, split_pages_output_dir)
-    except Exception as e:
-        raise DocumentProcessingError(f'Error processing document {file}: {e}')
-    
-    # Process each page in the document
-    if use_multithreading:
-        # If multi-threading is enabled, process each page in a separate thread
-        with ThreadPoolExecutor() as executor:
-            futures = []
-            for i, file_path in enumerate(files):
-                if exclude_pages is None or i+1 not in exclude_pages:
-                    futures.append(executor.submit(
-                        process_page, file_path, i+1))
-
-            # Wait for all threads to complete and collect the results
-            for future in futures:
-                result['pages'].append(future.result())
-        
-            # Sort the pages list by page number
-        result['pages'] = sorted(result['pages'], key=lambda x: x['page'])
-    else:
-        # If multi-threading is disabled, process each page sequentially in the main thread
-        for i, file_path in enumerate(files):
-            if exclude_pages is None or i+1 not in exclude_pages:
-                result['pages'].append(process_page(file_path, i+1))
-
-    # Delete the extracted pages if the delete_extracted_pages flag is set
-    if delete_split_pages:
-        shutil.rmtree(target_dir)
-
-    return result
-
-
-def process_page(file_path, index):
-    """
-    Process a PDF page and extract data from tables and lines.
-
-    Args:
-        path (str): The path to the PDF file.
-        index (int): The index of the page to process.
-
-    Raises:
-        PageProcessingError: If an error occurs while processing the page.
-
-    Returns:
-        dict: A dictionary containing the extracted data.
-    """
-
-    # Create an empty dictionary to store the extracted data
-    data = {}
-
-    # Print a message to the console indicating that the processing has started
-    print(f'starting {file_path}')
-
-    file_ext = os.path.splitext(file_path)[1].lower()
-
-    # Check if the file type is supported
-    if file_ext in config.supported_file_types:
-        print(f'processing {file_path}')
-
-        # Create the full file path
-        #file_path = path if not os.path.isabs(path) else os.path.join(os.path.dirname(path), path)
-
-        # Check if the file exists
-        if not os.path.exists(file_path):
-            raise PageProcessingError(f'File {file_path} does not exist')
-
-        try:
-            # Extract tables from the PDF page
-            raw_tables = extract_tables(file_path)
-                        # Extract data from the tables
-            tables = get_table_data(raw_tables)
-
-            # Extract lines from the PDF page
-            lines, table_lines = extract_lines(file_path, [Table(table._bbox, table.order)
-                                  for table in raw_tables])
-
-            tables = corrilate_table_data(table_lines, tables)
-
-            # Cleanse and tag the lines JSON structure
-            cleanse_and_tag_json_structure(lines)
-
-            images = get_images(file_path)
-
-            # Store the extracted data in the dictionary
-            data = {
-                'page': index,
-                'content': {
-                    'sections': lines,  # todo - extract sections
-                    'tables': tables,
-                    'images': images,
-                    # 'classification_training_data': "" #clean_text(training_data, remove_punctuation=True),
-                    # 'kvps': []
-                }
-            }
-
-            return data
-        except Exception as e:
-            # Raise an error if an exception occurs while processing the page
-            raise PageProcessingError(
-                f'Error processing page {index} of {file_path}: {e}')
+import json
+import shutil
+import os
+from concurrent.futures import ThreadPoolExecutor
+
+from .utils import split_document_pages
+from .page import extract_lines, extract_tables, get_images
+from .table import corrilate_table_data, get_table_data
+from .utils import split_document_pages
+from ..models.table import Table
+from ..settings import config
+from ..utils.json_utils import cleanse_and_tag_json_structure
+from ..exceptions import DocumentProcessingError, PageProcessingError
+
+
+def process_document(file: str, exclude_pages=None, use_multithreading=False,  split_pages_output_dir=None, delete_split_pages=True):
+    """
+    Process a document by splitting it into pages and processing each page individually.
+
+    Args:
+        file (str): The path to the input document file.
+        pages (list): A list of page numbers to exclude (non-zero based index). If None, all pages are processed (default=None).
+        use_multithreading (bool): Whether to use multi-threading to process the pages (default=False).
+        split_pages_output_dir (str): The path to the directory where extracted pages should be saved (default=None).
+        delete_split_pages (bool): Whether to delete the split pages after processing (default=True).
+
+    Returns:
+        dict: A dictionary containing the processed data for each page. The dictionary has the following keys:
+            - 'pages': A list of dictionaries containing the processed data for each page. Each dictionary has the following keys:
+                - 'page': An integer identifying the page number.
+                - 'content': A dictionary containing the extracted content for the page.
+
+    Raises: DocumentProcessingError if an error occurs while processing the document.
+    """
+    result = {
+        'document_name': os.path.basename(file),
+        'excluded_pages': exclude_pages if exclude_pages is not None else None,
+        'pages': []
+    }
+
+    try:
+        # Split the input document into individual pages
+        target_dir, files = split_document_pages(
+            file, split_pages_output_dir)
+    except Exception as e:
+        raise DocumentProcessingError(f'Error processing document {file}: {e}')
+    
+    # Process each page in the document
+    if use_multithreading:
+        # If multi-threading is enabled, process each page in a separate thread
+        with ThreadPoolExecutor() as executor:
+            futures = []
+            for i, file_path in enumerate(files):
+                if exclude_pages is None or i+1 not in exclude_pages:
+                    futures.append(executor.submit(
+                        process_page, file_path, i+1))
+
+            # Wait for all threads to complete and collect the results
+            for future in futures:
+                result['pages'].append(future.result())
+        
+            # Sort the pages list by page number
+        result['pages'] = sorted(result['pages'], key=lambda x: x['page'])
+    else:
+        # If multi-threading is disabled, process each page sequentially in the main thread
+        for i, file_path in enumerate(files):
+            if exclude_pages is None or i+1 not in exclude_pages:
+                result['pages'].append(process_page(file_path, i+1))
+
+    # Delete the extracted pages if the delete_extracted_pages flag is set
+    if delete_split_pages:
+        shutil.rmtree(target_dir)
+
+    return result
+
+
+def process_page(file_path, index):
+    """
+    Process a PDF page and extract data from tables and lines.
+
+    Args:
+        path (str): The path to the PDF file.
+        index (int): The index of the page to process.
+
+    Raises:
+        PageProcessingError: If an error occurs while processing the page.
+
+    Returns:
+        dict: A dictionary containing the extracted data.
+    """
+
+    # Create an empty dictionary to store the extracted data
+    data = {}
+
+    # Print a message to the console indicating that the processing has started
+    print(f'starting {file_path}')
+
+    file_ext = os.path.splitext(file_path)[1].lower()
+
+    # Check if the file type is supported
+    if file_ext in config.supported_file_types:
+        print(f'processing {file_path}')
+
+        # Create the full file path
+        #file_path = path if not os.path.isabs(path) else os.path.join(os.path.dirname(path), path)
+
+        # Check if the file exists
+        if not os.path.exists(file_path):
+            raise PageProcessingError(f'File {file_path} does not exist')
+
+        try:
+            # Extract tables from the PDF page
+            raw_tables = extract_tables(file_path)
+                        # Extract data from the tables
+            tables = get_table_data(raw_tables)
+
+            # Extract lines from the PDF page
+            lines, table_lines = extract_lines(file_path, [Table(table._bbox, table.order)
+                                  for table in raw_tables])
+
+            tables = corrilate_table_data(table_lines, tables)
+
+            # Cleanse and tag the lines JSON structure
+            cleanse_and_tag_json_structure(lines)
+
+            images = get_images(file_path)
+
+            # Store the extracted data in the dictionary
+            data = {
+                'page': index,
+                'content': {
+                    'sections': lines,  # todo - extract sections
+                    'tables': tables,
+                    'images': images,
+                    # 'classification_training_data': "" #clean_text(training_data, remove_punctuation=True),
+                    # 'kvps': []
+                }
+            }
+
+            return data
+        except Exception as e:
+            # Raise an error if an exception occurs while processing the page
+            raise PageProcessingError(
+                f'Error processing page {index} of {file_path}: {e}')
```

### Comparing `insights-extractor-0.1.0/src/extractlib/document/table.py` & `insights-extractor-0.1.1/src/extractlib/document/table.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import json
-from ..nlp.pre_process import clean_text
-from ..utils.json_utils import cleanse_and_tag_json_structure, extract_json_values
-
-
-
-def corrilate_table_data(table_elements, table_data):
-    # Initialize an empty dictionary to store tables
-    tables = {}
-    
-    # Iterate through each table in table_data
-    tbl_idx = 0
-    while tbl_idx < len(table_data):
-        table = table_data[tbl_idx]
-
-        # Iterate through each row in the table's JSON data
-        row_idx = 0
-        while row_idx < len(table['json']):
-            row = table['json'][row_idx]
-
-            # Iterate through each column in the row
-            col_idx = 0
-            while col_idx < len(row):
-                col = row[f'{col_idx}']
-                
-                # If the column is empty, increment the column index and continue to the next column
-                if not col:
-                    col_idx += 1
-                    continue
-                
-                ends_column = False
-
-                # Iterate through each line in table_elements
-                line_idx = 0
-                while line_idx < len(table_elements):
-                    line = table_elements[line_idx]
-                    
-                    # If the line text is empty, remove the line and continue to the next line
-                    if not line['text'].strip():
-                        table_elements.pop(line_idx)
-                        continue
-                    
-                    # If the line text is found in the column or _col_contains_line_text returns a positive value
-                    if line['text'] in col or _col_contains_line_text(col, line['text']) > -1:
-                        ends_column = col.endswith(line['text'])
-                        
-                        # Update the line with its row and column information
-                        line.update({'row': row_idx, 'column': col_idx})
-                        
-                        # If the table index is not in the tables dictionary, create a new empty list for the table index
-                        if tbl_idx not in tables:
-                            tables[tbl_idx] = []
-                        
-                        # Remove the line from table_elements and append it to the corresponding table in tables
-                        element = table_elements.pop(line_idx)
-                        del element['table']
-                        tables[tbl_idx].append(element)
-
-                        # If the column ends with the line text, increment the column index and break the loop
-                        if ends_column:
-                            col_idx += 1
-                            break
-                        continue
-                    else:
-                        col_idx += 1
-                        break
-
-            # Increment the row index
-            row_idx += 1
-
-        # If there are no more elements with 'table': 0, increment the table index
-        if not any(element.get('table') == 0 for element in table_elements):
-            tbl_idx += 1
-    
-    # Sort the elements in each table by their row and column values
-    sorted_tables = {key: sorted(tables[key], key=lambda x: (x['row'], x['column'])) for key in tables}
-    
-    # Return the sorted tables if table_elements is empty, otherwise return None
-    return sorted_tables if not any(table_elements) else None
-
-
-def _col_contains_line_text(col, line_text):
-    try:
-        return col.index(line_text.strip())
-    except Exception:
-        return -1
-
-def get_table_data(tables):
-    """
-    Extract and clean data from a list of PyMuPDF table objects.
-
-    Args:
-        tables (list): A list of PyMuPDF table objects to extract data from.
-
-    Returns:
-        list: A list of dictionaries containing cleaned data and metadata for each table.
-            Each dictionary has the following keys:
-            - 'valid': A boolean indicating whether the data is valid or not.
-            - 'table': An integer identifying the table.
-            - 'json': A list of dictionaries containing the raw data extracted from the table.
-            - 'data': A string containing the cleaned data extracted from the table.
-    """
-    result_tables = []
-
-    for idx in range(len(tables)):
-        jsonString = tables[idx].df.to_json(orient='records')
-        jsonData = json.loads(jsonString)
-
-        cleanse_and_tag_json_structure(jsonData)
-        dataValue = extract_json_values(jsonData, [])
-
-        cleaned = clean_text(dataValue, remove_punctuation=True)
-
-        table = {
-            'valid': True,
-            'table': idx,
-            'json': jsonData,
-            'classification_training_data': cleaned
-        }
-
-        result_tables.append(table)
-    return result_tables
-
-def _col_contains_target(col, target):
-    try:
-        return col.index(target)
-    except Exception:
+import json
+from ..nlp.pre_process import clean_text
+from ..utils.json_utils import cleanse_and_tag_json_structure, extract_json_values
+
+
+
+def corrilate_table_data(table_elements, table_data):
+    # Initialize an empty dictionary to store tables
+    tables = {}
+    
+    # Iterate through each table in table_data
+    tbl_idx = 0
+    while tbl_idx < len(table_data):
+        table = table_data[tbl_idx]
+
+        # Iterate through each row in the table's JSON data
+        row_idx = 0
+        while row_idx < len(table['json']):
+            row = table['json'][row_idx]
+
+            # Iterate through each column in the row
+            col_idx = 0
+            while col_idx < len(row):
+                col = row[f'{col_idx}']
+                
+                # If the column is empty, increment the column index and continue to the next column
+                if not col:
+                    col_idx += 1
+                    continue
+                
+                ends_column = False
+
+                # Iterate through each line in table_elements
+                line_idx = 0
+                while line_idx < len(table_elements):
+                    line = table_elements[line_idx]
+                    
+                    # If the line text is empty, remove the line and continue to the next line
+                    if not line['text'].strip():
+                        table_elements.pop(line_idx)
+                        continue
+                    
+                    # If the line text is found in the column or _col_contains_line_text returns a positive value
+                    if line['text'] in col or _col_contains_line_text(col, line['text']) > -1:
+                        ends_column = col.endswith(line['text'])
+                        
+                        # Update the line with its row and column information
+                        line.update({'row': row_idx, 'column': col_idx})
+                        
+                        # If the table index is not in the tables dictionary, create a new empty list for the table index
+                        if tbl_idx not in tables:
+                            tables[tbl_idx] = []
+                        
+                        # Remove the line from table_elements and append it to the corresponding table in tables
+                        element = table_elements.pop(line_idx)
+                        del element['table']
+                        tables[tbl_idx].append(element)
+
+                        # If the column ends with the line text, increment the column index and break the loop
+                        if ends_column:
+                            col_idx += 1
+                            break
+                        continue
+                    else:
+                        col_idx += 1
+                        break
+
+            # Increment the row index
+            row_idx += 1
+
+        # If there are no more elements with 'table': 0, increment the table index
+        if not any(element.get('table') == 0 for element in table_elements):
+            tbl_idx += 1
+    
+    # Sort the elements in each table by their row and column values
+    sorted_tables = {key: sorted(tables[key], key=lambda x: (x['row'], x['column'])) for key in tables}
+    
+    # Return the sorted tables if table_elements is empty, otherwise return None
+    return sorted_tables if not any(table_elements) else None
+
+
+def _col_contains_line_text(col, line_text):
+    try:
+        return col.index(line_text.strip())
+    except Exception:
+        return -1
+
+def get_table_data(tables):
+    """
+    Extract and clean data from a list of PyMuPDF table objects.
+
+    Args:
+        tables (list): A list of PyMuPDF table objects to extract data from.
+
+    Returns:
+        list: A list of dictionaries containing cleaned data and metadata for each table.
+            Each dictionary has the following keys:
+            - 'valid': A boolean indicating whether the data is valid or not.
+            - 'table': An integer identifying the table.
+            - 'json': A list of dictionaries containing the raw data extracted from the table.
+            - 'data': A string containing the cleaned data extracted from the table.
+    """
+    result_tables = []
+
+    for idx in range(len(tables)):
+        jsonString = tables[idx].df.to_json(orient='records')
+        jsonData = json.loads(jsonString)
+
+        cleanse_and_tag_json_structure(jsonData)
+        dataValue = extract_json_values(jsonData, [])
+
+        cleaned = clean_text(dataValue, remove_punctuation=True)
+
+        table = {
+            'valid': True,
+            'table': idx,
+            'json': jsonData,
+            'classification_training_data': cleaned
+        }
+
+        result_tables.append(table)
+    return result_tables
+
+def _col_contains_target(col, target):
+    try:
+        return col.index(target)
+    except Exception:
         return -1
```

### Comparing `insights-extractor-0.1.0/src/extractlib/document/utils.py` & `insights-extractor-0.1.1/src/extractlib/document/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from ..settings import config
-import os
-import fitz
-
-def split_document_pages(doc_path, output_dir=None):
-    """
-    Split a PDF document into individual pages and save each page to a separate PDF file.
-
-    Args:
-        doc_path (str): Path to the input PDF file.
-        output_dir (str): Directory to save the output files (default=None).
-
-    Raises:
-        Exception: If doc_path is a directory instead of a file.
-
-    Returns:
-        tuple: A tuple containing the path to the output directory and a list of the output file paths.
-    """
-
-    # Check if doc_path is a file
-    if os.path.isdir(doc_path):
-        raise Exception('doc_path must be a file, not a directory')
-
-    # Create an empty list to store the output file paths
-    files = []
-
-    # Get the PDF filename without extension
-    pdf_filename = os.path.splitext(os.path.basename(doc_path))[0]
-
-    # Create a directory for the PDF pages
-    target_dir = os.path.join(os.path.dirname(doc_path), pdf_filename) if output_dir is None else output_dir
-    os.makedirs(target_dir, exist_ok=True)
-
-    # Open the input PDF document
-    with fitz.open(doc_path) as doc:
-
-        # Loop over each page in the PDF document
-        for page_num in range(doc.page_count):
-            # Construct the output filename for this page
-            page_filename = f"{page_num+1}.pdf"
-            page_path = os.path.join(target_dir, page_filename)
-
-            # Create a new PDF document with only the current page
-            with fitz.open() as new_doc:
-                new_doc.insert_pdf(doc, from_page=page_num, to_page=page_num)
-
-                # Save the new PDF document to a file
-                new_doc.save(page_path)
-
-                # Add the output file path to the list of files
-                files.append(page_path)
-
-                # Print a message to the console (optional)
-                if config.std_out_logging:
-                    print(f"Saved page {page_num+1} to {page_path}")
-
-    # Return the path to the output directory and the list of output file paths
-    return (target_dir, files)
+from ..settings import config
+import os
+import fitz
+
+def split_document_pages(doc_path, output_dir=None):
+    """
+    Split a PDF document into individual pages and save each page to a separate PDF file.
+
+    Args:
+        doc_path (str): Path to the input PDF file.
+        output_dir (str): Directory to save the output files (default=None).
+
+    Raises:
+        Exception: If doc_path is a directory instead of a file.
+
+    Returns:
+        tuple: A tuple containing the path to the output directory and a list of the output file paths.
+    """
+
+    # Check if doc_path is a file
+    if os.path.isdir(doc_path):
+        raise Exception('doc_path must be a file, not a directory')
+
+    # Create an empty list to store the output file paths
+    files = []
+
+    # Get the PDF filename without extension
+    pdf_filename = os.path.splitext(os.path.basename(doc_path))[0]
+
+    # Create a directory for the PDF pages
+    target_dir = os.path.join(os.path.dirname(doc_path), pdf_filename) if output_dir is None else output_dir
+    os.makedirs(target_dir, exist_ok=True)
+
+    # Open the input PDF document
+    with fitz.open(doc_path) as doc:
+
+        # Loop over each page in the PDF document
+        for page_num in range(doc.page_count):
+            # Construct the output filename for this page
+            page_filename = f"{page_num+1}.pdf"
+            page_path = os.path.join(target_dir, page_filename)
+
+            # Create a new PDF document with only the current page
+            with fitz.open() as new_doc:
+                new_doc.insert_pdf(doc, from_page=page_num, to_page=page_num)
+
+                # Save the new PDF document to a file
+                new_doc.save(page_path)
+
+                # Add the output file path to the list of files
+                files.append(page_path)
+
+                # Print a message to the console (optional)
+                if config.std_out_logging:
+                    print(f"Saved page {page_num+1} to {page_path}")
+
+    # Return the path to the output directory and the list of output file paths
+    return (target_dir, files)
```

### Comparing `insights-extractor-0.1.0/src/extractlib/ner/__init__.py` & `insights-extractor-0.1.1/src/extractlib/ner/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import nltk
-from nltk import word_tokenize, pos_tag
-
-from nlp.stopwords import get_words
-
-nltk.download('averaged_perceptron_tagger')
-nltk.download('maxent_ne_chunker')
-nltk.download('words')
-
-stopwords = get_words()
-
-def get_entities(content):
-    """
-    Extract entities from text using NLTK.
-
-    Args:
-        text (str): The text to extract entities from.
-
-    Returns:
-        list: A list of entities.
-    """
-    try:
-        entities = []
-
-        words = word_tokenize(content)  
-        words = [word for word in words if word.lower() not in stopwords]
-
-        for token in nltk.sent_tokenize(content):
-            for chunk in nltk.ne_chunk(pos_tag(word_tokenize(token))):
-                if hasattr(chunk, 'label'):
-                    entities.append((' '.join(c[0] for c in chunk), chunk.label()))
-        return entities
-    except Exception as e:
-        print(f'Error processing: {e}')
+import nltk
+from nltk import word_tokenize, pos_tag
+
+from nlp.stopwords import get_words
+
+nltk.download('averaged_perceptron_tagger')
+nltk.download('maxent_ne_chunker')
+nltk.download('words')
+
+stopwords = get_words()
+
+def get_entities(content):
+    """
+    Extract entities from text using NLTK.
+
+    Args:
+        text (str): The text to extract entities from.
+
+    Returns:
+        list: A list of entities.
+    """
+    try:
+        entities = []
+
+        words = word_tokenize(content)  
+        words = [word for word in words if word.lower() not in stopwords]
+
+        for token in nltk.sent_tokenize(content):
+            for chunk in nltk.ne_chunk(pos_tag(word_tokenize(token))):
+                if hasattr(chunk, 'label'):
+                    entities.append((' '.join(c[0] for c in chunk), chunk.label()))
+        return entities
+    except Exception as e:
+        print(f'Error processing: {e}')
         raise e
```

### Comparing `insights-extractor-0.1.0/src/extractlib/nlp/pre_process.py` & `insights-extractor-0.1.1/src/extractlib/nlp/pre_process.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import re
-import string
-
-def clean_text(text, remove_punctuation=False, regex_list=None):
-    """
-    Clean a text string by removing new lines, extra whitespace, and optionally punctuation and non-ASCII characters,
-    and matching against a list of regex patterns.
-
-    Args:
-        text (str): The input text string to clean.
-        remove_punctuation (bool): Whether to remove punctuation from the text (default=False).
-        regex_list (list): A list of regex patterns to match against the input text (default=None).
-
-    Returns:
-        str: The cleaned text string.
-    """
-
-    # Remove all single quotes from the text
-    re.sub(r"'", "", text)
-
-    # Remove all new line characters from the text
-    text = re.sub('\n', ' ', text)
-
-    # Remove any extra whitespace from the text
-    text = re.sub('\s+', ' ', text).strip()
-
-    if remove_punctuation:
-        # Remove all punctuation from the text
-        text = text.translate(str.maketrans('', '', string.punctuation))
-
-    if regex_list is not None:
-        # Remove any substrings that match a regex pattern
-        for pattern in regex_list:
-            text = re.sub(pattern, '', text)
-
-    # Remove any non-ASCII characters from the text
-    text = text.encode('ascii', 'ignore').decode()
-
-    # Return the cleaned text string
-    return text
+import re
+import string
+
+def clean_text(text, remove_punctuation=False, regex_list=None):
+    """
+    Clean a text string by removing new lines, extra whitespace, and optionally punctuation and non-ASCII characters,
+    and matching against a list of regex patterns.
+
+    Args:
+        text (str): The input text string to clean.
+        remove_punctuation (bool): Whether to remove punctuation from the text (default=False).
+        regex_list (list): A list of regex patterns to match against the input text (default=None).
+
+    Returns:
+        str: The cleaned text string.
+    """
+
+    # Remove all single quotes from the text
+    re.sub(r"'", "", text)
+
+    # Remove all new line characters from the text
+    text = re.sub('\n', ' ', text)
+
+    # Remove any extra whitespace from the text
+    text = re.sub('\s+', ' ', text).strip()
+
+    if remove_punctuation:
+        # Remove all punctuation from the text
+        text = text.translate(str.maketrans('', '', string.punctuation))
+
+    if regex_list is not None:
+        # Remove any substrings that match a regex pattern
+        for pattern in regex_list:
+            text = re.sub(pattern, '', text)
+
+    # Remove any non-ASCII characters from the text
+    text = text.encode('ascii', 'ignore').decode()
+
+    # Return the cleaned text string
+    return text
```

### Comparing `insights-extractor-0.1.0/src/extractlib/utils/json_utils.py` & `insights-extractor-0.1.1/src/extractlib/utils/json_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import re
-
-from ..nlp.pre_process import clean_text
-from ..settings import config
-
-def extract_json_values(json_obj, result_str):
-    """
-    Recursively extract all string values from a nested JSON object and concatenate them into a single string.
-
-    Args:
-        json_obj (dict or list): A nested JSON object to extract values from.
-        result_str (list): A list used to accumulate the extracted values.
-
-    Returns:
-        str: A string containing all extracted values concatenated together, converted to lowercase.
-    """
-    if isinstance(json_obj, dict):
-        for key, value in json_obj.items():
-            extract_json_values(value, result_str)
-    elif isinstance(json_obj, list):
-        for item in json_obj:
-            extract_json_values(item, result_str)
-    else:
-        result_str.append(json_obj)
-    return ' '.join(result_str).lower()
-
-
-def extract_text_elements(elements, element_valid):
-    result = []
-    for element in elements:
-        if 'text' in element and element_valid(element):
-            result.append(element['text'])
-
-    return ' '.join(result)
-
-
-def cleanse_and_tag_json_structure(data):
-    """
-    Evaluate a JSON data structure for invalid content and tag it with validity information.
-
-    Args:
-        data (dict or list): A dictionary or list containing the JSON data structure to cleanse.
-
-    Returns: None
-
-    Example: { "valid": true | false, "item1": ..., "item2": ..., ... }
-    """
-
-    # Check if the data is a dictionary
-    if isinstance(data, dict):
-        keys_to_remove = []
-
-        # Loop over the dictionary keys and values
-        for key, value in data.items():
-            # If the value is a string
-            if isinstance(value, str):
-                # Check if the string contains any invalid content
-                if test_for_invalid_content(value, config.invalid_content_regexs):
-                    # If the string contains invalid content, tag the entire data structure as invalid
-                    data["valid"] = False
-                else:
-                    # Otherwise, clean the string using the clean_text function and update the dictionary value
-                    data[key] = clean_text(value, False)
-            else:
-                # If the value is not a string, recurse into the data structure to cleanse and tag nested values
-                cleanse_and_tag_json_structure(value)
-
-        # Remove any keys that were flagged for removal during the loop
-        for key in keys_to_remove:
-            del data[key]
-
-    # Check if the data is a list
-    elif isinstance(data, list):
-        # Loop over the list items
-        for i, value in enumerate(data):
-            # If the list item is a string
-            if isinstance(value, str):
-                # Check if the string contains any invalid content
-                if test_for_invalid_content(value, config.invalid_content_regexs):
-                    # If the string contains invalid content, tag the entire data structure as invalid
-                    data["valid"] = False
-                else:
-                    # Otherwise, clean the string using the clean_text function and update the list item
-                    data[i] = clean_text(value, False)
-            else:
-                # If the list item is not a string, recurse into the data structure to cleanse and tag nested values
-                cleanse_and_tag_json_structure(value)
-
-
-def test_for_invalid_content(text, regex_list=[]):
-    """
-    Check if a string contains any invalid content based on a list of regex statements.
-
-    Args:
-        text (str): The input text to check.
-        regex_list (list): A list of regex statements to evaluate against the input text.
-
-    Returns:
-        bool: True if the input text contains any invalid content, False otherwise.
-    """
-    for regex in regex_list:
-        if re.search(regex, text):
-            return True
+import re
+
+from ..nlp.pre_process import clean_text
+from ..settings import config
+
+def extract_json_values(json_obj, result_str):
+    """
+    Recursively extract all string values from a nested JSON object and concatenate them into a single string.
+
+    Args:
+        json_obj (dict or list): A nested JSON object to extract values from.
+        result_str (list): A list used to accumulate the extracted values.
+
+    Returns:
+        str: A string containing all extracted values concatenated together, converted to lowercase.
+    """
+    if isinstance(json_obj, dict):
+        for key, value in json_obj.items():
+            extract_json_values(value, result_str)
+    elif isinstance(json_obj, list):
+        for item in json_obj:
+            extract_json_values(item, result_str)
+    else:
+        result_str.append(json_obj)
+    return ' '.join(result_str).lower()
+
+
+def extract_text_elements(elements, element_valid):
+    result = []
+    for element in elements:
+        if 'text' in element and element_valid(element):
+            result.append(element['text'])
+
+    return ' '.join(result)
+
+
+def cleanse_and_tag_json_structure(data):
+    """
+    Evaluate a JSON data structure for invalid content and tag it with validity information.
+
+    Args:
+        data (dict or list): A dictionary or list containing the JSON data structure to cleanse.
+
+    Returns: None
+
+    Example: { "valid": true | false, "item1": ..., "item2": ..., ... }
+    """
+
+    # Check if the data is a dictionary
+    if isinstance(data, dict):
+        keys_to_remove = []
+
+        # Loop over the dictionary keys and values
+        for key, value in data.items():
+            # If the value is a string
+            if isinstance(value, str):
+                # Check if the string contains any invalid content
+                if test_for_invalid_content(value, config.invalid_content_regexs):
+                    # If the string contains invalid content, tag the entire data structure as invalid
+                    data["valid"] = False
+                else:
+                    # Otherwise, clean the string using the clean_text function and update the dictionary value
+                    data[key] = clean_text(value, False)
+            else:
+                # If the value is not a string, recurse into the data structure to cleanse and tag nested values
+                cleanse_and_tag_json_structure(value)
+
+        # Remove any keys that were flagged for removal during the loop
+        for key in keys_to_remove:
+            del data[key]
+
+    # Check if the data is a list
+    elif isinstance(data, list):
+        # Loop over the list items
+        for i, value in enumerate(data):
+            # If the list item is a string
+            if isinstance(value, str):
+                # Check if the string contains any invalid content
+                if test_for_invalid_content(value, config.invalid_content_regexs):
+                    # If the string contains invalid content, tag the entire data structure as invalid
+                    data["valid"] = False
+                else:
+                    # Otherwise, clean the string using the clean_text function and update the list item
+                    data[i] = clean_text(value, False)
+            else:
+                # If the list item is not a string, recurse into the data structure to cleanse and tag nested values
+                cleanse_and_tag_json_structure(value)
+
+
+def test_for_invalid_content(text, regex_list=[]):
+    """
+    Check if a string contains any invalid content based on a list of regex statements.
+
+    Args:
+        text (str): The input text to check.
+        regex_list (list): A list of regex statements to evaluate against the input text.
+
+    Returns:
+        bool: True if the input text contains any invalid content, False otherwise.
+    """
+    for regex in regex_list:
+        if re.search(regex, text):
+            return True
     return False
```

### Comparing `insights-extractor-0.1.0/src/insights_extractor.egg-info/PKG-INFO` & `insights-extractor-0.1.1/src/insights_extractor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,115 @@
-Metadata-Version: 2.1
-Name: insights-extractor
-Version: 0.1.0
-Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
-Author-email: Trae Moore <trae.dev@gmail.com>
-Project-URL: Homepage, https://github.com/traemoore/insightextractor
-Project-URL: Tests, https://github.com/traemoore/insightextractor-test
-Project-URL: Bug Tracker, https://github.com/traemoore/insightextractor/issues
-Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Extractlib
-
-This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
-
-
-## python dependency overview
-### Python Dependency Install
-<pre>pip install nltk==3.8.1 PyMuPDF==1.21.1 camelot-py==0.11.0 opencv-python==4.7.0.72 ghostscript==0.7</pre>
-
-## manually install supporting binaries
-
-### camelot dependencies
-- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
-
-#### Ubuntu
-<pre>$ apt install ghostscript python3-tk</pre>
-
-#### MacOS
-<pre>$ brew install ghostscript tcl-tk</pre>
-
-## windows dependency installations
-- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
-- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
- 
-# Configuration
-- configuration file should be placed in the root of the project and named 'extractlib.config.json'
-
-## Example 'extractlib.config.json' File
-### this file should be located in the root of your project
-<pre>
-{
-  "std_out_logging": true,
-  "supported_file_types": [".pdf"],
-  "invalid_content_regexs": ["X{2,}"],
-  "stop_words": [
-    "na",
-    "dependent",
-    "address",
-    "plans",
-    "network",
-    "nonnetwork",
-    "additional",
-    "covered"
-  ],
-  "keywords": {
-    "dental": 5,
-    "vision": 5,    
-    "life": 5,
-    "disability": 5
-  },
-  "keyword_synonyms": {
-    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
-    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
-    "life": [
-      "accident",
-      "critical",
-      "illness",
-      "accidental",
-      "dismember",
-      "AD&D"
-    ],
-    "disability": []
-  },
-  "word_min_length": 3
-}
-</pre>
-
-# access config variables
-<pre>
-from extractlib.settings import config
-
-print(json.dump(config.config_raw, indent=4))
-</pre>
-# Example implementation
-<pre>
-from extractlib.document.process import process_document
-import json
-
-def main(file: str):
-    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
-    # Save the HTML content to a temporary file
-    with open('temp.json', 'w') as f:
-        json.dump(result, f, indent=4)
-
-
-if __name__ == '__main__':
-
-    # get working directory
-    import os
-    target_dir = os.path.dirname(os.path.abspath(__file__))
-    main(f'{target_dir}/_testdata/PDF.pdf')
-</pre>
+Metadata-Version: 2.1
+Name: insights-extractor
+Version: 0.1.1
+Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
+Author-email: Trae Moore <trae.dev@gmail.com>
+Project-URL: Homepage, https://github.com/traemoore/insights-extractor
+Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
+Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
+Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Extractlib
+
+This is a Python package that provides a set of tools and utilities for processing and analyzing PDF documents. It includes functionality for extracting text and tables from PDFs, cleaning and preprocessing text data, and analyzing content for keywords and patterns. The package also provides a number of configuration options for customizing the behavior of the tools and utilities, making it flexible and easy to use in a variety of different contexts. Whether you need to extract data from PDF documents for data analysis, or analyze PDF content for specific keywords or patterns, this package provides the tools you need to get the job done quickly and efficiently.
+
+
+## Dependency Overview
+### Python Dependency Install
+This project leverages packages 
+<pre>
+nltk == 3.8.1 
+PyMuPDF == 1.21.1 
+camelot-py == 0.11.0 
+opencv-python == 4.7.0.72 
+ghostscript == 0.7
+</pre>
+
+## manually install supporting binaries
+
+### camelot dependencies
+- https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
+
+#### Ubuntu
+<pre>$ apt install ghostscript python3-tk</pre>
+
+#### MacOS
+<pre>$ brew install ghostscript tcl-tk</pre>
+
+## windows dependency installations
+- Install ghostscript: https://ghostscript.com/releases/gsdnld.html
+- Install Tinker: https://platform.activestate.com/activestate/activetcl-8.6/auto-fork?_ga=2.93217438.2024444162.1679060315-1994225326.1678735799
+ 
+# Configuration
+- configuration file should be placed in the root of the project and named 'extractlib.config.json'
+
+## Example 'extractlib.config.json' File
+### this file should be located in the root of your project
+<pre>
+{
+  "std_out_logging": true,
+  "supported_file_types": [".pdf"],
+  "invalid_content_regexs": ["X{2,}"],
+  "stop_words": [
+    "na",
+    "dependent",
+    "address",
+    "plans",
+    "network",
+    "nonnetwork",
+    "additional",
+    "covered"
+  ],
+  "keywords": {
+    "dental": 5,
+    "vision": 5,    
+    "life": 5,
+    "disability": 5
+  },
+  "keyword_synonyms": {
+    "dental": ["orthodontic", "Endo", "Perio", "Oral"],
+    "vision": ["eye", "vision", "lens", "lenses", "contact", "contacts"],
+    "life": [
+      "accident",
+      "critical",
+      "illness",
+      "accidental",
+      "dismember",
+      "AD&D"
+    ],
+    "disability": []
+  },
+  "word_min_length": 3
+}
+</pre>
+
+# access config variables
+<pre>
+from extractlib.settings import config
+
+print(json.dump(config.config_raw, indent=4))
+</pre>
+# Example implementation
+<pre>
+from extractlib.document.process import process_document
+import json
+
+def main(file: str):
+    result = process_document(file,  exclude_pages=[2,3], use_multithreading=False, split_pages_output_dir='./output', delete_split_pages=False)
+    # Save the HTML content to a temporary file
+    with open('temp.json', 'w') as f:
+        json.dump(result, f, indent=4)
+
+
+if __name__ == '__main__':
+
+    # get working directory
+    import os
+    target_dir = os.path.dirname(os.path.abspath(__file__))
+    main(f'{target_dir}/_testdata/PDF.pdf')
+</pre>
```

### Comparing `insights-extractor-0.1.0/src/insights_extractor.egg-info/SOURCES.txt` & `insights-extractor-0.1.1/src/insights_extractor.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
+dist/insights-extractor-0.1.0.tar.gz
+dist/insights_extractor-0.1.0-py3-none-any.whl
 src/extractlib/__init__.py
 src/extractlib/classification/__init__.py
 src/extractlib/classification/prep_utils.py
 src/extractlib/classification/utils/__init__.py
 src/extractlib/classification/utils/keywords.py
 src/extractlib/document/__init__.py
 src/extractlib/document/page.py
```

