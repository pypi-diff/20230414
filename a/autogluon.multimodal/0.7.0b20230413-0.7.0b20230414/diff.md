# Comparing `tmp/autogluon.multimodal-0.7.0b20230413.tar.gz` & `tmp/autogluon.multimodal-0.7.0b20230414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.0b20230413.tar", last modified: Thu Apr 13 09:04:33 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.0b20230414.tar", last modified: Fri Apr 14 09:04:19 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.0b20230413.tar` & `autogluon.multimodal-0.7.0b20230414.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.329052 autogluon.multimodal-0.7.0b20230413/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-13 09:04:33.329052 autogluon.multimodal-0.7.0b20230413/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:04:33.329052 autogluon.multimodal-0.7.0b20230413/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.317052 autogluon.multimodal-0.7.0b20230413/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.317052 autogluon.multimodal-0.7.0b20230413/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.321051 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.321051 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.321051 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26476 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.321051 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85367 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.325052 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.325052 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.325052 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   121528 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24352 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.329052 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29541 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    50614 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-13 09:03:58.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:33.321051 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:33.000000 autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.933719 autogluon.multimodal-0.7.0b20230414/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-14 09:04:19.933719 autogluon.multimodal-0.7.0b20230414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:04:19.933719 autogluon.multimodal-0.7.0b20230414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.921718 autogluon.multimodal-0.7.0b20230414/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.921718 autogluon.multimodal-0.7.0b20230414/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.925718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.925718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.925718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26476 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.925718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85367 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.929718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.929718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.929718 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121528 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24352 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.933719 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29541 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50614 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-14 09:03:45.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:19.921718 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:04:19.000000 autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.0b20230413/PKG-INFO` & `autogluon.multimodal-0.7.0b20230414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.0b20230413
+Version: 0.7.0b20230414
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.0b20230413/setup.py` & `autogluon.multimodal-0.7.0b20230414/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.0b20230414/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.0b20230413
+Version: 0.7.0b20230414
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.0b20230413/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.0b20230414/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.0b20230413
-autogluon.features==0.7.0b20230413
-autogluon.common==0.7.0b20230413
+autogluon.core[raytune]==0.7.0b20230414
+autogluon.features==0.7.0b20230414
+autogluon.common==0.7.0b20230414
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>0.1.5
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```
