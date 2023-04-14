# Comparing `tmp/thunno2-2.0.7.tar.gz` & `tmp/thunno2-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.7.tar", last modified: Fri Apr 14 16:14:39 2023, max compression
+gzip compressed data, was "thunno2-2.0.8.tar", last modified: Fri Apr 14 18:54:33 2023, max compression
```

## Comparing `thunno2-2.0.7.tar` & `thunno2-2.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.405978 thunno2-2.0.7/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 16:14:39.405825 thunno2-2.0.7/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 16:14:39.406018 thunno2-2.0.7/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.7/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.404841 thunno2-2.0.7/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.7/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.7/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.7/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     4608 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25412 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    21430 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.7/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.7/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 16:14:32.000000 thunno2-2.0.7/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.405562 thunno2-2.0.7/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.341474 thunno2-2.0.8/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 18:54:33.341352 thunno2-2.0.8/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 18:54:33.341510 thunno2-2.0.8/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.8/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.340671 thunno2-2.0.8/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.8/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.8/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.8/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6036 2023-04-14 17:00:15.000000 thunno2-2.0.8/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.8/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25799 2023-04-14 16:37:26.000000 thunno2-2.0.8/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    22283 2023-04-14 16:37:26.000000 thunno2-2.0.8/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.8/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.8/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 18:52:11.000000 thunno2-2.0.8/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.341182 thunno2-2.0.8/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.7/PKG-INFO` & `thunno2-2.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.7
+Version: 2.0.8
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.7.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.8.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.7/setup.py` & `thunno2-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/codepage.py` & `thunno2-2.0.8/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/commands.py` & `thunno2-2.0.8/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/constants.py` & `thunno2-2.0.8/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/dictionary.py` & `thunno2-2.0.8/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/helpers.py` & `thunno2-2.0.8/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/interpreter.py` & `thunno2-2.0.8/thunno2/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,21 @@
                         lst.append(info[i])
                     except:
                         lst.append('\\')
                 else:
                     lst.append(c)
                 i += 1
             ctx.stack.push(''.join(lst))
+        elif desc == 'one word dictionary compression':
+            ctx.stack.push(dictionary.dictionary_decompress_string(info).title())
+        elif desc == 'two words dictionary compression':
+            ctx.stack.push(
+                dictionary.dictionary_decompress_string(info[:2]).title()
+                + dictionary.dictionary_decompress_string(info[2:]).title()
+            )
         elif desc == 'compressed number' or desc == 'small compressed number':
             base255_number = decompress(info, '»')
             ctx.stack.push(base255_number)
         elif desc == 'compressed list':
             base255_number = decompress(info, '¿')
             decompressed_string = to_custom_base_string('][0123456789-.,', base255_number)
             try:
```

### Comparing `thunno2-2.0.7/thunno2/lexer.py` & `thunno2-2.0.8/thunno2/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from thunno2.commands import commands, DIGRAPHS, get_a_function, Void
 from thunno2.constants import CONSTANTS
 from thunno2.codepage import codepage_index
+from thunno2.dictionary import dictionary_codepage
 
 
 """Splits Thunno 2 code into tokens to make it easier for the interpreter"""
 
 """Creative Commons Legal Code
 
 CC0 1.0 Universal
@@ -189,19 +190,40 @@
                 x = code[index]
                 ret.append(('\'' + x, 'one character', x))
             except:
                 ret.append(('\'', 'one character', ''))
         elif char == '`':
             index += 2
             x = code[index - 1: index + 1]
-            ret.append(('`' + x, 'two characters', x))
+            if (len(x) != 2) or (x[0] not in dictionary_codepage) or (x[1] not in dictionary_codepage):
+                ret.append(('`' + x, 'two characters', x))
+            else:
+                ret.append(('`' + x, 'one word dictionary compression', x))
         elif char == 'ʋ':
             index += 3
             x = code[index - 2: index + 1]
-            ret.append(('ʋ' + x, 'three characters', x))
+            try:
+                nxt = code[index + 1]
+            except:
+                nxt = ''
+            if (len(x) != 3) or (
+                (
+                    x[0] not in dictionary_codepage
+                ) or (
+                    x[1] not in dictionary_codepage
+                ) or (
+                    x[2] not in dictionary_codepage
+                ) or (
+                    nxt not in dictionary_codepage
+                )
+            ):
+                ret.append(('ʋ' + x, 'three characters', x))
+            else:
+                index += 1
+                ret.append(('ʋ' + x + nxt, 'two words dictionary compression', x + nxt))
         elif char == '[':
             s = char
             index += 1
             try:
                 in_string = ''
                 nests = 1
                 while nests:
```

### Comparing `thunno2-2.0.7/thunno2/run.py` & `thunno2-2.0.8/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/tests.py` & `thunno2-2.0.8/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2/tokens.py` & `thunno2-2.0.8/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.7/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.8/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.7
+Version: 2.0.8
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.7.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.8.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

