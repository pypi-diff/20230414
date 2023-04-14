# Comparing `tmp/molgraph-0.2.4.tar.gz` & `tmp/molgraph-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.2.4.tar", last modified: Thu Apr  6 16:43:27 2023, max compression
+gzip compressed data, was "molgraph-0.3.0.tar", last modified: Fri Apr 14 13:04:52 2023, max compression
```

## Comparing `molgraph-0.2.4.tar` & `molgraph-0.3.0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.2.4/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-06 16:43:27.387179 molgraph-0.2.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2402 2022-09-20 11:35:03.000000 molgraph-0.2.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-04-06 16:42:38.000000 molgraph-0.2.4/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.2.4/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.2.4/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.2.4/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.2.4/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.2.4/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.2.4/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3221 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.2.4/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.2.4/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12913 2022-09-14 12:21:47.000000 molgraph-0.2.4/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.2.4/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7748 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.2.4/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.2.4/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.2.4/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10904 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6486 2022-09-02 12:17:48.000000 molgraph-0.2.4/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.2.4/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.2.4/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.2.4/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.2.4/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.2.4/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.2.4/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11055 2022-08-31 15:11:51.000000 molgraph-0.2.4/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9439 2022-09-14 10:36:59.000000 molgraph-0.2.4/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11842 2022-08-31 15:11:51.000000 molgraph-0.2.4/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2022-08-18 17:06:18.000000 molgraph-0.2.4/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20437 2022-08-31 15:11:51.000000 molgraph-0.2.4/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.2.4/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.2.4/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.2.4/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.2.4/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.2.4/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.2.4/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.2.4/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.2.4/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.2.4/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.2.4/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7338 2023-04-06 15:41:44.000000 molgraph-0.2.4/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8254 2023-04-06 15:41:44.000000 molgraph-0.2.4/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.2.4/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.2.4/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.2.4/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6937 2023-04-06 15:39:26.000000 molgraph-0.2.4/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.387179 molgraph-0.2.4/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.2.4/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.2.4/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.2.4/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    34971 2022-09-20 10:07:50.000000 molgraph-0.2.4/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-06 16:43:27.383180 molgraph-0.2.4/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-06 16:43:27.000000 molgraph-0.2.4/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2881 2023-04-06 16:43:27.000000 molgraph-0.2.4/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-06 16:43:27.000000 molgraph-0.2.4/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-04-06 16:43:27.000000 molgraph-0.2.4/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-04-06 16:43:27.000000 molgraph-0.2.4/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-06 16:43:27.387179 molgraph-0.2.4/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.2.4/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-14 13:04:52.577366 molgraph-0.3.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2402 2022-09-20 11:35:03.000000 molgraph-0.3.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.569366 molgraph-0.3.0/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.0/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.0/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.0/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.0/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.0/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.0/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.0/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3345 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.0/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11266 2022-09-02 16:19:13.000000 molgraph-0.3.0/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9279 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11313 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10527 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14948 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12894 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.0/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9916 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9754 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7748 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10599 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.0/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.0/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9441 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10267 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.0/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15618 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6486 2022-09-02 12:17:48.000000 molgraph-0.3.0/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.0/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.0/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.573366 molgraph-0.3.0/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.0/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1987 2022-08-18 17:05:36.000000 molgraph-0.3.0/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.0/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.0/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11055 2022-08-31 15:11:51.000000 molgraph-0.3.0/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9439 2022-09-14 10:36:59.000000 molgraph-0.3.0/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11842 2022-08-31 15:11:51.000000 molgraph-0.3.0/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2022-08-18 17:06:18.000000 molgraph-0.3.0/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20437 2022-08-31 15:11:51.000000 molgraph-0.3.0/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.0/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.0/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.0/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.0/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.0/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.0/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.0/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.0/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.0/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.0/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.0/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.0/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.0/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.577366 molgraph-0.3.0/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.0/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.0/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.0/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35151 2023-04-14 12:58:07.000000 molgraph-0.3.0/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-14 13:04:52.569366 molgraph-0.3.0/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-04-14 13:04:52.000000 molgraph-0.3.0/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2966 2023-04-14 13:04:52.000000 molgraph-0.3.0/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-14 13:04:52.000000 molgraph-0.3.0/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-04-14 13:04:52.000000 molgraph-0.3.0/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-04-14 13:04:52.000000 molgraph-0.3.0/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-14 13:04:52.577366 molgraph-0.3.0/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.0/setup.py
```

### Comparing `molgraph-0.2.4/LICENSE` & `molgraph-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/PKG-INFO` & `molgraph-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.2.4
+Version: 0.3.0
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.2.4/README.md` & `molgraph-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/_filter_warnings.py` & `molgraph-0.3.0/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/__init__.py` & `molgraph-0.3.0/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.0/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.0/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.0/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.0/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.0/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.0/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/encoders.py` & `molgraph-0.3.0/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/features.py` & `molgraph-0.3.0/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.0/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/ops.py` & `molgraph-0.3.0/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/chemistry/vis.py` & `molgraph-0.3.0/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/__init__.py` & `molgraph-0.3.0/molgraph/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from molgraph.layers.convolutional.gin_conv import GINConv
 from molgraph.layers.convolutional.gcnii_conv import GCNIIConv
 
 from molgraph.layers.geometric.gcf_conv import GCFConv
 from molgraph.layers.geometric.dtnn_conv import DTNNConv
 
 from molgraph.layers.message_passing.mpnn_conv import MPNNConv
+from molgraph.layers.message_passing.edge_conv import EdgeConv
 
 # readout
 from molgraph.layers.readout.segment_pool import SegmentPoolingReadout
 from molgraph.layers.readout.set_gather import SetGatherReadout
 from molgraph.layers.readout.transformer_encoder import TransformerEncoderReadout
+from molgraph.layers.readout.node_readout import NodeReadout
 
 # positional encoding
 from molgraph.layers.positional_encoding.laplacian import LaplacianPositionalEncoding
 
 # postprocessing
 from molgraph.layers.postprocessing.dot_product_incident import DotProductIncident
 from molgraph.layers.postprocessing.gather_incident import GatherIncident
```

### Comparing `molgraph-0.2.4/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.0/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.0/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.0/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.0/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.0/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/base.py` & `molgraph-0.3.0/molgraph/layers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Config = TypeVar('Config', bound=dict)
 Activation = Optional[Union[Callable[[tf.Tensor], tf.Tensor], str]]
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class BaseLayer(layers.Layer, ABC):
 
-    'Only meant to be a base layer for the built-in GNN layers.'
+    'Base layer for the built-in GNN layers.'
 
     def __init__(
         self,
         units: Optional[int] = None,
         batch_norm: bool = False,
         residual: bool = False,
         dropout: Optional[float] = None,
```

### Comparing `molgraph-0.2.4/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.0/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.0/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.0/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.0/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.0/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.0/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.0/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.0/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,277 +1,247 @@
 import tensorflow as tf
 from tensorflow import keras
+from tensorflow.keras import layers
 from tensorflow.keras import initializers
 from tensorflow.keras import regularizers
 from tensorflow.keras import constraints
 from tensorflow.keras import activations
-from tensorflow.keras import layers
-import math
 
 from typing import Optional
-from typing import Callable
 from typing import Union
-from typing import Tuple
+from typing import List
 
 from molgraph.tensors.graph_tensor import GraphTensor
-from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import compute_edge_weights_from_degrees
-from molgraph.layers.ops import propagate_node_features
-
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class MPNNConv(BaseLayer):
-
-    """Message passing neural network layer (MPNN)
+class EmbeddingLookup(layers.StringLookup):
 
-    Implementation is based on Gilmer et al. (2017) [#]_. In contrast to Gilmer
-    et al. this implementation does not use weight tying; for neither the message
-    function nor the update function. Furthermore, instead of the GRU-based
-    update function, here, a simple fully-connected (dense) layer is used.
+    '''A loookup layer and embedding layer in combination.
 
-    For an MPNN more similar to Gilmer et al., see ``molgraph.models.MPNN``.
+    Specify, as keyword argument only,
+    ``EmbeddingLookup(feature='node_feature')`` to perform standard scaling
+    on the ``node_feature`` field of the ``GraphTensor``, or,
+    ``EmbeddingLookup(feature='edge_feature')`` to perform standard scaling
+    on the ``edge_feature`` field of the ``GraphTensor``. If not specified,
+    the ``node_feature`` field will be considered.
 
     **Examples:**
 
-    Inputs a ``GraphTensor`` encoding (two) subgraphs:
+    Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
-    ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
+    ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
     ...         'node_feature': [
-    ...             [[1.0, 0.0], [1.0, 0.0]],
-    ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
-    ...         ],
-    ...         'edge_feature': [
-    ...             [[1.0, 0.0], [0.0, 1.0]],
-    ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
-    ...              [0.0, 1.0], [1.0, 0.0], [0.0, 1.0]]
+    ...             'Sym:C', 'Sym:C', 'Sym:C', 'Sym:O', 'Sym:N',
     ...         ],
+    ...         'graph_indicator': [0, 0, 1, 1, 1],
     ...     }
     ... )
-    >>> # Build a model with MPNNConv
-    >>> gnn_model = tf.keras.Sequential([
-    ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.MPNNConv(16, activation='relu'),
-    ...     molgraph.layers.MPNNConv(16, activation='relu')
+    >>> # Initialize layer
+    >>> embedding = molgraph.layers.EmbeddingLookup(
+    ...    feature='node_feature', output_dim=4)
+    >>> # Adapt layer to graph_tensor
+    >>> embedding.adapt(graph_tensor)
+    >>> model = tf.keras.Sequential([
+    ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
+    ...     embedding,
     ... ])
-    >>> gnn_model.output_shape
-    (None, None, 16)
+    >>> graph_tensor = model(graph_tensor)
+    >>> graph_tensor.node_feature.shape
+    TensorShape([5, 4])
 
-    Inputs a ``GraphTensor`` encoding a single disjoint graph:
+    Adapt layer on dataset, constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
-    ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [[0, 1], [2, 2, 3, 3, 4, 4]],
+    ...         'edge_src': [[1, 0], [3, 4, 2, 4, 3, 2]],
     ...         'node_feature': [
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0]
-    ...         ],
-    ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         'edge_feature': [
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0]
+    ...             ['Sym:C', 'Sym:C'], ['Sym:C', 'Sym:O', 'Sym:N'],
     ...         ],
     ...     }
     ... )
-    >>> # Build a model with MPNNConv
-    >>> gnn_model = tf.keras.Sequential([
-    ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.MPNNConv(16, activation='relu'),
-    ...     molgraph.layers.MPNNConv(16, activation='relu')
+    >>> # Obtain dataset
+    >>> ds = tf.data.Dataset.from_tensor_slices(graph_tensor).batch(2)
+    >>> # Initialize layer
+    >>> embedding = molgraph.layers.EmbeddingLookup(
+    ...    feature='node_feature', output_dim=4)
+    >>> # Adapt layer to graph_tensor
+    >>> embedding.adapt(ds)
+    >>> # Build model
+    >>> model = tf.keras.Sequential([
+    ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
+    ...     embedding,
     ... ])
-    >>> gnn_model.output_shape
-    (None, 16)
+    >>> # Predict (obtain new GraphTensor)
+    >>> output = model.predict(ds)
+    >>> output.node_feature.shape
+    TensorShape([2, None, 4])
 
     Args:
-        units (int, None):
-            Number of output units.
-        use_edge_features (bool):
-            Whether or not to use edge features. Default to True.
-        self_projection (bool):
-            Whether to apply self projection. Default to True.
-        batch_norm: (bool):
-            Whether to apply batch normalization to the output. Default to True.
-        residual: (bool)
-            Whether to add skip connection to the output. Default to True.
-        dropout: (float, None):
-            Dropout applied to the output of the layer. Default to None.
-        update_activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function used for the update function. Default to None.
-        activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer. Default to 'relu'.
-        use_bias (bool):
-            Whether the layer should use biases. Default to True.
-        kernel_initializer (tf.keras.initializers.Initializer, str):
-            Initializer function for the kernels. Default to
-            tf.keras.initializers.TruncatedNormal(stddev=0.005).
-        bias_initializer (tf.keras.initializers.Initializer, str):
-            Initializer function for the biases. Default to
-            tf.keras.initializers.Constant(0.).
-        kernel_regularizer (tf.keras.regularizers.Regularizer, None):
-            Regularizer function applied to the kernels. Default to None.
-        bias_regularizer (tf.keras.regularizers.Regularizer, None):
-            Regularizer function applied to the biases. Default to None.
-        activity_regularizer (tf.keras.regularizers.Regularizer, None):
-            Regularizer function applied to the final output of the layer.
-            Default to None.
-        kernel_constraint (tf.keras.constraints.Constraint, None):
-            Constraint function applied to the kernels. Default to None.
-        bias_constraint (tf.keras.constraints.Constraint, None):
-            Constraint function applied to the biases. Default to None.
-
-    References:
-        .. [#] https://arxiv.org/pdf/1704.01212.pdf
-
-    """
+        output_dim (int):
+            The output dimension of the embedding layer.
+        input_dim (int, None):
+            The input dimension to the embedding layer. If None, the input
+            dimension is determined by the vocabulary size (obtained from
+            adapting the StringLookup layer to the data). Default to None.
+        embedding_initializer (tf.keras.initializers.Initializer, str):
+            Initializer function for the embedding. Default to ``'uniform'``.
+        embedding_regularizer (tf.keras.regularizers.Regularizer, None):
+            Regularizer function applied to the embedding. Default to None.
+        embedding_constraint (tf.keras.constraints.Constraint, None):
+            Constraint function applied to the embedding. Default to None.
+        max_tokens (int, None):
+            Maximum number of tokens to use. Default to None.
+        num_oov_indices (int):
+            Number of out-of-vocabulary indices to use. Default to 1.
+        mask_token (str):
+            The token that represents masked input. Default to ``'[MASK]'``.
+        oov_token (str):
+            The token that represents out-of-vocabulary input. Default to ``'[UNK]'``.
+        vocabulary (list, None):
+            Optional vocabulary. If None, obtain a vocabulary via the ``adapt()``
+            method. Default to None.
+        **kwargs:
+            Specify the relevant ``feature``. Default to ``node_feature``.
+            The reminaing kwargs are passed to the parent class.
+    '''
 
     def __init__(
         self,
-        units: Optional[int] = None,
-        use_edge_features: bool = True,
-        self_projection: bool = True,
-        batch_norm: bool = True,
-        residual: bool = True,
-        dropout: Optional[float] = None,
-        update_activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
-        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
-        use_bias: bool = True,
-        kernel_initializer: Union[
-            str, initializers.Initializer
-        ] = initializers.TruncatedNormal(stddev=0.005),
-        bias_initializer: Union[
-            str, initializers.Initializer
-        ] = initializers.Constant(0.),
-        kernel_regularizer: Optional[regularizers.Regularizer] = None,
-        bias_regularizer: Optional[regularizers.Regularizer] = None,
-        activity_regularizer: Optional[regularizers.Regularizer] = None,
-        kernel_constraint: Optional[constraints.Constraint] = None,
-        bias_constraint: Optional[constraints.Constraint] = None,
+        output_dim,
+        input_dim: Optional[int] = None,
+        embeddings_initializer: Union[str, initializers.Initializer] = 'uniform',
+        embeddings_regularizer: Optional[regularizers.Regularizer] = None,
+        embeddings_constraint: Optional[constraints.Constraint] = None,
+        max_tokens: Optional[int] = None,
+        num_oov_indices: int = 1,
+        mask_token: str = '[MASK]',
+        oov_token: str = '[UNK]',
+        vocabulary: Optional[List[str]] = None,
         **kwargs
     ):
-        super().__init__(
-            units=units,
-            batch_norm=batch_norm,
-            residual=residual,
-            dropout=dropout,
-            activation=activation,
-            use_bias=use_bias,
-            kernel_initializer=kernel_initializer,
-            bias_initializer=bias_initializer,
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-            activity_regularizer=activity_regularizer,
-            kernel_constraint=kernel_constraint,
-            bias_constraint=bias_constraint,
-            **kwargs)
-
-        self.use_edge_features = use_edge_features
-        self.apply_self_projection = self_projection
-        self.update_activation = update_activation
-
-    def subclass_build(
-        self,
-        node_feature_shape: tf.TensorShape,
-        edge_feature_shape: Optional[tf.TensorShape] = None
-    ) -> None:
-        self.message_projection = self.get_dense(self.units * self.units)
-        self.update_step = keras.layers.Dense(
-            self.units, activation=self.update_activation)
-
-        if (
-            self.units != node_feature_shape[-1] and
-            not hasattr(self, 'node_resample')
-        ):
-            self.node_resample = self.get_dense(self.units)
-
-        if self.apply_self_projection:
-            self.self_projection = self.get_dense(self.units)
-
-    def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
-
-        if hasattr(self, 'node_resample'):
-            tensor = tensor.update({
-                'node_feature': self.node_resample(tensor.node_feature)})
-
-        # MPNN requires edge features, if edge features do not exist,
-        # we force edge features by initializing them as ones vector
-        if not hasattr(tensor, 'edge_feature') or not self.use_edge_features:
-            tensor = tensor.update({
-                'edge_feature': tf.ones(
-                    shape=[tf.shape(tensor.edge_dst)[0], 1], dtype=tf.float32)})
-
-        node_feature_aggregated = message_step(
-            node_feature=tensor.node_feature,
-            edge_feature=tensor.edge_feature,
-            edge_dst=tensor.edge_dst,
-            edge_src=tensor.edge_src,
-            projection=self.message_projection)
-
-        if self.apply_self_projection:
-            node_feature_aggregated += self.self_projection(tensor.node_feature)
+        if 'feature' in kwargs:
+            self.feature = kwargs['feature']
+            del kwargs['feature']
+        elif not hasattr(self, 'feature'):
+            self.feature = 'node_feature'
 
-        node_feature_update = self.update_step(
-            tf.concat([tensor.node_feature, node_feature_aggregated], axis=1))
-
-        return tensor.update({'node_feature': node_feature_update})
+        super().__init__(
+            max_tokens=max_tokens,
+            num_oov_indices=num_oov_indices,
+            mask_token=mask_token,
+            oov_token=oov_token,
+            vocabulary=vocabulary,
+            **kwargs
+        )
+
+        self.output_dim = output_dim
+        self.embeddings_initializer = initializers.get(embeddings_initializer)
+        self.embeddings_regularizer = regularizers.get(embeddings_regularizer)
+        self.embeddings_constraint = constraints.get(embeddings_constraint)
+        self._vocabulary_size = None
+        self._built_from_vocabulary_size = False
+
+    def adapt(self, data, batch_size=None, steps=None):
+        '''Adapts the layer to data.
+
+        When adapting the layer to the data, ``build()`` will be called
+        automatically (to initialize the relevant attributes). After adaption,
+        the layer is finalized and ready to be used.
+
+        Args:
+            data (GraphTensor, tf.data.Dataset):
+                Data to be used to adapt the layer. Can be either a
+                ``GraphTensor`` directly or a ``tf.data.Dataset`` constructed
+                from a ``GraphTensor``.
+            batch_size (int, None):
+                The batch size to be used during adaption. Default to None.
+            steps (int, None):
+                The number of steps of adaption. If None, the number of
+                samples divided by the batch_size is used. Default to None.
+        '''
+        if not isinstance(data,  GraphTensor):
+            data = data = data.map(
+                lambda x: getattr(x, self.feature))
+        else:
+            data = getattr(data, self.feature)
+        super().adapt(data, batch_size=batch_size, steps=steps)
+        self._vocabulary_size = self.vocabulary_size()
+
+    def call(self, tensor: GraphTensor) -> GraphTensor:
+        '''Defines the computation from inputs to outputs.
+
+        This method should not be called directly, but indirectly
+        via ``__call__()``. Upon first call, the layer is automatically
+        built via ``build()``.
+
+        Args:
+            data (GraphTensor):
+                Input to the layer.
+
+        Returns:
+            GraphTensor:
+                A ``GraphTensor`` with updated features. Either the
+                ``node_features`` field or the ``edge_features``
+                field (of the ``GraphTensor``) are updated.
+        '''
+        if not self._built_from_vocabulary_size:
+            self._build_from_vocabulary_size(self._vocabulary_size)
+
+        tensor = tensor.update({
+            self.feature: super().call(getattr(tensor, self.feature))
+        })
+        return tensor.update({
+            self.feature: tf.nn.embedding_lookup(
+                self.embeddings, getattr(tensor, self.feature))
+        })
+
+    def _build_from_vocabulary_size(self, vocabulary_size):
+        self._built_from_vocabulary_size = True
+
+        self.embeddings = self.add_weight(
+            shape=(vocabulary_size, self.output_dim),
+            dtype=tf.float32,
+            initializer=self.embeddings_initializer,
+            name='embeddings',
+            regularizer=self.embeddings_regularizer,
+            constraint=self.embeddings_constraint,
+            experimental_autocast=False
+        )
+
+    @classmethod
+    def from_config(cls, config):
+        vocabulary_size = config.pop('vocabulary_size')
+        layer = cls(**config)
+        if vocabulary_size is None:
+            pass
+        else:
+            layer._build_from_vocabulary_size(vocabulary_size)
+        return layer
 
     def get_config(self):
         base_config = super().get_config()
-        config = {
-            'use_edge_features': self.use_edge_features,
-            'self_projection': self.apply_self_projection,
-            'update_activation': self.update_activation
-        }
-        base_config.update(config)
+        base_config.update({
+            'vocabulary_size': self._vocabulary_size,
+            'output_dim': self.output_dim,
+            'embeddings_initializer': initializers.serialize(
+                self.embeddings_initializer),
+            'embeddings_regularizer': regularizers.serialize(
+                self.embeddings_regularizer),
+            'embeddings_constraint': constraints.serialize(
+                self.embeddings_constraint),
+        })
         return base_config
 
 
-def message_step(
-    node_feature: tf.Tensor,
-    edge_feature: tf.Tensor,
-    edge_dst: tf.Tensor,
-    edge_src: tf.Tensor,
-    projection: keras.layers.Dense,
-) -> tf.Tensor:
-    '''Performs a message passing step.
+@keras.utils.register_keras_serializable(package='molgraph')
+class NodeEmbeddingLookup(EmbeddingLookup):
+    feature = 'node_feature'
 
-    Args:
-        node_feature (tf.Tensor):
-            Node features; field of GraphTensor.
-        edge_feature (tf.Tensor):
-            Edge features; field of GraphTensor.
-        edge_dst (tf.Tensor):
-            Destination node indices; field of GraphTensor.
-        edge_src (tf.Tensor):
-            Source node indices; field of GraphTensor.
-        projection (keras.layers.Dense):
-            Dense layer that transforms edge features.
 
-    Returns (tf.Tensor):
-        Returns updated (aggregated) node features.
-    '''
-    output_units = int(math.sqrt(projection.units))
-    # Apply linear transformation to edge features
-    edge_feature = projection(edge_feature)
-    # Reshape edge features to match source nodes' features
-    edge_feature = tf.reshape(edge_feature, (-1, output_units, output_units))
-    # Obtain source nodes' features (1-hop neighbor nodes)
-    node_feature_src = tf.expand_dims(tf.gather(node_feature, edge_src), -1)
-    # Apply edge features (obtain messages to be passed to destination nodes)
-    messages = tf.squeeze(tf.matmul(edge_feature, node_feature_src), -1)
-    # Send messages to destination nodes
-    return tf.math.unsorted_segment_sum(
-        data=messages,
-        segment_ids=edge_dst,
-        num_segments=tf.shape(node_feature)[0])
+@keras.utils.register_keras_serializable(package='molgraph')
+class EdgeEmbeddingLookup(EmbeddingLookup):
+    feature = 'edge_feature'
```

### Comparing `molgraph-0.2.4/molgraph/layers/ops.py` & `molgraph-0.3.0/molgraph/layers/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.0/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.0/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.0/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.3.0/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.0/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.0/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.0/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.0/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.0/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.0/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.0/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/losses/link_losses.py` & `molgraph-0.3.0/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/losses/masked_losses.py` & `molgraph-0.3.0/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.0/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.0/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/models/dgin.py` & `molgraph-0.3.0/molgraph/models/dgin.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors import GraphTensor
 from molgraph.layers.ops import propagate_node_features
-from molgraph.models.dmpnn import edge_message_passing
+from molgraph.layers.message_passing.edge_conv import edge_message_step
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class DGIN(keras.layers.Layer):
+class DGIN(keras.models.Model):
 
     '''Directed graph isomorphism network (DGIN).
 
     Implementation is based on Wieder et al. (2021) [#]_. 
     
+    **Important:**
+
+    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
+    of molecules with a single atom, please add self loops: 
+    ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
+    
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
@@ -89,14 +95,16 @@
             None if dropout is None else keras.layers.Dropout(dropout))
         self.parallel_iterations = parallel_iterations
         self.dense_kwargs = {} if dense_kwargs is None else dense_kwargs
         self.dense_kwargs.pop('units', None)
         self.dense_kwargs.pop('activaton', None)
 
     def build(self, input_shape: Optional[Tuple[int, ...]] = None) -> None:
+        if not self.units:
+            self.units = input_shape[-1]
         self.initial_projection = keras.layers.Dense(
             self.units, self.activation, **self.dense_kwargs)
         self.update_projection = keras.layers.Dense(
             self.units, **self.dense_kwargs)
         self.node_projection = keras.layers.Dense(
             self.units + input_shape[-1], **self.dense_kwargs)
         self.epsilon = tf.Variable(0.)
@@ -135,16 +143,20 @@
         edge_feature = tf.concat([edge_feature, tensor.edge_feature], axis=-1)
         edge_feature = self.initial_projection(edge_feature)
         
         tensor = tensor.update({'edge_feature': edge_feature})
         
         for _ in range(self.edge_message_steps):
             
-            message = edge_message_passing(
-                tensor, self.parallel_iterations)
+            message = edge_message_step(
+                edge_feature=tensor.edge_feature,
+                edge_src=tensor.edge_src,
+                edge_dst=tensor.edge_dst,
+                graph_indicator=tensor.graph_indicator,
+                parallel_iterations=self.parallel_iterations)
 
             edge_feature = self.activation(
                 self.update_projection(message) + edge_feature)
             
             if self.dropout is not None:
                 edge_feature = self.dropout(edge_feature)
```

### Comparing `molgraph-0.2.4/molgraph/models/dmpnn.py` & `molgraph-0.3.0/molgraph/models/dmpnn.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 from tensorflow import keras
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors import GraphTensor
+from molgraph.layers.message_passing.edge_conv import edge_message_step
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class DMPNN(keras.layers.Layer):
+class DMPNN(keras.models.Model):
 
     '''Directed message passing neural network (DMPNN).
 
     Implementation is based on Yang et al. (2019) [#]_.
 
+    **Important:**
+
+    As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
+    of molecules with a single atom, please add self loops: 
+    ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
+
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
@@ -83,14 +90,16 @@
             None if dropout is None else keras.layers.Dropout(dropout))
         self.parallel_iterations = parallel_iterations
         self.dense_kwargs = {} if dense_kwargs is None else dense_kwargs
         self.dense_kwargs.pop('units', None)
         self.dense_kwargs.pop('activaton', None)
 
     def build(self, input_shape: Optional[Tuple[int, ...]] = None) -> None:
+        if not self.units:
+            self.units = input_shape[-1]
         self.initial_projection = keras.layers.Dense(
             self.units, self.activation, **self.dense_kwargs)
         self.update_projection = keras.layers.Dense(
             self.units, **self.dense_kwargs)
         self.final_projection = keras.layers.Dense(
             self.units, self.activation, **self.dense_kwargs)
         self.built = True
@@ -128,17 +137,21 @@
         edge_feature = tf.concat([edge_feature, tensor.edge_feature], axis=-1)
         edge_feature = self.initial_projection(edge_feature)
         
         tensor = tensor.update({'edge_feature': edge_feature})
         
         for _ in range(self.steps):
             
-            message = edge_message_passing(
-                tensor, self.parallel_iterations)
-
+            message = edge_message_step(
+                edge_feature=tensor.edge_feature,
+                edge_src=tensor.edge_src,
+                edge_dst=tensor.edge_dst,
+                graph_indicator=tensor.graph_indicator,
+                parallel_iterations=self.parallel_iterations)
+    
             edge_feature = self.activation(
                 self.update_projection(message) + edge_feature)
             
             if self.dropout is not None:
                 edge_feature = self.dropout(edge_feature)
 
             # TODO: should skip connection be applied? 
@@ -160,53 +173,8 @@
             'steps': self.steps,
             'dropout': self.dropout,
             'parallel_iterations': self.parallel_iterations,
             'dense_kwargs': self.dense_kwargs,
         }
         base_config.update(config)
         return base_config
-    
-    
-def _get_reverse_edge_features_fn(
-    tensor: GraphTensor
-) -> tf.Tensor:
-    # Find the index of "reverse" edge of edge_src->edge_dst
-    edge_exclude = tf.logical_and(
-        tensor.edge_src[:, None] == tensor.edge_dst,
-        tensor.edge_dst[:, None] == tensor.edge_src)
-    # Obtain index of edge_src->edge_dst ("forward") and its corresponding
-    # edge_src<-edge_dst ("reverse"). For molecules: forward and reverse
-    # edges are usually the same and always exist. 
-    edge_forward, edge_reverse = tf.split(tf.where(edge_exclude), 2, axis=-1)
-    return tf.tensor_scatter_nd_add(
-        tf.zeros_like(tensor.edge_feature), 
-        tf.expand_dims(edge_forward, -1), 
-        tf.gather(tensor.edge_feature, edge_reverse))
-
-def _get_reverse_edge_features(
-    tensor: GraphTensor, 
-    parallel_iterations: Optional[int] = None
-) -> tf.Tensor:
-    'Obtain reverse edge features to subtract from aggregated edge features.'
-    output_spec = tf.RaggedTensorSpec(
-        shape=[None, tensor.edge_feature.shape[-1]], 
-        ragged_rank=0, 
-        dtype=tf.float32)
-    reverse_edge_feature = tf.map_fn(
-        fn=_get_reverse_edge_features_fn, 
-        elems=tensor.separate(), 
-        fn_output_signature=output_spec,
-        parallel_iterations=parallel_iterations)
-    return reverse_edge_feature.merge_dims(outer_axis=0, inner_axis=1)
-    
-def edge_message_passing(
-    tensor: GraphTensor, 
-    parallel_iterations: Optional[int] = None
-) -> tf.Tensor:
-    num_nodes = tf.shape(tensor.node_feature)[0]
-    message = tf.math.unsorted_segment_sum(
-        tensor.edge_feature, tensor.edge_dst, num_nodes)
-    message = tf.gather(message, tensor.edge_src)
-    message = message - _get_reverse_edge_features(
-        tensor, parallel_iterations)
-    return message
```

### Comparing `molgraph-0.2.4/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.0/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.0/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/models/mpnn.py` & `molgraph-0.3.0/molgraph/models/mpnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
     '''Message passing neural network (MPNN) with weight tying.
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to
     ``MPNNConv``, which performs a single step of message passing, ``MPNN``
     performs n-steps of message passing. Furthermore, the weights are shared
     between the message functions of the different steps. And the update
-    functions correspond to a single GRU. This implementation is more similar
-    to Gilmer et al. compared to the stacking of ``MPNNConv`` layers.
+    functions correspond to a single GRU.
 
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
```

### Comparing `molgraph-0.2.4/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.0/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.0/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.2.4/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.0/molgraph/tensors/graph_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,20 +163,20 @@
     ... )
     >>> random_feature_1 = tf.random.uniform(
     ...     graph_tensor['node_feature'].shape)
     >>> random_feature_2 = tf.random.uniform(
     ...    graph_tensor['node_feature'].shape)
     >>> # Add new field
     >>> graph_tensor = graph_tensor.update({
-    ...     'random_feature': random_feature_1})
+    ...     'node_random_feature': random_feature_1})
     >>> # Update exisiting field
     >>> graph_tensor = graph_tensor.update({
     ...     'node_feature': random_feature_2})
     >>> # Remove field
-    >>> graph_tensor = graph_tensor.remove(['random_feature'])
+    >>> graph_tensor = graph_tensor.remove(['node_random_feature'])
     >>> graph_tensor
     GraphTensor(
       edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(5, 2), dtype=float32>,
       graph_indicator=<tf.Tensor: shape=(5,), dtype=int32>)
 
@@ -310,14 +310,19 @@
             # as the exisiting values of the graph tensor.
             _assert_compatible_sizes(
                 new_value, data['node_feature'], data['edge_dst'])
 
             if k in data:
                 data[k] = convert_tensor(new_value, data[k])
             else:
+                if 'node' not in k and 'edge' not in k:
+                    raise ValueError(
+                        'Please prepend `node_` or `edge_` to the new fields added, ' + 
+                        'depending on if they are associated with the nodes or edges ' + 
+                        'of the graph.')
                 data[k] = tf.cond(
                     _compatible_sizes(new_value, data['node_feature']),
                     lambda: convert_tensor(new_value, data['node_feature']),
                     lambda: convert_tensor(new_value, data['edge_dst']))
         return self.__class__(data)
 
     # TODO: modify spec accordingly
@@ -337,15 +342,15 @@
             by 'fields'.
         '''
         data = self._data.copy()
         if isinstance(fields, str):
             fields = [fields]
         for field in fields:
             if field in _non_updatable_fields:
-                raise ValueError(f'{k} cannot be removed.')
+                raise ValueError(f'{field} cannot be removed.')
             data.pop(field)
         return self.__class__(data)
 
     def merge(self) -> 'GraphTensor':
         '''Merges subgraphs into a single disjoint graph.
 
         Returns:
@@ -385,51 +390,49 @@
                     data))
 
         data = _remove_intersubgraph_edges(data)
 
         graph_indicator = data.pop('graph_indicator')
         edge_dst = data.pop('edge_dst')
         edge_src = data.pop('edge_src')
-
         graph_indicator_edges = tf.gather(graph_indicator, edge_dst)
 
         def to_ragged_tensor(
             tensor: Union[tf.Tensor, tf.RaggedTensor],
+            graph_indicator: tf.Tensor,
             num_subgraphs: tf.Tensor,
         ) -> tf.RaggedTensor:
-
             if isinstance(tensor, tf.RaggedTensor):
                 return tensor
-
-            value_rowids, nrows = tf.cond(
-                _compatible_sizes(tensor, graph_indicator),
-                lambda: (graph_indicator, num_subgraphs),
-                lambda: tf.cond(
-                    _compatible_sizes(tensor, graph_indicator_edges),
-                    lambda: (graph_indicator_edges, num_subgraphs),
-                    lambda: (tf.zeros(
-                        tf.shape(tensor)[0], dtype=graph_indicator.dtype),
-                            tf.constant(1, dtype=num_subgraphs.dtype))
-                )
-            )
             return tf.RaggedTensor.from_value_rowids(
-                tensor, value_rowids, nrows)
-
+                tensor, graph_indicator, num_subgraphs)
+        
         num_subgraphs = self.num_subgraphs
-        data = tf.nest.map_structure(
-            lambda x: to_ragged_tensor(x, num_subgraphs), data)
+
+        data_edges = {k: v for (k, v) in data.items() if 'edge' in k}
+        data_nodes = {k: v for (k, v) in data.items() if not 'edge' in k}
+
+        data_edges = tf.nest.map_structure(
+            lambda x: to_ragged_tensor(
+                x, graph_indicator_edges, num_subgraphs), data_edges)
+        data_nodes = tf.nest.map_structure(
+            lambda x: to_ragged_tensor(
+                x, graph_indicator, num_subgraphs), data_nodes)   
+
         decrement = tf.gather(
-            data['node_feature'].row_starts(), graph_indicator_edges)
+            data_nodes['node_feature'].row_starts(), graph_indicator_edges)
         decrement = tf.cast(decrement, dtype=edge_dst.dtype)
-        data['edge_dst'] = tf.RaggedTensor.from_value_rowids(
+        data_edges['edge_dst'] = tf.RaggedTensor.from_value_rowids(
             edge_dst - decrement, graph_indicator_edges, num_subgraphs)
-        data['edge_src'] = tf.RaggedTensor.from_value_rowids(
+        data_edges['edge_src'] = tf.RaggedTensor.from_value_rowids(
             edge_src - decrement, graph_indicator_edges, num_subgraphs)
 
-        return self.__class__(data)
+        data_nodes.update(data_edges)
+
+        return self.__class__(data_nodes)
 
     @property
     def _type_spec(self) -> 'GraphTensorSpec':
         'CompositeTensor API.'
         return self._spec
 
     @property
@@ -674,14 +677,16 @@
     Applied only when graph_tensor.separate() is called
     '''
     subgraphs_dst = tf.gather(data['graph_indicator'], data['edge_dst'])
     subgraphs_src = tf.gather(data['graph_indicator'], data['edge_src'])
     mask = tf.where((subgraphs_dst - subgraphs_src) == 0, True, False)
     data['edge_dst'] = tf.boolean_mask(data['edge_dst'], mask)
     data['edge_src'] = tf.boolean_mask(data['edge_src'], mask)
+    if 'edge_feature' in data:
+        data['edge_feature'] = tf.boolean_mask(data['edge_feature'], mask)
     return data
 
 def _maybe_convert_to_tensors(
     data: NestedArrays,
     check_values: bool = False,
     check_keys: bool = False,
 ) -> NestedTensors:
@@ -720,46 +725,51 @@
 
     data = {k: maybe_convert(v) for (k, v) in data.items()}
     _check_tensor_types(data)
     return data
 
 def _check_data_keys(data: NestedArrays):
     'Asserts that necessary fields exist in the graph (tensor)'
-    return [
-        tf.Assert(
-            req_field in data, [f'`data` requires `{req_field}` field']
-        )
-        for req_field in _required_fields]
+    for req_field in _required_fields:
+        assert_op = tf.Assert(
+            req_field in data, 
+            [f'`data` requires `{req_field}` field'])
+        _maybe_mark_used(assert_op)
+    return
 
 def _check_data_values(data: NestedArrays):
     'Asserts that the values of the data fields are of correct type'
-    return [
-        tf.Assert(
-            isinstance(v, _allowable_input_types),
+    for key, value in data.items():
+        assert_op = tf.Assert(
+            isinstance(value, _allowable_input_types),
             [
-                f'Field `{k}` is needs to be a `tf.Tensor`, ' +
+                f'Field `{key}` is needs to be a `tf.Tensor`, ' +
                 '`tf.RaggedTensor`, `np.ndarray`, `list` or `tuple`'
             ]
         )
-        for (k, v) in data.items()]
+        _maybe_mark_used(assert_op)
+    return
 
 def _check_tensor_types(data: NestedTensors):
     'Asserts that all nested values of data are of the same tensor type'
     tests = [isinstance(x, tf.Tensor) for x in data.values()]
     same_types = all(tests) or not any(tests)
-    return tf.Assert(
+    assert_op = tf.Assert(
         same_types, [
             f'Nested tensors are not the same type. ' +
              'Found both `tf.Tensor`s and `tf.RaggedTensor`s'])
+    _maybe_mark_used(assert_op)
+    return
 
 def _check_ragged_rank(x: tf.RaggedTensor):
-    return tf.Assert(
+    assert_op = tf.Assert(
         tf.math.equal(x.ragged_rank, 1),
-        ['Ragged rank of field needs to be 1.']
-    )
+        ['Ragged rank of field needs to be 1.'])
+    _maybe_mark_used(assert_op)
+    return
 
 def _compatible_sizes(
     a: Union[tf.Tensor, tf.RaggedTensor],
     b: Union[tf.Tensor, tf.RaggedTensor],
 ) -> bool:
     'Checks if the two inputs have the same number of nodes or edges'
     def _get_size(x):
@@ -769,27 +779,29 @@
         return tf.shape(x)[0]
     return _get_size(a) == _get_size(b)
 
 def _assert_compatible_sizes(
     target: Union[tf.Tensor, tf.RaggedTensor],
     *comparators: Union[tf.Tensor, tf.RaggedTensor]
 ):
-    return tf.Assert(
+    assert_op = tf.Assert(
         tf.math.reduce_any(
             tf.nest.map_structure(
                 lambda comparator: _compatible_sizes(target, comparator),
                 comparators
             )
         ), [
             'At least one of the added fields does not match ' +
             'the size of the existing fields. Namely, one of the ' +
             'added fields did not have the same numeber of ' +
             'nodes or edges as the existig fields'
         ]
     )
+    _maybe_mark_used(assert_op)
+    return
 
 def _maybe_add_graph_indicator(
     data: NestedTensors,
     spec: NestedTensorSpecs,
 ) -> NestedTensors:
     'Maybe adds `graph_indicator` to data and spec.'
     if (
@@ -807,38 +819,43 @@
             spec['graph_indicator'] = tf.RaggedTensorSpec(
                 x.shape, x.dtype, spec['edge_dst'].ragged_rank, spec['edge_dst'].row_splits_dtype
             )
     return data, spec
 
 def _assert_mergeable(data: NestedTensors):
     'Asserts that all nested tensors are ragged.'
-    return tf.Assert(
+    assert_op = tf.Assert(
         all([isinstance(x, tf.RaggedTensor) for x in data.values()]),
         [f'All data values need to be `tf.RaggedTensor`s to be merged'])
+    _maybe_mark_used(assert_op)
+    return
 
 def _assert_separable(data: NestedTensors):
     'Asserts that all nested tensors are non-ragged'
-    return tf.Assert(
+    assert_op = tf.Assert(
         all([isinstance(x, tf.Tensor) for x in data.values()]),
         [f'All data values need to be `tf.Tensor`s to be separated'])
+    _maybe_mark_used(assert_op)
+    return
 
 def _slice_to_tensor(slice_obj: slice, limit: int) -> tf.Tensor:
     '''Converts slice to a tf.range, which can subsequently be used with
     tf.gather to gather subgraphs.
 
     Note: GraphTensor is currently irreversible (e.g., x[::-1] or x[::-2]
     will not work).
     '''
     start = slice_obj.start
     stop = slice_obj.stop
     step = slice_obj.step
 
-    tf.Assert(
+    assert_op = tf.Assert(
         step is None or not (step < 0 or step == 0),
         ['Slice step cannot be negative or zero.'])
+    _maybe_mark_used(assert_op)
 
     limit = tf.convert_to_tensor(limit)
 
     if stop is None:
         stop = limit
     else:
         stop = tf.convert_to_tensor(stop)
@@ -867,14 +884,19 @@
     else:
         step = tf.convert_to_tensor(step)
 
     start = tf.cond(start > stop, lambda: stop, lambda: start)
 
     return tf.range(start, stop, step)
 
+def _maybe_mark_used(assert_op):
+    if hasattr(assert_op, 'mark_used'):
+        assert_op.mark_used()
+    return
+
 @tf.experimental.dispatch_for_api(tf.gather)
 def graph_tensor_gather(
     params: GraphTensor,
     indices,
     validate_indices=None,
     axis=None,
     batch_dims=0,
@@ -912,29 +934,19 @@
 ) -> GraphTensor:
     'Concatenates list of graph tensors into a single graph tensor.'
 
     if axis is not None and axis != 0:
         raise ValueError(
             f'axis=0 is required for `{values[0].__class__.__name__}`s.')
 
-    def get_row_lengths(x, dtype):
-        if hasattr(x, 'row_lengths'):
-            return tf.cast(x.row_lengths(), dtype=dtype)
-        return tf.cast(x.shape[:1], dtype=dtype)
-
-    def from_row_lengths(x, num_nodes, num_edges, dtype):
-        return tf.cond(
-            tf.shape(x, dtype)[0] == tf.reduce_sum(num_nodes),
-            lambda: tf.RaggedTensor.from_row_lengths(x, num_nodes),
-            lambda: tf.cond(
-                tf.shape(x, dtype)[0] == tf.reduce_sum(num_edges),
-                lambda: tf.RaggedTensor.from_row_lengths(x, num_edges),
-                lambda: tf.RaggedTensor.from_row_lengths(x, tf.shape(x)[:1])
-            )
-        )
+    def fast_ragged_stack(component_data, dtype):
+        row_lengths = [len(x) for x in component_data]
+        component_data_concat = tf.concat(component_data, axis=0)
+        return tf.RaggedTensor.from_row_lengths(
+            component_data_concat, tf.cast(row_lengths, dtype))
 
     structure = values[0]._data
 
     ragged = tf.nest.map_structure(
         lambda x: isinstance(x['node_feature'], tf.RaggedTensor), values)
 
     if 0 < sum(ragged) < len(ragged):
@@ -946,30 +958,24 @@
         ragged = ragged[0]
 
     flat_sequence = tf.nest.map_structure(
         lambda x: tf.nest.flatten(x, expand_composites=True), values)
 
     dtype = values[0]['edge_dst'].dtype
 
-    num_nodes = tf.concat([
-        get_row_lengths(x['node_feature'], dtype) for x in values], axis=0)
-
-    num_edges = tf.concat([
-        get_row_lengths(x['edge_dst'], dtype) for x in values], axis=0)
-
     if ragged:
         # Keep only values (resulting from tf.nest.flatten)
         flat_sequence = [f[::2] for f in flat_sequence]
 
     flat_sequence = list(zip(*flat_sequence))
-    flat_sequence = [tf.concat(x, axis=0) for x in flat_sequence]
-    values = tf.nest.pack_sequence_as(structure, flat_sequence)
-    values = tf.nest.map_structure(
-        lambda x: from_row_lengths(x, num_nodes, num_edges, dtype),
-        values)
+    flat_sequence_stacked = [
+        fast_ragged_stack(x, dtype) for x in flat_sequence
+    ]
+    values = tf.nest.pack_sequence_as(structure, flat_sequence_stacked)
+
     values = GraphTensor(values)
 
     if ragged:
         return values
 
     return values.merge()
```

### Comparing `molgraph-0.2.4/molgraph.egg-info/PKG-INFO` & `molgraph-0.3.0/molgraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.2.4
+Version: 0.3.0
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.2.4/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.0/molgraph.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,28 +37,30 @@
 molgraph/layers/convolutional/gin_conv.py
 molgraph/layers/convolutional/graph_sage_conv.py
 molgraph/layers/geometric/__init__.py
 molgraph/layers/geometric/_radial_basis.py
 molgraph/layers/geometric/dtnn_conv.py
 molgraph/layers/geometric/gcf_conv.py
 molgraph/layers/message_passing/__init__.py
+molgraph/layers/message_passing/edge_conv.py
 molgraph/layers/message_passing/mpnn_conv.py
 molgraph/layers/positional_encoding/__init__.py
 molgraph/layers/positional_encoding/laplacian.py
 molgraph/layers/postprocessing/__init__.py
 molgraph/layers/postprocessing/dot_product_incident.py
 molgraph/layers/postprocessing/extract_field.py
 molgraph/layers/postprocessing/gather_incident.py
 molgraph/layers/preprocessing/__init__.py
 molgraph/layers/preprocessing/center_scaling.py
 molgraph/layers/preprocessing/embedding_lookup.py
 molgraph/layers/preprocessing/min_max_scaling.py
 molgraph/layers/preprocessing/projection.py
 molgraph/layers/preprocessing/standard_scaling.py
 molgraph/layers/readout/__init__.py
+molgraph/layers/readout/node_readout.py
 molgraph/layers/readout/segment_pool.py
 molgraph/layers/readout/set_gather.py
 molgraph/layers/readout/transformer_encoder.py
 molgraph/losses/__init__.py
 molgraph/losses/link_losses.py
 molgraph/losses/masked_losses.py
 molgraph/metrics/__init__.py
```

### Comparing `molgraph-0.2.4/setup.py` & `molgraph-0.3.0/setup.py`

 * *Files identical despite different names*

