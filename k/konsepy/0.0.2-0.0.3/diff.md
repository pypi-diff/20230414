# Comparing `tmp/konsepy-0.0.2.tar.gz` & `tmp/konsepy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.2.tar", last modified: Thu Apr 13 23:43:36 2023, max compression
+gzip compressed data, was "konsepy-0.0.3.tar", last modified: Fri Apr 14 17:15:34 2023, max compression
```

## Comparing `konsepy-0.0.2.tar` & `konsepy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      996 2023-04-13 23:43:33.587374 konsepy-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-04-13 23:43:33.587374 konsepy-0.0.2/.gitignore
--rw-r--r--   0        0        0      244 2023-04-13 23:43:33.587374 konsepy-0.0.2/README.md
--rw-r--r--   0        0        0      905 2023-04-13 23:43:33.587374 konsepy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/__init__.py
--rw-r--r--   0        0        0     3953 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     2763 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/constants.py
--rw-r--r--   0        0        0     4025 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/importer.py
--rw-r--r--   0        0        0     5086 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/regex.py
--rw-r--r--   0        0        0     2390 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     3738 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/types.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 konsepy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-04-14 17:15:30.821401 konsepy-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-04-14 17:15:30.821401 konsepy-0.0.3/.gitignore
+-rw-r--r--   0        0        0      322 2023-04-14 17:15:30.821401 konsepy-0.0.3/README.md
+-rw-r--r--   0        0        0      905 2023-04-14 17:15:30.821401 konsepy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4077 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     2899 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4195 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5284 2023-04-14 17:15:30.821401 konsepy-0.0.3/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2390 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     3738 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-04-14 17:15:30.825401 konsepy-0.0.3/src/konsepy/types.py
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 konsepy-0.0.3/PKG-INFO
```

### Comparing `konsepy-0.0.2/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.2/pyproject.toml` & `konsepy-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.2/src/konsepy/bio_tag.py` & `konsepy-0.0.3/src/konsepy/bio_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 
     """
     outdir.mkdir(exist_ok=True)
 
     # prepare sentence splitter
     nlp = get_pipeline(sentence_model)
 
+    if not package_name and not regexes:
+        raise ValueError(f'Either `regexes` or `package_name` must be specified.')
     regexes = regexes or build_regex_dict(package_name)
 
     with (
         open(outdir / 'bio_tag_data.csv', 'w', newline='') as out,
         open(outdir / 'bio_tag_data.jsonl', 'w') as jsonl,
     ):
         writer = csv.DictWriter(
```

### Comparing `konsepy-0.0.2/src/konsepy/cli.py` & `konsepy-0.0.3/src/konsepy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,28 @@
     parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
     add_common_cli(parser)
     func(**vars(parser.parse_args()))
 
 
 def snippet_cli():
     parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
-    parser.add_argument('--concept-name', dest='concept_name', required=True,
-                        help='Name of concept to run regexes for.')
     parser.add_argument('--regexes', nargs='+',
                         help=r'REGEX_NAME==(?:re(?:gex)\sto\s(?:search|look)\sfor')
     parser.add_argument('--stop-after-regex-count', dest='stop_after_regex_count', default=None,
                         help='change to number if you want to limit number of regex "hits"; else keep None')
     add_common_cli(parser)
     return vars(parser.parse_args())
 
 
 def add_common_cli(parser: argparse.ArgumentParser):
     add_outdir_and_infiles(parser)
+    parser.add_argument('--package-name', dest='package_name',
+                        help='Name of package to run regular expressions from.')
+    parser.add_argument('--concepts', nargs='+',
+                        help='Name of concepts to process/run regular expressions for.')
     parser.add_argument('--require-regex', default=None,
                         help='Output text containing this regex but in which no regexes were found.')
     parser.add_argument('--start-after', default=0, type=int,
                         help='Start after skipping this many records')
     parser.add_argument('--stop-after', default=None, type=int,
                         help='change to number if you want to limit number of notes searched through; else None.')
     parser.add_argument('--select-probability', default=1.0, type=float,
```

### Comparing `konsepy-0.0.2/src/konsepy/get_text_snippets.py` & `konsepy-0.0.3/src/konsepy/get_text_snippets.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from konsepy.cli import snippet_cli
 from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
 from konsepy.importer import get_all_concepts
 from konsepy.textio import iterate_csv_file
 
 
-def get_text_snippets(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
-                      id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                      notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                      select_probability=1.0, label='snippets', stop_after_regex_count=None):
+def get_text_snippets_regexes(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
+                              id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                              notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                              select_probability=1.0, label='snippets', stop_after_regex_count=None):
     dt = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
     logger.warning('Snippets will have spaces normalized:'
                    ' multiple spaces/newlines/tabs will be converted'
                    ' to a single space in the output.')
     rx_count = 0
     outdir.mkdir(exist_ok=True)
     with open(outdir / f'{label}_{dt}.csv', 'w', newline='') as out:
@@ -47,40 +47,43 @@
                         postcontext,
                     ])
                     rx_count += 1
                     if stop_after_regex_count and rx_count >= stop_after_regex_count:
                         return
 
 
-def get_text_snippets_for_concept_algorithm(package, input_files, outdir, *, concept_name=None, start_after=0,
-                                            stop_after=None,
-                                            window_size=50, regexes=None,
+def get_text_snippets_for_concept_algorithm(package, input_files, outdir, *, concepts=None,
+                                            start_after=0, stop_after=None, window_size=50,
                                             id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                                             notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
                                             select_probability=1.0, label='snippets', stop_after_regex_count=None,
                                             **kwargs):
     regexes = [(regex, category)
-               for concept in get_all_concepts(package, concept_name)
+               for concept in get_all_concepts(package, *concepts)
                for regex, category in concept.regexes]
 
-    get_text_snippets(input_files, outdir, regexes,
-                      start_after=start_after,
-                      stop_after=stop_after,
-                      window_size=window_size,
-                      select_probability=select_probability,
-                      id_label=id_label,
-                      noteid_label=noteid_label,
-                      notedate_label=notedate_label,
-                      notetext_label=notetext_label,
-                      label=label,
-                      stop_after_regex_count=stop_after_regex_count,
-                      )
+    get_text_snippets_regexes(input_files, outdir, regexes,
+                              start_after=start_after,
+                              stop_after=stop_after,
+                              window_size=window_size,
+                              select_probability=select_probability,
+                              id_label=id_label,
+                              noteid_label=noteid_label,
+                              notedate_label=notedate_label,
+                              notetext_label=notetext_label,
+                              label=label,
+                              stop_after_regex_count=stop_after_regex_count,
+                              )
 
 
-if __name__ == '__main__':
+def get_text_snippets_cli(package_name=None):
     kwargs = snippet_cli()
-    kwargs['label'] = kwargs.get('concept_name', 'concept')
+    kwargs['package_name'] = kwargs.get('package_name', package_name)
 
-    if kwargs.get('concept_name', None):
+    if package_name and kwargs.get('concepts', None):
         get_text_snippets_for_concept_algorithm(**kwargs)
     else:
-        get_text_snippets(**kwargs)
+        get_text_snippets_regexes(**kwargs)
+
+
+if __name__ == '__main__':
+    get_text_snippets_cli()
```

### Comparing `konsepy-0.0.2/src/konsepy/importer.py` & `konsepy-0.0.3/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.2/src/konsepy/regex.py` & `konsepy-0.0.3/src/konsepy/regex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import re
 from collections import Counter, defaultdict
 
 from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
+from konsepy.importer import get_all_concepts
 from konsepy.textio import iterate_csv_file, output_results
 from loguru import logger
 
 
 def run_regex_on_files(input_files, regex_func, *, start_after=0, stop_after=None,
                        require_regex=None, window_size=50,
                        id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
@@ -60,33 +61,35 @@
                 end_snippet = m.end() + window_size
                 snippet = text[start_snippet:end_snippet + 1]
                 not_found_text[' '.join(snippet.split())] += 1
         else:
             not_found_text[' '.join(text.split())] += 1
 
 
-def run_regex_and_output(name, input_files, outdir, regex_func, *category_enums,
+def run_regex_and_output(package_name, input_files, outdir, *concepts,
                          start_after=0, stop_after=None, require_regex=None, window_size=50,
                          id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                          notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
                          select_probability=1.0):
     dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    curr_outdir = outdir / f'{name}_{dt}'
-    curr_outdir.mkdir(parents=True)
-    logger.add(curr_outdir / f'{name}_{dt}.log')
-    note_counter, cat_counter_mrns, not_found_text, mrn_to_cat, note_to_cat = run_regex_on_files(
-        input_files, regex_func, start_after=start_after, stop_after=stop_after, require_regex=require_regex,
-        window_size=window_size,
-        id_label=id_label, noteid_label=noteid_label,
-        notedate_label=notedate_label, notetext_label=notetext_label,
-        select_probability=select_probability
-    )
-    output_results(curr_outdir, not_found_text=not_found_text, note_counter=note_counter,
-                   cat_counter_mrns=cat_counter_mrns, category_enums=category_enums,
-                   note_to_cat=note_to_cat, mrn_to_cat=mrn_to_cat)
+    for iconcept in get_all_concepts(package_name, *concepts):
+        curr_outdir = outdir / f'{iconcept.name}_{dt}'
+        curr_outdir.mkdir(parents=True)
+        logger.add(curr_outdir / f'{iconcept.name}_{dt}.log')
+        note_counter, cat_counter_mrns, not_found_text, mrn_to_cat, note_to_cat = run_regex_on_files(
+            input_files, iconcept.run_func,
+            start_after=start_after, stop_after=stop_after, require_regex=require_regex,
+            window_size=window_size,
+            id_label=id_label, noteid_label=noteid_label,
+            notedate_label=notedate_label, notetext_label=notetext_label,
+            select_probability=select_probability
+        )
+        output_results(curr_outdir, not_found_text=not_found_text, note_counter=note_counter,
+                       cat_counter_mrns=cat_counter_mrns, category_enums=[iconcept.category_enum],
+                       note_to_cat=note_to_cat, mrn_to_cat=mrn_to_cat)
 
 
 def search_first_regex(regexes):
     """For each regex, only return first instance (use search)"""
 
     def _search_first_regex(text):
         for regex, category in regexes:
```

### Comparing `konsepy-0.0.2/src/konsepy/run_all.py` & `konsepy-0.0.3/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.2/src/konsepy/rxutils.py` & `konsepy-0.0.3/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.2/src/konsepy/textio.py` & `konsepy-0.0.3/src/konsepy/textio.py`

 * *Files identical despite different names*

