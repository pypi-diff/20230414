# Comparing `tmp/aihandler-1.8.21.tar.gz` & `tmp/aihandler-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.8.21.tar", last modified: Sun Apr  2 03:07:03 2023, max compression
+gzip compressed data, was "aihandler-1.9.0.tar", last modified: Fri Apr 14 21:01:51 2023, max compression
```

## Comparing `aihandler-1.8.21.tar` & `aihandler-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:07:03.585064 aihandler-1.8.21/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-02 03:06:50.000000 aihandler-1.8.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-02 03:07:03.585064 aihandler-1.8.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-02 03:06:50.000000 aihandler-1.8.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 03:07:03.585064 aihandler-1.8.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-02 03:06:50.000000 aihandler-1.8.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:07:03.581064 aihandler-1.8.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:07:03.585064 aihandler-1.8.21/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    47486 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-02 03:06:50.000000 aihandler-1.8.21/src/aihandler/socket_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:07:03.585064 aihandler-1.8.21/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-02 03:07:03.000000 aihandler-1.8.21/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-02 03:07:03.000000 aihandler-1.8.21/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 03:07:03.000000 aihandler-1.8.21/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-02 03:07:03.000000 aihandler-1.8.21/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-02 03:07:03.000000 aihandler-1.8.21/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 21:01:41.000000 aihandler-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-14 21:01:51.278233 aihandler-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-14 21:01:41.000000 aihandler-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:01:51.278233 aihandler-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 21:01:41.000000 aihandler-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.274233 aihandler-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50075 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.8.21/LICENSE` & `aihandler-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/PKG-INFO` & `aihandler-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.8.21
+Version: 1.9.0
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
@@ -47,15 +47,15 @@
 - Cuda capable GPU
 - 16gb+ ram
 
 [For Windows, follow windows branch instructions](https://github.com/Capsize-Games/aihandler/tree/develop-windows)
 
 Install
 ```
-pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.14.0.ckpt_fix.tar.gz
+pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.15.0.ckpt_fix_0.0.1.tar.gz
 pip install https://github.com/w4ffl35/transformers/archive/refs/tags/tensor_fix-v1.0.2.tar.gz
 pip install aihandler
 ```
 
 #### Optional
 
 These are optional instructions for installing TensorRT and Deepspeed for Windows
```

### Comparing `aihandler-1.8.21/README.md` & `aihandler-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - Cuda capable GPU
 - 16gb+ ram
 
 [For Windows, follow windows branch instructions](https://github.com/Capsize-Games/aihandler/tree/develop-windows)
 
 Install
 ```
-pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.14.0.ckpt_fix.tar.gz
+pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.15.0.ckpt_fix_0.0.1.tar.gz
 pip install https://github.com/w4ffl35/transformers/archive/refs/tags/tensor_fix-v1.0.2.tar.gz
 pip install aihandler
 ```
 
 #### Optional
 
 These are optional instructions for installing TensorRT and Deepspeed for Windows
```

### Comparing `aihandler-1.8.21/setup.py` & `aihandler-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import sys
 import platform
 from setuptools import setup, find_packages
 
 
 install_requires = [
-    "torch==1.13.1",
-    "torchvision==0.14.1",
-    "torchaudio==0.13.1",
+    "torch==2.0.0",
+    "torchvision==0.15.1",
+    "torchaudio==2.0.1",
     "einops==0.6.0",
     "ninja==1.11.1",
     "JIT==0.2.7",
-    "triton==2.0.0.dev20221202",
+    "triton==2.0.0",
     "tqdm==4.65.0",
-    "xformers==0.0.16",
+    "xformers==0.0.18",
     "bitsandbytes==0.37.0",
     "omegaconf==2.3.0",
     "accelerate==0.18.0",
     "controlnet_aux==0.0.1",
     "huggingface-hub==0.13.3",
     "numpy==1.23.5",
     "Pillow==9.4.0",
@@ -31,29 +31,29 @@
     "requests==2.28.2",
     "requests-oauthlib==1.3.1",
     "safetensors==0.3.0",
     "scipy==1.10.1",
     "tensorflow==2.12.0",
     "tokenizers==0.13.2",
     "tqdm==4.65.0",
-    "xformers==0.0.16",
     "charset-normalizer==3.1.0",
     "opencv-python==4.7.0.72",
     "setuptools==65.5.1",
     "sympy==1.11.1",
     "typing_extensions==4.5.0",
     "urllib3==1.26.15",
-    "diffusers==0.14.0",
-    "transformers==4.27.4"
+    "diffusers==0.15.0",
+    "transformers==4.27.4",
+    "compel==1.1.3",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.8.21",
+    version="1.9.0",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.8.21/src/aihandler/controlnet_utils.py` & `aihandler-1.9.0/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler/database.py` & `aihandler-1.9.0/src/aihandler/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from aihandler.qtvar import Var, BooleanVar, IntVar, StringVar, DoubleVar, FloatVar
+from aihandler.qtvar import Var, BooleanVar, IntVar, StringVar, DoubleVar, FloatVar, ListVar
 from aihandler.settings import \
     DEFAULT_MODEL, \
     DEFAULT_SCHEDULER, \
     DEFAULT_CANVAS_COLOR, \
     DEFAULT_GRID_COLOR, \
     DEFAULT_WORKING_SIZE
 
@@ -237,13 +237,27 @@
         self.controlnet_random_seed = BooleanVar(app)
         self.controlnet_model_var = StringVar(app, "Stable Diffusion Inpaint V2")
         self.controlnet_scheduler_var = StringVar(app, DEFAULT_SCHEDULER)
         self.controlnet_prompt_triggers = StringVar(app, "")
         self.controlnet_n_samples = IntVar(app, 1)
         self.controlnet_strength = DoubleVar(app, default_strength)
 
+        self.txt2vid_steps = IntVar(app, 20)
+        self.txt2vid_ddim_eta = DoubleVar(app, 0.5)
+        self.txt2vid_height = IntVar(app, 512)
+        self.txt2vid_width = IntVar(app, 512)
+        self.txt2vid_scale = DoubleVar(app, default_scale)
+        self.txt2vid_seed = IntVar(app, 42)
+        self.txt2vid_random_seed = BooleanVar(app)
+        self.txt2vid_model_var = StringVar(app, DEFAULT_MODEL)
+        self.txt2vid_scheduler_var = StringVar(app, DEFAULT_SCHEDULER)
+        self.txt2vid_prompt_triggers = StringVar(app, "")
+        self.txt2vid_n_samples = IntVar(app, 1)
+
+        self.available_extensions = ListVar(app, [])
+
     def set_namespace(self, namespace):
         self.namespace = namespace
 
     def reset_settings_to_default(self):
         self.initialize()
```

### Comparing `aihandler-1.8.21/src/aihandler/llmrunner.py` & `aihandler-1.9.0/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler/logger.py` & `aihandler-1.9.0/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler/offline_client.py` & `aihandler-1.9.0/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.0/src/aihandler/pyqt_offline_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,14 +171,18 @@
         self.create_worker_thread()
 
     def force_request_worker_quit(self):
         if self.request_worker_thread.isRunning():
             self.request_worker_thread.terminate()
             self.request_worker_thread.wait()
 
+    def cancel_current_request(self):
+        # cancel the current operation
+        pass
+
 
 class RequestWorker(QtCore.QObject):
     client: OfflineClient
     signalStatus = QtCore.pyqtSignal(str)
     running = False
 
     def __init__(self, parent=None, client=None, callback=None):
```

### Comparing `aihandler-1.8.21/src/aihandler/runner.py` & `aihandler-1.9.0/src/aihandler/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import io
 from aihandler.settings import LOG_LEVEL
 from aihandler.logger import logger
 import logging
 logging.disable(LOG_LEVEL)
 from PIL import Image
 from controlnet_aux import HEDdetector, MLSDdetector, OpenposeDetector
+from compel import Compel
 
 os.environ["DISABLE_TELEMETRY"] = "1"
 os.environ["HF_HUB_OFFLINE"] = "1"
 os.environ["TRANSFORMERS_OFFLINE"] = "1"
 
 
 def image_to_byte_array(image):
@@ -72,28 +73,32 @@
     txt2img = None
     img2img = None
     pix2pix = None
     outpaint = None
     depth2img = None
     controlnet = None
     superresolution = None
+    txt2vid = None
     state = None
     local_files_only = True
 
     # memory settings
     _use_last_channels = True
     _use_enable_sequential_cpu_offload = True
     _use_attention_slicing = True
     _use_tf32 = True
     _use_cudnn_benchmark = True
     _use_enable_vae_slicing = True
     _use_xformers = False
     _settings = None
     _action = None
     do_change_scheduler = False
+    embeds_loaded = False
+    controlnet_type = "canny"
+    options = {}
 
     @property
     def do_mega_scale(self):
         return self.is_superresolution
 
     @property
     def action(self):
@@ -112,14 +117,18 @@
         return self.action == "outpaint"
 
     @property
     def is_txt2img(self):
         return self.action == "txt2img"
 
     @property
+    def is_txt2vid(self):
+        return self.action == "txt2vid"
+
+    @property
     def is_img2img(self):
         return self.action == "img2img"
 
     @property
     def is_controlnet(self):
         return self.action == "controlnet"
 
@@ -160,15 +169,18 @@
             raise Exception("Chicken / egg problem, model path not set")
 
         if self.is_ckpt_model or self.is_safetensors:
             # skip scheduler for ckpt models
             return None
         # set logging level to fatal for all loggers
         import diffusers
-        scheduler_class = getattr(diffusers, self.schedulers[self.scheduler_name])
+        if self.is_txt2vid:
+            scheduler_class = getattr(diffusers, "DPMSolverMultistepScheduler")
+        else:
+            scheduler_class = getattr(diffusers, self.schedulers[self.scheduler_name])
         kwargs = {
             "subfolder": "scheduler"
         }
         # check if self.scheduler_name contains ++
         if self.scheduler_name.startswith("DPM"):
             kwargs["lower_order_final"] = self.num_inference_steps < 15
             if self.scheduler_name.find("++") != -1:
@@ -207,14 +219,16 @@
             return self.outpaint is not None
         elif self.is_depth2img:
             return self.depth2img is not None
         elif self.is_superresolution:
             return self.superresolution is not None
         elif self.is_controlnet:
             return self.controlnet is not None
+        elif self.is_txt2vid:
+            return self.txt2vid is not None
 
     @property
     def pipe(self):
         if self.is_txt2img:
             return self.txt2img
         elif self.is_img2img:
             return self.img2img
@@ -224,14 +238,16 @@
             return self.depth2img
         elif self.is_pix2pix:
             return self.pix2pix
         elif self.is_superresolution:
             return self.superresolution
         elif self.is_controlnet:
             return self.controlnet
+        elif self.is_txt2vid:
+            return self.txt2vid
         else:
             raise ValueError(f"Invalid action {self.action} unable to get pipe")
 
     @pipe.setter
     def pipe(self, value):
         if self.is_txt2img:
             self.txt2img = value
@@ -243,20 +259,22 @@
             self.depth2img = value
         elif self.is_pix2pix:
             self.pix2pix = value
         elif self.is_superresolution:
             self.superresolution = value
         elif self.is_controlnet:
             self.controlnet = value
+        elif self.is_txt2vid:
+            self.txt2vid = value
         else:
             raise ValueError(f"Invalid action {self.action} unable to set pipe")
 
     @property
     def use_last_channels(self):
-        return self._use_last_channels
+        return self._use_last_channels and not self.is_txt2vid
 
     @use_last_channels.setter
     def use_last_channels(self, value):
         self._use_last_channels = value
 
     @property
     def use_enable_sequential_cpu_offload(self):
@@ -311,14 +329,15 @@
     @use_xformers.setter
     def use_xformers(self, value):
         self._use_xformers = value
 
     @property
     def action_diffuser(self):
         from diffusers import (
+            DiffusionPipeline,
             StableDiffusionPipeline,
             StableDiffusionImg2ImgPipeline,
             StableDiffusionInstructPix2PixPipeline,
             StableDiffusionInpaintPipeline,
             StableDiffusionDepth2ImgPipeline,
             StableDiffusionUpscalePipeline,
             StableDiffusionControlNetPipeline
@@ -334,14 +353,16 @@
             return StableDiffusionInpaintPipeline
         elif self.is_depth2img:
             return StableDiffusionDepth2ImgPipeline
         elif self.is_superresolution:
             return StableDiffusionUpscalePipeline
         elif self.is_controlnet:
             return StableDiffusionControlNetPipeline
+        elif self.is_txt2vid:
+            return DiffusionPipeline
         else:
             raise ValueError("Invalid action")
 
     @property
     def is_ckpt_model(self):
         return self._is_ckpt_file(self.model)
 
@@ -354,26 +375,58 @@
         data_type = torch.half if self.cuda_is_available else torch.float
         return torch.float16 if self.use_xformers else data_type
 
     @property
     def device(self):
         return "cuda" if self.cuda_is_available else "cpu"
 
+    @property
+    def controlnet_model(self):
+        if self.controlnet_type == "canny":
+            return "lllyasviel/sd-controlnet-canny"
+        elif self.controlnet_type == "depth":
+            return "fusing/stable-diffusion-v1-5-controlnet-depth"
+        elif self.controlnet_type == "hed":
+            return "fusing/stable-diffusion-v1-5-controlnet-hed"
+        elif self.controlnet_type == "mlsd":
+            return "fusing/stable-diffusion-v1-5-controlnet-mlsd"
+        elif self.controlnet_type == "normal":
+            return "fusing/stable-diffusion-v1-5-controlnet-normal"
+        elif self.controlnet_type == "scribble":
+            return "fusing/stable-diffusion-v1-5-controlnet-scribble"
+        elif self.controlnet_type == "segmentation":
+            return "fusing/stable-diffusion-v1-5-controlnet-seg"
+        elif self.controlnet_type == "openpose":
+            return "fusing/stable-diffusion-v1-5-controlnet-openpose"
+
+    @property
+    def has_internet_connection(self):
+        try:
+            response = requests.get('https://huggingface.co/')
+            return True
+        except requests.ConnectionError:
+            return False
+
+    @property
+    def txt2vid_file(self):
+        return os.path.join(self.model_base_path, "videos", f"{self.prompt}_{self.seed}.mp4")
+
     def _clear_memory(self):
         torch.cuda.empty_cache()
         gc.collect()
 
     def move_models_to_cpu(self, skip_model):
         self.txt2img.to("cpu") if self.txt2img and skip_model != "txt2img" else None
         self.img2img.to("cpu") if self.img2img and skip_model != "img2img" else None
         self.pix2pix.to("cpu") if self.pix2pix and skip_model != "pix2pix" else None
         self.outpaint.to("cpu") if self.outpaint and skip_model != "outpaint" else None
         self.depth2img.to("cpu") if self.depth2img and skip_model != "depth2img" else None
         self.superresolution.to("cpu") if self.superresolution and skip_model != "superresolution" else None
         self.controlnet.to("cpu") if self.controlnet and skip_model != "controlnet" else None
+        self.txt2vid.to("cpu") if self.txt2vid and skip_model != "txt2vid" else None
         self._clear_memory()
 
     def load_controlnet_from_ckpt(self, pipeline):
         from diffusers import ControlNetModel, UniPCMultistepScheduler
         from diffusers import StableDiffusionControlNetPipeline
         controlnet = ControlNetModel.from_pretrained(
             self.controlnet_model,
@@ -393,35 +446,14 @@
             requires_safety_checker=pipeline.requires_safety_checker
         )
         if self.data["options"]["enable_model_cpu_offload"]:
             pipeline.scheduler = UniPCMultistepScheduler.from_config(self.pipe.scheduler.config)
             pipeline.enable_model_cpu_offload()
         return pipeline
 
-    controlnet_type = "canny"
-
-    @property
-    def controlnet_model(self):
-        if self.controlnet_type == "canny":
-            return "lllyasviel/sd-controlnet-canny"
-        elif self.controlnet_type == "depth":
-            return "fusing/stable-diffusion-v1-5-controlnet-depth"
-        elif self.controlnet_type == "hed":
-            return "fusing/stable-diffusion-v1-5-controlnet-hed"
-        elif self.controlnet_type == "mlsd":
-            return "fusing/stable-diffusion-v1-5-controlnet-mlsd"
-        elif self.controlnet_type == "normal":
-            return "fusing/stable-diffusion-v1-5-controlnet-normal"
-        elif self.controlnet_type == "scribble":
-            return "fusing/stable-diffusion-v1-5-controlnet-scribble"
-        elif self.controlnet_type == "segmentation":
-            return "fusing/stable-diffusion-v1-5-controlnet-seg"
-        elif self.controlnet_type == "openpose":
-            return "fusing/stable-diffusion-v1-5-controlnet-openpose"
-
     def load_controlnet(self):
         from diffusers import ControlNetModel
         return ControlNetModel.from_pretrained(
             self.controlnet_model,
             local_files_only=self.local_files_only,
             torch_dtype=self.data_type
         )
@@ -518,21 +550,19 @@
 
             if hasattr(self.pipe, "safety_checker") and self.do_nsfw_filter:
                 self.safety_checker = self.pipe.safety_checker
 
         # store the model_path
         self.pipe.model_path = self.model_path
 
-        #self._load_embeddings()
         embeddings_folder = os.path.join(self.model_base_path, "embeddings")
         self.load_learned_embed_in_clip(embeddings_folder)
 
         self._apply_memory_efficient_settings()
 
-    embeds_loaded = False
     def load_learned_embed_in_clip(self, learned_embeds_path):
         if self.embeds_loaded:
             return
         self.embeds_loaded = True
         if os.path.exists(learned_embeds_path):
             logger.info("Loading embeddings...")
             tokens = []
@@ -578,26 +608,14 @@
 
                     self.pipe.text_encoder = text_encoder
                     self.pipe.tokenizer = tokenizer
                 except Exception as e:
                     logger.warning(e)
             self.settings_manager.settings.available_embeddings.set(", ".join(tokens))
 
-    def _load_embeddings(self):
-        # in the embeddings foloder we will get all pt files and merge them into the model
-        embeddings_folder = os.path.join(self.model_base_path, "embeddings")
-        if os.path.exists(embeddings_folder):
-            logger.info("Loading embeddings...")
-            for f in os.listdir(embeddings_folder):
-                if f.endswith(".pt"):
-                    logger.debug(f"Loading {f}")
-                    embedding = torch.load(os.path.join(embeddings_folder, f))
-        else:
-            print("No embeddings folder found", embeddings_folder)
-
     def _apply_memory_efficient_settings(self):
         logger.debug("Applying memory efficient settings")
         # enhance with memory settings
         if self.use_last_channels:
             logger.debug("Enabling torch.channels_last")
             self.pipe.unet.to(memory_format=torch.channels_last)
         else:
@@ -749,14 +767,16 @@
         logger.debug(f"  use_enable_sequential_cpu_offload: {self.use_enable_sequential_cpu_offload}")
         logger.debug(f"  use_attention_slicing: {self.use_attention_slicing}")
         logger.debug(f"  use_tf32: {self.use_tf32}")
         logger.debug(f"  use_cudnn_benchmark: {self.use_cudnn_benchmark}")
         logger.debug(f"  use_enable_vae_slicing: {self.use_enable_vae_slicing}")
         logger.debug(f"  use_xformers: {self.use_xformers}")
 
+        self.options = options
+
         torch.backends.cuda.matmul.allow_tf32 = self.use_tf32
         torch.backends.cudnn.benchmark = self.use_cudnn_benchmark
 
     def load_safety_checker(self, action):
         if not self.do_nsfw_filter:
             self.pipe.safety_checker = None
         else:
@@ -783,40 +803,92 @@
                 #kwargs["generator"] = generator
 
             if self.is_controlnet:
                 if kwargs.get("strength"):
                     kwargs["controlnet_conditioning_scale"] = kwargs["strength"]
                     del kwargs["strength"]
 
-            output = self.pipe(
-                self.prompt,
-                negative_prompt=self.negative_prompt,
-                guidance_scale=self.guidance_scale,
-                num_inference_steps=self.num_inference_steps,
-                num_images_per_prompt=1,
-                callback=self.callback,
-                **kwargs
-            )
+            output = self.call_pipe(**kwargs)
         except Exception as e:
+            logger.warning("something went wrong")
+            print(e)
+            logger.error(e)
             if "`flshattF` is not supported because" in str(e):
                 # try again
                 logger.info("Disabling xformers and trying again")
                 self.pipe.enable_xformers_memory_efficient_attention(attention_op=None)
                 self.pipe.vae.enable_xformers_memory_efficient_attention(attention_op=None)
                 # redo the sample with xformers enabled
                 return self.do_sample(**kwargs)
             output = None
 
+        if self.is_txt2vid:
+            return self.handle_txt2vid_output(output)
+        else:
+            image = output.images[0] if output else None
+            nsfw_content_detected = None
+            if self.action_has_safety_checker:
+                nsfw_content_detected = output.nsfw_content_detected
+            return image, nsfw_content_detected
+
+    active_extensions = []
+
+    def handle_txt2vid_output(self, output):
+        pil_image = None
         if output:
-            image = output.images[0]
+            from diffusers.utils import export_to_video
+            video_frames = output.frames
+            os.makedirs(os.path.dirname(self.txt2vid_file), exist_ok=True)
+            export_to_video(video_frames, self.txt2vid_file)
+            pil_image = Image.fromarray(video_frames[0])
+        else:
+            print("failed to get output from txt2vid")
+        return pil_image, None
 
-        nsfw_content_detected = None
-        if self.action_has_safety_checker:
-            nsfw_content_detected = output.nsfw_content_detected
-        return image, nsfw_content_detected
+    def call_pipe_extension(self, **kwargs):
+        """
+        This calls the call_pipe method on all active extensions
+        :param kwargs:
+        :return:
+        """
+        for extension in self.active_extensions:
+            kwargs = extension.call_pipe(self.options, self.model_base_path, self.pipe, **kwargs)
+        return kwargs
+
+    def call_pipe(self, **kwargs):
+        """
+        Generate an image using the pipe
+        :param kwargs:
+        :return:
+        """
+        compel_proc = Compel(tokenizer=self.pipe.tokenizer, text_encoder=self.pipe.text_encoder)
+        prompt_embeds = compel_proc(self.prompt)
+        negative_prompt_embeds = compel_proc(self.negative_prompt) if self.negative_prompt else None
+
+        if self.is_txt2vid:
+            return self.pipe(
+                prompt_embeds=prompt_embeds,
+                negative_prompt_embeds=negative_prompt_embeds,
+                guidance_scale=self.guidance_scale,
+                num_inference_steps=self.num_inference_steps,
+                num_frames=self.batch_size,
+                callback=self.callback,
+            )
+        else:
+            print("CALLING PIPE ", self.prompt)
+            kwargs = self.call_pipe_extension(**kwargs)
+            return self.pipe(
+                prompt_embeds=prompt_embeds,
+                negative_prompt_embeds=negative_prompt_embeds,
+                guidance_scale=self.guidance_scale,
+                num_inference_steps=self.num_inference_steps,
+                num_images_per_prompt=1,
+                callback=self.callback,
+                **kwargs
+            )
 
     def _preprocess_canny(self, image):
         image = np.array(image)
         low_threshold = 100
         high_threshold = 200
         image = cv2.Canny(image, low_threshold, high_threshold)
         image = image[:, :, None]
@@ -947,14 +1019,16 @@
             image = data["options"]["image"]
             # todo: get mask to work
             #mask_bytes = data["options"]["mask"]
             #mask = Image.frombytes("RGB", (self.width, self.height), mask_bytes)
             #extra_args["depth_map"] = mask
             extra_args["image"] = image
             extra_args["strength"] = self.strength
+        elif action == "txt2vid":
+            pass
         elif self.is_superresolution:
             image = data["options"]["image"]
             if self.do_mega_scale:
                 pass
             else:
                 extra_args["image"] = image
         elif action == "outpaint":
@@ -962,78 +1036,78 @@
             mask = data["options"]["mask"]
             extra_args["image"] = image
             extra_args["mask_image"] = mask
             extra_args["width"] = self.width
             extra_args["height"] = self.height
 
         # do the sample
-        try:
-            if self.do_mega_scale:
-                # first we will downscale the original image using the PIL algorithm
-                # called "bicubic" which is a high quality algorithm
-                # then we will upscale the image using the super resolution model
-                # then we will upscale the image using the PIL algorithm called "bicubic"
-                # to the desired size
-                # the new dimensions of scaled_w and scaled_h should be the width and height
-                # of the image that current image but aspect ratio scaled to 128
-                # so if the image is 256x256 then the scaled_w and scaled_h should be 128x128 but
-                # if the image is 512x256 then the scaled_w and scaled_h should be 128x64
-
-                max_in_width = 512
-                scale_size = 256
-                in_width = self.width
-                in_height = self.height
-                original_image_width = data["options"]["original_image_width"]
-                original_image_height = data["options"]["original_image_height"]
-
-                if original_image_width > max_in_width:
-                    scale_factor = max_in_width / original_image_width
-                    in_width = int(original_image_width * scale_factor)
-                    in_height = int(original_image_height * scale_factor)
-                    scale_size = int(scale_size * scale_factor)
-
-                if in_width > max_in_width:
-                    # scale down in_width and in_height by scale_size
-                    # but keep the aspect ratio
-                    in_width = scale_size
-                    in_height = int((scale_size / original_image_width) * original_image_height)
-
-                # now we will scale the image to the new dimensions
-                # and then upscale it using the super resolution model
-                # and then downscale it using the PIL bicubic algorithm
-                # to the original dimensions
-                # this will give us a high quality image
-                scaled_w = int(in_width * (scale_size / in_height))
-                scaled_h = scale_size
-                downscaled_image = image.resize((scaled_w, scaled_h), Image.BILINEAR)
-                extra_args["image"] = downscaled_image
-                upscaled_image, nsfw_content_detected = self.do_sample(**extra_args)
-                # upscale back to self.width and self.height
-                image = upscaled_image.resize((original_image_width, original_image_height), Image.BILINEAR)
+        # try:
+        if self.do_mega_scale:
+            # first we will downscale the original image using the PIL algorithm
+            # called "bicubic" which is a high quality algorithm
+            # then we will upscale the image using the super resolution model
+            # then we will upscale the image using the PIL algorithm called "bicubic"
+            # to the desired size
+            # the new dimensions of scaled_w and scaled_h should be the width and height
+            # of the image that current image but aspect ratio scaled to 128
+            # so if the image is 256x256 then the scaled_w and scaled_h should be 128x128 but
+            # if the image is 512x256 then the scaled_w and scaled_h should be 128x64
+
+            max_in_width = 512
+            scale_size = 256
+            in_width = self.width
+            in_height = self.height
+            original_image_width = data["options"]["original_image_width"]
+            original_image_height = data["options"]["original_image_height"]
+
+            if original_image_width > max_in_width:
+                scale_factor = max_in_width / original_image_width
+                in_width = int(original_image_width * scale_factor)
+                in_height = int(original_image_height * scale_factor)
+                scale_size = int(scale_size * scale_factor)
+
+            if in_width > max_in_width:
+                # scale down in_width and in_height by scale_size
+                # but keep the aspect ratio
+                in_width = scale_size
+                in_height = int((scale_size / original_image_width) * original_image_height)
+
+            # now we will scale the image to the new dimensions
+            # and then upscale it using the super resolution model
+            # and then downscale it using the PIL bicubic algorithm
+            # to the original dimensions
+            # this will give us a high quality image
+            scaled_w = int(in_width * (scale_size / in_height))
+            scaled_h = scale_size
+            downscaled_image = image.resize((scaled_w, scaled_h), Image.BILINEAR)
+            extra_args["image"] = downscaled_image
+            upscaled_image, nsfw_content_detected = self.do_sample(**extra_args)
+            # upscale back to self.width and self.height
+            image = upscaled_image.resize((original_image_width, original_image_height), Image.BILINEAR)
 
-                return image
-            else:
-                image, nsfw_content_detected = self.do_sample(**extra_args)
-        except Exception as e:
-            if "PYTORCH_CUDA_ALLOC_CONF" in str(e):
-                raise Exception(self.cuda_error_message)
-            elif "`flshattF` is not supported because" in str(e):
-                # try again
-                logger.info("Disabling xformers and trying again")
-                self.pipe.enable_xformers_memory_efficient_attention(
-                    attention_op=None)
-                self.pipe.vae.enable_xformers_memory_efficient_attention(
-                    attention_op=None)
-                # redo the sample with xformers enabled
-                return self._sample_diffusers_model(data)
-            else:
-                if self.is_dev_env:
-                    traceback.print_exc()
-                logger.error("Something went wrong while generating image")
-                logger.error(e)
+            return image
+        else:
+            image, nsfw_content_detected = self.do_sample(**extra_args)
+        # except Exception as e:
+        #     if "PYTORCH_CUDA_ALLOC_CONF" in str(e):
+        #         raise Exception(self.cuda_error_message)
+        #     elif "`flshattF` is not supported because" in str(e):
+        #         # try again
+        #         logger.info("Disabling xformers and trying again")
+        #         self.pipe.enable_xformers_memory_efficient_attention(
+        #             attention_op=None)
+        #         self.pipe.vae.enable_xformers_memory_efficient_attention(
+        #             attention_op=None)
+        #         # redo the sample with xformers enabled
+        #         return self._sample_diffusers_model(data)
+        #     else:
+        #         if self.is_dev_env:
+        #             traceback.print_exc()
+        #         logger.error("Something went wrong while generating image")
+        #         logger.error(e)
 
         self.final_callback()
 
         return image, nsfw_content_detected
 
     def _blend_images_by_average(self, composite, original):
         # upscale the original image
@@ -1078,15 +1152,19 @@
         self._change_scheduler()
 
         if not self.use_enable_sequential_cpu_offload:
             self.move_models_to_cpu(self.action)
             self._clear_memory()
 
         self._apply_memory_efficient_settings()
-        for n in range(self.batch_size):
+        if self.is_txt2vid:
+            total_to_generate = 1
+        else:
+            total_to_generate = self.batch_size
+        for n in range(total_to_generate):
             image, nsfw_content_detected = self._sample_diffusers_model(data)
             self.image_handler(image, data, nsfw_content_detected)
             self.seed = self.seed + 1
             if self.do_cancel:
                 self.do_cancel = False
                 break
 
@@ -1103,41 +1181,39 @@
 
     def final_callback(self):
         total = int(self.num_inference_steps * self.strength)
         self.tqdm_callback(total, total, self.action)
 
     def callback(self, step: int, _time_step, _latents):
         # convert _latents to image
+        image = None
+        if not self.is_txt2vid:
+            image = self._latents_to_image(_latents)
+        data = self.data
+        if self.is_txt2vid:
+            data["video_filename"] = self.txt2vid_file
         self.tqdm_callback(
             step,
             int(self.num_inference_steps * self.strength),
             self.action,
-            image=self._latents_to_image(_latents),
-            data=self.data,
+            image=image,
+            data=data,
         )
         pass
 
     def _latents_to_image(self, latents: torch.Tensor):
         # convert tensor to image
         #image = self.pipe.vae.decoder(latents)
         image = latents.permute(0, 2, 3, 1)
         image = image.detach().cpu().numpy()
         image = image[0]
         image = (image * 255).astype(np.uint8)
         image = Image.fromarray(image)
         return image
 
-    @property
-    def has_internet_connection(self):
-        try:
-            response = requests.get('https://huggingface.co/')
-            return True
-        except requests.ConnectionError:
-            return False
-
     def generator_sample(
         self,
         data: dict,
         image_var: callable,
         error_var: callable = None
     ):
         # check if model in data is cached
@@ -1153,14 +1229,16 @@
             self.initialized = False
         elif data["action"] == "depth" and self.initialized and self.depth2img is None:
             self.initialized = False
         elif data["action"] == "superresolution" and self.initialized and self.superresolution is None:
             self.initialized = False
         elif data["action"] == "txt2img" and self.initialized and self.txt2img is None:
             self.initialized = False
+        elif data["action"] == "txt2vid" and self.initialized and self.txt2vid is None:
+            self.initialized = False
         error = None
         try:
             self._generate(data, image_var=image_var)
         except OSError as e:
             err = e.args[0]
             logger.error(err)
             error = "model_not_found"
```

### Comparing `aihandler-1.8.21/src/aihandler/settings.py` & `aihandler-1.9.0/src/aihandler/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,20 @@
         }
     },
     "vid2vid": {
         "SD Image Variations": {
             "path": "lambdalabs/sd-image-variations-diffusers",
             "branch": "v2.0",
         }
+    },
+    "txt2vid":  {
+        "damo-vilab": {
+            "path": "damo-vilab/text-to-video-ms-1.7b",
+            "branch": "fp16",
+        }
     }
 }
 TEXT_MODELS = {
     "flan-t5-xxl": {
         "path": "google/flan-t5-xxl",
         "class": "AutoModelForSeq2SeqLM",
         "tokenizer": "AutoTokenizer",
```

### Comparing `aihandler-1.8.21/src/aihandler/settings_manager.py` & `aihandler-1.9.0/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler/socket_server.py` & `aihandler-1.9.0/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.8.21/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.0/src/aihandler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.8.21
+Version: 1.9.0
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
@@ -47,15 +47,15 @@
 - Cuda capable GPU
 - 16gb+ ram
 
 [For Windows, follow windows branch instructions](https://github.com/Capsize-Games/aihandler/tree/develop-windows)
 
 Install
 ```
-pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.14.0.ckpt_fix.tar.gz
+pip install https://github.com/w4ffl35/diffusers/archive/refs/tags/v0.15.0.ckpt_fix_0.0.1.tar.gz
 pip install https://github.com/w4ffl35/transformers/archive/refs/tags/tensor_fix-v1.0.2.tar.gz
 pip install aihandler
 ```
 
 #### Optional
 
 These are optional instructions for installing TensorRT and Deepspeed for Windows
```

### Comparing `aihandler-1.8.21/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.0/src/aihandler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 README.md
 setup.py
 src/aihandler/__init__.py
 src/aihandler/base_runner.py
 src/aihandler/controlnet_utils.py
 src/aihandler/database.py
+src/aihandler/extension.py
 src/aihandler/llmrunner.py
 src/aihandler/logger.py
 src/aihandler/offline_client.py
 src/aihandler/pyqt_offline_client.py
 src/aihandler/qtvar.py
 src/aihandler/runner.py
 src/aihandler/settings.py
 src/aihandler/settings_manager.py
 src/aihandler/socket_server.py
+src/aihandler/util.py
 src/aihandler.egg-info/PKG-INFO
 src/aihandler.egg-info/SOURCES.txt
 src/aihandler.egg-info/dependency_links.txt
 src/aihandler.egg-info/requires.txt
 src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.8.21/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.0/src/aihandler.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-torch==1.13.1
-torchvision==0.14.1
-torchaudio==0.13.1
+torch==2.0.0
+torchvision==0.15.1
+torchaudio==2.0.1
 einops==0.6.0
 ninja==1.11.1
 JIT==0.2.7
-triton==2.0.0.dev20221202
+triton==2.0.0
 tqdm==4.65.0
-xformers==0.0.16
+xformers==0.0.18
 bitsandbytes==0.37.0
 omegaconf==2.3.0
 accelerate==0.18.0
 controlnet_aux==0.0.1
 huggingface-hub==0.13.3
 numpy==1.23.5
 Pillow==9.4.0
@@ -24,16 +24,16 @@
 requests==2.28.2
 requests-oauthlib==1.3.1
 safetensors==0.3.0
 scipy==1.10.1
 tensorflow==2.12.0
 tokenizers==0.13.2
 tqdm==4.65.0
-xformers==0.0.16
 charset-normalizer==3.1.0
 opencv-python==4.7.0.72
 setuptools==65.5.1
 sympy==1.11.1
 typing_extensions==4.5.0
 urllib3==1.26.15
-diffusers==0.14.0
+diffusers==0.15.0
 transformers==4.27.4
+compel==1.1.3
```

