# Comparing `tmp/funasr-0.3.1.tar.gz` & `tmp/funasr-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr-0.3.1.tar", last modified: Fri Mar 24 05:27:56 2023, max compression
+gzip compressed data, was "dist/funasr-0.4.1.tar", last modified: Fri Apr 14 15:33:48 2023, max compression
```

## Comparing `funasr-0.3.1.tar` & `funasr-0.4.1.tar`

### file list

```diff
@@ -1,419 +1,437 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1063 2023-02-24 12:39:00.000000 funasr-0.3.1/LICENSE
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6390 2023-03-24 05:27:56.000000 funasr-0.3.1/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5377 2023-03-16 11:52:44.000000 funasr-0.3.1/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      203 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/bin/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/__init__.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3798 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/aggregate_stats_dirs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    21262 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/asr_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9742 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/asr_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    25900 2023-03-17 12:37:43.000000 funasr-0.3.1/funasr/bin/asr_inference_mfcca.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    37619 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/bin/asr_inference_paraformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    30396 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/bin/asr_inference_paraformer_streaming.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    19175 2023-02-24 16:26:34.000000 funasr-0.3.1/funasr/bin/asr_inference_paraformer_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    32907 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/bin/asr_inference_paraformer_vad_punc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    34233 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/asr_inference_rnnt.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23924 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/bin/asr_inference_uniasr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23920 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/bin/asr_inference_uniasr_vad.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1006 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/asr_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1027 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/asr_train_paraformer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1024 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/asr_train_uniasr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5309 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/bin/build_trainer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1012 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/data2vec_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5326 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/diar_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1010 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/bin/diar_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14072 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/eend_ola_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     6814 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/lm_calc_perplexity.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14615 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/lm_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3950 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/lm_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1019 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/lm_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3049 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/modelscope_infer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3728 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/bin/punc_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/bin/punc_train.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      866 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/bin/punc_train_vadrealtime.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12010 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/punctuation_infer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11203 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/bin/punctuation_infer_vadrealtime.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    20635 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/sond_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14771 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/bin/sv_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     4717 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/sv_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     8449 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/bin/tokenize_text.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12520 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/bin/tp_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4009 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/bin/tp_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12389 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/bin/vad_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4236 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/bin/vad_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11415 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/bin/vad_inference_online.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/datasets/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4338 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/collate_fn.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15155 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/datasets/dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15562 2023-03-17 12:37:43.000000 funasr-0.3.1/funasr/datasets/iterable_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12671 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/iterable_dataset_modelscope.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/datasets/large_datasets/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3488 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/datasets/large_datasets/build_dataloader.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/datasets/large_datasets/datapipes/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8298 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/datapipes/batch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      519 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/datapipes/filter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      453 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/datapipes/map.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8055 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/datasets/large_datasets/dataset.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1382 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/clipping.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1013 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/filter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      948 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1201 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/padding.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2038 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/datasets/large_datasets/utils/tokenize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1281 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/datasets/ms_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    30261 2023-03-17 12:37:43.000000 funasr-0.3.1/funasr/datasets/preprocessor.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9174 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/export/export_model.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/models/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      623 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/export/models/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/models/decoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/decoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6326 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/decoder/sanm_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5470 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/export/models/decoder/transformer_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8423 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/export/models/e2e_asr_paraformer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/models/encoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/encoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3881 2023-03-15 12:41:42.000000 funasr-0.3.1/funasr/export/models/encoder/conformer_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3894 2023-02-24 16:26:34.000000 funasr-0.3.1/funasr/export/models/encoder/sanm_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/models/modules/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/modules/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1931 2023-03-15 12:41:42.000000 funasr-0.3.1/funasr/export/models/modules/decoder_layer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2354 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/export/models/modules/encoder_layer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/modules/feedforward.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8633 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/export/models/modules/multihead_att.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/models/predictor/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/models/predictor/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9917 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/export/models/predictor/cif.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      785 2023-02-24 16:26:34.000000 funasr-0.3.1/funasr/export/test_onnx.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      492 2023-03-10 10:56:01.000000 funasr-0.3.1/funasr/export/test_torchscripts.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/torch_quant/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      642 2023-03-10 03:02:25.000000 funasr-0.3.1/funasr/export/torch_quant/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2385 2023-03-16 11:05:28.000000 funasr-0.3.1/funasr/export/torch_quant/amp_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18267 2023-03-15 12:46:52.000000 funasr-0.3.1/funasr/export/torch_quant/graph.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7297 2023-03-15 12:46:52.000000 funasr-0.3.1/funasr/export/torch_quant/module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2063 2023-03-15 12:46:52.000000 funasr-0.3.1/funasr/export/torch_quant/observed_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    30293 2023-03-15 12:46:52.000000 funasr-0.3.1/funasr/export/torch_quant/observer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10070 2023-03-15 12:46:52.000000 funasr-0.3.1/funasr/export/torch_quant/quantizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      620 2023-03-10 03:02:25.000000 funasr-0.3.1/funasr/export/torch_quant/version.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/export/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2620 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/export/utils/torch_function.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/fileio/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/fileio/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2383 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/fileio/datadir_writer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2357 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/fileio/npy_scp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2361 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/fileio/rand_gen_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2273 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/fileio/read_text.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3479 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/fileio/sound_scp.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/iterators/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/iterators/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      234 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/iterators/abs_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7808 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/iterators/chunk_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1140 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/iterators/multiple_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5236 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/iterators/sequence_iter_factory.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/layers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      359 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/abs_normalize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6717 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/complex_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3503 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/global_mvn.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      349 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/inversible_interface.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2539 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/layers/label_aggregation.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2564 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/log_mel.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10488 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/mask_along_axis.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9033 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/sinc_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8436 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/stft.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2513 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/time_warp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2309 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/layers/utterance_mvn.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/lm/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/lm/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      772 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/lm/abs_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4709 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/lm/espnet_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5904 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/lm/seq_rnn_lm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4243 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/lm/transformer_lm.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/losses/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/losses/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2804 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/losses/label_smoothing_loss.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/main_funcs/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/main_funcs/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4687 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/main_funcs/average_nbest_models.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5610 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/main_funcs/calculate_all_attentions.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5029 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/main_funcs/collect_stats.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9906 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/main_funcs/pack_funcs.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6541 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/ctc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5298 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/data2vec.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/decoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      473 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/abs_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    40825 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/contextual_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12133 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/rnn_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    75098 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/decoder/sanm_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1389 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/sv_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28519 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/decoder/transformer_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16707 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/e2e_asr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/e2e_asr_common.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11424 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/e2e_asr_mfcca.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    64443 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/e2e_asr_paraformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10238 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/e2e_diar_eend_ola.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20396 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/e2e_diar_sond.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10048 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/e2e_sv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6701 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/e2e_tp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    51728 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/e2e_uni_asr.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    30033 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/e2e_vad.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/encoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      503 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/abs_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23724 2023-02-24 16:26:34.000000 funasr-0.3.1/funasr/models/encoder/conformer_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20993 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/data2vec_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    19855 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10164 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/encoder_layer_mfcca.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9281 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/models/encoder/fsmn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    17514 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/mfcca_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      909 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11037 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13971 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    21161 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    40679 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/encoder/resnet34_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3634 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/rnn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    44349 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/encoder/sanm_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    26890 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/encoder/transformer_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/frontend/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      400 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/abs_frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8895 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/default.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1405 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/frontend/eend_ola_feature.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5759 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/fused.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4990 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/s3prl.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20527 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/frontend/wav_frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6322 2023-02-24 16:26:34.000000 funasr-0.3.1/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2817 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/frontend/windowing.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/pooling/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/pooling/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3546 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/models/pooling/statistic_pooling.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/postencoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/postencoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      403 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/postencoder/abs_postencoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3626 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/predictor/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/predictor/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    34319 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/models/predictor/cif.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/preencoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/preencoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      402 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/preencoder/abs_preencoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1042 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/preencoder/linear.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10296 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/preencoder/sinc.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/models/specaug/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/specaug/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      426 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/specaug/abs_specaug.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6607 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/models/specaug/specaug.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      940 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/add_sos_eos.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28945 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/modules/attention.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/beam_search/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/beam_search/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13305 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/beam_search/batch_beam_search.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10175 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    53592 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/beam_search/beam_search.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/data2vec/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5831 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/data_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4474 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/ema_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      442 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/grad_multiply.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    26458 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/multihead_attention.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4021 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/quant_noise.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4858 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12734 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/data2vec/wav2vec2.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4244 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/dynamic_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4863 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/dynamic_conv2d.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/e2e_asr_common.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/eend_ola/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/modules/eend_ola/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5287 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/modules/eend_ola/encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2768 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14256 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/modules/embedding.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/frontends/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2731 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/beamformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5540 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/dnn_beamformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2825 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/dnn_wpe.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7958 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/feature_transform.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4585 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2648 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/frontends/mask_estimator.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      958 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/layer_norm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3590 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/lightconv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4230 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/lightconv2d.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1654 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/modules/mask.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4800 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/multi_layer_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16630 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/nets_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1936 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/positionwise_feed_forward.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      703 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/repeat.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/rnn/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/rnn/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4080 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/rnn/argument.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    66987 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/rnn/attentions.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    49387 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/rnn/decoders.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14180 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/rnn/encoders.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/scorers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/scorers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5026 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/scorers/ctc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13951 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/scorers/ctc_prefix_score.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1787 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/scorers/length_bonus.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5938 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/scorers/scorer_interface.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/modules/streaming_utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/streaming_utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    17400 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/streaming_utils/chunk_utilis.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1809 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/streaming_utils/load_fr_tf.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2399 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/streaming_utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14104 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/subsampling.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1898 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/modules/subsampling_without_posenc.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/optimizers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/optimizers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5643 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/optimizers/fairseq_adam.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/optimizers/sgd.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/punctuation/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/punctuation/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      887 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/punctuation/abs_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6543 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/punctuation/espnet_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    22665 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/punctuation/sanm_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4492 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/punctuation/target_delay_transformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      444 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/punctuation/text_preprocessor.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4490 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/punctuation/vad_realtime_transformer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/runtime/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/runtime/python/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/libtorch/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/runtime/python/libtorch/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      363 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/demo.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7736 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5123 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5063 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1433 2023-03-24 05:23:58.000000 funasr-0.3.1/funasr/runtime/python/libtorch/setup.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1092 2023-03-13 09:20:09.000000 funasr-0.3.1/funasr/runtime/python/libtorch/test_rtf.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      902 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/demo.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7685 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8795 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-27 05:06:50.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/infer_onnx.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-03-24 05:11:50.000000 funasr-0.3.1/funasr/runtime/python/onnxruntime/setup.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/samplers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      425 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/abs_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6231 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/build_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5716 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/folded_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5168 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/length_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5680 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/num_elements_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3144 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/sorted_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2940 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/samplers/unsorted_batch_sampler.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/schedulers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/schedulers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1679 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/schedulers/abs_scheduler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2067 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/schedulers/noam_lr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3658 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/schedulers/tri_stage_scheduler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1494 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/schedulers/warmup_lr.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/tasks/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/tasks/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    73384 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/tasks/abs_task.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    48161 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/tasks/asr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12089 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/tasks/data2vec.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    32195 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/tasks/diar.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6809 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/tasks/lm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8078 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/tasks/punctuation.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18764 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/tasks/sv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11665 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/tasks/vad.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/text/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      347 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/abs_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2205 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/build_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2230 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/char_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1479 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/cleaner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1968 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/korean_cleaner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16601 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/phoneme_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1294 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/sentencepiece_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2100 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/token_id_converter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2074 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/text/word_tokenizer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/torch_utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      987 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/add_gradient_noise.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2681 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/device_funcs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1052 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/forward_adaptor.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3788 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/initialize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3815 2023-03-16 11:52:44.000000 funasr-0.3.1/funasr/torch_utils/load_pretrained_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2498 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/model_summary.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      468 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/pytorch_version.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1615 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/recursive_op.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      167 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/torch_utils/set_all_random_seed.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/train/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/train/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1764 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/train/abs_espnet_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3017 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/train/class_choices.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14493 2023-03-09 02:53:43.000000 funasr-0.3.1/funasr/train/distributed_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18344 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/train/reporter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    35859 2023-03-24 03:38:09.000000 funasr-0.3.1/funasr/train/trainer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2664 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/asr_env_checking.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11612 2023-03-17 12:37:43.000000 funasr-0.3.1/funasr/utils/asr_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      582 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/build_dataclass.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1380 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/cli_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2078 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/compute_eer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/compute_min_dcf.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5123 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/compute_wer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1760 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/config_argparse.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1830 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/get_default_kwargs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5632 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/griffin_lim.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4001 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/job_runner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1607 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/misc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1357 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/modelscope_param.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3598 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/nested_dict_action.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7766 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2027 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/sized_dict.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13178 2023-03-22 05:51:29.000000 funasr-0.3.1/funasr/utils/timestamp_tools.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4185 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/types.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11759 2023-03-16 11:52:36.000000 funasr-0.3.1/funasr/utils/wav_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      380 2023-02-24 12:39:00.000000 funasr-0.3.1/funasr/utils/yaml_no_alias_safe_dump.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        6 2023-03-24 03:40:16.000000 funasr-0.3.1/funasr/version.txt
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6390 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12962 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      857 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        7 2023-03-24 05:27:56.000000 funasr-0.3.1/funasr.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-03-24 05:27:56.000000 funasr-0.3.1/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4562 2023-03-16 11:52:44.000000 funasr-0.3.1/setup.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/test/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1773 2023-03-13 12:16:53.000000 funasr-0.3.1/test/test_rtf.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:27:56.000000 funasr-0.3.1/tests/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    25140 2023-03-17 12:37:43.000000 funasr-0.3.1/tests/test_asr_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1210 2023-03-16 11:52:36.000000 funasr-0.3.1/tests/test_asr_vad_punc_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2083 2023-03-09 02:53:43.000000 funasr-0.3.1/tests/test_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      804 2023-03-16 11:52:36.000000 funasr-0.3.1/tests/test_lm_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2118 2023-03-16 11:52:36.000000 funasr-0.3.1/tests/test_punctuation_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1949 2023-03-17 07:00:20.000000 funasr-0.3.1/tests/test_sv_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1250 2023-03-16 11:52:36.000000 funasr-0.3.1/tests/test_vad_inference_pipeline.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1063 2023-02-24 12:39:00.000000 funasr-0.4.1/LICENSE
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6614 2023-04-14 15:33:48.000000 funasr-0.4.1/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5601 2023-04-14 15:32:13.000000 funasr-0.4.1/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      203 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/bin/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/__init__.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3798 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/aggregate_stats_dirs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    21262 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/asr_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9781 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/asr_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    25900 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/bin/asr_inference_mfcca.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    37621 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    33372 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    19177 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    32909 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    34244 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_rnnt.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23884 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/bin/asr_inference_uniasr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23931 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_uniasr_vad.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1006 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1027 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train_paraformer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1024 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train_uniasr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5309 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/bin/build_trainer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1012 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/data2vec_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5365 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/diar_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1010 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/bin/diar_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14072 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/eend_ola_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     6814 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_calc_perplexity.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14615 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3989 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/lm_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1019 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3049 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/modelscope_infer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3767 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/punc_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/bin/punc_train.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12002 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/bin/punctuation_infer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11193 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/punctuation_infer_vadrealtime.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    20635 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/sond_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14771 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/sv_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     4756 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/sv_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     8449 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/tokenize_text.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12520 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/bin/tp_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4048 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/tp_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12389 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/bin/vad_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4275 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/vad_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11682 2023-04-06 02:32:27.000000 funasr-0.4.1/funasr/bin/vad_inference_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4338 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/collate_fn.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15174 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15562 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/datasets/iterable_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12671 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/iterable_dataset_modelscope.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3488 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/datasets/large_datasets/build_dataloader.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8298 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      519 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      453 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/map.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8055 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/datasets/large_datasets/dataset.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1382 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/clipping.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1013 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/filter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      948 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1201 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/padding.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2037 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1281 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/ms_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    30767 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/preprocessor.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10833 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/export_model.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5091 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/export/models/CT_Transformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1540 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/export/models/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/decoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/decoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6326 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/decoder/sanm_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5470 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/export/models/decoder/transformer_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8441 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/export/models/e2e_asr_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2047 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/models/e2e_vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/encoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/encoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3881 2023-03-15 12:41:42.000000 funasr-0.4.1/funasr/export/models/encoder/conformer_encoder.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9141 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/models/encoder/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7524 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/encoder/sanm_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/modules/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/modules/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1931 2023-03-15 12:41:42.000000 funasr-0.4.1/funasr/export/models/modules/decoder_layer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2354 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/export/models/modules/encoder_layer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/modules/feedforward.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8644 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/modules/multihead_att.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/predictor/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/predictor/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9917 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/predictor/cif.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/test/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      785 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      702 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      966 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1046 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      477 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_torchscripts.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/torch_quant/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      642 2023-03-10 03:02:25.000000 funasr-0.4.1/funasr/export/torch_quant/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2385 2023-03-16 11:05:28.000000 funasr-0.4.1/funasr/export/torch_quant/amp_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18267 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/graph.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7297 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2063 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/observed_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    30293 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/observer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10070 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/quantizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      620 2023-03-10 03:02:25.000000 funasr-0.4.1/funasr/export/torch_quant/version.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2620 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/utils/torch_function.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/fileio/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2383 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/datadir_writer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2357 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/npy_scp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2361 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/rand_gen_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2273 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/read_text.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3479 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/fileio/sound_scp.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/iterators/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      234 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/abs_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7808 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/chunk_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1140 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/multiple_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5236 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/sequence_iter_factory.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/layers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      359 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/abs_normalize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6717 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/complex_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3503 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/global_mvn.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      349 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/inversible_interface.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2539 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/layers/label_aggregation.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2564 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/log_mel.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10488 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/mask_along_axis.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9033 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/sinc_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8436 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/stft.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2513 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/time_warp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2309 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/utterance_mvn.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/lm/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5436 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/lm/abs_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5904 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/seq_rnn_lm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4243 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/transformer_lm.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/losses/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/losses/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2804 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/losses/label_smoothing_loss.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/main_funcs/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4687 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/main_funcs/average_nbest_models.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5610 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/calculate_all_attentions.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5029 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/collect_stats.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9906 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/main_funcs/pack_funcs.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6541 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/ctc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5298 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/data2vec.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/decoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      473 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/abs_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    40834 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/contextual_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12133 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/rnn_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    75199 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/sanm_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1389 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/sv_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28528 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/transformer_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    16707 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/e2e_asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/e2e_asr_common.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11630 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/models/e2e_asr_mfcca.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    67325 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_asr_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10238 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/models/e2e_diar_eend_ola.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20581 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/e2e_diar_sond.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10098 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/e2e_sv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6710 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_tp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    51737 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_uni_asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    31090 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/encoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      503 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/abs_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23724 2023-02-24 16:26:34.000000 funasr-0.4.1/funasr/models/encoder/conformer_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20993 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/data2vec_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    19855 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10164 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9281 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/models/encoder/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    17514 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/mfcca_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      909 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11046 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13971 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    21170 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    41077 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/encoder/resnet34_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3634 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/rnn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    53220 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/sanm_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    26890 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/transformer_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/frontend/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      400 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/abs_frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8895 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/default.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1405 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/models/frontend/eend_ola_feature.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5759 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/fused.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4990 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/s3prl.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20552 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/models/frontend/wav_frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6322 2023-02-24 16:26:34.000000 funasr-0.4.1/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2817 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/windowing.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/pooling/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/pooling/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3546 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/models/pooling/statistic_pooling.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/postencoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      403 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/abs_postencoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3626 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/predictor/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/predictor/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    34651 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/predictor/cif.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/preencoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      402 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/abs_preencoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1042 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/linear.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10296 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/sinc.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/specaug/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      426 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/abs_specaug.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6607 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/specaug.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4661 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/target_delay_transformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4715 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/vad_realtime_transformer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      940 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/add_sos_eos.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28945 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/modules/attention.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/beam_search/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13305 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/batch_beam_search.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10175 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    53592 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/beam_search.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/data2vec/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5831 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/data_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4474 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/ema_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      442 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/grad_multiply.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    26458 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/multihead_attention.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4021 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/quant_noise.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4858 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12734 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/wav2vec2.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4244 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/dynamic_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4863 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/dynamic_conv2d.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/e2e_asr_common.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/eend_ola/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/modules/eend_ola/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5287 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/modules/eend_ola/encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2768 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14578 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/modules/embedding.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/frontends/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2731 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/beamformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5540 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/dnn_beamformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2825 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/dnn_wpe.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7958 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/feature_transform.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4585 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2648 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/mask_estimator.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      958 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/layer_norm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3590 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/lightconv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4230 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/lightconv2d.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1654 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/modules/mask.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4800 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/multi_layer_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    16630 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/nets_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1936 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/positionwise_feed_forward.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      703 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/repeat.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/rnn/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4080 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/argument.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    66987 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/attentions.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    49387 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/decoders.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14180 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/encoders.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/scorers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5026 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/ctc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13951 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/ctc_prefix_score.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1787 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/length_bonus.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5938 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/scorer_interface.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/streaming_utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    17409 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1809 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2399 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14104 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/subsampling.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1898 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/subsampling_without_posenc.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/optimizers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5643 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/fairseq_adam.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/sgd.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/python/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/runtime/python/libtorch/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      544 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/runtime/python/libtorch/demo.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      752 2023-04-06 02:53:05.000000 funasr-0.4.1/funasr/runtime/python/libtorch/demo_gpu.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8172 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5123 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4845 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1433 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/runtime/python/libtorch/setup.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      845 2023-04-06 02:55:18.000000 funasr-0.4.1/funasr/runtime/python/libtorch/test_rtf.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      617 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      751 2023-04-06 02:45:07.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_gpu.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      740 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      932 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      383 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      969 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-27 05:06:50.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/infer_onnx.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/setup.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      451 2023-03-29 03:37:22.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/test_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1473 2023-03-29 05:24:31.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/test_pipeline_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/samplers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      425 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/abs_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6231 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/build_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5716 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/folded_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5168 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/length_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5680 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/num_elements_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3144 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/sorted_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2940 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/unsorted_batch_sampler.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/schedulers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1679 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/abs_scheduler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2067 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/noam_lr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3658 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/tri_stage_scheduler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1494 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/warmup_lr.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/tasks/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/tasks/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    73893 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/tasks/abs_task.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    47984 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/tasks/asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12089 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/tasks/data2vec.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    32463 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/tasks/diar.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6782 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/tasks/lm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8029 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/tasks/punctuation.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18814 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/tasks/sv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12527 2023-04-07 14:32:06.000000 funasr-0.4.1/funasr/tasks/vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/text/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      347 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/abs_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2205 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/build_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2230 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/char_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1479 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/cleaner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1968 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/korean_cleaner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    16601 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/phoneme_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1294 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/sentencepiece_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2100 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/token_id_converter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2074 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/word_tokenizer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/torch_utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      987 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/add_gradient_noise.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2681 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/device_funcs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1052 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/forward_adaptor.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3788 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/initialize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3815 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/torch_utils/load_pretrained_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2498 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/model_summary.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      468 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/pytorch_version.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1615 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/recursive_op.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      167 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/set_all_random_seed.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/train/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1764 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/abs_espnet_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7280 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/train/abs_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3017 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/class_choices.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14493 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/train/distributed_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18344 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/reporter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    35996 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/train/trainer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2664 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/asr_env_checking.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11612 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/utils/asr_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      582 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/build_dataclass.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1380 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/cli_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2078 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/compute_eer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/compute_min_dcf.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5189 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/utils/compute_wer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1760 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/config_argparse.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1830 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/get_default_kwargs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5632 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/griffin_lim.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4001 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/job_runner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1607 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/misc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1357 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/modelscope_param.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3598 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/nested_dict_action.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7735 2023-04-06 02:32:27.000000 funasr-0.4.1/funasr/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2027 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/sized_dict.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13178 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/utils/timestamp_tools.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4185 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/types.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11759 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/utils/wav_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      380 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        6 2023-04-14 15:32:13.000000 funasr-0.4.1/funasr/version.txt
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6614 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13807 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      857 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        7 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:33:48.000000 funasr-0.4.1/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4562 2023-04-06 02:32:27.000000 funasr-0.4.1/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/test/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      494 2023-03-31 07:25:30.000000 funasr-0.4.1/test/test_moddelscope_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1028 2023-03-31 07:26:37.000000 funasr-0.4.1/test/test_moddelscope_punc_online.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      537 2023-03-31 14:17:23.000000 funasr-0.4.1/test/test_modelscope_paraformer_long.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      809 2023-04-14 02:06:28.000000 funasr-0.4.1/test/test_modelscope_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1399 2023-03-31 14:15:12.000000 funasr-0.4.1/test/test_modelscope_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2514 2023-04-13 11:54:40.000000 funasr-0.4.1/test/test_onnx_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1773 2023-03-13 12:16:53.000000 funasr-0.4.1/test/test_rtf.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/tests/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    25268 2023-04-14 02:00:09.000000 funasr-0.4.1/tests/test_asr_inference_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1210 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2083 2023-03-09 02:53:43.000000 funasr-0.4.1/tests/test_inference_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      804 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_lm_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2055 2023-04-14 02:00:09.000000 funasr-0.4.1/tests/test_punctuation_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1949 2023-03-17 07:00:20.000000 funasr-0.4.1/tests/test_sv_inference_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1250 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.3.1/LICENSE` & `funasr-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/PKG-INFO` & `funasr-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.3.1
+Version: 0.4.1
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,20 +30,19 @@
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Docs_CN**](https://alibaba-damo-academy.github.io/FunASR/cn/index.html)
 | [**Docs_EN**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
 
 
 ## What's new: 
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
@@ -52,19 +51,34 @@
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
+Install from pip
+```shell
+pip install -U funasr -i https://pypi.Python.org/simple
+```
+
+Or install from source code
+
+
 ``` sh
-pip install "modelscope[audio_asr]" --upgrade -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html
 git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install --editable ./
+pip install -e ./
 ```
+If you want to use the pretrained models in ModelScope, you should install the modelscope:
+
+```shell
+pip install -U modelscope
+# For the users in China, you could install with the command:
+# pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
+```
+
 For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
 
 ## Usage
 For users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-academy.github.io/FunASR/en/index.html))
 
 ## Contact
```

### Comparing `funasr-0.3.1/README.md` & `funasr-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Docs_CN**](https://alibaba-damo-academy.github.io/FunASR/cn/index.html)
 | [**Docs_EN**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
 
 
 ## What's new: 
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
@@ -25,19 +24,34 @@
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
+Install from pip
+```shell
+pip install -U funasr -i https://pypi.Python.org/simple
+```
+
+Or install from source code
+
+
 ``` sh
-pip install "modelscope[audio_asr]" --upgrade -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html
 git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install --editable ./
+pip install -e ./
 ```
+If you want to use the pretrained models in ModelScope, you should install the modelscope:
+
+```shell
+pip install -U modelscope
+# For the users in China, you could install with the command:
+# pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
+```
+
 For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
 
 ## Usage
 For users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-academy.github.io/FunASR/en/index.html))
 
 ## Contact
```

### Comparing `funasr-0.3.1/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.4.1/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/asr_inference.py` & `funasr-0.4.1/funasr/bin/asr_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_launch.py` & `funasr-0.4.1/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_mfcca.py` & `funasr-0.4.1/funasr/bin/asr_inference_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_paraformer.py` & `funasr-0.4.1/funasr/bin/asr_inference_paraformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,15 +793,15 @@
                         item = {'key': key, 'value': text_postprocessed}
                         if timestamp_postprocessed != "":
                             item['timestamp'] = timestamp_postprocessed
                         asr_result_list.append(item)
                         finish_count += 1
                         # asr_utils.print_progress(finish_count / file_count)
                         if writer is not None:
-                            ibest_writer["text"][key] = text_postprocessed
+                            ibest_writer["text"][key] = " ".join(word_lists)
 
                     logging.info("decoding, utt: {}, predictions: {}".format(key, text))
         rtf_avg = "decoding, feature length total: {}, forward_time total: {:.4f}, rtf avg: {:.4f}".format(length_total, forward_time_total, 100 * forward_time_total / (length_total * lfr_factor))
         logging.info(rtf_avg)
         if writer is not None:
             ibest_writer["rtf"]["rtf_avf"] = rtf_avg
         return asr_result_list
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.4.1/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Union
 from typing import Dict
 from typing import Any
 from typing import List
 
 import numpy as np
 import torch
+import torchaudio
 from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
@@ -38,14 +39,15 @@
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
 from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
+np.set_printoptions(threshold=np.inf)
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
             >>> speech2text = Speech2Text("asr_config.yml", "asr.pth")
@@ -199,31 +201,33 @@
 
         """
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
-
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             self.asr_model.frontend = None
         else:
             feats = speech
             feats_len = speech_lengths
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
+        feats_len = cache["encoder"]["stride"] + cache["encoder"]["pad_left"] + cache["encoder"]["pad_right"]
+        feats = feats[:,cache["encoder"]["start_idx"]:cache["encoder"]["start_idx"]+feats_len,:]
+        feats_len = torch.tensor([feats_len])
         batch = {"speech": feats, "speech_lengths": feats_len, "cache": cache}
 
         # a. To device
         batch = to_device(batch, device=self.device)
 
         # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode_chunk(**batch)
+        enc, enc_len = self.asr_model.encode_chunk(feats, feats_len, cache)
         if isinstance(enc, tuple):
             enc = enc[0]
         # assert len(enc) == 1, len(enc)
         enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
 
         predictor_outs = self.asr_model.calc_predictor_chunk(enc, cache)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
@@ -574,97 +578,143 @@
         penalty=penalty,
         nbest=nbest,
     )
     if export_mode:
         speech2text = Speech2TextExport(**speech2text_kwargs)
     else:
         speech2text = Speech2Text(**speech2text_kwargs)
-
+        
+    def _load_bytes(input):
+        middle_data = np.frombuffer(input, dtype=np.int16)
+        middle_data = np.asarray(middle_data)
+        if middle_data.dtype.kind not in 'iu':
+            raise TypeError("'middle_data' must be an array of integers")
+        dtype = np.dtype('float32')
+        if dtype.kind != 'f':
+            raise TypeError("'dtype' must be a floating point type")
+
+        i = np.iinfo(middle_data.dtype)
+        abs_max = 2 ** (i.bits - 1)
+        offset = i.min + abs_max
+        array = np.frombuffer((middle_data.astype(dtype) - offset) / abs_max, dtype=np.float32)
+        return array
+    
     def _forward(
             data_path_and_name_and_type,
             raw_inputs: Union[np.ndarray, torch.Tensor] = None,
             output_dir_v2: Optional[str] = None,
             fs: dict = None,
             param_dict: dict = None,
             **kwargs,
     ):
 
         # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, np.ndarray):
-                raw_inputs = torch.tensor(raw_inputs)
-
         is_final = False
         if param_dict is not None and "cache" in param_dict:
             cache = param_dict["cache"]
         if param_dict is not None and "is_final" in param_dict:
             is_final = param_dict["is_final"]
+
+        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
+            raw_inputs = _load_bytes(data_path_and_name_and_type[0])
+            raw_inputs = torch.tensor(raw_inputs)
+        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
+            raw_inputs = torchaudio.load(data_path_and_name_and_type[0])[0][0]
+            is_final = True
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, np.ndarray):
+                raw_inputs = torch.tensor(raw_inputs)
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         results = []
         asr_result = ""
         wait = True
         if len(cache) == 0:
-            cache["encoder"] = {"start_idx": 0, "pad_left": 0, "stride": 10, "pad_right": 5, "cif_hidden": None, "cif_alphas": None}
+            cache["encoder"] = {"start_idx": 0, "pad_left": 0, "stride": 10, "pad_right": 5, "cif_hidden": None, "cif_alphas": None, "is_final": is_final, "left": 0, "right": 0}
             cache_de = {"decode_fsmn": None}
             cache["decoder"] = cache_de
             cache["first_chunk"] = True
             cache["speech"] = []
-            cache["chunk_index"] = 0
-            cache["speech_chunk"] = []
+            cache["accum_speech"] = 0
 
         if raw_inputs is not None:
             if len(cache["speech"]) == 0:
                 cache["speech"] = raw_inputs
             else:
                 cache["speech"] = torch.cat([cache["speech"], raw_inputs], dim=0)
-            if len(cache["speech_chunk"]) == 0:
-                cache["speech_chunk"] = raw_inputs
-            else:
-                cache["speech_chunk"] = torch.cat([cache["speech_chunk"], raw_inputs], dim=0)
-            while len(cache["speech_chunk"]) >= 960:
+            cache["accum_speech"] += len(raw_inputs)
+            while cache["accum_speech"] >= 960:
                 if cache["first_chunk"]:
-                    if len(cache["speech_chunk"]) >= 14400:
-                        speech = torch.unsqueeze(cache["speech_chunk"][0:14400], axis=0)
-                        speech_length = torch.tensor([14400])
+                    if cache["accum_speech"] >= 14400:
+                        speech = torch.unsqueeze(cache["speech"], axis=0)
+                        speech_length = torch.tensor([len(cache["speech"])])
+                        cache["encoder"]["pad_left"] = 5 
+                        cache["encoder"]["pad_right"] = 5 
+                        cache["encoder"]["stride"] = 10
+                        cache["encoder"]["left"] = 5
+                        cache["encoder"]["right"] = 0
                         results = speech2text(cache, speech, speech_length)
-                        cache["speech_chunk"]= cache["speech_chunk"][4800:]
+                        cache["accum_speech"] -= 4800
                         cache["first_chunk"] = False
                         cache["encoder"]["start_idx"] = -5
+                        cache["encoder"]["is_final"] = False
                         wait = False
                     else:
                         if is_final:
-                            cache["encoder"]["stride"] = len(cache["speech_chunk"]) // 960
+                            cache["encoder"]["stride"] = len(cache["speech"]) // 960
+                            cache["encoder"]["pad_left"] = 0
                             cache["encoder"]["pad_right"] = 0
-                            speech = torch.unsqueeze(cache["speech_chunk"], axis=0)
-                            speech_length = torch.tensor([len(cache["speech_chunk"])])
+                            speech = torch.unsqueeze(cache["speech"], axis=0)
+                            speech_length = torch.tensor([len(cache["speech"])])
                             results = speech2text(cache, speech, speech_length)
-                            cache["speech_chunk"] = []
+                            cache["accum_speech"] = 0
                             wait = False
                         else:
                             break
                 else:
-                    if len(cache["speech_chunk"]) >= 19200:
+                    if cache["accum_speech"] >= 19200:
                         cache["encoder"]["start_idx"] += 10
+                        cache["encoder"]["stride"] = 10
                         cache["encoder"]["pad_left"] = 5
-                        speech = torch.unsqueeze(cache["speech_chunk"][:19200], axis=0)
-                        speech_length = torch.tensor([19200])
+                        cache["encoder"]["pad_right"] = 5
+                        cache["encoder"]["left"] = 0
+                        cache["encoder"]["right"] = 0
+                        speech = torch.unsqueeze(cache["speech"], axis=0)
+                        speech_length = torch.tensor([len(cache["speech"])])
                         results = speech2text(cache, speech, speech_length)
-                        cache["speech_chunk"] = cache["speech_chunk"][9600:]
+                        cache["accum_speech"] -= 9600
                         wait = False
                     else:
                         if is_final:
-                            cache["encoder"]["stride"] = len(cache["speech_chunk"]) // 960
-                            cache["encoder"]["pad_right"] = 0
-                            speech = torch.unsqueeze(cache["speech_chunk"], axis=0)
-                            speech_length = torch.tensor([len(cache["speech_chunk"])])
-                            results = speech2text(cache, speech, speech_length)
-                            cache["speech_chunk"] = []
-                            wait = False
+                            cache["encoder"]["is_final"] = True
+                            if cache["accum_speech"] >= 14400:
+                                cache["encoder"]["start_idx"] += 10
+                                cache["encoder"]["stride"] = 10
+                                cache["encoder"]["pad_left"] = 5
+                                cache["encoder"]["pad_right"] = 5
+                                cache["encoder"]["left"] = 0
+                                cache["encoder"]["right"] = cache["accum_speech"] // 960 - 15
+                                speech = torch.unsqueeze(cache["speech"], axis=0)
+                                speech_length = torch.tensor([len(cache["speech"])])
+                                results = speech2text(cache, speech, speech_length)
+                                cache["accum_speech"] -= 9600
+                                wait = False
+                            else:
+                                cache["encoder"]["start_idx"] += 10
+                                cache["encoder"]["stride"] = cache["accum_speech"] // 960 - 5
+                                cache["encoder"]["pad_left"] = 5
+                                cache["encoder"]["pad_right"] = 0
+                                cache["encoder"]["left"] = 0
+                                cache["encoder"]["right"] = 0
+                                speech = torch.unsqueeze(cache["speech"], axis=0)
+                                speech_length = torch.tensor([len(cache["speech"])])
+                                results = speech2text(cache, speech, speech_length)
+                                cache["accum_speech"] = 0
+                                wait = False
                         else:
                             break
                 
                 if len(results) >= 1:
                     asr_result += results[0][0]
             if asr_result == "":
                 asr_result = "sil"
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_paraformer_vad.py` & `funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
                 finish_count += 1
                 # asr_utils.print_progress(finish_count / file_count)
                 if writer is not None:
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["vad"][key] = "{}".format(vadsegments)
-                    ibest_writer["text"][key] = text_postprocessed
+                    ibest_writer["text"][key] = " ".join(word_lists)
                     ibest_writer["text_with_punc"][key] = text_postprocessed_punc
                     if time_stamp_postprocessed is not None:
                         ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
                 
                 logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_paraformer_vad_punc.py` & `funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad_punc.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
                 finish_count += 1
                 # asr_utils.print_progress(finish_count / file_count)
                 if writer is not None:
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["vad"][key] = "{}".format(vadsegments)
-                    ibest_writer["text"][key] = text_postprocessed
+                    ibest_writer["text"][key] = " ".join(word_lists)
                     ibest_writer["text_with_punc"][key] = text_postprocessed_punc
                     if time_stamp_postprocessed is not None:
                         ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
 
                 logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
         return asr_result_list
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_rnnt.py` & `funasr-0.4.1/funasr/bin/asr_inference_rnnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,21 +734,21 @@
                         # Write the result to each file
                         ibest_writer["token"][key] = " ".join(token)
                         # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                         ibest_writer["score"][key] = str(hyp.score)
                         ibest_writer["rtf"][key] = rtf_cur
 
                     if text is not None:
-                        text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
+                        text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
                         item = {'key': key, 'value': text_postprocessed}
                         asr_result_list.append(item)
                         finish_count += 1
                         # asr_utils.print_progress(finish_count / file_count)
                         if writer is not None:
-                            ibest_writer["text"][key] = text_postprocessed
+                            ibest_writer["text"][key] = " ".join(word_lists)
 
                     logging.info("decoding, utt: {}, predictions: {}".format(key, text))
         rtf_avg = "decoding, feature length total: {}, forward_time total: {:.4f}, rtf avg: {:.4f}".format(length_total, forward_time_total, 100 * forward_time_total / (length_total * lfr_factor))
         logging.info(rtf_avg)
         if writer is not None:
             ibest_writer["rtf"]["rtf_avf"] = rtf_avg
         return asr_result_list
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_uniasr.py` & `funasr-0.4.1/funasr/bin/asr_inference_uniasr_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     if param_dict is not None and "decoding_model" in param_dict:
         if param_dict["decoding_model"] == "fast":
             decoding_ind = 0
             decoding_mode = "model1"
         elif param_dict["decoding_model"] == "normal":
             decoding_ind = 0
             decoding_mode = "model2"
@@ -503,21 +503,21 @@
     
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
     
                 if text is not None:
-                    text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
+                    text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
-                        ibest_writer["text"][key] = text_postprocessed
+                        ibest_writer["text"][key] = " ".join(word_lists)
         return asr_result_list
     
     return _forward
 
 
 
 def get_parser():
```

### Comparing `funasr-0.3.1/funasr/bin/asr_inference_uniasr_vad.py` & `funasr-0.4.1/funasr/bin/asr_inference_uniasr.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,14 @@
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
 
 
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
@@ -394,15 +391,15 @@
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-
+    
     if param_dict is not None and "decoding_model" in param_dict:
         if param_dict["decoding_model"] == "fast":
             decoding_ind = 0
             decoding_mode = "model1"
         elif param_dict["decoding_model"] == "normal":
             decoding_ind = 0
             decoding_mode = "model2"
@@ -503,21 +500,21 @@
     
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
     
                 if text is not None:
-                    text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
+                    text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
-                        ibest_writer["text"][key] = text_postprocessed
+                        ibest_writer["text"][key] = " ".join(word_lists)
         return asr_result_list
     
     return _forward
 
 
 
 def get_parser():
```

### Comparing `funasr-0.3.1/funasr/bin/asr_train.py` & `funasr-0.4.1/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/asr_train_paraformer.py` & `funasr-0.4.1/funasr/bin/asr_train_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/asr_train_uniasr.py` & `funasr-0.4.1/funasr/bin/asr_train_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/build_trainer.py` & `funasr-0.4.1/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/data2vec_train.py` & `funasr-0.4.1/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/diar_inference_launch.py` & `funasr-0.4.1/funasr/bin/diar_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/diar_train.py` & `funasr-0.4.1/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/eend_ola_inference.py` & `funasr-0.4.1/funasr/bin/eend_ola_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/lm_calc_perplexity.py` & `funasr-0.4.1/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/lm_inference.py` & `funasr-0.4.1/funasr/bin/lm_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/lm_inference_launch.py` & `funasr-0.4.1/funasr/bin/lm_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/lm_train.py` & `funasr-0.4.1/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/modelscope_infer.py` & `funasr-0.4.1/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/punc_inference_launch.py` & `funasr-0.4.1/funasr/bin/punc_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/punc_train.py` & `funasr-0.4.1/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/punctuation_infer.py` & `funasr-0.4.1/funasr/bin/punctuation_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from funasr.tasks.punctuation import PunctuationTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.punctuation.text_preprocessor import split_to_mini_sentence
+from funasr.datasets.preprocessor import split_to_mini_sentence
 
 
 class Text2Punc:
 
     def __init__(
         self,
         train_config: Optional[str],
```

### Comparing `funasr-0.3.1/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.4.1/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from funasr.tasks.punctuation import PunctuationTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.punctuation.text_preprocessor import split_to_mini_sentence
+from funasr.datasets.preprocessor import split_to_mini_sentence
 
 
 class Text2Punc:
 
     def __init__(
         self,
         train_config: Optional[str],
@@ -86,15 +86,15 @@
             mini_sentence = mini_sentences[mini_sentence_i]
             mini_sentence_id = mini_sentences_id[mini_sentence_i]
             mini_sentence = cache_sent + mini_sentence
             mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0)
             data = {
                 "text": torch.unsqueeze(torch.from_numpy(mini_sentence_id), 0),
                 "text_lengths": torch.from_numpy(np.array([len(mini_sentence_id)], dtype='int32')),
-                "vad_indexes": torch.from_numpy(np.array([len(cache)-1], dtype='int32')),
+                "vad_indexes": torch.from_numpy(np.array([len(cache)], dtype='int32')),
             }
             data = to_device(data, self.device)
             y, _ = self.wrapped_model(**data)
             _, indices = y.view(-1, y.shape[-1]).topk(1, dim=1)
             punctuations = indices
             if indices.size()[0] != 1:
                 punctuations = torch.squeeze(indices)
```

### Comparing `funasr-0.3.1/funasr/bin/sond_inference.py` & `funasr-0.4.1/funasr/bin/sond_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/sv_inference.py` & `funasr-0.4.1/funasr/bin/sv_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/sv_inference_launch.py` & `funasr-0.4.1/funasr/bin/sv_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/tokenize_text.py` & `funasr-0.4.1/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/tp_inference.py` & `funasr-0.4.1/funasr/bin/tp_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/tp_inference_launch.py` & `funasr-0.4.1/funasr/bin/tp_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/vad_inference.py` & `funasr-0.4.1/funasr/bin/vad_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/bin/vad_inference_launch.py` & `funasr-0.4.1/funasr/bin/vad_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 # Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
```

### Comparing `funasr-0.3.1/funasr/bin/vad_inference_online.py` & `funasr-0.4.1/funasr/bin/vad_inference_online.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.models.frontend.wav_frontend import WavFrontendOnline
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.bin.vad_inference import Speech2VadSegment
 
-
+header_colors = '\033[95m'
+end_colors = '\033[0m'
 
 
 class Speech2VadSegmentOnline(Speech2VadSegment):
     """Speech2VadSegmentOnline class
 
     Examples:
         >>> import soundfile
@@ -51,15 +52,15 @@
         if self.vad_infer_args.frontend is not None:
             self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
 
 
     @torch.no_grad()
     def __call__(
             self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False
+            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
     ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
         """Inference
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
@@ -82,15 +83,16 @@
             feats_len = feats_len.int()
             waveforms = self.frontend.get_waveforms()
 
             batch = {
                 "feats": feats,
                 "waveform": waveforms,
                 "in_cache": in_cache,
-                "is_final": is_final
+                "is_final": is_final,
+                "max_end_sil": max_end_sil
             }
             # a. To device
             batch = to_device(batch, device=self.device)
             segments, in_cache = self.vad_model.forward_online(**batch)
             # in_cache.update(batch['in_cache'])
             # in_cache = {key: value for key, value in batch['in_cache'].items()}
         return fbanks, segments, in_cache
@@ -212,22 +214,24 @@
             ibest_writer = writer[f"1best_recog"]
         else:
             writer = None
             ibest_writer = None
 
         vad_results = []
         batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
-        is_final = param_dict['is_final'] if param_dict is not None else False
+        is_final = param_dict.get('is_final', False) if param_dict is not None else False
+        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             batch['in_cache'] = batch_in_cache
             batch['is_final'] = is_final
+            batch['max_end_sil'] = max_end_sil
 
             # do vad segment
             _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
             # param_dict['in_cache'] = batch['in_cache']
             if results:
                 for i, _ in enumerate(keys):
                     if results[i]:
```

### Comparing `funasr-0.3.1/funasr/datasets/collate_fn.py` & `funasr-0.4.1/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/dataset.py` & `funasr-0.4.1/funasr/datasets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # The file is as follows:
     #   utterance_id_A /some/where/a.wav
     #   utterance_id_B /some/where/a.flac
 
     # NOTE(kamo): SoundScpReader doesn't support pipe-fashion
     # like Kaldi e.g. "cat a.wav |".
     # NOTE(kamo): The audio signal is normalized to [-1,1] range.
-    loader = SoundScpReader(path, dest_sample_rate, normalize=True, always_2d=False)
+    loader = SoundScpReader(path, normalize=True, always_2d=False, dest_sample_rate = dest_sample_rate)
 
     # SoundScpReader.__getitem__() returns Tuple[int, ndarray],
     # but ndarray is desired, so Adapter class is inserted here
     return AdapterForSoundScpReader(loader, float_dtype)
 
 
 def kaldi_loader(path, float_dtype=None, max_cache_fd: int = 0):
```

### Comparing `funasr-0.3.1/funasr/datasets/iterable_dataset.py` & `funasr-0.4.1/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.4.1/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.4.1/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.4.1/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.4.1/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/dataset.py` & `funasr-0.4.1/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.4.1/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.4.1/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.4.1/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.4.1/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.4.1/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,26 +33,26 @@
     assert "text" in data
     assert isinstance(vocab, dict)
     text = data["text"]
     token = []
     vad = -2
 
     if bpe_tokenizer is not None:
-        text = bpe_tokenizer.text2tokens(text)
+        text = bpe_tokenizer.text2tokens("".join(text))
 
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         txt = forward_segment("".join(text).lower(), seg_dict)
         text = seg_tokenize(txt, seg_dict)
 
     length = len(text)
     for i in range(length):
         x = text[i]
-        if i == length-1 and "punc" in data and text[i].startswith("vad:"):
-            vad = x[-1][4:]
+        if i == length-1 and "punc" in data and x.startswith("vad:"):
+            vad = x[4:]
             if len(vad) == 0:
                 vad = -1
             else:
                 vad = int(vad)
         elif x in vocab:
             token.append(vocab[x])
         else:
```

### Comparing `funasr-0.3.1/funasr/datasets/ms_dataset.py` & `funasr-0.4.1/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/datasets/preprocessor.py` & `funasr-0.4.1/funasr/datasets/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,21 +782,36 @@
         self.vad_name = vad_name
 
     def _text_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         for i in range(self.num_tokenizer):
             text_name = self.text_name[i]
+            #import pdb; pdb.set_trace()
             if text_name in data and self.tokenizer[i] is not None:
                 text = data[text_name]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer[i].text2tokens(text)
                 if "vad:" in tokens[-1]:
                     vad = tokens[-1][4:]
                     tokens = tokens[:-1]
                     if len(vad) == 0:
                         vad = -1
                     else:
                         vad = int(vad)
                     data[self.vad_name] = np.array([vad], dtype=np.int64)
                 text_ints = self.token_id_converter[i].tokens2ids(tokens)
                 data[text_name] = np.array(text_ints, dtype=np.int64)
+        return data
+
+def split_to_mini_sentence(words: list, word_limit: int = 20):
+    assert word_limit > 1
+    if len(words) <= word_limit:
+        return [words]
+    sentences = []
+    length = len(words)
+    sentence_len = length // word_limit
+    for i in range(sentence_len):
+        sentences.append(words[i * word_limit:(i + 1) * word_limit])
+    if length % word_limit > 0:
+        sentences.append(words[sentence_len * word_limit:])
+    return sentences
```

### Comparing `funasr-0.3.1/funasr/export/export_model.py` & `funasr-0.4.1/funasr/export/export_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # assert torch_version > 1.9
 
 class ModelExport:
     def __init__(
         self,
         cache_dir: Union[Path, str] = None,
         onnx: bool = True,
+        device: str = "cpu",
         quant: bool = True,
         fallback_num: int = 0,
         audio_in: str = None,
         calib_num: int = 200,
     ):
         assert check_argument_types()
         self.set_all_random_seed(0)
@@ -32,14 +33,15 @@
         self.cache_dir = Path(cache_dir)
         self.export_config = dict(
             feats_dim=560,
             onnx=False,
         )
         print("output dir: {}".format(self.cache_dir))
         self.onnx = onnx
+        self.device = device
         self.quant = quant
         self.fallback_num = fallback_num
         self.frontend = None
         self.audio_in = audio_in
         self.calib_num = calib_num
         
 
@@ -108,14 +110,18 @@
 
     def _export_torchscripts(self, model, verbose, path, enc_size=None):
         if enc_size:
             dummy_input = model.get_dummy_inputs(enc_size)
         else:
             dummy_input = model.get_dummy_inputs()
 
+        if self.device == 'cuda':
+            model = model.cuda()
+            dummy_input = tuple([i.cuda() for i in dummy_input])
+
         # model_script = torch.jit.script(model)
         model_script = torch.jit.trace(model, dummy_input)
         model_script.save(os.path.join(path, f'{model.model_name}.torchscripts'))
 
         if self.quant:
             quant_model = self._torch_quantize(model)
             model_script = torch.jit.trace(quant_model, dummy_input)
@@ -157,39 +163,65 @@
             fbank, fbank_len = self.frontend(waveform, [waveform.size(1)])
             feats.append(fbank)
             feats_len.append(fbank_len)
         return feats, feats_len
     
     def export(self,
                tag_name: str = 'damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch',
-               mode: str = 'paraformer',
+               mode: str = None,
                ):
         
         model_dir = tag_name
-        if model_dir.startswith('damo/'):
+        if model_dir.startswith('damo'):
             from modelscope.hub.snapshot_download import snapshot_download
             model_dir = snapshot_download(model_dir, cache_dir=self.cache_dir)
-        asr_train_config = os.path.join(model_dir, 'config.yaml')
-        asr_model_file = os.path.join(model_dir, 'model.pb')
-        cmvn_file = os.path.join(model_dir, 'am.mvn')
-        json_file = os.path.join(model_dir, 'configuration.json')
+
         if mode is None:
             import json
+            json_file = os.path.join(model_dir, 'configuration.json')
             with open(json_file, 'r') as f:
                 config_data = json.load(f)
-                mode = config_data['model']['model_config']['mode']
+                if config_data['task'] == "punctuation":
+                    mode = config_data['model']['punc_model_config']['mode']
+                else:
+                    mode = config_data['model']['model_config']['mode']
         if mode.startswith('paraformer'):
             from funasr.tasks.asr import ASRTaskParaformer as ASRTask
-        elif mode.startswith('uniasr'):
-            from funasr.tasks.asr import ASRTaskUniASR as ASRTask
+            config = os.path.join(model_dir, 'config.yaml')
+            model_file = os.path.join(model_dir, 'model.pb')
+            cmvn_file = os.path.join(model_dir, 'am.mvn')
+            model, asr_train_args = ASRTask.build_model_from_file(
+                config, model_file, cmvn_file, 'cpu'
+            )
+            self.frontend = model.frontend
+        elif mode.startswith('offline'):
+            from funasr.tasks.vad import VADTask
+            config = os.path.join(model_dir, 'vad.yaml')
+            model_file = os.path.join(model_dir, 'vad.pb')
+            cmvn_file = os.path.join(model_dir, 'vad.mvn')
             
-        model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, 'cpu'
-        )
-        self.frontend = model.frontend
+            model, vad_infer_args = VADTask.build_model_from_file(
+                config, model_file, cmvn_file=cmvn_file, device='cpu'
+            )
+            self.export_config["feats_dim"] = 400
+            self.frontend = model.frontend
+        elif mode.startswith('punc'):
+            from funasr.tasks.punctuation import PunctuationTask as PUNCTask
+            punc_train_config = os.path.join(model_dir, 'config.yaml')
+            punc_model_file = os.path.join(model_dir, 'punc.pb')
+            model, punc_train_args = PUNCTask.build_model_from_file(
+                punc_train_config, punc_model_file, 'cpu'
+            )
+        elif mode.startswith('punc_VadRealtime'):
+            from funasr.tasks.punctuation import PunctuationTask as PUNCTask
+            punc_train_config = os.path.join(model_dir, 'config.yaml')
+            punc_model_file = os.path.join(model_dir, 'punc.pb')
+            model, punc_train_args = PUNCTask.build_model_from_file(
+                punc_train_config, punc_model_file, 'cpu'
+            )
         self._export(model, tag_name)
             
 
     def _export_onnx(self, model, verbose, path, enc_size=None):
         if enc_size:
             dummy_input = model.get_dummy_inputs(enc_size)
         else:
@@ -230,22 +262,24 @@
 
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument('--model-name', type=str, required=True)
     parser.add_argument('--export-dir', type=str, required=True)
     parser.add_argument('--type', type=str, default='onnx', help='["onnx", "torch"]')
+    parser.add_argument('--device', type=str, default='cpu', help='["cpu", "cuda"]')
     parser.add_argument('--quantize', type=str2bool, default=False, help='export quantized model')
     parser.add_argument('--fallback-num', type=int, default=0, help='amp fallback number')
     parser.add_argument('--audio_in', type=str, default=None, help='["wav", "wav.scp"]')
     parser.add_argument('--calib_num', type=int, default=200, help='calib max num')
     args = parser.parse_args()
 
     export_model = ModelExport(
         cache_dir=args.export_dir,
         onnx=args.type == 'onnx',
+        device=args.device,
         quant=args.quantize,
         fallback_num=args.fallback_num,
         audio_in=args.audio_in,
         calib_num=args.calib_num,
     )
     export_model.export(args.model_name)
```

### Comparing `funasr-0.3.1/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.4.1/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.4.1/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.4.1/funasr/export/models/e2e_asr_paraformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.export.models.decoder.sanm_decoder import ParaformerSANMDecoder as ParaformerSANMDecoder_export
 from funasr.export.models.decoder.transformer_decoder import ParaformerDecoderSAN as ParaformerDecoderSAN_export
 
 
 class Paraformer(nn.Module):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
     """
 
     def __init__(
             self,
             model,
@@ -108,15 +108,15 @@
                 1: 'logits_length'
             },
         }
 
 
 class BiCifParaformer(nn.Module):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
     """
 
     def __init__(
             self,
             model,
```

### Comparing `funasr-0.3.1/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.4.1/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/modules/decoder_layer.py` & `funasr-0.4.1/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/modules/encoder_layer.py` & `funasr-0.4.1/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/modules/feedforward.py` & `funasr-0.4.1/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/models/modules/multihead_att.py` & `funasr-0.4.1/funasr/export/models/modules/multihead_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
         x = pad_fn(x)
     else:
         x = torch.cat((cache[:, :, 1:], x), dim=2)
         cache = x
     return x, cache
 
 
-torch_version = float(".".join(torch.__version__.split(".")[:2]))
-if torch_version >= 1.8:
+torch_version = tuple([int(i) for i in torch.__version__.split(".")[:2]])
+if torch_version >= (1, 8):
     import torch.fx
     torch.fx.wrap('preprocess_for_attn')
 
 
 class MultiHeadedAttentionSANMDecoder(nn.Module):
     def __init__(self, model):
         super().__init__()
```

### Comparing `funasr-0.3.1/funasr/export/models/predictor/cif.py` & `funasr-0.4.1/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/test_onnx.py` & `funasr-0.4.1/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/__init__.py` & `funasr-0.4.1/funasr/export/torch_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/amp_module.py` & `funasr-0.4.1/funasr/export/torch_quant/amp_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/graph.py` & `funasr-0.4.1/funasr/export/torch_quant/graph.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/module.py` & `funasr-0.4.1/funasr/export/torch_quant/module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/observed_module.py` & `funasr-0.4.1/funasr/export/torch_quant/observed_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/observer.py` & `funasr-0.4.1/funasr/export/torch_quant/observer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/quantizer.py` & `funasr-0.4.1/funasr/export/torch_quant/quantizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/torch_quant/version.py` & `funasr-0.4.1/funasr/export/torch_quant/version.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/export/utils/torch_function.py` & `funasr-0.4.1/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/fileio/datadir_writer.py` & `funasr-0.4.1/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/fileio/npy_scp.py` & `funasr-0.4.1/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/fileio/rand_gen_dataset.py` & `funasr-0.4.1/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/fileio/read_text.py` & `funasr-0.4.1/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/fileio/sound_scp.py` & `funasr-0.4.1/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/iterators/chunk_iter_factory.py` & `funasr-0.4.1/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/iterators/multiple_iter_factory.py` & `funasr-0.4.1/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/iterators/sequence_iter_factory.py` & `funasr-0.4.1/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/complex_utils.py` & `funasr-0.4.1/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/global_mvn.py` & `funasr-0.4.1/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/label_aggregation.py` & `funasr-0.4.1/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/log_mel.py` & `funasr-0.4.1/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/mask_along_axis.py` & `funasr-0.4.1/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/sinc_conv.py` & `funasr-0.4.1/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/stft.py` & `funasr-0.4.1/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/time_warp.py` & `funasr-0.4.1/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/layers/utterance_mvn.py` & `funasr-0.4.1/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/lm/espnet_model.py` & `funasr-0.4.1/funasr/lm/abs_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,49 @@
+from abc import ABC
+from abc import abstractmethod
+from typing import Tuple
+
+import torch
+
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
 from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
-from funasr.lm.abs_model import AbsLM
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.train.abs_espnet_model import AbsESPnetModel
 
+class AbsLM(torch.nn.Module, BatchScorerInterface, ABC):
+    """The abstract LM class
+
+    To share the loss calculation way among different models,
+    We uses delegate pattern here:
+    The instance of this class should be passed to "LanguageModel"
+
+    >>> from funasr.lm.abs_model import AbsLM
+    >>> lm = AbsLM()
+    >>> model = LanguageESPnetModel(lm=lm)
+
+    This "model" is one of mediator objects for "Task" class.
+
+    """
+
+    @abstractmethod
+    def forward(
+        self, input: torch.Tensor, hidden: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        raise NotImplementedError
+
 
-class ESPnetLanguageModel(AbsESPnetModel):
+class LanguageModel(AbsESPnetModel):
     def __init__(self, lm: AbsLM, vocab_size: int, ignore_id: int = 0):
         assert check_argument_types()
         super().__init__()
         self.lm = lm
         self.sos = 1
         self.eos = 2
```

### Comparing `funasr-0.3.1/funasr/lm/seq_rnn_lm.py` & `funasr-0.4.1/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/lm/transformer_lm.py` & `funasr-0.4.1/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/losses/label_smoothing_loss.py` & `funasr-0.4.1/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/main_funcs/average_nbest_models.py` & `funasr-0.4.1/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.4.1/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/main_funcs/collect_stats.py` & `funasr-0.4.1/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/main_funcs/pack_funcs.py` & `funasr-0.4.1/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/ctc.py` & `funasr-0.4.1/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/data2vec.py` & `funasr-0.4.1/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/decoder/contextual_decoder.py` & `funasr-0.4.1/funasr/models/decoder/contextual_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,24 +70,24 @@
         x = self.src_attn(x, memory, memory_mask)
         x_src_attn = x
 
         x = residual + self.dropout(x)
         return x, tgt_mask, x_self_attn, x_src_attn
 
 
-class ContexutalBiasDecoder(nn.Module):
+class ContextualBiasDecoder(nn.Module):
     def __init__(
         self,
         size,
         src_attn,
         dropout_rate,
         normalize_before=True,
     ):
         """Construct an DecoderLayer object."""
-        super(ContexutalBiasDecoder, self).__init__()
+        super(ContextualBiasDecoder, self).__init__()
         self.size = size
         self.src_attn = src_attn
         if src_attn is not None:
             self.norm3 = LayerNorm(size)
         self.dropout = nn.Dropout(dropout_rate)
         self.normalize_before = normalize_before
 
@@ -98,15 +98,15 @@
                 x = self.norm3(x)
             x =  self.dropout(self.src_attn(x, memory, memory_mask))
         return x, tgt_mask, memory, memory_mask, cache
 
 
 class ContextualParaformerDecoder(ParaformerSANMDecoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2006.01713
     """
     def __init__(
         self,
         vocab_size: int,
         encoder_output_size: int,
@@ -182,15 +182,15 @@
                 PositionwiseFeedForwardDecoderSANM(attention_dim, linear_units, dropout_rate),
                 dropout_rate,
                 normalize_before,
                 concat_after,
             ),
         )
         self.dropout = nn.Dropout(dropout_rate)
-        self.bias_decoder = ContexutalBiasDecoder(
+        self.bias_decoder = ContextualBiasDecoder(
             size=attention_dim,
             src_attn=MultiHeadedAttentionCrossAtt(
                 attention_heads, attention_dim, src_attention_dropout_rate
             ),
             dropout_rate=dropout_rate,
             normalize_before=True,
         )
```

### Comparing `funasr-0.3.1/funasr/models/decoder/rnn_decoder.py` & `funasr-0.4.1/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/decoder/sanm_decoder.py` & `funasr-0.4.1/funasr/models/decoder/sanm_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         if self.src_attn is not None:
             residual = x
             if self.normalize_before:
                 x = self.norm3(x)
 
             x = residual + self.dropout(self.src_attn(x, memory, memory_mask))
 
-
         return x, tgt_mask, memory, memory_mask, cache
 
     def forward_chunk(self, tgt, tgt_mask, memory, memory_mask=None, cache=None):
         """Compute decoded features.
 
         Args:
             tgt (torch.Tensor): Input tensor (#batch, maxlen_out, size).
@@ -148,15 +147,15 @@
             x = residual + self.dropout(self.src_attn(x, memory, memory_mask))
 
 
         return x, tgt_mask, memory, memory_mask, cache
 
 class FsmnDecoderSCAMAOpt(BaseTransformerDecoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     SCAMA: Streaming chunk-aware multihead attention for online end-to-end speech recognition
     https://arxiv.org/abs/2006.01713
 
     """
     def __init__(
             self,
             vocab_size: int,
@@ -396,31 +395,31 @@
                 cache_layer_num += len(self.decoders2)
             cache = [None] * cache_layer_num
         new_cache = []
         # for c, decoder in zip(cache, self.decoders):
         for i in range(self.att_layer_num):
             decoder = self.decoders[i]
             c = cache[i]
-            x, tgt_mask, memory, memory_mask, c_ret = decoder(
+            x, tgt_mask, memory, memory_mask, c_ret = decoder.forward_chunk(
                 x, tgt_mask, memory, memory_mask, cache=c
             )
             new_cache.append(c_ret)
 
         if self.num_blocks - self.att_layer_num >= 1:
             for i in range(self.num_blocks - self.att_layer_num):
                 j = i + self.att_layer_num
                 decoder = self.decoders2[i]
                 c = cache[j]
-                x, tgt_mask, memory, memory_mask, c_ret = decoder(
+                x, tgt_mask, memory, memory_mask, c_ret = decoder.forward_chunk(
                     x, tgt_mask, memory, memory_mask, cache=c
                 )
                 new_cache.append(c_ret)
 
         for decoder in self.decoders3:
-            x, tgt_mask, memory, memory_mask, _ = decoder(
+            x, tgt_mask, memory, memory_mask, _ = decoder.forward_chunk(
                 x, tgt_mask, memory, None, cache=None
             )
 
         if self.normalize_before:
             y = self.after_norm(x[:, -1])
         else:
             y = x[:, -1]
@@ -809,15 +808,15 @@
                                                                                           var_dict_tf[name_tf].shape))
     
         return var_dict_torch_update
 
 
 class ParaformerSANMDecoder(BaseTransformerDecoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2006.01713
     """
     def __init__(
         self,
         vocab_size: int,
         encoder_output_size: int,
@@ -1073,32 +1072,32 @@
                 cache_layer_num += len(self.decoders2)
             cache = [None] * cache_layer_num
         new_cache = []
         # for c, decoder in zip(cache, self.decoders):
         for i in range(self.att_layer_num):
             decoder = self.decoders[i]
             c = cache[i]
-            x, tgt_mask, memory, memory_mask, c_ret = decoder(
+            x, tgt_mask, memory, memory_mask, c_ret = decoder.forward_chunk(
                 x, tgt_mask, memory, None, cache=c
             )
             new_cache.append(c_ret)
 
         if self.num_blocks - self.att_layer_num > 1:
             for i in range(self.num_blocks - self.att_layer_num):
                 j = i + self.att_layer_num
                 decoder = self.decoders2[i]
                 c = cache[j]
-                x, tgt_mask, memory, memory_mask, c_ret = decoder(
+                x, tgt_mask, memory, memory_mask, c_ret = decoder.forward_chunk(
                     x, tgt_mask, memory, None, cache=c
                 )
                 new_cache.append(c_ret)
 
         for decoder in self.decoders3:
 
-            x, tgt_mask, memory, memory_mask, _ = decoder(
+            x, tgt_mask, memory, memory_mask, _ = decoder.forward_chunk(
                 x, tgt_mask, memory, None, cache=None
             )
 
         if self.normalize_before:
             y = self.after_norm(x[:, -1])
         else:
             y = x[:, -1]
```

### Comparing `funasr-0.3.1/funasr/models/decoder/sv_decoder.py` & `funasr-0.4.1/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/decoder/transformer_decoder.py` & `funasr-0.4.1/funasr/models/decoder/transformer_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
                 concat_after,
             ),
         )
 
 
 class ParaformerDecoderSAN(BaseTransformerDecoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2006.01713
     """
     def __init__(
             self,
             vocab_size: int,
             encoder_output_size: int,
```

### Comparing `funasr-0.3.1/funasr/models/e2e_asr.py` & `funasr-0.4.1/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/e2e_asr_common.py` & `funasr-0.4.1/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/e2e_asr_mfcca.py` & `funasr-0.4.1/funasr/models/e2e_asr_mfcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     @contextmanager
     def autocast(enabled=True):
         yield
 import pdb
 import random
 import math
 class MFCCA(AbsESPnetModel):
-    """CTC-attention hybrid Encoder-Decoder model"""
+    """
+    Author: Audio, Speech and Language Processing Group (ASLP@NPU), Northwestern Polytechnical University
+    MFCCA:Multi-Frame Cross-Channel attention for multi-speaker ASR in Multi-party meeting scenario
+    https://arxiv.org/abs/2210.05265
+    """
 
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
```

### Comparing `funasr-0.3.1/funasr/models/e2e_asr_paraformer.py` & `funasr-0.4.1/funasr/models/e2e_asr_paraformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
 class Paraformer(AbsESPnetModel):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
     """
 
     def __init__(
             self,
             vocab_size: int,
@@ -366,27 +366,18 @@
 
         # Post-encoder, e.g. NLU
         if self.postencoder is not None:
             encoder_out, encoder_out_lens = self.postencoder(
                 encoder_out, encoder_out_lens
             )
 
-        assert encoder_out.size(0) == speech.size(0), (
-            encoder_out.size(),
-            speech.size(0),
-        )
-        assert encoder_out.size(1) <= encoder_out_lens.max(), (
-            encoder_out.size(),
-            encoder_out_lens.max(),
-        )
-
         if intermediate_outs is not None:
             return (encoder_out, intermediate_outs), encoder_out_lens
 
-        return encoder_out, encoder_out_lens
+        return encoder_out, torch.tensor([encoder_out.size(1)])
 
     def calc_predictor(self, encoder_out, encoder_out_lens):
 
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = self.predictor(encoder_out, None, encoder_out_mask,
                                                                                   ignore_id=self.ignore_id)
@@ -617,15 +608,15 @@
             ys_hat = self.ctc.argmax(encoder_out).data
             cer_ctc = self.error_calculator(ys_hat.cpu(), ys_pad.cpu(), is_ctc=True)
         return loss_ctc, cer_ctc
 
 
 class ParaformerBert(Paraformer):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer2: advanced paraformer with LFMMI and bert for non-autoregressive end-to-end speech recognition
     """
 
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
@@ -1030,24 +1021,84 @@
         self.step_cur += 1
         # for data-parallel
         text = text[:, : text_lengths.max()]
         speech = speech[:, :speech_lengths.max()]
 
         # 1. Encoder
         encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
+        intermediate_outs = None
+        if isinstance(encoder_out, tuple):
+            intermediate_outs = encoder_out[1]
+            encoder_out = encoder_out[0]
 
+        loss_att, acc_att, cer_att, wer_att = None, None, None, None
+        loss_ctc, cer_ctc = None, None
+        loss_pre = None
         stats = dict()
 
+        # 1. CTC branch
+        if self.ctc_weight != 0.0:
+            loss_ctc, cer_ctc = self._calc_ctc_loss(
+                encoder_out, encoder_out_lens, text, text_lengths
+            )
+
+            # Collect CTC branch stats
+            stats["loss_ctc"] = loss_ctc.detach() if loss_ctc is not None else None
+            stats["cer_ctc"] = cer_ctc
+
+        # Intermediate CTC (optional)
+        loss_interctc = 0.0
+        if self.interctc_weight != 0.0 and intermediate_outs is not None:
+            for layer_idx, intermediate_out in intermediate_outs:
+                # we assume intermediate_out has the same length & padding
+                # as those of encoder_out
+                loss_ic, cer_ic = self._calc_ctc_loss(
+                    intermediate_out, encoder_out_lens, text, text_lengths
+                )
+                loss_interctc = loss_interctc + loss_ic
+
+                # Collect Intermedaite CTC stats
+                stats["loss_interctc_layer{}".format(layer_idx)] = (
+                    loss_ic.detach() if loss_ic is not None else None
+                )
+                stats["cer_interctc_layer{}".format(layer_idx)] = cer_ic
+
+            loss_interctc = loss_interctc / len(intermediate_outs)
+
+            # calculate whole encoder loss
+            loss_ctc = (
+                               1 - self.interctc_weight
+                       ) * loss_ctc + self.interctc_weight * loss_interctc
+
+        # 2b. Attention decoder branch
+        if self.ctc_weight != 1.0:
+            loss_att, acc_att, cer_att, wer_att, loss_pre = self._calc_att_loss(
+                encoder_out, encoder_out_lens, text, text_lengths
+            )
+
         loss_pre2 = self._calc_pre2_loss(
             encoder_out, encoder_out_lens, text, text_lengths
         )
 
-        loss = loss_pre2
+        # 3. CTC-Att loss definition
+        if self.ctc_weight == 0.0:
+            loss = loss_att + loss_pre * self.predictor_weight + loss_pre2 * self.predictor_weight * 0.5
+        elif self.ctc_weight == 1.0:
+            loss = loss_ctc
+        else:
+            loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight + loss_pre2 * self.predictor_weight * 0.5
 
+        # Collect Attn branch stats
+        stats["loss_att"] = loss_att.detach() if loss_att is not None else None
+        stats["acc"] = acc_att
+        stats["cer"] = cer_att
+        stats["wer"] = wer_att
+        stats["loss_pre"] = loss_pre.detach().cpu() if loss_pre is not None else None
         stats["loss_pre2"] = loss_pre2.detach().cpu()
+
         stats["loss"] = torch.clone(loss.detach())
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
 
@@ -1090,14 +1141,15 @@
             sample_rate: float = 0.6,
             batch_rate: float = 0.5,
             double_rate: float = -1.0,
             target_buffer_length: int = -1,
             inner_dim: int = 256,
             bias_encoder_type: str = 'lstm',
             label_bracket: bool = False,
+            use_decoder_embedding: bool = False,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
@@ -1143,14 +1195,15 @@
         self.target_buffer_length = target_buffer_length
         self.double_rate = double_rate
 
         if self.target_buffer_length > 0:
             self.hotword_buffer = None
             self.length_record = []
             self.current_buffer_length = 0
+        self.use_decoder_embedding = use_decoder_embedding
 
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
@@ -1284,15 +1337,18 @@
                                          min(length - 1, start + self.max_hw_length - 1)) + 1
                     # print(start, end)
                     hw_tokens = ys_pad[i][start:end]
                     hw_lengths.append(len(hw_tokens) - 1)
                     hw_list.append(hw_tokens)
         # padding
         hw_list_pad = pad_list(hw_list, 0)
-        hw_embed = self.decoder.embed(hw_list_pad)
+        if self.use_decoder_embedding:
+            hw_embed = self.decoder.embed(hw_list_pad)
+        else:
+            hw_embed = self.bias_embed(hw_list_pad)
         hw_embed, (_, _) = self.bias_encoder(hw_embed)
         _ind = np.arange(0, len(hw_list)).tolist()
         # update self.hotword_buffer, throw a part if oversize
         selected = hw_embed[_ind, hw_lengths]
         if self.target_buffer_length > 0:
             _b = selected.shape[0]
             if self.hotword_buffer is None:
@@ -1400,21 +1456,27 @@
         return loss_att, acc_att, cer_att, wer_att, loss_pre
 
     def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, hw_list=None):
         if hw_list is None:
             # default hotword list
             hw_list = [torch.Tensor([self.sos]).long().to(encoder_out.device)]  # empty hotword list
             hw_list_pad = pad_list(hw_list, 0)
-            hw_embed = self.bias_embed(hw_list_pad)
+            if self.use_decoder_embedding:
+                hw_embed = self.decoder.embed(hw_list_pad)
+            else:
+                hw_embed = self.bias_embed(hw_list_pad)
             _, (h_n, _) = self.bias_encoder(hw_embed)
             contextual_info = h_n.squeeze(0).repeat(encoder_out.shape[0], 1, 1)
         else:
             hw_lengths = [len(i) for i in hw_list]
             hw_list_pad = pad_list([torch.Tensor(i).long() for i in hw_list], 0).to(encoder_out.device)
-            hw_embed = self.bias_embed(hw_list_pad)
+            if self.use_decoder_embedding:
+                hw_embed = self.decoder.embed(hw_list_pad)
+            else:
+                hw_embed = self.bias_embed(hw_list_pad)
             hw_embed = torch.nn.utils.rnn.pack_padded_sequence(hw_embed, hw_lengths, batch_first=True,
                                                                enforce_sorted=False)
             _, (h_n, _) = self.bias_encoder(hw_embed)
             # hw_embed, _ = torch.nn.utils.rnn.pad_packed_sequence(hw_embed, batch_first=True)
             contextual_info = h_n.squeeze(0).repeat(encoder_out.shape[0], 1, 1)
         decoder_outs = self.decoder(
             encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, contextual_info=contextual_info
```

### Comparing `funasr-0.3.1/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.4.1/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/e2e_diar_sond.py` & `funasr-0.4.1/funasr/models/e2e_diar_sond.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,20 @@
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
 class DiarSondModel(AbsESPnetModel):
-    """Speaker overlap-aware neural diarization model
-    reference: https://arxiv.org/abs/2211.10243
+    """
+    Author: Speech Lab, Alibaba Group, China
+    SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
+    https://arxiv.org/abs/2211.10243
+    TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
+    https://arxiv.org/abs/2303.05397
     """
 
     def __init__(
         self,
         vocab_size: int,
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
```

### Comparing `funasr-0.3.1/funasr/models/e2e_sv.py` & `funasr-0.4.1/funasr/models/e2e_sv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Author: Speech Lab, Alibaba Group, China
+"""
+
 import logging
 from contextlib import contextmanager
 from distutils.version import LooseVersion
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
```

### Comparing `funasr-0.3.1/funasr/models/e2e_tp.py` & `funasr-0.4.1/funasr/models/e2e_tp.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
 class TimestampPredictor(AbsESPnetModel):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     """
 
     def __init__(
             self,
             frontend: Optional[AbsFrontend],
             encoder: AbsEncoder,
             predictor: CifPredictorV3,
```

### Comparing `funasr-0.3.1/funasr/models/e2e_uni_asr.py` & `funasr-0.4.1/funasr/models/e2e_uni_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
 class UniASR(AbsESPnetModel):
     """
-    Author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     """
 
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
```

### Comparing `funasr-0.3.1/funasr/models/e2e_vad.py` & `funasr-0.4.1/funasr/models/e2e_vad.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 
 class VadDetectMode(Enum):
     kVadSingleUtteranceDetectMode = 0
     kVadMutipleUtteranceDetectMode = 1
 
 
 class VADXOptions:
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(
             self,
             sample_rate: int = 16000,
             detect_mode: int = VadDetectMode.kVadMutipleUtteranceDetectMode.value,
             snr_mode: int = 0,
             max_end_silence_time: int = 800,
             max_start_silence_time: int = 3000,
@@ -95,14 +100,19 @@
         self.speech_noise_thresh_high = speech_noise_thresh_high
         self.output_frame_probs = output_frame_probs
         self.frame_in_ms = frame_in_ms
         self.frame_length_ms = frame_length_ms
 
 
 class E2EVadSpeechBufWithDoa(object):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(self):
         self.start_ms = 0
         self.end_ms = 0
         self.buffer = []
         self.contain_seg_start_point = False
         self.contain_seg_end_point = False
         self.doa = 0
@@ -113,23 +123,33 @@
         self.buffer = []
         self.contain_seg_start_point = False
         self.contain_seg_end_point = False
         self.doa = 0
 
 
 class E2EVadFrameProb(object):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(self):
         self.noise_prob = 0.0
         self.speech_prob = 0.0
         self.score = 0.0
         self.frame_id = 0
         self.frm_state = 0
 
 
 class WindowDetector(object):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(self, window_size_ms: int, sil_to_speech_time: int,
                  speech_to_sil_time: int, frame_size_ms: int):
         self.window_size_ms = window_size_ms
         self.sil_to_speech_time = sil_to_speech_time
         self.speech_to_sil_time = speech_to_sil_time
         self.frame_size_ms = frame_size_ms
 
@@ -188,15 +208,20 @@
         return AudioChangeState.kChangeStateInvalid
 
     def FrameSizeMs(self) -> int:
         return int(self.frame_size_ms)
 
 
 class E2EVadModel(nn.Module):
-    def __init__(self, encoder: FSMN, vad_post_args: Dict[str, Any]):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
+    def __init__(self, encoder: FSMN, vad_post_args: Dict[str, Any], frontend=None):
         super(E2EVadModel, self).__init__()
         self.vad_opts = VADXOptions(**vad_post_args)
         self.windows_detector = WindowDetector(self.vad_opts.window_size_ms,
                                                self.vad_opts.sil_to_speech_time_thres,
                                                self.vad_opts.speech_to_sil_time_thres,
                                                self.vad_opts.frame_in_ms)
         self.encoder = encoder
@@ -225,14 +250,15 @@
         self.scores = None
         self.max_time_out = False
         self.decibel = []
         self.data_buf = None
         self.data_buf_all = None
         self.waveform = None
         self.ResetDetection()
+        self.frontend = frontend
 
     def AllResetDetection(self):
         self.is_final = False
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
@@ -455,33 +481,35 @@
         else:
             self.DetectLastFrames()
         segments = []
         for batch_num in range(0, feats.shape[0]):  # only support batch_size = 1 now
             segment_batch = []
             if len(self.output_data_buf) > 0:
                 for i in range(self.output_data_buf_offset, len(self.output_data_buf)):
-                    if not self.output_data_buf[i].contain_seg_start_point or not self.output_data_buf[
-                        i].contain_seg_end_point:
+                    if not is_final and (not self.output_data_buf[i].contain_seg_start_point or not self.output_data_buf[
+                        i].contain_seg_end_point):
                         continue
                     segment = [self.output_data_buf[i].start_ms, self.output_data_buf[i].end_ms]
                     segment_batch.append(segment)
                     self.output_data_buf_offset += 1  # need update this parameter
             if segment_batch:
                 segments.append(segment_batch)
         if is_final:
             # reset class variables and clear the dict for the next query
             self.AllResetDetection()
         return segments, in_cache
 
     def forward_online(self, feats: torch.Tensor, waveform: torch.tensor, in_cache: Dict[str, torch.Tensor] = dict(),
-                is_final: bool = False
+                is_final: bool = False, max_end_sil: int = 800
                 ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
+        self.max_end_sil_frame_cnt_thresh = max_end_sil - self.vad_opts.speech_to_sil_time_thres
         self.waveform = waveform  # compute decibel for each frame
-        self.ComputeDecibel()
+        
         self.ComputeScores(feats, in_cache)
+        self.ComputeDecibel()
         if not is_final:
             self.DetectCommonFrames()
         else:
             self.DetectLastFrames()
         segments = []
         for batch_num in range(0, feats.shape[0]):  # only support batch_size = 1 now
             segment_batch = []
```

### Comparing `funasr-0.3.1/funasr/models/encoder/conformer_encoder.py` & `funasr-0.4.1/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.4.1/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.4.1/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.4.1/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.4.1/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.4.1/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         # add parenthesis for repeat module
         return self.activation(outputs), ilens
 
 
 class ConvEncoder(AbsEncoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Convolution encoder in OpenNMT framework
     """
 
     def __init__(
             self,
             num_layers,
             input_units,
```

### Comparing `funasr-0.3.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             x = self.norm2(x)
 
         return x, mask, cache, mask_att_chunk_encoder
 
 
 class SelfAttentionEncoder(AbsEncoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     Self attention encoder in OpenNMT framework
     """
 
     def __init__(
         self,
         input_size: int,
         output_size: int = 256,
```

### Comparing `funasr-0.3.1/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.4.1/funasr/models/encoder/resnet34_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,14 +402,20 @@
             num_nodes_last_layer=256,
             pooling_type="window_shift",
             pool_size=20,
             stride=1,
             tf2torch_tensor_name_prefix_torch="encoder",
             tf2torch_tensor_name_prefix_tf="seq2seq/speech_encoder"
     ):
+        """
+        Author: Speech Lab, Alibaba Group, China
+        SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
+        https://arxiv.org/abs/2211.10243
+        """
+
         super(ResNet34Diar, self).__init__(
             input_size,
             use_head_conv=use_head_conv,
             batchnorm_momentum=batchnorm_momentum,
             use_head_maxpool=use_head_maxpool,
             num_nodes_pooling_layer=num_nodes_pooling_layer,
             layers_in_block=layers_in_block,
@@ -629,14 +635,20 @@
             num_nodes_last_layer=256,
             pooling_type="window_shift",
             pool_size=20,
             stride=1,
             tf2torch_tensor_name_prefix_torch="encoder",
             tf2torch_tensor_name_prefix_tf="seq2seq/speech_encoder"
     ):
+        """
+        Author: Speech Lab, Alibaba Group, China
+        TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
+        https://arxiv.org/abs/2303.05397
+        """
+
         super(ResNet34SpL2RegDiar, self).__init__(
             input_size,
             use_head_conv=use_head_conv,
             batchnorm_momentum=batchnorm_momentum,
             use_head_maxpool=use_head_maxpool,
             num_nodes_pooling_layer=num_nodes_pooling_layer,
             layers_in_block=layers_in_block,
```

### Comparing `funasr-0.3.1/funasr/models/encoder/rnn_encoder.py` & `funasr-0.4.1/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/encoder/sanm_encoder.py` & `funasr-0.4.1/funasr/models/encoder/sanm_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import torch
 import torch.nn as nn
 from funasr.modules.streaming_utils.chunk_utilis import overlap_chunk
 from typeguard import check_argument_types
 import numpy as np
 from funasr.modules.nets_utils import make_pad_mask
-from funasr.modules.attention import MultiHeadedAttention, MultiHeadedAttentionSANM
+from funasr.modules.attention import MultiHeadedAttention, MultiHeadedAttentionSANM, MultiHeadedAttentionSANMwithMask
 from funasr.modules.embedding import SinusoidalPositionEncoder
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
 from funasr.modules.multi_layer_conv import MultiLayeredConv1d
 from funasr.modules.positionwise_feed_forward import (
     PositionwiseFeedForward,  # noqa: H301
 )
@@ -23,15 +23,15 @@
 from funasr.modules.subsampling import Conv2dSubsampling2
 from funasr.modules.subsampling import Conv2dSubsampling6
 from funasr.modules.subsampling import Conv2dSubsampling8
 from funasr.modules.subsampling import TooShortUttError
 from funasr.modules.subsampling import check_short_utt
 from funasr.models.ctc import CTC
 from funasr.models.encoder.abs_encoder import AbsEncoder
-
+from funasr.modules.mask import subsequent_mask, vad_mask
 
 class EncoderLayerSANM(nn.Module):
     def __init__(
         self,
         in_size,
         size,
         self_attn,
@@ -113,15 +113,15 @@
             x = self.norm2(x)
 
 
         return x, mask, cache, mask_shfit_chunk, mask_att_chunk_encoder
 
 class SANMEncoder(AbsEncoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     San-m: Memory equipped self-attention for end-to-end speech recognition
     https://arxiv.org/abs/2006.01713
 
     """
 
     def __init__(
         self,
@@ -545,15 +545,15 @@
                                                                                       var_dict_tf[name_tf].shape))
     
         return var_dict_torch_update
 
 
 class SANMEncoderChunkOpt(AbsEncoder):
     """
-    author: Speech Lab, Alibaba Group, China
+    Author: Speech Lab of DAMO Academy, Alibaba Group
     SCAMA: Streaming chunk-aware multihead attention for online end-to-end speech recognition
     https://arxiv.org/abs/2006.01713
 
     """
 
     def __init__(
             self,
@@ -954,7 +954,235 @@
                     data_tf = torch.from_numpy(data_tf).type(torch.float32).to("cpu")
                     var_dict_torch_update[name] = data_tf
                     logging.info(
                         "torch tensor: {}, {}, loading from tf tensor: {}, {}".format(name, data_tf.size(), name_tf,
                                                                                       var_dict_tf[name_tf].shape))
     
         return var_dict_torch_update
+
+
+class SANMVadEncoder(AbsEncoder):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+
+    """
+
+    def __init__(
+        self,
+        input_size: int,
+        output_size: int = 256,
+        attention_heads: int = 4,
+        linear_units: int = 2048,
+        num_blocks: int = 6,
+        dropout_rate: float = 0.1,
+        positional_dropout_rate: float = 0.1,
+        attention_dropout_rate: float = 0.0,
+        input_layer: Optional[str] = "conv2d",
+        pos_enc_class=SinusoidalPositionEncoder,
+        normalize_before: bool = True,
+        concat_after: bool = False,
+        positionwise_layer_type: str = "linear",
+        positionwise_conv_kernel_size: int = 1,
+        padding_idx: int = -1,
+        interctc_layer_idx: List[int] = [],
+        interctc_use_conditioning: bool = False,
+        kernel_size : int = 11,
+        sanm_shfit : int = 0,
+        selfattention_layer_type: str = "sanm",
+    ):
+        assert check_argument_types()
+        super().__init__()
+        self._output_size = output_size
+
+        if input_layer == "linear":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Linear(input_size, output_size),
+                torch.nn.LayerNorm(output_size),
+                torch.nn.Dropout(dropout_rate),
+                torch.nn.ReLU(),
+                pos_enc_class(output_size, positional_dropout_rate),
+            )
+        elif input_layer == "conv2d":
+            self.embed = Conv2dSubsampling(input_size, output_size, dropout_rate)
+        elif input_layer == "conv2d2":
+            self.embed = Conv2dSubsampling2(input_size, output_size, dropout_rate)
+        elif input_layer == "conv2d6":
+            self.embed = Conv2dSubsampling6(input_size, output_size, dropout_rate)
+        elif input_layer == "conv2d8":
+            self.embed = Conv2dSubsampling8(input_size, output_size, dropout_rate)
+        elif input_layer == "embed":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Embedding(input_size, output_size, padding_idx=padding_idx),
+                SinusoidalPositionEncoder(),
+            )
+        elif input_layer is None:
+            if input_size == output_size:
+                self.embed = None
+            else:
+                self.embed = torch.nn.Linear(input_size, output_size)
+        elif input_layer == "pe":
+            self.embed = SinusoidalPositionEncoder()
+        else:
+            raise ValueError("unknown input_layer: " + input_layer)
+        self.normalize_before = normalize_before
+        if positionwise_layer_type == "linear":
+            positionwise_layer = PositionwiseFeedForward
+            positionwise_layer_args = (
+                output_size,
+                linear_units,
+                dropout_rate,
+            )
+        elif positionwise_layer_type == "conv1d":
+            positionwise_layer = MultiLayeredConv1d
+            positionwise_layer_args = (
+                output_size,
+                linear_units,
+                positionwise_conv_kernel_size,
+                dropout_rate,
+            )
+        elif positionwise_layer_type == "conv1d-linear":
+            positionwise_layer = Conv1dLinear
+            positionwise_layer_args = (
+                output_size,
+                linear_units,
+                positionwise_conv_kernel_size,
+                dropout_rate,
+            )
+        else:
+            raise NotImplementedError("Support only linear or conv1d.")
+
+        if selfattention_layer_type == "selfattn":
+            encoder_selfattn_layer = MultiHeadedAttention
+            encoder_selfattn_layer_args = (
+                attention_heads,
+                output_size,
+                attention_dropout_rate,
+            )
+
+        elif selfattention_layer_type == "sanm":
+            self.encoder_selfattn_layer = MultiHeadedAttentionSANMwithMask
+            encoder_selfattn_layer_args0 = (
+                attention_heads,
+                input_size,
+                output_size,
+                attention_dropout_rate,
+                kernel_size,
+                sanm_shfit,
+            )
+
+            encoder_selfattn_layer_args = (
+                attention_heads,
+                output_size,
+                output_size,
+                attention_dropout_rate,
+                kernel_size,
+                sanm_shfit,
+            )
+
+        self.encoders0 = repeat(
+            1,
+            lambda lnum: EncoderLayerSANM(
+                input_size,
+                output_size,
+                self.encoder_selfattn_layer(*encoder_selfattn_layer_args0),
+                positionwise_layer(*positionwise_layer_args),
+                dropout_rate,
+                normalize_before,
+                concat_after,
+            ),
+        )
+
+        self.encoders = repeat(
+            num_blocks-1,
+            lambda lnum: EncoderLayerSANM(
+                output_size,
+                output_size,
+                self.encoder_selfattn_layer(*encoder_selfattn_layer_args),
+                positionwise_layer(*positionwise_layer_args),
+                dropout_rate,
+                normalize_before,
+                concat_after,
+            ),
+        )
+        if self.normalize_before:
+            self.after_norm = LayerNorm(output_size)
+
+        self.interctc_layer_idx = interctc_layer_idx
+        if len(interctc_layer_idx) > 0:
+            assert 0 < min(interctc_layer_idx) and max(interctc_layer_idx) < num_blocks
+        self.interctc_use_conditioning = interctc_use_conditioning
+        self.conditioning_layer = None
+        self.dropout = nn.Dropout(dropout_rate)
+
+    def output_size(self) -> int:
+        return self._output_size
+
+    def forward(
+        self,
+        xs_pad: torch.Tensor,
+        ilens: torch.Tensor,
+        vad_indexes: torch.Tensor,
+        prev_states: torch.Tensor = None,
+        ctc: CTC = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
+        """Embed positions in tensor.
+
+        Args:
+            xs_pad: input tensor (B, L, D)
+            ilens: input length (B)
+            prev_states: Not to be used now.
+        Returns:
+            position embedded tensor and mask
+        """
+        masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
+        sub_masks = subsequent_mask(masks.size(-1), device=xs_pad.device).unsqueeze(0)
+        no_future_masks = masks & sub_masks
+        xs_pad *= self.output_size()**0.5
+        if self.embed is None:
+            xs_pad = xs_pad
+        elif (isinstance(self.embed, Conv2dSubsampling) or isinstance(self.embed, Conv2dSubsampling2)
+              or isinstance(self.embed, Conv2dSubsampling6) or isinstance(self.embed, Conv2dSubsampling8)):
+            short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
+            if short_status:
+                raise TooShortUttError(
+                    f"has {xs_pad.size(1)} frames and is too short for subsampling " +
+                    f"(it needs more than {limit_size} frames), return empty results",
+                    xs_pad.size(1),
+                    limit_size,
+                )
+            xs_pad, masks = self.embed(xs_pad, masks)
+        else:
+            xs_pad = self.embed(xs_pad)
+
+        # xs_pad = self.dropout(xs_pad)
+        mask_tup0 = [masks, no_future_masks]
+        encoder_outs = self.encoders0(xs_pad, mask_tup0)
+        xs_pad, _ = encoder_outs[0], encoder_outs[1]
+        intermediate_outs = []
+
+
+        for layer_idx, encoder_layer in enumerate(self.encoders):
+                if layer_idx + 1 == len(self.encoders):
+                    # This is last layer.
+                    coner_mask = torch.ones(masks.size(0),
+                                            masks.size(-1),
+                                            masks.size(-1),
+                                            device=xs_pad.device,
+                                            dtype=torch.bool)
+                    for word_index, length in enumerate(ilens):
+                        coner_mask[word_index, :, :] = vad_mask(masks.size(-1),
+                                                                vad_indexes[word_index],
+                                                                device=xs_pad.device)
+                    layer_mask = masks & coner_mask
+                else:
+                    layer_mask = no_future_masks
+                mask_tup1 = [masks, layer_mask]
+                encoder_outs = encoder_layer(xs_pad, mask_tup1)
+                xs_pad, layer_mask = encoder_outs[0], encoder_outs[1]
+
+        if self.normalize_before:
+            xs_pad = self.after_norm(xs_pad)
+
+        olens = masks.squeeze(1).sum(1)
+        if len(intermediate_outs) > 0:
+            return (xs_pad, intermediate_outs), olens, None
+        return xs_pad, olens, None
```

### Comparing `funasr-0.3.1/funasr/models/encoder/transformer_encoder.py` & `funasr-0.4.1/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/default.py` & `funasr-0.4.1/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.4.1/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/fused.py` & `funasr-0.4.1/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/s3prl.py` & `funasr-0.4.1/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/wav_frontend.py` & `funasr-0.4.1/funasr/models/frontend/wav_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,23 @@
     means = np.array(means_list).astype(np.float)
     vars = np.array(vars_list).astype(np.float)
     cmvn = np.array([means, vars])
     cmvn = torch.as_tensor(cmvn)
     return cmvn
 
 
-def apply_cmvn(inputs, cmvn_file):  # noqa
+def apply_cmvn(inputs, cmvn):  # noqa
     """
     Apply CMVN with mvn data
     """
 
     device = inputs.device
     dtype = inputs.dtype
     frame, dim = inputs.shape
 
-    cmvn = load_cmvn(cmvn_file)
     means = np.tile(cmvn[0:1, :dim], (frame, 1))
     vars = np.tile(cmvn[1:2, :dim], (frame, 1))
     inputs += torch.from_numpy(means).type(dtype).to(device)
     inputs *= torch.from_numpy(vars).type(dtype).to(device)
 
     return inputs.type(torch.float32)
 
@@ -107,14 +106,15 @@
         self.filter_length_max = filter_length_max
         self.lfr_m = lfr_m
         self.lfr_n = lfr_n
         self.cmvn_file = cmvn_file
         self.dither = dither
         self.snip_edges = snip_edges
         self.upsacle_samples = upsacle_samples
+        self.cmvn = None if self.cmvn_file is None else load_cmvn(self.cmvn_file)
 
     def output_size(self) -> int:
         return self.n_mels * self.lfr_m
 
     def forward(
             self,
             input: torch.Tensor,
@@ -136,16 +136,16 @@
                               energy_floor=0.0,
                               window_type=self.window,
                               sample_frequency=self.fs,
                               snip_edges=self.snip_edges)
 
             if self.lfr_m != 1 or self.lfr_n != 1:
                 mat = apply_lfr(mat, self.lfr_m, self.lfr_n)
-            if self.cmvn_file is not None:
-                mat = apply_cmvn(mat, self.cmvn_file)
+            if self.cmvn is not None:
+                mat = apply_cmvn(mat, self.cmvn)
             feat_length = mat.size(0)
             feats.append(mat)
             feats_lens.append(feat_length)
 
         feats_lens = torch.as_tensor(feats_lens)
         feats_pad = pad_sequence(feats,
                                  batch_first=True,
@@ -190,16 +190,16 @@
         batch_size = input.size(0)
         feats = []
         feats_lens = []
         for i in range(batch_size):
             mat = input[i, :input_lengths[i], :]
             if self.lfr_m != 1 or self.lfr_n != 1:
                 mat = apply_lfr(mat, self.lfr_m, self.lfr_n)
-            if self.cmvn_file is not None:
-                mat = apply_cmvn(mat, self.cmvn_file)
+            if self.cmvn is not None:
+                mat = apply_cmvn(mat, self.cmvn)
             feat_length = mat.size(0)
             feats.append(mat)
             feats_lens.append(feat_length)
 
         feats_lens = torch.as_tensor(feats_lens)
         feats_pad = pad_sequence(feats,
                                  batch_first=True,
```

### Comparing `funasr-0.3.1/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.4.1/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/frontend/windowing.py` & `funasr-0.4.1/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/pooling/statistic_pooling.py` & `funasr-0.4.1/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.4.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/predictor/cif.py` & `funasr-0.4.1/funasr/models/predictor/cif.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         if target_length is None and self.tail_threshold > 0.0:
             token_num_int = torch.max(token_num).type(torch.int32).item()
             acoustic_embeds = acoustic_embeds[:, :token_num_int, :]
 
         return acoustic_embeds, token_num, alphas, cif_peak
 
     def forward_chunk(self, hidden, cache=None):
+        b, t, d = hidden.size()
         h = hidden
         context = h.transpose(1, 2)
         queries = self.pad(context)
         output = torch.relu(self.cif_conv1d(queries))
         output = output.transpose(1, 2)
         output = self.cif_output(output)
         alphas = torch.sigmoid(output)
@@ -216,47 +217,54 @@
             mask_chunk_predictor = torch.zeros_like(alphas)
             mask_chunk_predictor[:, cache["pad_left"]:cache["stride"] + cache["pad_left"]] = 1.0
        
         if mask_chunk_predictor is not None:
             alphas = alphas * mask_chunk_predictor
       
         if cache is not None:
+            if cache["is_final"]:
+                alphas[:, cache["stride"] + cache["pad_left"] - 1] += 0.45
             if cache["cif_hidden"] is not None:
                 hidden = torch.cat((cache["cif_hidden"], hidden), 1)
             if cache["cif_alphas"] is not None:
                 alphas = torch.cat((cache["cif_alphas"], alphas), -1)
 
         token_num = alphas.sum(-1)
         acoustic_embeds, cif_peak = cif(hidden, alphas, self.threshold)
         len_time = alphas.size(-1)
         last_fire_place = len_time - 1
         last_fire_remainds = 0.0
         pre_alphas_length = 0
+        last_fire = False
  
         mask_chunk_peak_predictor = None
         if cache is not None:
             mask_chunk_peak_predictor = None
             mask_chunk_peak_predictor = torch.zeros_like(cif_peak)
             if cache["cif_alphas"] is not None:
                 pre_alphas_length = cache["cif_alphas"].size(-1)
                 mask_chunk_peak_predictor[:, :pre_alphas_length] = 1.0
             mask_chunk_peak_predictor[:, pre_alphas_length + cache["pad_left"]:pre_alphas_length + cache["stride"] + cache["pad_left"]] = 1.0
             
-
         if mask_chunk_peak_predictor is not None:
             cif_peak = cif_peak * mask_chunk_peak_predictor.squeeze(-1)
         
         for i in range(len_time):
             if cif_peak[0][len_time - 1 - i] > self.threshold or cif_peak[0][len_time - 1 - i] == self.threshold:
                 last_fire_place = len_time - 1 - i
                 last_fire_remainds = cif_peak[0][len_time - 1 - i] - self.threshold
+                last_fire = True
                 break
-        last_fire_remainds = torch.tensor([last_fire_remainds], dtype=alphas.dtype).to(alphas.device)
-        cache["cif_hidden"] = hidden[:, last_fire_place:, :]
-        cache["cif_alphas"] = torch.cat((last_fire_remainds.unsqueeze(0), alphas[:, last_fire_place+1:]), -1)
+        if last_fire:
+           last_fire_remainds = torch.tensor([last_fire_remainds], dtype=alphas.dtype).to(alphas.device)
+           cache["cif_hidden"] = hidden[:, last_fire_place:, :]
+           cache["cif_alphas"] = torch.cat((last_fire_remainds.unsqueeze(0), alphas[:, last_fire_place+1:]), -1)
+        else:
+           cache["cif_hidden"] = hidden
+           cache["cif_alphas"] = alphas
         token_num_int = token_num.floor().type(torch.int32).item()
         return acoustic_embeds[:, 0:token_num_int, :], token_num, alphas, cif_peak
 
     def tail_process_fn(self, hidden, alphas, token_num=None, mask=None):
         b, t, d = hidden.size()
         tail_threshold = self.tail_threshold
         if mask is not None:
```

### Comparing `funasr-0.3.1/funasr/models/preencoder/linear.py` & `funasr-0.4.1/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/preencoder/sinc.py` & `funasr-0.4.1/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/models/specaug/specaug.py` & `funasr-0.4.1/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/add_sos_eos.py` & `funasr-0.4.1/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/attention.py` & `funasr-0.4.1/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.4.1/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.4.1/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/beam_search/beam_search.py` & `funasr-0.4.1/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/data_utils.py` & `funasr-0.4.1/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/ema_module.py` & `funasr-0.4.1/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.4.1/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/quant_noise.py` & `funasr-0.4.1/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/utils.py` & `funasr-0.4.1/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.4.1/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/dynamic_conv.py` & `funasr-0.4.1/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/dynamic_conv2d.py` & `funasr-0.4.1/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/e2e_asr_common.py` & `funasr-0.4.1/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/eend_ola/encoder.py` & `funasr-0.4.1/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.4.1/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/embedding.py` & `funasr-0.4.1/funasr/modules/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright 2019 Shigeki Karita
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Positional Encoding Module."""
 
 import math
 import torch
-
+import torch.nn.functional as F
 
 def _pre_hook(
     state_dict,
     prefix,
     local_metadata,
     strict,
     missing_keys,
@@ -405,13 +405,22 @@
         positions = torch.arange(1, timesteps+1)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
 
         return x + position_encoding
 
     def forward_chunk(self, x, cache=None):
         start_idx = 0
+        pad_left = 0
+        pad_right = 0
         batch_size, timesteps, input_dim = x.size()
         if cache is not None:
             start_idx = cache["start_idx"]
+            pad_left = cache["left"]
+            pad_right = cache["right"]
         positions = torch.arange(1, timesteps+start_idx+1)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
-        return x + position_encoding[:, start_idx: start_idx + timesteps]
+        outputs = x + position_encoding[:, start_idx: start_idx + timesteps]
+        outputs = outputs.transpose(1,2)
+        outputs = F.pad(outputs, (pad_left, pad_right))
+        outputs = outputs.transpose(1,2)
+        return outputs
+
```

### Comparing `funasr-0.3.1/funasr/modules/frontends/beamformer.py` & `funasr-0.4.1/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.4.1/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.4.1/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/frontends/feature_transform.py` & `funasr-0.4.1/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/frontends/frontend.py` & `funasr-0.4.1/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/frontends/mask_estimator.py` & `funasr-0.4.1/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/layer_norm.py` & `funasr-0.4.1/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/lightconv.py` & `funasr-0.4.1/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/lightconv2d.py` & `funasr-0.4.1/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/mask.py` & `funasr-0.4.1/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/multi_layer_conv.py` & `funasr-0.4.1/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/nets_utils.py` & `funasr-0.4.1/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/positionwise_feed_forward.py` & `funasr-0.4.1/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/repeat.py` & `funasr-0.4.1/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/rnn/argument.py` & `funasr-0.4.1/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/rnn/attentions.py` & `funasr-0.4.1/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/rnn/decoders.py` & `funasr-0.4.1/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/rnn/encoders.py` & `funasr-0.4.1/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/scorers/ctc.py` & `funasr-0.4.1/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.4.1/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/scorers/length_bonus.py` & `funasr-0.4.1/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/scorers/scorer_interface.py` & `funasr-0.4.1/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.4.1/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch.nn.functional as F
 from funasr.modules.streaming_utils.utils import sequence_mask
 
 
 
 class overlap_chunk():
 	"""
-	author: Speech Lab, Alibaba Group, China
+	Author: Speech Lab of DAMO Academy, Alibaba Group
 	San-m: Memory equipped self-attention for end-to-end speech recognition
 	https://arxiv.org/abs/2006.01713
 
 	"""
 	def __init__(self,
 		chunk_size: tuple = (16,),
 		stride: tuple = (10,),
```

### Comparing `funasr-0.3.1/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.4.1/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/streaming_utils/utils.py` & `funasr-0.4.1/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/subsampling.py` & `funasr-0.4.1/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/modules/subsampling_without_posenc.py` & `funasr-0.4.1/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/optimizers/fairseq_adam.py` & `funasr-0.4.1/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/optimizers/sgd.py` & `funasr-0.4.1/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/punctuation/espnet_model.py` & `funasr-0.4.1/funasr/train/abs_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,61 @@
+from abc import ABC
+from abc import abstractmethod
+
+
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
 from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
-from funasr.punctuation.abs_model import AbsPunctuation
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.train.abs_espnet_model import AbsESPnetModel
 
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
+
+
+class AbsPunctuation(torch.nn.Module, BatchScorerInterface, ABC):
+    """The abstract class
+
+    To share the loss calculation way among different models,
+    We uses delegate pattern here:
+    The instance of this class should be passed to "LanguageModel"
+
+    This "model" is one of mediator objects for "Task" class.
+
+    """
+
+    @abstractmethod
+    def forward(self, input: torch.Tensor, hidden: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def with_vad(self) -> bool:
+        raise NotImplementedError
 
-class ESPnetPunctuationModel(AbsESPnetModel):
 
+class PunctuationModel(AbsESPnetModel):
+    
     def __init__(self, punc_model: AbsPunctuation, vocab_size: int, ignore_id: int = 0, punc_weight: list = None):
         assert check_argument_types()
         super().__init__()
         self.punc_model = punc_model
         self.punc_weight = torch.Tensor(punc_weight)
         self.sos = 1
         self.eos = 2
-
+        
         # ignore_id may be assumed as 0, shared with CTC-blank symbol for ASR.
         self.ignore_id = ignore_id
-        #if self.punc_model.with_vad():
+        # if self.punc_model.with_vad():
         #    print("This is a vad puncuation model.")
-
+    
     def nll(
         self,
         text: torch.Tensor,
         punc: torch.Tensor,
         text_lengths: torch.Tensor,
         punc_lengths: torch.Tensor,
         max_length: Optional[int] = None,
@@ -50,48 +75,49 @@
         # For data parallel
         if max_length is None:
             text = text[:, :text_lengths.max()]
             punc = punc[:, :text_lengths.max()]
         else:
             text = text[:, :max_length]
             punc = punc[:, :max_length]
-       
+        
         if self.punc_model.with_vad():
             # Should be VadRealtimeTransformer
             assert vad_indexes is not None
             y, _ = self.punc_model(text, text_lengths, vad_indexes)
         else:
             # Should be TargetDelayTransformer,
             y, _ = self.punc_model(text, text_lengths)
-
+        
         # Calc negative log likelihood
         # nll: (BxL,)
         if self.training == False:
             _, indices = y.view(-1, y.shape[-1]).topk(1, dim=1)
             from sklearn.metrics import f1_score
             f1_score = f1_score(punc.view(-1).detach().cpu().numpy(),
                                 indices.squeeze(-1).detach().cpu().numpy(),
                                 average='micro')
             nll = torch.Tensor([f1_score]).repeat(text_lengths.sum())
             return nll, text_lengths
         else:
             self.punc_weight = self.punc_weight.to(punc.device)
-            nll = F.cross_entropy(y.view(-1, y.shape[-1]), punc.view(-1), self.punc_weight, reduction="none", ignore_index=self.ignore_id)
+            nll = F.cross_entropy(y.view(-1, y.shape[-1]), punc.view(-1), self.punc_weight, reduction="none",
+                                  ignore_index=self.ignore_id)
         # nll: (BxL,) -> (BxL,)
         if max_length is None:
             nll.masked_fill_(make_pad_mask(text_lengths).to(nll.device).view(-1), 0.0)
         else:
             nll.masked_fill_(
                 make_pad_mask(text_lengths, maxlen=max_length + 1).to(nll.device).view(-1),
                 0.0,
             )
         # nll: (BxL,) -> (B, L)
         nll = nll.view(batch_size, -1)
         return nll, text_lengths
-
+    
     def batchify_nll(self,
                      text: torch.Tensor,
                      punc: torch.Tensor,
                      text_lengths: torch.Tensor,
                      punc_lengths: torch.Tensor,
                      batch_size: int = 100) -> Tuple[torch.Tensor, torch.Tensor]:
         """Compute negative log likelihood(nll) from transformer language model
@@ -109,15 +135,15 @@
         total_num = text.size(0)
         if total_num <= batch_size:
             nll, x_lengths = self.nll(text, punc, text_lengths)
         else:
             nlls = []
             x_lengths = []
             max_length = text_lengths.max()
-
+            
             start_idx = 0
             while True:
                 end_idx = min(start_idx + batch_size, total_num)
                 batch_text = text[start_idx:end_idx, :]
                 batch_punc = punc[start_idx:end_idx, :]
                 batch_text_lengths = text_lengths[start_idx:end_idx]
                 # batch_nll: [B * T]
@@ -128,37 +154,37 @@
                 if start_idx == total_num:
                     break
             nll = torch.cat(nlls)
             x_lengths = torch.cat(x_lengths)
         assert nll.size(0) == total_num
         assert x_lengths.size(0) == total_num
         return nll, x_lengths
-
+    
     def forward(
         self,
         text: torch.Tensor,
         punc: torch.Tensor,
         text_lengths: torch.Tensor,
         punc_lengths: torch.Tensor,
         vad_indexes: Optional[torch.Tensor] = None,
         vad_indexes_lengths: Optional[torch.Tensor] = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         nll, y_lengths = self.nll(text, punc, text_lengths, punc_lengths, vad_indexes=vad_indexes)
         ntokens = y_lengths.sum()
         loss = nll.sum() / ntokens
         stats = dict(loss=loss.detach())
-
+        
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, ntokens), loss.device)
         return loss, stats, weight
-
+    
     def collect_feats(self, text: torch.Tensor, punc: torch.Tensor,
                       text_lengths: torch.Tensor) -> Dict[str, torch.Tensor]:
         return {}
-
+    
     def inference(self,
                   text: torch.Tensor,
                   text_lengths: torch.Tensor,
                   vad_indexes: Optional[torch.Tensor] = None) -> Tuple[torch.Tensor, None]:
         if self.punc_model.with_vad():
             assert vad_indexes is not None
             return self.punc_model(text, text_lengths, vad_indexes)
```

### Comparing `funasr-0.3.1/funasr/punctuation/target_delay_transformer.py` & `funasr-0.4.1/funasr/models/target_delay_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Any
 from typing import List
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 
-from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.embedding import SinusoidalPositionEncoder
 #from funasr.models.encoder.transformer_encoder import TransformerEncoder as Encoder
-from funasr.punctuation.sanm_encoder import SANMEncoder as Encoder
+from funasr.models.encoder.sanm_encoder import SANMEncoder as Encoder
 #from funasr.modules.mask import subsequent_n_mask
-from funasr.punctuation.abs_model import AbsPunctuation
+from funasr.train.abs_model import AbsPunctuation
 
 
 class TargetDelayTransformer(AbsPunctuation):
-
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
+    https://arxiv.org/pdf/2003.01309.pdf
+    """
     def __init__(
         self,
         vocab_size: int,
         punc_size: int,
         pos_enc: str = None,
         embed_unit: int = 128,
         att_unit: int = 256,
```

### Comparing `funasr-0.3.1/funasr/punctuation/vad_realtime_transformer.py` & `funasr-0.4.1/funasr/models/vad_realtime_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 from typing import List
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 from funasr.modules.embedding import SinusoidalPositionEncoder
-from funasr.punctuation.sanm_encoder import SANMVadEncoder as Encoder
-from funasr.punctuation.abs_model import AbsPunctuation
+from funasr.models.encoder.sanm_encoder import SANMVadEncoder as Encoder
+from funasr.train.abs_model import AbsPunctuation
 
 
 class VadRealtimeTransformer(AbsPunctuation):
-
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
+    https://arxiv.org/pdf/2003.01309.pdf
+    """
     def __init__(
         self,
         vocab_size: int,
         punc_size: int,
         pos_enc: str = None,
         embed_unit: int = 128,
         att_unit: int = 256,
```

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 class Paraformer():
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
-                 pred_bias: int = 1,
                  quantize: bool = False,
                  intra_op_num_threads: int = 1,
                  ):
 
         if not Path(model_dir).exists():
             raise FileNotFoundError(f'{model_dir} does not exist.')
 
@@ -42,28 +41,37 @@
         self.tokenizer = CharTokenizer()
         self.frontend = WavFrontend(
             cmvn_file=cmvn_file,
             **config['frontend_conf']
         )
         self.ort_infer = torch.jit.load(model_file)
         self.batch_size = batch_size
+        self.device_id = device_id
         self.plot_timestamp_to = plot_timestamp_to
-        self.pred_bias = pred_bias
+        if "predictor_bias" in config['model_conf'].keys():
+            self.pred_bias = config['model_conf']['predictor_bias']
+        else:
+            self.pred_bias = 0
 
     def __call__(self, wav_content: Union[str, np.ndarray, List[str]], **kwargs) -> List:
         waveform_list = self.load_data(wav_content, self.frontend.opts.frame_opts.samp_freq)
         waveform_nums = len(waveform_list)
         asr_res = []
         for beg_idx in range(0, waveform_nums, self.batch_size):
             
             end_idx = min(waveform_nums, beg_idx + self.batch_size)
             feats, feats_len = self.extract_feat(waveform_list[beg_idx:end_idx])
             try:
-                outputs = self.ort_infer(feats, feats_len)
-                am_scores, valid_token_lens = outputs[0], outputs[1]
+                with torch.no_grad():
+                    if int(self.device_id) == -1:
+                        outputs = self.ort_infer(feats, feats_len)
+                        am_scores, valid_token_lens = outputs[0], outputs[1]
+                    else:
+                        outputs = self.ort_infer(feats.cuda(), feats_len.cuda())
+                        am_scores, valid_token_lens = outputs[0].cpu(), outputs[1].cpu()
                 if len(outputs) == 4:
                     # for BiCifParaformer Inference
                     us_alphas, us_peaks = outputs[2], outputs[3]
                 else:
                     us_alphas, us_peaks = None, None
             except:
                 #logging.warning(traceback.format_exc())
```

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,36 +19,33 @@
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
         check_argument_types()
 
-        # self.token_list = self.load_token(token_path)
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
+        self.token2id = {v: i for i, v in enumerate(self.token_list)}
+        self.unk_id = self.token2id[self.unk_symbol]
+
 
     def get_num_vocabulary_size(self) -> int:
         return len(self.token_list)
 
     def ids2tokens(self,
                    integers: Union[np.ndarray, Iterable[int]]) -> List[str]:
         if isinstance(integers, np.ndarray) and integers.ndim != 1:
             raise TokenIDConverterError(
                 f"Must be 1 dim ndarray, but got {integers.ndim}")
         return [self.token_list[i] for i in integers]
 
     def tokens2ids(self, tokens: Iterable[str]) -> List[int]:
-        token2id = {v: i for i, v in enumerate(self.token_list)}
-        if self.unk_symbol not in token2id:
-            raise TokenIDConverterError(
-                f"Unknown symbol '{self.unk_symbol}' doesn't exist in the token_list"
-            )
-        unk_id = token2id[self.unk_symbol]
-        return [token2id.get(i, unk_id) for i in tokens]
+
+        return [self.token2id.get(i, self.unk_id) for i in tokens]
 
 
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
@@ -130,15 +127,15 @@
 
     with open(str(yaml_path), 'rb') as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
 
 
 @functools.lru_cache()
-def get_logger(name='torch_paraformer'):
+def get_logger(name='funasr_torch'):
     """Initialize and get a logger by name.
     If the logger has not been initialized, this method will initialize the
     logger by adding one or two handlers, otherwise the initialized logger will
     be directly returned. During initialization, a StreamHandler will always be
     added.
     Args:
         name (str): Logger name.
```

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/setup.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         readme = f.read()
     return readme
 
 
 
 setuptools.setup(
     name='funasr_torch',
-    version='0.0.3',
+    version='0.0.4',
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab, Alibaba Group, China",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license="The MIT License",
     long_description=get_readme(),
```

### Comparing `funasr-0.3.1/funasr/runtime/python/libtorch/test_rtf.py` & `funasr-0.4.1/funasr/runtime/python/libtorch/test_rtf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #from torch_paraformer import Paraformer
-from rapid_paraformer import Paraformer
+from funasr_torch import Paraformer
 import time
 
-model_dir = "/home/gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch"
+model_dir = "/home/gzf/FunASR/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch"
 #model_dir ="/home/gzf/workspace/amp_int8/libtorch_fb20"
 #model_dir ="/home/gzf/workspace/amp_int8/onnx_dynamic"
-model = Paraformer(model_dir, batch_size=1, device_id="-1")
+model = Paraformer(model_dir, batch_size=1, device_id=0)
 
-wav_path = ["/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav", "/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav"]
-wav_path = ["/home/gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav"]
+wav_path = ["/home/gzf/FunASR/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav"]
 
 total = 0.0
 num = 100
 result = model(wav_path)
 for i in range(num):
   beg_time = time.time()
   result = model(wav_path)
```

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 class Paraformer():
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
-                 pred_bias: int = 1,
                  quantize: bool = False,
                  intra_op_num_threads: int = 4,
                  ):
 
         if not Path(model_dir).exists():
             raise FileNotFoundError(f'{model_dir} does not exist.')
 
@@ -43,15 +42,18 @@
         self.frontend = WavFrontend(
             cmvn_file=cmvn_file,
             **config['frontend_conf']
         )
         self.ort_infer = OrtInferSession(model_file, device_id, intra_op_num_threads=intra_op_num_threads)
         self.batch_size = batch_size
         self.plot_timestamp_to = plot_timestamp_to
-        self.pred_bias = pred_bias
+        if "predictor_bias" in config['model_conf'].keys():
+            self.pred_bias = config['model_conf']['predictor_bias']
+        else:
+            self.pred_bias = 0
 
     def __call__(self, wav_content: Union[str, np.ndarray, List[str]], **kwargs) -> List:
         waveform_list = self.load_data(wav_content, self.frontend.opts.frame_opts.samp_freq)
         waveform_nums = len(waveform_list)
         asr_res = []
         for beg_idx in range(0, waveform_nums, self.batch_size):
```

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,48 +20,33 @@
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
         check_argument_types()
 
-        # self.token_list = self.load_token(token_path)
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
+        self.token2id = {v: i for i, v in enumerate(self.token_list)}
+        self.unk_id = self.token2id[self.unk_symbol]
 
-    # @staticmethod
-    # def load_token(file_path: Union[Path, str]) -> List:
-    #     if not Path(file_path).exists():
-    #         raise TokenIDConverterError(f'The {file_path} does not exist.')
-    #
-    #     with open(str(file_path), 'rb') as f:
-    #         token_list = pickle.load(f)
-    #
-    #     if len(token_list) != len(set(token_list)):
-    #         raise TokenIDConverterError('The Token exists duplicated symbol.')
-    #     return token_list
 
     def get_num_vocabulary_size(self) -> int:
         return len(self.token_list)
 
     def ids2tokens(self,
                    integers: Union[np.ndarray, Iterable[int]]) -> List[str]:
         if isinstance(integers, np.ndarray) and integers.ndim != 1:
             raise TokenIDConverterError(
                 f"Must be 1 dim ndarray, but got {integers.ndim}")
         return [self.token_list[i] for i in integers]
 
     def tokens2ids(self, tokens: Iterable[str]) -> List[int]:
-        token2id = {v: i for i, v in enumerate(self.token_list)}
-        if self.unk_symbol not in token2id:
-            raise TokenIDConverterError(
-                f"Unknown symbol '{self.unk_symbol}' doesn't exist in the token_list"
-            )
-        unk_id = token2id[self.unk_symbol]
-        return [token2id.get(i, unk_id) for i in tokens]
+
+        return [self.token2id.get(i, self.unk_id) for i in tokens]
 
 
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
@@ -184,15 +169,15 @@
                           'https://onnxruntime.ai/docs/execution-providers/CUDA-ExecutionProvider.html',
                           RuntimeWarning)
 
     def __call__(self,
                  input_content: List[Union[np.ndarray, np.ndarray]]) -> np.ndarray:
         input_dict = dict(zip(self.get_input_names(), input_content))
         try:
-            return self.session.run(None, input_dict)
+            return self.session.run(self.get_output_names(), input_dict)
         except Exception as e:
             raise ONNXRuntimeError('ONNXRuntime inferece failed.') from e
 
     def get_input_names(self, ):
         return [v.name for v in self.session.get_inputs()]
 
     def get_output_names(self,):
@@ -211,26 +196,58 @@
     def _verify_model(model_path):
         model_path = Path(model_path)
         if not model_path.exists():
             raise FileNotFoundError(f'{model_path} does not exists.')
         if not model_path.is_file():
             raise FileExistsError(f'{model_path} is not a file.')
 
+def split_to_mini_sentence(words: list, word_limit: int = 20):
+    assert word_limit > 1
+    if len(words) <= word_limit:
+        return [words]
+    sentences = []
+    length = len(words)
+    sentence_len = length // word_limit
+    for i in range(sentence_len):
+        sentences.append(words[i * word_limit:(i + 1) * word_limit])
+    if length % word_limit > 0:
+        sentences.append(words[sentence_len * word_limit:])
+    return sentences
+
+def code_mix_split_words(text: str):
+    words = []
+    segs = text.split()
+    for seg in segs:
+        # There is no space in seg.
+        current_word = ""
+        for c in seg:
+            if len(c.encode()) == 1:
+                # This is an ASCII char.
+                current_word += c
+            else:
+                # This is a Chinese char.
+                if len(current_word) > 0:
+                    words.append(current_word)
+                    current_word = ""
+                words.append(c)
+        if len(current_word) > 0:
+            words.append(current_word)
+    return words
 
 def read_yaml(yaml_path: Union[str, Path]) -> Dict:
     if not Path(yaml_path).exists():
         raise FileExistsError(f'The {yaml_path} does not exist.')
 
     with open(str(yaml_path), 'rb') as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
 
 
 @functools.lru_cache()
-def get_logger(name='rapdi_paraformer'):
+def get_logger(name='funasr_onnx'):
     """Initialize and get a logger by name.
     If the logger has not been initialized, this method will initialize the
     logger by adding one or two handlers, otherwise the initialized logger will
     be directly returned. During initialization, a StreamHandler will always be
     added.
     Args:
         name (str): Logger name.
```

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/infer_onnx.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/infer_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.4.1/funasr/runtime/python/onnxruntime/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.2'
+VERSION_NUM = '0.0.5'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab, Alibaba Group, China",
```

### Comparing `funasr-0.3.1/funasr/samplers/build_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/samplers/folded_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/samplers/length_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.4.1/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/schedulers/abs_scheduler.py` & `funasr-0.4.1/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/schedulers/noam_lr.py` & `funasr-0.4.1/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.4.1/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/schedulers/warmup_lr.py` & `funasr-0.4.1/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/tasks/abs_task.py` & `funasr-0.4.1/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,14 +460,20 @@
         )
         group.add_argument(
             "--max_update",
             type=int,
             default=sys.maxsize,
             help="The maximum number update step to train",
         )
+        parser.add_argument(
+            "--batch_interval",
+            type=int,
+            default=10000,
+            help="The batch interval for saving model.",
+        )
         group.add_argument(
             "--patience",
             type=int_or_none,
             default=None,
             help="Number of epochs to wait without improvement "
                  "before stopping the training",
         )
@@ -1351,23 +1357,23 @@
                 )
 
             # 7. Build iterator factories
             if args.dataset_type == "large":
                 from funasr.datasets.large_datasets.build_dataloader import ArkDataLoader
                 train_iter_factory = ArkDataLoader(args.train_data_file, args.token_list, args.dataset_conf,
                                                    frontend_conf=args.frontend_conf if hasattr(args, "frontend_conf") else None,
-                                                   seg_dict_file=args.seg_dict_file if hasattr(args,
-                                                                                               "seg_dict_file") else None,
+                                                   seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
                                                    punc_dict_file=args.punc_list if hasattr(args, "punc_list") else None,
+                                                   bpemodel_file=args.bpemodel if hasattr(args, "bpemodel") else None,
                                                    mode="train")
                 valid_iter_factory = ArkDataLoader(args.valid_data_file, args.token_list, args.dataset_conf, 
                                                    frontend_conf=args.frontend_conf if hasattr(args, "frontend_conf") else None,
-                                                   seg_dict_file=args.seg_dict_file if hasattr(args,
-                                                                                               "seg_dict_file") else None,
+                                                   seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
                                                    punc_dict_file=args.punc_list if hasattr(args, "punc_list") else None,
+                                                   bpemodel_file=args.bpemodel if hasattr(args, "bpemodel") else None,
                                                    mode="eval")
             elif args.dataset_type == "small":
                 train_iter_factory = cls.build_iter_factory(
                     args=args,
                     distributed_option=distributed_option,
                     mode="train",
                 )
@@ -1572,21 +1578,29 @@
 
     @classmethod
     def build_sequence_iter_factory(
             cls, args: argparse.Namespace, iter_options: IteratorOptions, mode: str
     ) -> AbsIterFactory:
         assert check_argument_types()
 
+        if hasattr(args, "frontend_conf"):
+            if args.frontend_conf is not None and "fs" in args.frontend_conf:
+                dest_sample_rate = args.frontend_conf["fs"]
+            else:
+                dest_sample_rate = 16000
+        else:
+            dest_sample_rate = 16000
+
         dataset = ESPnetDataset(
             iter_options.data_path_and_name_and_type,
             float_dtype=args.train_dtype,
             preprocess=iter_options.preprocess_fn,
             max_cache_size=iter_options.max_cache_size,
             max_cache_fd=iter_options.max_cache_fd,
-            dest_sample_rate=args.frontend_conf["fs"],
+            dest_sample_rate=dest_sample_rate,
         )
         cls.check_task_requirements(
             dataset, args.allow_variable_data_keys, train=iter_options.train
         )
 
         if Path(
                 Path(iter_options.data_path_and_name_and_type[0][0]).parent, "utt2category"
```

### Comparing `funasr-0.3.1/funasr/tasks/asr.py` & `funasr-0.4.1/funasr/tasks/asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,20 +408,14 @@
         )
         parser.add_argument(
             "--noise_db_range",
             type=str,
             default="13_15",
             help="The range of noise decibel level.",
         )
-        parser.add_argument(
-            "--batch_interval",
-            type=int,
-            default=10000,
-            help="The batch interval for saving model.",
-        )
 
         for class_choices in cls.class_choices_list:
             # Append --<name> and --<name>_conf.
             # e.g. --encoder and --encoder_conf
             class_choices.add_arguments(group)
 
     @classmethod
```

### Comparing `funasr-0.3.1/funasr/tasks/data2vec.py` & `funasr-0.4.1/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/tasks/diar.py` & `funasr-0.4.1/funasr/tasks/diar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+Author: Speech Lab, Alibaba Group, China
+SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
+https://arxiv.org/abs/2211.10243
+TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
+https://arxiv.org/abs/2303.05397
+"""
+
 import argparse
 import logging
 import os
 from pathlib import Path
 from typing import Callable
 from typing import Collection
 from typing import Dict
```

### Comparing `funasr-0.3.1/funasr/tasks/lm.py` & `funasr-0.4.1/funasr/tasks/lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.lm.abs_model import AbsLM
-from funasr.lm.espnet_model import ESPnetLanguageModel
+from funasr.lm.abs_model import LanguageModel
 from funasr.lm.seq_rnn_lm import SequentialRNNLM
 from funasr.lm.transformer_lm import TransformerLM
 from funasr.tasks.abs_task import AbsTask
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
@@ -79,15 +79,15 @@
                 "kaiming_normal",
                 None,
             ],
         )
         group.add_argument(
             "--model_conf",
             action=NestedDictAction,
-            default=get_default_kwargs(ESPnetLanguageModel),
+            default=get_default_kwargs(LanguageModel),
             help="The keyword arguments for model class.",
         )
 
         group = parser.add_argument_group(description="Preprocess related")
         group.add_argument(
             "--use_preprocessor",
             type=str2bool,
@@ -174,15 +174,15 @@
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         return retval
 
     @classmethod
-    def build_model(cls, args: argparse.Namespace) -> ESPnetLanguageModel:
+    def build_model(cls, args: argparse.Namespace) -> LanguageModel:
         assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # "args" is saved as it is in a yaml file by BaseTask.main().
             # Overwriting token_list to keep it as "portable".
@@ -197,15 +197,15 @@
 
         # 1. Build LM model
         lm_class = lm_choices.get_class(args.lm)
         lm = lm_class(vocab_size=vocab_size, **args.lm_conf)
 
         # 2. Build ESPnetModel
         # Assume the last-id is sos_and_eos
-        model = ESPnetLanguageModel(lm=lm, vocab_size=vocab_size, **args.model_conf)
+        model = LanguageModel(lm=lm, vocab_size=vocab_size, **args.model_conf)
 
         # 3. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
         assert check_return_type(model)
         return model
```

### Comparing `funasr-0.3.1/funasr/tasks/punctuation.py` & `funasr-0.4.1/funasr/tasks/punctuation.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import PuncTrainTokenizerCommonPreprocessor
-from funasr.punctuation.abs_model import AbsPunctuation
-from funasr.punctuation.espnet_model import ESPnetPunctuationModel
-from funasr.punctuation.target_delay_transformer import TargetDelayTransformer
-from funasr.punctuation.vad_realtime_transformer import VadRealtimeTransformer
+from funasr.train.abs_model import AbsPunctuation
+from funasr.train.abs_model import PunctuationModel
+from funasr.models.target_delay_transformer import TargetDelayTransformer
+from funasr.models.vad_realtime_transformer import VadRealtimeTransformer
 from funasr.tasks.abs_task import AbsTask
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.get_default_kwargs import get_default_kwargs
 from funasr.utils.nested_dict_action import NestedDictAction
@@ -75,15 +75,15 @@
                 "kaiming_normal",
                 None,
             ],
         )
         group.add_argument(
             "--model_conf",
             action=NestedDictAction,
-            default=get_default_kwargs(ESPnetPunctuationModel),
+            default=get_default_kwargs(PunctuationModel),
             help="The keyword arguments for model class.",
         )
 
         group = parser.add_argument_group(description="Preprocess related")
         group.add_argument(
             "--use_preprocessor",
             type=str2bool,
@@ -179,15 +179,15 @@
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("vad",)
         return retval
 
     @classmethod
-    def build_model(cls, args: argparse.Namespace) -> ESPnetPunctuationModel:
+    def build_model(cls, args: argparse.Namespace) -> PunctuationModel:
         assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # "args" is saved as it is in a yaml file by BaseTask.main().
             # Overwriting token_list to keep it as "portable".
@@ -214,15 +214,15 @@
         punc_class = punc_choices.get_class(args.punctuation)
         punc = punc_class(vocab_size=vocab_size, punc_size=punc_size, **args.punctuation_conf)
 
         # 2. Build ESPnetModel
         # Assume the last-id is sos_and_eos
         if "punc_weight" in args.model_conf:
             args.model_conf.pop("punc_weight")
-        model = ESPnetPunctuationModel(punc_model=punc, vocab_size=vocab_size, punc_weight=punc_weight_list, **args.model_conf)
+        model = PunctuationModel(punc_model=punc, vocab_size=vocab_size, punc_weight=punc_weight_list, **args.model_conf)
 
         # FIXME(kamo): Should be done in model?
         # 3. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
         assert check_return_type(model)
```

### Comparing `funasr-0.3.1/funasr/tasks/sv.py` & `funasr-0.4.1/funasr/tasks/sv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Author: Speech Lab, Alibaba Group, China
+"""
+
 import argparse
 import logging
 import os
 from pathlib import Path
 from typing import Callable
 from typing import Collection
 from typing import Dict
```

### Comparing `funasr-0.3.1/funasr/tasks/vad.py` & `funasr-0.4.1/funasr/tasks/vad.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from funasr.models.encoder.conformer_encoder import ConformerEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.fused import FusedFrontends
-from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.windowing import SlidingWindow
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.postencoder.hugging_face_transformers_postencoder import (
     HuggingFaceTransformersPostEncoder,  # noqa: H301
 )
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
@@ -77,14 +77,15 @@
     name="frontend",
     classes=dict(
         default=DefaultFrontend,
         sliding_window=SlidingWindow,
         s3prl=S3prlFrontend,
         fused=FusedFrontends,
         wav_frontend=WavFrontend,
+        wav_frontend_online=WavFrontendOnline,
     ),
     type_check=AbsFrontend,
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
     classes=dict(
@@ -287,25 +288,43 @@
         encoder = encoder_class(**args.encoder_conf)
 
         # 5. Build model
         try:
             model_class = model_choices.get_class(args.model)
         except AttributeError:
             model_class = model_choices.get_class("e2evad")
-        model = model_class(encoder=encoder, vad_post_args=args.vad_post_conf)
+        
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+        
+        model = model_class(encoder=encoder, vad_post_args=args.vad_post_conf, frontend=frontend)
 
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
             model_file: Union[Path, str] = None,
             device: str = "cpu",
+            cmvn_file: Union[Path, str] = None,
     ):
         """Build model from the files.
 
         This method is used for inference or fine-tuning.
 
         Args:
             config_file: The yaml file saved when training.
@@ -321,14 +340,16 @@
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
             config_file = Path(config_file)
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
+        #if cmvn_file is not None:
+        args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
```

### Comparing `funasr-0.3.1/funasr/text/build_tokenizer.py` & `funasr-0.4.1/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/char_tokenizer.py` & `funasr-0.4.1/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/cleaner.py` & `funasr-0.4.1/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/korean_cleaner.py` & `funasr-0.4.1/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/phoneme_tokenizer.py` & `funasr-0.4.1/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.4.1/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/token_id_converter.py` & `funasr-0.4.1/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/text/word_tokenizer.py` & `funasr-0.4.1/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.4.1/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/device_funcs.py` & `funasr-0.4.1/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/forward_adaptor.py` & `funasr-0.4.1/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/initialize.py` & `funasr-0.4.1/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.4.1/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/model_summary.py` & `funasr-0.4.1/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/torch_utils/recursive_op.py` & `funasr-0.4.1/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/train/abs_espnet_model.py` & `funasr-0.4.1/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/train/class_choices.py` & `funasr-0.4.1/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/train/distributed_utils.py` & `funasr-0.4.1/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/train/reporter.py` & `funasr-0.4.1/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/train/trainer.py` & `funasr-0.4.1/funasr/train/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,17 +575,18 @@
         assert batch_interval > 0
  
         start_time = time.perf_counter()
         for iiter, (_, batch) in enumerate(
             reporter.measure_iter_time(iterator, "iter_time"), 1
         ):
             assert isinstance(batch, dict), type(batch)
-        
-            if rank == 0 and hasattr(model.module, "num_updates"):
-                num_batch_updates = model.module.get_num_updates()
+
+            if rank == 0:
+                if hasattr(model, "num_updates") or (hasattr(model, "module") and hasattr(model.module, "num_updates")):
+                    num_batch_updates = model.get_num_updates() if hasattr(model,"num_updates") else model.module.get_num_updates()
                 if (num_batch_updates%batch_interval == 0) and (options.oss_bucket is not None) and options.use_pai:
                     buffer = BytesIO()
                     torch.save(model.state_dict(), buffer)
                     options.oss_bucket.put_object(os.path.join(output_dir, f"{num_batch_updates}batch.pth"), buffer.getvalue())
  
             if distributed:
                 torch.distributed.all_reduce(iterator_stop, ReduceOp.SUM)
```

### Comparing `funasr-0.3.1/funasr/utils/asr_env_checking.py` & `funasr-0.4.1/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/asr_utils.py` & `funasr-0.4.1/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/build_dataclass.py` & `funasr-0.4.1/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/cli_utils.py` & `funasr-0.4.1/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/compute_eer.py` & `funasr-0.4.1/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/compute_min_dcf.py` & `funasr-0.4.1/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/compute_wer.py` & `funasr-0.4.1/funasr/utils/compute_wer.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
            rst['Ins'] += out_item['ins']
            rst['Del'] += out_item['del']
            rst['Sub'] += out_item['sub']
            rst['Snt'] += 1
            if out_item['wrong'] > 0:
                rst['wrong_sentences'] += 1
            cer_detail_writer.write(hyp_key + print_cer_detail(out_item) + '\n')
-           cer_detail_writer.write("ref:" + '\t' + "".join(ref_dict[hyp_key]) + '\n')
-           cer_detail_writer.write("hyp:" + '\t' + "".join(hyp_dict[hyp_key]) + '\n')
+           cer_detail_writer.write("ref:" + '\t' + " ".join(list(map(lambda x: x.lower(), ref_dict[hyp_key]))) + '\n')
+           cer_detail_writer.write("hyp:" + '\t' + " ".join(list(map(lambda x: x.lower(), hyp_dict[hyp_key]))) + '\n')
 
     if rst['Wrd'] > 0:
         rst['Err'] = round(rst['wrong_words'] * 100 / rst['Wrd'], 2)
     if rst['Snt'] > 0:
         rst['S.Err'] = round(rst['wrong_sentences'] * 100 / rst['Snt'], 2)
 
     cer_detail_writer.write('\n')
```

### Comparing `funasr-0.3.1/funasr/utils/config_argparse.py` & `funasr-0.4.1/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/get_default_kwargs.py` & `funasr-0.4.1/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/griffin_lim.py` & `funasr-0.4.1/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/job_runner.py` & `funasr-0.4.1/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/misc.py` & `funasr-0.4.1/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/modelscope_param.py` & `funasr-0.4.1/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/nested_dict_action.py` & `funasr-0.4.1/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/postprocess_utils.py` & `funasr-0.4.1/funasr/utils/postprocess_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 alpha_blank = True
                 if time_stamp is not None:
                     ts_flag = True
                     end = time_stamp[i][1] 
                     ts_lists.append([begin, end])
                     begin = end
             else:
-                raise ValueError('invalid character: {}'.format(ch))
+                word_lists.append(ch)
 
     if time_stamp is not None: 
         word_lists, ts_lists = abbr_dispose(word_lists, ts_lists)
         real_word_lists = []
         for ch in word_lists:
             if ch != ' ':
                 real_word_lists.append(ch)
```

### Comparing `funasr-0.3.1/funasr/utils/sized_dict.py` & `funasr-0.4.1/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/timestamp_tools.py` & `funasr-0.4.1/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/types.py` & `funasr-0.4.1/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr/utils/wav_utils.py` & `funasr-0.4.1/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/funasr.egg-info/PKG-INFO` & `funasr-0.4.1/funasr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.3.1
+Version: 0.4.1
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,20 +30,19 @@
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
-| [**Docs_CN**](https://alibaba-damo-academy.github.io/FunASR/cn/index.html)
 | [**Docs_EN**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
 
 
 ## What's new: 
 
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
@@ -52,19 +51,34 @@
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
+Install from pip
+```shell
+pip install -U funasr -i https://pypi.Python.org/simple
+```
+
+Or install from source code
+
+
 ``` sh
-pip install "modelscope[audio_asr]" --upgrade -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html
 git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install --editable ./
+pip install -e ./
 ```
+If you want to use the pretrained models in ModelScope, you should install the modelscope:
+
+```shell
+pip install -U modelscope
+# For the users in China, you could install with the command:
+# pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
+```
+
 For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
 
 ## Usage
 For users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-academy.github.io/FunASR/en/index.html))
 
 ## Contact
```

### Comparing `funasr-0.3.1/funasr.egg-info/SOURCES.txt` & `funasr-0.4.1/funasr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 funasr/bin/lm_calc_perplexity.py
 funasr/bin/lm_inference.py
 funasr/bin/lm_inference_launch.py
 funasr/bin/lm_train.py
 funasr/bin/modelscope_infer.py
 funasr/bin/punc_inference_launch.py
 funasr/bin/punc_train.py
-funasr/bin/punc_train_vadrealtime.py
 funasr/bin/punctuation_infer.py
 funasr/bin/punctuation_infer_vadrealtime.py
 funasr/bin/sond_inference.py
 funasr/bin/sv_inference.py
 funasr/bin/sv_inference_launch.py
 funasr/bin/tokenize_text.py
 funasr/bin/tp_inference.py
@@ -65,31 +64,38 @@
 funasr/datasets/large_datasets/utils/clipping.py
 funasr/datasets/large_datasets/utils/filter.py
 funasr/datasets/large_datasets/utils/low_frame_rate.py
 funasr/datasets/large_datasets/utils/padding.py
 funasr/datasets/large_datasets/utils/tokenize.py
 funasr/export/__init__.py
 funasr/export/export_model.py
-funasr/export/test_onnx.py
-funasr/export/test_torchscripts.py
+funasr/export/models/CT_Transformer.py
 funasr/export/models/__init__.py
 funasr/export/models/e2e_asr_paraformer.py
+funasr/export/models/e2e_vad.py
 funasr/export/models/decoder/__init__.py
 funasr/export/models/decoder/sanm_decoder.py
 funasr/export/models/decoder/transformer_decoder.py
 funasr/export/models/encoder/__init__.py
 funasr/export/models/encoder/conformer_encoder.py
+funasr/export/models/encoder/fsmn_encoder.py
 funasr/export/models/encoder/sanm_encoder.py
 funasr/export/models/modules/__init__.py
 funasr/export/models/modules/decoder_layer.py
 funasr/export/models/modules/encoder_layer.py
 funasr/export/models/modules/feedforward.py
 funasr/export/models/modules/multihead_att.py
 funasr/export/models/predictor/__init__.py
 funasr/export/models/predictor/cif.py
+funasr/export/test/__init__.py
+funasr/export/test/test_onnx.py
+funasr/export/test/test_onnx_punc.py
+funasr/export/test/test_onnx_punc_vadrealtime.py
+funasr/export/test/test_onnx_vad.py
+funasr/export/test/test_torchscripts.py
 funasr/export/torch_quant/__init__.py
 funasr/export/torch_quant/amp_module.py
 funasr/export/torch_quant/graph.py
 funasr/export/torch_quant/module.py
 funasr/export/torch_quant/observed_module.py
 funasr/export/torch_quant/observer.py
 funasr/export/torch_quant/quantizer.py
@@ -117,15 +123,14 @@
 funasr/layers/mask_along_axis.py
 funasr/layers/sinc_conv.py
 funasr/layers/stft.py
 funasr/layers/time_warp.py
 funasr/layers/utterance_mvn.py
 funasr/lm/__init__.py
 funasr/lm/abs_model.py
-funasr/lm/espnet_model.py
 funasr/lm/seq_rnn_lm.py
 funasr/lm/transformer_lm.py
 funasr/losses/__init__.py
 funasr/losses/label_smoothing_loss.py
 funasr/main_funcs/__init__.py
 funasr/main_funcs/average_nbest_models.py
 funasr/main_funcs/calculate_all_attentions.py
@@ -140,14 +145,16 @@
 funasr/models/e2e_asr_paraformer.py
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
 funasr/models/e2e_sv.py
 funasr/models/e2e_tp.py
 funasr/models/e2e_uni_asr.py
 funasr/models/e2e_vad.py
+funasr/models/target_delay_transformer.py
+funasr/models/vad_realtime_transformer.py
 funasr/models/decoder/__init__.py
 funasr/models/decoder/abs_decoder.py
 funasr/models/decoder/contextual_decoder.py
 funasr/models/decoder/rnn_decoder.py
 funasr/models/decoder/sanm_decoder.py
 funasr/models/decoder/sv_decoder.py
 funasr/models/decoder/transformer_decoder.py
@@ -243,42 +250,46 @@
 funasr/modules/streaming_utils/__init__.py
 funasr/modules/streaming_utils/chunk_utilis.py
 funasr/modules/streaming_utils/load_fr_tf.py
 funasr/modules/streaming_utils/utils.py
 funasr/optimizers/__init__.py
 funasr/optimizers/fairseq_adam.py
 funasr/optimizers/sgd.py
-funasr/punctuation/__init__.py
-funasr/punctuation/abs_model.py
-funasr/punctuation/espnet_model.py
-funasr/punctuation/sanm_encoder.py
-funasr/punctuation/target_delay_transformer.py
-funasr/punctuation/text_preprocessor.py
-funasr/punctuation/vad_realtime_transformer.py
 funasr/runtime/__init__.py
 funasr/runtime/python/__init__.py
 funasr/runtime/python/libtorch/__init__.py
 funasr/runtime/python/libtorch/demo.py
+funasr/runtime/python/libtorch/demo_gpu.py
 funasr/runtime/python/libtorch/setup.py
 funasr/runtime/python/libtorch/test_rtf.py
 funasr/runtime/python/libtorch/funasr_torch/__init__.py
 funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
 funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
 funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
 funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
 funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
 funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
 funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
 funasr/runtime/python/onnxruntime/__init__.py
 funasr/runtime/python/onnxruntime/demo.py
+funasr/runtime/python/onnxruntime/demo_gpu.py
+funasr/runtime/python/onnxruntime/demo_punc_offline.py
+funasr/runtime/python/onnxruntime/demo_punc_online.py
+funasr/runtime/python/onnxruntime/demo_vad_offline.py
+funasr/runtime/python/onnxruntime/demo_vad_online.py
 funasr/runtime/python/onnxruntime/infer_onnx.py
 funasr/runtime/python/onnxruntime/setup.py
+funasr/runtime/python/onnxruntime/test_pipeline.py
+funasr/runtime/python/onnxruntime/test_pipeline_online.py
 funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
 funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
 funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
 funasr/samplers/__init__.py
 funasr/samplers/abs_sampler.py
 funasr/samplers/build_batch_sampler.py
@@ -319,14 +330,15 @@
 funasr/torch_utils/load_pretrained_model.py
 funasr/torch_utils/model_summary.py
 funasr/torch_utils/pytorch_version.py
 funasr/torch_utils/recursive_op.py
 funasr/torch_utils/set_all_random_seed.py
 funasr/train/__init__.py
 funasr/train/abs_espnet_model.py
+funasr/train/abs_model.py
 funasr/train/class_choices.py
 funasr/train/distributed_utils.py
 funasr/train/reporter.py
 funasr/train/trainer.py
 funasr/utils/__init__.py
 funasr/utils/asr_env_checking.py
 funasr/utils/asr_utils.py
@@ -344,14 +356,20 @@
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
 funasr/utils/wav_utils.py
 funasr/utils/yaml_no_alias_safe_dump.py
+test/test_moddelscope_punc.py
+test/test_moddelscope_punc_online.py
+test/test_modelscope_paraformer_long.py
+test/test_modelscope_pipeline.py
+test/test_modelscope_vad.py
+test/test_onnx_encoder.py
 test/test_rtf.py
 tests/test_asr_inference_pipeline.py
 tests/test_asr_vad_punc_inference_pipeline.py
 tests/test_inference_pipeline.py
 tests/test_lm_pipeline.py
 tests/test_punctuation_pipeline.py
 tests/test_sv_inference_pipeline.py
```

### Comparing `funasr-0.3.1/funasr.egg-info/requires.txt` & `funasr-0.4.1/funasr.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 setuptools>=38.5.1
-typeguard==2.13.3
+typeguard<=2.13.3
 humanfriendly
 scipy>=1.4.1
 librosa==0.8.1
 jamo==0.4.1
 PyYAML>=5.1.2
 soundfile>=0.10.2
 h5py>=2.10.0
```

### Comparing `funasr-0.3.1/setup.py` & `funasr-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 
 requirements = {
     "install": [
         "setuptools>=38.5.1",
         # "configargparse>=1.2.1",
-        "typeguard==2.13.3",
+        "typeguard<=2.13.3",
         "humanfriendly",
         "scipy>=1.4.1",
         # "filelock",
         "librosa==0.8.1",
         "jamo==0.4.1",  # For kss
         "PyYAML>=5.1.2",
         "soundfile>=0.10.2",
```

### Comparing `funasr-0.3.1/test/test_rtf.py` & `funasr-0.4.1/test/test_rtf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/tests/test_asr_inference_pipeline.py` & `funasr-0.4.1/tests/test_asr_inference_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,22 +39,24 @@
     def test_transformer(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_data2vec_pretrain-zh-cn-aishell2-16k-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://modelscope.oss-cn-beijing.aliyuncs.com/test/audios/asr_example.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "每一天都要快乐喔"
 
     def test_paraformer(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_data2vec_pretrain-paraformer-zh-cn-aishell2-16k')
         rec_result = inference_pipeline(
             audio_in='https://modelscope.oss-cn-beijing.aliyuncs.com/test/audios/asr_example.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "每一天都要快乐喔"
 
 
 class TestMfccaInferencePipelines(unittest.TestCase):
     def test_funasr_path(self):
         import funasr
         import os
         logger.info("run_dir:{0} ; funasr_path: {1}".format(os.getcwd(), funasr.__file__))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funasr-0.3.1/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.4.1/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/tests/test_inference_pipeline.py` & `funasr-0.4.1/tests/test_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/tests/test_lm_pipeline.py` & `funasr-0.4.1/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/tests/test_punctuation_pipeline.py` & `funasr-0.4.1/tests/test_punctuation_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,20 @@
         rec_result = inference_pipeline(text_in=inputs)
         logger.info("punctuation inference result: {0}".format(rec_result))
 
     def test_vadrealtime_inference_pipeline(self):
         inference_pipeline = pipeline(
             task=Tasks.punctuation,
             model='damo/punc_ct-transformer_zh-cn-common-vad_realtime-vocab272727',
-            model_revision="v1.0.0",
         )
         inputs = "跨境河流是养育沿岸|人民的生命之源长期以来为帮助下游地区防灾减灾中方技术人员|在上游地区极为恶劣的自然条件下克服巨大困难甚至冒着生命危险|向印方提供汛期水文资料处理紧急事件中方重视印方在跨境河流问题上的关切|愿意进一步完善双方联合工作机制|凡是|中方能做的我们|都会去做而且会做得更好我请印度朋友们放心中国在上游的|任何开发利用都会经过科学|规划和论证兼顾上下游的利益"
         vads = inputs.split("|")
-        cache_out = []
         rec_result_all = "outputs:"
+        param_dict = {"cache": []}
         for vad in vads:
-            rec_result = inference_pipeline(text_in=vad, cache=cache_out)
-            cache_out = rec_result['cache']
-            rec_result_all += rec_result['text']
+            rec_result = inference_pipeline(text_in=vad, param_dict=param_dict)
+            rec_result_all += rec_result["text"]
         logger.info("punctuation inference result: {0}".format(rec_result_all))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `funasr-0.3.1/tests/test_sv_inference_pipeline.py` & `funasr-0.4.1/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.3.1/tests/test_vad_inference_pipeline.py` & `funasr-0.4.1/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

