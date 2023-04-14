# Comparing `tmp/cmip-0.0.1.tar.gz` & `tmp/cmip-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip-0.0.1.tar", last modified: Fri Apr 14 09:33:53 2023, max compression
+gzip compressed data, was "cmip-0.0.2.tar", last modified: Fri Apr 14 09:40:56 2023, max compression
```

## Comparing `cmip-0.0.1.tar` & `cmip-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.961792 cmip-0.0.1/
--rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      493 2023-04-14 09:33:53.959801 cmip-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2022-12-15 09:05:59.000000 cmip-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.915241 cmip-0.0.1/cmip/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.927785 cmip-0.0.1/cmip/data/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/data/ad.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/data/chinese_frequency.tsv
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/data/letter_mapping.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/data/pinyin.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.929789 cmip-0.0.1/cmip/gibberish/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/gibberish/__init__.py
--rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/gibberish/gibberish.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.931786 cmip-0.0.1/cmip/image/
--rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.938800 cmip-0.0.1/cmip/text/
--rw-rw-rw-   0        0        0     3028 2022-12-15 09:32:04.000000 cmip-0.0.1/cmip/text/__init__.py
--rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.1/cmip/text/ac_automation.py
--rw-rw-rw-   0        0        0     4417 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/text/encoder.py
--rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/text/normalize.py
--rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/text/similarity.py
--rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.1/cmip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.949788 cmip-0.0.1/cmip/web/
--rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.1/cmip/web/__init__.py
--rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.1/cmip/web/html.py
--rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/web/simhash_utils.py
--rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/web/utils.py
--rw-rw-rw-   0        0        0     4037 2023-03-01 10:38:36.000000 cmip-0.0.1/cmip/web/web_scraping.py
--rw-rw-rw-   0        0        0     3294 2023-04-14 09:29:32.000000 cmip-0.0.1/cmip/web/web_scraping2.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.953784 cmip-0.0.1/cmip/word_discover/
--rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/word_discover/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/word_discover/ngram.py
--rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.1/cmip/word_discover/word_discover.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.921234 cmip-0.0.1/cmip.egg-info/
--rw-rw-rw-   0        0        0      493 2023-04-14 09:33:53.000000 cmip-0.0.1/cmip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      762 2023-04-14 09:33:53.000000 cmip-0.0.1/cmip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:33:53.000000 cmip-0.0.1/cmip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-14 09:33:53.000000 cmip-0.0.1/cmip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 09:33:53.000000 cmip-0.0.1/cmip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 09:33:53.961792 cmip-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      742 2022-10-27 04:31:09.000000 cmip-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:33:53.957785 cmip-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.1/test/test_ac_automation.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.349835 cmip-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      493 2023-04-14 09:40:56.348837 cmip-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2022-12-15 09:05:59.000000 cmip-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.312827 cmip-0.0.2/cmip/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.323820 cmip-0.0.2/cmip/data/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/ad.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/chinese_frequency.tsv
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/letter_mapping.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/pinyin.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.325819 cmip-0.0.2/cmip/gibberish/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/gibberish/__init__.py
+-rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/gibberish/gibberish.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.327819 cmip-0.0.2/cmip/image/
+-rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.332821 cmip-0.0.2/cmip/text/
+-rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.2/cmip/text/__init__.py
+-rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.2/cmip/text/ac_automation.py
+-rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/text/normalize.py
+-rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/text/similarity.py
+-rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.2/cmip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.340825 cmip-0.0.2/cmip/web/
+-rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.2/cmip/web/__init__.py
+-rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.2/cmip/web/html.py
+-rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/web/simhash_utils.py
+-rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/web/utils.py
+-rw-rw-rw-   0        0        0     4037 2023-03-01 10:38:36.000000 cmip-0.0.2/cmip/web/web_scraping.py
+-rw-rw-rw-   0        0        0     3294 2023-04-14 09:29:32.000000 cmip-0.0.2/cmip/web/web_scraping2.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.344836 cmip-0.0.2/cmip/word_discover/
+-rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/ngram.py
+-rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/word_discover.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.319822 cmip-0.0.2/cmip.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:40:56.349835 cmip-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-14 09:40:49.000000 cmip-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.347839 cmip-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.2/test/test_ac_automation.py
```

### Comparing `cmip-0.0.1/LICENSE` & `cmip-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/gibberish/gibberish.py` & `cmip-0.0.2/cmip/gibberish/gibberish.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/image/__init__.py` & `cmip-0.0.2/cmip/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/text/__init__.py` & `cmip-0.0.2/cmip/text/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from cmip.text.ac_automation import ACAutomation
 from cmip.text.normalize import Normalize
-from cmip.text.encoder import FeatureEncoder
 from joblib import Parallel, delayed
 import multiprocessing
 import re
 
 n_cpus = multiprocessing.cpu_count()
 default_pattern = re.compile("[^\u4E00-\u9FEF\u3400-\u4DB5a-zA-Z0-9]+", re.U)
 
 
 class Text(object):
 
     def __init__(self, case_sensitive=True):
         self.aca = ACAutomation(case_sensitive=case_sensitive)
         self.norm = Normalize()
-        self.feature_encoder = FeatureEncoder()
         self.add_keywords_from_list = self.aca.add_keywords_from_list
         self.get_keywords = self.aca.get_keywords
         self.replace_keywords = self.aca.replace_keywords
         self.extract_keywords = self.aca.extract_keywords
         self.normalize = self.norm.normalize
         self.pinyin = self.norm.pinyin
-        self.encode = self.feature_encoder.encode
 
     def clean(self, sentence, patten: str = None, keep_space: bool = True, norm: bool = True, lower: bool = True,
               digital_norm: bool = False, max_repeat: int = 0) -> str:
         if patten is None:
             patten = default_pattern
         else:
             patten = re.compile(patten, re.U)
```

### Comparing `cmip-0.0.1/cmip/text/ac_automation.py` & `cmip-0.0.2/cmip/text/ac_automation.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/text/normalize.py` & `cmip-0.0.2/cmip/text/normalize.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/text/similarity.py` & `cmip-0.0.2/cmip/text/similarity.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/utils.py` & `cmip-0.0.2/cmip/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/web/html.py` & `cmip-0.0.2/cmip/web/html.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/web/simhash_utils.py` & `cmip-0.0.2/cmip/web/simhash_utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/web/utils.py` & `cmip-0.0.2/cmip/web/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/web/web_scraping.py` & `cmip-0.0.2/cmip/web/web_scraping.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/web/web_scraping2.py` & `cmip-0.0.2/cmip/web/web_scraping2.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/word_discover/ngram.py` & `cmip-0.0.2/cmip/word_discover/ngram.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip/word_discover/word_discover.py` & `cmip-0.0.2/cmip/word_discover/word_discover.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.1/cmip.egg-info/SOURCES.txt` & `cmip-0.0.2/cmip.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 cmip/data/letter_mapping.txt
 cmip/data/pinyin.txt
 cmip/gibberish/__init__.py
 cmip/gibberish/gibberish.py
 cmip/image/__init__.py
 cmip/text/__init__.py
 cmip/text/ac_automation.py
-cmip/text/encoder.py
 cmip/text/normalize.py
 cmip/text/similarity.py
 cmip/web/__init__.py
 cmip/web/html.py
 cmip/web/simhash_utils.py
 cmip/web/utils.py
 cmip/web/web_scraping.py
```

### Comparing `cmip-0.0.1/setup.py` & `cmip-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmip",
-    version="0.0.1",
+    version="0.0.2",
     author="geb",
     author_email="853934146@qq.com",
     description="An efficient information processing program.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikuh/cmip",
     packages=setuptools.find_packages(),
```

### Comparing `cmip-0.0.1/test/test_ac_automation.py` & `cmip-0.0.2/test/test_ac_automation.py`

 * *Files identical despite different names*

