# Comparing `tmp/qlcpy-1.0.4.tar.gz` & `tmp/qlcpy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlcpy-1.0.4.tar", last modified: Mon Nov 28 14:38:24 2022, max compression
+gzip compressed data, was "qlcpy-1.0.9.tar", last modified: Sun Jan  8 21:57:52 2023, max compression
```

## Comparing `qlcpy-1.0.4.tar` & `qlcpy-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1071 2022-11-12 12:54:28.000000 qlcpy-1.0.4/LICENSE
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1342 2022-11-28 14:38:24.313147 qlcpy-1.0.4/PKG-INFO
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      892 2022-11-25 17:29:58.000000 qlcpy-1.0.4/README.md
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      102 2022-11-25 12:27:29.000000 qlcpy-1.0.4/pyproject.toml
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/qlcpy/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1777 2022-11-28 14:35:24.000000 qlcpy-1.0.4/qlcpy/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       55 2022-11-22 17:09:48.000000 qlcpy-1.0.4/qlcpy/__main__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1590 2022-11-28 12:58:13.000000 qlcpy-1.0.4/qlcpy/arrays.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1410 2022-11-28 12:44:18.000000 qlcpy-1.0.4/qlcpy/generator.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/qlcpy/i18n/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      257 2022-11-28 10:13:02.000000 qlcpy-1.0.4/qlcpy/i18n/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2461 2022-11-27 14:09:07.000000 qlcpy-1.0.4/qlcpy/i18n/en.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2485 2022-11-27 14:08:54.000000 qlcpy-1.0.4/qlcpy/i18n/fi.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/qlcpy/instrument/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1482 2022-11-27 04:24:53.000000 qlcpy-1.0.4/qlcpy/instrument/Instrumentor.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2285 2022-11-26 06:48:45.000000 qlcpy-1.0.4/qlcpy/instrument/ProgramData.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1453 2022-11-22 15:04:31.000000 qlcpy-1.0.4/qlcpy/instrument/TransformAST.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4994 2022-11-24 06:23:14.000000 qlcpy-1.0.4/qlcpy/instrument/TransformForInstrumentor.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      761 2022-11-12 01:52:46.000000 qlcpy-1.0.4/qlcpy/instrument/WalkAST.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      531 2022-11-23 08:02:20.000000 qlcpy-1.0.4/qlcpy/instrument/WalkFind.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3529 2022-11-22 13:41:43.000000 qlcpy-1.0.4/qlcpy/instrument/WalkNames.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1516 2022-11-28 14:31:24.000000 qlcpy-1.0.4/qlcpy/instrument/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      906 2022-11-27 04:25:18.000000 qlcpy-1.0.4/qlcpy/instrument/trees.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1626 2022-11-28 12:45:02.000000 qlcpy-1.0.4/qlcpy/models.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      650 2022-11-27 04:29:28.000000 qlcpy-1.0.4/qlcpy/primitives.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/qlcpy/questions/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      887 2022-11-24 05:47:52.000000 qlcpy-1.0.4/qlcpy/questions/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2555 2022-11-28 13:00:03.000000 qlcpy-1.0.4/qlcpy/questions/dynamic.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2472 2022-11-27 00:05:54.000000 qlcpy-1.0.4/qlcpy/questions/lines.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1884 2022-11-23 09:49:25.000000 qlcpy-1.0.4/qlcpy/questions/options.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/qlcpy.egg-info/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1342 2022-11-28 14:38:24.000000 qlcpy-1.0.4/qlcpy.egg-info/PKG-INFO
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      816 2022-11-28 14:38:24.000000 qlcpy-1.0.4/qlcpy.egg-info/SOURCES.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)        1 2022-11-28 14:38:24.000000 qlcpy-1.0.4/qlcpy.egg-info/dependency_links.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       37 2022-11-28 14:38:24.000000 qlcpy-1.0.4/qlcpy.egg-info/entry_points.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)        6 2022-11-28 14:38:24.000000 qlcpy-1.0.4/qlcpy.egg-info/top_level.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      621 2022-11-28 14:38:24.317147 qlcpy-1.0.4/setup.cfg
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2022-11-28 14:38:24.313147 qlcpy-1.0.4/test/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1398 2022-11-26 06:38:34.000000 qlcpy-1.0.4/test/test_instrumentor.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      581 2022-11-26 06:38:41.000000 qlcpy-1.0.4/test/test_printer.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1970 2022-11-26 06:49:51.000000 qlcpy-1.0.4/test/test_transform.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.316547 qlcpy-1.0.9/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1071 2022-11-12 12:54:28.000000 qlcpy-1.0.9/LICENSE
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1342 2023-01-08 21:57:52.316547 qlcpy-1.0.9/PKG-INFO
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      892 2022-11-25 17:29:58.000000 qlcpy-1.0.9/README.md
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      102 2022-11-25 12:27:29.000000 qlcpy-1.0.9/pyproject.toml
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/qlcpy/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2121 2023-01-08 21:53:17.000000 qlcpy-1.0.9/qlcpy/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)       55 2022-11-22 17:09:48.000000 qlcpy-1.0.9/qlcpy/__main__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      547 2023-01-08 20:01:52.000000 qlcpy-1.0.9/qlcpy/arrays.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1602 2023-01-08 21:53:38.000000 qlcpy-1.0.9/qlcpy/generator.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/qlcpy/i18n/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      257 2022-11-28 10:13:02.000000 qlcpy-1.0.9/qlcpy/i18n/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3208 2023-01-08 20:30:19.000000 qlcpy-1.0.9/qlcpy/i18n/en.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3279 2023-01-08 20:31:09.000000 qlcpy-1.0.9/qlcpy/i18n/fi.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/qlcpy/instrument/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1471 2023-01-08 19:17:57.000000 qlcpy-1.0.9/qlcpy/instrument/Instrumentor.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2490 2023-01-08 19:28:48.000000 qlcpy-1.0.9/qlcpy/instrument/ProgramData.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1453 2022-11-22 15:04:31.000000 qlcpy-1.0.9/qlcpy/instrument/TransformAST.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4994 2023-01-08 19:17:57.000000 qlcpy-1.0.9/qlcpy/instrument/TransformForInstrumentor.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      761 2022-11-12 01:52:46.000000 qlcpy-1.0.9/qlcpy/instrument/WalkAST.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      531 2022-11-23 08:02:20.000000 qlcpy-1.0.9/qlcpy/instrument/WalkFind.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3529 2022-11-22 13:41:43.000000 qlcpy-1.0.9/qlcpy/instrument/WalkNames.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1676 2023-01-08 21:47:06.000000 qlcpy-1.0.9/qlcpy/instrument/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      543 2023-01-08 11:58:13.000000 qlcpy-1.0.9/qlcpy/instrument/trees.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1684 2023-01-08 10:34:47.000000 qlcpy-1.0.9/qlcpy/models.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      834 2023-01-08 15:24:48.000000 qlcpy-1.0.9/qlcpy/primitives.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/qlcpy/questions/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      944 2023-01-08 12:44:02.000000 qlcpy-1.0.9/qlcpy/questions/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4028 2023-01-08 20:32:46.000000 qlcpy-1.0.9/qlcpy/questions/dynamic.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2742 2023-01-08 19:23:00.000000 qlcpy-1.0.9/qlcpy/questions/lines.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1967 2023-01-08 15:12:50.000000 qlcpy-1.0.9/qlcpy/questions/options.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/qlcpy.egg-info/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1342 2023-01-08 21:57:52.000000 qlcpy-1.0.9/qlcpy.egg-info/PKG-INFO
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      816 2023-01-08 21:57:52.000000 qlcpy-1.0.9/qlcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)        1 2023-01-08 21:57:52.000000 qlcpy-1.0.9/qlcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)       37 2023-01-08 21:57:52.000000 qlcpy-1.0.9/qlcpy.egg-info/entry_points.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)        6 2023-01-08 21:57:52.000000 qlcpy-1.0.9/qlcpy.egg-info/top_level.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      621 2023-01-08 21:57:52.316547 qlcpy-1.0.9/setup.cfg
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-01-08 21:57:52.312547 qlcpy-1.0.9/test/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1398 2022-11-26 06:38:34.000000 qlcpy-1.0.9/test/test_instrumentor.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      581 2022-11-26 06:38:41.000000 qlcpy-1.0.9/test/test_printer.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1970 2023-01-08 09:40:33.000000 qlcpy-1.0.9/test/test_transform.py
```

### Comparing `qlcpy-1.0.4/LICENSE` & `qlcpy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/PKG-INFO` & `qlcpy-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlcpy
-Version: 1.0.4
+Version: 1.0.9
 Summary: Generates questions about given Python program
 Home-page: https://github.com/teemulehtinen/qlcpy
 Author: Teemu Lehtinen
 Author-email: teemu.t.lehtinen@aalto.fi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qlcpy-1.0.4/README.md` & `qlcpy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/__init__.py` & `qlcpy-1.0.9/qlcpy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,23 @@
     return f.read()
 
 def main():
   parser = argparse.ArgumentParser(
     description='QLCpy generates questions that target analysed facts about the given program'
   )
   parser.add_argument('program', nargs='?', default=None, help='A python program file')
+  parser.add_argument('-m', '--main', action='store_true', help='Run with "__name__" = "__main__"')
   parser.add_argument('-c', '--call', help='A python call to execute')
+  parser.add_argument(
+    '-sc',
+    '--silent-call',
+    help='A python call to execute silently without including it in the question prompts'
+  )
   parser.add_argument('-i', '--input', help='A text file to use as stdin')
-  parser.add_argument('-n', default=3, help='Number of questions (at maximum)')
+  parser.add_argument('-n', type=int, default=3, help='Number of questions (at maximum)')
   parser.add_argument('-t', '--types', nargs='+', help='Only these question types')
   parser.add_argument('-u', '--unique', action='store_true', help='Only unique question types')
   parser.add_argument('-l', '--lang', help='Language code for the text (en, fi)')
   parser.add_argument('--json', action='store_true', help='Print question data as JSON')
   parser.add_argument('--list-types', action='store_true', help='List available question types')
   args = parser.parse_args()
 
@@ -29,25 +35,28 @@
     print('Available QLC types:')
     for t in TEMPLATES:
       print(f'* {t.type:<25} {t.description}')
     parser.exit()
 
   if not args.program:
     parser.print_usage()
-    parser.exit()
-  with open(args.program, 'r') as f:
-    tree = ast.parse(f.read())
+    parser.exit()  
+  tree = ast.parse(_read_file(args.program))
 
   if args.lang:
     i18n.lang = args.lang
 
+  
+
   qlcs = generate(
     tree,
     [QLCRequest(args.n, types=args.types, unique_types=args.unique)],
-    args.call,
-    _read_file(args.input) if args.input else ""
+    call=args.call or args.silent_call,
+    input=_read_file(args.input) if args.input else "",
+    run_main=args.main,
+    silent_call=not args.silent_call is None,
   )
 
   if args.json:
     print(json.dumps(list(qlc.to_dict() for qlc in qlcs)))
   else:
     print('\n\n'.join(str(qlc) for qlc in qlcs))
```

### Comparing `qlcpy-1.0.4/qlcpy/generator.py` & `qlcpy-1.0.9/qlcpy/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,20 +14,25 @@
     select.update(r.types)
   return list(t for t in TEMPLATES if t.type in select)
 
 def generate(
   src: str,
   requests: Optional[List[QLCRequest]] = None,
   call: Optional[str] = None,
-  input: Optional[str] = None
+  input: Optional[str] = None,
+  run_main: bool = False,
+  silent_call: bool = False,
 ) -> List[QLC]:
   tree = ast.parse(src)
-  instrumentor = run_with_instrumentor(tree, parse_body(call), input)
+  call = call.replace('\\n', '\n') if call else None
+  instrumentor = run_with_instrumentor(tree, parse_body(call), input, run_main)
   prepared = list(
-    p for t in select_templates(requests) for p in t.maker(t.type, tree, call, instrumentor)
+    p
+    for t in select_templates(requests)
+    for p in t.maker(t.pos, t.type, tree, None if silent_call else call, instrumentor)
   )
   out: List[QLC] = []
   for r in requests:
     n = r.count - len(out) if r.fill else r.count
     while n > 0 and len(prepared) > 0:
       sample = prepared if r.types is None else list(p for p in prepared if p.type in r.types)
       picked = random.choice(sample) if sample else None
@@ -37,8 +42,8 @@
           prepared = list(p for p in prepared if p.type != picked.type)
         else:
           prepared = list(p for p in prepared if p != picked)
         if qlc is None:
           continue
         out.append(qlc)
       n -= 1
-  return out
+  return sorted(out, key=lambda qlc: qlc.pos)
```

### Comparing `qlcpy-1.0.4/qlcpy/i18n/en.py` & `qlcpy-1.0.9/qlcpy/i18n/en.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,23 +33,37 @@
     ),
   'q_loop_count_call':
     lambda line, call: (
       f'Line {line} has a loop structure. How many times does the loop execute '
       f'when running <em>{call}</em>?'
     ),
   'o_loop_count_correct': 'Correct, this is the number of times the loop executed.',
+  'o_loop_count_one_off': 'This number is off by one.',
   'o_loop_count_random': 'This is an incorrect, random number.',
 
   'q_variable_trace':
     lambda id, line: (
       f'Line {line} declares a variable named <em>{id}</em>. Which values and in which '
       'order are assigned to the variable when the program is run?'
     ),
   'q_variable_trace_call':
     lambda id, line, call: (
       f'Line {line} declares a variable named <em>{id}</em>. Which values and in which '
       f'order are assigned to the variable when running <em>{call}</em>?'
     ),
-  'o_variable_trace_correct': 'Correct, these values where assigned in this order to the variable.',
+  'o_variable_trace_correct': 'Correct, these values were assigned in this order to the variable.',
   'o_variable_trace_miss': 'This sequence is missing a value that was assigned to the variable.',
   'o_variable_trace_random': 'This is an incorrect, random sequence of values.',
+
+  'q_variable_trace_start':
+    lambda id, line: (
+      f'Line {line} declares a variable named <em>{id}</em>. Which are the first 4 values '
+      'that are assigned to the variable in the given order when the program is run?'
+    ),
+  'q_variable_trace_start_call':
+    lambda id, line, call: (
+      f'Line {line} declares a variable named <em>{id}</em>. Which are the first 4 values '
+      f'that are assigned to the variable in the given order when running <em>{call}</em>?'
+    ),
+  'o_variable_trace_start_correct': 'Correct, these 4 values where first assigned in this order to the variable.',
+  'o_variable_trace_start_random': 'This is an incorrect, random sequence of values.',
 }
```

### Comparing `qlcpy-1.0.4/qlcpy/i18n/fi.py` & `qlcpy-1.0.9/qlcpy/i18n/fi.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ),
   'q_loop_count_call':
     lambda line, call: (
       f'Rivillä {line} on toistorakenne. Kuinka monta kertaa toisto suoritetaan, '
       f'kun ajetaan <em>{call}</em>?'
     ),
   'o_loop_count_correct': 'Oikein, näin monta kertaa toisto tapahtui',
+  'o_loop_count_one_off': 'Tämä lukumäärä heittää yhdellä oikeasta.',
   'o_loop_count_random': 'Tämä on satunnainen väärä lukumäärä',
 
   'q_variable_trace':
     lambda id, line: (
       f'Rivillä {line} määritellään muuttuja <em>{id}</em>. Mitkä arvot ja missä ',
       'järjestyksessä siihen sijoitetaan, kun ohjelma ajetaan.'
     ),
@@ -48,8 +49,21 @@
     lambda id, line, call: (
       f'Rivillä {line} määritellään muuttuja <em>{id}</em>. Mitkä arvot ja missä järjestyksessä '
       f'siihen sijoitetaan, kun ajetaan <em>{call}</em>?'
     ),
   'o_variable_trace_correct': 'Oikein, nämä arvot sijoitettiin tässä järjestyksessä muuttujaan.',
   'o_variable_trace_miss': 'Tästä sarjasta puuttuu muuttujaan sijoitettu arvo.',
   'o_variable_trace_random': 'Tämä on satunnainen väärä arvojen sarja.',
+
+  'q_variable_trace_start':
+    lambda id, line: (
+      f'Rivillä {line} määritellään muuttuja <em>{id}</em>. Mitkä ovat 4 ensimmäistä arvoa, '
+      'jotka siihen sijoitetaan annetussa järjestyksessä, kun ohjelma ajetaan?'
+    ),
+  'q_variable_trace_start_call':
+    lambda id, line, call: (
+      f'Rivillä {line} määritellään muuttuja <em>{id}</em>. Mitkä ovat 4 ensimmäistä arvoa, '
+      f'jotka siihen sijoitetaan annetussa järjestyksessä, kun ajetaan <em>{call}</em>?'
+    ),
+  'o_variable_trace_start_correct': 'Oikein, ensimmäiseksi muuttujaan sijoitettiin nämä 4 arvoa tässä järjestyksessä.',
+  'o_variable_trace_start_random': 'Tämä on satunnainen väärä arvojen sarja.',
 }
```

### Comparing `qlcpy-1.0.4/qlcpy/instrument/Instrumentor.py` & `qlcpy-1.0.9/qlcpy/instrument/Instrumentor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Iterable, List, Optional
 
-from ..primitives import as_primitive
+from ..primitives import Primitive
 from .ProgramData import ProgramData
 
 class Instrumentor:
 
   def __init__(self, data: ProgramData):
     self.data = data
     self.errors: List[str] = []
 
   def val(self, target: Optional[int], value: Any) -> None:
     if target is None:
-      self.errors.append(f'Assignment of "{as_primitive(value)}" to unknown variable')
+      self.errors.append(f'Assignment of {Primitive(value)} to unknown variable')
     else:
-      self.data.element_n(target).value(as_primitive(value))
+      self.data.element_n(target).value(Primitive(value))
 
   def eval(self, target: Optional[int], branch: int) -> None:
     if target is None:
       self.errors.append(f'Evaluation of an unknown branch')
     else:
       self.data.element_n(target).evaluation(branch)
```

### Comparing `qlcpy-1.0.4/qlcpy/instrument/ProgramData.py` & `qlcpy-1.0.9/qlcpy/instrument/ProgramData.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from ast import AST
 from typing import Any, List, Optional
+from ..primitives import Primitive
 
 class ProgramData:
 
 	class Element:
 
 		def __init__(self, type: str, scope: int, id: str, declaration: Optional[AST]) -> None:
 			self.type = type
 			self.scope = scope
 			self.id = id
 			self.declaration = declaration
 			self.container_scope = None
 			self.references: List[AST] = []
-			self.values: List[Any] = []
+			self.values: List[Primitive] = []
 			self.evaluations: List[int] = []
 
 		def set_container_scope(self, scope: int) -> None:
 			self.container_scope = scope
 
 		def reference(self, node: AST) -> None:
 			self.references.append(node)
 		
-		def value(self, value: Any) -> None:
+		def value(self, value: Primitive) -> None:
 			self.values.append(value)
 
 		def evaluation(self, branch: int) -> None:
 			self.evaluations.append(branch)
 
 		def has_reference(self, node: AST) -> bool:
 			return node == self.declaration or node in self.references
@@ -65,10 +66,17 @@
 			if el.type in types:
 				yield el
 
 	def element_for_id(self, id: str) -> Element:
 		for el in self.elements:
 			if el.id == id:
 				return el
+		return None
 	
+	def element_for_scope(self, scope: int) -> Element:
+		for el in self.elements:
+			if el.container_scope == scope:
+				return el
+		return None
+
 	def __repr__(self) -> str:
 		return '\n'.join(str(el) for el in self.elements)
```

### Comparing `qlcpy-1.0.4/qlcpy/instrument/TransformAST.py` & `qlcpy-1.0.9/qlcpy/instrument/TransformAST.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/instrument/TransformForInstrumentor.py` & `qlcpy-1.0.9/qlcpy/instrument/TransformForInstrumentor.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/instrument/WalkAST.py` & `qlcpy-1.0.9/qlcpy/instrument/WalkAST.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/instrument/WalkFind.py` & `qlcpy-1.0.9/qlcpy/instrument/WalkFind.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/instrument/WalkNames.py` & `qlcpy-1.0.9/qlcpy/instrument/WalkNames.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/qlcpy/instrument/__init__.py` & `qlcpy-1.0.9/qlcpy/instrument/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,29 +17,39 @@
 
 def find_nodes(tree: AST, class_names: List[str]) -> List[AST]:
   return WalkFind().walk(tree, class_names)
 
 def transform(tree: AST, data: ProgramData, add: Optional[List[AST]]) -> AST:
   return TransformForInstrumentor(INSTRUMENT_NAME, TEMPORARY_NAME).transform(tree, data, add)
 
-def run(transformed: AST, data: ProgramData, input: Optional[str]) -> None:
+def run(
+  transformed: AST,
+  data: ProgramData,
+  input: Optional[str] = None,
+  run_main: bool = False,
+) -> None:
   instrumentor = Instrumentor(data)
+  locals = {
+    '__name__': '__main__' if run_main else 'builtins',
+    INSTRUMENT_NAME: instrumentor,
+  }
   with mock.patch('builtins.input', side_effect=(input or '').split('\n')) as input, \
       mock.patch('sys.stdout', new_callable=StringIO) as output, \
       mock.patch('sys.stderr', new_callable=StringIO) as errors:
-    exec(compile(transformed, '<string>', 'exec'), { INSTRUMENT_NAME: instrumentor })
+    exec(compile(transformed, '<string>', 'exec'), locals)
   return instrumentor
 
 def run_with_instrumentor(
   tree: AST,
   call: Optional[List[AST]] = None,
-  input: Optional[str] = None
+  input: Optional[str] = None,
+  run_main: bool = False,
 ) -> Instrumentor:
   data = collect_elements(tree)
   instrumented = transform(tree, data, call)
-  return run(instrumented, data, input)
+  return run(instrumented, data, input, run_main)
 
 def parse_body(call: Optional[str]):
   if call:
     mod = parse(call)
     return mod.body
   return None
```

### Comparing `qlcpy-1.0.4/qlcpy/models.py` & `qlcpy-1.0.9/qlcpy/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,16 @@
       'info': self.info,
     }
   
   def __repr__(self) -> str:
     return f'{"*" if self.correct  else " "} {self.answer}: {self.info} [{self.type}]'
 
 class QLC:
-  def __init__(self, type: str, question: str, options: List[QLCOption]):
+  def __init__(self, pos: int, type: str, question: str, options: List[QLCOption]):
+    self.pos = pos
     self.type = type
     self.question = question
     self.options = options
   
   def to_dict(self):
     return {
       'type': self.type,
@@ -54,12 +55,13 @@
       'options': list(o.to_dict() for o in self.options),
     }
 
   def __repr__(self) -> str:
     return '\n'.join([f'{self.question} [{self.type}]', *[str(o) for o in self.options]])
 
 class QLCPrepared:
-  def __init__(self, type: str):
+  def __init__(self, pos: int, type: str):
+    self.pos = pos
     self.type = type
 
   def make(self) -> Optional[QLC]:
     return None
```

### Comparing `qlcpy-1.0.4/qlcpy/questions/__init__.py` & `qlcpy-1.0.9/qlcpy/questions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 from ..instrument import Instrumentor
 from ..models import QLCPrepared
 from . import lines, dynamic
 
 QLCMaker = Callable[[str, AST, Optional[str], Instrumentor], List[QLCPrepared]]
 
 class QLCTemplate:
-  def __init__(self, type: str, description: str, maker: QLCMaker):
+  def __init__(self, pos: int, type: str, description: str, maker: QLCMaker):
+    self.pos = pos
     self.type = type
     self.description = description
     self.maker = maker
 
 TEMPLATES: List[QLCTemplate] = [
   QLCTemplate(
+    0,
     'LoopEnd',
     'The last line of a loop',
     lines.loop_end
   ),
   QLCTemplate(
+    1,
     'VariableDeclaration',
     'The declaration line for a variable',
     lines.variable_declaration
   ),
   QLCTemplate(
+    2,
     'LoopCount',
     'The number of times that a loop was evaluated',
     dynamic.loop_count
   ),
   QLCTemplate(
+    3,
     'VariableTrace',
     'The values that were assigned to a variable',
     dynamic.variable_trace
   ),
 ]
```

### Comparing `qlcpy-1.0.4/qlcpy/questions/dynamic.py` & `qlcpy-1.0.9/qlcpy/questions/dynamic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,160 @@
 from ast import AST
-from typing import Any, List, Optional
+from typing import List, Optional
 
-from ..arrays import random_steps
+from ..arrays import altered_arrays
 from ..i18n import t
-from ..instrument import find_nodes, Instrumentor, ProgramData
+from ..instrument import Instrumentor, ProgramData
 from ..models import QLC, QLCPrepared
-from ..primitives import primitive_to_str
-from .options import pick_options, options, fill_random_options
+from ..primitives import includes_references, primitives_to_str
+from .options import pick_options, options, take_options, fill_options, random_order
 
 class LoopCount(QLCPrepared):
-  def __init__(self, type: str, call: Optional[str], element: ProgramData.Element):
-    super().__init__(type)
+  def __init__(
+    self,
+    pos: int,
+    type: str,
+    call: Optional[str],
+    element: ProgramData.Element,
+    scope: ProgramData.Element,
+  ):
+    super().__init__(pos, type)
     self.call = call
     self.loop = element
+    self.scope = scope
 
   def make(self):
-    count = sum(1 for b in self.loop.evaluations if b == 0)
-    if count > 10:
+    if len(self.scope.evaluations) > 1:
       return None
+    count = sum(1 for b in self.loop.evaluations if b == 0)
     return QLC(
+      self.pos,
       self.type,
       (
         t('q_loop_count_call', self.loop.declaration.lineno, self.call)
         if self.call else
         t('q_loop_count', self.loop.declaration.lineno)
       ),
       pick_options(
         options([count], 'correct_count', t('o_loop_count_correct'), True),
-        fill_random_options(4, range(10), 'random_count', t('o_loop_count_random')),
+        options([count + 1], 'one_off_count', t('o_loop_count_one_off')),
+        fill_options(
+          4,
+          random_order(range(10)),
+          'random_count',
+          t('o_loop_count_random')
+        ),
       )
     )
 
 def loop_count(
+  pos: int,
   type: str,
   tree: AST,
   call: Optional[str],
   ins: Instrumentor
 ) -> List[QLCPrepared]:
-  return list(LoopCount(type, call, e) for e in ins.data.elements_for_types('loop'))
+  return list(
+    LoopCount(
+      pos,
+      type,
+      call,
+      e,
+      ins.data.element_for_scope(e.scope),
+    ) for e in ins.data.elements_for_types('loop')
+  )
 
 class VariableTrace(QLCPrepared):
-  def __init__(self, type: str, call: Optional[str], element: ProgramData.Element, seeds: List[Any]):
-    super().__init__(type)
+  def __init__(
+    self,
+    pos: int,
+    type: str,
+    call: Optional[str],
+    element: ProgramData.Element,
+    scope: ProgramData.Element,
+    all: List[ProgramData.Element]
+  ):
+    super().__init__(pos, type)
     self.call = call
     self.variable = element
-    self.seeds = seeds
+    self.scope = scope
+    self.all = all
   
   def make(self):
     decl = self.variable.declaration
     vals = self.variable.values
-    if decl is None or len(vals) > 5:
-      return None
+    other = [o.values for o in self.all if o != self.variable]
+    if (
+      decl is None
+      or len(vals) < 2
+      or includes_references(vals)
+      or len(self.scope.evaluations) > 1
+    ):
+      return None  
+    if len(vals) > 8:
+      return QLC(
+        self.pos,
+        self.type,
+        (
+          t('q_variable_trace_start_call', decl.id, decl.lineno, self.call)
+          if self.call else
+          t('q_variable_trace_start', decl.id, decl.lineno)
+        ),
+        pick_options(
+          options(
+            [f'{primitives_to_str(vals[:4])}, ...'],
+            'correct_trace',
+            t('o_variable_trace_start_correct'),
+            True
+          ),
+          fill_options(
+            4,
+            [
+              f'{primitives_to_str(a)}, ...'
+              for a in random_order(altered_arrays(vals[:4], other, True))
+            ],
+            'random_values',
+            t('o_variable_trace_start_random')
+          ),
+        )
+      )
     return QLC(
+      self.pos,
       self.type,
       (
         t('q_variable_trace_call', decl.id, decl.lineno, self.call)
         if self.call else
         t('q_variable_trace', decl.id, decl.lineno)
       ),
       pick_options(
-        options([primitive_to_str(vals)], 'correct_trace', t('o_variable_trace_correct'), True),
-        options(
-          [primitive_to_str(vals[:-1])] if len(vals) > 1 else [],
-          'miss_value',
-          t('o_variable_trace_miss')
-        ),
-        fill_random_options(
+        options([primitives_to_str(vals)], 'correct_trace', t('o_variable_trace_correct'), True),
+        options([primitives_to_str(vals[:-1])], 'miss_value', t('o_variable_trace_miss')),
+        fill_options(
           4,
-          [primitive_to_str(a) for a in random_steps(vals, self.seeds)],
+          [
+            primitives_to_str(a)
+            for a in random_order(altered_arrays(vals, other))
+          ],
           'random_values',
           t('o_variable_trace_random')
         ),
       )
     )
 
 def variable_trace(
+  pos: int,
   type: str,
   tree: AST,
   call: Optional[str],
   ins: Instrumentor
 ) -> List[VariableTrace]:
-  seeds = list(n.value for n in find_nodes(tree, ['Constant']))
-  return list(VariableTrace(type, call, e, seeds) for e in ins.data.elements_for_types('variable'))
+  vars = list(ins.data.elements_for_types(['variable']))
+  return list(
+    VariableTrace(
+      pos,
+      type,
+      call,
+      v,
+      ins.data.element_for_scope(v.scope),
+      vars
+    ) for v in vars
+  )
```

### Comparing `qlcpy-1.0.4/qlcpy/questions/lines.py` & `qlcpy-1.0.9/qlcpy/questions/lines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 import random
 from ast import AST
 from typing import List, Optional
 
 from ..i18n import t
 from ..instrument import find_nodes, Instrumentor, ProgramData
 from ..models import QLC, QLCPrepared
-from .options import pick_options, options, random_options, fill_random_options
+from .options import pick_options, options, take_options, fill_options, random_order
 
 class LoopEnd(QLCPrepared):
-  def __init__(self, type: str, node: AST):
-    super().__init__(type)
+  def __init__(self, pos: int, type: str, node: AST):
+    super().__init__(pos, type)
     self.node = node
 
   def make(self):
     beg = self.node.lineno
     end = self.node.end_lineno
     return QLC(
+      self.pos,
       self.type,
       t('q_loop_end', beg),
       pick_options(
         options([end], 'last_line_inside_block', t('o_loop_end_correct'), True),
         options([max(1, beg - 1)], 'line_before_block', t('o_loop_end_before')),
         options([end + 1], 'line_after_block', t('o_loop_end_after')),
-        fill_random_options(4, range(beg + 1, end), 'line_inside_block', t('o_loop_end_inside'))
+        fill_options(
+          4,
+          random_order(range(beg + 1, end)),
+          'line_inside_block',
+          t('o_loop_end_inside')
+        ),
+        fill_options(4, [end + 2], 'line_after_block', t('o_loop_end_after'))
       )
     )
 
 def loop_end(
+  pos: int,
   type: str,
   tree: AST,
   call: Optional[str],
   ins: Instrumentor
 ) -> List[LoopEnd]:
-  return list(LoopEnd(type, node) for node in find_nodes(tree, ['For', 'While']))
+  return list(
+    LoopEnd(pos, type, node) for node in find_nodes(tree, ['For', 'While'])
+  )
 
 class VariableDeclaration(QLCPrepared):
-  def __init__(self, type: str, element: ProgramData.Element):
-    super().__init__(type)
+  def __init__(self, pos: int, type: str, element: ProgramData.Element):
+    super().__init__(pos, type)
     self.variable = element
   
   def make(self):
     decl = self.variable.declaration
     refs = self.variable.references
     # NOTE: if-else structures can easily assign 1st time on 2nd store name, what to do?
     if decl is None or len(refs) == 0:
@@ -48,33 +58,37 @@
     ref = random.choice(refs)
     text_id = {
       'Store': 'q_variable_write_declaration',
       'Load': 'q_variable_read_declaration',
       'Del': 'q_variable_del_declaration',
     }
     return QLC(
+      self.pos,
       self.type,
       t(text_id[ref.ctx.__class__.__name__], ref.id, ref.lineno),
       pick_options(
         options([decl.lineno], 'declaration_line', t('o_variable_declaration_correct'), True),
-        random_options(
+        take_options(
           2,
-          [r.lineno for r in refs],
+          random_order(r.lineno for r in refs),
           'reference_line',
           t('o_variable_declaration_reference')
         ),
-        fill_random_options(
+        fill_options(
           4,
-          range(max(1, decl.lineno - 2), max(r.lineno for r in refs) + 3),
+          random_order(range(max(1, decl.lineno - 2), max(r.lineno for r in refs) + 3)),
           'random_line',
           t('o_variable_declaration_random')
         )
       )
     )
 
 def variable_declaration(
+  pos: int,
   type: str,
   tree: AST,
   call: Optional[str],
   ins: Instrumentor
 ) -> List[VariableDeclaration]:
-  return list(VariableDeclaration(type, e) for e in ins.data.elements_for_types('variable'))
+  return list(
+    VariableDeclaration(pos, type, e) for e in ins.data.elements_for_types('variable')
+  )
```

### Comparing `qlcpy-1.0.4/qlcpy/questions/options.py` & `qlcpy-1.0.9/qlcpy/questions/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Callable, Iterable, List, Optional
+from typing import Any, Iterable, List, Optional
 
 from ..models import QLCOption
 
 class QLCOptionRequest:
   def __init__(
     self,
     opt: Iterable[QLCOption],
@@ -12,22 +12,23 @@
   ):
     self.opt = opt
     self.n = n
     self.fill = fill
 
 def pick_options(*requests: QLCOptionRequest) -> List[QLCOption]:
   out: List[QLCOption] = []
+  answers: List[Any] = []
   for r in requests:
-    if not r.n is None and r.fill and len(out) >= r.n:
-      continue
-    opts = [o for o in r.opt if not o.answer in [u.answer for u in out]]
-    if r.n is None:
-      out.extend(opts)
-    else:
-      out.extend(random.sample(opts, min(max(0, r.n - len(out)) if r.fill else r.n, len(opts))))
+    target = 100 if r.n is None else (r.n if r.fill else len(out) + r.n)
+    for o in r.opt:
+      if len(out) >= target:
+        break
+      if not o.answer in answers:
+        answers.append(o.answer)
+        out.append(o)
   out_int = list(o for o in out if type(o.answer) == int)
   out_str = list(o for o in out if type(o.answer) != int)
   return [
     *[out_int[i] for i, _ in sorted(enumerate(out_int), key=lambda e: e[1].answer)],
     *[out_str[i] for i, _ in sorted(enumerate(out_str), key=lambda e: str(e[1].answer))]
   ]
 
@@ -43,24 +44,28 @@
   answers: Iterable[Any],
   type: str,
   info: Optional[str] = '',
   correct: Optional[bool] = False
 ) -> QLCOptionRequest:
   return QLCOptionRequest(opt(answers, type, info, correct))
 
-def random_options(
+def take_options(
   count: int,
   answers: Iterable[Any],
   type: str,
   info: Optional[str] = '',
   correct: Optional[bool] = False
 ) -> QLCOptionRequest:
   return QLCOptionRequest(opt(answers, type, info, correct), count)
 
-def fill_random_options(
+def fill_options(
   count: int,
   answers: Iterable[Any],
   type: str,
   info: Optional[str] = '',
   correct: Optional[bool] = False
 ) -> QLCOptionRequest:
   return QLCOptionRequest(opt(answers, type, info, correct), count, True)
+
+def random_order(answers: Iterable[Any]) -> Iterable[Any]:
+  mix_answers = list(answers)
+  return random.sample(mix_answers, len(mix_answers))
```

### Comparing `qlcpy-1.0.4/qlcpy.egg-info/PKG-INFO` & `qlcpy-1.0.9/qlcpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlcpy
-Version: 1.0.4
+Version: 1.0.9
 Summary: Generates questions about given Python program
 Home-page: https://github.com/teemulehtinen/qlcpy
 Author: Teemu Lehtinen
 Author-email: teemu.t.lehtinen@aalto.fi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qlcpy-1.0.4/qlcpy.egg-info/SOURCES.txt` & `qlcpy-1.0.9/qlcpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/setup.cfg` & `qlcpy-1.0.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qlcpy
-version = 1.0.4
+version = 1.0.9
 author = Teemu Lehtinen
 author_email = teemu.t.lehtinen@aalto.fi
 description = Generates questions about given Python program
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/teemulehtinen/qlcpy
 classifiers =
```

### Comparing `qlcpy-1.0.4/test/test_instrumentor.py` & `qlcpy-1.0.9/test/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/test/test_printer.py` & `qlcpy-1.0.9/test/test_printer.py`

 * *Files identical despite different names*

### Comparing `qlcpy-1.0.4/test/test_transform.py` & `qlcpy-1.0.9/test/test_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 """
 run = True
 while run:
   line = input('Read stdin')
   run = line != 'end'
 """
     )
-    instrumentor = run_with_instrumentor(tree, None, "line1\nline2\nend\n")
+    instrumentor = run_with_instrumentor(tree, input="line1\nline2\nend\n")
     line = instrumentor.data.element_for_id('line')
     self.assertEqual(line.values, ['line1', 'line2', 'end'])
```

