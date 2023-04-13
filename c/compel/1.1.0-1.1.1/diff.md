# Comparing `tmp/compel-1.1.0.tar.gz` & `tmp/compel-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-vxcwh51c/compel-1.1.0.tar", last modified: Fri Apr  7 12:11:04 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-kifytt8b/compel-1.1.1.tar", last modified: Thu Apr 13 23:56:13 2023, max compression
```

## Comparing `compel-1.1.0.tar` & `compel-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-07 12:11:04.000000 compel-1.1.0/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.0/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     6463 2023-04-07 12:11:04.000000 compel-1.1.0/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     5885 2023-04-07 11:43:19.000000 compel-1.1.0/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-07 11:44:18.000000 compel-1.1.0/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-07 12:11:04.000000 compel-1.1.0/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-07 12:11:04.000000 compel-1.1.0/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.0/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    13867 2023-04-07 10:02:49.000000 compel-1.1.0/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.0/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.0/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    23408 2023-04-07 09:51:02.000000 compel-1.1.0/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29480 2023-04-07 11:53:23.000000 compel-1.1.0/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     6463 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-07 12:11:04.000000 compel-1.1.0/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-07 12:11:04.000000 compel-1.1.0/test/
--rw-r--r--   0 damian     (501) staff       (20)    18392 2023-04-03 07:52:15.000000 compel-1.1.0/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    13788 2023-04-07 09:51:02.000000 compel-1.1.0/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    46708 2023-04-07 11:49:56.000000 compel-1.1.0/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     6620 2023-04-13 23:56:13.000000 compel-1.1.1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6042 2023-04-13 23:55:34.000000 compel-1.1.1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-13 23:55:39.000000 compel-1.1.1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-13 23:56:13.000000 compel-1.1.1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    13867 2023-04-13 23:44:59.000000 compel-1.1.1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    23408 2023-04-13 23:44:59.000000 compel-1.1.1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-13 23:50:41.000000 compel-1.1.1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     6620 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    18392 2023-04-13 23:44:59.000000 compel-1.1.1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    13788 2023-04-13 23:44:59.000000 compel-1.1.1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-13 23:53:08.000000 compel-1.1.1/test/test_prompt_parser.py
```

### Comparing `compel-1.1.0/LICENSE` & `compel-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/PKG-INFO` & `compel-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.0
+Version: 1.1.1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,17 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](https://invoke-ai.github.io/InvokeAI/features/PROMPTS/#prompt-syntax-features) - note however that cross-attention control `.swap()` is currently ignored by Compel.
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+
+Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
 ### Demo
 
@@ -71,14 +73,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
+
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
 
 #### 1.0.5 - fix incorrect parsing when passing invalid (auto1111) syntax that has a float
```

### Comparing `compel-1.1.0/README.md` & `compel-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](https://invoke-ai.github.io/InvokeAI/features/PROMPTS/#prompt-syntax-features) - note however that cross-attention control `.swap()` is currently ignored by Compel.
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+
+Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
 ### Demo
 
@@ -57,14 +59,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
+
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
 
 #### 1.0.5 - fix incorrect parsing when passing invalid (auto1111) syntax that has a float
```

### Comparing `compel-1.1.0/pyproject.toml` & `compel-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.0/src/compel/compel.py` & `compel-1.1.1/src/compel/compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/src/compel/conditioning_scheduler.py` & `compel-1.1.1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/src/compel/cross_attention_control.py` & `compel-1.1.1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/src/compel/embeddings_provider.py` & `compel-1.1.1/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/src/compel/prompt_parser.py` & `compel-1.1.1/src/compel/prompt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,30 +539,30 @@
         attention,
         cross_attention_substitute,
         parenthesized_fragment,
         quoted_fragment,
         non_syntax_word
     ]
     # a fragment that is permitted to contain commas
-    fragment_including_commas = pp.ZeroOrMore(pp.MatchFirst(
+    fragment_including_commas_or_periods = pp.ZeroOrMore(pp.MatchFirst(
         fragment_part_expressions + [
-            pp.Literal(',').set_parse_action(lambda x: Fragment(x[0]))
+            (pp.Literal(',') | pp.Literal('.')).set_parse_action(lambda x: Fragment(x[0]))
         ]
     ))
     # a fragment that is not permitted to contain commas
     fragment_excluding_commas = pp.ZeroOrMore(pp.MatchFirst(
         fragment_part_expressions
     ))
 
     # a fragment in double quotes (may be nested)
     quoted_fragment << pp.QuotedString(quote_char='"', esc_char=None, esc_quote='\\"')
-    quoted_fragment.set_parse_action(lambda x: parse_fragment_str(x, fragment_including_commas, in_quotes=True))
+    quoted_fragment.set_parse_action(lambda x: parse_fragment_str(x, fragment_including_commas_or_periods, in_quotes=True))
 
     # a fragment inside parentheses (may be nested)
-    parenthesized_fragment << (lparen + fragment_including_commas + rparen)
+    parenthesized_fragment << (lparen + fragment_including_commas_or_periods + rparen)
     parenthesized_fragment.set_name('parenthesized_fragment')
     parenthesized_fragment.set_debug(False)
 
     # a string of the form (<keyword>=<float|keyword> | <float> | <keyword>) where keyword is alphanumeric + '_'
     option = pp.Group(pp.MatchFirst([
         keyword + equals + (number | keyword),  # option=value
         number.copy().set_parse_action(pp.token_map(str)), # weight
```

### Comparing `compel-1.1.0/src/compel.egg-info/PKG-INFO` & `compel-1.1.1/src/compel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.0
+Version: 1.1.1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,17 @@
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
-Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](https://invoke-ai.github.io/InvokeAI/features/PROMPTS/#prompt-syntax-features) - note however that cross-attention control `.swap()` is currently ignored by Compel.
+Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
+
+Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
 ### Installation
 
 `pip install compel`
 
 ### Demo
 
@@ -71,14 +73,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
+
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
 
 #### 1.0.5 - fix incorrect parsing when passing invalid (auto1111) syntax that has a float
```

### Comparing `compel-1.1.0/test/test_compel.py` & `compel-1.1.1/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/test/test_embeddings_provider.py` & `compel-1.1.1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.0/test/test_prompt_parser.py` & `compel-1.1.1/test/test_prompt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,25 @@
         self.assertEqual(make_weighted_conjunction([('flames', pow(0.9, 2))]), parse_prompt("(flames)--"))
         self.assertEqual(make_weighted_conjunction([('flowers', pow(0.9, 3)), ('flames', pow(1.1, 3))]), parse_prompt("(flowers)--- flames+++"))
         self.assertEqual(make_weighted_conjunction([('pretty flowers', 1.1)]),
                          parse_prompt("(pretty flowers)+"))
         self.assertEqual(make_weighted_conjunction([('pretty flowers', 1.1), (', the flames are too hot', 1)]),
                          parse_prompt("(pretty flowers)+, the flames are too hot"))
 
+
+    def test_wayward_periods(self):
+        self.assertEqual(
+            make_weighted_conjunction([('a text .', 0.7), ('.', 1.0), ('a second text .', 0.8)]),
+            parse_prompt("(a text.)0.7. (a second text.)0.8"))
+
+        self.assertEqual(
+            make_weighted_conjunction([('a text .', 0.7), ('.', 1.0), ('a second text .', 0.8)]),
+            parse_prompt("\"a text.\"0.7. \"a second text.\"0.8"))
+
+
     def test_no_parens_attention_runon(self):
         self.assertEqual(make_weighted_conjunction([('fire', 1.0), ('flames', pow(1.1, 2))]), parse_prompt("fire flames++"))
         self.assertEqual(make_weighted_conjunction([('fire', 1.0), ('flames', pow(0.9, 2))]), parse_prompt("fire flames--"))
         self.assertEqual(make_weighted_conjunction([('flowers', 1.0), ('fire', pow(1.1, 2)), ('flames', 1.0)]), parse_prompt("flowers fire++ flames"))
         self.assertEqual(make_weighted_conjunction([('flowers', 1.0), ('fire', pow(0.9, 2)), ('flames', 1.0)]), parse_prompt("flowers fire-- flames"))
```

