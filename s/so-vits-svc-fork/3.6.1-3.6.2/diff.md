# Comparing `tmp/so_vits_svc_fork-3.6.1.tar.gz` & `tmp/so_vits_svc_fork-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.6.1.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.6.2.tar", max compression
```

## Comparing `so_vits_svc_fork-3.6.1.tar` & `so_vits_svc_fork-3.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-14 01:52:51.458950 so_vits_svc_fork-3.6.1/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-14 01:52:51.458950 so_vits_svc_fork-3.6.1/README.md
--rw-r--r--   0        0        0     3113 2023-04-14 01:52:52.474943 so_vits_svc_fork-3.6.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-14 01:52:52.426943 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-14 01:52:51.462950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-14 01:52:51.462950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-14 01:52:51.462950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25206 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1213 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1649 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1399 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1460 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    18383 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-14 01:52:51.466950 so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-14 11:56:20.132239 so_vits_svc_fork-3.6.2/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-14 11:56:20.132239 so_vits_svc_fork-3.6.2/README.md
+-rw-r--r--   0        0        0     3092 2023-04-14 11:56:21.104230 so_vits_svc_fork-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-14 11:56:21.056231 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1352 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2868 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25206 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1213 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1649 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1399 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1460 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2793 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4646 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4382 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:56:20.136239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    18383 2023-04-14 11:56:20.140239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13208 2023-04-14 11:56:20.140239 so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19923 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.6.2/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.6.1/LICENSE` & `so_vits_svc_fork-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/README.md` & `so_vits_svc_fork-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/pyproject.toml` & `so_vits_svc_fork-3.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.6.1"
+version = "3.6.2"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -58,15 +58,14 @@
 tqdm-joblib = "*"
 tensorboardx = "*"
 pyinputplus = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6"
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
-unidecode = "^1.3.6"
 lightning = "^2.0.1"
 fastapi = "==0.88"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Any
 
 import torch
 from sklearn.cluster import KMeans
 
 
 def get_cluster_model(ckpt_path: Path | str):
-    checkpoint = torch.load(ckpt_path)
+    with Path(ckpt_path).open("rb") as f:
+        checkpoint = torch.load(f, map_location="cpu", weights_only=True)
     kmeans_dict = {}
     for spk, ckpt in checkpoint.items():
         km = KMeans(ckpt["n_features_in_"])
         km.__dict__["n_features_in_"] = ckpt["n_features_in_"]
         km.__dict__["_n_threads"] = ckpt["_n_threads"]
         km.__dict__["cluster_centers_"] = ckpt["cluster_centers_"]
         kmeans_dict[spk] = km
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     use_minibatch: bool = True,
     verbose: bool = False,
 ) -> dict:
     input_dir = Path(input_dir)
     LOG.info(f"Loading features from {input_dir}")
     features = []
     for path in input_dir.rglob("*.data.pt"):
-        features.append(
-            torch.load(path, weights_only=True)["content"].squeeze(0).numpy().T
-        )
+        with path.open("rb") as f:
+            features.append(
+                torch.load(f, weights_only=True)["content"].squeeze(0).numpy().T
+            )
     if not features:
         raise ValueError(f"No features found in {input_dir}")
     features = np.concatenate(features, axis=0).astype(np.float32)
     if features.shape[0] < n_clusters:
         raise ValueError(
             "Too few HuBERT features to cluster. Consider using a smaller number of clusters."
         )
@@ -82,8 +83,9 @@
                 verbose=verbose,
             )
             for speaker_name in input_dir.iterdir()
         )
     assert parallel_result is not None
     checkpoint = dict(parallel_result)
     output_path.parent.mkdir(exist_ok=True, parents=True)
-    torch.save(checkpoint, output_path)
+    with output_path.open("wb") as f:
+        torch.save(checkpoint, f)
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         ]
         self.hps = hps
         self.random = Random(hps.train.seed)
         self.random.shuffle(self.datapaths)
         self.max_spec_len = 800
 
     def __getitem__(self, index: int) -> dict[str, torch.Tensor]:
-        data = torch.load(self.datapaths[index], weights_only=True, map_location="cpu")
+        with Path(self.datapaths[index]).open("rb") as f:
+            data = torch.load(f, weights_only=True, map_location="cpu")
 
         # cut long data randomly
         spec_len = data["mel_spec"].shape[1]
         hop_len = self.hps.data.hop_length
         if spec_len > self.max_spec_len:
             start = self.random.randint(0, spec_len - self.max_spec_len)
             end = start + self.max_spec_len - 10
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,19 +32,15 @@
     test = []
     spk_dict = {}
     spk_id = 0
     for speaker in os.listdir(input_dir):
         spk_dict[speaker] = spk_id
         spk_id += 1
         paths = []
-        for path in tqdm(list((input_dir / speaker).glob("**/*.wav"))):
-            if not path.name.isascii():
-                LOG.warning(
-                    f"file name {path} contains non-ascii characters. torch.save() and torch.load() may not work."
-                )
+        for path in tqdm(list((input_dir / speaker).rglob("*.wav"))):
             if get_duration(filename=path) < 0.3:
                 LOG.warning(f"skip {path} because it is too short.")
                 continue
             paths.append(path)
         shuffle(paths)
         if len(paths) <= 4:
             raise ValueError(
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,16 @@
         "f0": f0,
         "uv": uv,
         "content": c,
         "audio": audio,
         "spk": spk,
     }
     data = {k: v.cpu() for k, v in data.items()}
-    torch.save(data, data_path)
+    with data_path.open("wb") as f:
+        torch.save(data, f)
 
 
 def _process_batch(filepaths: Iterable[Path], pbar_position: int, **kwargs):
     content_model = utils.get_hubert_model(get_optimal_device())
 
     for filepath in tqdm(filepaths, position=pbar_position):
         _process_one(
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pathlib import Path
 from typing import Iterable
 
 import librosa
 import soundfile
 from joblib import Parallel, delayed
 from tqdm_joblib import tqdm_joblib
-from unidecode import unidecode
 
 from .preprocess_utils import check_hubert_min_duration
 
 LOG = getLogger(__name__)
 
 # input_dir and output_dir exists.
 # write code to convert input dir audio files to output dir audio files,
@@ -119,21 +118,14 @@
             )
             in_path_relative = new_in_path_relative
 
         if len(in_path_relative.parts) < 2:
             continue
         speaker_name = in_path_relative.parts[0]
         file_name = in_path_relative.with_suffix(".wav").name
-        new_filename = unidecode(file_name)
-        if new_filename != file_name:
-            LOG.warning(
-                f"Filename {file_name} contains non-ASCII characters. "
-                f"Replaced with {new_filename}."
-            )
-            file_name = new_filename
         out_path = output_dir / speaker_name / file_name
         out_path = _get_unique_filename(out_path, out_paths)
         out_path.parent.mkdir(parents=True, exist_ok=True)
         in_paths.append(in_path)
         out_paths.append(out_path)
 
     in_and_out_paths = list(zip(in_paths, out_paths))
```

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.6.1/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.6.2/src/so_vits_svc_fork/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,16 @@
     checkpoint_path: Path | str,
     model: torch.nn.Module,
     optimizer: torch.optim.Optimizer | None = None,
     skip_optimizer: bool = False,
 ) -> tuple[torch.nn.Module, torch.optim.Optimizer | None, float, int]:
     if not Path(checkpoint_path).is_file():
         raise FileNotFoundError(f"File {checkpoint_path} not found")
-    checkpoint_dict = torch.load(checkpoint_path, map_location="cpu")
+    with Path(checkpoint_path).open("rb") as f:
+        checkpoint_dict = torch.load(f, map_location="cpu", weights_only=True)
     iteration = checkpoint_dict["iteration"]
     learning_rate = checkpoint_dict["learning_rate"]
 
     # safe load module
     if hasattr(model, "module"):
         safe_load(model.module, checkpoint_dict["model"])
     else:
@@ -256,23 +257,24 @@
             iteration, checkpoint_path
         )
     )
     if hasattr(model, "module"):
         state_dict = model.module.state_dict()
     else:
         state_dict = model.state_dict()
-    torch.save(
-        {
-            "model": state_dict,
-            "iteration": iteration,
-            "optimizer": optimizer.state_dict(),
-            "learning_rate": learning_rate,
-        },
-        checkpoint_path,
-    )
+    with Path(checkpoint_path).open("wb") as f:
+        torch.save(
+            {
+                "model": state_dict,
+                "iteration": iteration,
+                "optimizer": optimizer.state_dict(),
+                "learning_rate": learning_rate,
+            },
+            f,
+        )
 
 
 def clean_checkpoints(
     path_to_models: Path | str, n_ckpts_to_keep: int = 2, sort_by_time: bool = True
 ) -> None:
     """Freeing up space by deleting saved ckpts
```

### Comparing `so_vits_svc_fork-3.6.1/PKG-INFO` & `so_vits_svc_fork-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.6.1
+Version: 3.6.2
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,15 +45,14 @@
 Requires-Dist: tensorboard
 Requires-Dist: tensorboardx
 Requires-Dist: torch (>=1.12)
 Requires-Dist: torchaudio (>=0.12)
 Requires-Dist: torchcrepe (>=0.0.17)
 Requires-Dist: tqdm
 Requires-Dist: tqdm-joblib
-Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/34j/so-vits-svc-fork/issues
 Project-URL: Changelog, https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://so-vits-svc-fork.readthedocs.io
 Project-URL: Repository, https://github.com/34j/so-vits-svc-fork
 Description-Content-Type: text/markdown
 
 # SoftVC VITS Singing Voice Conversion Fork
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.6.1 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.6.2 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -14,21 +14,21 @@
 (>=1.23,<2.0) Requires-Dist: onnx Requires-Dist: onnxoptimizer Requires-Dist:
 onnxsim Requires-Dist: pebble (>=5.0) Requires-Dist: praat-parselmouth
 Requires-Dist: pydub Requires-Dist: pyinputplus Requires-Dist: pysimplegui
 (>=4.6) Requires-Dist: pyworld Requires-Dist: requests Requires-Dist: rich
 Requires-Dist: scikit-maad Requires-Dist: scipy Requires-Dist: sounddevice
 Requires-Dist: starlette Requires-Dist: tensorboard Requires-Dist: tensorboardx
 Requires-Dist: torch (>=1.12) Requires-Dist: torchaudio (>=0.12) Requires-Dist:
-torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-Dist: tqdm-joblib Requires-
-Dist: unidecode (>=1.3.6,<2.0.0) Project-URL: Bug Tracker, https://github.com/
-34j/so-vits-svc-fork/issues Project-URL: Changelog, https://github.com/34j/so-
-vits-svc-fork/blob/main/CHANGELOG.md Project-URL: Documentation, https://so-
-vits-svc-fork.readthedocs.io Project-URL: Repository, https://github.com/34j/
-so-vits-svc-fork Description-Content-Type: text/markdown # SoftVC VITS Singing
-Voice Conversion Fork [ç®ä½ä¸­æ](README_zh_CN.md)
+torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-Dist: tqdm-joblib Project-
+URL: Bug Tracker, https://github.com/34j/so-vits-svc-fork/issues Project-URL:
+Changelog, https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://so-vits-svc-fork.readthedocs.io Project-
+URL: Repository, https://github.com/34j/so-vits-svc-fork Description-Content-
+Type: text/markdown # SoftVC VITS Singing Voice Conversion Fork [ç®ä½ä¸­æ]
+(README_zh_CN.md)
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with
 **realtime support** and **greatly improved interface**. Based on branch `4.0`
 (v1) and the models are compatible. ## Features not available in the original
 repo - **Realtime voice conversion** (enhanced in v1.1.0) - Integrates
```

