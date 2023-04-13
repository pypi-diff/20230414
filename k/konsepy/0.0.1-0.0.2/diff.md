# Comparing `tmp/konsepy-0.0.1.tar.gz` & `tmp/konsepy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.1.tar", last modified: Thu Apr 13 23:38:48 2023, max compression
+gzip compressed data, was "konsepy-0.0.2.tar", last modified: Thu Apr 13 23:43:36 2023, max compression
```

## Comparing `konsepy-0.0.1.tar` & `konsepy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       46 2023-04-13 23:38:42.158098 konsepy-0.0.1/.gitignore
--rw-r--r--   0        0        0      254 2023-04-13 23:16:11.077341 konsepy-0.0.1/README.md
--rw-r--r--   0        0        0      941 2023-04-13 23:30:13.242786 konsepy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-13 22:17:44.131507 konsepy-0.0.1/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4059 2023-04-13 23:00:11.382290 konsepy-0.0.1/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     2817 2023-04-13 22:55:28.265030 konsepy-0.0.1/src/konsepy/cli.py
--rw-r--r--   0        0        0      108 2023-04-13 21:00:01.919603 konsepy-0.0.1/src/konsepy/constants.py
--rw-r--r--   0        0        0     4111 2023-04-13 23:30:13.242786 konsepy-0.0.1/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1613 2023-04-13 23:07:16.490714 konsepy-0.0.1/src/konsepy/importer.py
--rw-r--r--   0        0        0     5204 2023-04-13 21:08:06.012513 konsepy-0.0.1/src/konsepy/regex.py
--rw-r--r--   0        0        0     2447 2023-04-13 23:07:57.272627 konsepy-0.0.1/src/konsepy/run_all.py
--rw-r--r--   0        0        0      684 2023-02-06 22:47:20.154377 konsepy-0.0.1/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     3825 2023-04-13 22:27:56.607540 konsepy-0.0.1/src/konsepy/textio.py
--rw-r--r--   0        0        0      211 2023-04-13 21:17:58.397367 konsepy-0.0.1/src/konsepy/types.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 konsepy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-04-13 23:43:33.587374 konsepy-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-04-13 23:43:33.587374 konsepy-0.0.2/.gitignore
+-rw-r--r--   0        0        0      244 2023-04-13 23:43:33.587374 konsepy-0.0.2/README.md
+-rw-r--r--   0        0        0      905 2023-04-13 23:43:33.587374 konsepy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     3953 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     2763 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4025 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5086 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2390 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     3738 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-04-13 23:43:33.587374 konsepy-0.0.2/src/konsepy/types.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 konsepy-0.0.2/PKG-INFO
```

### Comparing `konsepy-0.0.1/pyproject.toml` & `konsepy-0.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[build-system]
-requires = ['flit_core >=3.2,<4']
-build-backend = 'flit_core.buildapi'
-
-[project]
-name = 'konsepy'
-dynamic = ['version', 'description']
-authors = [
-    { name = 'dcronkite', email = 'dcronkite+pypi@gmail.com' },
-]
-readme = 'README.md'
-dependencies = [
-    'loguru',
-    'pytest',
-    'sas7bdat',
-]
-requires-python = '>=3.10'
-keywords = [
-    'nlp',
-]
-classifiers = [# https://pypi.org/classifiers/
-    'Development Status :: 5 - Production/Stable',
-    'Intended Audience :: Science/Research',
-    'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Topic :: Text Processing :: Linguistic',
-    'License :: OSI Approved :: MIT License',
-    'Intended Audience :: Healthcare Industry',
-]
-
-[project.urls]
-Home = 'https://github.com/kpwhri/konsepy'
-
-[project.optional-dependencies]
-ssplit = ['spacy']
+[build-system]
+requires = ['flit_core >=3.2,<4']
+build-backend = 'flit_core.buildapi'
+
+[project]
+name = 'konsepy'
+dynamic = ['version', 'description']
+authors = [
+    { name = 'dcronkite', email = 'dcronkite+pypi@gmail.com' },
+]
+readme = 'README.md'
+dependencies = [
+    'loguru',
+    'pytest',
+    'sas7bdat',
+]
+requires-python = '>=3.10'
+keywords = [
+    'nlp',
+]
+classifiers = [# https://pypi.org/classifiers/
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Science/Research',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: Text Processing :: Linguistic',
+    'License :: OSI Approved :: MIT License',
+    'Intended Audience :: Healthcare Industry',
+]
+
+[project.urls]
+Home = 'https://github.com/kpwhri/konsepy'
+
+[project.optional-dependencies]
+ssplit = ['spacy']
```

### Comparing `konsepy-0.0.1/src/konsepy/cli.py` & `konsepy-0.0.2/src/konsepy/cli.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import argparse
-from pathlib import Path
-
-from konsepy.constants import NOTETEXT_LABEL, NOTEDATE_LABEL, NOTEID_LABEL, ID_LABEL
-
-
-def concept_cli(func):
-    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
-    add_common_cli(parser)
-    func(**vars(parser.parse_args()))
-
-
-def snippet_cli():
-    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
-    parser.add_argument('--concept-name', dest='concept_name', required=True,
-                        help='Name of concept to run regexes for.')
-    parser.add_argument('--regexes', nargs='+',
-                        help=r'REGEX_NAME==(?:re(?:gex)\sto\s(?:search|look)\sfor')
-    parser.add_argument('--stop-after-regex-count', dest='stop_after_regex_count', default=None,
-                        help='change to number if you want to limit number of regex "hits"; else keep None')
-    add_common_cli(parser)
-    return vars(parser.parse_args())
-
-
-def add_common_cli(parser: argparse.ArgumentParser):
-    add_outdir_and_infiles(parser)
-    parser.add_argument('--require-regex', default=None,
-                        help='Output text containing this regex but in which no regexes were found.')
-    parser.add_argument('--start-after', default=0, type=int,
-                        help='Start after skipping this many records')
-    parser.add_argument('--stop-after', default=None, type=int,
-                        help='change to number if you want to limit number of notes searched through; else None.')
-    parser.add_argument('--select-probability', default=1.0, type=float,
-                        help='Set to less than 1.0 to increase note sample (e.g., 0.3); 1.0=don\'t skip anything')
-    parser.add_argument('--window-size', default=50, type=int,
-                        help='Change the window for the pre/post contexts')
-
-
-def add_outdir_and_infiles(parser: argparse.ArgumentParser = None):
-    if not parser:
-        parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
-    parser.add_argument('--outdir', type=Path, default=Path('.'),
-                        help='Directory to place output files.')
-    parser.add_argument('--input-files', nargs='+', type=str, default=list(),
-                        help='Input CSV or SAS file(s) to read.')
-    parser.add_argument('--id-label', default=ID_LABEL,
-                        help='Column label for individual id')
-    parser.add_argument('--noteid-label', default=NOTEID_LABEL,
-                        help='Column label for individual id')
-    parser.add_argument('--notedate-label', default=NOTEDATE_LABEL,
-                        help='Column label for individual id')
-    parser.add_argument('--notetext-label', default=NOTETEXT_LABEL,
-                        help='Column label for individual id')
-    return parser
+import argparse
+from pathlib import Path
+
+from konsepy.constants import NOTETEXT_LABEL, NOTEDATE_LABEL, NOTEID_LABEL, ID_LABEL
+
+
+def concept_cli(func):
+    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
+    add_common_cli(parser)
+    func(**vars(parser.parse_args()))
+
+
+def snippet_cli():
+    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
+    parser.add_argument('--concept-name', dest='concept_name', required=True,
+                        help='Name of concept to run regexes for.')
+    parser.add_argument('--regexes', nargs='+',
+                        help=r'REGEX_NAME==(?:re(?:gex)\sto\s(?:search|look)\sfor')
+    parser.add_argument('--stop-after-regex-count', dest='stop_after_regex_count', default=None,
+                        help='change to number if you want to limit number of regex "hits"; else keep None')
+    add_common_cli(parser)
+    return vars(parser.parse_args())
+
+
+def add_common_cli(parser: argparse.ArgumentParser):
+    add_outdir_and_infiles(parser)
+    parser.add_argument('--require-regex', default=None,
+                        help='Output text containing this regex but in which no regexes were found.')
+    parser.add_argument('--start-after', default=0, type=int,
+                        help='Start after skipping this many records')
+    parser.add_argument('--stop-after', default=None, type=int,
+                        help='change to number if you want to limit number of notes searched through; else None.')
+    parser.add_argument('--select-probability', default=1.0, type=float,
+                        help='Set to less than 1.0 to increase note sample (e.g., 0.3); 1.0=don\'t skip anything')
+    parser.add_argument('--window-size', default=50, type=int,
+                        help='Change the window for the pre/post contexts')
+
+
+def add_outdir_and_infiles(parser: argparse.ArgumentParser = None):
+    if not parser:
+        parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
+    parser.add_argument('--outdir', type=Path, default=Path('.'),
+                        help='Directory to place output files.')
+    parser.add_argument('--input-files', nargs='+', type=str, default=list(),
+                        help='Input CSV or SAS file(s) to read.')
+    parser.add_argument('--id-label', default=ID_LABEL,
+                        help='Column label for individual id')
+    parser.add_argument('--noteid-label', default=NOTEID_LABEL,
+                        help='Column label for individual id')
+    parser.add_argument('--notedate-label', default=NOTEDATE_LABEL,
+                        help='Column label for individual id')
+    parser.add_argument('--notetext-label', default=NOTETEXT_LABEL,
+                        help='Column label for individual id')
+    return parser
```

### Comparing `konsepy-0.0.1/src/konsepy/get_text_snippets.py` & `konsepy-0.0.2/src/konsepy/get_text_snippets.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import csv
-import datetime
-import re
-
-from loguru import logger
-
-from konsepy.cli import snippet_cli
-from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
-from konsepy.importer import get_all_concepts
-from konsepy.textio import iterate_csv_file
-
-
-def get_text_snippets(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
-                      id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                      notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                      select_probability=1.0, label='snippets', stop_after_regex_count=None):
-    dt = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
-    logger.warning('Snippets will have spaces normalized:'
-                   ' multiple spaces/newlines/tabs will be converted'
-                   ' to a single space in the output.')
-    rx_count = 0
-    outdir.mkdir(exist_ok=True)
-    with open(outdir / f'{label}_{dt}.csv', 'w', newline='') as out:
-        writer = csv.writer(out)
-        writer.writerow(['id', 'studyid', 'note_id', 'date', 'regex_name', 'precontext', 'term', 'postcontext'])
-        for _, studyid, note_id, note_date, text in iterate_csv_file(
-                input_files, start_after=start_after, stop_after=stop_after,
-                id_label=id_label, noteid_label=noteid_label,
-                notetext_label=notetext_label, notedate_label=notedate_label,
-                select_probability=select_probability
-        ):
-            text = ' '.join(text.split())  # remove newlines, etc. (bad for snippets in Excel)
-            for name, regex in regexes:
-                if isinstance(regex, str):
-                    regex = re.compile(regex, re.I)
-                for m in regex.finditer(text):
-                    precontext = text[max(m.start() - window_size, 0):m.start()]
-                    postcontext = text[m.end():m.end() + window_size]
-                    writer.writerow([
-                        rx_count,  # id
-                        studyid,
-                        note_id,
-                        note_date,
-                        name,
-                        precontext,
-                        m.group(),  # term
-                        postcontext,
-                    ])
-                    rx_count += 1
-                    if stop_after_regex_count and rx_count >= stop_after_regex_count:
-                        return
-
-
-def get_text_snippets_for_concept_algorithm(package, input_files, outdir, *, concept_name=None, start_after=0,
-                                            stop_after=None,
-                                            window_size=50, regexes=None,
-                                            id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                                            notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                                            select_probability=1.0, label='snippets', stop_after_regex_count=None,
-                                            **kwargs):
-    regexes = [(regex, category)
-               for concept in get_all_concepts(package, concept_name)
-               for regex, category in concept.regexes]
-
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
-
-
-if __name__ == '__main__':
-    kwargs = snippet_cli()
-    kwargs['label'] = kwargs.get('concept_name', 'concept')
-
-    if kwargs.get('concept_name', None):
-        get_text_snippets_for_concept_algorithm(**kwargs)
-    else:
-        get_text_snippets(**kwargs)
+import csv
+import datetime
+import re
+
+from loguru import logger
+
+from konsepy.cli import snippet_cli
+from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
+from konsepy.importer import get_all_concepts
+from konsepy.textio import iterate_csv_file
+
+
+def get_text_snippets(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
+                      id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                      notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                      select_probability=1.0, label='snippets', stop_after_regex_count=None):
+    dt = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
+    logger.warning('Snippets will have spaces normalized:'
+                   ' multiple spaces/newlines/tabs will be converted'
+                   ' to a single space in the output.')
+    rx_count = 0
+    outdir.mkdir(exist_ok=True)
+    with open(outdir / f'{label}_{dt}.csv', 'w', newline='') as out:
+        writer = csv.writer(out)
+        writer.writerow(['id', 'studyid', 'note_id', 'date', 'regex_name', 'precontext', 'term', 'postcontext'])
+        for _, studyid, note_id, note_date, text in iterate_csv_file(
+                input_files, start_after=start_after, stop_after=stop_after,
+                id_label=id_label, noteid_label=noteid_label,
+                notetext_label=notetext_label, notedate_label=notedate_label,
+                select_probability=select_probability
+        ):
+            text = ' '.join(text.split())  # remove newlines, etc. (bad for snippets in Excel)
+            for name, regex in regexes:
+                if isinstance(regex, str):
+                    regex = re.compile(regex, re.I)
+                for m in regex.finditer(text):
+                    precontext = text[max(m.start() - window_size, 0):m.start()]
+                    postcontext = text[m.end():m.end() + window_size]
+                    writer.writerow([
+                        rx_count,  # id
+                        studyid,
+                        note_id,
+                        note_date,
+                        name,
+                        precontext,
+                        m.group(),  # term
+                        postcontext,
+                    ])
+                    rx_count += 1
+                    if stop_after_regex_count and rx_count >= stop_after_regex_count:
+                        return
+
+
+def get_text_snippets_for_concept_algorithm(package, input_files, outdir, *, concept_name=None, start_after=0,
+                                            stop_after=None,
+                                            window_size=50, regexes=None,
+                                            id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                                            notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                                            select_probability=1.0, label='snippets', stop_after_regex_count=None,
+                                            **kwargs):
+    regexes = [(regex, category)
+               for concept in get_all_concepts(package, concept_name)
+               for regex, category in concept.regexes]
+
+    get_text_snippets(input_files, outdir, regexes,
+                      start_after=start_after,
+                      stop_after=stop_after,
+                      window_size=window_size,
+                      select_probability=select_probability,
+                      id_label=id_label,
+                      noteid_label=noteid_label,
+                      notedate_label=notedate_label,
+                      notetext_label=notetext_label,
+                      label=label,
+                      stop_after_regex_count=stop_after_regex_count,
+                      )
+
+
+if __name__ == '__main__':
+    kwargs = snippet_cli()
+    kwargs['label'] = kwargs.get('concept_name', 'concept')
+
+    if kwargs.get('concept_name', None):
+        get_text_snippets_for_concept_algorithm(**kwargs)
+    else:
+        get_text_snippets(**kwargs)
```

### Comparing `konsepy-0.0.1/src/konsepy/importer.py` & `konsepy-0.0.2/src/konsepy/importer.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import importlib
-import pkgutil
-from enum import EnumType
-from pathlib import Path
-
-from loguru import logger
-
-
-class ConceptImport:
-
-    def __init__(self, module_info, package_name):
-        self.name = module_info.name
-        self.imp = importlib.import_module(f'{package_name}.concepts.{self.name}')
-        self.category_enum = self._get_category()
-        self.run_func = self.imp.RUN_REGEXES_FUNC
-        self.regexes = self.imp.REGEXES
-
-    def run(self, sentence):
-        self.run_func(sentence)
-
-    @property
-    def domain(self):
-        return self.name
-
-    @property
-    def categories(self):
-        return [category.name for category in self.category_enum]
-
-    def _get_category(self):
-        for name, value in self.imp.__dict__.items():
-            if isinstance(value, EnumType):
-                return value
-        raise ValueError(f'Unable to identify category enum for concept "{self.name}".')
-
-    def __str__(self):
-        return f'ConceptImport<{self.name}>'
-
-
-def get_all_concepts(package_name: str, *concepts):
-    imp = importlib.import_module(f'{package_name}.concepts')
-    path = Path(imp.__file__).parent
-    for module_info in pkgutil.iter_modules([path]):
-        if concepts and module_info.name not in concepts:
-            continue  # look for only requested concepts if any supplied
-        try:
-            yield ConceptImport(module_info, package_name)
-        except ValueError as ve:
-            logger.warning(f'Failed to load concept: {package_name}.concepts.{module_info.name}')
-            logger.exception(ve)
+import importlib
+import pkgutil
+from enum import EnumType
+from pathlib import Path
+
+from loguru import logger
+
+
+class ConceptImport:
+
+    def __init__(self, module_info, package_name):
+        self.name = module_info.name
+        self.imp = importlib.import_module(f'{package_name}.concepts.{self.name}')
+        self.category_enum = self._get_category()
+        self.run_func = self.imp.RUN_REGEXES_FUNC
+        self.regexes = self.imp.REGEXES
+
+    def run(self, sentence):
+        self.run_func(sentence)
+
+    @property
+    def domain(self):
+        return self.name
+
+    @property
+    def categories(self):
+        return [category.name for category in self.category_enum]
+
+    def _get_category(self):
+        for name, value in self.imp.__dict__.items():
+            if isinstance(value, EnumType):
+                return value
+        raise ValueError(f'Unable to identify category enum for concept "{self.name}".')
+
+    def __str__(self):
+        return f'ConceptImport<{self.name}>'
+
+
+def get_all_concepts(package_name: str, *concepts):
+    imp = importlib.import_module(f'{package_name}.concepts')
+    path = Path(imp.__file__).parent
+    for module_info in pkgutil.iter_modules([path]):
+        if concepts and module_info.name not in concepts:
+            continue  # look for only requested concepts if any supplied
+        try:
+            yield ConceptImport(module_info, package_name)
+        except ValueError as ve:
+            logger.warning(f'Failed to load concept: {package_name}.concepts.{module_info.name}')
+            logger.exception(ve)
```

### Comparing `konsepy-0.0.1/src/konsepy/regex.py` & `konsepy-0.0.2/src/konsepy/regex.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import datetime
-import re
-from collections import Counter, defaultdict
-
-from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
-from konsepy.textio import iterate_csv_file, output_results
-from loguru import logger
-
-
-def run_regex_on_files(input_files, regex_func, *, start_after=0, stop_after=None,
-                       require_regex=None, window_size=50,
-                       id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                       notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                       select_probability=1.0):
-    count = 0  # default value; received from forloop below
-    cat_counter_notes = Counter()
-    cat_counter_mrns = defaultdict(set)
-    noteid_to_cat = defaultdict(Counter)
-    mrn_to_cat = defaultdict(Counter)
-    unique_mrns = set()
-    not_found_text = Counter()
-    if require_regex:
-        require_regex = re.compile(require_regex, re.I)
-    for count, mrn, note_id, note_date, text in iterate_csv_file(
-            input_files, start_after=start_after, stop_after=stop_after,
-            id_label=id_label, noteid_label=noteid_label,
-            notedate_label=notedate_label, notetext_label=notetext_label,
-            select_probability=select_probability
-    ):
-        if count % 10000 == 0:
-            logger.info(
-                f'Completed {count} records: {len(unique_mrns)} MRNs contain any category ({datetime.datetime.now()})')
-        extract_categories(
-            mrn, note_id, text, regex_func,
-            cat_counter_mrns=cat_counter_mrns, cat_counter_notes=cat_counter_notes,
-            mrn_to_cat=mrn_to_cat, require_regex=require_regex,
-            not_found_text=not_found_text, noteid_to_cat=noteid_to_cat,
-            unique_mrns=unique_mrns, window_size=window_size
-        )
-    logger.info(f'Finished. Total records: {count}  ({datetime.datetime.now()})')
-    return cat_counter_notes, cat_counter_mrns, not_found_text, mrn_to_cat, noteid_to_cat
-
-
-def extract_categories(mrn, note_id, text, regex_func, *,
-                       cat_counter_mrns=None, cat_counter_notes=None, mrn_to_cat=None,
-                       not_found_text=None, noteid_to_cat=None,
-                       require_regex=None, unique_mrns=None, window_size=50):
-    categories = list(regex_func(text))
-    for category in categories:
-        mrn_to_cat[mrn][category] += 1
-        noteid_to_cat[(mrn, note_id)][category] += 1
-        cat_counter_notes[category] += 1
-        cat_counter_mrns[category].add(mrn)
-    if categories:
-        unique_mrns.add(mrn)
-    if not categories and not_found_text:
-        if require_regex:
-            for m in require_regex.finditer(text):
-                start_snippet = max(0, m.start() - window_size)
-                end_snippet = m.end() + window_size
-                snippet = text[start_snippet:end_snippet + 1]
-                not_found_text[' '.join(snippet.split())] += 1
-        else:
-            not_found_text[' '.join(text.split())] += 1
-
-
-def run_regex_and_output(name, input_files, outdir, regex_func, *category_enums,
-                         start_after=0, stop_after=None, require_regex=None, window_size=50,
-                         id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                         notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                         select_probability=1.0):
-    dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
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
-
-
-def search_first_regex(regexes):
-    """For each regex, only return first instance (use search)"""
-
-    def _search_first_regex(text):
-        for regex, category in regexes:
-            if regex.search(text):
-                yield category
-
-    return _search_first_regex
-
-
-def search_all_regex(regexes):
-    """For each regex, return all (use finditer)"""
-
-    def _search_all_regex(text):
-        for regex, category in regexes:
-            for _ in regex.finditer(text):
-                yield category
-
-    return _search_all_regex
-
-
-def get_all_regex_by_index(regexes):
-    """For each regex, return all results, including indices"""
-
-    def _get_all_regex_by_index(text):
-        for regex, category in regexes:
-            for m in regex.finditer(text):
-                yield category.name, m.group(), m.start(), m.end()
-
-    return _get_all_regex_by_index
+import datetime
+import re
+from collections import Counter, defaultdict
+
+from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
+from konsepy.textio import iterate_csv_file, output_results
+from loguru import logger
+
+
+def run_regex_on_files(input_files, regex_func, *, start_after=0, stop_after=None,
+                       require_regex=None, window_size=50,
+                       id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                       notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                       select_probability=1.0):
+    count = 0  # default value; received from forloop below
+    cat_counter_notes = Counter()
+    cat_counter_mrns = defaultdict(set)
+    noteid_to_cat = defaultdict(Counter)
+    mrn_to_cat = defaultdict(Counter)
+    unique_mrns = set()
+    not_found_text = Counter()
+    if require_regex:
+        require_regex = re.compile(require_regex, re.I)
+    for count, mrn, note_id, note_date, text in iterate_csv_file(
+            input_files, start_after=start_after, stop_after=stop_after,
+            id_label=id_label, noteid_label=noteid_label,
+            notedate_label=notedate_label, notetext_label=notetext_label,
+            select_probability=select_probability
+    ):
+        if count % 10000 == 0:
+            logger.info(
+                f'Completed {count} records: {len(unique_mrns)} MRNs contain any category ({datetime.datetime.now()})')
+        extract_categories(
+            mrn, note_id, text, regex_func,
+            cat_counter_mrns=cat_counter_mrns, cat_counter_notes=cat_counter_notes,
+            mrn_to_cat=mrn_to_cat, require_regex=require_regex,
+            not_found_text=not_found_text, noteid_to_cat=noteid_to_cat,
+            unique_mrns=unique_mrns, window_size=window_size
+        )
+    logger.info(f'Finished. Total records: {count}  ({datetime.datetime.now()})')
+    return cat_counter_notes, cat_counter_mrns, not_found_text, mrn_to_cat, noteid_to_cat
+
+
+def extract_categories(mrn, note_id, text, regex_func, *,
+                       cat_counter_mrns=None, cat_counter_notes=None, mrn_to_cat=None,
+                       not_found_text=None, noteid_to_cat=None,
+                       require_regex=None, unique_mrns=None, window_size=50):
+    categories = list(regex_func(text))
+    for category in categories:
+        mrn_to_cat[mrn][category] += 1
+        noteid_to_cat[(mrn, note_id)][category] += 1
+        cat_counter_notes[category] += 1
+        cat_counter_mrns[category].add(mrn)
+    if categories:
+        unique_mrns.add(mrn)
+    if not categories and not_found_text:
+        if require_regex:
+            for m in require_regex.finditer(text):
+                start_snippet = max(0, m.start() - window_size)
+                end_snippet = m.end() + window_size
+                snippet = text[start_snippet:end_snippet + 1]
+                not_found_text[' '.join(snippet.split())] += 1
+        else:
+            not_found_text[' '.join(text.split())] += 1
+
+
+def run_regex_and_output(name, input_files, outdir, regex_func, *category_enums,
+                         start_after=0, stop_after=None, require_regex=None, window_size=50,
+                         id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                         notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                         select_probability=1.0):
+    dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    curr_outdir = outdir / f'{name}_{dt}'
+    curr_outdir.mkdir(parents=True)
+    logger.add(curr_outdir / f'{name}_{dt}.log')
+    note_counter, cat_counter_mrns, not_found_text, mrn_to_cat, note_to_cat = run_regex_on_files(
+        input_files, regex_func, start_after=start_after, stop_after=stop_after, require_regex=require_regex,
+        window_size=window_size,
+        id_label=id_label, noteid_label=noteid_label,
+        notedate_label=notedate_label, notetext_label=notetext_label,
+        select_probability=select_probability
+    )
+    output_results(curr_outdir, not_found_text=not_found_text, note_counter=note_counter,
+                   cat_counter_mrns=cat_counter_mrns, category_enums=category_enums,
+                   note_to_cat=note_to_cat, mrn_to_cat=mrn_to_cat)
+
+
+def search_first_regex(regexes):
+    """For each regex, only return first instance (use search)"""
+
+    def _search_first_regex(text):
+        for regex, category in regexes:
+            if regex.search(text):
+                yield category
+
+    return _search_first_regex
+
+
+def search_all_regex(regexes):
+    """For each regex, return all (use finditer)"""
+
+    def _search_all_regex(text):
+        for regex, category in regexes:
+            for _ in regex.finditer(text):
+                yield category
+
+    return _search_all_regex
+
+
+def get_all_regex_by_index(regexes):
+    """For each regex, return all results, including indices"""
+
+    def _get_all_regex_by_index(text):
+        for regex, category in regexes:
+            for m in regex.finditer(text):
+                yield category.name, m.group(), m.start(), m.end()
+
+    return _get_all_regex_by_index
```

### Comparing `konsepy-0.0.1/src/konsepy/run_all.py` & `konsepy-0.0.2/src/konsepy/run_all.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import datetime
-import pathlib
-from collections import Counter, defaultdict
-
-from loguru import logger
-
-from konsepy.cli import add_outdir_and_infiles
-from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
-from konsepy.importer import get_all_concepts
-from konsepy.regex import extract_categories
-from konsepy.textio import iterate_csv_file, output_results
-
-
-def run_all(input_files, outdir: pathlib.Path, package_name: str, *,
-            id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-            notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-            ):
-    dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    curr_outdir = outdir / f'run_all_{dt}'
-    curr_outdir.mkdir(parents=True)
-    logger.add(curr_outdir / f'run_all_{dt}.log')
-    count = 0  # default value; received from forloop below
-    cat_counter_notes = Counter()
-    cat_counter_mrns = defaultdict(set)
-    noteid_to_cat = defaultdict(Counter)
-    mrn_to_cat = defaultdict(Counter)
-    unique_mrns = set()
-    concepts = list(get_all_concepts(package_name))
-    logger.info(f'Loaded {len(concepts)} concepts for processing.')
-    for count, studyid, note_id, note_date, text in iterate_csv_file(
-            input_files,
-            id_label=id_label, noteid_label=noteid_label,
-            notedate_label=notedate_label, notetext_label=notetext_label,
-    ):
-        if count % 10000 == 0:
-            logger.info(f'Completed {count} records for {len(unique_mrns)} MRNs ({datetime.datetime.now()})')
-
-        for concept in concepts:
-            extract_categories(
-                studyid, note_id, text, concept.run_func,
-                cat_counter_mrns=cat_counter_mrns, cat_counter_notes=cat_counter_notes,
-                mrn_to_cat=mrn_to_cat, noteid_to_cat=noteid_to_cat,
-                unique_mrns=unique_mrns
-            )
-    logger.info(f'Finished. Total records: {count}  ({datetime.datetime.now()})')
-    output_results(curr_outdir, note_counter=cat_counter_notes,
-                   cat_counter_mrns=cat_counter_mrns,
-                   category_enums=[c.category_enum for c in concepts],
-                   note_to_cat=noteid_to_cat, mrn_to_cat=mrn_to_cat)
-
-
-if __name__ == '__main__':
-    import argparse
-
-    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
-    add_outdir_and_infiles(parser)
-    run_all(**vars(parser.parse_args()))
+import datetime
+import pathlib
+from collections import Counter, defaultdict
+
+from loguru import logger
+
+from konsepy.cli import add_outdir_and_infiles
+from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
+from konsepy.importer import get_all_concepts
+from konsepy.regex import extract_categories
+from konsepy.textio import iterate_csv_file, output_results
+
+
+def run_all(input_files, outdir: pathlib.Path, package_name: str, *,
+            id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+            notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+            ):
+    dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    curr_outdir = outdir / f'run_all_{dt}'
+    curr_outdir.mkdir(parents=True)
+    logger.add(curr_outdir / f'run_all_{dt}.log')
+    count = 0  # default value; received from forloop below
+    cat_counter_notes = Counter()
+    cat_counter_mrns = defaultdict(set)
+    noteid_to_cat = defaultdict(Counter)
+    mrn_to_cat = defaultdict(Counter)
+    unique_mrns = set()
+    concepts = list(get_all_concepts(package_name))
+    logger.info(f'Loaded {len(concepts)} concepts for processing.')
+    for count, studyid, note_id, note_date, text in iterate_csv_file(
+            input_files,
+            id_label=id_label, noteid_label=noteid_label,
+            notedate_label=notedate_label, notetext_label=notetext_label,
+    ):
+        if count % 10000 == 0:
+            logger.info(f'Completed {count} records for {len(unique_mrns)} MRNs ({datetime.datetime.now()})')
+
+        for concept in concepts:
+            extract_categories(
+                studyid, note_id, text, concept.run_func,
+                cat_counter_mrns=cat_counter_mrns, cat_counter_notes=cat_counter_notes,
+                mrn_to_cat=mrn_to_cat, noteid_to_cat=noteid_to_cat,
+                unique_mrns=unique_mrns
+            )
+    logger.info(f'Finished. Total records: {count}  ({datetime.datetime.now()})')
+    output_results(curr_outdir, note_counter=cat_counter_notes,
+                   cat_counter_mrns=cat_counter_mrns,
+                   category_enums=[c.category_enum for c in concepts],
+                   note_to_cat=noteid_to_cat, mrn_to_cat=mrn_to_cat)
+
+
+if __name__ == '__main__':
+    import argparse
+
+    parser = argparse.ArgumentParser(fromfile_prefix_chars='@!')
+    add_outdir_and_infiles(parser)
+    run_all(**vars(parser.parse_args()))
```

### Comparing `konsepy-0.0.1/src/konsepy/textio.py` & `konsepy-0.0.2/src/konsepy/textio.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""
-Simplify reading input files by creating an iterating wrapper.
-"""
-import csv
-import random
-
-from loguru import logger
-from sas7bdat import SAS7BDAT
-
-from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
-
-
-def iterate_csv_file(input_files, *, start_after=0, stop_after=None,
-                     id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                     notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                     select_probability=1.0, encoding='latin1'):
-    """Return count, mrn, note_id, text for each row in csv file"""
-    count = 0
-    total_count = 0
-    for input_file in input_files:
-        func = _extract_sas_file if input_file.endswith('sas7bdat') else _extract_csv_file
-        for mrn, text, note_id, date in func(input_file, encoding, id_label, noteid_label, notedate_label,
-                                             notetext_label):
-            if random.random() > select_probability:
-                continue
-            total_count += 1
-            if start_after >= total_count:
-                continue
-            count += 1
-            yield count, mrn, note_id, date, text
-            if stop_after and count > stop_after:
-                return
-
-
-def _extract_sas_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
-    with SAS7BDAT(input_file, skip_header=False, encoding=encoding) as fh:
-        header = []
-        for row in fh:
-            if not header:
-                header = row
-                continue
-            mrn = row[header.index(id_label)]
-            date = row[header.index(notedate_label)] if notedate_label else ''
-            text = row[header.index(noteid_label)]
-            noteid = row[header.index(notetext_label)]
-            yield mrn, text, noteid, date
-
-
-def _extract_csv_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
-    with open(input_file, encoding=encoding) as fh:
-        for row in csv.DictReader(fh):
-            text = row[notetext_label]
-            mrn = row[id_label]
-            date = row.get(notedate_label, '')
-            note_id = row[noteid_label]
-            yield mrn, text, note_id, date
-
-
-def output_results(outdir, *, not_found_text=None,
-                   note_counter=None, cat_counter_mrns=None,
-                   category_enums=None, note_to_cat=None, mrn_to_cat=None):
-    categories = [e for category_enum in category_enums for e in category_enum]
-    if not_found_text is not None:
-        with open(outdir / 'snippets.csv', 'w', newline='') as out:
-            writer = csv.writer(out)
-            writer.writerow(['count', 'snippet'])
-            for snippet, count in not_found_text.most_common():
-                writer.writerow([count, ' '.join(snippet.split())])
-
-    with open(outdir / 'category_counts.csv', 'w', newline='') as out:
-        writer = csv.writer(out)
-        writer.writerow(['category', 'note_count', 'mrn_count'])
-        for cat in categories:
-            writer.writerow([cat, note_counter[cat], len(cat_counter_mrns[cat])])
-
-    with open(outdir / 'mrn_category_counts.csv', 'w', newline='') as out:
-        writer = csv.DictWriter(out, ['mrn'] + categories)
-        writer.writeheader()
-        for mrn, note_counter in mrn_to_cat.items():
-            writer.writerow({'mrn': mrn} | dict(note_counter))
-
-    with open(outdir / 'notes_category_counts.csv', 'w', newline='') as out:
-        writer = csv.DictWriter(out, ['mrn', 'note_id'] + categories)
-        writer.writeheader()
-        for (mrn, note), note_counter in note_to_cat.items():
-            writer.writerow({'mrn': mrn, 'note_id': note} | dict(note_counter))
-    logger.info(f'Unique MRNs: {len(mrn_to_cat)}')
+"""
+Simplify reading input files by creating an iterating wrapper.
+"""
+import csv
+import random
+
+from loguru import logger
+from sas7bdat import SAS7BDAT
+
+from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
+
+
+def iterate_csv_file(input_files, *, start_after=0, stop_after=None,
+                     id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
+                     notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                     select_probability=1.0, encoding='latin1'):
+    """Return count, mrn, note_id, text for each row in csv file"""
+    count = 0
+    total_count = 0
+    for input_file in input_files:
+        func = _extract_sas_file if input_file.endswith('sas7bdat') else _extract_csv_file
+        for mrn, text, note_id, date in func(input_file, encoding, id_label, noteid_label, notedate_label,
+                                             notetext_label):
+            if random.random() > select_probability:
+                continue
+            total_count += 1
+            if start_after >= total_count:
+                continue
+            count += 1
+            yield count, mrn, note_id, date, text
+            if stop_after and count > stop_after:
+                return
+
+
+def _extract_sas_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
+    with SAS7BDAT(input_file, skip_header=False, encoding=encoding) as fh:
+        header = []
+        for row in fh:
+            if not header:
+                header = row
+                continue
+            mrn = row[header.index(id_label)]
+            date = row[header.index(notedate_label)] if notedate_label else ''
+            text = row[header.index(noteid_label)]
+            noteid = row[header.index(notetext_label)]
+            yield mrn, text, noteid, date
+
+
+def _extract_csv_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
+    with open(input_file, encoding=encoding) as fh:
+        for row in csv.DictReader(fh):
+            text = row[notetext_label]
+            mrn = row[id_label]
+            date = row.get(notedate_label, '')
+            note_id = row[noteid_label]
+            yield mrn, text, note_id, date
+
+
+def output_results(outdir, *, not_found_text=None,
+                   note_counter=None, cat_counter_mrns=None,
+                   category_enums=None, note_to_cat=None, mrn_to_cat=None):
+    categories = [e for category_enum in category_enums for e in category_enum]
+    if not_found_text is not None:
+        with open(outdir / 'snippets.csv', 'w', newline='') as out:
+            writer = csv.writer(out)
+            writer.writerow(['count', 'snippet'])
+            for snippet, count in not_found_text.most_common():
+                writer.writerow([count, ' '.join(snippet.split())])
+
+    with open(outdir / 'category_counts.csv', 'w', newline='') as out:
+        writer = csv.writer(out)
+        writer.writerow(['category', 'note_count', 'mrn_count'])
+        for cat in categories:
+            writer.writerow([cat, note_counter[cat], len(cat_counter_mrns[cat])])
+
+    with open(outdir / 'mrn_category_counts.csv', 'w', newline='') as out:
+        writer = csv.DictWriter(out, ['mrn'] + categories)
+        writer.writeheader()
+        for mrn, note_counter in mrn_to_cat.items():
+            writer.writerow({'mrn': mrn} | dict(note_counter))
+
+    with open(outdir / 'notes_category_counts.csv', 'w', newline='') as out:
+        writer = csv.DictWriter(out, ['mrn', 'note_id'] + categories)
+        writer.writeheader()
+        for (mrn, note), note_counter in note_to_cat.items():
+            writer.writerow({'mrn': mrn, 'note_id': note} | dict(note_counter))
+    logger.info(f'Unique MRNs: {len(mrn_to_cat)}')
```

### Comparing `konsepy-0.0.1/PKG-INFO` & `konsepy-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

