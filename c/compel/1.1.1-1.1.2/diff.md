# Comparing `tmp/compel-1.1.1.tar.gz` & `tmp/compel-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-kifytt8b/compel-1.1.1.tar", last modified: Thu Apr 13 23:56:13 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-oxd6xmuo/compel-1.1.2.tar", last modified: Fri Apr 14 00:29:27 2023, max compression
```

## Comparing `compel-1.1.1.tar` & `compel-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     6620 2023-04-13 23:56:13.000000 compel-1.1.1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6042 2023-04-13 23:55:34.000000 compel-1.1.1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-13 23:55:39.000000 compel-1.1.1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-13 23:56:13.000000 compel-1.1.1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.1/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    13867 2023-04-13 23:44:59.000000 compel-1.1.1/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.1/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.1/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    23408 2023-04-13 23:44:59.000000 compel-1.1.1/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-13 23:50:41.000000 compel-1.1.1/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     6620 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-13 23:56:13.000000 compel-1.1.1/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-13 23:56:13.000000 compel-1.1.1/test/
--rw-r--r--   0 damian     (501) staff       (20)    18392 2023-04-13 23:44:59.000000 compel-1.1.1/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    13788 2023-04-13 23:44:59.000000 compel-1.1.1/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-13 23:53:08.000000 compel-1.1.1/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.2/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     6766 2023-04-14 00:29:27.000000 compel-1.1.2/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6188 2023-04-14 00:28:54.000000 compel-1.1.2/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-14 00:29:02.000000 compel-1.1.2/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 00:29:27.000000 compel-1.1.2/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.2/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    13867 2023-04-13 23:44:59.000000 compel-1.1.2/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.2/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.2/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    23438 2023-04-14 00:26:23.000000 compel-1.1.2/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-13 23:50:41.000000 compel-1.1.2/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     6766 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/test/
+-rw-r--r--   0 damian     (501) staff       (20)    18392 2023-04-13 23:44:59.000000 compel-1.1.2/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    13788 2023-04-13 23:44:59.000000 compel-1.1.2/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-13 23:53:08.000000 compel-1.1.2/test/test_prompt_parser.py
```

### Comparing `compel-1.1.1/LICENSE` & `compel-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/PKG-INFO` & `compel-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: compel
-Version: 1.1.1
-Summary: A prompting enhancement library for transformers-type text embedding systems.
-Author-email: Damian Stewart <null@damianstewart.com>
-Project-URL: Homepage, https://github.com/damian0815/compel
-Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
@@ -73,14 +59,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
+
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
```

### Comparing `compel-1.1.1/README.md` & `compel-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: compel
+Version: 1.1.2
+Summary: A prompting enhancement library for transformers-type text embedding systems.
+Author-email: Damian Stewart <null@damianstewart.com>
+Project-URL: Homepage, https://github.com/damian0815/compel
+Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
@@ -59,14 +73,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
+
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
```

### Comparing `compel-1.1.1/pyproject.toml` & `compel-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.1/src/compel/compel.py` & `compel-1.1.2/src/compel/compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/src/compel/conditioning_scheduler.py` & `compel-1.1.2/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/src/compel/cross_attention_control.py` & `compel-1.1.2/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/src/compel/embeddings_provider.py` & `compel-1.1.2/src/compel/embeddings_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
             # embedding will be exactly half-way between the unweighted prompt and the prompt with the <1 weighted words
             # removed.
             # e.g. for "mountain:1 man:0.5", intuitively the "man" should be "half-gone". therefore, append an embedding
             # for "mountain" (i.e. without "man") to the already-produced embedding for "mountain man", and weight it
             # such that the resulting lerped embedding is exactly half-way between "mountain man" and "mountain".
             fragment_token_index_ranges = self._get_token_ranges_for_fragments(tokens.tolist(), fragments)
 
-            for index, fragment_weight in enumerate(weights):
+            for index in range(len(fragment_token_index_ranges)):
+                fragment_weight = weights[index]
                 if fragment_weight < 1:
                     if self.downweight_mode == DownweightMode.MASK:
                         fragment_start_token_id, fragment_end_token_id = fragment_token_index_ranges[index]
                         # mask out this fragment
                         mask_without_fragment = mask.clone()
                         mask_without_fragment[fragment_start_token_id:fragment_end_token_id+1] = 0
                         if not self.truncate_to_model_max_length:
@@ -150,15 +151,14 @@
                     # tan is 0.0 at 0,
                     #        1.0 at PI/4, and
                     #        inf at PI/2
                     # -> tan((1-weight)*PI/2) should give us ideal lerp weights
                     epsilon = 1e-5
                     fragment_weight = max(epsilon, fragment_weight) # inf is bad
                     embedding_lerp_weight = math.tan((1.0 - fragment_weight) * math.pi / 2)
-                    # todo handle negative weight?
 
                     per_embedding_weights.append(embedding_lerp_weight)
 
             lerped_embeddings = self.apply_embedding_weights(embeddings, per_embedding_weights, normalize=True).squeeze(0)
 
             #print(f"assembled tokens for '{fragments}' into tensor of shape {lerped_embeddings.shape}")
 
@@ -186,15 +186,15 @@
             of sequence marker and end with the end-of-sequence marker (`eos`).
         :return: A list of lists of token ids corresponding to the input strings.
         """
         # for args documentation of self.tokenizer() see ENCODE_KWARGS_DOCSTRING in tokenization_utils_base.py
         # (part of `transformers` lib)
         token_ids_list = self.tokenizer(
             texts,
-            truncation=False,
+            truncation=self.truncate_to_model_max_length,
             padding='do_not_pad',
             return_tensors=None,  # just give me lists of ints
         )['input_ids']
 
         result = []
         for token_ids in token_ids_list:
             # trim eos/bos
```

### Comparing `compel-1.1.1/src/compel/prompt_parser.py` & `compel-1.1.2/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/src/compel.egg-info/PKG-INFO` & `compel-1.1.2/src/compel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.1
+Version: 1.1.2
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,14 +73,16 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
+
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
 * any appearances of `withLora(name[, weight])` or `useLora(name[, weight])` anywhere in the prompt string will be parsed to `LoraWeight` instances, and returned on the outermost `Conjunction` returned by `parse_prompt_string()`.
```

### Comparing `compel-1.1.1/test/test_compel.py` & `compel-1.1.2/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/test/test_embeddings_provider.py` & `compel-1.1.2/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.1/test/test_prompt_parser.py` & `compel-1.1.2/test/test_prompt_parser.py`

 * *Files identical despite different names*

