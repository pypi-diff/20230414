# Comparing `tmp/thunno2-2.0.8.tar.gz` & `tmp/thunno2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.8.tar", last modified: Fri Apr 14 18:54:33 2023, max compression
+gzip compressed data, was "thunno2-2.0.9.tar", last modified: Fri Apr 14 19:09:18 2023, max compression
```

## Comparing `thunno2-2.0.8.tar` & `thunno2-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.341474 thunno2-2.0.8/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 18:54:33.341352 thunno2-2.0.8/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 18:54:33.341510 thunno2-2.0.8/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.8/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.340671 thunno2-2.0.8/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.8/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.8/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.8/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6036 2023-04-14 17:00:15.000000 thunno2-2.0.8/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.8/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25799 2023-04-14 16:37:26.000000 thunno2-2.0.8/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    22283 2023-04-14 16:37:26.000000 thunno2-2.0.8/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.8/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.8/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.8/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 18:52:11.000000 thunno2-2.0.8/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 18:54:33.341182 thunno2-2.0.8/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 18:54:33.000000 thunno2-2.0.8/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595983 thunno2-2.0.9/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 19:09:18.595862 thunno2-2.0.9/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 19:09:18.596019 thunno2-2.0.9/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.9/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595187 thunno2-2.0.9/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.9/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.9/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.9/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:07:56.000000 thunno2-2.0.9/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.9/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25799 2023-04-14 16:37:26.000000 thunno2-2.0.9/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    22283 2023-04-14 16:37:26.000000 thunno2-2.0.9/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-14 19:08:45.000000 thunno2-2.0.9/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.9/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 19:09:07.000000 thunno2-2.0.9/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595713 thunno2-2.0.9/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.8/PKG-INFO` & `thunno2-2.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.8
+Version: 2.0.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.9.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.8/setup.py` & `thunno2-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/codepage.py` & `thunno2-2.0.9/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/commands.py` & `thunno2-2.0.9/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/constants.py` & `thunno2-2.0.9/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/dictionary.py` & `thunno2-2.0.9/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/flags.py` & `thunno2-2.0.9/thunno2/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,30 +160,31 @@
                     if isinstance(x, tuple):
                         new_inputs = process_input_flags(new_flags, '\n'.join(map(repr, x)))
                     else:
                         new_inputs = [x]
                 except:
                     new_inputs = [line]
                 try:
-                    expected = process_input_flags('', output)
+                    expected = process_input_flags('', output)[0]
                 except:
                     expected = output.strip()
-                commands.ctx.og_input_list = new_inputs.copy()
-                commands.ctx.other_il = new_inputs.copy()
-                print(line, '--> ', end='')
-                interpreter.run(code, n=0, iteration_index=0)
-                process_output_flags(new_flags, False)
-                actual_output = next(commands.ctx.stack.rmv(0))
-                print(actual_output, end=' ')
-                if actual_output == expected:
-                    print('PASS ✅')
-                else:
-                    print(f'FAIL ❌ (Expected {expected})')
-            except:
-                pass
+            except Exception as e:
+                print(f'FAIL ❌ (Got error {e})')
+                continue
+            commands.ctx.og_input_list = new_inputs.copy()
+            commands.ctx.other_il = new_inputs.copy()
+            print(line, '--> ', end='')
+            interpreter.run(code, n=0, iteration_index=0)
+            process_output_flags(new_flags, False)
+            actual_output = next(commands.ctx.stack.rmv(1))
+            print(actual_output, end='\t')
+            if actual_output == expected:
+                print('PASS ✅')
+            else:
+                print(f'FAIL ❌ (Expected {expected})')
         return None
 
     inputs = process_input_flags(flags, inputs)
     commands.ctx.og_input_list = inputs.copy()
     commands.ctx.other_il = inputs.copy()
     interpreter.run(code, n=0, iteration_index=0)
     process_output_flags(flags)
```

### Comparing `thunno2-2.0.8/thunno2/helpers.py` & `thunno2-2.0.9/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/interpreter.py` & `thunno2-2.0.9/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/lexer.py` & `thunno2-2.0.9/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/run.py` & `thunno2-2.0.9/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/tests.py` & `thunno2-2.0.9/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2/tokens.py` & `thunno2-2.0.9/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.8/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.9/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.8
+Version: 2.0.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.9.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

