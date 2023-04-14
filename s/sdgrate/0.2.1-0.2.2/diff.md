# Comparing `tmp/sdgrate-0.2.1.tar.gz` & `tmp/sdgrate-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgrate-0.2.1.tar", last modified: Thu Mar 23 15:19:14 2023, max compression
+gzip compressed data, was "sdgrate-0.2.2.tar", last modified: Fri Apr 14 18:27:58 2023, max compression
```

## Comparing `sdgrate-0.2.1.tar` & `sdgrate-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-03-23 15:19:14.855845 sdgrate-0.2.1/
--rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.1/MANIFEST.in
--rw-r--r--   0 damian     (501) staff       (20)    10171 2023-03-23 15:19:14.855652 sdgrate-0.2.1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     9596 2023-03-23 15:18:24.000000 sdgrate-0.2.1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      940 2023-03-23 15:18:48.000000 sdgrate-0.2.1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-03-23 15:19:14.855882 sdgrate-0.2.1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-03-23 15:19:14.852107 sdgrate-0.2.1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-03-23 15:19:14.854542 sdgrate-0.2.1/src/sdgrate/
--rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.1/src/sdgrate/LibreBaskerville-DpdE.ttf
--rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.1/src/sdgrate/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.1/src/sdgrate/checkpoint_merger_mbw.py
--rw-r--r--   0 damian     (501) staff       (20)    27750 2023-03-23 15:17:51.000000 sdgrate-0.2.1/src/sdgrate/grate.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-03-23 15:19:14.855486 sdgrate-0.2.1/src/sdgrate.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    10171 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      376 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       45 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/entry_points.txt
--rw-r--r--   0 damian     (501) staff       (20)       82 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        8 2023-03-23 15:19:14.000000 sdgrate-0.2.1/src/sdgrate.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.079668 sdgrate-0.2.2/
+-rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.2/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.2/MANIFEST.in
+-rw-r--r--   0 damian     (501) staff       (20)    10485 2023-04-14 18:27:58.079545 sdgrate-0.2.2/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     9909 2023-04-14 18:27:34.000000 sdgrate-0.2.2/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      953 2023-04-14 18:10:52.000000 sdgrate-0.2.2/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 18:27:58.079706 sdgrate-0.2.2/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.075359 sdgrate-0.2.2/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.078560 sdgrate-0.2.2/src/sdgrate/
+-rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.2/src/sdgrate/LibreBaskerville-DpdE.ttf
+-rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.2/src/sdgrate/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.2/src/sdgrate/checkpoint_merger_mbw.py
+-rw-r--r--   0 damian     (501) staff       (20)    28585 2023-04-14 18:17:41.000000 sdgrate-0.2.2/src/sdgrate/grate.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.079328 sdgrate-0.2.2/src/sdgrate.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    10485 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      376 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       45 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/entry_points.txt
+-rw-r--r--   0 damian     (501) staff       (20)       90 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        8 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/top_level.txt
```

### Comparing `sdgrate-0.2.1/LICENSE` & `sdgrate-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.1/PKG-INFO` & `sdgrate-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sdgrate
-Version: 0.2.1
-Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
-Author-email: Damian Stewart <null@damianstewart.com>
-Project-URL: Homepage, https://github.com/damian0815/grate
-Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Grate
 
 Make a matrix of images by running the same prompt through multiple Stable Diffusion models. 
 
 ![Demo output of a grid of prompts rendered with three different stable diffusion models](grate-demo.png)
 
 Supports huggingface repo ids, local CompVis-style `.ckpt` files, and paths to local folder hierarchies containing diffusers-format models. Uses DDPM++2 sampler with 15 steps for all generations.
@@ -86,15 +72,15 @@
              [--disable_nsfw_checker] [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
-             [--save_merge_float32]
+             [--save_merge_float32] [--use_penultimate_clip_layer]
 
 Generates a grid of images by running a set of prompts through different
 Stable Diffusion models. Optionally, merge models together: if one or more of
 the --merge_ options is passed, grate will produce multiple merged models
 using all possible combinations of the passed values, and render each on its
 own row in the output image. For example, grate --merge_alphas 0.333 0.667
 --merge_algorithm weighted_sum sigmoid will produce an output image with 4
@@ -161,16 +147,24 @@
                         (Optional) Override the merge alpha with a text-
                         encoder-specific alpha.
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
+  --use_penultimate_clip_layer
+                        (Optional) Use the outputs from penultimate (second to
+                        last) CLIP hidden layer.
+
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
+
+## Changelog
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sdgrate-0.2.1/README.md` & `sdgrate-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: sdgrate
+Version: 0.2.2
+Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
+Author-email: Damian Stewart <null@damianstewart.com>
+Project-URL: Homepage, https://github.com/damian0815/grate
+Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Grate
 
 Make a matrix of images by running the same prompt through multiple Stable Diffusion models. 
 
 ![Demo output of a grid of prompts rendered with three different stable diffusion models](grate-demo.png)
 
 Supports huggingface repo ids, local CompVis-style `.ckpt` files, and paths to local folder hierarchies containing diffusers-format models. Uses DDPM++2 sampler with 15 steps for all generations.
@@ -72,15 +86,15 @@
              [--disable_nsfw_checker] [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
-             [--save_merge_float32]
+             [--save_merge_float32] [--use_penultimate_clip_layer]
 
 Generates a grid of images by running a set of prompts through different
 Stable Diffusion models. Optionally, merge models together: if one or more of
 the --merge_ options is passed, grate will produce multiple merged models
 using all possible combinations of the passed values, and render each on its
 own row in the output image. For example, grate --merge_alphas 0.333 0.667
 --merge_algorithm weighted_sum sigmoid will produce an output image with 4
@@ -147,16 +161,24 @@
                         (Optional) Override the merge alpha with a text-
                         encoder-specific alpha.
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
+  --use_penultimate_clip_layer
+                        (Optional) Use the outputs from penultimate (second to
+                        last) CLIP hidden layer.
+
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
+
+## Changelog
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sdgrate-0.2.1/pyproject.toml` & `sdgrate-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "sdgrate"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A grid image generator for Stable Diffusion models based on 🧨diffusers."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "diffusers[torch] >=0.13, <0.14",
+    "diffusers[torch]>=0.13",
+    "compel~=1.1.3",
     "huggingface-hub",
     "Pillow",
     "tqdm",
     "transformers",
     "safetensors"
 ]
```

### Comparing `sdgrate-0.2.1/src/sdgrate/LibreBaskerville-DpdE.ttf` & `sdgrate-0.2.2/src/sdgrate/LibreBaskerville-DpdE.ttf`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.1/src/sdgrate/checkpoint_merger_mbw.py` & `sdgrate-0.2.2/src/sdgrate/checkpoint_merger_mbw.py`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.1/src/sdgrate/grate.py` & `sdgrate-0.2.2/src/sdgrate/grate.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import argparse
 import pathlib
 from typing import Optional
 
 import torch
+from compel import Compel
 from diffusers.pipelines.stable_diffusion.convert_from_ckpt import load_pipeline_from_original_stable_diffusion_ckpt
 from diffusers import StableDiffusionPipeline, DPMSolverMultistepScheduler
 from PIL import Image, ImageDraw, ImageFont
 from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.utils import is_xformers_available
 from tqdm import tqdm
 
@@ -177,14 +178,15 @@
                device: str = None,
                batch_size=1,
                sample_w=512,
                sample_h=512,
                cfg=7.5,
                num_inference_steps=15,  # ddpm++ solver: 15 is typically enough
                disable_nsfw_checker: bool = False,
+               use_penultimate_clip_layer: bool = False
                ) -> list[Image]:
     # ddpm++
     pipeline.scheduler = DPMSolverMultistepScheduler.from_config(pipeline.scheduler.config,
                                                                  algorithm_type="dpmsolver++")
     if device is None:
         device = 'cuda' if torch.cuda.is_available() else 'mps' if torch.backends.mps.is_available() else 'cpu'
     if device == 'cuda':
@@ -195,19 +197,23 @@
     pipeline = pipeline.to(device)
     if disable_nsfw_checker:
         pipeline.safety_checker = disable_nsfw_safety_checker
     images = []
     negative_prompts = negative_prompts or [""] * len(prompts)
     batches = chunk_list(list(zip(prompts, negative_prompts, seeds)), batch_size)
     progress_bar = tqdm(list(batches))
+    compel = Compel(tokenizer=pipeline.tokenizer,
+                    text_encoder=pipeline.text_encoder,
+                    use_penultimate_clip_layer=use_penultimate_clip_layer)
     for batch in progress_bar:
         batch_prompts, batch_negative_prompts, batch_seeds = zip(*batch)
         print(f" - {batch_prompts}")
         generator_device = 'cpu' if device == 'mps' else device
         manual_seed_generators = [torch.Generator(generator_device).manual_seed(seed) for seed in batch_seeds]
+        positive_embeds = compel(batch_prompts)
         pipeline_output: StableDiffusionPipelineOutput = pipeline(prompt=list(batch_prompts),
                                                                   negative_prompt=list(batch_negative_prompts),
                                                                   generator=manual_seed_generators,
                                                                   width=sample_w,
                                                                   height=sample_h,
                                                                   num_inference_steps=num_inference_steps,
                                                                   guidance_scale=cfg)
@@ -299,14 +305,15 @@
                size: tuple[int, int],
                batch_size: int,
                inference_steps: int = 15,
                save_partial_filename: Optional[str] = None,
                local_files_only: bool = False,
                merge_config: Optional[dict] = None,
                disable_nsfw_checker: bool = False,
+               use_penultimate_clip_layer: bool = False,
                ) -> Image:
     all_images = []
     print(f"{len(prompts)} prompts")
 
     row_labels = []
 
     def save_partial_if_requested():
@@ -350,15 +357,16 @@
                                     seeds=seeds,
                                     pipeline=pipeline,
                                     device=device,
                                     batch_size=batch_size,
                                     cfg=cfg,
                                     num_inference_steps=inference_steps,
                                     sample_w=size[0], sample_h=size[1],
-                                    disable_nsfw_checker=disable_nsfw_checker,)
+                                    disable_nsfw_checker=disable_nsfw_checker,
+                                    use_penultimate_clip_layer=use_penultimate_clip_layer)
             all_images += row_images
             save_partial_if_requested()
 
             save_merge_path_prefix = merge_config.get('save_merge_path_prefix', None)
             if save_merge_path_prefix is not None:
                 save_half = merge_config.get('save_merge_half', True)
                 if save_half:
@@ -379,15 +387,16 @@
                                     seeds=seeds,
                                     pipeline=pipeline,
                                     device=device,
                                     batch_size=batch_size,
                                     cfg=cfg,
                                     num_inference_steps=inference_steps,
                                     sample_w=size[0], sample_h=size[1],
-                                    disable_nsfw_checker=disable_nsfw_checker,)
+                                    disable_nsfw_checker=disable_nsfw_checker,
+                                    use_penultimate_clip_layer=use_penultimate_clip_layer)
             all_images += row_images
             save_partial_if_requested()
             del pipeline
         grid_image = make_image_grid(all_images, len(repo_ids_or_paths), len(prompts), row_labels, prompts)
 
     return grid_image
 
@@ -500,14 +509,17 @@
     parser.add_argument("--save_merge_path_prefix",
                         required=False,
                         type=str,
                         help="(Optional) If doing a merge, save all merge combinations using this path as a prefix.")
     parser.add_argument("--save_merge_float32",
                         action="store_true",
                         help="(Optional) If saving merges, save with float32 precision (default is float16).")
+    parser.add_argument("--use_penultimate_clip_layer",
+                        action="store_true",
+                        help="(Optional) Use the outputs from penultimate (second to last) CLIP hidden layer.")
     args = parser.parse_args()
 
 
     def use_arg_list_or_expand_or_default(arg: list, required_count: int, default: list|None) -> list:
         if arg is None:
             return default
         elif len(arg) == 1:
@@ -554,12 +566,13 @@
                device=args.device,
                size=(args.width, args.height),
                batch_size=args.batch_size,
                cfg=args.cfg,
                inference_steps=args.steps,
                local_files_only=args.local_files_only,
                save_partial_filename=args.output_path,
-               disable_nsfw_checker=args.disable_nsfw_checker,)
+               disable_nsfw_checker=args.disable_nsfw_checker,
+               use_penultimate_clip_layer=args.use_penultimate_clip_layer)
     print(f"grate saved to {args.output_path}")
 
 if __name__ == '__main__':
     main()
```

### Comparing `sdgrate-0.2.1/src/sdgrate.egg-info/PKG-INFO` & `sdgrate-0.2.2/src/sdgrate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgrate
-Version: 0.2.1
+Version: 0.2.2
 Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/grate
 Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -86,15 +86,15 @@
              [--disable_nsfw_checker] [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
-             [--save_merge_float32]
+             [--save_merge_float32] [--use_penultimate_clip_layer]
 
 Generates a grid of images by running a set of prompts through different
 Stable Diffusion models. Optionally, merge models together: if one or more of
 the --merge_ options is passed, grate will produce multiple merged models
 using all possible combinations of the passed values, and render each on its
 own row in the output image. For example, grate --merge_alphas 0.333 0.667
 --merge_algorithm weighted_sum sigmoid will produce an output image with 4
@@ -161,16 +161,24 @@
                         (Optional) Override the merge alpha with a text-
                         encoder-specific alpha.
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
+  --use_penultimate_clip_layer
+                        (Optional) Use the outputs from penultimate (second to
+                        last) CLIP hidden layer.
+
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
+
+## Changelog
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
```

