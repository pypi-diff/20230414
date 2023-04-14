# Comparing `tmp/setfit-0.6.0.tar.gz` & `tmp/setfit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setfit-0.6.0.tar", last modified: Wed Feb  8 13:29:06 2023, max compression
+gzip compressed data, was "setfit-0.7.0.tar", last modified: Fri Apr 14 15:11:49 2023, max compression
```

## Comparing `setfit-0.6.0.tar` & `setfit-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-02-08 13:29:06.253082 setfit-0.6.0/
--rw-r--r--   0 lewtun     (501) staff       (20)    11357 2022-06-30 07:14:50.000000 setfit-0.6.0/LICENSE
--rw-r--r--   0 lewtun     (501) staff       (20)    17361 2023-02-08 13:29:06.253231 setfit-0.6.0/PKG-INFO
--rw-r--r--   0 lewtun     (501) staff       (20)    16232 2023-02-08 13:06:36.000000 setfit-0.6.0/README.md
--rw-r--r--   0 lewtun     (501) staff       (20)      440 2023-02-08 13:29:06.253693 setfit-0.6.0/setup.cfg
--rw-r--r--   0 lewtun     (501) staff       (20)     2317 2023-02-08 13:25:01.000000 setfit-0.6.0/setup.py
-drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-02-08 13:29:06.249035 setfit-0.6.0/src/
-drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-02-08 13:29:06.251521 setfit-0.6.0/src/setfit/
--rw-r--r--   0 lewtun     (501) staff       (20)      244 2023-02-08 13:25:01.000000 setfit-0.6.0/src/setfit/__init__.py
--rw-r--r--   0 lewtun     (501) staff       (20)    11775 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/data.py
-drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-02-08 13:29:06.252946 setfit-0.6.0/src/setfit/exporters/
--rw-r--r--   0 lewtun     (501) staff       (20)        0 2022-12-14 14:45:31.000000 setfit-0.6.0/src/setfit/exporters/__init__.py
--rw-r--r--   0 lewtun     (501) staff       (20)    12181 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/exporters/onnx.py
--rw-r--r--   0 lewtun     (501) staff       (20)     1719 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/exporters/openvino.py
--rw-r--r--   0 lewtun     (501) staff       (20)     1167 2022-12-14 14:45:31.000000 setfit-0.6.0/src/setfit/exporters/utils.py
--rw-r--r--   0 lewtun     (501) staff       (20)     1360 2022-10-14 07:36:48.000000 setfit-0.6.0/src/setfit/integrations.py
--rw-r--r--   0 lewtun     (501) staff       (20)     9743 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/logging.py
--rw-r--r--   0 lewtun     (501) staff       (20)    30091 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/modeling.py
--rw-r--r--   0 lewtun     (501) staff       (20)      357 2022-09-16 13:35:41.000000 setfit-0.6.0/src/setfit/pipeline.py
--rw-r--r--   0 lewtun     (501) staff       (20)    25337 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/trainer.py
--rw-r--r--   0 lewtun     (501) staff       (20)    11483 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/trainer_distillation.py
--rw-r--r--   0 lewtun     (501) staff       (20)     5353 2023-02-08 13:06:36.000000 setfit-0.6.0/src/setfit/utils.py
-drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-02-08 13:29:06.252448 setfit-0.6.0/src/setfit.egg-info/
--rw-r--r--   0 lewtun     (501) staff       (20)    17361 2023-02-08 13:29:05.000000 setfit-0.6.0/src/setfit.egg-info/PKG-INFO
--rw-r--r--   0 lewtun     (501) staff       (20)      577 2023-02-08 13:29:06.000000 setfit-0.6.0/src/setfit.egg-info/SOURCES.txt
--rw-r--r--   0 lewtun     (501) staff       (20)        1 2023-02-08 13:29:05.000000 setfit-0.6.0/src/setfit.egg-info/dependency_links.txt
--rw-r--r--   0 lewtun     (501) staff       (20)        1 2022-07-04 07:31:20.000000 setfit-0.6.0/src/setfit.egg-info/not-zip-safe
--rw-r--r--   0 lewtun     (501) staff       (20)      577 2023-02-08 13:29:06.000000 setfit-0.6.0/src/setfit.egg-info/requires.txt
--rw-r--r--   0 lewtun     (501) staff       (20)        7 2023-02-08 13:29:06.000000 setfit-0.6.0/src/setfit.egg-info/top_level.txt
+drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-04-14 15:11:49.234290 setfit-0.7.0/
+-rw-r--r--   0 lewtun     (501) staff       (20)    11357 2022-06-30 07:14:50.000000 setfit-0.7.0/LICENSE
+-rw-r--r--   0 lewtun     (501) staff       (20)    17363 2023-04-14 15:11:49.234420 setfit-0.7.0/PKG-INFO
+-rw-r--r--   0 lewtun     (501) staff       (20)    16233 2023-04-14 13:07:51.000000 setfit-0.7.0/README.md
+-rw-r--r--   0 lewtun     (501) staff       (20)      440 2023-04-14 15:11:49.234862 setfit-0.7.0/setup.cfg
+-rw-r--r--   0 lewtun     (501) staff       (20)     2710 2023-04-14 15:09:38.000000 setfit-0.7.0/setup.py
+drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-04-14 15:11:49.230666 setfit-0.7.0/src/
+drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-04-14 15:11:49.232565 setfit-0.7.0/src/setfit/
+-rw-r--r--   0 lewtun     (501) staff       (20)      244 2023-04-14 15:09:38.000000 setfit-0.7.0/src/setfit/__init__.py
+-rw-r--r--   0 lewtun     (501) staff       (20)    11742 2023-02-19 17:21:49.000000 setfit-0.7.0/src/setfit/data.py
+drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-04-14 15:11:49.234124 setfit-0.7.0/src/setfit/exporters/
+-rw-r--r--   0 lewtun     (501) staff       (20)        0 2022-12-14 14:45:31.000000 setfit-0.7.0/src/setfit/exporters/__init__.py
+-rw-r--r--   0 lewtun     (501) staff       (20)    12181 2023-02-08 13:06:36.000000 setfit-0.7.0/src/setfit/exporters/onnx.py
+-rw-r--r--   0 lewtun     (501) staff       (20)     1719 2023-02-08 13:06:36.000000 setfit-0.7.0/src/setfit/exporters/openvino.py
+-rw-r--r--   0 lewtun     (501) staff       (20)     1167 2022-12-14 14:45:31.000000 setfit-0.7.0/src/setfit/exporters/utils.py
+-rw-r--r--   0 lewtun     (501) staff       (20)     1360 2022-10-14 07:36:48.000000 setfit-0.7.0/src/setfit/integrations.py
+-rw-r--r--   0 lewtun     (501) staff       (20)     9743 2023-02-08 13:06:36.000000 setfit-0.7.0/src/setfit/logging.py
+-rw-r--r--   0 lewtun     (501) staff       (20)    31352 2023-04-14 13:07:51.000000 setfit-0.7.0/src/setfit/modeling.py
+-rw-r--r--   0 lewtun     (501) staff       (20)      357 2022-09-16 13:35:41.000000 setfit-0.7.0/src/setfit/pipeline.py
+-rw-r--r--   0 lewtun     (501) staff       (20)    28368 2023-04-14 13:07:51.000000 setfit-0.7.0/src/setfit/trainer.py
+-rw-r--r--   0 lewtun     (501) staff       (20)    11930 2023-04-14 13:07:51.000000 setfit-0.7.0/src/setfit/trainer_distillation.py
+-rw-r--r--   0 lewtun     (501) staff       (20)     5353 2023-02-08 13:06:36.000000 setfit-0.7.0/src/setfit/utils.py
+drwxr-xr-x   0 lewtun     (501) staff       (20)        0 2023-04-14 15:11:49.233476 setfit-0.7.0/src/setfit.egg-info/
+-rw-r--r--   0 lewtun     (501) staff       (20)    17363 2023-04-14 15:11:49.000000 setfit-0.7.0/src/setfit.egg-info/PKG-INFO
+-rw-r--r--   0 lewtun     (501) staff       (20)      577 2023-04-14 15:11:49.000000 setfit-0.7.0/src/setfit.egg-info/SOURCES.txt
+-rw-r--r--   0 lewtun     (501) staff       (20)        1 2023-04-14 15:11:49.000000 setfit-0.7.0/src/setfit.egg-info/dependency_links.txt
+-rw-r--r--   0 lewtun     (501) staff       (20)        1 2022-07-04 07:31:20.000000 setfit-0.7.0/src/setfit.egg-info/not-zip-safe
+-rw-r--r--   0 lewtun     (501) staff       (20)      638 2023-04-14 15:11:49.000000 setfit-0.7.0/src/setfit.egg-info/requires.txt
+-rw-r--r--   0 lewtun     (501) staff       (20)        7 2023-04-14 15:11:49.000000 setfit-0.7.0/src/setfit.egg-info/top_level.txt
```

### Comparing `setfit-0.6.0/LICENSE` & `setfit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/PKG-INFO` & `setfit-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: setfit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Efficient few-shot learning with Sentence Transformers
 Home-page: https://github.com/SetFit/setfit
 Download-URL: https://github.com/SetFit/setfit/tags
 Maintainer: Lewis Tunstall, Tom Aarsen
 Maintainer-email: lewis@huggingface.co
 License: Apache 2.0
 Keywords: nlp,machine learning,fewshot learning,transformers
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: optuna
 Provides-Extra: quality
 Provides-Extra: tests
 Provides-Extra: onnx
 Provides-Extra: openvino
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: compat_tests
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/huggingface/setfit/main/assets/setfit.png">
 
 <p align="center">
@@ -424,23 +424,22 @@
 ├── setup.cfg       <- Configuration file to define package metadata
 ├── setup.py        <- Make this project pip installable with `pip install -e`
 ├── src             <- Source code for SetFit
 └── tests           <- Unit tests
 ```
 
 ## Related work
+
 * [jxpress/setfit-pytorch-lightning](https://github.com/jxpress/setfit-pytorch-lightning) - A PyTorch Lightning implementation of SetFit.
 
 ## Citation
 
 ```@misc{https://doi.org/10.48550/arxiv.2209.11055,
   doi = {10.48550/ARXIV.2209.11055},
   url = {https://arxiv.org/abs/2209.11055},
   author = {Tunstall, Lewis and Reimers, Nils and Jo, Unso Eun Seo and Bates, Luke and Korat, Daniel and Wasserblat, Moshe and Pereg, Oren},
   keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
   title = {Efficient Few-Shot Learning Without Prompts},
   publisher = {arXiv},
   year = {2022},
   copyright = {Creative Commons Attribution 4.0 International}}
 ```
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: setfit Version: 0.6.0 Summary: Efficient few-shot
+Metadata-Version: 2.1 Name: setfit Version: 0.7.0 Summary: Efficient few-shot
 learning with Sentence Transformers Home-page: https://github.com/SetFit/setfit
 Download-URL: https://github.com/SetFit/setfit/tags Maintainer: Lewis Tunstall,
 Tom Aarsen Maintainer-email: lewis@huggingface.co License: Apache 2.0 Keywords:
-nlp,machine learning,fewshot learning,transformers Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
-text/markdown Provides-Extra: optuna Provides-Extra: quality Provides-Extra:
-tests Provides-Extra: onnx Provides-Extra: openvino Provides-Extra: dev
+nlp,machine learning,fewshot learning,transformers Classifier: Development
+Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
+Provides-Extra: optuna Provides-Extra: quality Provides-Extra: tests Provides-
+Extra: onnx Provides-Extra: openvino Provides-Extra: docs Provides-Extra: dev
 Provides-Extra: compat_tests License-File: LICENSE [https://
 raw.githubusercontent.com/huggingface/setfit/main/assets/setfit.png]
                 ð¤ Models_&_Datasets | ð Blog | ð Paper
 # SetFit - Efficient Few-shot Learning with Sentence Transformers SetFit is an
 efficient and prompt-free framework for few-shot fine-tuning of [Sentence
 Transformers](https://sbert.net/). It achieves high accuracy with little
 labeled data - for instance, with only 8 labeled examples per class on the
```

### Comparing `setfit-0.6.0/README.md` & `setfit-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -393,14 +393,15 @@
 ├── setup.cfg       <- Configuration file to define package metadata
 ├── setup.py        <- Make this project pip installable with `pip install -e`
 ├── src             <- Source code for SetFit
 └── tests           <- Unit tests
 ```
 
 ## Related work
+
 * [jxpress/setfit-pytorch-lightning](https://github.com/jxpress/setfit-pytorch-lightning) - A PyTorch Lightning implementation of SetFit.
 
 ## Citation
 
 ```@misc{https://doi.org/10.48550/arxiv.2209.11055,
   doi = {10.48550/ARXIV.2209.11055},
   url = {https://arxiv.org/abs/2209.11055},
```

### Comparing `setfit-0.6.0/setup.py` & `setfit-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,33 +11,40 @@
 
 INTEGRATIONS_REQUIRE = ["optuna"]
 REQUIRED_PKGS = ["datasets>=2.3.0", "sentence-transformers>=2.2.1", "evaluate>=0.3.0"]
 QUALITY_REQUIRE = ["black", "flake8", "isort", "tabulate"]
 ONNX_REQUIRE = ["onnxruntime", "onnx", "skl2onnx"]
 OPENVINO_REQUIRE = ["hummingbird-ml", "openvino>=2022.3"]
 TESTS_REQUIRE = ["pytest", "pytest-cov"] + ONNX_REQUIRE + OPENVINO_REQUIRE
+DOCS_REQUIRE = ["hf-doc-builder>=0.3.0"]
 EXTRAS_REQUIRE = {
     "optuna": INTEGRATIONS_REQUIRE,
     "quality": QUALITY_REQUIRE,
     "tests": TESTS_REQUIRE,
     "onnx": ONNX_REQUIRE,
     "openvino": ONNX_REQUIRE + OPENVINO_REQUIRE,
+    "docs": DOCS_REQUIRE,
 }
 
 
 def combine_requirements(base_keys):
     return list(set(k for v in base_keys for k in EXTRAS_REQUIRE[v]))
 
 
 EXTRAS_REQUIRE["dev"] = combine_requirements([k for k in EXTRAS_REQUIRE])
-EXTRAS_REQUIRE["compat_tests"] = [requirement.replace(">=", "==") for requirement in REQUIRED_PKGS] + TESTS_REQUIRE
+# For the combatibility tests we add pandas<2, as pandas 2.0.0 onwards is incompatible with old datasets versions,
+# and we assume few to no users would use old datasets versions with new pandas versions.
+# The only alternative is incrementing the minimum version for datasets, which seems unnecessary.
+EXTRAS_REQUIRE["compat_tests"] = (
+    [requirement.replace(">=", "==") for requirement in REQUIRED_PKGS] + TESTS_REQUIRE + ["pandas<2"]
+)
 
 setup(
     name="setfit",
-    version="0.6.0",
+    version="0.7.0",
     description="Efficient few-shot learning with Sentence Transformers",
     long_description=README_TEXT,
     long_description_content_type="text/markdown",
     maintainer=MAINTAINER,
     maintainer_email=MAINTAINER_EMAIL,
     url="https://github.com/SetFit/setfit",
     download_url="https://github.com/SetFit/setfit/tags",
```

### Comparing `setfit-0.6.0/src/setfit/data.py` & `setfit-0.7.0/src/setfit/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import warnings
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import torch
-from datasets import Dataset, DatasetDict, concatenate_datasets, load_dataset
+from datasets import Dataset, DatasetDict, load_dataset
 from torch.utils.data import Dataset as TorchDataset
 
+from . import logging
+
+
+logging.set_verbosity_info()
+logger = logging.get_logger(__name__)
 
 if TYPE_CHECKING:
     from transformers import PreTrainedTokenizerBase
 
 
 TokenizerOutput = Dict[str, List[int]]
 SEEDS = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
@@ -156,22 +161,23 @@
             examples.append(subset)
     return pd.concat(examples)
 
 
 def sample_dataset(dataset: Dataset, label_column: str = "label", num_samples: int = 8, seed: int = 42) -> Dataset:
     """Samples a Dataset to create an equal number of samples per class (when possible)."""
     shuffled_dataset = dataset.shuffle(seed=seed)
-    num_labels = len(dataset.unique(label_column))
-    samples = []
-    for label in range(num_labels):
-        data = shuffled_dataset.filter(lambda example: int(example[label_column]) == label)
-        num_label_samples = min(len(data), num_samples)
-        samples.append(data.select([i for i in range(num_label_samples)]))
 
-    all_samples = concatenate_datasets(samples)
+    df = shuffled_dataset.to_pandas()
+    df = df.groupby(label_column)
+
+    # sample num_samples, or at least as much as possible
+    df = df.apply(lambda x: x.sample(min(num_samples, len(x))))
+    df = df.reset_index(drop=True)
+
+    all_samples = Dataset.from_pandas(df)
     return all_samples.shuffle(seed=seed)
 
 
 def create_fewshot_splits(
     dataset: Dataset,
     sample_sizes: List[int],
     add_data_augmentation: bool = False,
```

### Comparing `setfit-0.6.0/src/setfit/exporters/onnx.py` & `setfit-0.7.0/src/setfit/exporters/onnx.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit/exporters/openvino.py` & `setfit-0.7.0/src/setfit/exporters/openvino.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit/exporters/utils.py` & `setfit-0.7.0/src/setfit/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit/integrations.py` & `setfit-0.7.0/src/setfit/integrations.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit/logging.py` & `setfit-0.7.0/src/setfit/logging.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit/modeling.py` & `setfit-0.7.0/src/setfit/modeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import tempfile
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
 
 
 # Google Colab runs on Python 3.7, so we need this to be compatible
 try:
@@ -17,15 +18,15 @@
 import torch.nn as nn
 from huggingface_hub import PyTorchModelHubMixin, hf_hub_download
 from sentence_transformers import InputExample, SentenceTransformer, models
 from sklearn.linear_model import LogisticRegression
 from sklearn.multiclass import OneVsRestClassifier
 from sklearn.multioutput import ClassifierChain, MultiOutputClassifier
 from torch.utils.data import DataLoader
-from tqdm.auto import tqdm
+from tqdm.auto import trange
 
 from . import logging
 from .data import SetFitDataset
 
 
 if TYPE_CHECKING:
     from numpy import ndarray
@@ -175,15 +176,15 @@
                 make sure to store embeddings under the key: 'sentence_embedding'
                 and the outputs will be under the key: 'prediction'.
             temperature (`float`, *optional*):
                 A logits' scaling factor. Higher values makes the model less
                 confident and higher values makes it more confident.
                 Will override the temperature given during initialization.
         Returns:
-        [`Dict[str, torch.Tensor]` or `Tuple[torch.Tensor]`]
+            [`Dict[str, torch.Tensor]` or `Tuple[torch.Tensor]`]
         """
         temperature = temperature or self.temperature
         is_features_dict = False  # whether `features` is dict or not
         if isinstance(features, dict):
             assert "sentence_embedding" in features
             is_features_dict = True
         x = features["sentence_embedding"] if is_features_dict else features
@@ -293,15 +294,15 @@
             self.model_body.train()
             self.model_head.train()
 
             dataloader = self._prepare_dataloader(x_train, y_train, batch_size, max_length)
             criterion = self.model_head.get_loss_fn()
             optimizer = self._prepare_optimizer(learning_rate, body_learning_rate, l2_weight)
             scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=5, gamma=0.5)
-            for epoch_idx in tqdm(range(num_epochs), desc="Epoch", disable=not show_progress_bar):
+            for epoch_idx in trange(num_epochs, desc="Epoch", disable=not show_progress_bar):
                 for batch in dataloader:
                     features, labels = batch
                     optimizer.zero_grad()
 
                     # to model's device
                     features = {k: v.to(device) for k, v in features.items()}
                     labels = labels.to(device)
@@ -400,45 +401,54 @@
         if component is None or component == "head":
             self._freeze_or_not(self.model_head, to_freeze=False)
 
     def _freeze_or_not(self, model: torch.nn.Module, to_freeze: bool) -> None:
         for param in model.parameters():
             param.requires_grad = not to_freeze
 
+    def _output_type_conversion(
+        self, outputs: Union[torch.Tensor, "ndarray"], as_numpy: bool = False
+    ) -> Union[torch.Tensor, "ndarray"]:
+        """Return `outputs` in the desired type:
+        * Numpy array if no differentiable head is used.
+        * Torch tensor if a differentiable head is used.
+
+        Note:
+            If the model is trained with string labels, which is only possible with a non-differentiable head,
+            then we cannot output using torch Tensors, but only using a numpy array.
+
+        Returns:
+            Union[torch.Tensor, "ndarray"]: The input, correctly converted to the desired type.
+        """
+        if as_numpy and self.has_differentiable_head:
+            outputs = outputs.detach().cpu().numpy()
+        elif not as_numpy and not self.has_differentiable_head and outputs.dtype.char != "U":
+            # Only output as tensor if the output isn't a string
+            outputs = torch.from_numpy(outputs)
+        return outputs
+
     def predict(self, x_test: List[str], as_numpy: bool = False) -> Union[torch.Tensor, "ndarray"]:
         embeddings = self.model_body.encode(
             x_test,
             normalize_embeddings=self.normalize_embeddings,
             convert_to_tensor=self.has_differentiable_head,
         )
 
         outputs = self.model_head.predict(embeddings)
-
-        if as_numpy and self.has_differentiable_head:
-            outputs = outputs.detach().cpu().numpy()
-        elif not as_numpy and not self.has_differentiable_head:
-            outputs = torch.from_numpy(outputs)
-
-        return outputs
+        return self._output_type_conversion(outputs, as_numpy=as_numpy)
 
     def predict_proba(self, x_test: List[str], as_numpy: bool = False) -> Union[torch.Tensor, "ndarray"]:
         embeddings = self.model_body.encode(
             x_test,
             normalize_embeddings=self.normalize_embeddings,
             convert_to_tensor=self.has_differentiable_head,
         )
 
         outputs = self.model_head.predict_proba(embeddings)
-
-        if as_numpy and self.has_differentiable_head:
-            outputs = outputs.detach().cpu().numpy()
-        elif not as_numpy and not self.has_differentiable_head:
-            outputs = torch.from_numpy(outputs)
-
-        return outputs
+        return self._output_type_conversion(outputs, as_numpy=as_numpy)
 
     def to(self, device: Union[str, torch.device]) -> "SetFitModel":
         """Move this SetFitModel to `device`, and then return `self`. This method does not copy.
 
         Args:
             device (Union[str, torch.device]): The identifier of the device to move the model to.
 
@@ -461,25 +471,33 @@
         Args:
             path (str): The path to save the model card to.
             model_name (str, *optional*): The name of the model. Defaults to `SetFit Model`.
         """
         if not os.path.exists(path):
             os.makedirs(path)
 
+        # If the model_path is a folder that exists locally, i.e. when create_model_card is called
+        # via push_to_hub, and the path is in a temporary folder, then we only take the last two
+        # directories
+        model_path = Path(model_name)
+        if model_path.exists() and Path(tempfile.gettempdir()) in model_path.resolve().parents:
+            model_name = "/".join(model_path.parts[-2:])
+
         model_card_content = MODEL_CARD_TEMPLATE.format(model_name=model_name)
         with open(os.path.join(path, "README.md"), "w", encoding="utf-8") as f:
             f.write(model_card_content)
 
     def __call__(self, inputs):
         return self.predict(inputs)
 
-    def _save_pretrained(self, save_directory: str) -> None:
+    def _save_pretrained(self, save_directory: Union[Path, str]) -> None:
+        save_directory = str(save_directory)
         self.model_body.save(path=save_directory, create_model_card=False)
         self.create_model_card(path=save_directory, model_name=save_directory)
-        joblib.dump(self.model_head, f"{save_directory}/{MODEL_HEAD_NAME}")
+        joblib.dump(self.model_head, str(Path(save_directory) / MODEL_HEAD_NAME))
 
     @classmethod
     def _from_pretrained(
         cls,
         model_id: str,
         revision: Optional[str] = None,
         cache_dir: Optional[str] = None,
@@ -562,15 +580,15 @@
                     else:
                         raise ValueError(f"multi_target_strategy {multi_target_strategy} is not supported.")
 
                     model_head = multilabel_classifier
                 else:
                     model_head = clf
 
-        return SetFitModel(
+        return cls(
             model_body=model_body,
             model_head=model_head,
             multi_target_strategy=multi_target_strategy,
             normalize_embeddings=normalize_embeddings,
         )
 
 
@@ -673,27 +691,29 @@
 
 
 def sentence_pairs_generation(sentences, labels, pairs):
     # Initialize two empty lists to hold the (sentence, sentence) pairs and
     # labels to indicate if a pair is positive or negative
 
     num_classes = np.unique(labels)
-    idx = [np.where(labels == i)[0] for i in num_classes]
+    label_to_idx = {x: i for i, x in enumerate(num_classes)}
+    positive_idxs = [np.where(labels == i)[0] for i in num_classes]
+    negative_idxs = [np.where(labels != i)[0] for i in num_classes]
 
     for first_idx in range(len(sentences)):
         current_sentence = sentences[first_idx]
         label = labels[first_idx]
-        second_idx = np.random.choice(idx[np.where(num_classes == label)[0][0]])
+        second_idx = np.random.choice(positive_idxs[label_to_idx[label]])
         positive_sentence = sentences[second_idx]
         # Prepare a positive pair and update the sentences and labels
         # lists, respectively
         pairs.append(InputExample(texts=[current_sentence, positive_sentence], label=1.0))
 
-        negative_idx = np.where(labels != label)[0]
-        negative_sentence = sentences[np.random.choice(negative_idx)]
+        third_idx = np.random.choice(negative_idxs[label_to_idx[label]])
+        negative_sentence = sentences[third_idx]
         # Prepare a negative pair of sentences and update our lists
         pairs.append(InputExample(texts=[current_sentence, negative_sentence], label=0.0))
     # Return a 2-tuple of our sentence pairs and labels
     return pairs
 
 
 def sentence_pairs_generation_multilabel(sentences, labels, pairs):
```

### Comparing `setfit-0.6.0/src/setfit/trainer.py` & `setfit-0.7.0/src/setfit/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import math
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Union
 
 import evaluate
 import numpy as np
+from datasets import DatasetDict
 from sentence_transformers import InputExample, losses
 from sentence_transformers.datasets import SentenceLabelDataset
 from sentence_transformers.losses.BatchHardTripletLoss import BatchHardTripletLossDistanceFunction
 from torch.utils.data import DataLoader
+from tqdm.auto import trange
 from transformers.trainer_utils import HPSearchBackend, default_compute_objective, number_of_arguments, set_seed
 
 from . import logging
 from .integrations import default_hp_search_backend, is_optuna_available, run_hp_search_optuna
 from .modeling import SupConLoss, sentence_pairs_generation, sentence_pairs_generation_multilabel
 from .utils import BestRun, default_hp_space_optuna
 
@@ -37,14 +39,17 @@
             The evaluation dataset.
         model_init (`Callable[[], SetFitModel]`, *optional*):
             A function that instantiates the model to be used. If provided, each call to [`~SetFitTrainer.train`] will start
             from a new instance of the model as given by this function when a `trial` is passed.
         metric (`str` or `Callable`, *optional*, defaults to `"accuracy"`):
             The metric to use for evaluation. If a string is provided, we treat it as the metric name and load it with default settings.
             If a callable is provided, it must take two arguments (`y_pred`, `y_test`).
+        metric_kwargs (`Dict[str, Any]`, *optional*):
+            Keyword arguments passed to the evaluation function if `metric` is an evaluation string like "f1".
+            For example useful for providing an averaging strategy for computing f1 in a multi-label setting.
         loss_class (`nn.Module`, *optional*, defaults to `CosineSimilarityLoss`):
             The loss function to use for contrastive training.
         num_iterations (`int`, *optional*, defaults to `20`):
             The number of iterations to generate sentence pairs for.
             This argument is ignored if triplet loss is used.
             It is only used in conjunction with `CosineSimilarityLoss`.
         num_epochs (`int`, *optional*, defaults to `1`):
@@ -78,14 +83,15 @@
     def __init__(
         self,
         model: Optional["SetFitModel"] = None,
         train_dataset: Optional["Dataset"] = None,
         eval_dataset: Optional["Dataset"] = None,
         model_init: Optional[Callable[[], "SetFitModel"]] = None,
         metric: Union[str, Callable[["Dataset", "Dataset"], Dict[str, float]]] = "accuracy",
+        metric_kwargs: Optional[Dict[str, Any]] = None,
         loss_class=losses.CosineSimilarityLoss,
         num_iterations: int = 20,
         num_epochs: int = 1,
         learning_rate: float = 2e-5,
         batch_size: int = 16,
         seed: int = 42,
         column_mapping: Optional[Dict[str, str]] = None,
@@ -100,14 +106,15 @@
                 f"warmup_proportion must be greater than or equal to 0.0 and less than or equal to 1.0! But it was: {warmup_proportion}"
             )
 
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.model_init = model_init
         self.metric = metric
+        self.metric_kwargs = metric_kwargs
         self.loss_class = loss_class
         self.num_iterations = num_iterations
         self.num_epochs = num_epochs
         self.learning_rate = learning_rate
         self.batch_size = batch_size
         self.seed = seed
         self.column_mapping = column_mapping
@@ -133,26 +140,41 @@
     def _validate_column_mapping(self, dataset: "Dataset") -> None:
         """
         Validates the provided column mapping against the dataset.
         """
         required_columns = {"text", "label"}
         column_names = set(dataset.column_names)
         if self.column_mapping is None and not required_columns.issubset(column_names):
-            raise ValueError(
-                f"A column mapping must be provided when the dataset does not contain the following columns: {required_columns}"
-            )
+            # Issue #226: load_dataset will automatically assign points to "train" if no split is specified
+            if column_names == {"train"} and isinstance(dataset, DatasetDict):
+                raise ValueError(
+                    "SetFit expected a Dataset, but it got a DatasetDict with the split ['train']. "
+                    "Did you mean to select the training split with dataset['train']?"
+                )
+            elif isinstance(dataset, DatasetDict):
+                raise ValueError(
+                    f"SetFit expected a Dataset, but it got a DatasetDict with the splits {sorted(column_names)}. "
+                    "Did you mean to select one of these splits from the dataset?"
+                )
+            else:
+                raise ValueError(
+                    f"SetFit expected the dataset to have the columns {sorted(required_columns)}, "
+                    f"but only the columns {sorted(column_names)} were found. "
+                    "Either make sure these columns are present, or specify which columns to use with column_mapping in SetFitTrainer."
+                )
         if self.column_mapping is not None:
             missing_columns = required_columns.difference(self.column_mapping.values())
             if missing_columns:
                 raise ValueError(
                     f"The following columns are missing from the column mapping: {missing_columns}. Please provide a mapping for all required columns."
                 )
             if not set(self.column_mapping.keys()).issubset(column_names):
                 raise ValueError(
-                    f"The following columns are missing from the dataset: {set(self.column_mapping.keys()).difference(column_names)}. Please provide a mapping for all required columns."
+                    f"The column mapping expected the columns {sorted(self.column_mapping.keys())} in the dataset, "
+                    f"but the dataset had the columns {sorted(column_names)}."
                 )
 
     def _apply_column_mapping(self, dataset: "Dataset", column_mapping: Dict[str, str]) -> "Dataset":
         """
         Applies the provided column mapping to the dataset, renaming columns accordingly.
         Extra features not in the column mapping are prefixed with `"feat_"`.
         """
@@ -345,15 +367,15 @@
                         model=self.model.model_body,
                         distance_metric=self.distance_metric,
                         margin=self.margin,
                     )
             else:
                 train_examples = []
 
-                for _ in range(self.num_iterations):
+                for _ in trange(self.num_iterations, desc="Generating Training Pairs", disable=not show_progress_bar):
                     if self.model.multi_target_strategy is not None:
                         train_examples = sentence_pairs_generation_multilabel(
                             np.array(x_train), np.array(y_train), train_examples
                         )
                     else:
                         train_examples = sentence_pairs_generation(
                             np.array(x_train), np.array(y_train), train_examples
@@ -413,16 +435,17 @@
 
         logger.info("***** Running evaluation *****")
         y_pred = self.model.predict(x_test)
 
         if isinstance(self.metric, str):
             metric_config = "multilabel" if self.model.multi_target_strategy is not None else None
             metric_fn = evaluate.load(self.metric, config_name=metric_config)
+            metric_kwargs = self.metric_kwargs or {}
 
-            return metric_fn.compute(predictions=y_pred, references=y_test)
+            return metric_fn.compute(predictions=y_pred, references=y_test, **metric_kwargs)
 
         elif callable(self.metric):
             return self.metric(y_pred, y_test)
 
         else:
             raise ValueError("metric must be a string or a callable")
 
@@ -498,34 +521,49 @@
             HPSearchBackend.OPTUNA: run_hp_search_optuna,
         }
         best_run = backend_dict[backend](self, n_trials, direction, **kwargs)
 
         self.hp_search_backend = None
         return best_run
 
-    def push_to_hub(
-        self,
-        repo_path_or_name: Optional[str] = None,
-        repo_url: Optional[str] = None,
-        commit_message: Optional[str] = "Add SetFit model",
-        organization: Optional[str] = None,
-        private: Optional[bool] = None,
-        api_endpoint: Optional[str] = None,
-        use_auth_token: Optional[Union[bool, str]] = None,
-        git_user: Optional[str] = None,
-        git_email: Optional[str] = None,
-        config: Optional[dict] = None,
-        skip_lfs_files: bool = False,
-    ):
-        return self.model.push_to_hub(
-            repo_path_or_name,
-            repo_url,
-            commit_message,
-            organization,
-            private,
-            api_endpoint,
-            use_auth_token,
-            git_user,
-            git_email,
-            config,
-            skip_lfs_files,
-        )
+    def push_to_hub(self, repo_id: str, **kwargs) -> str:
+        """Upload model checkpoint to the Hub using `huggingface_hub`.
+
+        See the full list of parameters for your `huggingface_hub` version in the\
+        [huggingface_hub documentation](https://huggingface.co/docs/huggingface_hub/package_reference/mixins#huggingface_hub.ModelHubMixin.push_to_hub).
+
+        Args:
+            repo_id (`str`):
+                The full repository ID to push to, e.g. `"tomaarsen/setfit_sst2"`.
+            config (`dict`, *optional*):
+                Configuration object to be saved alongside the model weights.
+            commit_message (`str`, *optional*):
+                Message to commit while pushing.
+            private (`bool`, *optional*, defaults to `False`):
+                Whether the repository created should be private.
+            api_endpoint (`str`, *optional*):
+                The API endpoint to use when pushing the model to the hub.
+            token (`str`, *optional*):
+                The token to use as HTTP bearer authorization for remote files.
+                If not set, will use the token set when logging in with
+                `transformers-cli login` (stored in `~/.huggingface`).
+            branch (`str`, *optional*):
+                The git branch on which to push the model. This defaults to
+                the default branch as specified in your repository, which
+                defaults to `"main"`.
+            create_pr (`boolean`, *optional*):
+                Whether or not to create a Pull Request from `branch` with that commit.
+                Defaults to `False`.
+            allow_patterns (`List[str]` or `str`, *optional*):
+                If provided, only files matching at least one pattern are pushed.
+            ignore_patterns (`List[str]` or `str`, *optional*):
+                If provided, files matching any of the patterns are not pushed.
+
+        Returns:
+            str: The url of the commit of your model in the given repository.
+        """
+        if "/" not in repo_id:
+            raise ValueError(
+                '`repo_id` must be a full repository ID, including organisation, e.g. "tomaarsen/setfit_sst2".'
+            )
+        commit_message = kwargs.pop("commit_message", "Add SetFit model")
+        return self.model.push_to_hub(repo_id, commit_message=commit_message, **kwargs)
```

### Comparing `setfit-0.6.0/src/setfit/trainer_distillation.py` & `setfit-0.7.0/src/setfit/trainer_distillation.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,16 +188,22 @@
                         distance_metric=BatchHardTripletLossDistanceFunction.cosine_distance,
                         margin=0.25,
                     )
             else:
                 train_examples = []
 
                 # **************** student training ****************
-                x_train_embd_student = self.teacher_model.model_body.encode(x_train)
+                x_train_embd_student = self.teacher_model.model_body.encode(
+                    x_train, convert_to_tensor=self.teacher_model.has_differentiable_head
+                )
                 y_train = self.teacher_model.model_head.predict(x_train_embd_student)
+                if not self.teacher_model.has_differentiable_head and self.student_model.has_differentiable_head:
+                    y_train = torch.from_numpy(y_train)
+                elif self.teacher_model.has_differentiable_head and not self.student_model.has_differentiable_head:
+                    y_train = y_train.detach().cpu().numpy()
 
                 cos_sim_matrix = util.cos_sim(x_train_embd_student, x_train_embd_student)
 
                 train_examples = []
                 for _ in range(self.num_iterations):
                     train_examples = sentence_pairs_generation_cos_sim(
                         np.array(x_train), train_examples, cos_sim_matrix
```

### Comparing `setfit-0.6.0/src/setfit/utils.py` & `setfit-0.7.0/src/setfit/utils.py`

 * *Files identical despite different names*

### Comparing `setfit-0.6.0/src/setfit.egg-info/PKG-INFO` & `setfit-0.7.0/src/setfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: setfit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Efficient few-shot learning with Sentence Transformers
 Home-page: https://github.com/SetFit/setfit
 Download-URL: https://github.com/SetFit/setfit/tags
 Maintainer: Lewis Tunstall, Tom Aarsen
 Maintainer-email: lewis@huggingface.co
 License: Apache 2.0
 Keywords: nlp,machine learning,fewshot learning,transformers
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: optuna
 Provides-Extra: quality
 Provides-Extra: tests
 Provides-Extra: onnx
 Provides-Extra: openvino
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: compat_tests
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/huggingface/setfit/main/assets/setfit.png">
 
 <p align="center">
@@ -424,23 +424,22 @@
 ├── setup.cfg       <- Configuration file to define package metadata
 ├── setup.py        <- Make this project pip installable with `pip install -e`
 ├── src             <- Source code for SetFit
 └── tests           <- Unit tests
 ```
 
 ## Related work
+
 * [jxpress/setfit-pytorch-lightning](https://github.com/jxpress/setfit-pytorch-lightning) - A PyTorch Lightning implementation of SetFit.
 
 ## Citation
 
 ```@misc{https://doi.org/10.48550/arxiv.2209.11055,
   doi = {10.48550/ARXIV.2209.11055},
   url = {https://arxiv.org/abs/2209.11055},
   author = {Tunstall, Lewis and Reimers, Nils and Jo, Unso Eun Seo and Bates, Luke and Korat, Daniel and Wasserblat, Moshe and Pereg, Oren},
   keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
   title = {Efficient Few-Shot Learning Without Prompts},
   publisher = {arXiv},
   year = {2022},
   copyright = {Creative Commons Attribution 4.0 International}}
 ```
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: setfit Version: 0.6.0 Summary: Efficient few-shot
+Metadata-Version: 2.1 Name: setfit Version: 0.7.0 Summary: Efficient few-shot
 learning with Sentence Transformers Home-page: https://github.com/SetFit/setfit
 Download-URL: https://github.com/SetFit/setfit/tags Maintainer: Lewis Tunstall,
 Tom Aarsen Maintainer-email: lewis@huggingface.co License: Apache 2.0 Keywords:
-nlp,machine learning,fewshot learning,transformers Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
-text/markdown Provides-Extra: optuna Provides-Extra: quality Provides-Extra:
-tests Provides-Extra: onnx Provides-Extra: openvino Provides-Extra: dev
+nlp,machine learning,fewshot learning,transformers Classifier: Development
+Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
+Provides-Extra: optuna Provides-Extra: quality Provides-Extra: tests Provides-
+Extra: onnx Provides-Extra: openvino Provides-Extra: docs Provides-Extra: dev
 Provides-Extra: compat_tests License-File: LICENSE [https://
 raw.githubusercontent.com/huggingface/setfit/main/assets/setfit.png]
                 ð¤ Models_&_Datasets | ð Blog | ð Paper
 # SetFit - Efficient Few-shot Learning with Sentence Transformers SetFit is an
 efficient and prompt-free framework for few-shot fine-tuning of [Sentence
 Transformers](https://sbert.net/). It achieves high accuracy with little
 labeled data - for instance, with only 8 labeled examples per class on the
```

### Comparing `setfit-0.6.0/src/setfit.egg-info/SOURCES.txt` & `setfit-0.7.0/src/setfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

