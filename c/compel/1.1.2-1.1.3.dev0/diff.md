# Comparing `tmp/compel-1.1.2.tar.gz` & `tmp/compel-1.1.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-oxd6xmuo/compel-1.1.2.tar", last modified: Fri Apr 14 00:29:27 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-emvysva3/compel-1.1.3.dev0.tar", last modified: Fri Apr 14 08:44:46 2023, max compression
```

## Comparing `compel-1.1.2.tar` & `compel-1.1.3.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.2/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     6766 2023-04-14 00:29:27.000000 compel-1.1.2/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6188 2023-04-14 00:28:54.000000 compel-1.1.2/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-04-14 00:29:02.000000 compel-1.1.2/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 00:29:27.000000 compel-1.1.2/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.2/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    13867 2023-04-13 23:44:59.000000 compel-1.1.2/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.2/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.2/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    23438 2023-04-14 00:26:23.000000 compel-1.1.2/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-13 23:50:41.000000 compel-1.1.2/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     6766 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 00:29:27.000000 compel-1.1.2/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 00:29:27.000000 compel-1.1.2/test/
--rw-r--r--   0 damian     (501) staff       (20)    18392 2023-04-13 23:44:59.000000 compel-1.1.2/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    13788 2023-04-13 23:44:59.000000 compel-1.1.2/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-13 23:53:08.000000 compel-1.1.2/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6400 2023-04-14 08:44:28.000000 compel-1.1.3.dev0/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-04-14 08:42:50.000000 compel-1.1.3.dev0/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.3.dev0/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14494 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.3.dev0/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    24862 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/test/
+-rw-r--r--   0 damian     (501) staff       (20)    14454 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/test/test_prompt_parser.py
```

### Comparing `compel-1.1.2/LICENSE` & `compel-1.1.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.2/PKG-INFO` & `compel-1.1.3.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.2
+Version: 1.1.3.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,14 +73,18 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
```

### Comparing `compel-1.1.2/README.md` & `compel-1.1.3.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
```

### Comparing `compel-1.1.2/pyproject.toml` & `compel-1.1.3.dev0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.2"
+version = "1.1.3.dev0"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.2/src/compel/compel.py` & `compel-1.1.3.dev0/src/compel/compel.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     def __init__(self,
                  tokenizer: CLIPTokenizer,
                  text_encoder: CLIPTextModel,
                  textual_inversion_manager: Optional[BaseTextualInversionManager] = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate_long_prompts: bool = True,
                  padding_attention_mask_value: int = 1,
-                 downweight_mode: DownweightMode = DownweightMode.MASK):
+                 downweight_mode: DownweightMode = DownweightMode.MASK,
+                 use_penultimate_clip_layer: bool=False
+                 ):
         """
         Initialize Compel. The tokenizer and text_encoder can be lifted directly from any DiffusionPipeline.
 
         `textual_inversion_manager`: Optional instance to handle expanding multi-vector textual inversion tokens.
         `dtype_for_device_getter`: A Callable that returns a torch dtype for a given device. You probably don't need to
             use this.
         `truncate_long_prompts`: if True, truncate input prompts to 77 tokens long including beginning/end markers
@@ -38,22 +40,26 @@
             If False, do not truncate, and instead assemble as many 77 token long chunks, each capped by beginning/end
             markers, as is necessary to encode the whole prompt. You will likely need to supply both positive and
             negative prompts in this case - use `pad_conditioning_tensors_to_same_length` to prevent having tensor
             length mismatch errors when passing the embeds on to your DiffusionPipeline for inference.
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: Specifies whether downweighting should be applied by MASKing out the downweighted tokens
             (default) or REMOVEing them (legacy behaviour; messes up position embeddings of tokens following).
+        `use_penultimate_clip_layer`: If True, use the penultimate hidden layer output of the CLIP text encoder's output,
+            rather than the final hidden layer output. For SD2.0/2.1 you should probably pass `True` here because SD2
+            is "conditioned on the penultimate text embeddings of a CLIP ViT-H/14 text encoder".
         """
         self.conditioning_provider = EmbeddingsProvider(tokenizer=tokenizer,
                                                         text_encoder=text_encoder,
                                                         textual_inversion_manager=textual_inversion_manager,
                                                         dtype_for_device_getter=dtype_for_device_getter,
                                                         truncate=truncate_long_prompts,
                                                         padding_attention_mask_value = padding_attention_mask_value,
-                                                        downweight_mode = downweight_mode
+                                                        downweight_mode=downweight_mode,
+                                                        use_penultimate_clip_layer=use_penultimate_clip_layer
                                                         )
 
     @property
     def device(self):
         return self.conditioning_provider.text_encoder.device
 
     def make_conditioning_scheduler(self, positive_prompt: str, negative_prompt: str='') -> ConditioningScheduler:
@@ -147,22 +153,25 @@
         for i, c in enumerate(conditionings):
             while c.shape[1] < max_token_count:
                 c = torch.cat([c, empty_z], dim=1)
             conditionings[i] = c
         return conditionings
 
 
-    def _get_conditioning_for_flattened_prompt(self, prompt: FlattenedPrompt, should_return_tokens: bool=False
+    def _get_conditioning_for_flattened_prompt(self,
+                                               prompt: FlattenedPrompt,
+                                               should_return_tokens: bool=False
                                                ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         if type(prompt) is not FlattenedPrompt:
             raise ValueError(f"embeddings can only be made from FlattenedPrompts, got {type(prompt).__name__} instead")
         fragments = [x.text for x in prompt.children]
         weights = [x.weight for x in prompt.children]
         conditioning, tokens = self.conditioning_provider.get_embeddings_for_weighted_prompt_fragments(
-            text_batch=[fragments], fragment_weights_batch=[weights], should_return_tokens=True, device=self.device)
+            text_batch=[fragments], fragment_weights_batch=[weights],
+            should_return_tokens=True, device=self.device)
         if should_return_tokens:
             return conditioning, tokens
         else:
             return conditioning
 
     def _get_conditioning_for_blend(self, blend: Blend):
         conditionings_to_blend = []
```

### Comparing `compel-1.1.2/src/compel/conditioning_scheduler.py` & `compel-1.1.3.dev0/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.2/src/compel/cross_attention_control.py` & `compel-1.1.3.dev0/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.2/src/compel/embeddings_provider.py` & `compel-1.1.3.dev0/src/compel/embeddings_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,37 @@
     def __init__(self,
                  tokenizer: CLIPTokenizer,
                  text_encoder: CLIPTextModel,
                  textual_inversion_manager: BaseTextualInversionManager = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate: bool = True,
                  padding_attention_mask_value: int = 1,
-                 downweight_mode: DownweightMode = DownweightMode.MASK
+                 downweight_mode: DownweightMode = DownweightMode.MASK,
+                 use_penultimate_clip_layer: bool=False
                  ):
         """
         `tokenizer`: converts strings to lists of int token ids
         `text_encoder`: convert lists of token ids to embedding tensors
         `textual_inversion_manager`: manage token insertion for textual inversions with vector length >1
         `dtype_for_device_getter`: callback that returns an appropriate dtype for the requested device. if unset, defaults to torch.float32.
         `truncate`: if True, truncate inputs to the maximum length specified by the tokenizer. if False, returns
                     tensors that may be longer than the maximum length (but will always be an integer multiple of maximum length)
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
+        `downweight_mode`: if MASK, downweight by blending with a version of the prompt with the downweighted terms masked out.
+                    if REMOVE, the blend is against a version of the prompt with the downweighted tokens removed
+        `use_penultimate_clip_layer`: Whether to tuse the penultimate hidden state output of the CLIP emcoder (True) or
+                    the final hidden state output (False, default).
         """
         self.tokenizer = tokenizer
         self.text_encoder = text_encoder
         self.textual_inversion_manager = textual_inversion_manager
         self.truncate_to_model_max_length = truncate
         self.padding_attention_mask_value = padding_attention_mask_value
         self.downweight_mode = downweight_mode
+        self.use_penultimate_clip_layer = use_penultimate_clip_layer
 
         # by default always use float32
         self.get_dtype_for_device = dtype_for_device_getter
 
 
     @property
     def max_token_count(self) -> int:
@@ -66,15 +72,15 @@
         # blended_embeddings now has shape (77, 768)
         return blended_embeddings
 
     def get_embeddings_for_weighted_prompt_fragments(self,
                                                      text_batch: List[List[str]],
                                                      fragment_weights_batch: List[List[float]],
                                                      should_return_tokens: bool = False,
-                                                     device='cpu',
+                                                     device='cpu'
                                  ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         """
 
         :param text_batch: A list of fragments of text to which different weights are to be applied.
         :param fragment_weights_batch: A list of weights, one for each entry in `fragments`.
         :param should_return_tokens: If True, return a tuple of (embeddings, tokens), otherwise just return embeddings.
         :param device: Where to put the constructed tensor(s)
@@ -126,23 +132,24 @@
                         # mask out this fragment
                         mask_without_fragment = mask.clone()
                         mask_without_fragment[fragment_start_token_id:fragment_end_token_id+1] = 0
                         if not self.truncate_to_model_max_length:
                             # but don't mask chunk-delimiting eos/bos markers
                             mask_without_fragment[0::self.tokenizer.model_max_length] = 1
                             mask_without_fragment[self.tokenizer.model_max_length-1::self.tokenizer.model_max_length] = 1
-                        embedding_without_this = self.build_weighted_embedding_tensor(tokens, per_token_weights, mask_without_fragment)
+                        embedding_without_this = self.build_weighted_embedding_tensor(tokens,
+                                                                                      per_token_weights,
+                                                                                      mask_without_fragment)
                     else:
                         fragments_without_this = fragments[0:index] + fragments[index+1:]
                         weights_without_this = weights[0:index] + weights[index+1:]
                         tokens_without_fragment, per_token_weights_without_fragment, mask_without_fragment = \
                             self.get_token_ids_and_expand_weights(fragments_without_this, weights_without_this, device=device)
                         embedding_without_this = self.build_weighted_embedding_tensor(tokens_without_fragment,
-                                                                                      per_token_weights_without_fragment,
-                                                                                      mask_without_fragment)
+                                                                                      per_token_weights_without_fragment)
 
                     embeddings = torch.cat((embeddings, embedding_without_this.unsqueeze(0)), dim=1)
                     # weight of the embedding *without* this fragment gets *stronger* as its weight approaches 0
                     # if fragment_weight = 0, basically we want embedding_without_this to completely overwhelm base_embedding
                     # therefore:
                     # fragment_weight = 1: we are at base_z => lerp weight 0
                     # fragment_weight = 0.5: we are halfway between base_z and here => lerp weight 1
@@ -311,43 +318,57 @@
             raise ValueError(f"token_ids has shape {token_ids.shape} - expected a multiple of {self.max_token_count}")
 
         chunk_start_index = 0
         empty_token_ids = torch.tensor([self.tokenizer.bos_token_id] +
                                        [self.tokenizer.eos_token_id] +
                                        [self.tokenizer.pad_token_id] * (self.max_token_count - 2),
                                        dtype=torch.int, device=self.text_encoder.device).unsqueeze(0)
-        empty_z = self.text_encoder(empty_token_ids, return_dict=False)[0]
+        empty_z = self._encode_token_ids_to_embeddings(empty_token_ids)
         weighted_z = None
 
         chunk_size = self.max_token_count
         while chunk_start_index < token_ids.shape[0]:
             next_chunk_start_index = chunk_start_index+chunk_size
             chunk_per_token_weights = per_token_weights[chunk_start_index:next_chunk_start_index]
             chunk_token_ids = token_ids[chunk_start_index:next_chunk_start_index].unsqueeze(0)
             chunk_attention_mask = (
                 attention_mask[chunk_start_index:next_chunk_start_index].unsqueeze(0)
                 if attention_mask is not None
                 else None
             )
 
-            z = self.text_encoder(chunk_token_ids, chunk_attention_mask, return_dict=False)[0]
+            z = self._encode_token_ids_to_embeddings(chunk_token_ids, chunk_attention_mask)
             batch_weights_expanded = chunk_per_token_weights.reshape(
                 chunk_per_token_weights.shape + (1,)).expand(z.shape).to(z)
 
             z_delta_from_empty = z - empty_z
             this_weighted_z = empty_z + (z_delta_from_empty * batch_weights_expanded)
             weighted_z = (
                 this_weighted_z
                 if weighted_z is None
                 else torch.cat([weighted_z, this_weighted_z], dim=1)
             )
             chunk_start_index += chunk_size
 
         return weighted_z
 
+    def _encode_token_ids_to_embeddings(self, token_ids: torch.Tensor,
+                                        attention_mask: Optional[torch.Tensor]=None) -> torch.Tensor:
+        text_encoder_output = self.text_encoder(token_ids,
+                                                attention_mask,
+                                                output_hidden_states=self.use_penultimate_clip_layer,
+                                                return_dict=True)
+        if self.use_penultimate_clip_layer:
+            # needs normalizing
+            penultimate_hidden_state = text_encoder_output.hidden_states[-2]
+            return self.text_encoder.text_model.final_layer_norm(penultimate_hidden_state)
+        else:
+            # already normalized
+            return text_encoder_output.last_hidden_state
+
     def _get_token_ranges_for_fragments(self, chunked_and_padded_token_ids: List[int], fragments: List[str]) -> List[Tuple[int, int]]:
         """
         Match token id sequences for the strings in `fragments` with token id sequences in `chunked_and_padded_token_ids`,
          taking into account any eos and bos markers marking `self.tokenizer.max_model_length` sized chunks.
 
         Returns a list of tuples indicating start and end indices of each fragment's corresponding token id sequence in
          `chunked_and_padded_token_ids`.
```

### Comparing `compel-1.1.2/src/compel/prompt_parser.py` & `compel-1.1.3.dev0/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.2/src/compel.egg-info/PKG-INFO` & `compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.2
+Version: 1.1.3.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,14 +73,18 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
 
 * `Compel.parse_prompt_string()` now returns a `Conjunction`
```

### Comparing `compel-1.1.2/test/test_compel.py` & `compel-1.1.3.dev0/test/test_embeddings_provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,321 +1,328 @@
+import math
 import unittest
-from typing import List, Optional
 
 import torch
 
-from src.compel import EmbeddingsProvider
-from src.compel.conditioning_scheduler import StaticConditioningScheduler, ConditioningScheduler
+from src.compel.embeddings_provider import EmbeddingsProvider, DownweightMode
 from prompting_test_utils import DummyTokenizer, DummyTransformer, KNOWN_WORDS, KNOWN_WORDS_TOKEN_IDS, NullTransformer
 
-from src.compel.compel import Compel
 
-
-def make_dummy_compel():
-    tokenizer = DummyTokenizer()
-    text_encoder = DummyTransformer()
-    return Compel(tokenizer=tokenizer, text_encoder=text_encoder)
-
-
-def make_test_conditioning(text_encoder: DummyTransformer,
-                           tokenizer: DummyTokenizer,
-                           token_ids: List[int],
-                           truncate: bool=True,
-                           pad_mask_value: int=1
-                           ) -> torch.Tensor:
-    remaining_tokens = token_ids.copy()
-    conditioning = None
-    chunk_length = tokenizer.model_max_length-2
-    while True:
-        pre_padding = [tokenizer.bos_token_id]
-        chunk_token_ids = remaining_tokens[0:chunk_length]
-        remaining_tokens = remaining_tokens[chunk_length:]
-        pad_length = (tokenizer.model_max_length - len(chunk_token_ids) - 2)
-        post_padding = [tokenizer.eos_token_id] + \
-                       [tokenizer.pad_token_id] * pad_length
-        chunk_mask_tensor = torch.tensor([1] + [1] * len(chunk_token_ids) + [1] + [pad_mask_value] * pad_length, device=text_encoder.device)
-        chunk_token_ids_tensor = torch.tensor(pre_padding + chunk_token_ids + post_padding, device=text_encoder.device)
-
-        assert chunk_token_ids_tensor.shape[0] == tokenizer.model_max_length
-        this_conditioning = text_encoder(input_ids=chunk_token_ids_tensor.unsqueeze(0),
-                                         attention_mask=chunk_mask_tensor.unsqueeze(0)
-                                         ).last_hidden_state
-        conditioning = (
-            this_conditioning
-            if conditioning is None
-            else torch.cat([conditioning, this_conditioning], dim=1)
-        )
-        if truncate or len(remaining_tokens) == 0:
-            break
-
-    return conditioning
+def make_dummy_embeddings_provider(max_length=10, embedding_length=768, **kwargs) -> EmbeddingsProvider:
+    tokenizer = DummyTokenizer(max_length)
+    text_encoder = DummyTransformer(embedding_length=embedding_length)
+    return EmbeddingsProvider(tokenizer=tokenizer, text_encoder=text_encoder, **kwargs)
 
 
 class EmbeddingsProviderTestCase(unittest.TestCase):
 
     def test_tokenizing(self):
         tokenizer = DummyTokenizer(model_max_length=5)
-        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=NullTransformer(), padding_attention_mask_value=0)
+        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=NullTransformer(),
+                                                 padding_attention_mask_value=0)
 
         prompts = ['a b']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
         self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 0, 1, 5, 4], dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor([1.0] + [0.8] * 2 + [1.0] * 2)))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 1, 1, 0])))
 
         prompts = ['a b c']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
         self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 0, 1, 2, 5], dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] + [0.8] * 3 + [1.0]))))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 1, 1, 1])))
 
         prompts = ['']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
         self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 5, 4, 4, 4], dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] * 5))))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 0, 0, 0])))
 
         prompts = []
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[], device='cpu')
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[],
+                                                                                                      device='cpu')
         self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 5, 4, 4, 4], dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] * 5))))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 0, 0, 0])))
 
         # truncation
         prompts = ['a b c a b c a b c']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
         self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 0, 1, 2, 5], dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] + [0.8] * 3 + [1.0]))))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 1, 1, 1])))
 
     def test_long_tokenizing(self):
         tokenizer = DummyTokenizer(model_max_length=5)
-        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=NullTransformer(), truncate=False, padding_attention_mask_value=0)
+        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=NullTransformer(),
+                                                 truncate=False, padding_attention_mask_value=0)
 
         prompts = ['a b c c b a a c b']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
-        self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 0, 1, 2, 5] + [3, 2, 1, 0, 5] + [3, 0, 2, 1, 5], dtype=torch.int64)))
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
+        self.assertTrue(torch.equal(token_ids_tensor,
+                                    torch.tensor([3, 0, 1, 2, 5] + [3, 2, 1, 0, 5] + [3, 0, 2, 1, 5],
+                                                 dtype=torch.int64)))
         self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] + [0.8] * 3 + [1.0]) * 3)))
         self.assertTrue(torch.equal(mask, torch.tensor(([1, 1, 1, 1, 1] * 3))))
 
         prompts = ['a b c c b a a c b a']
-        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts, weights=[0.8], device='cpu')
-        self.assertTrue(torch.equal(token_ids_tensor, torch.tensor([3, 0, 1, 2, 5, 3, 2, 1, 0, 5, 3, 0, 2, 1, 5, 3, 0, 5, 4, 4], dtype=torch.int64)))
-        self.assertTrue(torch.equal(weights_tensor, torch.tensor(([1.0] + [0.8] * 3 + [1.0]) * 3 + ([1.0] + [0.8] + [1.0]) + ([1.0] * 2))))
+        token_ids_tensor, weights_tensor, mask = embeddings_provider.get_token_ids_and_expand_weights(prompts,
+                                                                                                      weights=[0.8],
+                                                                                                      device='cpu')
+        self.assertTrue(torch.equal(token_ids_tensor,
+                                    torch.tensor([3, 0, 1, 2, 5, 3, 2, 1, 0, 5, 3, 0, 2, 1, 5, 3, 0, 5, 4, 4],
+                                                 dtype=torch.int64)))
+        self.assertTrue(torch.equal(weights_tensor, torch.tensor(
+            ([1.0] + [0.8] * 3 + [1.0]) * 3 + ([1.0] + [0.8] + [1.0]) + ([1.0] * 2))))
         self.assertTrue(torch.equal(mask, torch.tensor([1, 1, 1, 1, 1] * 3 + [1, 1, 1] + [0, 0])))
 
-
     def test_tokenize_to_mask(self):
         tokenizer = DummyTokenizer(model_max_length=7)
         text_encoder = DummyTransformer()
-        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=text_encoder, padding_attention_mask_value=0)
+        embeddings_provider = EmbeddingsProvider(tokenizer=tokenizer, text_encoder=text_encoder,
+                                                 padding_attention_mask_value=0)
 
         fragments = ['a b']
-        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1]*len(fragments), device='cpu')
+        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1] * len(fragments),
+                                                                          device='cpu')
         self.assertSequenceEqual(mask.tolist(), [1, 1, 1, 1, 0, 0, 0])
 
         fragments = ['a b c a b c a']
-        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1]*len(fragments), device='cpu')
+        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1] * len(fragments),
+                                                                          device='cpu')
         self.assertSequenceEqual(mask.tolist(), [1, 1, 1, 1, 1, 1, 1])
 
         fragments = ['a', 'b c']
         _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1, 2], device='cpu')
         self.assertSequenceEqual(mask.tolist(), [1, 1, 1, 1, 1, 0, 0])
 
         # eos/bos only
         fragments = []
-        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1]*len(fragments), device='cpu')
+        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1] * len(fragments),
+                                                                          device='cpu')
         self.assertSequenceEqual(mask.tolist(), [1, 1, 0, 0, 0, 0, 0])
 
         # too long
         fragments = ['a b c a b c a b c a b c']
-        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1]*len(fragments), device='cpu')
+        _, _, mask = embeddings_provider.get_token_ids_and_expand_weights(fragments, weights=[1] * len(fragments),
+                                                                          device='cpu')
         self.assertSequenceEqual(mask.tolist(), [1, 1, 1, 1, 1, 1, 1])
 
+    def test_get_token_ids(self):
+        ep = make_dummy_embeddings_provider()
 
-class CompelTestCase(unittest.TestCase):
-
-
-    def test_basic_prompt(self):
-        tokenizer = DummyTokenizer()
-        text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder)
-
-        # test "a b c" makes it to the Conditioning intact for t=0, t=0.5, t=1
-        prompt = " ".join(KNOWN_WORDS[:3])
-        conditioning_scheduler = compel.make_conditioning_scheduler(prompt)
-        conditioning_scheduler_2 = compel.make_conditioning_scheduler(prompt)
-        expected_positive_conditioning = make_test_conditioning(text_encoder, tokenizer, KNOWN_WORDS_TOKEN_IDS[:3])
-        expected_negative_conditioning = make_test_conditioning(text_encoder, tokenizer, [])
-        self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
-                                                         expected_positive_conditioning,
-                                                         expected_negative_conditioning)
-
-
-    def test_basic_negative_prompt(self):
-        tokenizer = DummyTokenizer()
-        text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder)
-
-        # positive "a b c" negative "c b a" makes it to the Conditioning intact for t=0, t=0.5, t=1
-        positive_prompt = " ".join(KNOWN_WORDS[:3])
-        negative_prompt = " ".join(reversed(KNOWN_WORDS[:3]))
-        conditioning_scheduler = compel.make_conditioning_scheduler(positive_prompt, negative_prompt)
-        expected_positive_conditioning = make_test_conditioning(text_encoder, tokenizer, KNOWN_WORDS_TOKEN_IDS[:3])
-        expected_negative_conditioning = make_test_conditioning(text_encoder, tokenizer, list(reversed(KNOWN_WORDS_TOKEN_IDS[:3]))
-        )
-        self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
-                                                         expected_positive_conditioning,
-                                                         expected_negative_conditioning)
-
-    def test_too_long_prompt_truncate(self):
-        tokenizer = DummyTokenizer()
-        text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder)
-
-        positive_prompt = " ".join(KNOWN_WORDS[:3] * 40)
-        conditioning_scheduler = compel.make_conditioning_scheduler(positive_prompt)
-        expected_positive_conditioning = make_test_conditioning(text_encoder, tokenizer, KNOWN_WORDS_TOKEN_IDS[:3] * 40)
-        expected_negative_conditioning = make_test_conditioning(text_encoder, tokenizer, [])
-        self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
-                                                         expected_positive_conditioning,
-                                                         expected_negative_conditioning)
-
-
-    def test_too_long_prompt_notruncate(self):
-        tokenizer = DummyTokenizer(model_max_length=10)
-        text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
-
-        positive_prompt = " ".join(KNOWN_WORDS[:3] * 4)
-        conditioning_scheduler = compel.make_conditioning_scheduler(positive_prompt)
-        expected_positive_conditioning = make_test_conditioning(text_encoder,
-                                                                tokenizer,
-                                                                KNOWN_WORDS_TOKEN_IDS[:3] * 4,
-                                                                truncate=False)
-        expected_negative_conditioning = make_test_conditioning(text_encoder,
-                                                                tokenizer, [],
-                                                                truncate=False)
-        [expected_positive_conditioning, expected_negative_conditioning] = compel.pad_conditioning_tensors_to_same_length(
-            [expected_positive_conditioning, expected_negative_conditioning])
-
-        self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
-                                                         expected_positive_conditioning,
-                                                         expected_negative_conditioning)
-
-
-    def test_pad_conditioning_tensors_to_same_length(self):
-        tokenizer = DummyTokenizer(model_max_length=5)
-        text_encoder = DummyTransformer(embedding_length=7)
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length*2, text_encoder.embedding_length])
-        embeds_b = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        [padded_embeds_a, padded_embeds_b] = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-        self.assertEqual(padded_embeds_a.shape, padded_embeds_b.shape)
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([1, tokenizer.model_max_length*2, text_encoder.embedding_length])
-        [padded_embeds_a, padded_embeds_b] = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-        self.assertEqual(padded_embeds_a.shape, padded_embeds_b.shape)
-
-        embeds_a = torch.randn([tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([tokenizer.model_max_length*2, text_encoder.embedding_length])
-        [padded_embeds_a, padded_embeds_b] = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-        self.assertEqual(padded_embeds_a.shape, padded_embeds_b.shape)
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([2, tokenizer.model_max_length+1, text_encoder.embedding_length])
-        with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length+1])
-        embeds_b = torch.randn([1, tokenizer.model_max_length+1, text_encoder.embedding_length])
-        with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([tokenizer.model_max_length+1, text_encoder.embedding_length])
-        with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-
-        embeds_a = torch.randn([text_encoder.embedding_length])
-        embeds_b = torch.randn([text_encoder.embedding_length])
+        prompts = [" ".join(KNOWN_WORDS), " ".join(reversed(KNOWN_WORDS))]
+        expected_token_ids = [KNOWN_WORDS_TOKEN_IDS, list(reversed(KNOWN_WORDS_TOKEN_IDS))]
+        token_ids = ep.get_token_ids(prompts, include_start_and_end_markers=False)
+        self.assertEqual(expected_token_ids, token_ids)
+
+        expected_token_ids_with_bos_eos = [[ep.tokenizer.bos_token_id] + x + [ep.tokenizer.eos_token_id] for x in expected_token_ids]
+        print(expected_token_ids_with_bos_eos)
+        token_ids = ep.get_token_ids(prompts, include_start_and_end_markers=True)
+        self.assertEqual(expected_token_ids_with_bos_eos, token_ids)
+
+
+    def test_build_weighted_embeddings_tensor(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length)
+
+        # check that if fails if too short
+        token_ids = torch.tensor(KNOWN_WORDS_TOKEN_IDS)
+        per_token_weights = torch.tensor([1] * len(KNOWN_WORDS_TOKEN_IDS))
         with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
+            ep.build_weighted_embedding_tensor(token_ids, per_token_weights)
 
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([text_encoder.embedding_length])
-        with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-
-        embeds_a = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length])
-        embeds_b = torch.randn([1, tokenizer.model_max_length, text_encoder.embedding_length, 1, 1])
-        with self.assertRaises(ValueError):
-            _ = compel.pad_conditioning_tensors_to_same_length([embeds_a, embeds_b])
-
-
-    def test_device(self):
-        device = "mps" if torch.backends.mps.is_available() else "cuda" if torch.cuda.is_available() else "cpu"
-        tokenizer = DummyTokenizer()
-        text_encoder = DummyTransformer(device=device)
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder)
-
-        # test "a b c" makes it to the Conditioning intact for t=0, t=0.5, t=1
-        prompt = " ".join(KNOWN_WORDS[:3])
-        conditioning_scheduler = compel.make_conditioning_scheduler(prompt)
-        expected_positive_conditioning = make_test_conditioning(text_encoder, tokenizer, KNOWN_WORDS_TOKEN_IDS[:3])
-        expected_negative_conditioning = make_test_conditioning(text_encoder, tokenizer, [])
-        self.assert_constant_scheduling_matches_expected(conditioning_scheduler,
-                                                         expected_positive_conditioning,
-                                                         expected_negative_conditioning)
-
-
-    def assert_constant_scheduling_matches_expected(self,
-                                                    conditioning_scheduler: ConditioningScheduler,
-                                                    expected_positive_conditioning: torch.Tensor,
-                                                    expected_negative_conditioning: torch.Tensor):
-        self.assertIs(StaticConditioningScheduler, type(conditioning_scheduler))
-
-        conditioning_at_start = conditioning_scheduler.get_conditioning_for_step_pct(0)
-        self.assertTrue(torch.allclose(expected_positive_conditioning,
-                                       conditioning_at_start.positive_conditioning,
-                                       atol=1e-6))
-        self.assertTrue(torch.allclose(expected_negative_conditioning,
-                                       conditioning_at_start.negative_conditioning,
-                                       atol=1e-6))
-
-        conditioning_at_mid = conditioning_scheduler.get_conditioning_for_step_pct(0.5)
-        self.assertTrue(torch.allclose(expected_positive_conditioning,
-                                       conditioning_at_mid.positive_conditioning,
-                                       atol=1e-6))
-        self.assertTrue(torch.allclose(expected_negative_conditioning,
-                                       conditioning_at_mid.negative_conditioning,
-                                       atol=1e-6))
-
-        conditioning_at_end = conditioning_scheduler.get_conditioning_for_step_pct(1.0)
-        self.assertTrue(torch.allclose(expected_positive_conditioning,
-                                       conditioning_at_end.positive_conditioning,
-                                       atol=1e-6))
-        self.assertTrue(torch.allclose(expected_negative_conditioning,
-                                       conditioning_at_end.negative_conditioning,
-                                       atol=1e-6))
-
-
-
-    def test_long_bad_prompt(self):
-        max_length = 5
-        tokenizer = DummyTokenizer(model_max_length=max_length)
-        text_encoder = DummyTransformer()
-        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
+        # all weighted
+        empty_z = ep.build_weighted_embedding_tensor(torch.tensor([ep.tokenizer.bos_token_id] +
+                                                                  [ep.tokenizer.eos_token_id] +
+                                                                  [ep.tokenizer.pad_token_id] * (max_length - 2)),
+                                                     torch.tensor([1] * max_length))
+        token_ids = torch.tensor([ep.tokenizer.bos_token_id] + KNOWN_WORDS_TOKEN_IDS +
+                                 [ep.tokenizer.eos_token_id] +
+                                 [ep.tokenizer.pad_token_id] * (max_length - 2 - len(KNOWN_WORDS_TOKEN_IDS)))
+        unweighted_embeddings = ep.build_weighted_embedding_tensor(token_ids, torch.tensor([1] * len(token_ids)))
+
+        # confirm that the weighting works as expected (delta from empty)
+        weight = 2.0
+        weighted_embeddings_2 = ep.build_weighted_embedding_tensor(token_ids, torch.tensor([weight] * len(token_ids)))
+        self.assertTrue(torch.allclose(empty_z + (unweighted_embeddings-empty_z) * weight,
+                                       weighted_embeddings_2,
+                                       atol=1e-5))
+
+        # different weights at different places
+        rand_weights = 1 + torch.rand([len(token_ids)])
+        weighted_embeddings_rand = ep.build_weighted_embedding_tensor(token_ids, rand_weights)
+        weights_expanded = rand_weights.unsqueeze(1).expand(-1,768).unsqueeze(0)
+        self.assertTrue(torch.allclose(empty_z + (unweighted_embeddings-empty_z) * weights_expanded,
+                                       weighted_embeddings_rand,
+                                       atol=1e-7))
+
+        # mask
+        mask = torch.Tensor([1, 1, 1, 0, 0, 0, 0, 0, 0, 0])
+        weighted_embeddings_masked = ep.build_weighted_embedding_tensor(token_ids, torch.tensor([1] * len(token_ids)),
+                                                                        attention_mask=mask)
+        # note: test framework's masking is not expected to match the actual Text Encoder's - it just does a brainless multiply
+        self.assertTrue(torch.allclose(unweighted_embeddings * mask.unsqueeze(1).expand(-1,768).unsqueeze(0),
+                                       weighted_embeddings_masked,
+                                       atol=1e-7))
+
+        mask = torch.Tensor([0, 1, 1, 1, 0, 0, 1, 0, 1, 1])
+        weighted_embeddings_masked = ep.build_weighted_embedding_tensor(token_ids, torch.tensor([1] * len(token_ids)),
+                                                                        attention_mask=mask)
+        # note: test framework's masking is not expected to match the actual Text Encoder's - it just does a brainless multiply
+        self.assertTrue(torch.allclose(unweighted_embeddings * mask.unsqueeze(1).expand(-1,768).unsqueeze(0),
+                                       weighted_embeddings_masked,
+                                       atol=1e-7))
+
+
+
+    def test_upweighting_prompt_fragments(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length, padding_attention_mask_value=0)
+
+        text_batch = [[' '.join(KNOWN_WORDS)]]
+        fragment_weights_batch = [[1]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+
+        pad_length = (max_length-2-len(KNOWN_WORDS_TOKEN_IDS))
+        expected_token_ids = torch.tensor([ep.tokenizer.bos_token_id] + KNOWN_WORDS_TOKEN_IDS + [ep.tokenizer.eos_token_id] +
+                                          [ep.tokenizer.pad_token_id] * pad_length)
+        expected_mask = torch.tensor([1] + [1] * len(KNOWN_WORDS_TOKEN_IDS) + [1] + [0] * pad_length)
+        expected_embeddings = ep.build_weighted_embedding_tensor(expected_token_ids, torch.tensor([1] * len(expected_token_ids)), expected_mask)
+        self.assertTrue(torch.allclose(expected_embeddings, embeddings, atol=1e-8))
+
+        # weighted fragments
+        text_batch = [[KNOWN_WORDS[0], ' '.join(KNOWN_WORDS[1:3])]]
+        fragment_weights_batch = [[1, 2]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+        expected_weights = [1] + [1] + [2, 2] + [1] * 6
+        expected_embeddings = ep.build_weighted_embedding_tensor(expected_token_ids, torch.tensor(expected_weights), expected_mask)
+        self.assertTrue(torch.allclose(expected_embeddings, embeddings, atol=1e-8))
+
+
+    def test_downweighting_prompt_fragments_mask(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length, padding_attention_mask_value=0, downweight_mode=DownweightMode.MASK)
+
+        # downweighting
+        text_batch = [[KNOWN_WORDS[0], KNOWN_WORDS[1]]]
+        downweighted_fragment_weight = 0.5
+        fragment_weights_batch = [[1, downweighted_fragment_weight]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+        expected_token_ids = torch.tensor([ep.tokenizer.bos_token_id] + KNOWN_WORDS_TOKEN_IDS[0:2] +
+                             [ep.tokenizer.eos_token_id] +
+                             [ep.tokenizer.pad_token_id] * (max_length-4))
+        expected_weights = [1] + [1, downweighted_fragment_weight] + [1] * 7
+        # when downweighting, additionally blend against a version of the prompt with the downweighted term masked out
+        unweighted_mask = torch.tensor([1, 1, 1, 1] + [0] * 6)
+        downweighted_fragment_dropper_mask = torch.tensor([1, 1, 0, 1] + [0] * 6)
+
+        expected_embeddings_main_part = ep.build_weighted_embedding_tensor(expected_token_ids,
+                                                                           torch.tensor(expected_weights),
+                                                                           attention_mask=unweighted_mask)
+        expected_embeddings_downweighted_dropped = ep.build_weighted_embedding_tensor(expected_token_ids,
+                                                                                      torch.tensor(expected_weights),
+                                                                                      attention_mask=downweighted_fragment_dropper_mask)
+        # use tan, like in EmbeddingsProvider.get_embeddings_for_weighted_prompt_fragments()
+        downweighted_lerp_weight = math.tan((1.0 - downweighted_fragment_weight) * math.pi / 2)
+        blend_weights = [1.0, downweighted_lerp_weight]
+
+        expected_embeddings = EmbeddingsProvider.apply_embedding_weights(torch.cat([expected_embeddings_main_part,
+                                                                                    expected_embeddings_downweighted_dropped]).unsqueeze(0),
+                                                                         per_embedding_weights=blend_weights,
+                                                                         normalize=True)
+        self.assertTrue(torch.allclose(embeddings, expected_embeddings, atol=1e-8))
+
+    def test_downweighting_prompt_fragments_remove(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length, downweight_mode=DownweightMode.REMOVE)
+        # downweighting
+        text_batch = [[KNOWN_WORDS[0], KNOWN_WORDS[1]]]
+        downweighted_fragment_weight = 0.5
+        fragment_weights_batch = [[1, downweighted_fragment_weight]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+        expected_token_ids = torch.tensor([ep.tokenizer.bos_token_id] + KNOWN_WORDS_TOKEN_IDS[0:2] +
+                             [ep.tokenizer.eos_token_id] +
+                             [ep.tokenizer.pad_token_id] * (max_length-4))
+        expected_weights = [1] + [1, downweighted_fragment_weight] + [1] * 7
+        # when downweighting, additionally blend against a version of the prompt without the downweighted term
+        expected_token_ids_cut = torch.tensor([ep.tokenizer.bos_token_id] + KNOWN_WORDS_TOKEN_IDS[0:1] +
+                             [ep.tokenizer.eos_token_id] +
+                             [ep.tokenizer.pad_token_id] * (max_length-3))
+        expected_weights_cut = [1] + [1] + [1] * 8
+        expected_embeddings_main_part = ep.build_weighted_embedding_tensor(expected_token_ids, torch.tensor(expected_weights))
+        expected_embeddings_cut = ep.build_weighted_embedding_tensor(expected_token_ids_cut, torch.tensor(expected_weights_cut))
+
+        downweighted_lerp_weight = math.tan((1.0 - downweighted_fragment_weight) * math.pi / 2)
+        blend_weights = [1.0, downweighted_lerp_weight]
+
+        expected_embeddings = EmbeddingsProvider.apply_embedding_weights(torch.cat([expected_embeddings_main_part,
+                                                                                    expected_embeddings_cut]).unsqueeze(0),
+                                                                         per_embedding_weights=blend_weights,
+                                                                         normalize=True)
+        self.assertTrue(torch.allclose(expected_embeddings, embeddings, atol=1e-8))
+
+
+    def test_too_long_weighted_prompt_fragments_truncate(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length, truncate=True, padding_attention_mask_value=0)
+
+
+        # too many weighted fragments
+        text_batch = [[KNOWN_WORDS[0], ' '.join(reversed(KNOWN_WORDS*3)), ' '.join(KNOWN_WORDS[1:3], )]]
+        fragment_weights_batch = [[1, 2, 3]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+
+        expected_token_ids = torch.tensor([ep.tokenizer.bos_token_id] +
+                                          ([KNOWN_WORDS_TOKEN_IDS[0]] +
+                                          list(reversed(KNOWN_WORDS_TOKEN_IDS*3)) +
+                                          [KNOWN_WORDS_TOKEN_IDS[1]])[0:8] +
+                                          [ep.tokenizer.eos_token_id])
+        expected_weights = [1] + [1] + [2, 2, 2, 2, 2, 2, 2] + [1]
+        expected_embeddings = ep.build_weighted_embedding_tensor(expected_token_ids, torch.tensor(expected_weights))
+        self.assertTrue(torch.allclose(expected_embeddings, embeddings, atol=1e-8))
+
+
+    def test_too_long_weighted_prompt_fragments_notruncate(self):
+        max_length = 10
+        ep = make_dummy_embeddings_provider(max_length=max_length, truncate=False, padding_attention_mask_value=0)
+
+        # too many weighted fragments
+        text_batch = [[KNOWN_WORDS[0], ' '.join(reversed(KNOWN_WORDS*3)), ' '.join(KNOWN_WORDS[1:3], )]]
+        fragment_weights_batch = [[1, 2, 3]]
+        embeddings = ep.get_embeddings_for_weighted_prompt_fragments(text_batch, fragment_weights_batch)
+
+        expected_token_ids_part1 = ([ep.tokenizer.bos_token_id] +
+                                          [KNOWN_WORDS_TOKEN_IDS[0]] +
+                                          list(reversed(KNOWN_WORDS_TOKEN_IDS*3))[0:7] +
+                                          [ep.tokenizer.eos_token_id])
+        expected_token_ids_part2 = ([ep.tokenizer.bos_token_id] +
+                                          list(reversed(KNOWN_WORDS_TOKEN_IDS*3))[7:9] +
+                                          KNOWN_WORDS_TOKEN_IDS[1:3] +
+                                          [ep.tokenizer.eos_token_id] +
+                                          ([ep.tokenizer.pad_token_id] * 4))
+        expected_token_ids = torch.tensor(expected_token_ids_part1 + expected_token_ids_part2)
+        expected_weights = ([1] + [1] + [2, 2, 2, 2, 2, 2, 2] + [1] +
+                            [1] + [2, 2] + [3, 3] + [1] + ([1] * 4))
+        expected_mask = torch.Tensor([1] * 16 + [0] * 4)
+        expected_embeddings = ep.build_weighted_embedding_tensor(expected_token_ids, torch.tensor(expected_weights), attention_mask=expected_mask)
+        self.assertTrue(torch.allclose(expected_embeddings, embeddings, atol=1e-8))
 
-        positive_prompt = "a b c withLora(something)"
-        negative_prompt = '("a b c a b c a b", "c").blend()'
-        positive_conditioning = compel.build_conditioning_tensor(positive_prompt)
-        negative_conditioning = compel.build_conditioning_tensor(negative_prompt)
 
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `compel-1.1.2/test/test_prompt_parser.py` & `compel-1.1.3.dev0/test/test_prompt_parser.py`

 * *Files identical despite different names*

