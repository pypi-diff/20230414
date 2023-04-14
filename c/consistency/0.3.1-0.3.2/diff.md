# Comparing `tmp/consistency-0.3.1.tar.gz` & `tmp/consistency-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistency-0.3.1.tar", last modified: Tue Mar 28 07:51:05 2023, max compression
+gzip compressed data, was "consistency-0.3.2.tar", last modified: Fri Apr 14 11:04:29 2023, max compression
```

## Comparing `consistency-0.3.1.tar` & `consistency-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:05.710079 consistency-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 07:50:56.000000 consistency-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-28 07:51:05.710079 consistency-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-28 07:50:56.000000 consistency-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:05.710079 consistency-0.3.1/consistency/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-28 07:50:56.000000 consistency-0.3.1/consistency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-03-28 07:50:56.000000 consistency-0.3.1/consistency/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 07:50:56.000000 consistency-0.3.1/consistency/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-28 07:50:56.000000 consistency-0.3.1/consistency/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:05.710079 consistency-0.3.1/consistency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-28 07:51:05.000000 consistency-0.3.1/consistency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-28 07:51:05.000000 consistency-0.3.1/consistency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:51:05.000000 consistency-0.3.1/consistency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 07:51:05.000000 consistency-0.3.1/consistency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 07:51:05.000000 consistency-0.3.1/consistency.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 07:51:05.710079 consistency-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-28 07:50:56.000000 consistency-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:04:29.474503 consistency-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 11:04:21.000000 consistency-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 11:04:29.474503 consistency-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-14 11:04:21.000000 consistency-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:04:29.474503 consistency-0.3.2/consistency/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 11:04:21.000000 consistency-0.3.2/consistency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-14 11:04:21.000000 consistency-0.3.2/consistency/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 11:04:21.000000 consistency-0.3.2/consistency/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-14 11:04:21.000000 consistency-0.3.2/consistency/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:04:29.474503 consistency-0.3.2/consistency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 11:04:29.000000 consistency-0.3.2/consistency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 11:04:29.000000 consistency-0.3.2/consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:04:29.000000 consistency-0.3.2/consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 11:04:29.000000 consistency-0.3.2/consistency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 11:04:29.000000 consistency-0.3.2/consistency.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:04:29.474503 consistency-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 11:04:21.000000 consistency-0.3.2/setup.py
```

### Comparing `consistency-0.3.1/LICENSE` & `consistency-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `consistency-0.3.1/PKG-INFO` & `consistency-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistency
-Version: 0.3.1
+Version: 0.3.2
 Summary: Consistency Model - Pytorch
 Home-page: https://github.com/junhsss/consistency-models
 Author: junhsss
 Author-email: junhsssr@gmail.com
 License: MIT
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consistency-0.3.1/README.md` & `consistency-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     "consistency/cifar10-32-demo",
     custom_pipeline="consistency/pipeline",
 )
 
 pipeline().images[0]  # Super Fast Generation! 🤯
 ```
 
+[**Try it yourself!**](https://colab.research.google.com/github/junhsss/consistency-models/blob/main/examples/sample.ipynb)
+
 <br />
 
 ## Quickstart
 
 ### Basic
 
 Just wrap your favorite _U-Net_ with `Consistency`.
@@ -85,22 +87,22 @@
 
 You can safely drop `consistency` afterwards. Good luck! 🤞
 
 ```python
 from diffusers import DiffusionPipeline
 
 pipeline = DiffusionPipeline.from_pretrained(
-    "your_model_id",
+    "your_name/your_model_id",
     custom_pipeline="consistency/pipeline",
 )
 
 pipeline().images[0]
 ```
 
-A complete example can be found in [this **script**](https://github.com/junhsss/consistency-models/blob/main/examples/train.py) or in [this **colab notebook**](https://colab.research.google.com/github/junhsss/consistency-models/blob/main/examples/consistency_models.ipynb).
+A complete example can be found in [**here**](https://github.com/junhsss/consistency-models/blob/main/examples/unconditional_image_generation) or in [this **colab notebook**](https://colab.research.google.com/github/junhsss/consistency-models/blob/main/examples/consistency_models.ipynb).
 
 Checkout [this **Wandb workspace**](https://wandb.ai/junhsss/consistency?workspace=user-junhsss) for some experiment results.
 
 <br />
 
 ## Available Models
```

#### html2text {}

```diff
@@ -5,15 +5,17 @@
 sample quality without adversarial training. They support _fast one-step
 generation_ by design, while still allowing for few-step sampling to trade
 compute for sample quality.
 ## Installation ```sh $ pip install consistency ``` ### Note You **don't need
 to install** `consistency` for just trying things out: ```python from diffusers
 import DiffusionPipeline pipeline = DiffusionPipeline.from_pretrained
 ( "consistency/cifar10-32-demo", custom_pipeline="consistency/pipeline", )
-pipeline().images[0] # Super Fast Generation! ð¤¯ ```
+pipeline().images[0] # Super Fast Generation! ð¤¯ ``` [**Try it yourself!**]
+(https://colab.research.google.com/github/junhsss/consistency-models/blob/main/
+examples/sample.ipynb)
 ## Quickstart ### Basic Just wrap your favorite _U-Net_ with `Consistency`.
 ```python import torch from diffusers import UNet2DModel from consistency
 import Consistency from consistency.loss import PerceptualLoss consistency =
 Consistency( model=UNet2DModel(sample_size=224), loss_fn=PerceptualLoss
 (net_type=("vgg", "squeeze")) ) samples = consistency.sample(16) # multi-step
 sampling, sample from the ema model samples = consistency.sample(16, steps=5,
 use_ema=True) ``` `Consistency` is self-contained with the training logic and
@@ -22,19 +24,19 @@
 Trainer(max_epochs=8000, accelerator="auto") trainer.fit(consistency,
 some_dataloader) ``` ### Push to HF Hub Provide your `model_id` and `token` to
 `Consistency`. ```python consistency = Consistency( model=UNet2DModel
 (sample_size=224), loss_fn=PerceptualLoss(net_type=("vgg", "squeeze"))
 model_id="your_model_id", token="your_token" # Not needed if logged in via
 huggingface-cli push_every_n_steps=10000, ) ``` You can safely drop
 `consistency` afterwards. Good luck! ð¤ ```python from diffusers import
-DiffusionPipeline pipeline = DiffusionPipeline.from_pretrained
-( "your_model_id", custom_pipeline="consistency/pipeline", ) pipeline().images
-[0] ``` A complete example can be found in [this **script**](https://
-github.com/junhsss/consistency-models/blob/main/examples/train.py) or in [this
-**colab notebook**](https://colab.research.google.com/github/junhsss/
+DiffusionPipeline pipeline = DiffusionPipeline.from_pretrained( "your_name/
+your_model_id", custom_pipeline="consistency/pipeline", ) pipeline().images[0]
+``` A complete example can be found in [**here**](https://github.com/junhsss/
+consistency-models/blob/main/examples/unconditional_image_generation) or in
+[this **colab notebook**](https://colab.research.google.com/github/junhsss/
 consistency-models/blob/main/examples/consistency_models.ipynb). Checkout [this
 **Wandb workspace**](https://wandb.ai/junhsss/consistency?workspace=user-
 junhsss) for some experiment results.
 ## Available Models | model_id | dataset | | ----------------------------------
 -------------------------------------------------------------------------------
 -------- | --------------------------------------------------------------------
 ---------------------- | | consistency/cifar10-32-demo | cifar10 | If you've
```

### Comparing `consistency-0.3.1/consistency/consistency.py` & `consistency-0.3.2/consistency/consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         bins_rho: float = 7,
         initial_ema_decay: float = 0.9,
         optimizer_type: Type[optim.Optimizer] = optim.RAdam,
         samples_path: str = "samples/",
         save_samples_every_n_epoch: int = 10,
         num_samples: int = 16,
         sample_steps: int = 1,
-        use_ema: bool = False,
+        use_ema: bool = True,
         sample_seed: int = 0,
         model_id: Optional[str] = None,
         token: Optional[str] = None,
         push_every_n_steps: Optional[int] = 100,
         **kwargs,
     ) -> None:
         super().__init__()
```

### Comparing `consistency-0.3.1/consistency/loss.py` & `consistency-0.3.2/consistency/loss.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             else:
                 raise TypeError(
                     f"'net_type' should be on of {available_net_types}, got {net_type}"
                 )
 
         self.lpips_losses = nn.ModuleList()
 
-        if isinstance(net_type, str) and net_type in available_net_types:
+        if isinstance(net_type, str):
             _append_net_type(net_type)
 
         elif isinstance(net_type, Sequence):
             for _net_type in sorted(net_type):
                 _append_net_type(_net_type)
 
         self.lpips_losses.requires_grad_(False)
```

### Comparing `consistency-0.3.1/consistency/pipeline.py` & `consistency-0.3.2/consistency/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,25 +31,23 @@
         img_size = self.unet.config.sample_size
         shape = (1, 3, img_size, img_size)
 
         model = self.unet
 
         time: float = time_max
 
-        sample = randn_tensor(shape, generator=generator) * time
+        sample = randn_tensor(shape, generator=generator, device=self.device) * time
 
         for step in self.progress_bar(range(steps)):
             if step > 0:
                 time = self.search_previous_time(time)
                 sigma = math.sqrt(time**2 - time_min**2 + 1e-6)
-                sample = sample + sigma * randn_tensor(
-                    sample.shape, device=sample.device, generator=generator
-                )
+                sample = sample + sigma * randn_tensor(sample.shape, device=self.device, generator=generator)
 
-            out = model(sample, torch.tensor([time], device=sample.device)).sample
+            out = model(sample, torch.tensor([time], device=self.device)).sample
 
             skip_coef = data_std**2 / ((time - time_min) ** 2 + data_std**2)
             out_coef = data_std * time / (time**2 + data_std**2) ** (0.5)
 
             sample = (sample * skip_coef + out * out_coef).clamp(-1.0, 1.0)
 
         sample = (sample / 2 + 0.5).clamp(0, 1)
@@ -59,12 +57,12 @@
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image,)
 
         return ImagePipelineOutput(images=image)
 
-    # TODO: Implement greedy search on FID
-    def search_previous_time(
-        self, time, time_min: float = 0.002, time_max: float = 80.0
-    ):
+    def search_previous_time(self, time, time_min: float = 0.002, time_max: float = 80.0):
         return (2 * time + time_min) / 3
+
+    def cuda(self):
+        self.to("cuda")
```

### Comparing `consistency-0.3.1/consistency.egg-info/PKG-INFO` & `consistency-0.3.2/consistency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistency
-Version: 0.3.1
+Version: 0.3.2
 Summary: Consistency Model - Pytorch
 Home-page: https://github.com/junhsss/consistency-models
 Author: junhsss
 Author-email: junhsssr@gmail.com
 License: MIT
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consistency-0.3.1/setup.py` & `consistency-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 setup(
     name="consistency",
     packages=find_packages(),
     version=__version__,
     license="MIT",
     description="Consistency Model - Pytorch",
```

