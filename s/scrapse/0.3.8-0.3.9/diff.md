# Comparing `tmp/scrapse-0.3.8.tar.gz` & `tmp/scrapse-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapse-0.3.8.tar", max compression
+gzip compressed data, was "scrapse-0.3.9.tar", max compression
```

## Comparing `scrapse-0.3.8.tar` & `scrapse-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1278 2023-03-21 11:04:50.701989 scrapse-0.3.8/README.md
--rw-r--r--   0        0        0      709 2023-03-22 22:28:01.248998 scrapse-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-20 10:25:30.867753 scrapse-0.3.8/scrapse/__init__.py
--rw-r--r--   0        0        0       48 2023-02-17 23:02:02.467334 scrapse-0.3.8/scrapse/__main__.py
--rw-r--r--   0        0        0     9913 2023-03-22 22:25:09.063424 scrapse-0.3.8/scrapse/leggitalia/commands/dump_judgments.py
--rw-r--r--   0        0        0      337 2023-03-20 11:21:34.107694 scrapse-0.3.8/scrapse/leggitalia/commands/save_cookie.py
--rw-r--r--   0        0        0     4834 2023-03-21 10:21:03.703908 scrapse-0.3.8/scrapse/leggitalia/commands/scrap_judgments.py
--rw-r--r--   0        0        0     1425 2023-03-20 11:34:25.439314 scrapse-0.3.8/scrapse/leggitalia/commands/scrap_voices.py
--rw-r--r--   0        0        0      393 2023-03-20 11:21:34.111429 scrapse-0.3.8/scrapse/leggitalia/commands/show_filters.py
--rw-r--r--   0        0        0     1007 2023-03-21 10:15:58.934025 scrapse-0.3.8/scrapse/leggitalia/leggitalia.py
--rw-r--r--   0        0        0     9895 2023-03-22 22:01:53.116186 scrapse-0.3.8/scrapse/leggitalia/utils.py
--rw-r--r--   0        0        0      729 2023-03-22 22:28:01.241059 scrapse-0.3.8/scrapse/main.py
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 scrapse-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1278 2023-03-21 11:04:50.701989 scrapse-0.3.9/README.md
+-rw-r--r--   0        0        0      894 2023-04-14 12:28:27.924996 scrapse-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-20 10:25:30.867753 scrapse-0.3.9/scrapse/__init__.py
+-rw-r--r--   0        0        0       48 2023-02-17 23:02:02.467334 scrapse-0.3.9/scrapse/__main__.py
+-rw-r--r--   0        0        0     1724 2023-03-27 13:06:03.246672 scrapse-0.3.9/scrapse/judgment/anonimization_utils.py
+-rw-r--r--   0        0        0     9042 2023-03-27 13:06:03.246975 scrapse-0.3.9/scrapse/judgment/commands/extraction.py
+-rw-r--r--   0        0        0     2531 2023-03-27 13:06:03.247363 scrapse-0.3.9/scrapse/judgment/conversion_utils.py
+-rw-r--r--   0        0        0     2748 2023-03-27 13:06:03.247577 scrapse-0.3.9/scrapse/judgment/extraction_utils.py
+-rw-r--r--   0        0        0      810 2023-03-28 12:56:56.887519 scrapse-0.3.9/scrapse/judgment/general_utils.py
+-rw-r--r--   0        0        0      702 2023-03-27 13:06:03.248078 scrapse-0.3.9/scrapse/judgment/judgment.py
+-rw-r--r--   0        0        0     9971 2023-04-13 12:48:48.240674 scrapse-0.3.9/scrapse/leggitalia/commands/dump_judgments.py
+-rw-r--r--   0        0        0      338 2023-03-27 13:06:03.249752 scrapse-0.3.9/scrapse/leggitalia/commands/save_cookie.py
+-rw-r--r--   0        0        0     4827 2023-04-12 18:35:09.235245 scrapse-0.3.9/scrapse/leggitalia/commands/scrap_judgments.py
+-rw-r--r--   0        0        0     1441 2023-04-12 18:17:08.847602 scrapse-0.3.9/scrapse/leggitalia/commands/scrap_voices.py
+-rw-r--r--   0        0        0      394 2023-03-27 13:06:03.250059 scrapse-0.3.9/scrapse/leggitalia/commands/show_filters.py
+-rw-r--r--   0        0        0    95863 2023-04-12 17:02:46.147640 scrapse-0.3.9/scrapse/leggitalia/comuni.txt
+-rw-r--r--   0        0        0     1007 2023-03-21 10:15:58.934025 scrapse-0.3.9/scrapse/leggitalia/leggitalia.py
+-rw-r--r--   0        0        0    10162 2023-04-12 18:17:08.873593 scrapse-0.3.9/scrapse/leggitalia/utils.py
+-rw-r--r--   0        0        0      827 2023-04-14 12:28:27.919315 scrapse-0.3.9/scrapse/main.py
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 scrapse-0.3.9/PKG-INFO
```

### Comparing `scrapse-0.3.8/README.md` & `scrapse-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `scrapse-0.3.8/scrapse/leggitalia/commands/dump_judgments.py` & `scrapse-0.3.9/scrapse/leggitalia/commands/dump_judgments.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,33 +50,31 @@
 
 
 def extract_object(soup):
     keyword = 'oggetto:'
     tag = soup.find(text=lambda t: t and keyword in t.lower())
     return tag.parent.text.replace('(asterisco)', '').lower().split(keyword, 1)[1].strip() if tag is not None else None
 
-
-def extract_tribunal_section(soup):
+def extract_tribunal_section(soup, ldi):
+    ##Da definire meglio la sezione, volendo anche l'ente giuduziario.
     estrcomp = soup.find('div', class_='estrcomp')
     section = [section.strip().lower() for section in SECTIONS if section in estrcomp.text][0]
-    tribunal = estrcomp.text.lower().split(section, 1)[0].replace('tribunale', '').strip()
-    # print(f'tribunale {tribunal}')
-    # print(f'section {section}')
+    tribunal = ''.join([comune.strip() for comune in ldi.comuni if str(comune) in estrcomp.text.lower().split()])
     return tribunal, section
 
 
 def extract_sent_anno(soup):
     text = soup.find('div', class_='estrcomp').text
     match_date = re.search(r'\d{2}/\d{2}/\d{4}', text)
     return datetime.strptime(match_date.group(), '%d/%m/%Y').year
 
 
-def extract_metadata(soup, file_name):
+def extract_metadata(soup, file_name, ldi):
     extract_sent_anno(soup)
-    tribunale, sezione = extract_tribunal_section(soup)
+    tribunale, sezione = extract_tribunal_section(soup, ldi)
     judgment_metadata = JudgmentMetadata(
         nomefile=file_name,
         origine='onelegale',
         tribunale=tribunale,
         sezione=sezione,
         voci=extract_voices(soup),
         sent_anno=extract_sent_anno(soup),
@@ -118,18 +116,18 @@
         fatto_decisione=corpus.get('fatto-decisione'),
         pqm=corpus.get('pqm'),
     )
 
     return judgment_corpus
 
 
-def extract_metadata_and_corpus(file):
+def extract_metadata_and_corpus(file, ldi):
     soup = read_file(file)
     file_name = file.split('/')[-1].split('.')[0]
-    judgment_metadata = extract_metadata(soup, file_name)
+    judgment_metadata = extract_metadata(soup, file_name, ldi)
     judgment_corpus = extract_corpus(soup, file_name)
     return judgment_metadata, judgment_corpus
 
 
 def build_dict(metadata_and_corpus):
     metadata_dict, corpus_dict = dict(), dict()
     for metadata, corpus in metadata_and_corpus:
@@ -164,15 +162,15 @@
         f.write(json.dumps([data for data in unified_judgments], cls=JudgmentEncoder, indent=4, ensure_ascii=False))
 
 
 def dump_judgments(
         directory: str = typer.Option(None, '--directory', '-d', help='Folder path from which to read judgments.',
                                       show_default=False),
         extension: str = typer.Option('HTM', '--extension', '-e', help='File extension to read.'),
-        path: str = typer.Option('/'.join([LeggiDiItalia.main_directory_path, 'judgments_dump']), '--path', '-p',
+        path: str = typer.Option(LeggiDiItalia.main_directory_path_dump_judgments, '--path', '-p',
                                  help='Folder path from which to read judgments.'),
         mongo: bool = typer.Option(False, '--mongodb', '-m', help='Dump judgments for mongoDB'),
         unified: bool = typer.Option(False, '--unified', '-u', help='Dump judgments into unified json file'),
 ):
     """
     Dump judgments to json format
     """
@@ -182,44 +180,48 @@
                 "[progress.description]{task.description}",
                 BarColumn(),
                 "[progress.percentage]{task.percentage:>3.0f}%",
                 TimeRemainingColumn(),
                 TimeElapsedColumn(),
                 refresh_per_second=5,
         ) as progress:
+
+            ldi = LeggiDiItalia()
+            ldi.load_comuni()
+
             files_to_read = ['/'.join([directory, filename]) for filename in os.listdir(directory) if
                              filename.endswith(extension)]
             progress_task = progress.add_task(description="[green]Extract metadata and corpus progress",
                                               total=len(files_to_read), completed=0)
 
             metadata_and_corpus = list()
             with ThreadPoolExecutor() as executor:
-                for index, file in enumerate(files_to_read[:100]):
-                    metadata_and_corpus.append(executor.submit(extract_metadata_and_corpus, file).result())
+                for index, file in enumerate(files_to_read):
+                    metadata_and_corpus.append(executor.submit(extract_metadata_and_corpus, file, ldi).result())
                     progress.update(progress_task, completed=index)
 
             if mongo:
                 progress.update(progress_task, description="[green]Save json for MongoDB progress", total=3,
                                 completed=0)
                 dump_judgments_directory_path = Path(
-                    '/'.join([path, f'mongodb_{datetime.now().strftime("%d-%Y_%H-%M-%S")}']))
+                    '/'.join([path, f'mongodb_{directory.split("/")[-1]}']))
                 dump_judgments_directory_path.mkdir(exist_ok=True, parents=True)
                 progress.update(progress_task, completed=1)
                 metadata_dict, corpus_dict = build_dict(metadata_and_corpus)
                 progress.update(progress_task, completed=2)
 
                 with ThreadPoolExecutor() as executor:
                     executor.submit(save_json_mongodb, metadata_dict, dump_judgments_directory_path, 'metadata')
                     executor.submit(save_json_mongodb, corpus_dict, dump_judgments_directory_path, 'corpus')
                 progress.update(progress_task, completed=3)
 
             if unified:
                 progress.update(progress_task, description="[green]Save unified json progress", total=3, completed=0)
                 dump_judgments_directory_path = Path(
-                    '/'.join([path, f'unified_{str(datetime.now().strftime("%d-%Y_%H-%M-%S"))}']))
+                    '/'.join([path, f'unified_{directory.split("/")[-1]}']))
                 dump_judgments_directory_path.mkdir(exist_ok=True, parents=True)
                 progress.update(progress_task, completed=1)
 
                 unified_judgments = [Judgment(metadata=metadata, corpus=corpus) for metadata, corpus in
                                      metadata_and_corpus]
                 progress.update(progress_task, completed=2)
                 save_json_unified(unified_judgments, dump_judgments_directory_path)
```

### Comparing `scrapse-0.3.8/scrapse/leggitalia/commands/scrap_judgments.py` & `scrapse-0.3.9/scrapse/leggitalia/commands/scrap_judgments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import typer
 import requests
 import math
+import re
 
 from scrapse.leggitalia.utils import LeggiDiItalia, SECTIONS
 from pathlib import Path
 from bs4 import BeautifulSoup
 from rich.progress import Progress, SpinnerColumn, TextColumn, BarColumn, TimeRemainingColumn, TimeElapsedColumn
 from concurrent.futures import ThreadPoolExecutor
 
 
-def extract_file_name(soup, judgment_id):
-    estrcomp = soup.find('div', class_='estrcomp')
-    file_name = estrcomp.text.lower().split(
-        [section.strip().lower() for section in SECTIONS if section in estrcomp.text][0], 1)[0].strip() + judgment_id
-    file_name = file_name.replace(' ', '').replace('tribunale', '')
-    return file_name
+def extract_file_name(ldi, soup, judgment_id):
+    estrcomp = soup.find('div', class_='estrcomp').text.lower().split()
+    comune = ''.join([comune.strip() for comune in ldi.comuni if str(comune) in estrcomp])
+    return ''.join([comune, '_', judgment_id])
 
 
 def search_judgments(ldi):
     with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=False,
@@ -55,34 +54,36 @@
                               range(0, len(judgments_id), ldi.batch_size)]
 
     request = requests.post(url=ldi.baseurl, headers=ldi.headers, params=ldi.build_export_query(formatted_judgments_id))
 
     soup = BeautifulSoup(request.text, 'html.parser')
     for index, judgment in enumerate(soup.find_all("div", {"class": "doc_body"})):
         output_file = Path('/'.join(
-            (f'{ldi.judgment_directory_path}', f'{extract_file_name(judgment, judgments_id[index])}.{ldi.extension}')))
+            (f'{ldi.judgment_directory_path}', f'{extract_file_name(ldi, judgment, judgments_id[index])}.{ldi.extension}')))
         output_file.write_text(str(judgment))
 
 
 def scrap_judgments(
         judicial_bodies: str = typer.Option(None, "--judicial-bodies", "-j", help="Filter judging bodies"),
         location: str = typer.Option(None, "--location", "-l", help="Filter location of the court of reference"),
         sections: str = typer.Option(None, "--sections", "-s", help="Reference section filter, may change by location"),
-        path: Path = typer.Option(LeggiDiItalia.main_directory_path, "--path", "-p",
+        path: Path = typer.Option(LeggiDiItalia.main_directory_path_scrap_judgments, "--path", "-p",
                                   help="Path where to save downloaded judgments"),
         extension: str = typer.Option("HTM", "--extension", "-e", help="Desired extension of judgments"),
 ):
     """
         Extract the judgments from the platform https://pa.leggiditalia.it """'\n'"""
         It is necessary to specify at least one filter among: -j, -l and -s. """'\n'"""
         Provide an input list with the following formatting: -s 'par1, par2, ...'
     """
     ldi = LeggiDiItalia(judicial_bodies=judicial_bodies, location=location, sections=sections,
                         path=path, extension=extension, command='scrap_judgments')
+
     number_of_judgments = search_judgments(ldi)
+    ldi.build_scraped_judgments_directory_path()
     pagination = build_pagination(ldi, number_of_judgments)
 
     with Progress(
             "[progress.description]{task.description}",
             BarColumn(),
             "[progress.percentage]{task.percentage:>3.0f}%",
             TimeRemainingColumn(),
```

### Comparing `scrapse-0.3.8/scrapse/leggitalia/commands/scrap_voices.py` & `scrapse-0.3.9/scrapse/leggitalia/commands/scrap_voices.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         if 'folder' in voice:
             del voice['folder']
             voice['items'] = extract_voices(ldi, key=voice['key'])
     return voices
 
 
 def scrap_voices(
-        path: str = typer.Option(LeggiDiItalia.main_directory_path, '--path', '-p',
+        path: str = typer.Option(LeggiDiItalia.main_directory_path_scrap_judgments, '--path', '-p',
                                  help='Path where to save json file'),
         show: bool = typer.Option(True, '--show', '-s', help='View extracted voices.')
 ):
     """
         Extraction of the voices tree
     """
     ldi = LeggiDiItalia(path=path, command='scrap_voices')
```

### Comparing `scrapse-0.3.8/scrapse/leggitalia/leggitalia.py` & `scrapse-0.3.9/scrapse/leggitalia/leggitalia.py`

 * *Files identical despite different names*

### Comparing `scrapse-0.3.8/scrapse/leggitalia/utils.py` & `scrapse-0.3.9/scrapse/leggitalia/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
-import json
 
 from json import JSONEncoder
 from pathlib import Path
 from rich.console import Console
+from datetime import datetime
+import pandas as pd
 
 LOCATIONS = ['asti', 'alessandria', 'cuneo', 'ivrea', 'novara', 'torino']
 
 SECTIONS = [
     'Sez. Unite', '(Ad. Plen.)', 'Sez. I', 'Sez. I bis', 'Sez. I ter', 'Sez. I quater', 'Sez. II',
     'Sez. II bis', 'Sez. II ter', 'Sez. II quater', 'Sez. III', 'Sez. III bis', 'Sez. III ter',
     'Sez. III quater', 'Sez. IV', 'Sez. IV bis', 'Sez. IV ter', 'Sez. IV quater', 'Sez. V', 'Sez. V bis',
@@ -88,68 +89,74 @@
 
     batch_size = 100
 
     judgment_directory_path = None
 
     voices_directory_path = None
 
-    main_directory_path = '/'.join([str(Path.home()), 'scrapse', 'leggitalia'])
+    main_directory_path_scrap_judgments = '/'.join([str(Path.home()), 'scrapse', 'leggitalia', 'scraped_judgments'])
+    main_directory_path_dump_judgments = '/'.join([str(Path.home()), 'scrapse', 'leggitalia', 'dumped_judgments'])
+
+    comuni = None
 
     def __init__(self, judicial_bodies=None, sections=None, location=None, extension=None, path=None,
                  command=None) -> None:
         super().__init__()
         if command == 'scrap_judgments':
             self.judicial_bodies = judicial_bodies
             self.sections = sections
             self.location = location
             self.extension = extension
             self.path = str(path)
             self.check_filters()
             self.build_headers()
             self.build_search_query()
-            self.build_judgments_directory_path()
+            self.load_comuni()
         elif command == 'scrap_voices':
             self.build_voices_directory_path()
 
     def check_filters(self):
         if self.judicial_bodies is None and self.sections is None and self.location is None:
             Console(stderr=True).print('No filter was provided.\nUse --help for more info.')
             raise typer.Exit()
 
     def build_headers(self):
         path = Path('ldi_cookie.txt')
         if path.is_file():
             self.headers['Cookie'] = path.open(mode='r').read()
 
-    def build_judgments_directory_path(self):
+    def build_scraped_judgments_directory_path(self):
         filters_to_join = [self.judicial_bodies, self.sections, self.location]
-        directory = '_'.join(
+        joined_filters = '_'.join(
             ['&'.join(filter.split(',')).replace(' ', '').lower() for filter in filters_to_join if filter is not None])
 
-        self.judgment_directory_path = Path('/'.join((self.path, directory)))
+        directory_name = '_'.join([joined_filters, datetime.now().strftime('%Y%m%d%H%M%S')])
+
+        self.judgment_directory_path = Path('/'.join([self.path, directory_name]))
         self.judgment_directory_path.mkdir(exist_ok=True, parents=True)
 
     def build_search_query(self):
         base_query = """{"mode":"AND","items":[{"mode":"AND","items":[{"field":"operasez","mode":"IN","value":["60","46","47","55","78","59","07"]},{"field":"tipo","mode":"EQUAL","value":"giurisprudenza/sentenze"}]}]}"""
         if self.judicial_bodies is not None:
             base_query = base_query[
                          :-2] + ''',{"field":"giuri_ente","mode":"IN","value":[''' + ','.join(
-                f'"{item}"' for item in self.judicial_bodies.split(",")) + ''']}''' + base_query[
-                                                                                      -2:]
+                f'"{item}"' for item in self.judicial_bodies.split(",")) + ''']}''' + base_query[-2:]
         if self.sections is not None:
             base_query = base_query[
                          :-2] + ''',{"field":"giuri_sezione","mode":"IN","value":[''' + ','.join(
-                f'"{item}"' for item in self.sections.split(",")) + ''']}''' + base_query[
-                                                                               -2:]
+                f'"{item}"' for item in self.sections.split(",")) + ''']}''' + base_query[-2:]
         if self.location is not None:
             base_query = base_query[
                          :-2] + ''',{"field":"localita_ft","mode":"EQUAL","value":"''' + self.location + '''"}''' + base_query[
                                                                                                                     -2:]
         self.search_judgment_params['query'] = base_query
 
+    def load_comuni(self):
+        self.comuni = pd.read_csv('scrapse/leggitalia/comuni.txt', header=None)[0].str.lower().tolist()
+
     def pagination_query(self, page):
         self.search_judgment_params['start'] = page[0]
         self.search_judgment_params['rows'] = page[1]
         return self.search_judgment_params
 
     def build_export_query(self, ids):
         self.export_judgment_params['ids'] = ids
```

### Comparing `scrapse-0.3.8/scrapse/main.py` & `scrapse-0.3.9/scrapse/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import typer
 
 from typing import Optional
 from pathlib import Path
 from scrapse.leggitalia.leggitalia import leggitalia_app
+#from scrapse.judgment.judgment import judgment_app
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 app = typer.Typer()
 app.add_typer(leggitalia_app, name='leggitalia')
+#app.add_typer(judgment_app, name='judgment')
 
 
 def version_callback(value: bool):
     if value:
         print(f"ScrapSE {__version__}")
         raise typer.Exit()
```

### Comparing `scrapse-0.3.8/PKG-INFO` & `scrapse-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: scrapse
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package to download and manage judgments
 Home-page: https://gitlab.di.unito.it/ngupp/ngupp-scrapse
 Keywords: scraping,judgments
 Author: zaharia laurentiu jr marius
 Author-email: zaharialorenzo@gmail.com
 Maintainer: zaharia laurentiu jr marius
 Maintainer-email: zaharialorenzo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: docx (>=0.2.4,<0.3.0)
+Requires-Dist: docx2txt (>=0.8,<0.9)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: spacy (>=3.5.1,<4.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://gitlab.di.unito.it/ngupp/ngupp-scrapse
 Description-Content-Type: text/markdown
 
 # ScrapSE
 
 ## Package description
```

