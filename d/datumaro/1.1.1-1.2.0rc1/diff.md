# Comparing `tmp/datumaro-1.1.1.tar.gz` & `tmp/datumaro-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.1.1.tar", last modified: Tue Mar 28 01:36:19 2023, max compression
+gzip compressed data, was "datumaro-1.2.0rc1.tar", last modified: Fri Apr 14 10:11:45 2023, max compression
```

## Comparing `datumaro-1.1.1.tar` & `datumaro-1.2.0rc1.tar`

### file list

```diff
@@ -1,271 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.066109 datumaro-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-03-28 01:36:09.000000 datumaro-1.1.1/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-28 01:36:09.000000 datumaro-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-28 01:36:09.000000 datumaro-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-28 01:36:09.000000 datumaro-1.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-28 01:36:19.066109 datumaro-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-28 01:36:09.000000 datumaro-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.038108 datumaro-1.1.1/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.038108 datumaro-1.1.1/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.038108 datumaro-1.1.1/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.042108 datumaro-1.1.1/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/describe_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.042108 datumaro-1.1.1/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.042108 datumaro-1.1.1/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/project/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.042108 datumaro-1.1.1/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.046108 datumaro-1.1.1/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.046108 datumaro-1.1.1/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10672 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/hl_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/media_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    69870 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89331 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.046108 datumaro-1.1.1/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.046108 datumaro-1.1.1/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.050108 datumaro-1.1.1/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20633 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18957 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.054108 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38474 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.058108 datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/synthia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.062108 datumaro-1.1.1/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    40387 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    47389 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.066109 datumaro-1.1.1/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 01:36:09.000000 datumaro-1.1.1/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:19.038108 datumaro-1.1.1/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 01:36:19.000000 datumaro-1.1.1/datumaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-28 01:36:09.000000 datumaro-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-28 01:36:09.000000 datumaro-1.1.1/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-28 01:36:09.000000 datumaro-1.1.1/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 01:36:19.066109 datumaro-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-28 01:36:09.000000 datumaro-1.1.1/setup.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)   361854 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/3rd-party.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1090 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/LICENSE
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      103 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/MANIFEST.in
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      229 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/NOTICE
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5901 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/PKG-INFO
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5328 2023-03-29 05:58:32.000000 datumaro-1.2.0rc1/README.md
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1715 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      178 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/__main__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/capi/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3379 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/capi/pybind.cpp
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-04-03 09:17:53.000000 datumaro-1.2.0rc1/datumaro/cli/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5494 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/__main__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      962 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5063 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/convert.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3991 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/detect_format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10146 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/download.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9340 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/explain.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9046 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/filter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3073 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/generate.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9396 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/cli/commands/merge.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5979 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/patch.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1355 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/__init__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      134 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9162 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/diff.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5906 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/export.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4242 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/info.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3120 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/stats.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8369 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/transform.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4843 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/validate.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      116 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5227 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/add.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1957 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/create.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5892 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/import_.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1677 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/remove.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      123 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2946 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2150 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2758 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/info.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1132 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/log.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1412 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/status.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4250 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/search.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/contexts/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      121 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9089 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/model.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/contexts/project/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4501 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/project/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2553 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/source.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4097 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/util.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/util/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3988 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13328 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/diff.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      391 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/util/errors.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5638 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/project.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/__init__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/algorithms/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      135 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/__init__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      111 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7851 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8073 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/rise.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    29706 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/annotation.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/annotations/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      118 2023-03-30 07:03:27.000000 datumaro-1.2.0rc1/datumaro/components/annotations/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8964 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/annotations/matcher.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5242 2023-03-30 07:03:27.000000 datumaro-1.2.0rc1/datumaro/components/annotations/merger.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2146 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/cli_plugin.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8101 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/config.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3570 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/config_model.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2240 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/crypter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    52703 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/dataset.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10947 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/dataset_base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9776 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/environment.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17884 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/errors.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13568 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19651 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/extractor_tfds.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10063 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/filter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19613 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/format_detection.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      534 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/generator.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/hl_ops/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8556 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/hl_ops/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8657 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/components/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2901 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/launcher.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    36037 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/media.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2450 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/media_manager.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/merge/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      662 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2047 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11438 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/exact_merge.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20825 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/intersect_merge.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3412 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/union_merge.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    23475 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/operations.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5222 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/progress_reporting.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    89324 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/project.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5206 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/searcher.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9352 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/shift_analyzer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1830 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/transformer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2105 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/validator.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17135 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/visualizer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      164 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/errors.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      172 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/ops.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/__init__.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1148 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4038 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2217 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6297 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2017.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8482 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2020.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      232 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5909 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2351 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    14655 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1514 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2129 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/importer.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8441 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5585 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3501 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3659 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats_numpy.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17438 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/camvid.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      183 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7512 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10476 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12141 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cifar.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20683 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cityscapes.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19013 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    28658 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      477 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6074 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6348 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3128 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_super_resolution.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13642 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20627 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      214 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/format.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       72 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11047 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    15359 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      317 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1236 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/importer.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      286 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6627 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11117 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      828 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1921 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      631 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11105 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2236 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1563 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5235 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11780 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6440 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      311 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1828 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_dir.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3950 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_zip.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6824 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8124 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5752 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kinetics.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5975 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11358 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3970 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3713 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/importer.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11148 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17769 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      711 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20175 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/labelme.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    14960 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/lfw.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10904 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12550 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3712 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6396 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/market1501.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5013 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mars.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9041 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7026 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist_csv.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10664 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mot.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6493 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mots.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      556 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5193 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4937 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3937 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4813 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      563 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1873 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1625 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    38486 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/open_images.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6888 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16130 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      420 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7024 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/synthia.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7629 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8812 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      308 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    15332 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vgg_face2.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6379 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/video.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16609 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    30069 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9071 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2897 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2813 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_csv.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3854 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_json.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10103 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/widerface.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12374 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/base.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12070 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      457 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/format.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5573 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/importer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16787 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/ndr.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9757 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/launcher.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/sampler/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       72 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7785 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/random_sampler.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8754 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2869 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/searcher.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1213 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/shift_analyzer.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    32124 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/splitter.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      155 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11335 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11577 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/image_generator.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6194 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/utils.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/tiling/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      116 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9398 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/merge_tile.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9834 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/tile.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1141 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    41229 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/transforms.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    47389 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/validators.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      376 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/project.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/datumaro/util/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4809 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/__init__.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8473 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/annotation_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1198 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/attrs_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      262 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/definitions.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      882 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/util/file_utils.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11657 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/util/image.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      968 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/image_cache.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      795 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/log_utils.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11440 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/mask_tools.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2062 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/meta_file_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8479 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/os_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      758 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/util/pickle_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      246 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/samples.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4702 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/scope.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      616 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/telemetry_stub.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6254 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/util/telemetry_utils.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2579 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/tf_util.py
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       25 2023-04-14 10:04:40.000000 datumaro-1.2.0rc1/datumaro/version.py
+drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro.egg-info/
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5901 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/PKG-INFO
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10677 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        1 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       53 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/entry_points.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      764 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/requires.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        9 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/top_level.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2488 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/pyproject.toml
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      692 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/requirements-core.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      266 2023-03-29 05:58:32.000000 datumaro-1.2.0rc1/requirements-default.txt
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       38 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/setup.cfg
+-rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3342 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/setup.py
```

### Comparing `datumaro-1.1.1/3rd-party.txt` & `datumaro-1.2.0rc1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/LICENSE` & `datumaro-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/PKG-INFO` & `datumaro-1.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.1.1
+Version: 1.2.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.1.1/README.md` & `datumaro-1.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/__init__.py` & `datumaro-1.2.0rc1/datumaro/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright (C) 2019-2022 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from . import errors as errors
 from . import ops as ops
 from . import project as project
+from .components.algorithms import RISE, LossDynamicsAnalyzer
 from .components.annotation import (
     NO_GROUP,
     Annotation,
     AnnotationType,
     Bbox,
     BinaryMaskImage,
     Caption,
@@ -38,24 +39,22 @@
     DatasetBase,
     DatasetItem,
     IDataset,
     SubsetBase,
 )
 from .components.environment import Environment, PluginRegistry
 from .components.exporter import Exporter, ExportErrorPolicy, FailingExportErrorPolicy
-from .components.hl_ops import (  # pylint: disable=redefined-builtin
-    export,
-    filter,
-    merge,
-    run_model,
-    transform,
-    validate,
-)
+from .components.hl_ops import HLOps
 from .components.importer import FailingImportErrorPolicy, Importer, ImportErrorPolicy
 from .components.launcher import Launcher, ModelTransform
 from .components.media import ByteImage, Image, MediaElement, Video, VideoFrame
 from .components.media_manager import MediaManager
-from .components.progress_reporting import NullProgressReporter, ProgressReporter
+from .components.progress_reporting import (
+    NullProgressReporter,
+    ProgressReporter,
+    SimpleProgressReporter,
+    TQDMProgressReporter,
+)
 from .components.transformer import ItemTransform, Transform
 from .components.validator import Validator
 from .components.visualizer import Visualizer
-from .version import VERSION
+from .version import __version__
```

### Comparing `datumaro-1.1.1/datumaro/capi/pybind.cpp` & `datumaro-1.2.0rc1/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/commands/checkout.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.project import load_project
+from ....util import MultilineFormatter
+from ....util.project import load_project
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Navigate to a revision",
         description="""
         Command forms:|n
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/commit.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.project import load_project
+from ....util import MultilineFormatter
+from ....util.project import load_project
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Create a revision",
         description="""
         Creates a new revision from the current state of the working directory.|n
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/convert.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 import os
 import os.path as osp
 
 from datumaro.components.dataset import Dataset
 from datumaro.components.project import Environment
 from datumaro.util.os_util import make_file_name
 
-from ..contexts.project import FilterModes
 from ..util import MultilineFormatter
 from ..util.errors import CliException
-from ..util.project import generate_next_file_name
+from ..util.project import FilterModes, generate_next_file_name
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     builtin_readers = sorted(set(Environment().importers) | set(Environment().extractors))
     builtin_writers = sorted(Environment().exporters)
 
     parser = parser_ctor(
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/create.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging as log
 import os
 import os.path as osp
 
 from datumaro.components.project import Project
 from datumaro.util.os_util import rmtree
 
-from ..util import MultilineFormatter
-from ..util.errors import CliException
+from ....util import MultilineFormatter
+from ....util.errors import CliException
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Create empty project",
         description="""
         Create an empty Datumaro project. A project is required for the most of
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/detect_format.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/commands/diff.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.operations import DistanceComparator, ExactComparator
 from datumaro.util import dump_json_file
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
-from ..contexts.project.diff import DiffVisualizer
-from ..util import MultilineFormatter
-from ..util.errors import CliException
-from ..util.project import generate_next_file_name, load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.diff import DiffVisualizer
+from ....util.errors import CliException
+from ....util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 class ComparisonMethod(Enum):
     equality = auto()
     distance = auto()
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/download.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,164 @@
-# Copyright (C) 2021-2022 Intel Corporation
+# Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
-from datumaro.components.extractor_tfds import AVAILABLE_TFDS_DATASETS, TFDS_EXTRACTOR_AVAILABLE
-from datumaro.components.project import Environment
-from datumaro.util.os_util import make_file_name
+from datumaro.components.environment import Environment
+from datumaro.components.errors import ProjectNotFoundError
+from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
-from ..util.project import generate_next_file_name
+from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    builtin_writers = sorted(Environment().exporters)
-    if TFDS_EXTRACTOR_AVAILABLE:
-        available_datasets = ", ".join(f"tfds:{name}" for name in AVAILABLE_TFDS_DATASETS)
-    else:
-        available_datasets = "N/A (TensorFlow and/or TensorFlow Datasets " "are not installed)"
-
     parser = parser_ctor(
-        help="Download a publicly available dataset",
+        help="Updates dataset from another one",
         description="""
-        Downloads a publicly available dataset and saves it in a given format.|n
+        Updates items of the first dataset with items from the second one.|n
         |n
-        Currently, the only source of datasets is the TensorFlow Datasets
-        library. Therefore, to use this command you must install TensorFlow &
-        TFDS, which you can do as follows:|n
+        By default, datasets are updated in-place. The '-o/--output-dir'
+        option can be used to specify another output directory. When
+        updating in-place, use the '--overwrite' parameter along with the
+        '--save-images' export option (in-place updates fail by default
+        to prevent data loss).|n
+        |n
+        Unlike the regular project data source joining, the datasets are not
+        required to have the same labels. The labels from the "patch"
+        dataset are projected onto the labels of the patched dataset,
+        so only the annotations with the matching labels are used, i.e.
+        all the annotations having unknown labels are ignored. Currently,
+        this command doesn't allow to update the label information in the
+        patched dataset.|n
+        |n
+        The command supports passing extra exporting options for the output
+        dataset. The extra options should be passed after the main arguments
+        and after the '--' separator. Particularly, this is useful to include
+        images in the output dataset with '--save-images'.|n
+        |n
+        This command can be applied to the current project targets or
+        arbitrary datasets outside a project. Note that if the target dataset
+        is read-only (e.g. if it is a project, stage or a cache entry),
+        the output directory must be provided.|n
+        |n
+        This command has the following invocation syntax:
+        - %(prog)s <target dataset revpath> <patch dataset revpath>|n
+        |n
+        <revpath> - either a dataset path or a revision path. The full
+        syntax is:|n
+        - Dataset paths:|n
+        |s|s- <dataset path>[ :<format> ]|n
+        - Revision paths:|n
+        |s|s- <project path> [ @<rev> ] [ :<target> ]|n
+        |s|s- <rev> [ :<target> ]|n
+        |s|s- <target>|n
+        |n
+        The current project (-p/--project) is also used as a context for
+        plugins, so it can be useful for dataset paths having custom formats.
+        When not specified, the current project's working tree is used.|n
         |n
-        |s|spip install datumaro[tf,tfds]|n
+        Examples:|n
+        - Update a VOC-like dataset with COCO-like annotations:|n
+        |s|s%(prog)s --overwrite dataset1/:voc dataset2/:coco -- --save-images|n
         |n
-        Supported datasets: {}|n
+        - Generate a patched dataset, based on a project:|n
+        |s|s%(prog)s -o patched_proj1/ proj1/ proj2/|n
         |n
-        For information about the datasets, run "datum describe-downloads".
-        More detailed information can be found in the TFDS Catalog:
-        <https://www.tensorflow.org/datasets/catalog/overview>.|n
+        - Update the "source1" source in the current project with a dataset:|n
+        |s|s%(prog)s -p proj/ --overwrite source1 path/to/dataset2:coco|n
         |n
-        Supported output formats: {}|n
+        - Generate a patched source from a previous revision and a dataset:|n
+        |s|s%(prog)s -o new_src2/ HEAD~2:source-2 path/to/dataset2:yolo|n
         |n
-        Examples:|n
-        - Download the MNIST dataset:|n
-        |s|s%(prog)s -i tfds:mnist -- --save-media|n
-        |n
-        - Download the VOC 2012 dataset, saving only the annotations in the COCO
-          format into a specific directory:|n
-        |s|s%(prog)s -i tfds:voc/2012 -f coco -o path/I/like/
-        """.format(
-            available_datasets, ", ".join(builtin_writers)
-        ),
+        - Update a dataset in a custom format, described in a project plugin:|n
+        |s|s%(prog)s -p proj/ --overwrite dataset/:my_format dataset2/:coco
+        """,
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument("-i", "--dataset-id", required=True, help="Which dataset to download")
-    parser.add_argument(
-        "-f", "--output-format", help="Output format (default: original format of the dataset)"
-    )
+    parser.add_argument("target", help="Target dataset revpath")
+    parser.add_argument("patch", help="Patch dataset revpath")
     parser.add_argument(
         "-o",
         "--output-dir",
         dest="dst_dir",
-        help="Directory to save output (default: a subdir in the current one)",
+        default=None,
+        help="Output directory (default: save in-place)",
     )
     parser.add_argument(
-        "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
+        "--overwrite",
+        action="store_true",
+        help="Overwrite existing files in the save directory, " "if it is not empty",
+    )
+    parser.add_argument(
+        "-p",
+        "--project",
+        dest="project_dir",
+        help="Directory of the 'current' project (default: current dir)",
     )
-    parser.add_argument("-s", "--subset", help="Save only the specified subset")
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
-        help="Additional arguments for output format (pass '-- -h' for help). "
-        "Must be specified after the main command arguments",
+        help="Additional arguments for exporting (pass '-- -h' for help). "
+        "Must be specified after the main command arguments and after "
+        "the '--' separator",
     )
-    parser.set_defaults(command=download_command)
+    parser.set_defaults(command=patch_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        download_command: ["dst_dir", "extra_args"],
+        patch_command: ["target", "patch", "dst_dir", "project_dir", "extra_args"],
     }
 
 
-def download_command(args):
-    env = Environment()
+@scoped
+def patch_command(args):
+    project = None
+    try:
+        project = scope_add(load_project(args.project_dir))
+    except ProjectNotFoundError:
+        if args.project_dir:
+            raise
 
-    if args.dataset_id.startswith("tfds:"):
-        if TFDS_EXTRACTOR_AVAILABLE:
-            tfds_ds_name = args.dataset_id[5:]
-            tfds_ds = AVAILABLE_TFDS_DATASETS.get(tfds_ds_name)
-            if tfds_ds:
-                default_output_format = tfds_ds.metadata.default_output_format
-                extractor_factory = tfds_ds.make_extractor
-            else:
-                raise CliException(f"Unsupported TFDS dataset '{tfds_ds_name}'")
-        else:
-            raise CliException(
-                "TFDS datasets are not available, because TFDS and/or "
-                "TensorFlow are not installed.\n"
-                "You can install them with: pip install datumaro[tf,tfds]"
-            )
+    if project is not None:
+        env = project.env
     else:
-        raise CliException(f"Unknown dataset ID '{args.dataset_id}'")
+        env = Environment()
 
-    output_format = args.output_format or default_output_format
+    target_dataset, _project = parse_full_revpath(args.target, project)
+    if _project is not None:
+        scope_add(_project)
 
     try:
-        exporter = env.exporters[output_format]
+        exporter = env.exporters[target_dataset.format]
     except KeyError:
-        raise CliException("Exporter for format '%s' is not found" % output_format)
+        raise CliException("Exporter for format '%s' is not found" % args.format)
+
     extra_args = exporter.parse_cmdline(args.extra_args)
 
-    dst_dir = args.dst_dir
-    if dst_dir:
-        if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
-            raise CliException(
-                "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
-            )
-    else:
-        dst_dir = generate_next_file_name(
-            "%s-%s"
-            % (
-                make_file_name(args.dataset_id),
-                make_file_name(output_format),
-            )
+    dst_dir = args.dst_dir or target_dataset.data_path
+    if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
+        raise CliException(
+            "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
         )
     dst_dir = osp.abspath(dst_dir)
 
-    log.info("Downloading the dataset")
-    extractor = extractor_factory()
+    patch_dataset, _project = parse_full_revpath(args.patch, project)
+    if _project is not None:
+        scope_add(_project)
+
+    target_dataset.update(patch_dataset)
 
-    if args.subset:
-        try:
-            extractor = extractor.subsets()[args.subset]
-        except KeyError:
-            raise CliException("Subset '%s' is not present in the dataset" % args.subset)
+    target_dataset.save(save_dir=dst_dir, **extra_args)
 
-    log.info("Exporting the dataset")
-    exporter.convert(extractor, dst_dir, default_image_ext=".png", **extra_args)
+    log.info("Patched dataset has been saved to '%s'" % dst_dir)
 
-    log.info("Dataset exported to '%s' as '%s'" % (dst_dir, output_format))
+    return 0
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/explain.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/commands/filter.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.filter import DatasetItemEncoder
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
-from ..contexts.project import FilterModes
 from ..util import MultilineFormatter
 from ..util.errors import CliException
-from ..util.project import load_project, parse_full_revpath
+from ..util.project import FilterModes, load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Extract subdataset",
         description="""
         Extracts a subdataset that contains only items matching filter.|n
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/generate.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/commands/info.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import argparse
 
 from datumaro.components.annotation import AnnotationType
 from datumaro.components.errors import DatasetMergeError, MissingObjectError, ProjectNotFoundError
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.project import load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Prints dataset overview",
         description="""
         Prints info about the dataset at <revpath>, or about the current
@@ -84,15 +84,19 @@
         # TODO: avoid computing working tree hashes
         dataset, target_project = parse_full_revpath(args.target, project)
         if target_project:
             scope_add(target_project)
     except DatasetMergeError as e:
         dataset_problem = (
             "Can't merge project sources automatically: %s. "
-            "The conflicting sources are: %s" % (e, ", ".join(e.sources))
+            "The conflicting sources are: %s"
+            % (
+                e,
+                ", ".join(e.sources),
+            )
         )
     except MissingObjectError as e:
         dataset_problem = str(e)
 
     def print_dataset_info(dataset, indent=""):
         print("%slength:" % indent, len(dataset))
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/log.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 
 from datumaro.util.scope import scope_add, scoped
 
-from ..util.project import load_project
+from ....util.project import load_project
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(description="Prints project history.")
 
     parser.add_argument(
         "-n",
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/merge.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import os.path as osp
 from collections import OrderedDict
 
 from datumaro.components.dataset import DEFAULT_FORMAT
 from datumaro.components.environment import Environment
 from datumaro.components.errors import DatasetMergeError, DatasetQualityError, ProjectNotFoundError
-from datumaro.components.operations import IntersectMerge
+from datumaro.components.merge.intersect_merge import IntersectMerge
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter, join_cli_args
 from ..util.errors import CliException
 from ..util.project import generate_next_file_name, load_project, parse_full_revpath
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/patch.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/export.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,164 +1,181 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
 from datumaro.components.environment import Environment
 from datumaro.components.errors import ProjectNotFoundError
+from datumaro.components.project import ProjectBuildTargets
+from datumaro.util.os_util import make_file_name
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.errors import CliException
-from ..util.project import load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.errors import CliException
+from ....util.project import FilterModes, generate_next_file_name, load_project
+
+__all__ = [
+    "build_parser",
+    "get_sensitive_args",
+]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
+    builtins = sorted(Environment().exporters)
+
     parser = parser_ctor(
-        help="Updates dataset from another one",
+        help="Export project",
         description="""
-        Updates items of the first dataset with items from the second one.|n
+        Exports a project in some format.|n
         |n
-        By default, datasets are updated in-place. The '-o/--output-dir'
-        option can be used to specify another output directory. When
-        updating in-place, use the '--overwrite' parameter along with the
-        '--save-images' export option (in-place updates fail by default
-        to prevent data loss).|n
-        |n
-        Unlike the regular project data source joining, the datasets are not
-        required to have the same labels. The labels from the "patch"
-        dataset are projected onto the labels of the patched dataset,
-        so only the annotations with the matching labels are used, i.e.
-        all the annotations having unknown labels are ignored. Currently,
-        this command doesn't allow to update the label information in the
-        patched dataset.|n
-        |n
-        The command supports passing extra exporting options for the output
-        dataset. The extra options should be passed after the main arguments
-        and after the '--' separator. Particularly, this is useful to include
-        images in the output dataset with '--save-images'.|n
-        |n
-        This command can be applied to the current project targets or
-        arbitrary datasets outside a project. Note that if the target dataset
-        is read-only (e.g. if it is a project, stage or a cache entry),
-        the output directory must be provided.|n
-        |n
-        This command has the following invocation syntax:
-        - %(prog)s <target dataset revpath> <patch dataset revpath>|n
-        |n
-        <revpath> - either a dataset path or a revision path. The full
-        syntax is:|n
-        - Dataset paths:|n
-        |s|s- <dataset path>[ :<format> ]|n
-        - Revision paths:|n
-        |s|s- <project path> [ @<rev> ] [ :<target> ]|n
-        |s|s- <rev> [ :<target> ]|n
-        |s|s- <target>|n
-        |n
-        The current project (-p/--project) is also used as a context for
-        plugins, so it can be useful for dataset paths having custom formats.
-        When not specified, the current project's working tree is used.|n
+        Each dataset format has its own export
+        options, which are passed after the '--' separator (see examples),
+        pass '-- -h' for more info. If not stated otherwise, by default
+        only annotations are exported, to include images pass
+        '--save-images' parameter.|n
+        |n
+        A filter can be passed, check the 'filter' command description for
+        more info.|n
+        |n
+        Formats:|n
+        Datasets come in a wide variety of formats. Each dataset
+        format defines its own data structure and rules on how to
+        interpret the data. Check the user manual for the list of
+        supported formats, examples and documentation.
+        |n
+        The list of supported formats can be extended by plugins.
+        Check the "plugins" section of the developer guide for information
+        about plugin implementation.|n
+        |n
+        List of builtin dataset formats: {}|n
+        |n
+        The command can only be applied to a project build target, a stage
+        or the combined 'project' target, in which case all the targets will
+        be affected.
         |n
         Examples:|n
-        - Update a VOC-like dataset with COCO-like annotations:|n
-        |s|s%(prog)s --overwrite dataset1/:voc dataset2/:coco -- --save-images|n
-        |n
-        - Generate a patched dataset, based on a project:|n
-        |s|s%(prog)s -o patched_proj1/ proj1/ proj2/|n
-        |n
-        - Update the "source1" source in the current project with a dataset:|n
-        |s|s%(prog)s -p proj/ --overwrite source1 path/to/dataset2:coco|n
-        |n
-        - Generate a patched source from a previous revision and a dataset:|n
-        |s|s%(prog)s -o new_src2/ HEAD~2:source-2 path/to/dataset2:yolo|n
+        - Export project as a VOC-like dataset, include images:|n
+        |s|s%(prog)s -f voc -- --save-images|n
         |n
-        - Update a dataset in a custom format, described in a project plugin:|n
-        |s|s%(prog)s -p proj/ --overwrite dataset/:my_format dataset2/:coco
-        """,
+        - Export project as a COCO-like dataset in other directory:|n
+        |s|s%(prog)s -f coco -o path/I/like/
+        """.format(
+            ", ".join(builtins)
+        ),
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument("target", help="Target dataset revpath")
-    parser.add_argument("patch", help="Patch dataset revpath")
+    parser.add_argument(
+        "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
+    )  # workaround for -- eaten by positionals
+    parser.add_argument(
+        "target",
+        nargs="?",
+        default="project",
+        help="A project target to be exported (default: %(default)s)",
+    )
+    parser.add_argument("-e", "--filter", help="XML XPath filter expression for dataset items")
+    parser.add_argument(
+        "--filter-mode",
+        default=FilterModes.i.name,
+        type=FilterModes.parse,
+        help="Filter mode (options: %s; default: %s)"
+        % (", ".join(FilterModes.list_options()), "%(default)s"),
+    )
     parser.add_argument(
         "-o",
         "--output-dir",
         dest="dst_dir",
-        default=None,
-        help="Output directory (default: save in-place)",
+        help="Directory to save output (default: a subdir in the current one)",
     )
     parser.add_argument(
-        "--overwrite",
-        action="store_true",
-        help="Overwrite existing files in the save directory, " "if it is not empty",
+        "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
     )
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
-        help="Directory of the 'current' project (default: current dir)",
+        help="Directory of the project to operate on (default: current dir)",
     )
+    parser.add_argument("-f", "--format", required=True, help="Output format")
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
-        help="Additional arguments for exporting (pass '-- -h' for help). "
+        help="Additional arguments for exporter (pass '-- -h' for help). "
         "Must be specified after the main command arguments and after "
         "the '--' separator",
     )
-    parser.set_defaults(command=patch_command)
+    parser.set_defaults(command=export_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        patch_command: ["target", "patch", "dst_dir", "project_dir", "extra_args"],
+        export_command: ["dst_dir", "project_dir", "name", "extra_args", "target", "filter"],
     }
 
 
 @scoped
-def patch_command(args):
+def export_command(args):
+    has_sep = "--" in args._positionals
+    if has_sep:
+        pos = args._positionals.index("--")
+        if 1 < pos:
+            raise argparse.ArgumentError(None, message="Expected no more than 1 target argument")
+    else:
+        pos = 1
+    args.target = (args._positionals[:pos] or [ProjectBuildTargets.MAIN_TARGET])[0]
+    args.extra_args = args._positionals[pos + has_sep :]
+
+    show_plugin_help = "-h" in args.extra_args or "--help" in args.extra_args
+
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
-        if args.project_dir:
+        if not show_plugin_help:
             raise
 
     if project is not None:
         env = project.env
     else:
         env = Environment()
 
-    target_dataset, _project = parse_full_revpath(args.target, project)
-    if _project is not None:
-        scope_add(_project)
-
     try:
-        exporter = env.exporters[target_dataset.format]
+        exporter = env.exporters[args.format]
     except KeyError:
         raise CliException("Exporter for format '%s' is not found" % args.format)
 
     extra_args = exporter.parse_cmdline(args.extra_args)
 
-    dst_dir = args.dst_dir or target_dataset.data_path
-    if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
-        raise CliException(
-            "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
-        )
+    dst_dir = args.dst_dir
+    if dst_dir:
+        if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
+            raise CliException(
+                "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
+            )
+    else:
+        dst_dir = generate_next_file_name("export-%s" % make_file_name(args.format))
     dst_dir = osp.abspath(dst_dir)
 
-    patch_dataset, _project = parse_full_revpath(args.patch, project)
-    if _project is not None:
-        scope_add(_project)
+    if args.filter:
+        filter_args = FilterModes.make_filter_args(args.filter_mode)
+        filter_expr = args.filter
+
+    log.info("Loading the project...")
+
+    dataset = project.working_tree.make_dataset(args.target)
+    if args.filter:
+        dataset.filter(filter_expr, **filter_args)
 
-    target_dataset.update(patch_dataset)
+    log.info("Exporting...")
 
-    target_dataset.save(save_dir=dst_dir, **extra_args)
+    dataset.export(save_dir=dst_dir, format=exporter, **extra_args)
 
-    log.info("Patched dataset has been saved to '%s'" % dst_dir)
+    log.info("Results have been saved to '%s'" % dst_dir)
 
     return 0
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/search.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/commands/status.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 
 from datumaro.cli.util import MultilineFormatter
 from datumaro.util.scope import scope_add, scoped
 
-from ..util.project import load_project
+from ....util.project import load_project
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Prints project status.",
         description="""
         This command prints the summary of the project changes between
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/transform.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 from datumaro.components.environment import Environment
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.errors import CliException
-from ..util.project import load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.errors import CliException
+from ....util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     builtins = sorted(Environment().transforms)
 
     parser = parser_ctor(
         help="Transform project",
```

### Comparing `datumaro-1.1.1/datumaro/cli/commands/validate.py` & `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from datumaro.components.environment import Environment
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.validator import TaskType
 from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.errors import CliException
-from ..util.project import generate_next_file_name, load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.errors import CliException
+from ....util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Validate project",
         description="""
         Validates a dataset according to the task type and
@@ -42,15 +42,15 @@
     )
 
     task_types = ", ".join(t.name for t in TaskType)
 
     def _parse_task_type(s):
         try:
             return TaskType[s.lower()].name
-        except:
+        except Exception:
             raise argparse.ArgumentTypeError(
                 "Unknown task type %s. Expected " "one of: %s" % (s, task_types)
             )
 
     parser.add_argument(
         "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
     )  # workaround for -- eaten by positionals
@@ -122,15 +122,15 @@
 
     extra_args = validator_type.parse_cmdline(args.extra_args)
 
     dataset, target_project = parse_full_revpath(args.target, project)
     if target_project:
         scope_add(target_project)
 
-    dst_file_name = f"validation-report"
+    dst_file_name = "validation-report"
     if args.subset_name is not None:
         dataset = dataset.get_subset(args.subset_name)
         dst_file_name += f"-{args.subset_name}"
 
     validator = validator_type(**extra_args)
     report = validator.validate(dataset)
```

### Comparing `datumaro-1.1.1/datumaro/cli/contexts/model.py` & `datumaro-1.2.0rc1/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/contexts/project/diff.py` & `datumaro-1.2.0rc1/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/contexts/util.py` & `datumaro-1.2.0rc1/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/cli/util/__init__.py` & `datumaro-1.2.0rc1/datumaro/cli/util/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -36,14 +36,35 @@
             formatted_paragraph = (
                 textwrap.fill(paragraph, width, initial_indent=indent, subsequent_indent=indent)
                 + "\n"
             )
             multiline_text += formatted_paragraph
         return multiline_text
 
+    def _format_action(self, action):
+        """
+        This requires to remove an ugly curly braced list generated by add_subparsers().
+        Please see the following example.
+
+        <w/o this patch>
+            Commands:
+            {get,describe}
+                get           Download a publicly available dataset
+                describe      Print information about downloadable datasets
+
+        <w/ this patch>
+            Commands:
+                get           Download a publicly available dataset
+                describe      Print information about downloadable datasets
+        """
+        parts = super()._format_action(action)
+        if action.nargs == argparse.PARSER:
+            parts = "\n".join(parts.split("\n")[1:])
+        return parts
+
 
 def required_count(nmin=0, nmax=0):
     assert 0 <= nmin and 0 <= nmax and nmin or nmax
 
     class RequiredCount(argparse.Action):
         def __call__(self, parser, args, values, option_string=None):
             k = len(values)
@@ -82,9 +103,23 @@
 def show_video_import_warning():
     log.warning(
         "Using 'video_frames' in a project may lead "
         "to different results across multiple runs, if the "
         "system setup changes (library version, OS, etc.). "
         "If you need stable results, consider splitting the video "
         "manually using instructions at: "
-        "https://openvinotoolkit.github.io/datumaro/docs/user-manual/media_formats/"
+        "https://openvinotoolkit.github.io/datumaro/docs/media_formats/"
     )
+
+
+def make_subcommands_help(commands, help_line_start=0):
+    desc = ""
+    for command_name, command_type, command_help in commands:
+        msg = ("  %-" + str(max(0, help_line_start - 2 - 1)) + "s%s\n") % (
+            command_name,
+            command_help,
+        )
+        if command_type is None:
+            msg = msg.lstrip()  # un-indent for not subparser
+        desc += msg
+
+    return desc
```

### Comparing `datumaro-1.1.1/datumaro/cli/util/project.py` & `datumaro-1.2.0rc1/datumaro/cli/util/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import re
+from enum import Enum
 from typing import Optional, Tuple
 
 from datumaro.cli.util.errors import WrongRevpathError
 from datumaro.components.dataset import Dataset
 from datumaro.components.environment import DEFAULT_ENVIRONMENT, Environment
 from datumaro.components.errors import DatumaroError, ProjectNotFoundError
 from datumaro.components.project import Project, Revision
 from datumaro.util.os_util import generate_next_name
 from datumaro.util.scope import on_error_do, scoped
 
 
 def load_project(project_dir, readonly=False):
+    """load a Project."""
     return Project(project_dir, readonly=readonly)
 
 
 def generate_next_file_name(basename, basedir=".", sep=".", ext=""):
     """
     If basedir does not contain basename, returns basename,
     otherwise generates a name by appending sep to the basename
@@ -147,22 +149,60 @@
 
 def split_local_revpath(revpath: str) -> Tuple[Revision, str]:
     """
     Splits the given string into revpath components.
 
     A local revpath is a path to a revision withing the current project.
     The syntax is:
-        - [ <revision> : ] [ <target> ]
+      - [ <revision> : ] [ <target> ]
     At least one part must be present.
 
     Returns: (revision, build target)
     """
 
     sep_pos = revpath.find(":")
     if -1 < sep_pos:
         rev = revpath[:sep_pos]
         target = revpath[sep_pos + 1 :]
     else:
         rev = ""
         target = revpath
 
     return rev, target
+
+
+class FilterModes(Enum):
+    # primary
+    items = 1
+    annotations = 2
+    items_annotations = 3
+
+    # shortcuts
+    i = 1
+    a = 2
+    i_a = 3
+    a_i = 3
+    annotations_items = 3
+
+    @staticmethod
+    def parse(s):
+        s = s.lower()
+        s = s.replace("+", "_")
+        return FilterModes[s]
+
+    @classmethod
+    def make_filter_args(cls, mode):
+        if mode == cls.items:
+            return {}
+        elif mode == cls.annotations:
+            return {"filter_annotations": True}
+        elif mode == cls.items_annotations:
+            return {
+                "filter_annotations": True,
+                "remove_empty": True,
+            }
+        else:
+            raise NotImplementedError()
+
+    @classmethod
+    def list_options(cls):
+        return [m.name.replace("_", "+") for m in cls]
```

### Comparing `datumaro-1.1.1/datumaro/components/algorithms/rise.py` & `datumaro-1.2.0rc1/datumaro/components/algorithms/rise.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from math import ceil
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType
 from datumaro.util.annotation_util import nms
 
+__all__ = ["RISE"]
 
-def flatmatvec(mat):
+
+def _flatmatvec(mat):
     return np.reshape(mat, (len(mat), -1))
 
 
-def expand(array, axis=None):
+def _expand(array, axis=None):
     if axis is None:
         axis = len(array.shape)
     return np.expand_dims(array, axis=axis)
 
 
 class RISE:
     """
@@ -60,18 +62,18 @@
                 labels.append(r)
             elif r.type is AnnotationType.bbox:
                 bboxes.append(r)
         return labels, bboxes
 
     def normalize_hmaps(self, heatmaps, counts):
         eps = np.finfo(heatmaps.dtype).eps
-        mhmaps = flatmatvec(heatmaps)
-        mhmaps /= expand(counts * self.prob + eps)
-        mhmaps -= expand(np.min(mhmaps, axis=1))
-        mhmaps /= expand(np.max(mhmaps, axis=1) + eps)
+        mhmaps = _flatmatvec(heatmaps)
+        mhmaps /= _expand(counts * self.prob + eps)
+        mhmaps -= _expand(np.min(mhmaps, axis=1))
+        mhmaps /= _expand(np.max(mhmaps, axis=1) + eps)
         return np.reshape(mhmaps, heatmaps.shape)
 
     def apply(self, image, progressive=False):
         import cv2
 
         assert len(image.shape) in [2, 3], "Expected an input image in (H, W, C) format"
         if len(image.shape) == 3:
@@ -88,15 +90,15 @@
 
         rng = lambda shape=None: np.random.rand(*shape)
         samples = np.prod(image_size)
         if self.max_samples is not None:
             samples = min(self.max_samples, samples)
         batch_size = self.batch_size
 
-        result = next(iter(model.launch(expand(image, 0))))
+        result = next(iter(model.launch(_expand(image, 0))))
         result_labels, result_bboxes = self.split_outputs(result)
         if 0 < self.det_conf_thresh:
             result_bboxes = [
                 b for b in result_bboxes if self.det_conf_thresh <= b.attributes["score"]
             ]
         if 0 < self.nms_thresh:
             result_bboxes = nms(result_bboxes, self.nms_thresh)
@@ -115,30 +117,30 @@
         heatmaps_count = len(predicted_labels) + len(predicted_bboxes)
         heatmaps = np.zeros((heatmaps_count, *image_size), dtype=np.float32)
         total_counts = np.zeros(heatmaps_count, dtype=np.int32)
         confs = np.zeros(heatmaps_count, dtype=np.float32)
 
         heatmap_id = 0
 
-        label_heatmaps = None
+        # label_heatmaps = None
         label_total_counts = None
         label_confs = None
         if len(predicted_labels) != 0:
             step = len(predicted_labels)
-            label_heatmaps = heatmaps[heatmap_id : heatmap_id + step]
+            # label_heatmaps = heatmaps[heatmap_id : heatmap_id + step]
             label_total_counts = total_counts[heatmap_id : heatmap_id + step]
             label_confs = confs[heatmap_id : heatmap_id + step]
             heatmap_id += step
 
-        bbox_heatmaps = None
+        # bbox_heatmaps = None
         bbox_total_counts = None
         bbox_confs = None
         if len(predicted_bboxes) != 0:
             step = len(predicted_bboxes)
-            bbox_heatmaps = heatmaps[heatmap_id : heatmap_id + step]
+            # bbox_heatmaps = heatmaps[heatmap_id : heatmap_id + step]
             bbox_total_counts = total_counts[heatmap_id : heatmap_id + step]
             bbox_confs = confs[heatmap_id : heatmap_id + step]
             heatmap_id += step
 
         ups_mask = np.empty(upsampled_size.astype(int), dtype=np.float32)
         masks = np.empty((batch_size, *image_size), dtype=np.float32)
 
@@ -157,15 +159,15 @@
                 mask = ups_mask[
                     int(offsets[0]) : int(image_size[0] + offsets[0]),
                     int(offsets[1]) : int(image_size[1] + offsets[1]),
                 ]
                 batch_masks[i] = mask
 
             batch_inputs = full_batch_inputs[:current_batch_size]
-            np.multiply(expand(batch_masks), expand(image, 0), out=batch_inputs)
+            np.multiply(_expand(batch_masks), _expand(image, 0), out=batch_inputs)
 
             results = model.launch(batch_inputs)
             for mask, result in zip(batch_masks, results):
                 result_labels, result_bboxes = self.split_outputs(result)
 
                 confs.fill(0)
                 if len(predicted_labels) != 0:
```

### Comparing `datumaro-1.1.1/datumaro/components/annotation.py` & `datumaro-1.2.0rc1/datumaro/components/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,16 +685,21 @@
         if (
             not Annotation.__eq__(self, other)
             or self.label != other.label
             or self.z_order != other.z_order
         ):
             return False
 
-        self_polygon = sg.Polygon(self.get_points())
-        other_polygon = sg.Polygon(other.get_points())
+        self_points = self.get_points()
+        other_points = other.get_points()
+        self_polygon = sg.Polygon(self_points)
+        other_polygon = sg.Polygon(other_points)
+        # if polygon is not valid, compare points
+        if not (self_polygon.is_valid and other_polygon.is_valid):
+            return self_points == other_points
         inter_area = self_polygon.intersection(other_polygon).area
         return abs(self_polygon.area - inter_area) < CHECK_POLYGON_EQ_EPSILONE
 
 
 @attrs(slots=True, init=False, order=False)
 class Bbox(_Shape):
     _type = AnnotationType.bbox
```

### Comparing `datumaro-1.1.1/datumaro/components/cli_plugin.py` & `datumaro-1.2.0rc1/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/config.py` & `datumaro-1.2.0rc1/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/config_model.py` & `datumaro-1.2.0rc1/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/crypter.py` & `datumaro-1.2.0rc1/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/dataset.py` & `datumaro-1.2.0rc1/datumaro/components/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     UnknownFormatError,
 )
 from datumaro.components.exporter import ExportContext, Exporter, ExportErrorPolicy, _ExportFail
 from datumaro.components.filter import XPathAnnotationsFilter, XPathDatasetFilter
 from datumaro.components.importer import ImportContext, ImportErrorPolicy, _ImportFail
 from datumaro.components.launcher import Launcher, ModelTransform
 from datumaro.components.media import Image, MediaElement
+from datumaro.components.merge import DEFAULT_MERGE_POLICY
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
 from datumaro.components.transformer import ItemTransform, Transform
 from datumaro.plugins.transforms import ProjectLabels
 from datumaro.util import is_method_redefined
 from datumaro.util.log_utils import logging_disabled
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scoped
@@ -335,15 +336,18 @@
     def get_annotated_type(self):
         annotation_types = []
         for item in self.parent._data.get_subset(self.name):
             annotation_types.extend([str(anno.type).split(".")[-1] for anno in item.annotations])
         return list(set(annotation_types))
 
     def as_dataset(self) -> Dataset:
-        return Dataset.from_extractors(self, env=self.parent.env)
+        dataset = Dataset.from_extractors(self, env=self.parent.env)
+        dataset._format = self.parent._format
+        dataset._source_path = self.parent._source_path
+        return dataset
 
 
 class DatasetStorage(IDataset):
     def __init__(
         self,
         source: Union[IDataset, DatasetItemStorage] = None,
         infos: Optional[DatasetInfo] = None,
@@ -872,37 +876,41 @@
             def categories(self):
                 return categories
 
         return cls.from_extractors(_extractor(), env=env)
 
     @staticmethod
     def from_extractors(
-        *sources: IDataset, env: Optional[Environment] = None, merge_policy: str = None
+        *sources: IDataset,
+        env: Optional[Environment] = None,
+        merge_policy: str = DEFAULT_MERGE_POLICY,
     ) -> Dataset:
         """
         Creates a new dataset from one or several `Extractor`s.
 
         In case of a single input, creates a lazy wrapper around the input.
         In case of several inputs, merges them and caches the resulting
         dataset.
 
         Parameters:
             sources: one or many input extractors
             env: A context for plugins, which will be used for this dataset.
                 If not specified, the builtin plugins will be used.
+            merge_policy: Policy on how to merge multiple datasets.
+                Possible options are "exact", "intersect", and "union".
 
         Returns:
             dataset: A new dataset with contents produced by input extractors
         """
 
         if len(sources) == 1:
             source = sources[0]
             dataset = Dataset(source=source, env=env)
         else:
-            from datumaro.components.merger import get_merger
+            from datumaro.components.merge import get_merger
 
             merger = get_merger(merge_policy)
 
             categories = merger.merge_categories(s.categories() for s in sources)
             infos = merger.merge_infos(s.infos() for s in sources)
             media_type = merger.merge_media_types(sources)
             source = merger.merge(*sources)
@@ -990,15 +998,15 @@
     def get_annotated_items(self):
         return self._data.get_annotated_items()
 
     def get_annotations(self):
         return self._data.get_annotations()
 
     def get_datasetitem_by_path(self, path):
-        if not self._source_path in path:
+        if self._source_path not in path:
             path = osp.join(self._source_path, path)
         return self._data.get_datasetitem_by_path(path)
 
     def get_subset_info(self):
         return (
             f"{subset_name}: # of items={len(self.get_subset(subset_name))}, "
             f"# of annotated items={self.get_subset(subset_name).get_annotated_items()}, "
@@ -1381,28 +1389,26 @@
 
         if not progress_reporter:
             progress_reporter = NullProgressReporter()
         pbars = progress_reporter.split(len(detected_sources))
 
         try:
             extractors = []
-            merge_policy = None
             for src_conf, pbar in zip(detected_sources, pbars):
                 if not isinstance(src_conf, Source):
                     src_conf = Source(src_conf)
 
                 extractor_kwargs = dict(src_conf.options)
 
                 assert "ctx" not in extractor_kwargs
                 extractor_kwargs["ctx"] = ImportContext(
                     progress_reporter=pbar, error_policy=error_policy
                 )
 
-                if not merge_policy:
-                    merge_policy = extractor_kwargs.get("merge_policy", None)
+                merge_policy = extractor_kwargs.get("merge_policy", DEFAULT_MERGE_POLICY)
 
                 try:
                     extractors.append(
                         env.make_extractor(src_conf.format, src_conf.url, **extractor_kwargs)
                     )
                 except TypeError as e:
                     # TODO: for backward compatibility. To be removed after 0.3
```

### Comparing `datumaro-1.1.1/datumaro/components/dataset_base.py` & `datumaro-1.2.0rc1/datumaro/components/dataset_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,19 @@
         if image is not None:
             warnings.warn(
                 "'image' is deprecated and will be " "removed in future. Use 'media' instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             if isinstance(image, str):
-                image = Image(path=image)
-            elif isinstance(image, np.ndarray) or callable(image):
-                image = Image(data=image)
+                image = Image.from_file(path=image)
+            elif isinstance(image, np.ndarray):
+                image = Image.from_numpy(data=image)
+            elif isinstance(image, bytes) or callable(image):
+                image = Image.from_bytes(data=image)
             assert isinstance(image, Image)
             media = image
         elif point_cloud is not None:
             warnings.warn(
                 "'point_cloud' is deprecated and will be "
                 "removed in future. Use 'media' instead.",
                 DeprecationWarning,
@@ -77,15 +79,17 @@
                 warnings.warn(
                     "'related_images' is deprecated and will be "
                     "removed in future. Use 'media' instead.",
                     DeprecationWarning,
                     stacklevel=2,
                 )
             if isinstance(point_cloud, str):
-                point_cloud = PointCloud(path=point_cloud, extra_images=related_images)
+                point_cloud = PointCloud.from_file(path=point_cloud, extra_images=related_images)
+            elif isinstance(point_cloud, bytes):
+                point_cloud = PointCloud.from_bytes(data=point_cloud, extra_images=related_images)
             assert isinstance(point_cloud, PointCloud)
             media = point_cloud
 
         self.__attrs_init__(
             id=id, subset=subset, media=media, annotations=annotations, attributes=attributes
         )
```

### Comparing `datumaro-1.1.1/datumaro/components/environment.py` & `datumaro-1.2.0rc1/datumaro/components/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             exports = module.exports
         else:
             for symbol in dir(module):
                 if symbol.startswith("_"):
                     continue
                 exports.append(getattr(module, symbol))
 
-        exports = [s for s in exports if isclass(s) and issubclass(s, types) and not s in types]
+        exports = [s for s in exports if isclass(s) and issubclass(s, types) and s not in types]
 
         return exports
 
     @classmethod
     def _load_plugins(cls, module_names, *, importer, types=None):
         types = tuple(types or plugin_types())
```

### Comparing `datumaro-1.1.1/datumaro/components/errors.py` & `datumaro-1.2.0rc1/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/exporter.py` & `datumaro-1.2.0rc1/datumaro/components/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,44 +269,42 @@
             return
 
         basedir = basedir or self._save_dir
         path = path or osp.join(basedir, self._make_pcd_filename(item, name=name, subdir=subdir))
         path = osp.abspath(path)
 
         os.makedirs(osp.dirname(path), exist_ok=True)
-        if item.media and osp.isfile(item.media.path):
-            if item.media.path != path:
-                shutil.copyfile(item.media.path, path)
+        item.media.save(path, crypter=NULL_CRYPTER)
 
     def _save_meta_file(self, path):
         save_meta_file(path, self._extractor.categories())
 
 
-# TODO: Currently, ExportContextComponent is introduced only for Datumaro and DatumaroBinary format for multi-processing.
-# We need to propagate this to everywhere in Datumaro 1.2.0
+# TODO: Currently, ExportContextComponent is introduced only for Datumaro and DatumaroBinary format
+# for multi-processing. We need to propagate this to everywhere in Datumaro 1.2.0
 class ExportContextComponent:
     def __init__(
         self,
         save_dir: str,
         save_media: bool,
         images_dir: str,
         pcd_dir: str,
-        related_images_dir: str,
         crypter: Crypter = NULL_CRYPTER,
         image_ext: Optional[str] = None,
         default_image_ext: Optional[str] = None,
+        source_path: Optional[str] = None,
     ):
         self._save_dir = save_dir
         self._save_media = save_media
         self._images_dir = images_dir
         self._pcd_dir = pcd_dir
-        self._related_images_dir = related_images_dir
         self._crypter = crypter
         self._image_ext = image_ext
         self._default_image_ext = default_image_ext
+        self._source_path = source_path
 
     def find_image_ext(self, item: Union[DatasetItem, Image]):
         src_ext = None
 
         if isinstance(item, DatasetItem) and isinstance(item.media, Image):
             src_ext = item.media.ext
         elif isinstance(item, Image):
@@ -321,14 +319,19 @@
 
     def make_image_filename(self, item, *, name=None, subdir=None):
         return self._make_item_filename(item, name=name, subdir=subdir) + self.find_image_ext(item)
 
     def make_pcd_filename(self, item, *, name=None, subdir=None):
         return self._make_item_filename(item, name=name, subdir=subdir) + ".pcd"
 
+    def make_pcd_extra_image_filename(self, item, idx, image, *, name=None, subdir=None):
+        return self._make_item_filename(
+            item, name=name if name else f"{item.id}/extra_image_{idx}", subdir=subdir
+        ) + self.find_image_ext(image)
+
     def save_image(
         self,
         item: DatasetItem,
         *,
         encryption: bool = False,
         basedir: Optional[str] = None,
         subdir: Optional[str] = None,
@@ -362,34 +365,38 @@
         basedir = self._pcd_dir if basedir is None else basedir
         basedir = osp.join(basedir, subdir) if subdir is not None else basedir
         fname = self.make_pcd_filename(item) if fname is None else fname
         path = osp.join(basedir, fname)
         path = osp.abspath(path)
 
         os.makedirs(osp.dirname(path), exist_ok=True)
-        if item.media and osp.isfile(item.media.path):
-            if item.media.path != path:
-                shutil.copyfile(item.media.path, path)
+
+        def helper(i, image):
+            basedir = self._images_dir
+            basedir = osp.join(basedir, subdir) if subdir is not None else basedir
+            return {"fp": osp.join(basedir, self.make_pcd_extra_image_filename(item, i, image))}
+
+        item.media.save(path, helper, crypter=NULL_CRYPTER)
 
     @property
     def images_dir(self) -> str:
         return self._images_dir
 
     @property
     def pcd_dir(self) -> str:
         return self._pcd_dir
 
     @property
-    def related_images_dir(self) -> str:
-        return self._related_images_dir
-
-    @property
     def save_dir(self) -> str:
         return self._save_dir
 
     @property
     def save_media(self) -> bool:
         return self._save_media
 
     @property
     def crypter(self) -> Crypter:
         return self._crypter
+
+    @property
+    def source_path(self) -> str:
+        return self._source_path if self._source_path else ""
```

### Comparing `datumaro-1.1.1/datumaro/components/extractor_tfds.py` & `datumaro-1.2.0rc1/datumaro/components/extractor_tfds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# Copyright (C) 2021-2022 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import itertools
 import logging as log
 import os.path as osp
 from types import SimpleNamespace as namespace
 from typing import Any, Callable, Dict, Iterator, Mapping, Optional, Sequence, Tuple, Type, Union
 
 import attrs
+import numpy as np
 from attrs import field, frozen
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, DatasetItem, IDataset
-from datumaro.components.media import ByteImage, Image, MediaElement
+from datumaro.components.media import Image, MediaElement
 from datumaro.util.tf_util import import_tf
 
 try:
     tf = import_tf()
     import tensorflow_datasets as tfds
 except ImportError:
     log.debug(
@@ -136,18 +137,22 @@
         self,
         tfds_example: Any,
         item: DatasetItem,
         state: namespace,
     ) -> None:
         if self.filename_feature_name:
             filename = tfds_example[self.filename_feature_name].numpy().decode("UTF-8")
+            if osp.exists(filename):
+                item.media = Image.from_file(path=filename)
+                return
+        data = tfds_example[self.feature_name].numpy()
+        if isinstance(data, np.ndarray):
+            item.media = Image.from_numpy(data=data)
         else:
-            filename = None
-
-        item.media = ByteImage(data=tfds_example[self.feature_name].numpy(), path=filename)
+            item.media = Image.from_bytes(data=data)
 
 
 @frozen
 class _AddLabelFromClassLabelFeature:
     feature_name: str
 
     def __call__(
@@ -309,14 +314,39 @@
     ],
     id_generator=_GenerateIdFromFilenameFeature("file_name"),
     metadata=TfdsDatasetMetadata(
         human_name="ImageNet", default_output_format="imagenet_txt", media_type=Image
     ),
 )
 
+_EUROSAT_ADAPTER = _TfdsAdapter(
+    category_transformers=[_SetLabelCategoriesFromClassLabelFeature("label")],
+    data_transformers=[
+        _SetImageFromImageFeature("image"),
+        _AddLabelFromClassLabelFeature("label"),
+    ],
+    id_generator=_GenerateIdFromFilenameFeature("filename"),
+    metadata=TfdsDatasetMetadata(
+        human_name="EuroSAT", default_output_format="imagenet_txt", media_type=Image
+    ),
+)
+
+
+_UC_MERCED_ADAPTER = _TfdsAdapter(
+    category_transformers=[_SetLabelCategoriesFromClassLabelFeature("label")],
+    data_transformers=[
+        _SetImageFromImageFeature("image"),
+        _AddLabelFromClassLabelFeature("label"),
+    ],
+    id_generator=_GenerateIdFromFilenameFeature("filename"),
+    metadata=TfdsDatasetMetadata(
+        human_name="UCMerced", default_output_format="imagenet_txt", media_type=Image
+    ),
+)
+
 
 def _voc_save_pose_names(
     tfds_builder: tfds.core.DatasetBuilder,
     categories: CategoriesInfo,
     state: namespace,
 ) -> None:
     # TFDS represents poses as indexes, but Datumaro represents them as strings.
@@ -365,14 +395,16 @@
 _TFDS_ADAPTERS = {
     "cifar10": _evolve_adapter_meta(_CIFAR_ADAPTER, human_name="CIFAR-10"),
     "cifar100": _evolve_adapter_meta(_CIFAR_ADAPTER, human_name="CIFAR-100"),
     "coco/2014": _evolve_adapter_meta(_COCO_ADAPTER, human_name="COCO (2014-2015)"),
     "imagenet_v2": _evolve_adapter_meta(_IMAGENET_ADAPTER, human_name="ImageNetV2"),
     "mnist": _MNIST_ADAPTER,
     "voc/2012": _evolve_adapter_meta(_VOC_ADAPTER, human_name="PASCAL VOC 2012"),
+    "eurosat": _evolve_adapter_meta(_EUROSAT_ADAPTER, human_name="EuroSAT"),
+    "uc_merced": _evolve_adapter_meta(_UC_MERCED_ADAPTER, human_name="UCMerced"),
 }
 
 # Assign the TFDS catalog page as the documentation URL for all datasets.
 _TFDS_ADAPTERS = {
     name: _evolve_adapter_meta(
         adapter,
         home_url="https://www.tensorflow.org/datasets/catalog/" + name.split("/", maxsplit=1)[0],
```

### Comparing `datumaro-1.1.1/datumaro/components/filter.py` & `datumaro-1.2.0rc1/datumaro/components/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 
 # Disable B410: import_lxml - the library is used for writing
-from lxml import etree as ET  # nosec, lxml has proper XPath implementation
+from lxml import etree as ET  # nosec
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     Bbox,
     Caption,
     Ellipse,
@@ -49,15 +49,16 @@
         else:
             h = "unknown"
             w = h
         ET.SubElement(image_elem, "width").text = str(w)
         ET.SubElement(image_elem, "height").text = str(h)
 
         ET.SubElement(image_elem, "has_data").text = "%d" % int(image.has_data)
-        ET.SubElement(image_elem, "path").text = image.path
+        if hasattr(image, "path"):
+            ET.SubElement(image_elem, "path").text = image.path
 
         return image_elem
 
     @classmethod
     def encode_annotation_base(cls, annotation):
         assert isinstance(annotation, Annotation)
         ann_elem = ET.Element("annotation")
```

### Comparing `datumaro-1.1.1/datumaro/components/format_detection.py` & `datumaro-1.2.0rc1/datumaro/components/format_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # the dataset belongs to the format; for example, because the format
     # has explicit identification via magic numbers/files.
 
 
 @dataclass(order=True, frozen=True)
 class DetectedFormat:
     confidence: FormatDetectionConfidence = field(compare=True)
-    name: str
+    name: str = field(compare=False)
 
     def __eq__(self, __o: "DetectedFormat") -> bool:
         return self.name == __o.name
 
     def __str__(self) -> str:
         return self.name
```

### Comparing `datumaro-1.1.1/datumaro/components/generator.py` & `datumaro-1.2.0rc1/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/hl_ops.py` & `datumaro-1.2.0rc1/datumaro/components/hl_ops/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,219 +1,246 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import inspect
 import os
 import os.path as osp
 import shutil
-from typing import Dict, Optional, Type, Union
+from typing import Dict, Iterable, Optional, Type, Union
 
 from datumaro.components.dataset import Dataset, DatasetItemStorageDatasetView, IDataset
 from datumaro.components.environment import Environment
+from datumaro.components.errors import DatasetError
 from datumaro.components.exporter import Exporter
 from datumaro.components.filter import XPathAnnotationsFilter, XPathDatasetFilter
 from datumaro.components.launcher import Launcher, ModelTransform
-from datumaro.components.operations import ExactMerge
+from datumaro.components.merge.exact_merge import ExactMerge
 from datumaro.components.transformer import Transform
 from datumaro.components.validator import TaskType, Validator
 from datumaro.util import parse_str_enum_value
 from datumaro.util.scope import on_error_do, scoped
 
+__all__ = ["HLOps"]
 
-def transform(
-    dataset: IDataset,
-    method: Union[str, Type[Transform]],
-    *,
-    env: Optional[Environment] = None,
-    **kwargs,
-) -> IDataset:
-    """
-    Applies some function to dataset items.
-
-    Results are computed lazily, if the transform supports this.
-
-    Args:
-        dataset: The dataset to be transformed
-        method: The transformation to be applied to the dataset.
-            If a string is passed, it is treated as a plugin name,
-            which is searched for in the environment
-            set by the 'env' argument
-        env: A plugin collection. If not set, the built-in plugins are used
-        **kwargs: Parameters for the transformation
 
-    Returns: a wrapper around the input dataset
-    """
+class HLOps:
+    """High-level dataset operations for Python API."""
 
-    if isinstance(method, str):
-        if env is None:
-            env = Environment()
-        method = env.transforms[method]
-
-    if not (inspect.isclass(method) and issubclass(method, Transform)):
-        raise TypeError("Unexpected 'method' argument type: %s" % type(method))
-
-    produced = method(dataset, **kwargs)
-
-    return Dataset(source=produced, env=env)
-
-
-def filter(
-    dataset: IDataset,
-    expr: str,
-    *,  # pylint: disable=redefined-builtin
-    filter_annotations: bool = False,
-    remove_empty: bool = False,
-) -> IDataset:
-    """
-    Filters out some dataset items or annotations, using a custom filter
-    expression.
-
-    Args:
-        dataset: The dataset to be filtered
-        expr: XPath-formatted filter expression
-            (e.g. `/item[subset = 'train']`, `/item/annotation[label = 'cat']`)
-        filter_annotations: Indicates if the filter should be
-            applied to items or annotations
-        remove_empty: When filtering annotations, allows to
-            exclude empty items from the resulting dataset
-
-    Returns: a wrapper around the input dataset, which is computed lazily
-        during iteration
-    """
-
-    if filter_annotations:
-        return transform(dataset, XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty)
-    else:
-        if not expr:
-            return dataset
-        return transform(dataset, XPathDatasetFilter, xpath=expr)
-
-
-def merge(*datasets: IDataset) -> IDataset:
-    """
-    Merges several datasets using the "simple" (exact matching) algorithm:
-
-        - items are matched by (id, subset) pairs
-        - matching items share the fields available
-
-            - nothing + nothing = nothing,
-            - nothing + something = something
-            - something A + something B = conflict
-        - annotations are matched by value and shared
-        - in case of conflicts, throws an error
-
-    Returns: a wrapper around the input datasets
-    """
-
-    merger = ExactMerge()
-    infos = merger.merge_infos(d.infos() for d in datasets)
-    categories = merger.merge_categories(d.categories() for d in datasets)
-    media_type = merger.merge_media_types(datasets)
-    return DatasetItemStorageDatasetView(
-        merger.merge(*datasets), infos=infos, categories=categories, media_type=media_type
-    )
-
-
-def run_model(
-    dataset: IDataset,
-    model: Union[Launcher, Type[ModelTransform]],
-    *,
-    batch_size: int = 1,
-    append_annotation: bool = False,
-    **kwargs,
-) -> IDataset:
-    """
-    Applies a model to dataset items' media and produces a dataset with
-    media and annotations.
-
-    Args:
-        dataset: The dataset to be transformed
-        model: The model to be applied to the dataset
-        batch_size: The number of dataset items processed
-            simultaneously by the model
-        append_annotation: Whether append new annotation to existed annotations
-        **kwargs: Parameters for the model
-
-    Returns: a wrapper around the input dataset, which is computed lazily
-        during iteration
-    """
-
-    if isinstance(model, Launcher):
-        return transform(
-            dataset,
-            ModelTransform,
-            launcher=model,
-            batch_size=batch_size,
-            append_annotation=append_annotation,
-            **kwargs,
+    @staticmethod
+    def transform(
+        dataset: IDataset,
+        method: Union[str, Type[Transform]],
+        *,
+        env: Optional[Environment] = None,
+        **kwargs,
+    ) -> IDataset:
+        """
+        Applies some function to dataset items.
+
+        Results are computed lazily, if the transform supports this.
+
+        Args:
+            dataset: The dataset to be transformed
+            method: The transformation to be applied to the dataset.
+                If a string is passed, it is treated as a plugin name,
+                which is searched for in the environment
+                set by the 'env' argument
+            env: A plugin collection. If not set, the built-in plugins are used
+            **kwargs: Parameters for the transformation
+
+        Returns: a wrapper around the input dataset
+        """
+
+        if isinstance(method, str):
+            if env is None:
+                env = Environment()
+            method = env.transforms[method]
+
+        if not (inspect.isclass(method) and issubclass(method, Transform)):
+            raise TypeError(f"Unexpected 'method' argument type: {type(method)}")
+
+        produced = method(dataset, **kwargs)
+
+        return Dataset(source=produced, env=env)
+
+    @staticmethod
+    def filter(
+        dataset: IDataset,
+        expr: str,
+        *,  # pylint: disable=redefined-builtin
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
+    ) -> IDataset:
+        """
+        Filters out some dataset items or annotations, using a custom filter
+        expression.
+
+        Args:
+            dataset: The dataset to be filtered
+            expr: XPath-formatted filter expression
+                (e.g. `/item[subset = 'train']`, `/item/annotation[label = 'cat']`)
+            filter_annotations: Indicates if the filter should be
+                applied to items or annotations
+            remove_empty: When filtering annotations, allows to
+                exclude empty items from the resulting dataset
+
+        Returns: a wrapper around the input dataset, which is computed lazily
+            during iteration
+        """
+
+        if filter_annotations:
+            return HLOps.transform(
+                dataset, XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty
+            )
+        else:
+            if not expr:
+                return dataset
+            return HLOps.transform(dataset, XPathDatasetFilter, xpath=expr)
+
+    @staticmethod
+    def merge(*datasets: IDataset) -> IDataset:
+        """
+        Merges several datasets using the "simple" (exact matching) algorithm:
+
+            - items are matched by (id, subset) pairs
+            - matching items share the fields available
+
+                - nothing + nothing = nothing,
+                - nothing + something = something
+                - something A + something B = conflict
+            - annotations are matched by value and shared
+            - in case of conflicts, throws an error
+
+        Returns: a wrapper around the input datasets
+        """
+
+        merger = ExactMerge()
+        infos = merger.merge_infos(d.infos() for d in datasets)
+        categories = merger.merge_categories(d.categories() for d in datasets)
+        media_type = merger.merge_media_types(datasets)
+        return DatasetItemStorageDatasetView(
+            merger.merge(*datasets), infos=infos, categories=categories, media_type=media_type
         )
-    elif inspect.isclass(model) and issubclass(model, ModelTransform):
-        return transform(
-            dataset, model, batch_size=batch_size, append_annotation=append_annotation, **kwargs
-        )
-    else:
-        raise TypeError("Unexpected model argument type: %s" % type(model))
 
+    @staticmethod
+    def run_model(
+        dataset: IDataset,
+        model: Union[Launcher, Type[ModelTransform]],
+        *,
+        batch_size: int = 1,
+        append_annotation: bool = False,
+        **kwargs,
+    ) -> IDataset:
+        """
+        Run the model on the dataset item media entities, such as images,
+        to obtain pseudo labels and add them as dataset annotations.
+
+        Args:
+            dataset: The dataset to be transformed
+            model: The model to be applied to the dataset
+            batch_size: The number of dataset items processed
+                simultaneously by the model
+            append_annotation: Whether append new annotation to existed annotations
+            **kwargs: Parameters for the model
+
+        Returns: a wrapper around the input dataset, which is computed lazily
+            during iteration
+        """
+
+        if isinstance(model, Launcher):
+            return HLOps.transform(
+                dataset,
+                ModelTransform,
+                launcher=model,
+                batch_size=batch_size,
+                append_annotation=append_annotation,
+                **kwargs,
+            )
+        elif inspect.isclass(model) and issubclass(model, ModelTransform):
+            return HLOps.transform(
+                dataset, model, batch_size=batch_size, append_annotation=append_annotation, **kwargs
+            )
+        else:
+            raise TypeError(f"Unexpected model argument type: {type(model)}")
+
+    @staticmethod
+    @scoped
+    def export(
+        dataset: IDataset,
+        path: str,
+        format: Union[str, Type[Exporter]],
+        *,
+        env: Optional[Environment] = None,
+        **kwargs,
+    ) -> None:
+        """
+        Saves the input dataset in some format.
+
+        Args:
+            dataset: The dataset to be saved
+            path: The output directory
+            format: The desired output format for the dataset.
+                If a string is passed, it is treated as a plugin name,
+                which is searched for in the environment set by the 'env' argument
+            env: A plugin collection. If not set, the built-in plugins are used
+            **kwargs: Parameters for the export format
+        """
+
+        if isinstance(format, str):
+            if env is None:
+                env = Environment()
+            exporter = env.exporters[format]
+        else:
+            exporter = format
+
+        if not (inspect.isclass(exporter) and issubclass(exporter, Exporter)):
+            raise TypeError(f"Unexpected 'format' argument type: {type(exporter)}")
+
+        path = osp.abspath(path)
+        if not osp.exists(path):
+            on_error_do(shutil.rmtree, path, ignore_errors=True)
+        os.makedirs(path, exist_ok=True)
+
+        exporter.convert(dataset, save_dir=path, **kwargs)
+
+    @staticmethod
+    def validate(
+        dataset: IDataset,
+        task: Union[str, TaskType],
+        *,
+        env: Optional[Environment] = None,
+        **kwargs,
+    ) -> Dict:
+        """
+        Checks dataset annotations for correctness relatively to a task type.
+
+        Args:
+            dataset: The dataset to check
+            task: Target task type - classification, detection etc.
+            env: A plugin collection. If not set, the built-in plugins are used
+            **kwargs: Parameters for the validator
+
+        Returns: a dictionary with validation results
+        """
 
-@scoped
-def export(
-    dataset: IDataset,
-    path: str,
-    format: Union[str, Type[Exporter]],
-    *,
-    env: Optional[Environment] = None,
-    **kwargs,
-) -> None:
-    """
-    Saves the input dataset in some format.
-
-    Args:
-        dataset: The dataset to be saved
-        path: The output directory
-        format: The desired output format for the dataset.
-            If a string is passed, it is treated as a plugin name,
-            which is searched for in the environment set by the 'env' argument
-        env: A plugin collection. If not set, the built-in plugins are used
-        **kwargs: Parameters for the export format
-    """
+        task = parse_str_enum_value(task, TaskType).name
 
-    if isinstance(format, str):
         if env is None:
             env = Environment()
-        exporter = env.exporters[format]
-    else:
-        exporter = format
 
-    if not (inspect.isclass(exporter) and issubclass(exporter, Exporter)):
-        raise TypeError("Unexpected 'format' argument type: %s" % type(exporter))
+        validator: Validator = env.validators[task](**kwargs)
+        return validator.validate(dataset)
 
-    path = osp.abspath(path)
-    if not osp.exists(path):
-        on_error_do(shutil.rmtree, path, ignore_errors=True)
-    os.makedirs(path, exist_ok=True)
+    @staticmethod
+    def aggregate(dataset: Dataset, from_subsets: Iterable[str], to_subset: str) -> Dataset:
+        subset_names = set(dataset.subsets().keys())
+
+        for subset in from_subsets:
+            if subset not in subset_names:
+                raise DatasetError(
+                    f"{subset} is not found in the subset names ({subset_names}) in the dataset."
+                )
 
-    exporter.convert(dataset, save_dir=path, **kwargs)
-
-
-def validate(
-    dataset: IDataset, task: Union[str, TaskType], *, env: Optional[Environment] = None, **kwargs
-) -> Dict:
-    """
-    Checks dataset annotations for correctness relatively to a task type.
-
-    Args:
-        dataset: The dataset to check
-        task: Target task type - classification, detection etc.
-        env: A plugin collection. If not set, the built-in plugins are used
-        **kwargs: Parameters for the validator
-
-    Returns: a dictionary with validation results
-    """
-
-    task = parse_str_enum_value(task, TaskType).name
-
-    if env is None:
-        env = Environment()
-
-    validator: Validator = env.validators[task](**kwargs)
-    return validator.validate(dataset)
+        return HLOps.transform(
+            dataset, "map_subsets", mapping={subset: to_subset for subset in from_subsets}
+        )
```

### Comparing `datumaro-1.1.1/datumaro/components/importer.py` & `datumaro-1.2.0rc1/datumaro/components/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,14 @@
                     )
                     if (callable(file_filter) and file_filter(p)) or (not callable(file_filter))
                 )
                 if sources:
                     break
         return sources
 
-    @classmethod
-    def get_extractor_name(cls) -> str:
-        return cls.NAME.replace("_importer", "")
-
 
 def with_subset_dirs(input_cls: Importer):
     @wraps(input_cls, updated=())
     class WrappedImporter(input_cls):
         NAME = input_cls.NAME
 
         @classmethod
```

### Comparing `datumaro-1.1.1/datumaro/components/launcher.py` & `datumaro-1.2.0rc1/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/media.py` & `datumaro-1.2.0rc1/datumaro/components/merge/intersect_merge.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,680 +1,559 @@
-# Copyright (C) 2021-2022 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
-
-import os
-import os.path as osp
-import shutil
-import weakref
-from enum import IntEnum
-from typing import Callable, Iterable, Iterator, List, Optional, Tuple, Union
-
-import cv2
-import numpy as np
-
-from datumaro.components.crypter import NULL_CRYPTER, Crypter
-from datumaro.components.errors import MediaShapeError
-from datumaro.util.definitions import BboxIntCoords
-from datumaro.util.image import (
-    _image_loading_errors,
-    copyto_image,
-    decode_image,
-    lazy_image,
-    save_image,
-)
+import logging as log
+from collections import OrderedDict
 
+import attr
+from attr import attrib, attrs
 
-class MediaType(IntEnum):
-    NONE = 0
-    MEDIA_ELEMENT = 1
-    IMAGE = 2
-    BYTE_IMAGE = 3
-    VIDEO_FRAME = 4
-    VIDEO = 5
-    POINT_CLOUD = 6
-    MULTIFRAME_IMAGE = 7
-    ROI_IMAGE = 8
-    MOSAIC_IMAGE = 9
-
-
-class MediaElement:
-    _type = MediaType.MEDIA_ELEMENT
-
-    def __init__(self, path: str, crypter: Crypter = NULL_CRYPTER) -> None:
-        assert path, "Path can't be empty"
-        self._path = path
-        self._crypter = crypter
-
-    @property
-    def path(self) -> str:
-        """Path to the media file"""
-        return self._path
-
-    @property
-    def ext(self) -> str:
-        """Media file extension (with the leading dot)"""
-        return osp.splitext(osp.basename(self.path))[1]
-
-    @property
-    def is_encrypted(self) -> bool:
-        return self._crypter.is_null_crypter
-
-    def set_crypter(self, crypter: Crypter):
-        self._crypter = crypter
-
-    def __eq__(self, other: object) -> bool:
-        # We need to compare exactly with this type
-        if type(other) is not __class__:  # pylint: disable=unidiomatic-typecheck
-            return False
-        return self._path == other._path
-
-    @property
-    def type(self) -> MediaType:
-        return self._type
-
-
-class Image(MediaElement):
-    _type = MediaType.IMAGE
-
-    def __init__(
-        self,
-        data: Union[np.ndarray, Callable[[str], np.ndarray], None] = None,
-        *,
-        path: Optional[str] = None,
-        ext: Optional[str] = None,
-        size: Optional[Tuple[int, int]] = None,
-        crypter: Crypter = NULL_CRYPTER,
-    ) -> None:
-        """
-        Creates an image.
-
-        Any combination of the `data`, `path` and `size` is possible,
-        but at least one of these arguments must be provided.
-        The `ext` parameter cannot be used as a single argument for
-        construction.
-
-        Args:
-            data: Image pixels or a function to retrieve them. The expected
-                image shape is (H, W [, C]). If a function is provided,
-                it must accept image path as the first argument.
-            path: Image path
-            ext: Image extension. Cannot be used together with `path`. It can
-                be used for saving with a custom extension - in that case,
-                the image need to have the `data` and `ext` fields defined.
-            size: A pair (H, W), which represents image size.
-        """
-
-        if size is not None:
-            assert (
-                len(size) == 2 and 0 < size[0] and 0 < size[1]
-            ), f"Invalid image size info '{size}'"
-            size = tuple(map(int, size))
-        self._size = size  # (H, W)
-
-        if path is None:
-            path = ""
-        elif path:
-            path = path.replace("\\", "/")
-        self._path = path
-
-        if ext:
-            assert not path, "Can't specify both 'path' and 'ext' for image"
-
-            if not ext.startswith("."):
-                ext = "." + ext
-            ext = ext.lower()
-        else:
-            ext = None
-        self._ext = ext
-
-        self._crypter = crypter
-
-        if not isinstance(data, np.ndarray):
-            assert path or callable(data) or size, "Image can not be empty"
-            assert data is None or callable(data), f"Image data has unexpected type '{type(data)}'"
-            if data or path and osp.isfile(path):
-                data = lazy_image(path, loader=data, crypter=self._crypter)
-        self._data = data
-
-    @property
-    def data(self) -> np.ndarray:
-        """Image data in BGR HWC [0; 255] (float) format"""
-
-        if callable(self._data):
-            data = self._data()
-        else:
-            data = self._data
-
-        if self._size is None and data is not None:
-            if not 2 <= data.ndim <= 3:
-                raise MediaShapeError("An image should have 2 (gray) or 3 (rgb) dims.")
-            self._size = tuple(map(int, data.shape[:2]))
-        return data
-
-    @property
-    def has_data(self) -> bool:
-        return self._data is not None
-
-    @property
-    def has_size(self) -> bool:
-        """Indicates that size info is cached and won't require image loading"""
-        return self._size is not None or isinstance(self._data, np.ndarray)
-
-    @property
-    def size(self) -> Optional[Tuple[int, int]]:
-        """Returns (H, W)"""
-
-        if self._size is None:
-            try:
-                data = self.data
-            except _image_loading_errors:
-                return None
-            if data is not None:
-                self._size = tuple(map(int, data.shape[:2]))
-        return self._size
-
-    @property
-    def ext(self) -> str:
-        """Media file extension"""
-        if self._ext is not None:
-            return self._ext
-        else:
-            return osp.splitext(osp.basename(self.path))[1]
-
-    def __eq__(self, other):
-        if not isinstance(other, __class__):
-            return False
-        return (
-            (np.array_equal(self.size, other.size))
-            and (self.has_data == other.has_data)
-            and (self.has_data and np.array_equal(self.data, other.data) or not self.has_data)
+from datumaro.components.annotation import (
+    AnnotationType,
+    LabelCategories,
+    MaskCategories,
+    PointsCategories,
+)
+from datumaro.components.annotations.merger import (
+    AnnotationMerger,
+    BboxMerger,
+    CaptionsMerger,
+    Cuboid3dMerger,
+    EllipseMerger,
+    HashKeyMerger,
+    ImageAnnotationMerger,
+    LabelMerger,
+    LineMerger,
+    MaskMerger,
+    PointsMerger,
+    PolygonMerger,
+)
+from datumaro.components.dataset import Dataset
+from datumaro.components.errors import (
+    AnnotationsTooCloseError,
+    ConflictingCategoriesError,
+    FailedAttrVotingError,
+    NoMatchingAnnError,
+    NoMatchingItemError,
+    WrongGroupError,
+)
+from datumaro.components.merge import Merger
+from datumaro.util import find
+from datumaro.util.annotation_util import find_instances, max_bbox
+from datumaro.util.attrs_util import ensure_cls
+
+__all__ = ["IntersectMerge"]
+
+
+@attrs
+class IntersectMerge(Merger):
+    def __init__(self, **options):
+        super().__init__(**options)
+
+    @attrs(repr_ns="IntersectMerge", kw_only=True)
+    class Conf:
+        pairwise_dist = attrib(converter=float, default=0.5)
+        sigma = attrib(converter=list, factory=list)
+
+        output_conf_thresh = attrib(converter=float, default=0)
+        quorum = attrib(converter=int, default=0)
+        ignored_attributes = attrib(converter=set, factory=set)
+
+        def _groups_converter(value):
+            result = []
+            for group in value:
+                rg = set()
+                for label in group:
+                    optional = label.endswith("?")
+                    name = label if not optional else label[:-1]
+                    rg.add((name, optional))
+                result.append(rg)
+            return result
+
+        groups = attrib(converter=_groups_converter, factory=list)
+        close_distance = attrib(converter=float, default=0.75)
+
+    conf = attrib(converter=ensure_cls(Conf), factory=Conf)
+
+    # Error trackers:
+    errors = attrib(factory=list, init=False)
+
+    def add_item_error(self, error, *args, **kwargs):
+        self.errors.append(error(self._item_id, *args, **kwargs))
+
+    # Indexes:
+    _dataset_map = attrib(init=False)  # id(dataset) -> (dataset, index)
+    _item_map = attrib(init=False)  # id(item) -> (item, id(dataset))
+    _ann_map = attrib(init=False)  # id(ann) -> (ann, id(item))
+    _item_id = attrib(init=False)
+    _item = attrib(init=False)
+
+    # Misc.
+    _infos = attrib(init=False)  # merged infos
+    _categories = attrib(init=False)  # merged categories
+
+    def merge(self, datasets):
+        self._infos = self.merge_infos([d.infos() for d in datasets])
+        self._categories = self.merge_categories([d.categories() for d in datasets])
+        merged = Dataset(
+            infos=self._infos,
+            categories=self._categories,
+            media_type=self.merge_media_types(datasets),
         )
 
-    def save(self, path, crypter: Crypter = NULL_CRYPTER):
-        cur_path = osp.abspath(self.path)
-        path = osp.abspath(path)
-
-        cur_ext = self.ext.lower()
-        new_ext = osp.splitext(osp.basename(path))[1].lower()
-
-        os.makedirs(osp.dirname(path), exist_ok=True)
-        if cur_ext == new_ext and osp.isfile(cur_path):
-            copyto_image(
-                src_path=cur_path, dst_path=path, src_crypter=self._crypter, dst_crypter=crypter
-            )
-        else:
-            save_image(path, self.data, crypter=crypter)
-
-    def set_crypter(self, crypter: Crypter):
-        super().set_crypter(crypter)
-        if isinstance(self._data, lazy_image):
-            self._data._crypter = crypter
-
-
-class ByteImage(Image):
-    _type = MediaType.BYTE_IMAGE
-
-    _FORMAT_MAGICS = (
-        (b"\x89PNG\r\n\x1a\n", ".png"),
-        (b"\xff\xd8\xff", ".jpg"),
-        (b"BM", ".bmp"),
-    )
-
-    def __init__(
-        self,
-        data: Union[bytes, Callable[[str], bytes], None] = None,
-        *,
-        path: Optional[str] = None,
-        ext: Optional[str] = None,
-        size: Optional[Tuple[int, int]] = None,
-        crypter: Crypter = NULL_CRYPTER,
-    ):
-        if not isinstance(data, bytes):
-            assert path or callable(data), "Image can not be empty"
-            assert data is None or callable(data)
-            if path and osp.isfile(path) or data:
-                data = lazy_image(path, loader=data)
-
-        self._bytes_data = data
+        self._check_groups_definition()
 
-        if ext is None and path is None and isinstance(data, bytes):
-            ext = self._guess_ext(data)
-
-        super().__init__(
-            path=path, ext=ext, size=size, data=lambda _: decode_image(self.get_bytes())
-        )
-        if data is None:
-            # We don't expect decoder to produce images from nothing,
-            # otherwise using this class makes no sense. We undefine
-            # data to avoid using default image loader for loading binaries
-            # from the path, when no data is provided.
-            self._data = None
-
-        self._crypter = crypter
-
-    @classmethod
-    def _guess_ext(cls, data: bytes) -> Optional[str]:
-        return next(
-            (ext for magic, ext in cls._FORMAT_MAGICS if data.startswith(magic)),
-            None,
+        item_matches, item_map = self.match_items(datasets)
+        self._item_map = item_map
+        self._dataset_map = {id(d): (d, i) for i, d in enumerate(datasets)}
+
+        for item_id, items in item_matches.items():
+            self._item_id = item_id
+
+            if len(items) < len(datasets):
+                missing_sources = set(id(s) for s in datasets) - set(items)
+                missing_sources = [self._dataset_map[s][1] for s in missing_sources]
+                self.add_item_error(NoMatchingItemError, sources=missing_sources)
+            merged.put(self.merge_items(items))
+
+        return merged
+
+    def get_ann_source(self, ann_id):
+        return self._item_map[self._ann_map[ann_id][1]][1]
+
+    def merge_categories(self, sources):
+        dst_categories = {}
+
+        label_cat = self._merge_label_categories(sources)
+        if label_cat is None:
+            label_cat = LabelCategories()
+        dst_categories[AnnotationType.label] = label_cat
+
+        points_cat = self._merge_point_categories(sources, label_cat)
+        if points_cat is not None:
+            dst_categories[AnnotationType.points] = points_cat
+
+        mask_cat = self._merge_mask_categories(sources, label_cat)
+        if mask_cat is not None:
+            dst_categories[AnnotationType.mask] = mask_cat
+
+        return dst_categories
+
+    def merge_items(self, items):
+        self._item = next(iter(items.values()))
+
+        self._ann_map = {}
+        sources = []
+        for item in items.values():
+            self._ann_map.update({id(a): (a, id(item)) for a in item.annotations})
+            sources.append(item.annotations)
+        log.debug(
+            "Merging item %s: source annotations %s" % (self._item_id, list(map(len, sources)))
         )
 
-    def get_bytes(self):
-        if callable(self._bytes_data):
-            return self._bytes_data()
-        return self._bytes_data
-
-    def save(self, path, crypter: Crypter = NULL_CRYPTER):
-        if not crypter.is_null_crypter:
-            raise NotImplementedError(
-                f"{self.__class__.__name__} does not implement save() with non NullCrypter."
-            )
-
-        cur_path = osp.abspath(self.path)
-        path = osp.abspath(path)
-
-        cur_ext = self.ext.lower()
-        new_ext = osp.splitext(osp.basename(path))[1].lower()
-
-        os.makedirs(osp.dirname(path), exist_ok=True)
-        if cur_ext == new_ext and osp.isfile(cur_path):
-            if cur_path != path:
-                shutil.copyfile(cur_path, path)
-        elif cur_ext == new_ext:
-            with open(path, "wb") as f:
-                f.write(self.get_bytes())
-        else:
-            save_image(path, self.data)
-
-
-class VideoFrame(Image):
-    _type = MediaType.VIDEO_FRAME
-
-    def __init__(self, video: Video, index: int):
-        self._video = video
-        self._index = index
-
-        super().__init__(lambda _: self._video.get_frame_data(self._index))
-
-    @property
-    def size(self) -> Tuple[int, int]:
-        return self._video.frame_size
-
-    @property
-    def index(self) -> int:
-        return self._index
-
-    @property
-    def video(self) -> Video:
-        return self._video
-
-
-class _VideoFrameIterator(Iterator[VideoFrame]):
-    """
-    Provides sequential access to the video frames.
-    """
-
-    _video: Video
-    _iterator: Iterator[VideoFrame]
-    _pos: int
-    _current_frame_data: Optional[np.ndarray]
-
-    def __init__(self, video: Video):
-        self._video = video
-        self._reset()
-
-    def _reset(self):
-        self._video._reset_reader()
-        self._iterator = self._decode(self._video._get_reader())
-        self._pos = -1
-        self._current_frame_data = None
-
-    def _decode(self, cap) -> Iterator[VideoFrame]:
-        """
-        Decodes video frames using opencv
-        """
-
-        self._pos = -1
-
-        success, frame = cap.read()
-        while success:
-            self._pos += 1
-            if self._video._includes_frame(self._pos):
-                self._current_frame_data = frame.astype(float)
-                yield self._make_frame(index=self._pos)
-
-            success, frame = cap.read()
-
-        if self._video._frame_count is None:
-            self._video._frame_count = self._pos + 1
-
-    def _make_frame(self, index) -> VideoFrame:
-        return VideoFrame(self._video, index=index)
-
-    def __next__(self):
-        return next(self._iterator)
-
-    def __getitem__(self, idx: int) -> VideoFrame:
-        if not self._video._includes_frame(idx):
-            raise IndexError(f"Video doesn't contain frame #{idx}.")
-
-        return self._navigate_to(idx)
-
-    def get_frame_data(self, idx: int) -> np.ndarray:
-        self._navigate_to(idx)
-        return self._current_frame_data
-
-    def _navigate_to(self, idx: int) -> VideoFrame:
-        """
-        Iterates over frames to the required position.
-        """
-
-        if idx < 0:
-            raise IndexError()
-
-        if idx < self._pos:
-            self._reset()
-
-        if self._pos < idx:
-            try:
-                while self._pos < idx:
-                    v = self.__next__()
-            except StopIteration as e:
-                raise IndexError() from e
-        else:
-            v = self._make_frame(index=self._pos)
-
-        return v
-
-
-class Video(MediaElement, Iterable[VideoFrame]):
-    _type = MediaType.VIDEO
-
-    """
-    Provides random access to the video frames.
-    """
-
-    def __init__(
-        self, path: str, *, step: int = 1, start_frame: int = 0, end_frame: Optional[int] = None
-    ) -> None:
-        super().__init__(path)
-
-        if end_frame:
-            assert start_frame < end_frame
-        assert 0 < step
-        self._step = step
-        self._start_frame = start_frame
-        self._end_frame = end_frame or None
-
-        self._reader = None
-        self._iterator: Optional[_VideoFrameIterator] = None
-        self._frame_size: Optional[Tuple[int, int]] = None
-
-        # We don't provide frame count unless we have a reliable source of
-        # this information.
-        # - Not all videos provide length / duration metainfo
-        # - We can get an estimation based on metadata, but it
-        #   can be invalid or inaccurate due to variable frame rate
-        #   or fractional values rounded up. Relying on the value will give
-        #   errors during requesting frames.
-        # https://stackoverflow.com/a/47796468
-        self._frame_count = None
-        self._length = None
-
-        from .media_manager import MediaManager
-
-        MediaManager.get_instance().push(weakref.ref(self), self)
-
-    def close(self):
-        self._iterator = None
-
-        if self._reader is not None:
-            self._reader.release()
-            self._reader = None
-
-    def __getitem__(self, idx: int) -> VideoFrame:
-        if not self._includes_frame(idx):
-            raise IndexError(f"Video doesn't contain frame #{idx}.")
-
-        return self._get_iterator()[idx]
-
-    def get_frame_data(self, idx: int) -> VideoFrame:
-        if not self._includes_frame(idx):
-            raise IndexError(f"Video doesn't contain frame #{idx}.")
-
-        return self._get_iterator().get_frame_data(idx)
-
-    def __iter__(self) -> Iterator[VideoFrame]:
-        """
-        Iterates over frames lazily, if possible.
-        """
-
-        if self._frame_count is not None:
-            # Decoding is not necessary to get frame pointers
-            # However, it can be inacurrate
-            end_frame = self._get_end_frame()
-            for index in range(self._start_frame, end_frame, self._step):
-                yield VideoFrame(video=self, index=index)
-        else:
-            # Need to decode to iterate over frames
-            yield from self._get_iterator()
-
-    @property
-    def length(self) -> Optional[int]:
-        """
-        Returns frame count, if video provides such information.
-
-        Note that not all videos provide length / duration metainfo, so the
-        result may be undefined.
-
-        Also note, that information may be inaccurate because of variable
-        FPS in video or incorrect metainfo. The count is only guaranteed to
-        be valid after video is completely read once.
-
-        The count is affected by the frame filtering options of the object,
-        i.e. start frame, end frame and frame step.
-        """
-
-        if self._length is None:
-            end_frame = self._get_end_frame()
-
-            length = None
-            if end_frame is not None:
-                length = (end_frame - self._start_frame) // self._step
-                assert 0 < length
-
-            self._length = length
-
-        return self._length
-
-    @property
-    def frame_size(self) -> Tuple[int, int]:
-        """Returns (H, W)"""
-
-        if self._frame_size is None:
-            self._frame_size = self._get_frame_size()
-        return self._frame_size
-
-    def _get_frame_size(self) -> Tuple[int, int]:
-        cap = self._get_reader()
-        w = cap.get(cv2.CAP_PROP_FRAME_WIDTH)
-        h = cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
-
-        if h and w:
-            frame_size = (int(h), int(w))
-        else:
-            image = next(self._get_iterator()).data
-            frame_size = image.shape[0:2]
-
-        return frame_size
-
-    def _get_end_frame(self):
-        if self._end_frame is not None and self._frame_count is not None:
-            end_frame = min(self._end_frame, self._frame_count)
-        else:
-            end_frame = self._end_frame or self._frame_count
-
-        return end_frame
-
-    def _includes_frame(self, i):
-        end_frame = self._get_end_frame()
-        if self._start_frame <= i:
-            if (i - self._start_frame) % self._step == 0:
-                if end_frame is None or i < end_frame:
-                    return True
-
-        return False
-
-    def _get_iterator(self):
-        if self._iterator is None:
-            self._iterator = _VideoFrameIterator(self)
-        return self._iterator
-
-    def _get_reader(self):
-        if self._reader is None:
-            self._reset_reader()
-        return self._reader
-
-    def _reset_reader(self):
-        if self._reader is not None:
-            self._reader.release()
-        self._reader = cv2.VideoCapture(self._path)
-        assert self._reader.isOpened()
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, __class__):
-            return False
+        annotations = self.merge_annotations(sources)
 
+        annotations = [
+            a for a in annotations if self.conf.output_conf_thresh <= a.attributes.get("score", 1)
+        ]
+
+        return self._item.wrap(annotations=annotations)
+
+    def merge_annotations(self, sources):
+        self._make_mergers(sources)
+
+        clusters = self._match_annotations(sources)
+
+        joined_clusters = sum(clusters.values(), [])
+        group_map = self._find_cluster_groups(joined_clusters)
+
+        annotations = []
+        for t, clusters in clusters.items():
+            for cluster in clusters:
+                self._check_cluster_sources(cluster)
+
+            merged_clusters = self._merge_clusters(t, clusters)
+
+            for merged_ann, cluster in zip(merged_clusters, clusters):
+                attributes = self._find_cluster_attrs(cluster, merged_ann)
+                attributes = {
+                    k: v for k, v in attributes.items() if k not in self.conf.ignored_attributes
+                }
+                attributes.update(merged_ann.attributes)
+                merged_ann.attributes = attributes
+
+                new_group_id = find(enumerate(group_map), lambda e: id(cluster) in e[1][0])
+                if new_group_id is None:
+                    new_group_id = 0
+                else:
+                    new_group_id = new_group_id[0] + 1
+                merged_ann.group = new_group_id
+
+            if self.conf.close_distance:
+                self._check_annotation_distance(t, merged_clusters)
+
+            annotations += merged_clusters
+
+        if self.conf.groups:
+            self._check_groups(annotations)
+
+        return annotations
+
+    def match_items(self, datasets):
+        item_ids = set((item.id, item.subset) for d in datasets for item in d)
+
+        item_map = {}  # id(item) -> (item, id(dataset))
+
+        matches = OrderedDict()
+        for item_id, item_subset in sorted(item_ids, key=lambda e: e[0]):
+            items = {}
+            for d in datasets:
+                item = d.get(item_id, subset=item_subset)
+                if item:
+                    items[id(d)] = item
+                    item_map[id(item)] = (item, id(d))
+            matches[(item_id, item_subset)] = items
+
+        return matches, item_map
+
+    def _merge_label_categories(self, sources):
+        same = True
+        common = None
+        for src_categories in sources:
+            src_cat = src_categories.get(AnnotationType.label)
+            if common is None:
+                common = src_cat
+            elif common != src_cat:
+                same = False
+                break
+
+        if same:
+            return common
+
+        dst_cat = LabelCategories()
+        for src_id, src_categories in enumerate(sources):
+            src_cat = src_categories.get(AnnotationType.label)
+            if src_cat is None:
+                continue
+
+            for src_label in src_cat.items:
+                dst_label = dst_cat.find(src_label.name)[1]
+                if dst_label is not None:
+                    if dst_label != src_label:
+                        if (
+                            src_label.parent
+                            and dst_label.parent
+                            and src_label.parent != dst_label.parent
+                        ):
+                            raise ConflictingCategoriesError(
+                                "Can't merge label category %s (from #%s): "
+                                "parent label conflict: %s vs. %s"
+                                % (src_label.name, src_id, src_label.parent, dst_label.parent),
+                                sources=list(range(src_id)),
+                            )
+                        dst_label.parent = dst_label.parent or src_label.parent
+                        dst_label.attributes |= src_label.attributes
+                    else:
+                        pass
+                else:
+                    dst_cat.add(src_label.name, src_label.parent, src_label.attributes)
+
+        return dst_cat
+
+    def _merge_point_categories(self, sources, label_cat):
+        dst_point_cat = PointsCategories()
+
+        for src_id, src_categories in enumerate(sources):
+            src_label_cat = src_categories.get(AnnotationType.label)
+            src_point_cat = src_categories.get(AnnotationType.points)
+            if src_label_cat is None or src_point_cat is None:
+                continue
+
+            for src_label_id, src_cat in src_point_cat.items.items():
+                src_label = src_label_cat.items[src_label_id].name
+                dst_label_id = label_cat.find(src_label)[0]
+                dst_cat = dst_point_cat.items.get(dst_label_id)
+                if dst_cat is not None:
+                    if dst_cat != src_cat:
+                        raise ConflictingCategoriesError(
+                            "Can't merge point category for label "
+                            "%s (from #%s): %s vs. %s" % (src_label, src_id, src_cat, dst_cat),
+                            sources=list(range(src_id)),
+                        )
+                    else:
+                        pass
+                else:
+                    dst_point_cat.add(dst_label_id, src_cat.labels, src_cat.joints)
+
+        if len(dst_point_cat.items) == 0:
+            return None
+
+        return dst_point_cat
+
+    def _merge_mask_categories(self, sources, label_cat):
+        dst_mask_cat = MaskCategories()
+
+        for src_id, src_categories in enumerate(sources):
+            src_label_cat = src_categories.get(AnnotationType.label)
+            src_mask_cat = src_categories.get(AnnotationType.mask)
+            if src_label_cat is None or src_mask_cat is None:
+                continue
+
+            for src_label_id, src_cat in src_mask_cat.colormap.items():
+                src_label = src_label_cat.items[src_label_id].name
+                dst_label_id = label_cat.find(src_label)[0]
+                dst_cat = dst_mask_cat.colormap.get(dst_label_id)
+                if dst_cat is not None:
+                    if dst_cat != src_cat:
+                        raise ConflictingCategoriesError(
+                            "Can't merge mask category for label "
+                            "%s (from #%s): %s vs. %s" % (src_label, src_id, src_cat, dst_cat),
+                            sources=list(range(src_id)),
+                        )
+                    else:
+                        pass
+                else:
+                    dst_mask_cat.colormap[dst_label_id] = src_cat
+
+        if len(dst_mask_cat.colormap) == 0:
+            return None
+
+        return dst_mask_cat
+
+    def _match_annotations(self, sources):
+        all_by_type = {}
+        for s in sources:
+            src_by_type = {}
+            for a in s:
+                src_by_type.setdefault(a.type, []).append(a)
+            for k, v in src_by_type.items():
+                all_by_type.setdefault(k, []).append(v)
+
+        clusters = {}
+        for k, v in all_by_type.items():
+            clusters.setdefault(k, []).extend(self._match_ann_type(k, v))
+
+        return clusters
+
+    def _make_mergers(self, sources):
+        def _make(c, **kwargs):
+            kwargs.update(attr.asdict(self.conf))
+            fields = attr.fields_dict(c)
+            return c(**{k: v for k, v in kwargs.items() if k in fields}, context=self)
+
+        def _for_type(t, **kwargs):
+            if t is AnnotationType.unknown:
+                return _make(AnnotationMerger, **kwargs)
+            elif t is AnnotationType.label:
+                return _make(LabelMerger, **kwargs)
+            elif t is AnnotationType.bbox:
+                return _make(BboxMerger, **kwargs)
+            elif t is AnnotationType.mask:
+                return _make(MaskMerger, **kwargs)
+            elif t is AnnotationType.polygon:
+                return _make(PolygonMerger, **kwargs)
+            elif t is AnnotationType.polyline:
+                return _make(LineMerger, **kwargs)
+            elif t is AnnotationType.points:
+                return _make(PointsMerger, **kwargs)
+            elif t is AnnotationType.caption:
+                return _make(CaptionsMerger, **kwargs)
+            elif t is AnnotationType.cuboid_3d:
+                return _make(Cuboid3dMerger, **kwargs)
+            elif t is AnnotationType.super_resolution_annotation:
+                return _make(ImageAnnotationMerger, **kwargs)
+            elif t is AnnotationType.depth_annotation:
+                return _make(ImageAnnotationMerger, **kwargs)
+            elif t is AnnotationType.ellipse:
+                return _make(EllipseMerger, **kwargs)
+            elif t is AnnotationType.hash_key:
+                return _make(HashKeyMerger, **kwargs)
+            else:
+                raise NotImplementedError("Type %s is not supported" % t)
+
+        instance_map = {}
+        for s in sources:
+            s_instances = find_instances(s)
+            for inst in s_instances:
+                inst_bbox = max_bbox(
+                    [
+                        a
+                        for a in inst
+                        if a.type
+                        in {AnnotationType.polygon, AnnotationType.mask, AnnotationType.bbox}
+                    ]
+                )
+                for ann in inst:
+                    instance_map[id(ann)] = [inst, inst_bbox]
+
+        self._mergers = {t: _for_type(t, instance_map=instance_map) for t in AnnotationType}
+
+    def _match_ann_type(self, t, sources):
+        return self._mergers[t].match_annotations(sources)
+
+    def _merge_clusters(self, t, clusters):
+        return self._mergers[t].merge_clusters(clusters)
+
+    def _find_cluster_groups(self, clusters):
+        cluster_groups = []
+        visited = set()
+        for a_idx, cluster_a in enumerate(clusters):
+            if a_idx in visited:
+                continue
+            visited.add(a_idx)
+
+            cluster_group = {id(cluster_a)}
+
+            # find segment groups in the cluster group
+            a_groups = set(ann.group for ann in cluster_a)
+            for cluster_b in clusters[a_idx + 1 :]:
+                b_groups = set(ann.group for ann in cluster_b)
+                if a_groups & b_groups:
+                    a_groups |= b_groups
+
+            # now we know all the segment groups in this cluster group
+            # so we can find adjacent clusters
+            for b_idx, cluster_b in enumerate(clusters[a_idx + 1 :]):
+                b_idx = a_idx + 1 + b_idx
+                b_groups = set(ann.group for ann in cluster_b)
+                if a_groups & b_groups:
+                    cluster_group.add(id(cluster_b))
+                    visited.add(b_idx)
+
+            if a_groups == {0}:
+                continue  # skip annotations without a group
+            cluster_groups.append((cluster_group, a_groups))
+        return cluster_groups
+
+    def _find_cluster_attrs(self, cluster, ann):
+        quorum = self.conf.quorum or 0
+
+        # TODO: when attribute types are implemented, add linear
+        # interpolation for contiguous values
+
+        attr_votes = {}  # name -> { value: score , ... }
+        for s in cluster:
+            for name, value in s.attributes.items():
+                votes = attr_votes.get(name, {})
+                votes[value] = 1 + votes.get(value, 0)
+                attr_votes[name] = votes
+
+        attributes = {}
+        for name, votes in attr_votes.items():
+            winner, count = max(votes.items(), key=lambda e: e[1])
+            if count < quorum:
+                if sum(votes.values()) < quorum:
+                    # blame provokers
+                    missing_sources = set(
+                        self.get_ann_source(id(a))
+                        for a in cluster
+                        if s.attributes.get(name) == winner
+                    )
+                else:
+                    # blame outliers
+                    missing_sources = set(
+                        self.get_ann_source(id(a))
+                        for a in cluster
+                        if s.attributes.get(name) != winner
+                    )
+                missing_sources = [self._dataset_map[s][1] for s in missing_sources]
+                self.add_item_error(
+                    FailedAttrVotingError, name, votes, ann, sources=missing_sources
+                )
+                continue
+            attributes[name] = winner
+
+        return attributes
+
+    def _check_cluster_sources(self, cluster):
+        if len(cluster) == len(self._dataset_map):
+            return
+
+        def _has_item(s):
+            item = self._dataset_map[s][0].get(*self._item_id)
+            if not item:
+                return False
+            if len(item.annotations) == 0:
+                return False
+            return True
+
+        missing_sources = set(self._dataset_map) - set(self.get_ann_source(id(a)) for a in cluster)
+        missing_sources = [self._dataset_map[s][1] for s in missing_sources if _has_item(s)]
+        if missing_sources:
+            self.add_item_error(NoMatchingAnnError, cluster[0], sources=missing_sources)
+
+    def _check_annotation_distance(self, t, annotations):
+        for a_idx, a_ann in enumerate(annotations):
+            for b_ann in annotations[a_idx + 1 :]:
+                d = self._mergers[t].distance(a_ann, b_ann)
+                if self.conf.close_distance < d:
+                    self.add_item_error(AnnotationsTooCloseError, a_ann, b_ann, d)
+
+    def _check_groups(self, annotations):
+        check_groups = []
+        for check_group_raw in self.conf.groups:
+            check_group = set(l[0] for l in check_group_raw)
+            optional = set(l[0] for l in check_group_raw if l[1])
+            check_groups.append((check_group, optional))
+
+        def _check_group(group_labels, group):
+            for check_group, optional in check_groups:
+                common = check_group & group_labels
+                real_miss = check_group - common - optional
+                extra = group_labels - check_group
+                if common and (extra or real_miss):
+                    self.add_item_error(WrongGroupError, group_labels, check_group, group)
+                    break
+
+        groups = find_instances(annotations)
+        for group in groups:
+            group_labels = set()
+            for ann in group:
+                if not hasattr(ann, "label"):
+                    continue
+                label = self._get_label_name(ann.label)
+
+                if ann.group:
+                    group_labels.add(label)
+                else:
+                    _check_group({label}, [ann])
+
+            if not group_labels:
+                continue
+            _check_group(group_labels, group)
+
+    def _get_label_name(self, label_id):
+        if label_id is None:
+            return None
+        return self._categories[AnnotationType.label].items[label_id].name
+
+    def _get_label_id(self, label):
+        return self._categories[AnnotationType.label].find(label)[0]
+
+    def _get_src_label_name(self, ann, label_id):
+        if label_id is None:
+            return None
+        item_id = self._ann_map[id(ann)][1]
+        dataset_id = self._item_map[item_id][1]
         return (
-            self.path == other.path
-            and self._start_frame == other._start_frame
-            and self._step == other._step
-            and self._end_frame == other._end_frame
+            self._dataset_map[dataset_id][0].categories()[AnnotationType.label].items[label_id].name
         )
 
-    def __hash__(self):
-        # Required for caching
-        return hash((self._path, self._step, self._start_frame, self._end_frame))
-
-
-class PointCloud(MediaElement):
-    _type = MediaType.POINT_CLOUD
-
-    def __init__(
-        self,
-        path: str,
-        extra_images: Optional[List[Image]] = None,
-        crypter: Crypter = NULL_CRYPTER,
-    ):
-        self._path = path
-
-        self.extra_images: List[Image] = extra_images or []
-
-        self._crypter = crypter
-
-
-class MultiframeImage(MediaElement):
-    _type = MediaType.MULTIFRAME_IMAGE
-
-    def __init__(
-        self,
-        images: Optional[Iterable[Union[str, Image, np.ndarray, Callable[[str], np.ndarray]]]],
-        *,
-        path: Optional[str] = None,
-    ):
-        self._path = path
-
-        if images is None:
-            images = []
-
-        self._images = [None] * len(images)
-        for i, image in enumerate(images):
-            assert isinstance(image, (str, Image, np.ndarray)) or callable(image)
-
-            if isinstance(image, str):
-                image = Image(path=image)
-            elif isinstance(image, np.ndarray) or callable(image):
-                image = Image(data=image)
-
-            self._images[i] = image
-
-        assert self._path or self._images
-
-    @property
-    def data(self) -> List[Image]:
-        return self._images
-
-
-class RoIImage(Image):
-    _type = MediaType.ROI_IMAGE
-
-    def __init__(
-        self,
-        data: Union[np.ndarray, Callable[[str], np.ndarray], None] = None,
-        *,
-        path: Optional[str] = None,
-        ext: Optional[str] = None,
-        roi: BboxIntCoords,
-    ) -> None:
-        assert len(roi) == 4 and all(isinstance(v, int) for v in roi)
-        self._roi = roi
-        _, _, w, h = self._roi
-        super().__init__(data=data, path=path, ext=ext, size=(h, w))
-
-    @classmethod
-    def create_from_image(cls, img: Image, roi: BboxIntCoords) -> RoIImage:
-        if not isinstance(img, Image):
-            raise TypeError(f"type(img)={type(img)} should be Image.")
-
-        data = lambda _: img._data() if isinstance(img._data, lazy_image) else img._data
-        return cls(data=data, path=img._path, ext=img._ext, roi=roi)
-
-    @property
-    def roi(self) -> BboxIntCoords:
-        return self._roi
-
-    @property
-    def data(self) -> np.ndarray:
-        """Image data in BGR HWC [0; 255] (float) format"""
-        x, y, w, h = self._roi
-        img = super().data
-        return img[y : y + h, x : x + w]
-
-    def save(self, path, crypter: Crypter = NULL_CRYPTER):
-        if not crypter.is_null_crypter:
-            raise NotImplementedError(
-                f"{self.__class__.__name__} does not implement save() with non NullCrypter."
-            )
-        path = osp.abspath(path)
-        os.makedirs(osp.dirname(path), exist_ok=True)
-        save_image(path, self.data)
-
-
-ImageWithRoI = Tuple[Image, BboxIntCoords]
-
-
-class MosaicImage(Image):
-    _type = MediaType.MOSAIC_IMAGE
-
-    def __init__(self, imgs: List[ImageWithRoI], size: Tuple[int, int]) -> None:
-        def _get_mosaic_img(_) -> np.ndarray:
-            h, w = self.size
-            mosaic_img = np.zeros(shape=(h, w, 3), dtype=np.uint8)
-            for img, roi in imgs:
-                assert isinstance(img, Image), "MosaicImage can only take a list of Images."
-                x, y, w, h = roi
-                mosaic_img[y : y + h, x : x + w] = img.data
-            return mosaic_img
-
-        super().__init__(data=_get_mosaic_img, path=None, ext=None, size=size)
-
-    def save(self, path, crypter: Crypter = NULL_CRYPTER):
-        if not crypter.is_null_crypter:
-            raise NotImplementedError(
-                f"{self.__class__.__name__} does not implement save() with non NullCrypter."
-            )
-        path = osp.abspath(path)
-        os.makedirs(osp.dirname(path), exist_ok=True)
-        save_image(path, self.data)
+    def _get_any_label_name(self, ann, label_id):
+        if label_id is None:
+            return None
+        try:
+            return self._get_src_label_name(ann, label_id)
+        except KeyError:
+            return self._get_label_name(label_id)
+
+    def _check_groups_definition(self):
+        for group in self.conf.groups:
+            for label, _ in group:
+                _, entry = self._categories[AnnotationType.label].find(label)
+                if entry is None:
+                    raise ValueError(
+                        "Datasets do not contain "
+                        "label '%s', available labels %s"
+                        % (label, [i.name for i in self._categories[AnnotationType.label].items])
+                    )
```

### Comparing `datumaro-1.1.1/datumaro/components/media_manager.py` & `datumaro-1.2.0rc1/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/merger.py` & `datumaro-1.2.0rc1/datumaro/components/merge/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,24 +49,7 @@
                 ):
                     # Symmetric comparision is needed in the case of subclasses:
                     # eg. Image and ByteImage
                     raise MediaTypeError("Datasets have different media types")
             return media_type
 
         return None
-
-
-def get_merger(key):
-    if key == "union":
-        from datumaro.components.operations import UnionMerge
-
-        merger = UnionMerge()
-    elif key == "intersect":
-        from datumaro.components.operations import IntersectMerge
-
-        merger = IntersectMerge()
-    else:
-        from datumaro.components.operations import ExactMerge
-
-        merger = ExactMerge()
-
-    return merger
```

### Comparing `datumaro-1.1.1/datumaro/components/project.py` & `datumaro-1.2.0rc1/datumaro/components/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
         if idx is None:
             raise KeyError("Can't find stage '%s'" % name)
         target.stages.remove(idx)
 
     def add_transform_stage(
         self, target: str, transform: str, params: Optional[Dict] = None, name: Optional[str] = None
     ):
-        if not transform in self._tree.env.transforms:
+        if transform not in self._tree.env.transforms:
             raise KeyError("Unknown transform '%s'" % transform)
 
         return self.add_stage(
             target,
             {
                 "type": BuildStageType.transform.name,
                 "kind": transform,
@@ -868,15 +868,15 @@
             },
             name=name,
         )
 
     def add_inference_stage(
         self, target: str, model: str, params: Optional[Dict] = None, name: Optional[str] = None
     ):
-        if not model in self._tree._project.models:
+        if model not in self._tree._project.models:
             raise KeyError("Unknown model '%s'" % model)
 
         return self.add_stage(
             target,
             {
                 "type": BuildStageType.inference.name,
                 "kind": model,
@@ -964,15 +964,15 @@
                 for prev_stage in prev_stages:
                     graph.add_edge(prev_stage, stage_name)
                 prev_stages = [stage_name]
 
         return pipeline
 
     def make_pipeline(self, target: str) -> Pipeline:
-        if not target in self:
+        if target not in self:
             raise UnknownTargetError(target)
 
         # a subgraph with all the target dependencies
         if "." not in target:
             target = self.make_target_name(target, self[target].head.name)
 
         return self._make_full_pipeline().get_slice(target)
@@ -1908,15 +1908,15 @@
         """
 
         if self._is_working_tree_ref(ref):
             return self._ObjectIdKind.tree, ref
 
         try:
             obj_type, obj_hash = self._git.rev_parse(ref)
-        except Exception:  # nosec - B110:try_except_pass
+        except Exception:  # nosec try_except_pass
             pass  # Ignore git errors
         else:
             if obj_type != "commit":
                 raise UnknownRefError(obj_hash)
 
             return self._ObjectIdKind.tree, obj_hash
 
@@ -2479,15 +2479,15 @@
         MediaManager.get_instance().clear()
 
         if sources:
             rev_tree = self.get_rev(rev)
 
             # Check targets
             for s in sources:
-                if not s in rev_tree.sources:
+                if s not in rev_tree.sources:
                     raise UnknownSourceError(s)
 
             rev_dir = rev_tree.config.base_dir
             with self._make_tmp_dir() as tmp_dir:
                 dvcfiles = []
 
                 for s in sources:
@@ -2666,15 +2666,15 @@
             model_dir = None
         return self._env.make_launcher(model.launcher, **model.options, model_dir=model_dir)
 
     def add_model(self, name: str, launcher: str, options: Dict[str, Any] = None) -> Model:
         if self.readonly:
             raise ReadonlyProjectError()
 
-        if not launcher in self.env.launchers:
+        if launcher not in self.env.launchers:
             raise KeyError("Unknown launcher '%s'" % launcher)
 
         if not name:
             raise ValueError("Model name can't be empty")
 
         if name in self.models:
             raise KeyError("Model '%s' already exists" % name)
```

### Comparing `datumaro-1.1.1/datumaro/components/searcher.py` & `datumaro-1.2.0rc1/datumaro/components/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/shift_analyzer.py` & `datumaro-1.2.0rc1/datumaro/components/shift_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+# ruff: noqa: E501
+
 from collections import defaultdict
 from typing import Dict, List, Optional
 
 import numpy as np
 import pyemd
 from scipy import linalg
 from scipy.stats import anderson_ksamp
```

### Comparing `datumaro-1.1.1/datumaro/components/transformer.py` & `datumaro-1.2.0rc1/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/validator.py` & `datumaro-1.2.0rc1/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/components/visualizer.py` & `datumaro-1.2.0rc1/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
                 mask_path = osp.splitext(image_path)[0] + "_parts_%s.png" % (part_level + 1)
 
             self._items.append(
                 DatasetItem(
                     item_id,
                     subset=subset,
-                    media=Image(path=image_path),
+                    media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
             )
 
     def _load_item_info(self, path):
         attr_path = osp.splitext(path)[0] + "_atr.txt"
         if not osp.isfile(attr_path):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                         )
                     )
 
             self._items.append(
                 DatasetItem(
                     item_id,
                     subset=subset,
-                    media=Image(path=image_path),
+                    media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
             )
 
     def _load_item_info(self, path):
         json_path = osp.splitext(path)[0] + ".json"
         item_info = []
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 )
 
                 item = items.get(item_id)
                 if item is None:
                     item = DatasetItem(
                         id=item_id,
                         subset=self._subset,
-                        media=Image(path=image_path),
+                        media=Image.from_file(path=image_path),
                     )
                     items[item_id] = item
 
                 if "excluded_timestamps" in self._subset:
                     continue
 
                 bbox = list(map(float, data[2:6]))  # (x1, y1, x2, y2)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/brats.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/camvid.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                         if labels[label_id] in self._labels:
                             image = self._lazy_extract_mask(mask, label_id)
                             item_annotations.append(Mask(image=image, label=label_id))
 
                 items[item_id] = DatasetItem(
                     id=item_id,
                     subset=self._subset,
-                    media=Image(path=image_path),
+                    media=Image.from_file(path=image_path),
                     annotations=item_annotations,
                 )
 
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 for label in label_ids:
                     while len(label_categories) <= label:
                         label_categories.add("class-%d" % len(label_categories))
                     anno.append(Label(label))
 
                 image = images.get(item_id)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
         landmark_path = osp.join(root_dir, AlignCelebaPath.LANDMARKS_FILE)
         if osp.isfile(landmark_path):
             with open(landmark_path, encoding="utf-8") as f:
                 landmarks_number = int(f.readline().strip())
@@ -137,15 +137,15 @@
                         )
 
                     attrs = {name: 0 < int(ann) for name, ann in zip(attr_names, item_ann)}
 
                     if item_id not in items:
                         image = images.get(item_id)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[item_id] = DatasetItem(id=item_id, media=image)
 
                     items[item_id].attributes = attrs
 
                 if attr_number - 1 != counter:
                     raise DatasetImportError(
@@ -161,15 +161,15 @@
                     item_id, item_ann = self.split_annotation(line)
                     subset_id = item_ann[0]
                     subset = AlignCelebaPath.SUBSETS[subset_id]
 
                     if item_id not in items:
                         image = images.get(item_id)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
                         items[item_id] = DatasetItem(id=item_id, media=image)
 
                     items[item_id].subset = subset
 
                     if "default" in self._subsets:
                         self._subsets.pop()
                     self._subsets.append(subset)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import logging as log
 import os.path as osp
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Label,
     LabelCategories,
@@ -75,15 +74,15 @@
                 for label in label_ids:
                     while len(label_categories) <= label:
                         label_categories.add("class-%d" % len(label_categories))
                     anno.append(Label(label))
 
                 image = images.get(item_id)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
         landmark_path = osp.join(root_dir, CelebaPath.LANDMARKS_FILE)
         if osp.isfile(landmark_path):
             with open(landmark_path, encoding="utf-8") as f:
                 landmarks_number = int(f.readline().strip())
@@ -175,15 +174,15 @@
                         )
 
                     attrs = {name: 0 < int(ann) for name, ann in zip(attr_names, item_ann)}
 
                     if item_id not in items:
                         image = images.get(item_id)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[item_id] = DatasetItem(id=item_id, media=image)
 
                     items[item_id].attributes = attrs
 
                 if attr_number - 1 != counter:
                     raise DatasetImportError(
@@ -199,15 +198,15 @@
                     item_id, item_ann = self.split_annotation(line)
                     subset_id = item_ann[0]
                     subset = CelebaPath.SUBSETS[subset_id]
 
                     if item_id not in items:
                         image = images.get(item_id)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[item_id] = DatasetItem(id=item_id, media=image)
 
                     items[item_id].subset = subset
 
                     if "default" in self._subsets:
                         self._subsets.pop()
@@ -232,35 +231,36 @@
 
 
 class CelebaImporter(Importer):
     PATH_CLS = CelebaPath
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
-        super().detect(context)
+        try:
+            super().detect(context)
+        except DatasetImportError as e:
+            context.fail(str(e))
         return FormatDetectionConfidence.MEDIUM
 
     @classmethod
     def find_sources(cls, path):
         dirname = osp.dirname(cls.PATH_CLS.LABELS_FILE)
         filename, ext = osp.splitext(osp.basename(cls.PATH_CLS.LABELS_FILE))
         sources = cls._find_sources_recursive(
             path, ext=ext, extractor_name=cls.NAME, filename=filename, dirname=dirname
         )
 
         if len(sources) > 1:
-            log.error(
+            raise DatasetImportError(
                 f"{cls.NAME} label file ({cls.PATH_CLS.LABELS_FILE}) must be unique "
                 f"but the found sources have multiple duplicates. sources = {sources}"
             )
-            return []
 
         for source in sources:
             anno_dir = osp.dirname(source["url"])
             root_dir = osp.dirname(anno_dir)
             img_dir = osp.join(root_dir, cls.PATH_CLS.IMAGES_DIR)
             if not osp.exists(img_dir):
-                log.error(f"Cannot find {cls.NAME}'s images directory at {img_dir}")
-                return []
+                raise DatasetImportError(f"Cannot find {cls.NAME}'s images directory at {img_dir}")
             source["url"] = root_dir
 
         return sources
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cifar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
-import pickle  # nosec - disable B403:import_pickle check - fixed
+import pickle  # nosec import_pickle
 from collections import OrderedDict
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset import ItemStatus
@@ -147,15 +147,15 @@
                 elif image is not None:
                     image = image.astype(np.uint8).reshape(
                         3, CifarPath.IMAGE_SIZE, CifarPath.IMAGE_SIZE
                     )
                     image = np.transpose(image, (1, 2, 0))
 
             if image is not None:
-                image = Image(data=image)
+                image = Image.from_numpy(data=image)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=annotations
             )
 
         return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,22 +277,24 @@
                         id=ann_id,
                         attributes={"is_crowd": is_crowd},
                     )
                 )
 
             image = image_path_by_id.pop(item_id, None)
             if image:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=anns
             )
 
         for item_id, path in image_path_by_id.items():
-            items[item_id] = DatasetItem(id=item_id, subset=self._subset, media=Image(path=path))
+            items[item_id] = DatasetItem(
+                id=item_id, subset=self._subset, media=Image.from_file(path=path)
+            )
 
         self._categories = self._load_categories(
             self._path, use_train_label_map=mask_suffix is CityscapesPath.LABEL_TRAIN_IDS_SUFFIX
         )
         return items
 
     @staticmethod
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,17 @@
                 else:
                     image_size = None
 
                 file_name = self._parse_field(img_info, "file_name", str)
                 items[img_id] = DatasetItem(
                     id=osp.splitext(file_name)[0],
                     subset=self._subset,
-                    media=Image(path=osp.join(self._images_dir, file_name), size=image_size),
+                    media=Image.from_file(
+                        path=osp.join(self._images_dir, file_name), size=image_size
+                    ),
                     annotations=[],
                     attributes={"id": img_id},
                 )
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(img_id, self._subset))
 
         if self._task is not CocoTask.panoptic:
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         ]
 
         for mask_path in masks:
             item_id = osp.splitext(osp.basename(mask_path))[0][len(self._mask_prefix) :]
 
             image = images.get(item_id)
             if image:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
 
             annotations = []
             mask = lazy_mask(mask_path, self._categories[AnnotationType.mask].inverse_colormap)
             mask = mask()  # loading mask through cache
 
             classes = np.unique(mask)
             for label_id in classes:
@@ -123,25 +123,24 @@
         return lambda: mask == c
 
 
 class CommonSemanticSegmentationImporter(Importer):
     """CommonSemanticSegmentation is introduced in the accuracy checker tool of OpenVINO™
     to cover a general format of datasets for semantic segmentation task.
     This should have the following structure:
-
-    └─ Dataset/
-        ├── dataset_meta.json # a list of labels
-        ├── images/
-        │   ├── <img1>.png
-        │   ├── <img2>.png
-        │   └── ...
-        └── masks/
-            ├── <img1>.png
-            ├── <img2>.png
-            └── ...
+        - Dataset/
+            - dataset_meta.json # a list of labels
+            - images/
+                - <img1>.png
+                - <img2>.png
+                - ...
+            - masks/
+                - <img1>.png
+                - <img2>.png
+                - ...
     """
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument("--image-prefix", default="", help="Image prefix (default: '')")
         parser.add_argument("--mask-prefix", default="", help="Mask prefix (default: '')")
@@ -162,21 +161,23 @@
         return [{"url": path, "format": "common_semantic_segmentation"}]
 
 
 @with_subset_dirs
 class CommonSemanticSegmentationWithSubsetDirsImporter(CommonSemanticSegmentationImporter):
     """It supports the following subset sub-directory structure for CommonSemanticSegmentation.
 
+    ```
     Dataset/
     └─ <split: train,val, ...>
         ├── dataset_meta.json # a list of labels
         ├── images/
         │   ├── <img1>.png
         │   ├── <img2>.png
         │   └── ...
         └── masks/
             ├── <img1>.png
             ├── <img2>.png
             └── ...
 
     Then, the imported dataset will have train, val, ... CommonSemanticSegmentation subsets.
+    ```
     """
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,32 +42,35 @@
         lr_image_dir = osp.join(path, CommonSuperResolutionPath.LR_IMAGES_DIR)
         for lr_image in find_images(lr_image_dir, recursive=True):
             item_id = osp.splitext(osp.relpath(lr_image, lr_image_dir))[0].replace("\\", "/")
 
             attributes = {}
             upsampled_image = upsampled_images.get(item_id)
             if upsampled_image:
-                attributes["upsampled"] = Image(path=upsampled_image)
+                attributes["upsampled"] = Image.from_file(path=upsampled_image)
 
             items[item_id] = DatasetItem(
-                id=item_id, subset=self._subset, media=Image(path=lr_image), attributes=attributes
+                id=item_id,
+                subset=self._subset,
+                media=Image.from_file(path=lr_image),
+                attributes=attributes,
             )
 
         hr_image_dir = osp.join(path, CommonSuperResolutionPath.HR_IMAGES_DIR)
         for hr_image in find_images(hr_image_dir, recursive=True):
             item_id = osp.splitext(osp.relpath(hr_image, hr_image_dir))[0].replace("\\", "/")
             if item_id not in items:
                 attributes = {}
                 upsampled_image = upsampled_images.get(item_id)
                 if upsampled_image:
-                    attributes["upsampled"] = Image(path=upsampled_image)
+                    attributes["upsampled"] = Image.from_file(path=upsampled_image)
 
                 items[item_id] = DatasetItem(id=item_id, subset=self._subset, attributes=attributes)
 
-            items[item_id].annotations = [SuperResolutionAnnotation(Image(path=hr_image))]
+            items[item_id].annotations = [SuperResolutionAnnotation(Image.from_file(path=hr_image))]
 
         return items
 
 
 class CommonSuperResolutionImporter(Importer):
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,17 +313,17 @@
 
     def _load_items(self, parsed):
         for frame_id, item_desc in parsed.items():
             name = item_desc.get("name", "frame_%06d.png" % int(frame_id))
             image = osp.join(self._images_dir, name)
             image_size = (item_desc.get("height"), item_desc.get("width"))
             if all(image_size):
-                image = Image(path=image, size=tuple(map(int, image_size)))
+                image = Image.from_file(path=image, size=tuple(map(int, image_size)))
             else:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
 
             subset = item_desc.get("subset")
             if subset is not None and subset != self._subset:
                 continue
             parsed[frame_id] = DatasetItem(
                 id=osp.splitext(name)[0],
                 subset=self._subset,
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     PolyLine,
     RleMask,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import parse_json_file
-from datumaro.version import VERSION
+from datumaro.version import __version__
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
 class DatumaroBase(SubsetBase):
     LEGACY_VERSION = "legacy"
     CURRENT_DATUMARO_FORMAT_VERSION = DATUMARO_FORMAT_VERSION
@@ -41,15 +41,15 @@
 
         dm_version = self._get_dm_format_version(path)
 
         # when backward compatibility happen, we should implement version specific readers
         if dm_version not in self.ALLOWED_VERSIONS:
             raise DatasetImportError(
                 f"Datumaro format version of the given dataset is {dm_version}, "
-                f"but not supported by this Datumaro version: {VERSION}. "
+                f"but not supported by this Datumaro version: {__version__}. "
                 f"The allowed datumaro format versions are {self.ALLOWED_VERSIONS}. "
                 "Please install the latest Datumaro."
             )
 
         self.default_reader(path=path)
 
     def default_reader(self, path: str):
@@ -67,19 +67,14 @@
         self._images_dir = images_dir
 
         pcd_dir = ""
         if rootpath and osp.isdir(osp.join(rootpath, DatumaroPath.PCD_DIR)):
             pcd_dir = osp.join(rootpath, DatumaroPath.PCD_DIR)
         self._pcd_dir = pcd_dir
 
-        related_images_dir = ""
-        if rootpath and osp.isdir(osp.join(rootpath, DatumaroPath.RELATED_IMAGES_DIR)):
-            related_images_dir = osp.join(rootpath, DatumaroPath.RELATED_IMAGES_DIR)
-        self._related_images_dir = related_images_dir
-
         super().__init__(subset=osp.splitext(osp.basename(path))[0])
         self._load_impl(path)
 
     def _get_dm_format_version(self, path: str):
         """
         Get Datumaro format at exporting the dataset
 
@@ -151,32 +146,36 @@
                 image_path = osp.join(self._images_dir, self._subset, image_filename)
                 if not osp.isfile(image_path):
                     # backward compatibility
                     old_image_path = osp.join(self._images_dir, image_filename)
                     if osp.isfile(old_image_path):
                         image_path = old_image_path
 
-                media = Image(path=image_path, size=image_info.get("size"))
+                media = Image.from_file(path=image_path, size=image_info.get("size"))
                 self._media_type = Image
 
             pcd_info = item_desc.get("point_cloud")
             if media and pcd_info:
                 raise DatasetImportError("Dataset cannot contain multiple media types")
             if pcd_info:
                 pcd_path = pcd_info.get("path")
                 point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
 
                 related_images = None
                 ri_info = item_desc.get("related_images")
                 if ri_info:
                     related_images = [
-                        Image(size=ri.get("size"), path=ri.get("path")) for ri in ri_info
+                        Image.from_file(
+                            size=ri.get("size"),
+                            path=osp.join(self._images_dir, self._subset, ri.get("path")),
+                        )
+                        for ri in ri_info
                     ]
 
-                media = PointCloud(point_cloud, extra_images=related_images)
+                media = PointCloud.from_file(path=point_cloud, extra_images=related_images)
                 self._media_type = PointCloud
 
             media_desc = item_desc.get("media")
             if not media and media_desc and media_desc.get("path"):
                 media = MediaElement(path=media_desc.get("path"))
                 self._media_type = MediaElement
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 20% similar despite different names*

```diff
@@ -84,54 +84,43 @@
             context: Context instance to help the media export
             encryption: If false, prevent the media from being encrypted
         """
         if item.media is None:
             yield
         elif isinstance(item.media, Image):
             image = item.media_as(Image)
-            path = image.path
 
             if context.save_media:
                 # Temporarily update image path and save it.
                 fname = context.make_image_filename(item)
                 context.save_image(item, encryption=encryption, fname=fname, subdir=item.subset)
-                image._path = fname
+                item.media = Image.from_file(path=fname, size=image._size)
 
             yield
-            image._path = path
+            item.media = image
         elif isinstance(item.media, PointCloud):
             pcd = item.media_as(PointCloud)
-            path = pcd.path
 
             if context.save_media:
-                # Temporarily update pcd path and save it.
-                fname = context.make_pcd_filename(item)
-                context.save_point_cloud(item, fname=fname, subdir=item.subset)
-                pcd._path = fname
-
-                # Temporarily update pcd related images paths and save them.
-                for i, img in enumerate(sorted(pcd.extra_images, key=lambda v: v.path)):
-                    img.__path = img.path
-                    fname = osp.join(item.id, f"image_{i}{context.find_image_ext(img)}")
-                    img._path = fname
-
-                    if img.has_data:
-                        context.save_image(
-                            item,
-                            basedir=context.related_images_dir,
-                            subdir=item.subset,
-                            fname=fname,
+                pcd_fname = context.make_pcd_filename(item)
+                context.save_point_cloud(item, fname=pcd_fname, subdir=item.subset)
+
+                extra_images = []
+                for i, extra_image in enumerate(pcd.extra_images):
+                    extra_images.append(
+                        Image.from_file(
+                            path=context.make_pcd_extra_image_filename(item, i, extra_image)
                         )
+                    )
+
+                # Temporarily update media with a new pcd saved into disk.
+                item.media = PointCloud.from_file(path=pcd_fname, extra_images=extra_images)
 
             yield
-            pcd._path = path
-            if context.save_media:
-                for img in pcd.extra_images:
-                    img._path = img.__path
-                    del img.__path
+            item.media = pcd
         else:
             raise NotImplementedError
 
     def add_item(self, item: DatasetItem, *args, **kwargs):
         annotations = []
         item_desc = {
             "id": item.id,
@@ -140,26 +129,26 @@
 
         if item.attributes:
             item_desc["attr"] = item.attributes
 
         with self.context_save_media(item, self.export_context):
             if isinstance(item.media, Image):
                 image = item.media_as(Image)
-                item_desc["image"] = {
-                    "path": image.path,
-                }
+                item_desc["image"] = {"path": getattr(image, "path", None)}
                 if item.media.has_size:  # avoid occasional loading
                     item_desc["image"]["size"] = image.size
             elif isinstance(item.media, PointCloud):
                 pcd = item.media_as(PointCloud)
 
-                item_desc["point_cloud"] = {"path": pcd.path}
+                item_desc["point_cloud"] = {"path": getattr(pcd, "path", None)}
 
                 related_images = [
-                    {"path": img.path, "size": img.size} if img.has_size else {"path": img.path}
+                    {"path": getattr(img, "path", None), "size": img.size}
+                    if img.has_size
+                    else {"path": getattr(img, "path", None)}
                     for img in pcd.extra_images
                 ]
 
                 if related_images:
                     item_desc["related_images"] = related_images
             elif isinstance(item.media, MediaElement):
                 item_desc["media"] = {"path": item.media.path}
@@ -375,22 +364,24 @@
 
 
 class DatumaroExporter(Exporter):
     DEFAULT_IMAGE_EXT = DatumaroPath.IMAGE_EXT
     PATH_CLS = DatumaroPath
 
     def create_writer(
-        self, subset: str, images_dir: str, pcd_dir: str, related_images_dir: str
+        self,
+        subset: str,
+        images_dir: str,
+        pcd_dir: str,
     ) -> _SubsetWriter:
         export_context = ExportContextComponent(
             save_dir=self._save_dir,
             save_media=self._save_media,
             images_dir=images_dir,
             pcd_dir=pcd_dir,
-            related_images_dir=related_images_dir,
             crypter=NULL_CRYPTER,
             image_ext=self._image_ext,
             default_image_ext=self._default_image_ext,
         )
 
         return _SubsetWriter(
             context=self,
@@ -406,19 +397,20 @@
         self._images_dir = images_dir
 
         annotations_dir = osp.join(self._save_dir, self.PATH_CLS.ANNOTATIONS_DIR)
         os.makedirs(annotations_dir, exist_ok=True)
         self._annotations_dir = annotations_dir
 
         self._pcd_dir = osp.join(self._save_dir, self.PATH_CLS.PCD_DIR)
-        self._related_images_dir = osp.join(self._save_dir, self.PATH_CLS.RELATED_IMAGES_DIR)
 
         writers = {
             subset: self.create_writer(
-                subset, self._images_dir, self._pcd_dir, self._related_images_dir
+                subset,
+                self._images_dir,
+                self._pcd_dir,
             )
             for subset in self._extractor.subsets()
         }
 
         for writer in writers.values():
             writer.add_infos(self._extractor.infos())
             writer.add_categories(self._extractor.categories())
@@ -461,12 +453,10 @@
 
             pcd_path = osp.join(
                 save_dir, cls.PATH_CLS.PCD_DIR, item.subset, conv._make_pcd_filename(item)
             )
             if osp.isfile(pcd_path):
                 os.unlink(pcd_path)
 
-            related_images_path = osp.join(
-                save_dir, cls.PATH_CLS.RELATED_IMAGES_DIR, item.subset, item.id
-            )
+            related_images_path = osp.join(save_dir, cls.PATH_CLS.IMAGES_DIR, item.subset, item.id)
             if osp.isdir(related_images_path):
                 shutil.rmtree(related_images_path)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,10 +33,10 @@
                 raise Exception
 
     @classmethod
     def find_sources(cls, path) -> List[Dict]:
         return cls._find_sources_recursive(
             path,
             cls.PATH_CLS.ANNOTATION_EXT,
-            cls.get_extractor_name(),
+            cls.NAME,
             dirname=cls.PATH_CLS.ANNOTATIONS_DIR,
         )
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import struct
 from io import BufferedReader
-from typing import Any, Dict, Optional
+from multiprocessing.pool import AsyncResult, Pool
+from typing import Any, Dict, List, Optional
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
+from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.media import Image, MediaElement, MediaType, PointCloud
 from datumaro.plugins.data_formats.datumaro_binary.format import DatumaroBinaryPath
 from datumaro.plugins.data_formats.datumaro_binary.mapper import DictMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import IntListMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.dataset_item import DatasetItemMapper
 
 from ..datumaro.base import DatumaroBase
 
 
 class DatumaroBinaryBase(DatumaroBase):
     """"""
 
-    def __init__(self, path: str, encryption_key: Optional[bytes] = None):
+    def __init__(self, path: str, encryption_key: Optional[bytes] = None, num_workers: int = 0):
+        """
+        Parameters
+        ----------
+        path
+            Directory path to import DatumaroBinary format dataset
+        encryption_key
+            If the dataset is encrypted, it (secret key) is needed to import the dataset.
+        num_workers
+            The number of multi-processing workers for import. If num_workers = 0, do not use multiprocessing.
+        """
         self._fp: Optional[BufferedReader] = None
         self._crypter = Crypter(encryption_key) if encryption_key is not None else NULL_CRYPTER
         self._media_encryption = False
+        self._num_workers = num_workers
         super().__init__(path)
 
     def _get_dm_format_version(self, path: str) -> str:
         with open(path, "rb") as fp:
             self._fp = fp
             self._check_signature()
             dm_format_version = self._read_version()
@@ -87,31 +100,79 @@
         elif media_type == MediaType.POINT_CLOUD:
             self._media_type = PointCloud
         elif media_type == MediaType.MEDIA_ELEMENT:
             self._media_type = MediaElement
         else:
             raise NotImplementedError(f"media_type={media_type} is currently not supported.")
 
-    def _read_items(self):
+    def _read_items(self) -> None:
         (n_blob_sizes_bytes,) = struct.unpack("<I", self._fp.read(4))
         blob_sizes_bytes = self._crypter.decrypt(self._fp.read(n_blob_sizes_bytes))
         blob_sizes, _ = IntListMapper.backward(blob_sizes_bytes, 0)
 
-        self._items = []
-
         media_path_prefix = {
             MediaType.IMAGE: osp.join(self._images_dir, self._subset),
             MediaType.POINT_CLOUD: osp.join(self._pcd_dir, self._subset),
         }
 
-        # For each blob, we decrypt the blob first, then extract items.
-        for blob_size in blob_sizes:
-            blob_bytes = self._crypter.decrypt(self._fp.read(blob_size))
-            offset = 0
-
-            while offset < len(blob_bytes):
-                item, offset = DatasetItemMapper.backward(blob_bytes, offset, media_path_prefix)
-                if item.media is not None and self._media_encryption:
-                    item.media.set_crypter(self._crypter)
-                self._items.append(item)
+        if self._num_workers > 0:
+            self._items = self._read_items_mp(blob_sizes, media_path_prefix)
+        else:
+            self._items = self._read_items_sp(blob_sizes, media_path_prefix)
+
+        for item in self._items:
+            if item.media is not None and self._media_encryption:
+                item.media.set_crypter(self._crypter)
+
+    def _read_items_mp(
+        self, blob_sizes: List[int], media_path_prefix: Dict[MediaType, str]
+    ) -> List[DatasetItem]:
+        async_results: List[AsyncResult] = []
+
+        with Pool(processes=self._num_workers) as pool:
+            for blob_size in blob_sizes:
+                blob_bytes = self._fp.read(blob_size)
+                async_results += [
+                    pool.apply_async(
+                        self._read_blob,
+                        (
+                            blob_bytes,
+                            self._crypter,
+                            media_path_prefix,
+                        ),
+                    )
+                ]
+
+            return [
+                item
+                for async_result in async_results
+                for item in async_result.get(timeout=DatumaroBinaryPath.MP_TIMEOUT)
+            ]
+
+    def _read_items_sp(
+        self, blob_sizes: List[int], media_path_prefix: Dict[MediaType, str]
+    ) -> List[DatasetItem]:
+        items_list = [
+            self._read_blob(self._fp.read(blob_size), self._crypter, media_path_prefix)
+            for blob_size in blob_sizes
+        ]
+
+        return [item for items in items_list for item in items]
+
+    @staticmethod
+    def _read_blob(
+        blob_bytes: bytes, crypter: Crypter, media_path_prefix: Dict[MediaType, str]
+    ) -> List[DatasetItem]:
+        items = []
+        offset = 0
+
+        # Decrypt bytes first
+        blob_bytes = crypter.decrypt(blob_bytes)
+
+        # Extract items
+        while offset < len(blob_bytes):
+            item, offset = DatasetItemMapper.backward(blob_bytes, offset, media_path_prefix)
+            items.append(item)
+
+        assert offset == len(blob_bytes)
 
-            assert offset == len(blob_bytes)
+        return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,17 @@
         with _SubsetWriter.context_save_media(item, context=context, encryption=media_encryption):
             return DatasetItemMapper.forward(item)
 
     def _dump_items(self, pool: Optional[Pool] = None):
         # Await async results
         if pool is not None:
             self._bytes = [
-                result.get() for result in self._bytes if isinstance(result, ApplyResult)
+                result.get(timeout=DatumaroBinaryPath.MP_TIMEOUT)
+                for result in self._bytes
+                if isinstance(result, ApplyResult)
             ]
 
         # Divide items to blobs
         blobs = [bytearray()]
         cur_blob = blobs[-1]
         for _bytes in self._bytes:
             cur_blob += _bytes
@@ -289,23 +291,20 @@
             save_media=save_media,
             image_ext=image_ext,
             default_image_ext=default_image_ext,
             save_dataset_meta=save_dataset_meta,
             ctx=ctx,
         )
 
-    def create_writer(
-        self, subset: str, images_dir: str, pcd_dir: str, related_images_dir: str
-    ) -> _SubsetWriter:
+    def create_writer(self, subset: str, images_dir: str, pcd_dir: str) -> _SubsetWriter:
         export_context = ExportContextComponent(
             save_dir=self._save_dir,
             save_media=self._save_media,
             images_dir=images_dir,
             pcd_dir=pcd_dir,
-            related_images_dir=related_images_dir,
             crypter=self._crypter,
             image_ext=self._image_ext,
             default_image_ext=self._default_image_ext,
         )
 
         return _SubsetWriter(
             context=self,
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 _SIGNATURE = "signature:datumaro_binary"
 
 
 class DatumaroBinaryPath:
     IMAGES_DIR = "images"
     ANNOTATIONS_DIR = "annotations"
     PCD_DIR = "point_clouds"
-    RELATED_IMAGES_DIR = "related_images"
     MASKS_DIR = "masks"
 
     ANNOTATION_EXT = ".datum"
     IMAGE_EXT = ".jpg"
     MASK_EXT = ".png"
     SIGNATURE = _SIGNATURE
     SIGNATURE_LEN = len(_SIGNATURE)
 
     SECRET_KEY_FILE = "secret_key.txt"
 
     MAX_BLOB_SIZE = 2**20  # 1 Mega bytes
+    MP_TIMEOUT = 300.0  # 5 minutes
 
     @classmethod
     def check_signature(cls, signature: str):
         if signature != cls.SIGNATURE:
             raise DatasetImportError(
                 f"Input signature={signature} is not aligned with the ground truth signature={cls.SIGNATURE}"
             )
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+# ruff: noqa: F405
+
 from .annotation import *
 from .common import *
 from .dataset_item import *
 from .media import *
 
 __all__ = [
     # anns
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .common import Mapper, StringMapper
 
 
 class MediaMapper(Mapper):
     @classmethod
     def forward(cls, obj: Optional[MediaElement]) -> bytes:
         if obj is None:
-            return struct.pack(f"<I", MediaType.NONE)
+            return struct.pack("<I", MediaType.NONE)
         elif obj._type == MediaType.IMAGE:
             return ImageMapper.forward(obj)
         elif obj._type == MediaType.POINT_CLOUD:
             return PointCloudMapper.forward(obj)
         elif obj._type == MediaType.MEDIA_ELEMENT:
             return MediaElementMapper.forward(obj)
         else:
@@ -44,64 +44,68 @@
         elif media_type == MediaType.MEDIA_ELEMENT:
             return MediaElementMapper.backward(_bytes, offset, media_path_prefix)
         else:
             raise DatumaroError(f"{media_type} is not allowed for MediaMapper.")
 
 
 class MediaElementMapper(Mapper):
+    MAGIC_PATH = "/NOT/A/REAL/PATH"
     MEDIA_TYPE = MediaType.MEDIA_ELEMENT
 
     @classmethod
     def forward(cls, obj: MediaElement) -> bytes:
         bytes_arr = bytearray()
-        bytes_arr.extend(struct.pack(f"<I", obj.type))
-        bytes_arr.extend(StringMapper.forward(obj.path))
+        bytes_arr.extend(struct.pack("<I", obj.type))
+        path = getattr(obj, "path", cls.MAGIC_PATH)
+        bytes_arr.extend(StringMapper.forward(path))
 
         return bytes(bytes_arr)
 
     @classmethod
     def backward_dict(
         cls,
         _bytes: bytes,
         offset: int = 0,
         media_path_prefix: Optional[Dict[MediaType, str]] = None,
     ) -> Tuple[Dict, int]:
         (media_type,) = struct.unpack_from("<I", _bytes, offset)
         assert media_type == cls.MEDIA_TYPE, f"Expect {cls.MEDIA_TYPE} but actual is {media_type}."
         offset += 4
         path, offset = StringMapper.backward(_bytes, offset)
+        if path == cls.MAGIC_PATH:
+            path = None
         return {
             "type": media_type,
             "path": path
-            if media_path_prefix is None
+            if path == cls.MAGIC_PATH or media_path_prefix is None
             else osp.join(media_path_prefix[cls.MEDIA_TYPE], path),
         }, offset
 
     @classmethod
     def backward(
         cls,
         _bytes: bytes,
         offset: int = 0,
         media_path_prefix: Optional[Dict[MediaType, str]] = None,
     ) -> Tuple[MediaElement, int]:
-        media_dict, offset = cls.backward_dict(_bytes, offset, media_path_prefix)
-        return MediaElement(path=media_dict["path"]), offset
+        _, offset = cls.backward_dict(_bytes, offset, media_path_prefix)
+        return MediaElement(), offset
 
 
 class ImageMapper(MediaElementMapper):
     MAGIC_SIZE_FOR_NONE = (-1583, -1597)
     MEDIA_TYPE = MediaType.IMAGE
 
     @classmethod
     def forward(cls, obj: Image) -> bytes:
         size = obj.size if obj.has_size else cls.MAGIC_SIZE_FOR_NONE
 
         bytes_arr = bytearray()
         bytes_arr.extend(super().forward(obj))
-        bytes_arr.extend(struct.pack(f"<ii", size[0], size[1]))
+        bytes_arr.extend(struct.pack("<ii", size[0], size[1]))
 
         return bytes(bytes_arr)
 
     @classmethod
     def backward(
         cls,
         _bytes: bytes,
@@ -109,27 +113,29 @@
         media_path_prefix: Optional[Dict[MediaType, str]] = None,
     ) -> Tuple[Image, int]:
         media_dict, offset = cls.backward_dict(_bytes, offset, media_path_prefix)
         height, width = struct.unpack_from("<ii", _bytes, offset)
         size = (height, width)
         offset += 8
         return (
-            Image(path=media_dict["path"], size=size if size != cls.MAGIC_SIZE_FOR_NONE else None),
+            Image.from_file(
+                path=media_dict["path"], size=size if size != cls.MAGIC_SIZE_FOR_NONE else None
+            ),
             offset,
         )
 
 
 class PointCloudMapper(MediaElementMapper):
     MEDIA_TYPE = MediaType.POINT_CLOUD
 
     @classmethod
     def forward(cls, obj: PointCloud) -> bytes:
         bytes_arr = bytearray()
         bytes_arr.extend(super().forward(obj))
-        bytes_arr.extend(struct.pack(f"<I", len(obj.extra_images)))
+        bytes_arr.extend(struct.pack("<I", len(obj.extra_images)))
         for img in obj.extra_images:
             bytes_arr.extend(ImageMapper.forward(img))
 
         return bytes(bytes_arr)
 
     @classmethod
     def backward(
@@ -140,11 +146,11 @@
     ) -> Tuple[PointCloud, int]:
         media_dict, offset = cls.backward_dict(_bytes, offset, media_path_prefix)
         (len_extra_images,) = struct.unpack_from("<I", _bytes, offset)
         offset += 4
 
         extra_images = []
         for _ in range(len_extra_images):
-            img, offset = ImageMapper.backward(_bytes, offset)
+            img, offset = ImageMapper.backward(_bytes, offset, media_path_prefix)
             extra_images.append(img)
 
-        return PointCloud(media_dict["path"], extra_images), offset
+        return PointCloud.from_file(path=media_dict["path"], extra_images=extra_images), offset
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                     image = objects[0][:-1]
                     captions = []
 
                 item_id = osp.splitext(image)[0]
                 image_path = osp.join(osp.dirname(self._path), IcdarPath.IMAGES_DIR, image)
                 if item_id not in items:
                     items[item_id] = DatasetItem(
-                        item_id, subset=self._subset, media=Image(path=image_path)
+                        item_id, subset=self._subset, media=Image.from_file(path=image_path)
                     )
 
                 annotations = items[item_id].annotations
                 for caption in captions:
                     annotations.append(Caption(caption))
 
         return items
@@ -101,15 +101,15 @@
                 item_id = osp.join(osp.dirname(item_id), osp.basename(item_id)[3:])
             item_id = item_id.replace("\\", "/")
 
             if item_id not in items:
                 image = None
                 image_path = images.get(item_id)
                 if image_path:
-                    image = Image(path=image_path)
+                    image = Image.from_file(path=image_path)
 
                 items[item_id] = DatasetItem(item_id, subset=self._subset, media=image)
             annotations = items[item_id].annotations
 
             with open(path, encoding="utf-8") as f:
                 for line in f:
                     line = line.strip()
@@ -172,15 +172,15 @@
             if item_id.endswith("_GT"):
                 item_id = item_id[:-3]
 
             if item_id not in items:
                 image = None
                 image_path = images.get(item_id)
                 if image_path:
-                    image = Image(path=image_path)
+                    image = Image.from_file(path=image_path)
 
                 items[item_id] = DatasetItem(item_id, subset=self._subset, media=image)
             annotations = items[item_id].annotations
 
             colors = [(255, 255, 255)]
             chars = [""]
             centers = [0]
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_dir.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     def __init__(self, url, subset=None):
         super().__init__(subset=subset)
 
         assert osp.isdir(url), url
 
         for path in find_images(url, recursive=True):
             item_id = osp.relpath(osp.splitext(path)[0], url)
-            self._items.append(DatasetItem(id=item_id, subset=self._subset, media=Image(path=path)))
+            self._items.append(
+                DatasetItem(id=item_id, subset=self._subset, media=Image.from_file(path=path))
+            )
 
 
 class ImageDirExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
     def apply(self):
         os.makedirs(self._save_dir, exist_ok=True)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_zip.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os.path as osp
 from enum import Enum
 from zipfile import ZIP_BZIP2, ZIP_DEFLATED, ZIP_LZMA, ZIP_STORED, ZipFile
 
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.exporter import Exporter
 from datumaro.components.importer import Importer
-from datumaro.components.media import ByteImage
+from datumaro.components.media import Image
 from datumaro.util import parse_str_enum_value
 from datumaro.util.image import IMAGE_EXTENSIONS, encode_image
 
 
 class Compression(Enum):
     ZIP_STORED = ZIP_STORED
     ZIP_DEFLATED = ZIP_DEFLATED
@@ -26,24 +26,24 @@
 class ImageZipPath:
     DEFAULT_ARCHIVE_NAME = "default.zip"
     DEFAULT_COMPRESSION = Compression.ZIP_STORED
 
 
 class ImageZipBase(SubsetBase):
     def __init__(self, url, subset=None):
-        super().__init__(subset=subset, media_type=ByteImage)
+        super().__init__(subset=subset, media_type=Image)
 
         assert url.endswith(".zip"), url
 
         with ZipFile(url, "r") as zf:
             for path in zf.filelist:
                 item_id, extension = osp.splitext(path.filename)
                 if extension.lower() not in IMAGE_EXTENSIONS:
                     continue
-                image = ByteImage(data=zf.read(path.filename))
+                image = Image.from_bytes(data=zf.read(path.filename))
                 self._items.append(DatasetItem(id=item_id, media=image, subset=self._subset))
 
 
 class ImageZipImporter(Importer):
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".zip", "image_zip")
@@ -111,13 +111,12 @@
                 if item.media:
                     self._archive_image(zf, item)
                 else:
                     log.debug("Item '%s' has no image info", item.id)
 
     def _archive_image(self, zipfile, item):
         image_name = self._make_image_filename(item)
-        if osp.isfile(item.media.path):
+        path = getattr(item.media, "path", None)
+        if path is not None and osp.isfile(path):
             zipfile.write(item.media.path, arcname=image_name)
-        elif isinstance(item.media, ByteImage):
-            zipfile.writestr(image_name, item.media.get_bytes())
         elif item.media.has_data:
             zipfile.writestr(image_name, encode_image(item.media.data, osp.splitext(image_name)[1]))
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datumaro.components.media import Image
 from datumaro.util.definitions import SUBSET_NAME_BLACKLIST
 from datumaro.util.image import find_images
 
 
 class ImagenetPath:
     IMAGE_DIR_NO_LABEL = "no_label"
+    SEP_TOKEN = ":"
 
 
 class ImagenetBase(SubsetBase):
     def __init__(self, path, subset=None):
         assert osp.isdir(path), path
         super().__init__(subset=subset)
 
@@ -41,18 +42,20 @@
 
         # Images should be in root/label_dir/*.img and root/*.img is not allowed.
         # => max_depth=1, min_depth=1
         for image_path in find_images(path, recursive=True, max_depth=1, min_depth=1):
             label = osp.basename(osp.dirname(image_path))
             image_name = osp.splitext(osp.basename(image_path))[0]
 
-            item_id = osp.join(label, image_name)
+            item_id = label + ImagenetPath.SEP_TOKEN + image_name
             item = items.get(item_id)
             if item is None:
-                item = DatasetItem(id=item_id, subset=self._subset, media=Image(path=image_path))
+                item = DatasetItem(
+                    id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
+                )
                 items[item_id] = item
             annotations = item.annotations
 
             if label != ImagenetPath.IMAGE_DIR_NO_LABEL:
                 label = self._categories[AnnotationType.label].find(label)[0]
                 annotations.append(Label(label=label))
 
@@ -125,44 +128,60 @@
 
     Then, it will have three subsets: train, val, and test and they have label_0 and label_1 labels.
     """
 
 
 class ImagenetExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
+    USE_SUBSET_DIRS = False
 
     def apply(self):
-        def _get_dir_name(id_parts, label_name):
-            if 1 < len(id_parts) and id_parts[0] == label_name:
-                return ""
+        def _get_name(item: DatasetItem) -> str:
+            id_parts = item.id.split(ImagenetPath.SEP_TOKEN)
+
+            if len(id_parts) == 1:
+                # e.g. item.id = my_img_1
+                return item.id
             else:
-                return label_name
+                # e.g. item.id = label_1:my_img_1
+                return "_".join(id_parts[1:])  # ":" is not allowed in windows
 
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
 
-        if 1 < len(self._extractor.subsets()):
+        if 1 < len(self._extractor.subsets()) and not self.USE_SUBSET_DIRS:
             log.warning(
-                "ImageNet format only supports exporting a single "
-                "subset, subset information will not be used."
+                f"There are more than one subset in the dataset ({len(self._extractor.subsets())}). "
+                "However, ImageNet format exports all dataset items into the same directory. "
+                "Therefore, subset information will be lost. To prevent it, please use ImagenetWithSubsetDirsExporter. "
+                'For example, dataset.export("<path/to/output>", format="imagenet_with_subset_dirs").'
             )
 
-        subset_dir = self._save_dir
+        root_dir = self._save_dir
         extractor = self._extractor
         labels = {}
         for item in self._extractor:
-            id_parts = item.id.split("/")
+            file_name = _get_name(item)
             labels = set(p.label for p in item.annotations if p.type == AnnotationType.label)
 
             for label in labels:
                 label_name = extractor.categories()[AnnotationType.label][label].name
                 self._save_image(
-                    item, subdir=osp.join(subset_dir, _get_dir_name(id_parts, label_name))
+                    item,
+                    subdir=osp.join(root_dir, item.subset, label_name)
+                    if self.USE_SUBSET_DIRS
+                    else osp.join(root_dir, label_name),
+                    name=file_name,
                 )
 
             if not labels:
                 self._save_image(
                     item,
-                    subdir=osp.join(
-                        subset_dir, _get_dir_name(id_parts, ImagenetPath.IMAGE_DIR_NO_LABEL)
-                    ),
+                    subdir=osp.join(root_dir, item.subset, ImagenetPath.IMAGE_DIR_NO_LABEL)
+                    if self.USE_SUBSET_DIRS
+                    else osp.join(root_dir, ImagenetPath.IMAGE_DIR_NO_LABEL),
+                    name=file_name,
                 )
+
+
+class ImagenetWithSubsetDirsExporter(ImagenetExporter):
+    USE_SUBSET_DIRS = True
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                             )
 
                     anno.append(Label(label))
 
                 items[item_id] = DatasetItem(
                     id=item_id,
                     subset=self._subset,
-                    media=Image(path=osp.join(self.image_dir, image)),
+                    media=Image.from_file(path=osp.join(self.image_dir, image)),
                     annotations=anno,
                 )
 
         return items
 
 
 class ImagenetTxtImporter(Importer, CliPlugin):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                             id=ann_id,
                             attributes={"is_crowd": isCrowd},
                         )
                     )
 
                 image = image_path_by_id.pop(item_id, None)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(
                     id=item_id, annotations=anns, media=image, subset=self._subset
                 )
 
         det_dir = osp.join(self._path, KittiPath.LABELS_DIR)
         if self._task == KittiTask.detection:
@@ -132,23 +132,23 @@
                             attributes=attributes,
                             label=label_id,
                         )
                     )
 
                 image = image_path_by_id.pop(item_id, None)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(
                     id=item_id, annotations=anns, media=image, subset=self._subset
                 )
 
         for item_id, image_path in image_path_by_id.items():
             items[item_id] = DatasetItem(
-                id=item_id, subset=self._subset, media=Image(path=image_path)
+                id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
             )
 
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,32 +237,36 @@
 
         items = {}
         for frame_id, item_desc in parsed.items():
             name = name_mapping.get(frame_id, "%010d" % int(frame_id))
             items[frame_id] = DatasetItem(
                 id=name,
                 subset=self._subset,
-                media=PointCloud(
-                    osp.join(self._rootdir, KittiRawPath.PCD_DIR, name + ".pcd"),
-                    extra_images=[Image(path=image) for image in sorted(images.get(name, []))],
+                media=PointCloud.from_file(
+                    path=osp.join(self._rootdir, KittiRawPath.PCD_DIR, name + ".pcd"),
+                    extra_images=[
+                        Image.from_file(path=image) for image in sorted(images.get(name, []))
+                    ],
                 ),
                 annotations=item_desc.get("annotations"),
                 attributes={"frame": int(frame_id)},
             )
 
         for frame_id, name in name_mapping.items():
             if frame_id in items:
                 continue
 
             items[frame_id] = DatasetItem(
                 id=name,
                 subset=self._subset,
-                media=PointCloud(
-                    osp.join(self._rootdir, KittiRawPath.PCD_DIR, name + ".pcd"),
-                    extra_images=[Image(path=image) for image in sorted(images.get(name, []))],
+                media=PointCloud.from_file(
+                    path=osp.join(self._rootdir, KittiRawPath.PCD_DIR, name + ".pcd"),
+                    extra_images=[
+                        Image.from_file(path=image) for image in sorted(images.get(name, []))
+                    ],
                 ),
                 attributes={"frame": int(frame_id)},
             )
 
         return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             image_size = None
             imagesize_elem = root.find("imagesize")
             if imagesize_elem is not None:
                 width_elem = imagesize_elem.find("ncols")
                 height_elem = imagesize_elem.find("nrows")
                 image_size = (int(height_elem.text), int(width_elem.text))
 
-            image = Image(path=image_path, size=image_size)
+            image = Image.from_file(path=image_path, size=image_size)
 
             annotations = self._parse_annotations(root, osp.join(dataset_root, subset), categories)
 
             items.append(
                 DatasetItem(id=item_id, subset=subset, media=image, annotations=annotations)
             )
             subsets.add(items[-1].subset)
@@ -412,15 +412,15 @@
             ET.SubElement(image_elem, "nrows").text = str(image_size[0])
             ET.SubElement(image_elem, "ncols").text = str(image_size[1])
 
         groups = defaultdict(list)
 
         obj_id = 0
         for ann in item.annotations:
-            if not ann.type in {AnnotationType.polygon, AnnotationType.bbox, AnnotationType.mask}:
+            if ann.type not in {AnnotationType.polygon, AnnotationType.bbox, AnnotationType.mask}:
                 continue
 
             obj_elem = ET.SubElement(root_elem, "object")
             ET.SubElement(obj_elem, "name").text = self._get_label(ann.label)
             ET.SubElement(obj_elem, "deleted").text = "0"
             ET.SubElement(obj_elem, "verified").text = "0"
             ET.SubElement(obj_elem, "occluded").text = (
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/lfw.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                         label = get_label_id(label_name)
                         if label is not None:
                             annotations.append(Label(label))
                             item_id = item_id[len(label_name) + 1 :]
                     if item_id not in items:
                         image = images.get(item_id)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[item_id] = DatasetItem(
                             id=item_id, subset=self._subset, media=image, annotations=annotations
                         )
                 elif len(pair) == 3:
                     image1, id1 = self.get_image_name(pair[0], pair[1])
                     image2, id2 = self.get_image_name(pair[0], pair[2])
@@ -112,26 +112,26 @@
 
                     if id1 not in items:
                         annotations = []
                         annotations.append(Label(label))
 
                         image = images.get(image1)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[id1] = DatasetItem(
                             id=id1, subset=self._subset, media=image, annotations=annotations
                         )
                     if id2 not in items:
                         annotations = []
                         annotations.append(Label(label))
 
                         image = images.get(image2)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[id2] = DatasetItem(
                             id=id2, subset=self._subset, media=image, annotations=annotations
                         )
 
                     # pairs form a directed graph
                     if not items[id1].annotations[0].attributes.get("positive_pairs"):
@@ -148,28 +148,28 @@
                     if id1 not in items:
                         annotations = []
                         label = get_label_id(pair[0])
                         annotations.append(Label(label))
 
                         image = images.get(image1)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[id1] = DatasetItem(
                             id=id1, subset=self._subset, media=image, annotations=annotations
                         )
                     if id2 not in items:
                         annotations = []
                         if pair[2] != "-":
                             label = get_label_id(pair[2])
                             annotations.append(Label(label))
 
                         image = images.get(image2)
                         if image:
-                            image = Image(path=image)
+                            image = Image.from_file(path=image)
 
                         items[id2] = DatasetItem(
                             id=id2, subset=self._subset, media=image, annotations=annotations
                         )
 
                     # pairs form a directed graph
                     if not items[id1].annotations[0].attributes.get("negative_pairs"):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             for img in config["images"]
         }
 
         for item_ann in config["annotations"]:
             item_id = item_ann["image_id"]
             image = None
             if images_info.get(item_id):
-                image = Image(
+                image = Image.from_file(
                     path=images_info[item_id]["path"],
                     size=self._get_image_size(images_info[item_id]),
                 )
 
             annotations = []
             mask_path = osp.join(
                 self._annotations_dir, MapillaryVistasPath.PANOPTIC_DIR, item_ann["file_name"]
@@ -212,15 +212,15 @@
                     Mask(label=label_id, image=self._lazy_extract_mask(class_mask, label_id))
                 )
 
             items[item_id] = DatasetItem(id=item_id, subset=self._subset, annotations=annotations)
 
         for image_path in find_images(self._images_dir, recursive=True):
             item_id = osp.splitext(osp.relpath(image_path, self._images_dir))[0]
-            image = Image(path=image_path)
+            image = Image.from_file(path=image_path)
             if item_id in items:
                 items[item_id].media = image
             else:
                 items[item_id] = DatasetItem(id=item_id, subset=self._subset, media=image)
 
         self._load_polygons(items)
         return items.values()
@@ -231,15 +231,15 @@
             item_id = osp.splitext(osp.relpath(item_path, polygons_dir))[0]
             item = items.get(item_id)
             item_info = {}
             item_info = parse_json_file(item_path)
 
             image_size = self._get_image_size(item_info)
             if image_size and item.has_image:
-                item.media = Image(path=item.image.path, size=image_size)
+                item.media = Image.from_file(path=item.image.path, size=image_size)
 
             polygons = item_info["objects"]
             annotations = []
             for polygon in polygons:
                 label = polygon["label"]
                 label_id = self._categories[AnnotationType.label].find(label)[0]
                 if label_id is None:
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/market1501.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,15 +91,18 @@
                 custom_name = search.groups()[5]
                 if custom_name:
                     item_id = osp.join(osp.dirname(item_id), custom_name)
 
             item = items.get(item_id)
             if item is None:
                 item = DatasetItem(
-                    id=item_id, subset=subset, media=Image(path=image_path), attributes=attributes
+                    id=item_id,
+                    subset=subset,
+                    media=Image.from_file(path=image_path),
+                    attributes=attributes,
                 )
                 items[item_id] = item
 
         return items
 
 
 class Market1501Importer(Importer):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mars.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mars.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                         f"the directory name: {label}"
                     )
                     continue
 
                 items.append(
                     DatasetItem(
                         id=item_id,
-                        media=Image(path=image_path),
+                        media=Image.from_file(path=image_path),
                         subset=subset,
                         annotations=[Label(label=label_id)],
                         attributes={
                             "person_id": pedestrian_id,
                             "camera_id": int(image_name[5]),
                             "track_id": int(image_name[7:11]),
                             "frame_id": int(image_name[12:15]),
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     h, w = int(meta[i][-2]), int(meta[i][-1])
                     image = images[pix_num : pix_num + h * w].reshape(h, w)
                     pix_num += h * w
                 else:
                     image = images[i].reshape(MnistPath.IMAGE_SIZE, MnistPath.IMAGE_SIZE)
 
             if image is not None:
-                image = Image(data=image)
+                image = Image.from_numpy(data=image)
 
             if 0 < len(meta) and (len(meta[i]) == 1 or len(meta[i]) == 3):
                 i = meta[i][0]
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=annotations)
         return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     image = np.array([int(pix) for pix in data[1:]], dtype="uint8").reshape(
                         int(meta[i][-2]), int(meta[i][-1])
                     )
                 else:
                     image = np.array([int(pix) for pix in data[1:]], dtype="uint8").reshape(28, 28)
 
             if image is not None:
-                image = Image(data=image)
+                image = Image.from_numpy(data=image)
 
             if 0 < len(meta) and len(meta[i]) in [1, 3]:
                 i = meta[i][0]
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=item_anno)
         return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mot.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mot.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,25 +130,27 @@
         items = OrderedDict()
 
         if self._seq_info:
             for frame_id in range(1, self._seq_info["seqlength"] + 1):  # base-1 frame ids
                 items[frame_id] = DatasetItem(
                     id=frame_id,
                     subset=self._subset,
-                    media=Image(
+                    media=Image.from_file(
                         path=osp.join(
                             self._image_dir, "%06d%s" % (frame_id, self._seq_info["imext"])
                         ),
                         size=(self._seq_info["imheight"], self._seq_info["imwidth"]),
                     ),
                 )
         elif osp.isdir(self._image_dir):
             for p in find_images(self._image_dir):
                 frame_id = int(osp.splitext(osp.relpath(p, self._image_dir))[0])
-                items[frame_id] = DatasetItem(id=frame_id, subset=self._subset, media=Image(path=p))
+                items[frame_id] = DatasetItem(
+                    id=frame_id, subset=self._subset, media=Image.from_file(path=p)
+                )
 
         with open(path, newline="", encoding="utf-8") as csv_file:
             # NOTE: Different MOT files have different count of fields
             # (7, 9 or 10). This is handled by reader:
             # - all extra fields go to a separate field
             # - all unmet fields have None values
             for row in csv.DictReader(csv_file, fieldnames=MotPath.FIELDS):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mots.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mots.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         else:
             images = {}
 
         for p in sorted(iglob(self._anno_dir + "/**/*.png", recursive=True)):
             item_id = osp.splitext(osp.relpath(p, self._anno_dir))[0]
             image = images.get(item_id)
             if image:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
             items.append(
                 DatasetItem(
                     id=item_id,
                     subset=self._subset,
                     media=image,
                     annotations=self._parse_annotations(p),
                 )
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                     )
 
                     group_num += 1
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
-                media=Image(path=osp.join(root_dir, ann.get("img_paths", ""))),
+                media=Image.from_file(path=osp.join(root_dir, ann.get("img_paths", ""))),
                 annotations=annotations,
             )
 
         return items
 
 
 class MpiiJsonImporter(Importer):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 group_num += 1
 
             item_id = osp.splitext(image)[0]
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
-                media=Image(path=osp.join(root_dir, image)),
+                media=Image.from_file(path=osp.join(root_dir, image)),
                 annotations=annotations,
             )
 
         return items
 
 
 class MpiiImporter(Importer):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         for image_path in find_images(self._path, recursive=True, max_depth=2):
             label = osp.basename(osp.dirname(image_path))
             label_id = self._categories[AnnotationType.label].find(label)[0]
             item_id = label + "/" + osp.splitext(osp.basename(image_path))[0]
 
             item = items.get(item_id)
             if item is None:
-                item = DatasetItem(id=item_id, subset=self._subset, media=Image(path=image_path))
+                item = DatasetItem(
+                    id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
+                )
                 items[item_id] = item
 
             anns = item.annotations
             if self._task == MvtecTask.classification:
                 anns.append(Label(label=label_id))
             elif self._task == MvtecTask.segmentation:
                 mask_path = osp.join(self._path, "..", MvtecPath.MASK_DIR)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
 
     @classmethod
     def find_sources(cls, path):
         subset_paths = glob(osp.join(path, "*"), recursive=False)
 
         # MVTec format should have MvtecPath.MASK_DIR directory.
-        if not MvtecPath.MASK_DIR in [osp.basename(path) for path in subset_paths]:
+        if MvtecPath.MASK_DIR not in [osp.basename(path) for path in subset_paths]:
             return []
 
         sources = []
         for extractor_type in cls._TASKS.values():
             for subset_path in subset_paths:
                 if osp.isdir(subset_path) and MvtecPath.MASK_DIR not in subset_path:
                     sources.append(
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,16 +32,16 @@
             item_id = osp.splitext(osp.basename(anno_file))[0]
             with h5py.File(anno_file, "r") as f:
                 image = np.transpose(f["rgb"], (1, 2, 0))
                 depth = f["depth"][:].astype("float16")
 
             items[item_id] = DatasetItem(
                 id=item_id,
-                media=Image(data=image),
-                annotations=[DepthAnnotation(image=Image(data=depth))],
+                media=Image.from_numpy(data=image),
+                annotations=[DepthAnnotation(image=Image.from_numpy(data=depth))],
             )
 
         return items
 
 
 class NyuDepthV2Importer(Importer):
     @classmethod
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/open_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         image = None
         if image_path is None:
             log.warning(
                 "Can't find image for item: %s. "
                 "It should be in the '%s' directory" % (item_id, OpenImagesPath.IMAGES_DIR)
             )
         else:
-            image = Image(path=image_path, size=self._image_meta.get(item_id))
+            image = Image.from_file(path=image_path, size=self._image_meta.get(item_id))
 
         item = DatasetItem(id=item_id, media=image, subset=subset)
         self._items.append(item)
         return item
 
     def _get_subset_name(self, filename):
         parts = filename.split("-")
@@ -477,18 +477,19 @@
     def _load_masks(self, items_by_id, normalized_coords):
         label_categories = self._categories[AnnotationType.label]
 
         for mask_path in self._glob_annotations("*" + OpenImagesPath.MASK_DESCRIPTION_FILE_SUFFIX):
             with self._open_csv_annotation(mask_path) as mask_reader:
                 for mask_description in mask_reader:
                     mask_path = mask_description["MaskPath"]
+                    image_id = mask_description["ImageID"]
+
                     if _RE_INVALID_PATH_COMPONENT.fullmatch(mask_path):
-                        raise UnsupportedMaskPathError(item_id=item.id, mask_path=mask_path)
+                        raise UnsupportedMaskPathError(item_id=image_id, mask_path=mask_path)
 
-                    image_id = mask_description["ImageID"]
                     item = items_by_id.get(image_id)
                     if item is None:
                         item = items_by_id.setdefault(
                             image_id, self._add_item(image_id, self._get_subset_name(mask_path))
                         )
 
                     label_name = mask_description["LabelName"]
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,20 +157,22 @@
                 self._rootdir,
                 PointCloudPath.BASE_DIR,
                 PointCloudPath.RELATED_IMAGES_DIR,
                 name + "_pcd",
             )
             related_images = None
             if osp.isdir(related_images_dir):
-                related_images = [Image(path=image) for image in find_images(related_images_dir)]
+                related_images = [
+                    Image.from_file(path=image) for image in find_images(related_images_dir)
+                ]
 
             parsed[frame_id] = DatasetItem(
                 id=name,
                 subset=self._subset,
-                media=PointCloud(pcd_path, extra_images=related_images),
+                media=PointCloud.from_file(path=pcd_path, extra_images=related_images),
                 annotations=frame_desc.get("annotations"),
                 attributes={"frame": int(frame_id), **frame_desc["attributes"]},
             )
 
         return parsed
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/synthia.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/synthia.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                             label=segm_id,
                             attributes=attr,
                         )
                     )
 
                 image = images.get(item_id)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
         elif osp.isdir(osp.join(root_dir, SynthiaPath.SEMANTIC_SEGM_DIR)):
             gt_dir = osp.join(root_dir, SynthiaPath.SEMANTIC_SEGM_DIR)
             gt_images = find_images(gt_dir, recursive=True)
             for gt_img in gt_images:
@@ -171,15 +171,15 @@
                 for label_id in classes:
                     anno.append(
                         Mask(image=self._lazy_extract_mask(color_mask, label_id), label=label_id)
                     )
 
                 image = images.get(item_id)
                 if image:
-                    image = Image(path=image)
+                    image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
 
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import OrderedDict
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.importer import Importer
-from datumaro.components.media import ByteImage
+from datumaro.components.media import Image
 from datumaro.util.image import decode_image, lazy_image
 from datumaro.util.tf_util import import_tf as _import_tf
 
 from .format import DetectionApiPath
 
 tf = _import_tf()
 
@@ -152,23 +152,22 @@
                     h = clamp(shape[4] * frame_height, 0, frame_height) - y
                     annotations.append(Bbox(x, y, w, h, label=dataset_labels.get(label)))
 
             image_size = None
             if frame_height and frame_width:
                 image_size = (frame_height, frame_width)
 
-            image_params = {}
-            if frame_image:
-                image_params["data"] = frame_image
-            if frame_filename:
-                image_params["path"] = osp.join(images_dir, frame_filename)
-
             image = None
-            if image_params:
-                image = ByteImage(**image_params, size=image_size)
+            if frame_image:
+                if isinstance(frame_image, np.ndarray):
+                    image = Image.from_numpy(data=frame_image, size=image_size)
+                else:
+                    image = Image.from_bytes(data=frame_image, size=image_size)
+            elif frame_filename:
+                image = Image.from_file(path=osp.join(images_dir, frame_filename), size=image_size)
 
             dataset_items.append(
                 DatasetItem(
                     id=item_id,
                     subset=subset,
                     media=image,
                     annotations=annotations,
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import os.path as osp
 import string
 from collections import OrderedDict
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.exporter import Exporter
-from datumaro.components.media import ByteImage, Image
+from datumaro.components.media import ByteImage, Image, ImageFromBytes
 from datumaro.util.annotation_util import find_group_leader, find_instances, max_bbox
 from datumaro.util.image import encode_image
 from datumaro.util.mask_tools import merge_masks
 from datumaro.util.tf_util import import_tf as _import_tf
 
 from .format import DetectionApiPath
 
@@ -207,26 +207,30 @@
         features.update(self._export_instances(instances, width, height))
 
         tf_example = tf.train.Example(features=tf.train.Features(feature=features))
 
         return tf_example
 
     def _save_image(self, item, path=None):  # pylint: disable=arguments-differ
-        src_ext = item.media.ext.lower()
+        src_ext = item.media.ext.lower() if item.media.ext else item.media.ext
         dst_ext = osp.splitext(osp.basename(path))[1].lower()
         fmt = DetectionApiPath.IMAGE_EXT_FORMAT.get(dst_ext, "")
         if not fmt:
             log.warning(
                 "Item '%s': can't find format string for the '%s' "
                 "image extension, the corresponding field will be empty." % (item.id, dst_ext)
             )
 
-        if src_ext == dst_ext and isinstance(item.media, ByteImage):
-            buffer = item.media.get_bytes()
-        else:
+        buffer = None
+        if src_ext == dst_ext:
+            if isinstance(item.media, ByteImage):
+                buffer = item.media.get_bytes()
+            elif isinstance(item.media, ImageFromBytes):
+                buffer = item.media.bytes
+        if buffer is None:
             buffer = encode_image(item.media.data, dst_ext)
         return buffer, fmt
 
     @classmethod
     def patch(cls, dataset, patch, save_dir, **kwargs):
         for subset in patch.updated_subsets:
             cls.convert(dataset.get_subset(subset), save_dir=save_dir, **kwargs)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 label = None
                 if "/" in item_id:
                     label = _get_label(item_id)
 
                 if item_id not in items:
                     image = images.get(row["NAME_ID"])
                     if image:
-                        image = Image(path=image)
+                        image = Image.from_file(path=image)
                     items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
 
                 annotations = items[item_id].annotations
                 if [a for a in annotations if a.type == AnnotationType.points]:
                     raise Exception(
                         "Item %s: an image can have only one " "set of landmarks" % item_id
                     )
@@ -164,15 +164,15 @@
                 label = None
                 if "/" in item_id:
                     label = _get_label(item_id)
 
                 if item_id not in items:
                     image = images.get(row["NAME_ID"])
                     if image:
-                        image = Image(path=image)
+                        image = Image.from_file(path=image)
                     items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
 
                 annotations = items[item_id].annotations
                 if [a for a in annotations if a.type == AnnotationType.bbox]:
                     raise Exception("Item %s: an image can have only one " "bbox" % item_id)
 
                 if len([p for p in row if row[p] == ""]) == 0 and len(row) == 5:
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/video.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
         for item_id in self._ctx.progress_reporter.iter(
             self._items, desc=f"Parsing labels in '{self._subset}'"
         ):
             log.debug("Reading item '%s'", item_id)
             image = images.get(item_id)
             if image:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
             yield DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=annotations.get(item_id)
             )
 
     def _load_annotations(self):
         annotations = {}
         task_dir = osp.dirname(self._path)
@@ -217,15 +217,15 @@
 
                     anns = self._parse_annotations(root_elem, item_id=(item_id, self._subset))
 
                 if image is None:
                     image = images.pop(item_id, None)
 
                 if image or size:
-                    image = Image(path=image, size=size)
+                    image = Image.from_file(path=image, size=size)
 
                 yield DatasetItem(id=item_id, subset=self._subset, media=image, annotations=anns)
             except ElementTree.ParseError as e:
                 readable_wrapper = InvalidAnnotationError("Failed to parse XML file")
                 readable_wrapper.__cause__ = e
                 self._ctx.error_policy.report_item_error(
                     readable_wrapper, item_id=(item_id, self._subset)
@@ -376,15 +376,15 @@
         for item_id in self._ctx.progress_reporter.iter(
             self._items, desc=f"Parsing segmentation in '{self._subset}'"
         ):
             log.debug("Reading item '%s'", item_id)
 
             image = images.get(item_id)
             if image:
-                image = Image(path=image)
+                image = Image.from_file(path=image)
 
             try:
                 yield DatasetItem(
                     id=item_id,
                     subset=self._subset,
                     media=image,
                     annotations=self._load_annotations(item_id),
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
             if item.media and item.media.has_size:
                 h, w = item.media.size
                 size_elem = ET.SubElement(root_elem, "size")
                 ET.SubElement(size_elem, "width").text = str(w)
                 ET.SubElement(size_elem, "height").text = str(h)
                 depth = ""
-                if item.media.data is not None:
+                if item.media.has_data:
                     depth = str(item.media.data.shape[-1])
                 ET.SubElement(size_elem, "depth").text = depth
 
             item_segmented = 0 < len(masks)
             ET.SubElement(root_elem, "segmented").text = str(int(item_segmented))
 
             objects_with_parts = []
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             for row in csv.DictReader(content):
                 item_id = osp.splitext(row["image"])[0]
 
                 if item_id not in items:
                     items[item_id] = DatasetItem(
                         id=item_id,
                         subset=self._subset,
-                        media=Image(path=osp.join(osp.dirname(path), row["image"])),
+                        media=Image.from_file(path=osp.join(osp.dirname(path), row["image"])),
                     )
 
                 annotations = items[item_id].annotations
 
                 label_name = row.get("label")
                 x_min = row.get("xmin")
                 y_min = row.get("ymin")
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
                             )
                         )
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
                 attributes={"id": id},
-                media=Image(path=osp.join(osp.dirname(path), asset.get("asset", {}).get("path"))),
+                media=Image.from_file(
+                    path=osp.join(osp.dirname(path), asset.get("asset", {}).get("path"))
+                ),
                 annotations=annotations,
             )
 
         return items
 
 
 class VottJsonImporter(Importer):
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/widerface.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                     if label is not None:
                         annotations.append(Label(label=label))
                 item_id = item_id[len(item_id.split("/")[0]) + 1 :]
 
             items[item_id] = DatasetItem(
                 id=item_id,
                 subset=self._subset,
-                media=Image(path=image_path),
+                media=Image.from_file(path=image_path),
                 annotations=annotations,
             )
 
             try:
                 bbox_count = int(lines[line_idx + 1])
             except ValueError:  # can be the next image
                 continue
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         self._image_info = self.parse_image_info(rootpath, image_info)
 
         config = self._parse_config(config_path)
 
         names_path = config.get("names")
         if not names_path:
-            raise InvalidAnnotationError(f"Failed to parse names file path from config")
+            raise InvalidAnnotationError("Failed to parse names file path from config")
 
         # The original format is like this:
         #
         # classes = 2
         # train  = data/train.txt
         # valid  = data/test.txt
         # names = data/obj.names
@@ -169,15 +169,15 @@
     def _get(self, item_id: str, subset_name: str) -> Optional[DatasetItem]:
         subset = self._subsets[subset_name]
         item = subset.items[item_id]
 
         if isinstance(item, str):
             try:
                 image_size = self._image_info.get(item_id)
-                image = Image(path=osp.join(self._path, item), size=image_size)
+                image = Image.from_file(path=osp.join(self._path, item), size=image_size)
 
                 anno_path = osp.splitext(image.path)[0] + ".txt"
                 annotations = self._parse_annotations(
                     anno_path,
                     image,
                     label_categories=self._categories[AnnotationType.label],
                 )
@@ -322,15 +322,15 @@
             for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
             if extract_subset_name_from_parent(img_file, rootpath) == self._subset
         }
 
         for url in urls:
             try:
                 fname = _get_fname(url)
-                img = Image(path=img_files[fname])
+                img = Image.from_file(path=img_files[fname])
                 anns = YoloStrictBase._parse_annotations(
                     url,
                     img,
                     label_categories=label_categories,
                 )
                 self._items.append(
                     DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
```

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/ndr.py` & `datumaro-1.2.0rc1/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.2.0rc1/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.2.0rc1/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/searcher.py` & `datumaro-1.2.0rc1/datumaro/plugins/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/shift_analyzer.py` & `datumaro-1.2.0rc1/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/splitter.py` & `datumaro-1.2.0rc1/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -993,8 +993,8 @@
 66 88 107
 77 97 115
 73 94 104
 66 83 93
 85 103 111
 93 116 124
 73 118 131
-102 115 126
+102 115 126
```

### Comparing `datumaro-1.1.1/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.2.0rc1/datumaro/plugins/tiling/merge_tile.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             max_w = max(max_w, x + w)
             max_h = max(max_h, y + h)
         img_size = (max_h, max_w)
 
         merged_item = self.wrap_item(
             items[0],
             id=item_id,
-            media=MosaicImage(
+            media=MosaicImage.from_image_roi_pairs(
                 [
                     (
                         item.media,
                         item.attributes.get("roi"),
                     )
                     for item in items
                 ],
```

### Comparing `datumaro-1.1.1/datumaro/plugins/tiling/tile.py` & `datumaro-1.2.0rc1/datumaro/plugins/tiling/tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         )
         parser.add_argument(
             "--threshold-drop-ann",
             type=float,
             default=0.5,
             help="Threshold for dropping Polygon and Bbox annotations when tiling."
             " Polygon and Bbox should be cropped if they exist on the edge of the tiled image."
-            " If an area of the cropped annotation / an area of the original annoation  < `threshold_drop_ann`,"
+            " If an area of the cropped annotation / an area of the original annoation < `threshold_drop_ann`,"
             " drop the corresponding annotation.",
         )
         return parser
 
     def __init__(
         self,
         extractor,
@@ -234,15 +234,15 @@
         items: List[DatasetItem] = []
         rois = self._extract_rois(item.media)
         for idx, roi in enumerate(rois):
             items += [
                 self.wrap_item(
                     item,
                     id=item.id + f"_tile_{idx}",
-                    media=RoIImage.create_from_image(item.media, roi),
+                    media=RoIImage.from_image(item.media, roi),
                     attributes=self._get_tiled_attributes(item, idx, roi),
                     annotations=self._get_tiled_annotations(item, roi),
                 )
             ]
 
         return items
```

### Comparing `datumaro-1.1.1/datumaro/plugins/tiling/util.py` & `datumaro-1.2.0rc1/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/plugins/transforms.py` & `datumaro-1.2.0rc1/datumaro/plugins/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,42 @@
         self._start = start
 
     def __iter__(self):
         for i, item in enumerate(self._extractor):
             yield self.wrap_item(item, id=i + self._start)
 
 
+class Sort(Transform, CliPlugin):
+    """
+    Sorts dataset items.
+    """
+
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument("-k", "--key", type=str, default=None, help="key functions to sort.")
+        return parser
+
+    def __init__(self, extractor, key=None):
+        super().__init__(extractor)
+        if key:
+            if isinstance(key, str):
+                key = eval(key)
+            if not callable(key):
+                raise Exception("key must be a function with one argument.")
+        else:
+            key = lambda item: item.id
+        self._key = key
+
+    def __iter__(self):
+        items = sorted(list(iter(self._extractor)), key=lambda item: self._key(item))
+        for item in items:
+            yield item
+
+
 class MapSubsets(ItemTransform, CliPlugin):
     """
     Renames subsets in the dataset.
     """
 
     @staticmethod
     def _mapping_arg(s):
@@ -952,27 +980,27 @@
 
         assert width > 0 and height > 0
         self._width = width
         self._height = height
 
     @staticmethod
     def _lazy_resize_image(image, new_size):
-        def _resize_image(_):
+        def _resize_image():
             h, w = image.size
             yscale = new_size[0] / float(h)
             xscale = new_size[1] / float(w)
 
             # LANCZOS4 is preferable for upscaling, but it works quite slow
             method = cv2.INTER_AREA if (xscale * yscale) < 1 else cv2.INTER_CUBIC
 
             resized_image = cv2.resize(image.data / 255.0, new_size[::-1], interpolation=method)
             resized_image *= 255.0
             return resized_image
 
-        return Image(_resize_image, ext=image.ext, size=new_size)
+        return Image.from_numpy(_resize_image, ext=image.ext, size=new_size)
 
     @staticmethod
     def _lazy_resize_mask(mask, new_size):
         def _resize_image():
             # Can use only NEAREST for masks,
             # because we can't have interpolated values
             rescaled_mask = cv2.resize(
```

### Comparing `datumaro-1.1.1/datumaro/plugins/validators.py` & `datumaro-1.2.0rc1/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/__init__.py` & `datumaro-1.2.0rc1/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/annotation_util.py` & `datumaro-1.2.0rc1/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/attrs_util.py` & `datumaro-1.2.0rc1/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/image.py` & `datumaro-1.2.0rc1/datumaro/util/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #
 # SPDX-License-Identifier: MIT
 
 import importlib
 import os
 import os.path as osp
 import shlex
-import shutil
 import warnings
 import weakref
+from contextlib import contextmanager
 from enum import Enum, auto
-from io import BytesIO
+from io import BytesIO, IOBase
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 
 import numpy as np
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.errors import DatumaroError
 
@@ -89,45 +89,59 @@
 
     assert len(image.shape) in {2, 3}
     if len(image.shape) == 3:
         assert image.shape[2] in {3, 4}
     return image
 
 
-def copyto_image(src_path: str, dst_path: str, src_crypter: Crypter, dst_crypter: Crypter) -> None:
-    if src_crypter == dst_crypter:
-        if src_path == dst_path:
-            return
-
-        shutil.copyfile(src_path, dst_path)
+def copyto_image(
+    src: Union[str, IOBase], dst: Union[str, IOBase], src_crypter: Crypter, dst_crypter: Crypter
+) -> None:
+    if src_crypter == dst_crypter and src == dst:
         return
 
-    with open(src_path, "rb") as read_fp:
-        _bytes = src_crypter.decrypt(read_fp.read())
+    @contextmanager
+    def _open(fp, mode):
+        was_file = False
+        if not isinstance(fp, IOBase):
+            was_file = True
+            fp = open(fp, mode)
+        yield fp
+        if was_file:
+            fp.close()
+
+    with _open(src, "rb") as src_fp:
+        _bytes = src_crypter.decrypt(src_fp.read())
 
-    with open(dst_path, "wb") as write_fp:
-        write_fp.write(dst_crypter.encrypt(_bytes))
+    with _open(dst, "wb") as dst_fp:
+        dst_fp.write(dst_crypter.encrypt(_bytes))
 
 
 def save_image(
-    path: str,
+    dst: Union[str, IOBase],
     image: np.ndarray,
+    ext: Optional[str] = None,
     create_dir: bool = False,
     dtype: DTypeLike = np.uint8,
     crypter: Crypter = NULL_CRYPTER,
     **kwargs,
 ) -> None:
     # NOTE: Check destination path for existence
     # OpenCV silently fails if target directory does not exist
-    dst_dir = osp.dirname(path)
-    if dst_dir:
-        if create_dir:
-            os.makedirs(dst_dir, exist_ok=True)
-        elif not osp.isdir(dst_dir):
-            raise FileNotFoundError("Directory does not exist: '%s'" % dst_dir)
+    if isinstance(dst, IOBase):
+        ext = ext if ext else ".png"
+    else:
+        dst_dir = osp.dirname(dst)
+        if dst_dir:
+            if create_dir:
+                os.makedirs(dst_dir, exist_ok=True)
+            elif not osp.isdir(dst_dir):
+                raise FileNotFoundError("Directory does not exist: '%s'" % dst_dir)
+        # file extension and actual encoding can be differ
+        ext = ext if ext else osp.splitext(dst)[1]
 
     if not kwargs:
         kwargs = {}
 
     # NOTE: OpenCV documentation says "If the image format is not supported,
     # the image will be converted to 8-bit unsigned and saved that way".
     # Conversion from np.int32 to np.uint8 is not working properly
@@ -135,35 +149,40 @@
     if dtype == np.int32:
         backend = _IMAGE_BACKENDS.PIL
     if backend == _IMAGE_BACKENDS.cv2:
         # cv2.imwrite does not support paths that are not representable
         # in the locale encoding on Windows, so we write the image bytes
         # ourselves.
 
-        ext = osp.splitext(path)[1]
         image_bytes = encode_image(image, ext, dtype=dtype, **kwargs)
 
-        with open(path, "wb") as f:
-            f.write(crypter.encrypt(image_bytes))
+        if isinstance(dst, str):
+            with open(dst, "wb") as f:
+                f.write(crypter.encrypt(image_bytes))
+        else:
+            dst.write(crypter.encrypt(image_bytes))
     elif backend == _IMAGE_BACKENDS.PIL:
         from PIL import Image
 
+        if ext.startswith("."):
+            ext = ext[1:]
+
         if not crypter.is_null_crypter:
             raise DatumaroError("PIL backend should have crypter=NullCrypter.")
 
         params = {}
         params["quality"] = kwargs.get("jpeg_quality")
         if kwargs.get("jpeg_quality") == 100:
             params["subsampling"] = 0
 
         image = image.astype(dtype)
         if len(image.shape) == 3 and image.shape[2] in {3, 4}:
             image[:, :, :3] = image[:, :, 2::-1]  # BGR to RGB
         image = Image.fromarray(image)
-        image.save(path, **params)
+        image.save(dst, format=ext, **params)
     else:
         raise NotImplementedError()
 
 
 def encode_image(image: np.ndarray, ext: str, dtype: DTypeLike = np.uint8, **kwargs) -> bytes:
     if not kwargs:
         kwargs = {}
@@ -172,15 +191,15 @@
         import cv2
 
         params = []
 
         if not ext.startswith("."):
             ext = "." + ext
 
-        if ext.upper() == ".JPG":
+        if ext.upper() in (".JPG", ".JPEG"):
             params = [int(cv2.IMWRITE_JPEG_QUALITY), kwargs.get("jpeg_quality", 75)]
 
         image = image.astype(dtype)
         success, result = cv2.imencode(ext, image, params=params)
         if not success:
             raise Exception("Failed to encode image to '%s' format" % (ext))
         return result.tobytes()
```

### Comparing `datumaro-1.1.1/datumaro/util/image_cache.py` & `datumaro-1.2.0rc1/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/log_utils.py` & `datumaro-1.2.0rc1/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/mask_tools.py` & `datumaro-1.2.0rc1/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/meta_file_util.py` & `datumaro-1.2.0rc1/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/os_util.py` & `datumaro-1.2.0rc1/datumaro/util/os_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,36 @@
 
 try:
     # Declare functions to remove files and directories.
     #
     # Use rmtree from GitPython to avoid the problem with removal of
     # readonly files on Windows, which Git uses extensively
     # It double checks if a file cannot be removed because of readonly flag
-    from git.util import rmfile, rmtree  # pylint: disable=unused-import
+    from git.util import rmfile, rmtree  # noqa: F401
 except ModuleNotFoundError:
-    from os import remove as rmfile  # pylint: disable=unused-import
-    from shutil import rmtree as rmtree  # pylint: disable=unused-import
+    from os import remove as rmfile  # noqa: F401
+    from shutil import rmtree as rmtree  # noqa: F401
 
 from . import cast
 from .definitions import DEFAULT_SUBSET_NAME
 
 DEFAULT_MAX_DEPTH = 10
 DEFAULT_MIN_DEPTH = 0
 
 
 def check_instruction_set(instruction):
     return instruction == str.strip(
         # Let's ignore a warning from bandit about using shell=True.
         # In this case it isn't a security issue and we use some
         # shell features like pipes.
-        subprocess.check_output(  # nosec B602
+        subprocess.check_output(
             'lscpu | grep -o "%s" | head -1' % instruction, shell=True
-        ).decode("utf-8")
+        ).decode(  # nosec B602
+            "utf-8"
+        )
     )
 
 
 def import_foreign_module(name, path):
     module = None
     default_path = sys.path.copy()
     try:
```

### Comparing `datumaro-1.1.1/datumaro/util/pickle_util.py` & `datumaro-1.2.0rc1/datumaro/util/pickle_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import pickle  # nosec - disable B403:import_pickle check - fixed
+import pickle  # nosec import_pickle
 
 import numpy.core.multiarray
 
 
 class RestrictedUnpickler(pickle.Unpickler):
     def find_class(self, module, name):
         if module == "numpy.core.multiarray" and name in PickleLoader.safe_numpy:
```

### Comparing `datumaro-1.1.1/datumaro/util/scope.py` & `datumaro-1.2.0rc1/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/telemetry_stub.py` & `datumaro-1.2.0rc1/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro/util/telemetry_utils.py` & `datumaro-1.2.0rc1/datumaro/util/telemetry_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,65 +18,66 @@
 except ImportError:
     tm = telemetry_stub
 
 NO_TELEMETRY_KEY = "DATUMARO_NO_OV_TELEMETRY"
 
 
 def _get_action_name(command):
-    if command is contexts.project.info_command:
+    # TODO: We should clean these nonsense if-else branches.
+    if command is commands.require_project.versioning.info.info_command:
         return "project_info_result"
-    elif command is contexts.project.stats_command:
+    elif command is commands.require_project.dataset_operations.stats.stats_command:
         return "project_stats_result"
     elif command is contexts.project.migrate_command:
         return "project_migrate_result"
-    elif command is contexts.project.export_command:
+    elif command is commands.require_project.dataset_operations.export.export_command:
         return "project_export_result"
-    elif command is commands.validate.validate_command:
+    elif command is commands.require_project.dataset_operations.validate.validate_command:
         return "project_validate_result"
     elif command is commands.filter.filter_command:
         return "project_filter_result"
-    elif command is commands.transform.transform_command:
+    elif command is commands.require_project.dataset_operations.transform.transform_command:
         return "project_transform_result"
-    elif command is contexts.source.import_command:
+    elif command is commands.require_project.modification.import_.import_command:
         return "source_add_result"
-    elif command is contexts.source.remove_command:
+    elif command is commands.require_project.modification.remove.remove_command:
         return "source_remove_result"
     elif command is contexts.source.info_command:
         return "source_info_result"
     elif command is contexts.model.add_command:
         return "model_add_result"
     elif command is contexts.model.remove_command:
         return "model_remove_result"
     elif command is contexts.model.run_command:
         return "model_run_result"
     elif command is contexts.model.info_command:
         return "model_info_result"
-    elif command is commands.checkout.checkout_command:
+    elif command is commands.require_project.versioning.checkout.checkout_command:
         return "checkout_result"
-    elif command is commands.commit.commit_command:
+    elif command is commands.require_project.versioning.commit.commit_command:
         return "commit_result"
     elif command is commands.convert.convert_command:
         return "convert_result"
-    elif command is commands.create.create_command:
+    elif command is commands.require_project.modification.create.create_command:
         return "create_result"
-    elif command is commands.diff.diff_command:
+    elif command is commands.require_project.dataset_operations.diff.diff_command:
         return "diff_result"
     elif command is commands.explain.explain_command:
         return "explain_result"
     elif command is commands.generate.generate_command:
         return "generate_result"
-    elif command is commands.info.info_command:
+    elif command is commands.require_project.dataset_operations.info.info_command:
         return "info_result"
-    elif command is commands.log.log_command:
+    elif command is commands.require_project.versioning.log.log_command:
         return "log_result"
     elif command is commands.merge.merge_command:
         return "merge_result"
     elif command is commands.patch.patch_command:
         return "patch_result"
-    elif command is commands.status.status_command:
+    elif command is commands.require_project.versioning.status.status_command:
         return "status_result"
 
     return f"{command.__name__}_result"
 
 
 ARG_USED_FLAG = "True"
```

### Comparing `datumaro-1.1.1/datumaro/util/tf_util.py` & `datumaro-1.2.0rc1/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.1.1/datumaro.egg-info/PKG-INFO` & `datumaro-1.2.0rc1/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.1.1
+Version: 1.2.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.1.1/datumaro.egg-info/SOURCES.txt` & `datumaro-1.2.0rc1/datumaro.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,45 +19,49 @@
 datumaro.egg-info/entry_points.txt
 datumaro.egg-info/requires.txt
 datumaro.egg-info/top_level.txt
 datumaro/capi/pybind.cpp
 datumaro/cli/__init__.py
 datumaro/cli/__main__.py
 datumaro/cli/commands/__init__.py
-datumaro/cli/commands/add.py
-datumaro/cli/commands/checkout.py
-datumaro/cli/commands/commit.py
 datumaro/cli/commands/convert.py
-datumaro/cli/commands/create.py
-datumaro/cli/commands/describe_downloads.py
 datumaro/cli/commands/detect_format.py
-datumaro/cli/commands/diff.py
 datumaro/cli/commands/download.py
 datumaro/cli/commands/explain.py
-datumaro/cli/commands/export.py
 datumaro/cli/commands/filter.py
 datumaro/cli/commands/generate.py
-datumaro/cli/commands/import_.py
-datumaro/cli/commands/info.py
-datumaro/cli/commands/log.py
 datumaro/cli/commands/merge.py
 datumaro/cli/commands/patch.py
-datumaro/cli/commands/remove.py
 datumaro/cli/commands/search.py
-datumaro/cli/commands/stats.py
-datumaro/cli/commands/status.py
-datumaro/cli/commands/transform.py
-datumaro/cli/commands/validate.py
+datumaro/cli/commands/require_project/__init__.py
+datumaro/cli/commands/require_project/dataset_operations/__init__.py
+datumaro/cli/commands/require_project/dataset_operations/diff.py
+datumaro/cli/commands/require_project/dataset_operations/export.py
+datumaro/cli/commands/require_project/dataset_operations/info.py
+datumaro/cli/commands/require_project/dataset_operations/stats.py
+datumaro/cli/commands/require_project/dataset_operations/transform.py
+datumaro/cli/commands/require_project/dataset_operations/validate.py
+datumaro/cli/commands/require_project/modification/__init__.py
+datumaro/cli/commands/require_project/modification/add.py
+datumaro/cli/commands/require_project/modification/create.py
+datumaro/cli/commands/require_project/modification/import_.py
+datumaro/cli/commands/require_project/modification/remove.py
+datumaro/cli/commands/require_project/versioning/__init__.py
+datumaro/cli/commands/require_project/versioning/checkout.py
+datumaro/cli/commands/require_project/versioning/commit.py
+datumaro/cli/commands/require_project/versioning/info.py
+datumaro/cli/commands/require_project/versioning/log.py
+datumaro/cli/commands/require_project/versioning/status.py
 datumaro/cli/contexts/__init__.py
 datumaro/cli/contexts/model.py
 datumaro/cli/contexts/source.py
 datumaro/cli/contexts/util.py
 datumaro/cli/contexts/project/__init__.py
-datumaro/cli/contexts/project/diff.py
 datumaro/cli/util/__init__.py
+datumaro/cli/util/diff.py
 datumaro/cli/util/errors.py
 datumaro/cli/util/project.py
 datumaro/components/__init__.py
 datumaro/components/annotation.py
 datumaro/components/cli_plugin.py
 datumaro/components/config.py
 datumaro/components/config_model.py
@@ -67,39 +71,51 @@
 datumaro/components/environment.py
 datumaro/components/errors.py
 datumaro/components/exporter.py
 datumaro/components/extractor_tfds.py
 datumaro/components/filter.py
 datumaro/components/format_detection.py
 datumaro/components/generator.py
-datumaro/components/hl_ops.py
 datumaro/components/importer.py
 datumaro/components/launcher.py
 datumaro/components/media.py
 datumaro/components/media_manager.py
-datumaro/components/merger.py
 datumaro/components/operations.py
 datumaro/components/progress_reporting.py
 datumaro/components/project.py
 datumaro/components/searcher.py
 datumaro/components/shift_analyzer.py
 datumaro/components/transformer.py
 datumaro/components/validator.py
 datumaro/components/visualizer.py
 datumaro/components/algorithms/__init__.py
 datumaro/components/algorithms/rise.py
+datumaro/components/algorithms/noisy_label_detection/__init__.py
+datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+datumaro/components/annotations/__init__.py
+datumaro/components/annotations/matcher.py
+datumaro/components/annotations/merger.py
+datumaro/components/hl_ops/__init__.py
+datumaro/components/merge/__init__.py
+datumaro/components/merge/base.py
+datumaro/components/merge/exact_merge.py
+datumaro/components/merge/intersect_merge.py
+datumaro/components/merge/union_merge.py
 datumaro/plugins/__init__.py
 datumaro/plugins/ndr.py
 datumaro/plugins/searcher.py
 datumaro/plugins/shift_analyzer.py
 datumaro/plugins/splitter.py
 datumaro/plugins/transforms.py
 datumaro/plugins/validators.py
 datumaro/plugins/accuracy_checker_plugin/__init__.py
 datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+datumaro/plugins/accuracy_checker_plugin/details/ac.py
+datumaro/plugins/accuracy_checker_plugin/details/representation.py
 datumaro/plugins/data_formats/__init__.py
 datumaro/plugins/data_formats/ade20k2017.py
 datumaro/plugins/data_formats/ade20k2020.py
 datumaro/plugins/data_formats/brats.py
 datumaro/plugins/data_formats/brats_numpy.py
 datumaro/plugins/data_formats/camvid.py
 datumaro/plugins/data_formats/cifar.py
@@ -123,14 +139,20 @@
 datumaro/plugins/data_formats/open_images.py
 datumaro/plugins/data_formats/synthia.py
 datumaro/plugins/data_formats/vgg_face2.py
 datumaro/plugins/data_formats/video.py
 datumaro/plugins/data_formats/vott_csv.py
 datumaro/plugins/data_formats/vott_json.py
 datumaro/plugins/data_formats/widerface.py
+datumaro/plugins/data_formats/arrow/__init__.py
+datumaro/plugins/data_formats/arrow/arrow_dataset.py
+datumaro/plugins/data_formats/arrow/base.py
+datumaro/plugins/data_formats/arrow/exporter.py
+datumaro/plugins/data_formats/arrow/format.py
+datumaro/plugins/data_formats/arrow/importer.py
 datumaro/plugins/data_formats/ava/__init__.py
 datumaro/plugins/data_formats/ava/ava.py
 datumaro/plugins/data_formats/ava/ava_label_pb2.py
 datumaro/plugins/data_formats/celeba/__init__.py
 datumaro/plugins/data_formats/celeba/align_celeba.py
 datumaro/plugins/data_formats/celeba/celeba.py
 datumaro/plugins/data_formats/coco/__init__.py
@@ -148,15 +170,14 @@
 datumaro/plugins/data_formats/datumaro/format.py
 datumaro/plugins/data_formats/datumaro/importer.py
 datumaro/plugins/data_formats/datumaro_binary/__init__.py
 datumaro/plugins/data_formats/datumaro_binary/base.py
 datumaro/plugins/data_formats/datumaro_binary/exporter.py
 datumaro/plugins/data_formats/datumaro_binary/format.py
 datumaro/plugins/data_formats/datumaro_binary/importer.py
-datumaro/plugins/data_formats/datumaro_binary/mapper.py
 datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
 datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
 datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
 datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
 datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
 datumaro/plugins/data_formats/icdar/__init__.py
 datumaro/plugins/data_formats/icdar/base.py
@@ -215,14 +236,15 @@
 datumaro/plugins/tiling/merge_tile.py
 datumaro/plugins/tiling/tile.py
 datumaro/plugins/tiling/util.py
 datumaro/util/__init__.py
 datumaro/util/annotation_util.py
 datumaro/util/attrs_util.py
 datumaro/util/definitions.py
+datumaro/util/file_utils.py
 datumaro/util/image.py
 datumaro/util/image_cache.py
 datumaro/util/log_utils.py
 datumaro/util/mask_tools.py
 datumaro/util/meta_file_util.py
 datumaro/util/os_util.py
 datumaro/util/pickle_util.py
```

### Comparing `datumaro-1.1.1/datumaro.egg-info/requires.txt` & `datumaro-1.2.0rc1/datumaro.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 scipy
 requests
 pandas>=1.1.5
 openvino==2022.3.0
 tokenizers
 cryptography>=38.03
 pyemd
+pyarrow
 opencv-python
 
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
@@ -40,11 +41,11 @@
 [tf]
 tensorflow
 
 [tf-gpu]
 tensorflow-gpu
 
 [tfds]
-tensorflow-datasets!=4.5.0,!=4.5.1
+tensorflow-datasets<4.9.0
 
 [tfds-dev]
-tensorflow-datasets[dev]!=4.5.0,!=4.5.1
+tensorflow-datasets[dev]<4.9.0
```

### Comparing `datumaro-1.1.1/requirements-core.txt` & `datumaro-1.2.0rc1/requirements-core.txt`

 * *Files 13% similar despite different names*

```diff
@@ -37,7 +37,10 @@
 tokenizers
 
 # Encryption
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
+
+# apache arrow
+pyarrow
```

### Comparing `datumaro-1.1.1/setup.py` & `datumaro-1.2.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+# ruff: noqa: E501
+
 import os
 import os.path as osp
 import re
 from distutils.util import strtobool
 
 import setuptools
 from pybind11.setup_helpers import Pybind11Extension, build_ext
@@ -22,15 +24,15 @@
 
     with open(file_path, "r") as version_file:
         version_text = version_file.read()
 
     # PEP440:
     # https://www.python.org/dev/peps/pep-0440/#appendix-b-parsing-version-strings-with-regular-expressions
     pep_regex = r"([1-9]\d*!)?(0|[1-9]\d*)(\.(0|[1-9]\d*))*((a|b|rc)(0|[1-9]\d*))?(\.post(0|[1-9]\d*))?(\.dev(0|[1-9]\d*))?"
-    version_regex = r"VERSION\s*=\s*.(" + pep_regex + ")."
+    version_regex = r"__version__\s*=\s*.(" + pep_regex + ")."
     match = re.match(version_regex, version_text)
     if not match:
         raise RuntimeError("Failed to find version string in '%s'" % file_path)
 
     version = version_text[match.start(1) : match.end(1)]
     return version
 
@@ -80,19 +82,19 @@
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
         "tfds": [
-            "tensorflow-datasets!=4.5.0,!=4.5.1"
-        ],  # 4.5.0 fails on Windows, https://github.com/tensorflow/datasets/issues/3709
+            "tensorflow-datasets<4.9.0"
+        ],  # 4.9.0 fails on Windows and MacOS, https://github.com/openvinotoolkit/datumaro/actions/runs/4618774184
         "tfds-dev": [
-            "tensorflow-datasets[dev]!=4.5.0,!=4.5.1"
-        ],  # 4.5.0 fails on Windows, https://github.com/tensorflow/datasets/issues/3709
+            "tensorflow-datasets[dev]<4.9.0"
+        ],  # 4.9.0 fails on Windows and MacOS, https://github.com/openvinotoolkit/datumaro/actions/runs/4618774184
         "tf-gpu": ["tensorflow-gpu"],
         "default": DEFAULT_REQUIREMENTS,
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
             "datum=datumaro.cli.__main__:main",
```

