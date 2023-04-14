# Comparing `tmp/mathtranslate-2.1.8.tar.gz` & `tmp/mathtranslate-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.1.8.tar", last modified: Sun Apr  2 20:01:09 2023, max compression
+gzip compressed data, was "mathtranslate-2.1.9.tar", last modified: Mon Apr  3 02:34:30 2023, max compression
```

## Comparing `mathtranslate-2.1.8.tar` & `mathtranslate-2.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:01:09.841297 mathtranslate-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-02 20:01:09.841297 mathtranslate-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:01:09.841297 mathtranslate-2.1.8/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/tencent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/mathtranslate/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:01:09.841297 mathtranslate-2.1.8/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-02 20:01:09.000000 mathtranslate-2.1.8/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 20:01:09.841297 mathtranslate-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-02 20:00:50.000000 mathtranslate-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/setup.py
```

### Comparing `mathtranslate-2.1.8/LICENSE` & `mathtranslate-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.8/PKG-INFO` & `mathtranslate-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.1.8
+Version: 2.1.9
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: Jiace Sun
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.8 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.9 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 Jiace Sun Author-email: susyustc@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE # MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
                                   [logo.jpg]
```

### Comparing `mathtranslate-2.1.8/README.md` & `mathtranslate-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.8/mathtranslate/config.py` & `mathtranslate-2.1.9/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.8/mathtranslate/process_latex.py` & `mathtranslate-2.1.9/mathtranslate/process_latex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import re
 import regex
 from .config import math_code, test_environment
 
 match_code = r"(" + math_code + r"_\d+(?:_\d+)*)"
 match_code_replace = math_code + r"_(\d+(?:_\d+)*)*"
 
-options = r"\[[a-zA-Z\s,\\\*\.\+\-=_{}]*?\]"  # ,\*.+-=_{}
+#options = r"\[[a-zA-Z\s,\\\*\.\+\-=_{}\(\)\!]*?\]"  # ,\*.+-=_{}!
+options = r"\[.*?\]"
+spaces = r"[ \t]*"
+
+get_pattern_brace = lambda index: rf"\{{((?:[^{{}}]++|(?{index}))++)\}}"
+get_pattern_env = lambda name: rf"\\begin{spaces}\{{({name})\}}{spaces}({options})?(.*?)\\end{spaces}\{{\1\}}".replace('options', options)
+get_pattern_command_full = lambda name: rf'\\({name}){spaces}({options})?{spaces}({get_pattern_brace(3)})'
+match_command_name = r'[a-zA-Z]+\*?'
+
+pattern_env = get_pattern_env(r'.*?')  # \begin{xxx} \end{xxx}, group 1: name, group 2: option, group 3: content
+pattern_command_full = get_pattern_command_full(match_command_name)   # \xxx[xxx]{xxx} and \xxx{xxx}, group 1: name, group 2: option, group 4: content
+pattern_command_simple = rf'\\({match_command_name})'  # \xxx, group 1: name
+pattern_brace = get_pattern_brace(0)  # {xxx}, group 1: content
 
-pattern_env = r"\\begin[ \t]*\{(.*?)\}[ \t]*(options)?(.*?)\\end[ \t]*\{\1\}".replace('options', options)  # \begin{xxx} \end{xxx}, group 1: name, group 2: option, group 3: content
-pattern_command_full = r"\\([a-zA-Z]+\*?)[ \t]*(options)?[ \t]*(\{((?:[^{}]++|(?3))++)\})".replace('options', options)   # \xxx[xxx]{xxx} and \xxx{xxx}, group 1: name, group 2: option, group 4: content
-pattern_command_simple = r"\\([a-zA-Z]+\*?)"  # \xxx, group 1: name
-pattern_brace = r"\{((?:[^{}]++|(?0))++)\}"  # {xxx}, group 1: content
 pattern_theorem = r"\\newtheorem[ \t]*\{(.+?)\}"  # \newtheorem{xxx}, group 1: name
 pattern_accent = r"\\([`'\"^~=.])(?:\{([a-zA-Z])\}|([a-zA-Z]))"  # match special characters with accents, group 1: accent, group 2/3: normal character
 match_code_accent = rf'{math_code}([A-Z]{{2}})([a-zA-Z])'  # group 1: accent name, group 2: normal character
 list_special = ['\\', '%', '&', '#', '$', '{', '}', ' ']  # all special characters in form of \x
 
 special_character_forward = {
     '\\': 'BS',
@@ -130,17 +138,15 @@
         total_num += num_modify
         if num_modify == 0:
             break
     n_good = len(set(matched_indices).intersection(set(range(nobjs))))
     n_bad1 = len(matched_indices) - n_good
     n_bad2 = nobjs - n_good
     n_bad = max(n_bad1, n_bad2)
-    if final and n_bad > 0:
-        print(n_bad, 'latex objects are probably wrong in total', nobjs)
-    return text
+    return text, n_bad, nobjs
 
 
 def remove_tex_comments(text):
     """
     Removes all TeX comments in a given string with the format "% comment text".
     Does not match "\%".
     If "%" is at the beginning of a line then delete this line.
@@ -163,47 +169,43 @@
         assert False, "latex is not complete"
     pre = text[:begin_doc_index + len(begin_code)]
     body = text[begin_doc_index + len(begin_code):end_doc_index]
     post = text[end_doc_index:]
     return body, pre, post
 
 
-def process_specific_env(latex, function, env_names):
-    pattern = regex.compile(pattern_env, regex.DOTALL)
+def process_specific_env(latex, function, env_name):
+    pattern = regex.compile(get_pattern_env(env_name), regex.DOTALL)
 
     def process_function(match):
-        # \begin{env_name} content \end{env_name}
-        env_name = match.group(1)
+        # \begin{env_name}[options] content \end{env_name}
+        name = match.group(1)
+        assert re.match(env_name, name)
         options = match.group(2)
         if options is None:
             options = ''
         content = match.group(3)
-        if env_name in env_names:
-            processed_content = function(content)
-            return rf'\begin{{{env_name}}}{options}{processed_content}\end{{{env_name}}}'
-        else:
-            return match.group(0)
+        processed_content = function(content)
+        return rf'\begin{{{env_name}}}{options}{processed_content}\end{{{env_name}}}'
     return pattern.sub(process_function, latex)
 
 
-def process_specific_commands(latex, function, command_names):
-    pattern = regex.compile(pattern_command_full, regex.DOTALL)
+def process_specific_command(latex, function, command_name):
+    pattern = regex.compile(get_pattern_command_full(command_name), regex.DOTALL)
 
     def process_function(match):
         # \{command_name}[options]{content}
-        command_name = match.group(1)
+        name = match.group(1)
+        assert re.match(command_name, name)
         options = match.group(2)
         if options is None:
             options = ''
         content = match.group(4)
-        if command_name in command_names:
-            processed_content = function(content)
-            return rf'\{command_name}{options}{{{processed_content}}}'
-        else:
-            return match.group(0)
+        processed_content = function(content)
+        return rf'\{command_name}{options}{{{processed_content}}}'
     return pattern.sub(process_function, latex)
 
 
 def remove_blank_lines(text):
     pattern = re.compile(r'\n\n+')
     text = pattern.sub('\n', text)
     return text
@@ -295,18 +297,19 @@
         return rf'\{special}{{{char}}}'
 
     text = re.compile(match_code_accent).sub(replace_function, text)
 
     return text
 
 
-def combine_sentences(text):
-    pattern = re.compile(r'\n(\s*([^\s]))')
+def combine_split_to_sentences(text):
+    n = len(math_code)
+    pattern = re.compile(r'\n(\s*([^\s]+))')
 
     def process_function(match):
-        char = match.group(2)
-        if char == '\\':
+        string = match.group(2)
+        if string[0:n] == math_code:
             return match.group(0)
         else:
             return ' '+match.group(1)
 
     return pattern.sub(process_function, text)
```

### Comparing `mathtranslate-2.1.8/mathtranslate/process_text.py` & `mathtranslate-2.1.9/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.8/mathtranslate/tencent.py` & `mathtranslate-2.1.9/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.8/mathtranslate/translate.py` & `mathtranslate-2.1.9/mathtranslate/translate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/env python
 from . import process_latex
 from . import process_text
-from .config import math_code
 from .process_text import char_limit
 import time
 import re
+import tqdm
 
 default_begin = r'''
 \documentclass[UTF8]{article}
 \usepackage{xeCJK}
 \usepackage{amsmath,amssymb}
 \begin{document}
 '''
 default_end = r'''
 \end{document}
 '''
 
+# TODO: add more here
+environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof']
+command_list = ['section', 'subsection', 'subsubsection', 'caption', 'subcaption', 'footnote', 'paragraph']
+
 
 class TextTranslator:
     def __init__(self, engine, language_to, language_from):
         if engine == 'google':
             import mtranslate as translator
         elif engine == 'tencent':
             from mathtranslate.tencent import Translator
@@ -39,16 +43,15 @@
             return text
         while True:
             try:
                 result = self.try_translate(text)
                 break
             except BaseException as e:
                 if hasattr(self.translator, "is_error_request_frequency") and self.translator.is_error_request_frequency(e):
-                    print("sleep 1 second to wait")
-                    time.sleep(1)
+                    time.sleep(0.5)
                 else:
                     raise e
         return result
 
 
 class LatexTranslator:
     def __init__(self, translator: TextTranslator, debug=False):
@@ -84,132 +87,117 @@
         parts.append(part)
         parts_translated = []
         for part in parts:
             parts_translated.append(self.translator.translate(part))
         text_translated = '\n'.join(parts_translated)
         return text_translated.replace("\u200b", "")
 
-    def translate_paragraph_latex(self, latex_original_paragraph, num, complete):
+    def translate_paragraph_latex(self, latex_original_paragraph):
         '''
         Translate a latex paragraph, which means that it could contain latex objects
         '''
-        latex_original_paragraph = process_latex.combine_sentences(latex_original_paragraph)
         text_original_paragraph, objs = process_latex.replace_latex_objects(latex_original_paragraph)
         # Since \n is equivalent to space in latex, we change \n back to space
         # otherwise the translators view them as separate sentences
+        text_original_paragraph = process_latex.combine_split_to_sentences(text_original_paragraph)
         text_original_paragraph = process_text.split_too_long_paragraphs(text_original_paragraph)
-        if not complete:
+        if not self.complete:
             text_original_paragraph = process_text.split_titles(text_original_paragraph)
+        # Remove additional space
         text_original_paragraph = re.sub(r'  +', ' ', text_original_paragraph)
         if self.debug:
-            print(f'\n\nParagraph {num}\n\n', file=self.f_old)
+            print(f'\n\nParagraph {self.num}\n\n', file=self.f_old)
             print(text_original_paragraph, file=self.f_old)
         text_translated_paragraph = self.translate_paragraph_text(text_original_paragraph)
         if self.debug:
-            print(f'\n\nParagraph {num}\n\n', file=self.f_new)
+            print(f'\n\nParagraph {self.num}\n\n', file=self.f_new)
             print(text_translated_paragraph, file=self.f_new)
-            print(f'\n\nParagraph {num}\n\n', file=self.f_obj)
+            print(f'\n\nParagraph {self.num}\n\n', file=self.f_obj)
             for i, obj in enumerate(objs):
                 print(f'obj {i}', file=self.f_obj)
                 print(obj, file=self.f_obj)
-        latex_translated_paragraph = process_latex.recover_latex_objects(text_translated_paragraph, objs, final=True)
+        latex_translated_paragraph, nbad, ntotal = process_latex.recover_latex_objects(text_translated_paragraph, objs, final=True)
+        self.nbad += nbad
+        self.ntotal += ntotal
         return latex_translated_paragraph
 
     def split_latex_to_paragraphs(self, latex):
         '''
         1. convert latex to text and objects
         2. split text
         3. convert text back to objects
         '''
         text, objs = process_latex.replace_latex_objects(latex)
         paragraphs_text = re.split(r'\n\n+', text)
-        paragraphs_latex = [process_latex.recover_latex_objects(paragraph_text, objs) for paragraph_text in paragraphs_text]
+        paragraphs_latex = [process_latex.recover_latex_objects(paragraph_text, objs)[0] for paragraph_text in paragraphs_text]
         return paragraphs_latex
 
-    def _translate_latex_objects(self, match_function, latex_original, names, complete):
+    def translate_latex_all_objects(self, latex, envs, commands):
         '''
         Terminology:
         env: '\\begin{xxx} \\end{xxx}'
         command: '\\command[options]{text}
         object: env or command
         '''
-        latex_translated = latex_original
-
-        num = 0
-
-        def translate_function(latex):
-            # Translate anything inside an environment or command
-            nonlocal num
-            result = self.translate_paragraph_latex(latex, num, complete)
-            num += 1
-            print(num)
-            return result
-
-        names = names + [item + '*' for item in names]
-        latex_translated = match_function(latex_translated, translate_function, names)
-        return latex_translated
-
-    def translate_latex_env(self, latex_original, names, complete):
-        return self._translate_latex_objects(process_latex.process_specific_env, latex_original, names, complete)
-
-    def translate_latex_commands(self, latex_original, names, complete):
-        return self._translate_latex_objects(process_latex.process_specific_commands, latex_original, names, complete)
+        for env_name in envs:
+            latex = process_latex.process_specific_env(latex, self.translate_paragraph_latex, env_name)
+            latex = process_latex.process_specific_env(latex, self.translate_paragraph_latex, env_name + r'\*')
+        for command_name in commands:
+            latex = process_latex.process_specific_command(latex, self.translate_paragraph_latex, command_name)
+            latex = process_latex.process_specific_command(latex, self.translate_paragraph_latex, command_name + r'\*')
+        return latex
+
+    def translate_full_latex(self, latex_original):
+        self.nbad = 0
+        self.ntotal = 0
 
-    def translate_full_latex(self, latex_original, loadmain=False):
         latex_original = process_latex.remove_tex_comments(latex_original)
 
         latex_original = process_latex.replace_accent(latex_original)
         latex_original = process_latex.replace_special(latex_original)
 
-        complete = process_latex.is_complete(latex_original)
+        self.complete = process_latex.is_complete(latex_original)
         theorems = process_latex.get_theorems(latex_original)
-        if complete:
+        if self.complete:
             print('It is a full latex document')
             latex_original, tex_begin, tex_end = process_latex.split_latex_document(latex_original, r'\begin{document}', r'\end{document}')
             tex_begin = process_latex.remove_blank_lines(tex_begin)
             # TODO: change xeCJK to be compatible with other compiler & languages
             tex_begin = process_latex.insert_macro(tex_begin, r'\usepackage{xeCJK}')
         else:
             print('It is not a full latex document')
             latex_original = process_text.connect_paragraphs(latex_original)
             tex_begin = default_begin
             tex_end = default_end
 
-        if loadmain:
-            latex_translated = open('text_after_main.txt').read()
-        else:
-            latex_original_paragraphs = self.split_latex_to_paragraphs(latex_original)
-            latex_translated_paragraphs = []
+        latex_original_paragraphs = self.split_latex_to_paragraphs(latex_original)
+        latex_translated_paragraphs = []
 
-            num = 0
-            print('processing main text')
-            for latex_original_paragraph in latex_original_paragraphs:
-                latex_translated_paragraph = self.translate_paragraph_latex(latex_original_paragraph, num, complete)
+        self.num = 0
+        for latex_original_paragraph in tqdm.tqdm(latex_original_paragraphs):
+            try:
+                latex_translated_paragraph = self.translate_paragraph_latex(latex_original_paragraph)
+                latex_translated_paragraph = self.translate_latex_all_objects(latex_translated_paragraph, environment_list + theorems, command_list)
                 latex_translated_paragraphs.append(latex_translated_paragraph)
-                print(num, '/', len(latex_original_paragraphs))
-                num += 1
-
-            latex_translated = '\n\n'.join(latex_translated_paragraphs)
-
-            if self.debug:
-                print(latex_translated, file=open('text_after_main.txt', 'w'))
+            except BaseException as e:
+                print('Error found in Parapragh', self.num)
+                print('Content')
+                print(latex_original_paragraph)
+                raise e
+            self.num += 1
 
-        # TODO: add more here
-        environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof']
-        print('processing latex environments')
-        latex_translated = self.translate_latex_env(latex_translated, environment_list + theorems, complete)
-
-        command_list = ['section', 'subsection', 'subsubsection', 'caption', 'subcaption', 'footnote', 'paragraph']
-        print('processing latex commands')
-        latex_translated = self.translate_latex_commands(latex_translated, command_list, complete)
+        latex_translated = '\n\n'.join(latex_translated_paragraphs)
 
         latex_translated = tex_begin + '\n' + latex_translated + '\n' + tex_end
 
         # Title is probably outside the body part
-        print('processing title')
-        latex_translated = self.translate_latex_commands(latex_translated, ['title'], complete)
+        self.num = 'title'
+        latex_translated = process_latex.process_specific_command(latex_translated, self.translate_paragraph_latex, 'title')
 
         latex_translated = process_latex.recover_special(latex_translated)
         latex_translated = process_latex.recover_accent(latex_translated)
 
         self.close()
+
+        print(self.ntotal - self.nbad, '/',  self.ntotal, 'latex object are correctly translated')
+
         return latex_translated
```

### Comparing `mathtranslate-2.1.8/mathtranslate/translate_tex.py` & `mathtranslate-2.1.9/mathtranslate/translate_tex.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     parser.add_argument("-engine", default=default_engine, help=f'translation engine, avaiable options include google and tencent. default is {default_engine}')
     parser.add_argument("-from", default=default_language_from, dest='l_from', help=f'language from, default is {default_language_from}')
     parser.add_argument("-to", default=default_language_to, dest='l_to', help=f'language to, default is {default_language_to}')
     parser.add_argument("--list", action='store_true', help='list codes for languages')
     parser.add_argument("--setkey", action='store_true', help='set id and key of tencent translator')
     parser.add_argument("--setdefault", action='store_true', help='set default translation engine and languages')
     parser.add_argument("--debug", action='store_true')
-    parser.add_argument("--loadmain", action='store_true')
     parser.add_argument("--compile", action='store_true')
     options = parser.parse_args()
 
     if options.setkey:
         print('Tencent secretID')
         config.set_variable(config.tencent_secret_id_path, config.tencent_secret_id_default)
         print('Tencent secretKey')
@@ -162,15 +161,15 @@
         output_path = options.o
 
     text_translator = TextTranslator(options.engine, options.l_to, options.l_from)
     latex_translator = LatexTranslator(text_translator, options.debug)
 
     input_encoding = get_file_encoding(input_path)
     text_original = open(input_path, encoding=input_encoding).read()
-    text_final = latex_translator.translate_full_latex(text_original, options.loadmain)
+    text_final = latex_translator.translate_full_latex(text_original)
     with open(output_path, "w", encoding='utf-8') as file:
         print(text_final, file=file)
     print(output_path, 'is generated')
 
     if options.compile:
         os.system(f'xelatex {output_path}')
     else:
```

### Comparing `mathtranslate-2.1.8/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.1.9/mathtranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.1.8
+Version: 2.1.9
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: Jiace Sun
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.8 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.9 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 Jiace Sun Author-email: susyustc@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE # MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
                                   [logo.jpg]
```

### Comparing `mathtranslate-2.1.8/setup.py` & `mathtranslate-2.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["mtranslate",
                       "tencentcloud-sdk-python",
                       "chardet",
                       "requests",
                       "regex",
+                      "tqdm",
                       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
```

