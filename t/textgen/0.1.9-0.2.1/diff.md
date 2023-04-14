# Comparing `tmp/textgen-0.1.9.tar.gz` & `tmp/textgen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.1.9.tar", last modified: Wed Apr 12 09:55:05 2023, max compression
+gzip compressed data, was "textgen-0.2.1.tar", last modified: Fri Apr 14 03:39:06 2023, max compression
```

## Comparing `textgen-0.1.9.tar` & `textgen-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.809881 textgen-0.1.9/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.1.9/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    30674 2023-04-12 09:55:05.810717 textgen-0.1.9/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    25881 2023-04-11 07:50:53.000000 textgen-0.1.9/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-12 09:55:05.812715 textgen-0.1.9/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1395 2023-04-12 09:49:33.000000 textgen-0.1.9/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.737362 textgen-0.1.9/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.750356 textgen-0.1.9/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.1.9/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.1.9/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.1.9/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.1.9/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.1.9/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.754473 textgen-0.1.9/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.1.9/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    31686 2023-04-11 15:12:32.000000 textgen-0.1.9/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6228 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.756991 textgen-0.1.9/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.1.9/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    14188 2023-04-12 06:51:22.000000 textgen-0.1.9/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.759489 textgen-0.1.9/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.1.9/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.762844 textgen-0.1.9/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.1.9/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.1.9/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.767938 textgen-0.1.9/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.1.9/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.1.9/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.774012 textgen-0.1.9/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.1.9/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.1.9/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.1.9/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.1.9/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.1.9/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.777513 textgen-0.1.9/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.1.9/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    23061 2023-04-11 14:20:32.000000 textgen-0.1.9/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4853 2023-04-12 05:35:51.000000 textgen-0.1.9/textgen/llama/llama_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.788862 textgen-0.1.9/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.1.9/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73298 2022-09-09 11:41:34.000000 textgen-0.1.9/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18559 2022-06-19 09:29:30.000000 textgen-0.1.9/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.1.9/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.1.9/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.1.9/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10741 2022-06-15 12:49:21.000000 textgen-0.1.9/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.798950 textgen-0.1.9/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.1.9/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.1.9/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.1.9/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50541 2023-02-16 08:10:32.000000 textgen-0.1.9/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.1.9/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.805866 textgen-0.1.9/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.1.9/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.1.9/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.1.9/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.741739 textgen-0.1.9/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    30674 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      145 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.101297 textgen-0.2.1/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.1/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    31932 2023-04-14 03:39:06.101662 textgen-0.2.1/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    26931 2023-04-14 03:27:18.000000 textgen-0.2.1/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-14 03:39:06.102206 textgen-0.2.1/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1419 2023-04-14 03:39:03.000000 textgen-0.2.1/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.051495 textgen-0.2.1/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-14 03:39:03.000000 textgen-0.2.1/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.061156 textgen-0.2.1/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.1/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.1/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.1/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.1/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.1/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.1/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.065210 textgen-0.2.1/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.1/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    31490 2023-04-13 13:14:14.000000 textgen-0.2.1/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.1/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.068221 textgen-0.2.1/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.1/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14437 2023-04-13 13:05:38.000000 textgen-0.2.1/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.069715 textgen-0.2.1/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.1/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.073006 textgen-0.2.1/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.1/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.1/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.076325 textgen-0.2.1/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.1/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.1/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.082343 textgen-0.2.1/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.1/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.1/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.1/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.1/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.1/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.086202 textgen-0.2.1/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.1/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23037 2023-04-13 13:50:42.000000 textgen-0.2.1/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5753 2023-04-13 14:13:30.000000 textgen-0.2.1/textgen/llama/llama_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.093854 textgen-0.2.1/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.1/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73142 2023-04-12 10:22:29.000000 textgen-0.2.1/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.1/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.1/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.1/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.1/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.1/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.098379 textgen-0.2.1/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.1/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.1/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.1/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50541 2023-02-16 08:10:32.000000 textgen-0.2.1/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.1/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.100461 textgen-0.2.1/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.1/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.1/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.1/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.053838 textgen-0.2.1/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    31932 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      158 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.1.9/LICENSE` & `textgen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/PKG-INFO` & `textgen-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.1.9
+Version: 0.2.1
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -48,56 +48,73 @@
         
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
         ## 功能列表
+        
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
+          算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-        - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
-        
+        - [TGLS](textgen/unsup_generation)
+          ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ## Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Introduce|Training|Inference| 
-        |:-- |:--- |:--- |:--- |:--- |
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
+        |Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
         |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
         
         # Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
-        model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+        model trained
+        by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
         
         # Install
         
         ```shell
+        pip install git+https://github.com/huggingface/transformers
+        pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
@@ -107,14 +124,15 @@
         ```
         
         # Usage
         
         ## ChatGLM-6B LoRA 模型
         
         ### 使用ChatGLM-6B LoRA微调后的模型
+        
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import ChatGlmModel
@@ -138,17 +156,23 @@
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import LlamaModel
         
-        model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
-        r = model.predict(["失眠了怎么办？"])
-        print(r)
+        
+        def generate_prompt(instruction):
+            return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+        
+        
+        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+        predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
+        r = model.predict([predict_sentence])
+        print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
         ### 训练LLAMA LoRA模型
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
         ## ConvSeq2Seq 模型
@@ -463,17 +487,19 @@
         
         前10句是真实用户评论，后10句是生成的。
         
         # Dataset
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        3.
+        5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
+           ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
         # Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
```

### Comparing `textgen-0.1.9/README.md` & `textgen-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,56 +40,73 @@
 
 1. 回译（BT, Back Translate）：中文-英文-中文
 2. GPT2模型续写：短文本->长文本
 3. BART摘要模型：长文本->短文本
 4. TGLS：无监督相似文本生成模型
 
 ## 功能列表
+
 - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
 - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-- [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+- [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
+  算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
 - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
 - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
 - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
 - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
 - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-- [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
-
+- [TGLS](textgen/unsup_generation)
+  ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
 
 ## Release Models
 
 release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
 
-|Model|Arch|Introduce|Training|Inference| 
-|:-- |:--- |:--- |:--- |:--- |
-|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
+|Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
+|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
+|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
 |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
+script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
+|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
+script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
+|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
+script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
+script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+|[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
+script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
+script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
 
 # Demo
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
 
 ![](docs/hf.png)
 
 run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
 
 ```shell
 python examples/gradio_demo.py
 ```
 
-model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+model trained
+by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
 
 # Install
 
 ```shell
+pip install git+https://github.com/huggingface/transformers
+pip install git+https://github.com/huggingface/peft
 pip install -U textgen
 ```
 
 or
 
 ```shell
 pip install torch # conda install pytorch
@@ -99,14 +116,15 @@
 ```
 
 # Usage
 
 ## ChatGLM-6B LoRA 模型
 
 ### 使用ChatGLM-6B LoRA微调后的模型
+
 example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
 
 ```python
 import sys
 
 sys.path.append('../..')
 from textgen import ChatGlmModel
@@ -130,17 +148,23 @@
 
 ```python
 import sys
 
 sys.path.append('../..')
 from textgen import LlamaModel
 
-model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
-r = model.predict(["失眠了怎么办？"])
-print(r)
+
+def generate_prompt(instruction):
+    return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+
+
+model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
+r = model.predict([predict_sentence])
+print(r)  # ['地球是唯一一颗拥有生命的行星。']
 ```
 
 ### 训练LLAMA LoRA模型
 
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
 
 ## ConvSeq2Seq 模型
@@ -455,17 +479,19 @@
 
 前10句是真实用户评论，后10句是生成的。
 
 # Dataset
 
 1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+3.
+5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
 4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
+   ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
 
 # Contact
 
 - Issue(建议)
   ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
```

### Comparing `textgen-0.1.9/setup.py` & `textgen-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.1.9',
+    version='0.2.1',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
@@ -29,14 +29,15 @@
         'loguru',
         'jieba>=0.39',
         'transformers',
         'datasets',
         'gensim>=4.0.0',
         'text2vec',
         'tensorboard',
+        'tensorboardX',
         'tqdm>=4.47.0',
         'pandas',
         'wandb>=0.10.32',
         'sacremoses',
         'Rouge',
         'cpm_kernels',
         'peft',
```

### Comparing `textgen-0.1.9/textgen/__init__.py` & `textgen-0.2.1/textgen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.1.9'
+__version__ = '0.2.1'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
```

### Comparing `textgen-0.1.9/textgen/augment/sentence_level_augment.py` & `textgen-0.2.1/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/augment/text_augment.py` & `textgen-0.2.1/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/augment/tokenizer.py` & `textgen-0.2.1/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/augment/translate_api.py` & `textgen-0.2.1/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/augment/word_level_augment.py` & `textgen-0.2.1/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/augment/word_vocab.py` & `textgen-0.2.1/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/chatglm/chatglm_model.py` & `textgen-0.2.1/textgen/chatglm/chatglm_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,24 +101,25 @@
             self.args.int8 = False
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
         config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, **kwargs)
-        if self.device != "cpu":
-            self.model = model_class.from_pretrained(
-                model_name, config=config, trust_remote_code=True, load_in_8bit=self.args.int8).cuda()
-            if self.args.quantization_bit:
-                logger.debug(f"Quantized to {self.args.quantization_bit} bit")
-                self.model = self.model.quantize(self.args.quantization_bit)
-        else:
-            self.model = model_class.from_pretrained(
-                model_name, config=config, trust_remote_code=True).float()
-
+        self.model = model_class.from_pretrained(
+            model_name,
+            config=config,
+            trust_remote_code=True,
+            load_in_8bit=self.args.int8,
+            torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            device_map="auto",
+        )
+        if self.args.quantization_bit:
+            logger.debug(f"Quantized to {self.args.quantization_bit} bit")
+            self.model = self.model.quantize(self.args.quantization_bit)
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
             self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name, trust_remote_code=True)
         else:
             self.tokenizer = tokenizer_class.from_pretrained(model_name, trust_remote_code=True)
             self.args.tokenizer_name = self.args.model_name
 
@@ -135,16 +136,15 @@
         len_ids = [len(example) for example in batch]
         longest = max(len_ids)
         input_ids = []
         labels_list = []
         for ids_l, example in sorted(zip(len_ids, batch), key=lambda x: -x[0]):
             ids = list(example)
             seq_len = ids.index(self.tokenizer.bos_token_id) + 1  # is equal to prompt length
-            ignore_idx = -100
-            labels = ([ignore_idx] * (seq_len - 1) + ids[(seq_len - 1):] + [ignore_idx] * (longest - ids_l))
+            labels = ([-100] * (seq_len - 1) + ids[(seq_len - 1):] + [-100] * (longest - ids_l))
             ids = ids + [self.tokenizer.pad_token_id] * (longest - ids_l)
             _ids = torch.LongTensor(ids)
             labels_list.append(torch.LongTensor(labels))
             input_ids.append(_ids)
         input_ids = torch.stack(input_ids)
         labels = torch.stack(labels_list)
         return {"input_ids": input_ids, "labels": labels}
@@ -345,14 +345,16 @@
                 lora_path = os.path.join(self.args.output_dir, self.args.lora_name)
                 if lora_path and os.path.exists(lora_path):
                     self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
                     logger.info(f"Loaded lora model from {lora_path}")
                     self.lora_loaded = True
             if torch.__version__ >= "2" and sys.platform != "win32":
                 self.model = torch.compile(self.model)
+            if self.args.fp16:
+                self.model.half()
 
     def process_response(self, response):
         response = response.strip().replace("[[训练时间]]", "2023年")
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
@@ -376,15 +378,14 @@
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if not self.lora_loaded:
             self.load_lora()
-        self._move_model_to_device()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
@@ -438,17 +439,14 @@
             for i, (old_query, response) in enumerate(history):
                 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
             prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
         response = self.predict([prompt], keep_prompt=keep_prompt, max_length=len(prompt) + max_length, **kwargs)[0]
         history = history + [(query, response)]
         return response, history
 
-    def _move_model_to_device(self):
-        self.model.to(self.device, dtype=torch.float16 if self.args.fp16 else torch.float32)
-
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
         Creates a ChatGLMDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
```

### Comparing `textgen-0.1.9/textgen/chatglm/chatglm_utils.py` & `textgen-0.2.1/textgen/chatglm/chatglm_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
     dataset = dataset.map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
-        batched=False,
-    ).filter(lambda x: tokenizer.bos_token_id in list(x['input_ids']))  # must contain bos_token_id
+        batched=False, remove_columns=dataset.column_names
+    ).filter(lambda x: tokenizer.gmask_token_id in list(x['input_ids']))  # exclude samples without gmask
 
     dataset.set_format(type="np", columns=["input_ids"])
 
     return dataset["input_ids"]
 
 
 class ChatGlmDataset(Dataset):
```

### Comparing `textgen-0.1.9/textgen/config/global_args.py` & `textgen-0.2.1/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/config/model_args.py` & `textgen-0.2.1/textgen/config/model_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,26 @@
     fp16: bool = False
     gradient_accumulation_steps: int = 1
     learning_rate: float = 2e-5
     local_rank: int = -1
     logging_steps: int = 50
     manual_seed: int = None
     max_grad_norm: float = 1.0
-    max_seq_length: int = 128
+    max_seq_length: int = 128  # max length of input sequence
     model_name: str = None
     model_type: str = None
     multiprocessing_chunksize: int = -1
     n_gpu: int = 1
     no_cache: bool = False
     no_save: bool = False
     not_saved_args: list = field(default_factory=list)
     num_train_epochs: int = 1
     optimizer: str = "AdamW"
     output_dir: str = "outputs/"
-    overwrite_output_dir: bool = False
+    overwrite_output_dir: bool = True
     polynomial_decay_schedule_lr_end: float = 1e-7
     polynomial_decay_schedule_power: float = 1.0
     process_count: int = field(default_factory=get_default_process_count)
     quantized_model: bool = False
     reprocess_input_data: bool = True
     save_best_model: bool = True
     save_eval_checkpoints: bool = True
@@ -149,15 +149,15 @@
 
     model_class: str = "T5Model"
     dataset_class: Dataset = None
     do_sample: bool = False
     early_stopping: bool = True
     evaluate_generated_text: bool = False
     length_penalty: float = 2.0
-    max_length: int = 20
+    max_length: int = 128  # max length of the sequence to be generated
     max_steps: int = -1
     num_beams: int = 1
     num_return_sequences: int = 1
     preprocess_inputs: bool = True
     repetition_penalty: float = 1.0
     scheduler: str = "constant_schedule_with_warmup"
     adafactor_relative_step: bool = False
@@ -179,15 +179,15 @@
 
     model_class: str = "CopyT5Model"
     dataset_class: Dataset = None
     do_sample: bool = False
     early_stopping: bool = True
     evaluate_generated_text: bool = False
     length_penalty: float = 2.0
-    max_length: int = 20
+    max_length: int = 128  # max length of the sequence to be generated
     max_steps: int = -1
     num_beams: int = 3
     num_return_sequences: int = 1
     preprocess_inputs: bool = True
     repetition_penalty: float = 1.0
     scheduler: str = "linear_schedule_with_warmup"
     adafactor_relative_step: bool = False
@@ -243,15 +243,15 @@
     dataset_class: Dataset = None
     do_sample: bool = False
     early_stopping: bool = True
     evaluate_generated_text: bool = False
     faiss_d: int = 768
     faiss_m: int = 128
     length_penalty: float = 2.0
-    max_length: int = 20
+    max_length: int = 128  # max length of the sequence to be generated
     max_steps: int = -1
     num_beams: int = 1
     num_return_sequences: int = 1
     rag_embed_batch_size: int = 16
     repetition_penalty: float = 1.0
     top_k: float = None
     top_p: float = None
@@ -271,15 +271,15 @@
     """
 
     model_class: str = "LanguageGenerationModel"
     do_sample: bool = True
     early_stopping: bool = True
     evaluate_generated_text: bool = False
     length_penalty: float = 2.0
-    max_length: int = 20
+    max_length: int = 128  # max length of the sequence to be generated
     max_steps: int = -1
     num_beams: int = 1
     num_return_sequences: int = 1
     repetition_penalty: float = 1.0
     top_k: float = 50
     top_p: float = 0.95
     prompt: str = ""
@@ -398,14 +398,15 @@
     quantization_bit: int = None  # if use quantization bit, set 4, else None
     debug: bool = False
     max_seq_length: int = 256  # max length of input sequence
     max_length = 384  # max length of the sequence to be generated
     do_sample: bool = True
     early_stopping: bool = True
     evaluate_generated_text: bool = True
+    is_chat_task: bool = True
     warmup_steps: int = 50
     optimizer: str = "adamw_torch"
     save_strategy: str = "steps"
     eval_steps: int = 200
     save_steps: int = 400
     pad_to_multiple_of: int = 8
     max_eval_samples: int = 20
```

### Comparing `textgen-0.1.9/textgen/custom_models/models.py` & `textgen-0.2.1/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/data/HowNetPOSWord.txt` & `textgen-0.2.1/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/data/stopwords.txt` & `textgen-0.2.1/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_generation/language_generation_model.py` & `textgen-0.2.1/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_generation/language_generation_utils.py` & `textgen-0.2.1/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_modeling/language_modeling_model.py` & `textgen-0.2.1/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.2.1/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_modeling/songnet_model.py` & `textgen-0.2.1/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/language_modeling/songnet_utils.py` & `textgen-0.2.1/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/llama/llama_model.py` & `textgen-0.2.1/textgen/llama/llama_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,32 +380,33 @@
             # unwind broken decapoda-research config
             self.tokenizer.padding_side = "left"
             self.model.config.pad_token_id = self.tokenizer.pad_token_id = 0  # unk
             self.model.config.bos_token_id = 1
             self.model.config.eos_token_id = 2
             if torch.__version__ >= "2" and sys.platform != "win32":
                 self.model = torch.compile(self.model)
+            if self.args.fp16:
+                self.model.half()
 
     @torch.no_grad()
     def predict(self, sentences, keep_prompt=False, max_length=None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
-            sentences: A python list of text (str) to be sent to the model for prediction. 
+            sentences: A python list of text (str) to be sent to the model for prediction. Note that the prefix should be prepended to the text.
             keep_prompt: Whether to keep the prompt in the generated text.
             max_length: The maximum length of the generated text.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if not self.lora_loaded:
             self.load_lora()
-        self._move_model_to_device()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
@@ -427,15 +428,15 @@
                 return_dict_in_generate=True,
                 output_scores=True,
                 **kwargs,
             )
             outputs = self.model.generate(**inputs, generation_config=generation_config)
             for idx, (prompt_text, generated_sequence) in enumerate(zip(batch, outputs.sequences)):
                 # Decode text
-                text = self.tokenizer.decode(generated_sequence)
+                text = self.tokenizer.decode(generated_sequence, skip_special_tokens=True)
                 prompt_len = len(prompt_text)
                 gen_text = text[prompt_len:]
                 if keep_prompt:
                     total_sequence = prompt_text + gen_text
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
@@ -462,17 +463,14 @@
             for i, (old_query, response) in enumerate(history):
                 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
             prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
         response = self.predict([prompt], keep_prompt=keep_prompt, max_length=len(prompt) + max_length, **kwargs)[0]
         history = history + [(query, response)]
         return response, history
 
-    def _move_model_to_device(self):
-        self.model.to(self.device, dtype=torch.float16 if self.args.fp16 else torch.float32)
-
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
         Creates a LlamaDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
```

### Comparing `textgen-0.1.9/textgen/llama/llama_utils.py` & `textgen-0.2.1/textgen/llama/llama_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,49 +11,67 @@
 import datasets
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
 from loguru import logger
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
 
+PROMPT_DICT = {
+    "prompt_input": (
+        "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
+        "### Instruction:\n{instruction}\n### Input:\n{input_text}\n\n### Response:"
+    ),
+    "prompt_no_input": (
+        "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
+        "### Instruction:\n{instruction}\n\n### Response:"
+    ),
+}
+
 
 def preprocess_data(data):
     instruction, input_text, target_text, tokenizer, args = data
 
-    prompt = f"问：{instruction}\n"
     if input_text:
-        prompt += f"{input_text}\n"
-    prompt += "答："
-    if target_text:
-        prompt += f"{target_text}"
+        prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
+    else:
+        prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
 
-    full_max_length = args.max_seq_length + args.max_length
+    full_prompt = prompt + target_text + tokenizer.eos_token
     example = tokenizer(
-        prompt,
+        full_prompt,
         truncation=True,
-        max_length=full_max_length,
+        max_length=args.max_seq_length + args.max_length,
         padding=False,
         return_tensors=None,
     )
     if (
             example["input_ids"][-1] != tokenizer.eos_token_id
-            and len(example["input_ids"]) < full_max_length
+            and len(example["input_ids"]) < args.max_seq_length + args.max_length
     ):
         example["input_ids"].append(tokenizer.eos_token_id)
         example["attention_mask"].append(1)
-
     example["labels"] = example["input_ids"].copy()
+    if args.is_chat_task:
+        user_example = tokenizer(
+            prompt,
+            truncation=True,
+            max_length=args.max_seq_length,
+            padding=False,
+            return_tensors=None,
+        )
+        user_prompt_len = len(user_example["input_ids"])
+        example["labels"] = [-100] * user_prompt_len + example["labels"][user_prompt_len:]
 
     return example
 
 
-def preprocess_batch_for_hf_dataset(dataset, tokenizer, args):
-    data = (dataset["instruction"], dataset["input"], dataset["output"], tokenizer, args)
-    dataset = preprocess_data(data)
-    return dataset
+def preprocess_batch_for_hf_dataset(example, tokenizer, args):
+    data = (example["instruction"], example["input"], example["output"], tokenizer, args)
+    example = preprocess_data(data)
+    return example
 
 
 def load_hf_dataset(data, tokenizer, args, mode):
     if isinstance(data, str):
         if data.endswith('.json') or data.endswith('.jsonl'):
             dataset = load_dataset("json", data_files=data)
         elif os.path.isdir(data):
@@ -71,19 +89,17 @@
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
     dataset = dataset.map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
-        batched=False,
+        batched=False, remove_columns=dataset.column_names
     ).filter(lambda x: len(x['input_ids']) > 0)
 
-    dataset.set_format(type="np", columns=["input_ids"])
-
     return dataset
 
 
 class LlamaDataset(Dataset):
     def __init__(self, tokenizer, args, data, mode):
         cached_features_file = os.path.join(
             args.cache_dir,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `textgen-0.1.9/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.2.1/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,32 +4,24 @@
 @description: refer https://github.com/ThilinaRajapakse/simpletransformers
 """
 import math
 import os
 import random
 import warnings
 from dataclasses import asdict
-from multiprocessing import Pool, cpu_count
+from multiprocessing import Pool
 
 import numpy as np
 import pandas as pd
 import torch
+from datasets import load_from_disk
+from loguru import logger
+from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from torch.utils.tensorboard import SummaryWriter
-from torch.utils.data import DataLoader, Dataset, RandomSampler, SequentialSampler
-from torch.utils.data.distributed import DistributedSampler
 from tqdm.auto import tqdm, trange
-from transformers.optimization import (
-    get_constant_schedule,
-    get_constant_schedule_with_warmup,
-    get_linear_schedule_with_warmup,
-    get_cosine_schedule_with_warmup,
-    get_cosine_with_hard_restarts_schedule_with_warmup,
-    get_polynomial_decay_schedule_with_warmup,
-)
-from transformers.optimization import AdamW, Adafactor
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoTokenizer,
     BartConfig,
     BartForConditionalGeneration,
     BartTokenizerFast,
@@ -41,38 +33,42 @@
     BertTokenizerFast,
     DistilBertConfig,
     DistilBertModel,
     DistilBertTokenizerFast,
     ElectraConfig,
     ElectraModel,
     ElectraTokenizerFast,
-    EncoderDecoderConfig,
     EncoderDecoderModel,
     LongformerConfig,
     LongformerModel,
     LongformerTokenizerFast,
     MarianConfig,
     MarianMTModel,
     MarianTokenizer,
     MobileBertConfig,
     MobileBertModel,
     MobileBertTokenizerFast,
-    PreTrainedModel,
-    PreTrainedTokenizerFast,
     RagTokenizer,
     RagRetriever,
     RagTokenForGeneration,
     RagSequenceForGeneration,
     RagConfig,
     RobertaConfig,
     RobertaModel,
     RobertaTokenizerFast,
 )
-from datasets import load_from_disk
-from loguru import logger
+from transformers.optimization import AdamW, Adafactor
+from transformers.optimization import (
+    get_constant_schedule,
+    get_constant_schedule_with_warmup,
+    get_linear_schedule_with_warmup,
+    get_cosine_schedule_with_warmup,
+    get_cosine_with_hard_restarts_schedule_with_warmup,
+    get_polynomial_decay_schedule_with_warmup,
+)
 
 from textgen.config.model_args import Seq2SeqArgs
 from textgen.seq2seq.bart_seq2seq_utils import (
     Seq2SeqDataset,
     SimpleSummarizationDataset,
     add_faiss_index_to_dataset,
     generate_faiss_index_dataset,
```

### Comparing `textgen-0.1.9/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.2.1/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             max_length=args.max_seq_length,
             padding="max_length",
             return_tensors="pt",
             truncation=True,
         )
         target_inputs = encoder_tokenizer.generator(
             target_text,
-            max_length=args.max_seq_length,
+            max_length=args.max_length,
             padding="max_length",
             return_tensors="pt",
             truncation=True,
         )
         source_ids = source_inputs["input_ids"].squeeze()
         target_ids = target_inputs["input_ids"].squeeze()
         src_mask = source_inputs["attention_mask"].squeeze()
@@ -225,15 +225,15 @@
             padding="max_length",
             return_tensors="pt",
             truncation=True,
         )
 
         target_text = decoder_tokenizer.encode(
             target_text,
-            max_length=args.max_seq_length,
+            max_length=args.max_length,
             padding="max_length",
             return_tensors="pt",
             truncation=True,
         )
         return (torch.flatten(input_text), torch.flatten(target_text))
 
 
@@ -308,15 +308,15 @@
         padding="max_length",
         return_tensors="pt",
         truncation=True,
     )
 
     target_ids = tokenizer.batch_encode_plus(
         [target_text],
-        max_length=args.max_seq_length,
+        max_length=args.max_length,
         padding="max_length",
         return_tensors="pt",
         truncation=True,
     )
 
     return {
         "source_ids": input_ids["input_ids"].squeeze(),
@@ -330,14 +330,15 @@
 
     tokenized_example = tokenizer.prepare_seq2seq_batch(
         src_texts=[input_text],
         tgt_texts=[target_text],
         src_lang=args.src_lang,
         tgt_lang=args.tgt_lang,
         max_length=args.max_seq_length,
+        max_target_length=args.max_length,
         padding="max_length",  # pad_to_max_length=True won't work in this case
         return_tensors="pt",
         truncation=True,
     )
 
     decoder_input_ids = tokenized_example["labels"].clone()
     decoder_input_ids = shift_tokens_right(
```

### Comparing `textgen-0.1.9/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.2.1/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/seq2seq/data_reader.py` & `textgen-0.2.1/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/seq2seq/seq2seq_model.py` & `textgen-0.2.1/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.2.1/textgen/seq2seq/seq2seq_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,14 @@
         if self.config.pad_token_id is None and self.config.eos_token_id is not None:
             logger.warning(
                 f"The `config.pad_token_id` is `None`. Using `config.eos_token_id` = {self.config.eos_token_id} for padding.."
             )
 
         if self.args.label_smoothing == 0:
             self.loss_fn = torch.nn.CrossEntropyLoss(ignore_index=self.config.pad_token_id)
-        else:
-            # dynamically import label_smoothed_nll_loss
-            from utils import label_smoothed_nll_loss
-
-            self.loss_fn = label_smoothed_nll_loss
 
     def create_optimizer_and_scheduler(self, num_training_steps: int):
         """
         Setup the optimizer and the learning rate scheduler.
 
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
         Trainer's init through :obj:`optimizers`, or subclass and override this method in a subclass.
```

### Comparing `textgen-0.1.9/textgen/t5/copyt5_model.py` & `textgen-0.2.1/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/t5/copyt5_utils.py` & `textgen-0.2.1/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/t5/t5_model.py` & `textgen-0.2.1/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/t5/t5_utils.py` & `textgen-0.2.1/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/unsup_generation/tgls_model.py` & `textgen-0.2.1/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen/unsup_generation/tgls_util.py` & `textgen-0.2.1/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.9/textgen.egg-info/PKG-INFO` & `textgen-0.2.1/textgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.1.9
+Version: 0.2.1
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -48,56 +48,73 @@
         
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
         ## 功能列表
+        
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
+          算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-        - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
-        
+        - [TGLS](textgen/unsup_generation)
+          ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ## Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Introduce|Training|Inference| 
-        |:-- |:--- |:--- |:--- |:--- |
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
+        |Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
         |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
+        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
+        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
         
         # Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
-        model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+        model trained
+        by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
         
         # Install
         
         ```shell
+        pip install git+https://github.com/huggingface/transformers
+        pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
@@ -107,14 +124,15 @@
         ```
         
         # Usage
         
         ## ChatGLM-6B LoRA 模型
         
         ### 使用ChatGLM-6B LoRA微调后的模型
+        
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import ChatGlmModel
@@ -138,17 +156,23 @@
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import LlamaModel
         
-        model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
-        r = model.predict(["失眠了怎么办？"])
-        print(r)
+        
+        def generate_prompt(instruction):
+            return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+        
+        
+        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+        predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
+        r = model.predict([predict_sentence])
+        print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
         ### 训练LLAMA LoRA模型
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
         ## ConvSeq2Seq 模型
@@ -463,17 +487,19 @@
         
         前10句是真实用户评论，后10句是生成的。
         
         # Dataset
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        3.
+        5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
+           ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
         # Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
```

### Comparing `textgen-0.1.9/textgen.egg-info/SOURCES.txt` & `textgen-0.2.1/textgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

