# Comparing `tmp/konsepy-0.0.3.tar.gz` & `tmp/konsepy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.3.tar", last modified: Fri Apr 14 17:15:34 2023, max compression
+gzip compressed data, was "konsepy-0.0.4.tar", last modified: Fri Apr 14 18:07:27 2023, max compression
```

## Comparing `konsepy-0.0.3.tar` & `konsepy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      996 2023-04-14 17:15:30.821401 konsepy-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-04-14 17:15:30.821401 konsepy-0.0.3/.gitignore
--rw-r--r--   0        0        0      322 2023-04-14 17:15:30.821401 konsepy-0.0.3/README.md
--rw-r--r--   0        0        0      905 2023-04-14 17:15:30.821401 konsepy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4077 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     2899 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/constants.py
--rw-r--r--   0        0        0     4195 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/importer.py
--rw-r--r--   0        0        0     5284 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/regex.py
--rw-r--r--   0        0        0     2390 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     3738 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/types.py
--rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 konsepy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-04-14 18:07:23.814765 konsepy-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-04-14 18:07:23.814765 konsepy-0.0.4/.gitignore
+-rw-r--r--   0        0        0      335 2023-04-14 18:07:23.814765 konsepy-0.0.4/README.md
+-rw-r--r--   0        0        0      905 2023-04-14 18:07:23.814765 konsepy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4077 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     2899 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4249 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5284 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2390 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     3738 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/types.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.4/PKG-INFO
```

### Comparing `konsepy-0.0.3/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/pyproject.toml` & `konsepy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/bio_tag.py` & `konsepy-0.0.4/src/konsepy/bio_tag.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/cli.py` & `konsepy-0.0.4/src/konsepy/cli.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/get_text_snippets.py` & `konsepy-0.0.4/src/konsepy/get_text_snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from konsepy.importer import get_all_concepts
 from konsepy.textio import iterate_csv_file
 
 
 def get_text_snippets_regexes(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
                               id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                               notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                              select_probability=1.0, label='snippets', stop_after_regex_count=None):
+                              select_probability=1.0, label='snippets', stop_after_regex_count=None, **kwargs):
     dt = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
     logger.warning('Snippets will have spaces normalized:'
                    ' multiple spaces/newlines/tabs will be converted'
                    ' to a single space in the output.')
     rx_count = 0
     outdir.mkdir(exist_ok=True)
     with open(outdir / f'{label}_{dt}.csv', 'w', newline='') as out:
@@ -26,15 +26,16 @@
         for _, studyid, note_id, note_date, text in iterate_csv_file(
                 input_files, start_after=start_after, stop_after=stop_after,
                 id_label=id_label, noteid_label=noteid_label,
                 notetext_label=notetext_label, notedate_label=notedate_label,
                 select_probability=select_probability
         ):
             text = ' '.join(text.split())  # remove newlines, etc. (bad for snippets in Excel)
-            for name, regex in regexes:
+            for regex_ in regexes:
+                name, regex = regex_.split('==')
                 if isinstance(regex, str):
                     regex = re.compile(regex, re.I)
                 for m in regex.finditer(text):
                     precontext = text[max(m.start() - window_size, 0):m.start()]
                     postcontext = text[m.end():m.end() + window_size]
                     writer.writerow([
                         rx_count,  # id
```

### Comparing `konsepy-0.0.3/src/konsepy/importer.py` & `konsepy-0.0.4/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/regex.py` & `konsepy-0.0.4/src/konsepy/regex.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/run_all.py` & `konsepy-0.0.4/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/rxutils.py` & `konsepy-0.0.4/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/src/konsepy/textio.py` & `konsepy-0.0.4/src/konsepy/textio.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.3/PKG-INFO` & `konsepy-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,14 +24,14 @@
 
 # konsepy
 
 Framework for build NLP information extraction systems using regular expressions.
 
 ## Usage
 
-For now, find documentation for this library (and a template to download) from https://github.com/kpwhri/konsepy.
+For now, find documentation for this library (and a template to download) from https://github.com/kpwhri/konsepy_nlp_template.
 
 
 ## Roadmap
 
 * Change labels to some metadata object to allow more diverse input sources and run info
```

