# Comparing `tmp/e2eAIOK-1.0.1b2023041100.tar.gz` & `tmp/e2eAIOK-1.0.1b2023041400.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e2eAIOK-1.0.1b2023041100.tar", last modified: Tue Apr 11 00:02:58 2023, max compression
+gzip compressed data, was "dist/e2eAIOK-1.0.1b2023041400.tar", last modified: Fri Apr 14 00:44:58 2023, max compression
```

## Comparing `e2eAIOK-1.0.1b2023041100.tar` & `e2eAIOK-1.0.1b2023041400.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/TransformerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/TransformerLM.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/asr_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/asr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/augment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/wer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/init_asr_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/supernet_asr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/Accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/asr_nas.py
--rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/metric_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/DeNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/benchmark_network_latency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/cv_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/supernet_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/ZenNet.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/Linear_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/attention_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/multihead_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/qkv_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/embedding_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/layernorm_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/bert_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/supernet_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/utils_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/compute_de_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/transformer_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/BaseSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/RandomSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/SearchEngineFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/SigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/supernet_hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/office31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/default_ma.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/finetunner/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6002 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/SDA.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/image_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/torch_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/extend_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/dataloader/hydrodataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroautolearner.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroconnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydromodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydromodelzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroweblistener.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 00:02:57.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:02:58.000000 e2eAIOK-1.0.1b2023041100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-11 00:02:52.000000 e2eAIOK-1.0.1b2023041100/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-14 00:44:54.000000 e2eAIOK-1.0.1b2023041400/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/TransformerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/TransformerLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/asr_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/asr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/augment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/wer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/init_asr_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/supernet_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/Accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/asr_nas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/metric_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/DeNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/benchmark_network_latency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/cv_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/supernet_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/ZenNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/Linear_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/attention_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/multihead_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/qkv_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/embedding_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/layernorm_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/bert_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/supernet_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/utils_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/compute_de_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/transformer_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/BaseSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/RandomSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/SearchEngineFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/SigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/supernet_hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/office31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/default_ma.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/finetunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6002 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/SDA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/torch_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/extend_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/dataloader/hydrodataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroautolearner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroconnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydromodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydromodelzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroweblistener.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 00:44:57.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:44:58.000000 e2eAIOK-1.0.1b2023041400/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-14 00:44:55.000000 e2eAIOK-1.0.1b2023041400/setup.py
```

### Comparing `e2eAIOK-1.0.1b2023041100/PKG-INFO` & `e2eAIOK-1.0.1b2023041400/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK
-Version: 1.0.1b2023041100
+Version: 1.0.1b2023041400
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
```

### Comparing `e2eAIOK-1.0.1b2023041100/README.md` & `e2eAIOK-1.0.1b2023041400/README.md`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/TransformerBase.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/TransformerBase.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/TransformerLM.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/TransformerLM.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/asr_model_builder.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/asr_model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/asr_trainer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/asr_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/augment.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/augment.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/batch.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/batch.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataio.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataio.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataloader.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/dataset.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/sampler.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/sampler.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/dataio/wer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/dataio/wer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/features.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/librispeech_prepare.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/librispeech_prepare.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/features.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/signal_processing.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/signal_processing.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/ctc.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/ctc.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/decoders/seq2seq.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/decoders/seq2seq.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/init_asr_parser.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/init_asr_parser.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/CNN.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/CNN.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/containers.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/containers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/lib/convolution.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/lib/convolution.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/model_builder_denas_asr.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/model_builder_denas_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/supernet_asr.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/supernet_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/losses.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/losses.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/trainer/schedulers.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/trainer/schedulers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/Accuracy.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/Accuracy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/asr_nas.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/asr_nas.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/checkpoints.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/data_pipeline.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/data_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/depgraph.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/depgraph.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/distributed.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/edit_distance.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/edit_distance.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/metric_stats.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/metric_stats.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/parameter_transfer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/parameter_transfer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/asr/utils/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/asr/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/benchmark_network_latency.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/benchmark_network_latency.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/cv_trainer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/cv_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/model_builder_denas_cv.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/model_builder_denas_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/supernet_transformer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/supernet_transformer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/third_party/ZenNet.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/third_party/ZenNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/cnn.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/cv/utils/vit.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/cv/utils/vit.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/attention.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/attention.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/decoder.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/decoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/encoder.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/encoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/normalization.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/normalization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/asr/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/asr/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/Linear_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/embedding_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/layernorm_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/multihead_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/multihead_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/qkv_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/qkv_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/cv/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/cv/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/Linear_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_attention_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_attention_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/layernorm_super.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/optimization.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/optimization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/module/nlp/tokenization.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/module/nlp/tokenization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/bert_trainer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/bert_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/supernet_bert.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/supernet_bert.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/nlp/utils_eval.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/nlp/utils_eval.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/basic_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/basic_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/compute_de_score.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/compute_de_score.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/scores/transformer_proxy.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/scores/transformer_proxy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/BaseSearchEngine.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/BaseSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/RandomSearchEngine.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/RandomSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/SearchEngineFactory.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/SearchEngineFactory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/SigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/SigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/search.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/search.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/supernet_hf.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/supernet_hf.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/thirdparty/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/thirdparty/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/train.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/DeNas/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/DeNas/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/factory.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/__init__.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/cifar.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/composed_dataset.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/composed_dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/dataset/office31.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/dataset/office31.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/default_ma.conf` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/default_ma.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/main.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/main.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/task.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/task.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/ModelAdapter/training/train.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/ModelAdapter/training/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/SDA.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/SDA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         super().__init__(dataset_meta_path, train_path, eval_path, args)
         logging.basicConfig(
             level=logging.INFO,
             format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         self.logger = logging.getLogger('sigopt')
         self.python_path = self.params['python_path'] if "python_path" in self.params else "/opt/intel/oneapi/intelpython/latest/envs/tensorflow/bin"
         self.train_python = f"{self.python_path}/python"
-        self.train_script = os.path.join(os.getcwd(),"modelzoo/bert/benchmarks/launch_benchmark.py")
+        self.train_script =  self.params["train_script"] if "train_script" in self.params else os.path.join(os.getcwd(),"modelzoo/bert/benchmarks/launch_benchmark.py")
         self.train_path = train_path
         self.test_path = eval_path
         self.dataset_meta_path = dataset_meta_path
-        self.current_path = os.getcwd()
-        self.extra_pythonpath = f"{self.current_path}/modelzoo/bert/benchmarks/"
+        self.current_path = self.params["current_path"] if "current_path" in self.params else os.getcwd()
+        self.extra_pythonpath = os.path.join(self.current_path, "modelzoo/bert/benchmarks/")
 
     def initialize_model_parameter(self, assignments=None):
         '''
             Add model specific parameters
             For sigopt parameters, set parameter explicitly and the parameter will not be optimized by sigopt
         '''
         config = {}
@@ -107,15 +107,15 @@
             lines = f.readlines()
         self.training_time = float(lines[-1])
         metrics = self.update_metrics()
         return self.training_time, model_path, metrics
 
     def dist_launch(self, args):
         # construct BERT launch command
-        os.environ["MODEL_DIR"] = MODEL_DIR = os.path.join(os.getcwd(),"modelzoo/bert")
+        os.environ["MODEL_DIR"] = MODEL_DIR = os.path.join(self.current_path,"modelzoo/bert")
         os.environ["OUTPUT_DIR"] = OUT_DIR = self.params['model_saved_path']
         os.environ["DATASET_DIR"] = os.path.dirname(self.dataset_meta_path)
         os.environ["CHECKPOINT_DIR"] = "$DATASET_DIR/pre-trained-model/bert-large-uncased/wwm_uncased_L-24_H-1024_A-16"
         os.environ["HOROVOD_CPU_OPERATIONS"] = "CCL"
         os.environ["NOINSTALL"] = "True"
         os.environ["CCL_WORKER_COUNT"] = str(args['ccl_worker_num'])
         os.environ["CCL_WORKER_AFFINITY"] = "16,17,34,35"
@@ -167,15 +167,15 @@
 
         print(f'training launch command: {cmd}')
         process = subprocess.Popen(cmd, shell=True)
         process.wait()
 
     def launch(self, args):
         # construct BERT launch command
-        os.environ["MODEL_DIR"] = MODEL_DIR = os.path.join(os.getcwd(),"modelzoo/bert")
+        os.environ["MODEL_DIR"] = MODEL_DIR = os.path.join(self.current_path,"modelzoo/bert")
         os.environ["OUTPUT_DIR"] = OUT_DIR = self.params['model_saved_path']
         os.environ["DATASET_DIR"] = os.path.dirname(self.dataset_meta_path)
         os.environ["CHECKPOINT_DIR"] = "$DATASET_DIR/pre-trained-model/bert-large-uncased/wwm_uncased_L-24_H-1024_A-16"
         mpi_num_proc_arg = ""
 
         if not os.path.exists(os.environ["OUTPUT_DIR"]):
             os.makedirs(os.environ["OUTPUT_DIR"])
```

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,24 +60,24 @@
 
         Returns
         -------
         sigopt_experiment_id: str
           sigopt experiment id for this task
         """
         # 1. create sigopt yaml
-        sigopt_config = self.generate_sigopt_yaml()
-        yaml.dump(sigopt_config, sys.stdout)
+        hpo_config = self.generate_sigopt_yaml()
+        yaml.dump(hpo_config, sys.stdout)
         n = timeout_input("Please confirm with sigopt parameters?(n for exit)",
                           default='y', interactive=self.interative)
         if n != 'y':
             exit()
-        self.params['model_parameter'] = sigopt_config
+        self.params['model_parameter'] = hpo_config
         # 2. create sigopt connection
         self.conn, self.experiment = self._setup_sigopt_connection(
-            sigopt_config, experiment_id)
+            hpo_config, experiment_id)
         return self.experiment.id
 
     def register(self, info):
         for k, v in info.items():
             if k == "score_metrics" and 'metrics' in dir(self):
                 if not isinstance(v, list) or not (len(v) > 0 and isinstance(v[0], tuple)):
                     raise ValueError("[Register advisor] scores metrics should be a pair, ex: ('mean_accuracy', 'maximize')")
@@ -88,41 +88,41 @@
                 self.training_time_as_metrics = True
             if k == "hyper_parameters" and 'parameters' in dir(self):
                 if not isinstance(v, dict):
                     raise ValueError("""
         [Register advisor] hyper_parameters should be a dict, ex: 
         {'max_depth':11, 'learning_rate':float(0.9), 'min_split_loss':float(7)}""")
                 self.parameters = v
-            if k == "sigopt_config" and 'sigopt_config' in dir(self):
+            if k == "hpo_config" and 'hpo_config' in dir(self):
                 if not isinstance(v, list) or not (len(v) > 0 and isinstance(v[0], dict)):
                     raise ValueError("""
-        [Register advisor] sigopt_config should be a list, ex: 
+        [Register advisor] hpo_config should be a list, ex: 
         [{
             'name': 'learning_rate',
             'bounds': {
                 'min': 0.0,
                 'max': 1.0
             },
             'type': 'double'
         }]""")
-                self.sigopt_config = v
+                self.hpo_config = v
                 self.parameters = dict((i["name"], None) for i in v)
             if k == "execute_cmd" and "execute_cmd_base" in dir(self):
                 self.execute_cmd_base = v
             if k == "result_file_name" and "result_file_name" in dir(self):
                 self.result_file_name = v
             if k == "observation_budget" and "observation_budget" in dir(self):
                 self.observation_budget = v
 
-    def _setup_sigopt_connection(self, sigopt_config, experiment_id=None):
-        name = sigopt_config["experiment"]
-        parameters = sigopt_config["parameters"]
-        metrics = sigopt_config["metrics"]
-        observation_budget = sigopt_config["observation_budget"]
-        project = sigopt_config["project"]
+    def _setup_sigopt_connection(self, hpo_config, experiment_id=None):
+        name = hpo_config["experiment"]
+        parameters = hpo_config["parameters"]
+        metrics = hpo_config["metrics"]
+        observation_budget = hpo_config["observation_budget"]
+        project = hpo_config["project"]
 
         num_tried = 0
         while True:
             try:
                 conn = Connection()
                 if experiment_id:
                     experiment = conn.experiments(experiment_id).fetch()
```

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,45 +19,45 @@
         self.metrics = [("mean_accuracy", "maximize")]
         self.training_time_as_metrics = False
         self.parameters = {
             'max_depth':11,
             'learning_rate':float(0.9),
             'min_split_loss':float(7)
         }
-        self.sigopt_config = [{
+        self.hpo_config = [{
             'name': 'learning_rate',
             'bounds': {
                 'min': 0.0,
                 'max': 1.0
             },
             'type': 'double'
         }]
         self.execute_cmd_base = "/opt/intel/oneapi/intelpython/latest/bin/python /home/vmagent/app/e2eaiok/example/sklearn_train.py"
         self.result_file_name = "result"
         self.observation_budget = 1
         self.sigopt_enable_parameters = []
         self.sigopt_list_parameters = {}
 
-    def __fix(self, sigopt_config):
-        for k, v in enumerate(sigopt_config):
+    def __fix(self, hpo_config):
+        for k, v in enumerate(hpo_config):
             if 'grid' in v:
                 if ('type' in v and v['type'] in ['str', 'bool']) or (not 'type' in v):
                      # handle config with string grid
                      # handle config with bool config
                      max_len = len(v['grid'])
                      self.sigopt_list_parameters[v['name']] = v['grid']
-                     sigopt_config[k]['grid'] = list(range(max_len))
-                     sigopt_config[k]['type'] = 'int'
+                     hpo_config[k]['grid'] = list(range(max_len))
+                     hpo_config[k]['type'] = 'int'
             if len(v) == 1 and 'name' in v:
                 # handle config with no option
-                sigopt_config[k]['grid'] = [0, 1]
-                sigopt_config[k]['type'] = 'int'
+                hpo_config[k]['grid'] = [0, 1]
+                hpo_config[k]['type'] = 'int'
                 self.sigopt_enable_parameters.append(v['name'])
 
-        return sigopt_config
+        return hpo_config
 
 
     # ====== Implementation of required methods ======
 
     def update_metrics(self):
         metrics = []
         for metric in self.metrics:
@@ -82,15 +82,15 @@
             self.params['save_path'], get_hash_string(str(tuned_parameters)))
         return config
 
     def generate_sigopt_yaml(self, file='test_sigopt.yaml'):
         config = {}
         config['project'] = 'e2eaiok'
         config['experiment'] = self.experiment_name
-        config['parameters'] = self.__fix(self.sigopt_config)
+        config['parameters'] = self.__fix(self.hpo_config)
         config['metrics'] = []
         for metric in self.metrics:
             config['metrics'].append({
             'name': metric[0],
             'strategy': 'optimize',
             'objective': metric[1]
         })
```

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/TestAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/TestAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/default.conf` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/default.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_asr.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_cv.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_builder_nlp.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_builder_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/data_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/data_utils/image_list.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/data_utils/image_list.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/data_builder.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/data_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/lenet.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/lenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/cv/resnet_cifar.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model/model_utils/model_utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model/model_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/model_builder.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/torch_trainer.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/extend_distributed.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/extend_distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/trainer/utils/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/trainer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/common/utils.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/common/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/dataloader/hydrodataloader.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/dataloader/hydrodataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroDB.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroDB.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroautolearner.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroautolearner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroconfig.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroconfig.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydromodel.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydromodel.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK/utils/hydroserver.py` & `e2eAIOK-1.0.1b2023041400/e2eAIOK/utils/hydroserver.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/PKG-INFO` & `e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK
-Version: 1.0.1b2023041100
+Version: 1.0.1b2023041400
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
```

### Comparing `e2eAIOK-1.0.1b2023041100/e2eAIOK.egg-info/SOURCES.txt` & `e2eAIOK-1.0.1b2023041400/e2eAIOK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023041100/setup.py` & `e2eAIOK-1.0.1b2023041400/setup.py`

 * *Files identical despite different names*

