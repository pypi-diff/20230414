# Comparing `tmp/tensorflow_model_analysis-0.9.1.tar.gz` & `tmp/tensorflow_model_analysis-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorflow_model_analysis-0.9.1.tar", last modified: Mon Aug 27 22:28:49 2018, max compression
+gzip compressed data, was "dist/tensorflow_model_analysis-0.9.2.tar", last modified: Tue Sep 11 22:02:03 2018, max compression
```

## Comparing `tensorflow_model_analysis-0.9.1.tar` & `tensorflow_model_analysis-0.9.2.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)        1 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/namespace_packages.txt
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1163 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/PKG-INFO
--rw-r--r--   0 paulyang (56870) primarygroup (89939)       26 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/top_level.txt
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     5135 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 paulyang (56870) primarygroup (89939)        1 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/not-zip-safe
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      162 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/requires.txt
--rw-r--r--   0 paulyang (56870) primarygroup (89939)        1 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1163 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/PKG-INFO
--rw-r--r--   0 paulyang (56870) primarygroup (89939)       38 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/setup.cfg
--rw-r--r--   0 paulyang (56870) primarygroup (89939)       28 2018-08-27 22:28:24.000000 tensorflow_model_analysis-0.9.1/MANIFEST.in
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     9201 2018-08-27 22:28:33.000000 tensorflow_model_analysis-0.9.1/setup.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2890 2018-08-27 22:28:24.000000 tensorflow_model_analysis-0.9.1/README.md
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      937 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/visualization.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1716 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/renderer.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/__init__.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/tfma_widget/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2320 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/tfma_widget/widget.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      734 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/tfma_widget/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/__init__.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/colab/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2601 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/colab/renderer.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:35.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/colab/__init__.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4519 2018-08-27 22:28:36.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/model_eval_lib_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:36.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2048 2018-08-27 22:28:36.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/model_eval_lib.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1949 2018-08-27 22:28:36.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/util.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    13173 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/tfma_unit.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    10054 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/model_eval_lib_test.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    10511 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/serialization.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2261 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/api_types.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    12145 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/evaluate_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    13022 2018-08-27 22:28:37.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/serialization_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:38.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    16992 2018-08-27 22:28:38.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/evaluate.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     7303 2018-08-27 22:28:38.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/tfma_unit_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:38.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    14220 2018-08-27 22:28:38.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/model_eval_lib.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3639 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/types.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1678 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/types_compat.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      994 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/constants.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      754 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/version.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3950 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/feature_extractor_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3702 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/predict_extractor.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3327 2018-08-27 22:28:39.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/predict_extractor_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:40.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4371 2018-08-27 22:28:40.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/feature_extractor.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     1479 2018-08-27 22:28:40.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/__init__.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4642 2018-08-27 22:28:40.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/testutil.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     5382 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/encoding.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    14446 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/util.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2952 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/encoding_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     7971 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/graph_ref.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    26531 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/integration_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      838 2018-08-27 22:28:41.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/constants.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    11483 2018-08-27 22:28:42.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metrics.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    32952 2018-08-27 22:28:42.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:42.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    40932 2018-08-27 22:28:43.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2170 2018-08-27 22:28:43.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metric_keys.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     9429 2018-08-27 22:28:43.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/util_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     6918 2018-08-27 22:28:43.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/graph_ref_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:43.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    19237 2018-08-27 22:28:44.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/load.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     6222 2018-08-27 22:28:44.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/exporter.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     7948 2018-08-27 22:28:44.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/export.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3589 2018-08-27 22:28:44.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/dofn.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4471 2018-08-27 22:28:44.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/multi_head.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     6277 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/util.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3737 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator_extra_fields.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2153 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_classifier.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2372 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4757 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier_extra_fields.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3399 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4155 2018-08-27 22:28:45.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4083 2018-08-27 22:28:46.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/custom_estimator.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2628 2018-08-27 22:28:46.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier_multivalent.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:46.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    10485 2018-08-27 22:28:46.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fake_sequence_to_prediction.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2370 2018-08-27 22:28:46.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_regressor.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2151 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_regressor.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3440 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/csv_linear_classifier.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     4189 2018-08-27 22:28:24.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/extension.js
--rw-r--r--   0 paulyang (56870) primarygroup (89939)   812483 2018-08-27 22:28:26.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/vulcanized_template.html
--rw-r--r--   0 paulyang (56870) primarygroup (89939)   677995 2018-08-27 22:28:24.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/index.js.map
--rw-r--r--   0 paulyang (56870) primarygroup (89939)   551156 2018-08-27 22:28:24.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/index.js
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/proto/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/proto/__init__.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)    10121 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slicer.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      575 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/__init__.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2389 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slice_accessor_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     9876 2018-08-27 22:28:47.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slicer_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     2532 2018-08-27 22:28:48.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slice_accessor.py
-drwxr-xr-x   0 paulyang (56870) primarygroup (89939)        0 2018-08-27 22:28:49.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     7602 2018-08-27 22:28:48.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/util.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     3145 2018-08-27 22:28:48.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/widget_view.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)     9812 2018-08-27 22:28:48.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/util_test.py
--rw-r--r--   0 paulyang (56870) primarygroup (89939)      839 2018-08-27 22:28:48.000000 tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/__init__.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)       28 2018-09-11 22:01:52.000000 tensorflow_model_analysis-0.9.2/MANIFEST.in
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     9201 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/setup.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)       38 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/setup.cfg
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     9876 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slicer_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2389 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slice_accessor_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    10121 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slicer.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2532 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slice_accessor.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    32952 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    40932 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    11483 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metrics.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2170 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metric_keys.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     9429 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/util_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     5382 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/encoding.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      838 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/constants.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     7971 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/graph_ref.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2952 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/encoding_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3589 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/dofn.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     6222 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/exporter.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    26531 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/integration_test.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4155 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4757 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier_extra_fields.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2151 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_regressor.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4471 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/multi_head.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3440 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/csv_linear_classifier.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4083 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/custom_estimator.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3399 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2628 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier_multivalent.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3737 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator_extra_fields.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2370 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_regressor.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     6277 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/util.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2153 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_classifier.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    10485 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fake_sequence_to_prediction.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2372 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4642 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/testutil.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    14446 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/util.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     6918 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/graph_ref_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     7948 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/export.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    19237 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/load.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3799 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/types.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/tfma_widget/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2320 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/tfma_widget/widget.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      734 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/tfma_widget/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1716 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/renderer.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      937 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/visualization.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/__init__.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/colab/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2601 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/colab/renderer.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/colab/__init__.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4189 2018-09-11 22:01:52.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/extension.js
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)   812483 2018-09-11 22:01:53.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/vulcanized_template.html
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)   551155 2018-09-11 22:01:52.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/index.js
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)   677995 2018-09-11 22:01:52.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/index.js.map
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      994 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/constants.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2048 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/model_eval_lib.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4519 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/model_eval_lib_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/__init__.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4688 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/predict_extractor.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3473 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/predict_extractor_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3950 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/feature_extractor_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     4371 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/feature_extractor.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      754 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/version.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1678 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/types_compat.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/proto/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/proto/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1479 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/__init__.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     9812 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/util_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3145 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/widget_view.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      839 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     7602 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/util.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1949 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/util.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    14219 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/model_eval_lib.py
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    12145 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/evaluate_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2682 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/slice.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3872 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/slice_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     2261 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/api_types.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    10511 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/serialization.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    13022 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/serialization_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    17234 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/evaluate.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    13173 2018-09-11 22:01:55.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/tfma_unit.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     7303 2018-09-11 22:01:57.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/tfma_unit_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)    10054 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/model_eval_lib_test.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      575 2018-09-11 22:01:56.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/__init__.py
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1129 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/PKG-INFO
+drwxr-xr-x   0 xinzha   (332398) primarygroup (89939)        0 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     5228 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)        1 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/not-zip-safe
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)      162 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/requires.txt
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     1129 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)        1 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/namespace_packages.txt
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)       26 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/top_level.txt
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)        1 2018-09-11 22:02:03.000000 tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 xinzha   (332398) primarygroup (89939)     3092 2018-09-11 22:01:52.000000 tensorflow_model_analysis-0.9.2/README.md
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/PKG-INFO` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.2
 Name: tensorflow-model-analysis
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library for analyzing TensorFlow models
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: tensorflow-extended-dev@googlegroups.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis.egg-info/SOURCES.txt` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 tensorflow_model_analysis/api/tfma_unit_test.py
 tensorflow_model_analysis/api/impl/__init__.py
 tensorflow_model_analysis/api/impl/api_types.py
 tensorflow_model_analysis/api/impl/evaluate.py
 tensorflow_model_analysis/api/impl/evaluate_test.py
 tensorflow_model_analysis/api/impl/serialization.py
 tensorflow_model_analysis/api/impl/serialization_test.py
+tensorflow_model_analysis/api/impl/slice.py
+tensorflow_model_analysis/api/impl/slice_test.py
 tensorflow_model_analysis/contrib/__init__.py
 tensorflow_model_analysis/contrib/model_eval_lib.py
 tensorflow_model_analysis/contrib/model_eval_lib_test.py
 tensorflow_model_analysis/eval_saved_model/__init__.py
 tensorflow_model_analysis/eval_saved_model/constants.py
 tensorflow_model_analysis/eval_saved_model/dofn.py
 tensorflow_model_analysis/eval_saved_model/encoding.py
```

### Comparing `tensorflow_model_analysis-0.9.1/PKG-INFO` & `tensorflow_model_analysis-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.2
 Name: tensorflow_model_analysis
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library for analyzing TensorFlow models
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: tensorflow-extended-dev@googlegroups.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tensorflow_model_analysis-0.9.1/setup.py` & `tensorflow_model_analysis-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         'numpy>=1.10,<2',
         'jupyter>=1.0,<2',
         'ipywidgets>=7.0,<8',
         # TF now requires protobuf>=3.6.0.
         'protobuf>=3.6.0,<4',
         # For apitools.
         'six>=1.9,<2',
-        'tensorflow-transform>=0.8,<1',
+        'tensorflow-transform>=0.9,<1',
     ],
     'python_requires':
         '>=2.7,<3',
     'packages':
         find_packages(),
     'zip_safe':
         False,
```

### Comparing `tensorflow_model_analysis-0.9.1/README.md` & `tensorflow_model_analysis-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- See: www.tensorflow.org/tfx/model_analysis/ -->
 
-# TensorFlow Model Analysis
+# TensorFlow Model Analysis [![PyPI](https://img.shields.io/pypi/pyversions/tensorflow-model-analysis.svg?style=plastic)](https://github.com/tensorflow/model-analysis)
 
 *TensorFlow Model Analysis* (TFMA) is a library for evaluating TensorFlow models.
 It allows users to evaluate their models on large amounts of data in a
 distributed manner, using the same metrics defined in their trainer. These
 metrics can be computed over different slices of data and visualized in Jupyter
 notebooks.
 
@@ -54,15 +54,16 @@
 The following table is the TFMA package versions that are compatible with each
 other. This is determined by our testing framework, but other *untested*
 combinations may also work.
 
 |tensorflow-model-analysis  |tensorflow    |apache-beam[gcp]|
 |---------------------------|--------------|----------------|
 |GitHub master              |1.9           |2.6.0           |
-|0.9.1                      |1.9           |2.6.0           |
+|0.9.2                      |1.9           |2.6.0           |
+|0.9.1                      |1.10          |2.6.0           |
 |0.9.0                      |1.9           |2.5.0           |
 |0.6.0                      |1.6           |2.4.0           |
 
 ## Questions
 
 Please direct any questions about working with TFMA to
 [Stack Overflow](https://stackoverflow.com) using the
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/visualization.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/visualization.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/renderer.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/renderer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/tfma_widget/widget.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/tfma_widget/widget.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/jupyter/tfma_widget/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/tfma_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/colab/renderer.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/colab/renderer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/notebook/colab/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/model_eval_lib_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/model_eval_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/contrib/model_eval_lib.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/contrib/model_eval_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/util.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/util.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/tfma_unit.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/tfma_unit.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/model_eval_lib_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/model_eval_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/serialization.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/serialization.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/api_types.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/api_types.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/evaluate_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/evaluate_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/serialization_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/serialization_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/impl/evaluate.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from __future__ import print_function
 
 
 
 
 import apache_beam as beam
 
-from tensorflow_model_analysis import constants
 from tensorflow_model_analysis import types
+from tensorflow_model_analysis.api.impl import slice as slice_api
 from tensorflow_model_analysis.eval_saved_model import dofn
 from tensorflow_model_analysis.eval_saved_model import load
 from tensorflow_model_analysis.eval_saved_model.post_export_metrics import metric_keys
 from tensorflow_model_analysis.extractors import feature_extractor
 from tensorflow_model_analysis.extractors import predict_extractor
 from tensorflow_model_analysis.slicer import slicer
 from tensorflow_transform.beam import shared
@@ -40,50 +40,14 @@
 # in Beam type annotations is not complete.
 _BeamSliceKeyType = beam.typehints.Tuple[  # pylint: disable=invalid-name
     beam.typehints.Tuple[bytes, beam.typehints.Union[bytes, int, float]], Ellipsis]
 
 _METRICS_NAMESPACE = 'tensorflow_model_analysis'
 
 
-@beam.typehints.with_input_types(beam.typehints.Any)
-@beam.typehints.with_output_types(
-    beam.typehints.Tuple[_BeamSliceKeyType, beam.typehints.Any])
-class _SliceDoFn(beam.DoFn):
-  """A DoFn that performs slicing."""
-
-  def __init__(self, slice_spec):
-    self._slice_spec = slice_spec
-    self._num_slices_generated_per_instance = beam.metrics.Metrics.distribution(
-        _METRICS_NAMESPACE, 'num_slices_generated_per_instance')
-    self._post_slice_num_instances = beam.metrics.Metrics.counter(
-        _METRICS_NAMESPACE, 'post_slice_num_instances')
-
-  def process(self, element):
-    features = element.features
-    slice_count = 0
-    for slice_key in slicer.get_slices_for_features_dict(
-        features, self._slice_spec):
-      slice_count += 1
-      yield (slice_key, element)
-
-    self._num_slices_generated_per_instance.update(slice_count)
-    self._post_slice_num_instances.inc(slice_count)
-
-
-@beam.ptransform_fn
-@beam.typehints.with_input_types(
-    beam.typehints.Tuple[types.DictOfTensorType, beam.typehints.Any]
-)
-@beam.typehints.with_output_types(
-    beam.typehints.Tuple[_BeamSliceKeyType, beam.typehints.Any])  # pylint: disable=invalid-name
-def _Slice(intro_result,
-           slice_spec):
-  return intro_result | beam.ParDo(_SliceDoFn(slice_spec))
-
-
 def _add_metric_variables(  # pylint: disable=invalid-name
     left,
     right):
   if left is not None and right is not None:
     if len(left) != len(right):
       raise ValueError('metric variables lengths should match, but got '
                        '%d and %d' % (len(left), len(right)))
@@ -153,15 +117,15 @@
   and accumulate FeaturesPredictionsLabels accordingly. We do one final
   "intro metrics" and merge step before producing the final output value.
 
   See also:
   BEAM-3737: Key-aware batching function.
   """
 
-  _DEFAULT_BATCH_SIZE = 1000
+  _DEFAULT_DESIRED_BATCH_SIZE = 1000
 
   def __init__(self,
                eval_saved_model_path,
                add_metrics_callbacks,
                shared_handle,
                desired_batch_size = None):
     self._eval_saved_model_path = eval_saved_model_path
@@ -174,15 +138,15 @@
         _METRICS_NAMESPACE, 'combine_batch_size')
 
     # We really want the batch size to be adaptive like it is in
     # beam.BatchElements(), but there isn't an easy way to make it so.
     if desired_batch_size > 0:
       self._desired_batch_size = desired_batch_size
     else:
-      self._desired_batch_size = self._DEFAULT_BATCH_SIZE
+      self._desired_batch_size = self._DEFAULT_DESIRED_BATCH_SIZE
 
   def _start_bundle(self):
     # There's no initialisation method for CombineFns.
     # See BEAM-3736: Add SetUp() and TearDown() for CombineFns.
     self._eval_saved_model = self._shared_handle.acquire(
         dofn.make_construct_fn(self._eval_saved_model_path,
                                self._add_metrics_callbacks,
@@ -196,32 +160,33 @@
     intro metrics for the batch and updates accumulator in place.
 
     Args:
       accumulator: Accumulator. Will be updated in place.
       force: Force intro metrics even if accumulator has less FPLs than the
         batch size.
     """
+    # Note that we're mutating the accumulator in-place. Beam guarantees that
+    # this is safe.
+
     if self._eval_saved_model is None:
       self._start_bundle()
     batch_size = len(accumulator.fpls)
     if force or batch_size >= self._desired_batch_size:
-      self._combine_batch_size.update(batch_size)
-      if accumulator.fpls:  # Might be empty if force is True
+      if accumulator.fpls:
+        self._combine_batch_size.update(batch_size)
         accumulator.add_metrics_variables(
             self._eval_saved_model.metrics_reset_update_get_list(
                 accumulator.fpls))
-      accumulator.fpls = []
+        del accumulator.fpls[:]
 
   def create_accumulator(self):
     return _AggState()
 
   def add_input(self, accumulator,
                 elem):
-    # Note that we're mutating the accumulator in-place. Beam guarantees that
-    # this is safe.
     accumulator.add_fpl(elem)
     self._maybe_do_batch(accumulator)
     return accumulator
 
   def merge_accumulators(self, accumulators):
     result = _AggState()
     for acc in accumulators:
@@ -231,42 +196,49 @@
       # During the "map" side of combining combining happens per bundle,
       # but on the "reduce" side it's across all bundles (for a given key).
       #
       # So we could potentially accumulate get num_bundles * batch_size
       # elements if we don't process the batches within the loop, which
       # could cause OOM errors (b/77293756).
       self._maybe_do_batch(result)
+
+    # Ensure (via 'force=True') that all "merged" accumulators that are produced
+    # are compact and "fully" merged (ie ready for use for extract_output). Any
+    # overhead that might be induced by this due to possibly small batches is
+    # likely dwarfed by the overhead that materializing large accumulators
+    # induces.
+    self._maybe_do_batch(result, force=True)
+
     return result
 
   def extract_output(self,
                      accumulator):
-    # Note that we're mutating the accumulator in-place. Beam guarantees that
-    # this is safe.
-    self._maybe_do_batch(accumulator, force=True)
     return accumulator.metric_variables
 
 
 @beam.ptransform_fn
 @beam.typehints.with_input_types(
     beam.typehints.Tuple[_BeamSliceKeyType, beam.typehints.Any])
 @beam.typehints.with_output_types(beam.typehints.Tuple[
     _BeamSliceKeyType, beam.typehints.List[beam.typehints.Any]])
 def _Aggregate(  # pylint: disable=invalid-name
     slice_result,
     eval_saved_model_path,
     add_metrics_callbacks,
+    shared_handle,
     desired_batch_size = None,
 ):
+  """PTransform for computing, aggregating and combining metrics."""
   return (
       slice_result
-      | 'CombinePerKey' >> beam.CombinePerKey(
+      | 'CombinePerSlice' >> beam.CombinePerKey(
           _AggregateCombineFn(
               eval_saved_model_path=eval_saved_model_path,
               add_metrics_callbacks=add_metrics_callbacks,
-              shared_handle=shared.Shared(),
+              shared_handle=shared_handle,
               desired_batch_size=desired_batch_size))
   )
 
 
 @beam.typehints.with_input_types(beam.typehints.Tuple[
     _BeamSliceKeyType, beam.typehints.List[beam.typehints.Any]])
 # No typehint for output type, since it's a multi-output DoFn result that
@@ -297,47 +269,78 @@
 
 @beam.ptransform_fn
 @beam.typehints.with_input_types(beam.typehints.Tuple[
     _BeamSliceKeyType, beam.typehints.List[beam.typehints.Any]])
 # No typehint for output type, since it's a multi-output DoFn result that
 # Beam doesn't support typehints for yet (BEAM-3280).
 def _ExtractOutput(  # pylint: disable=invalid-name
-    aggregate_result, eval_saved_model_path,
-    add_metrics_callbacks
+    aggregate_result,
+    eval_saved_model_path,
+    add_metrics_callbacks,
+    shared_handle,
 ):
+  """PTransform for extracting metrics output."""
   return aggregate_result | beam.ParDo(
       _ExtractOutputDoFn(
           eval_saved_model_path=eval_saved_model_path,
           add_metrics_callbacks=add_metrics_callbacks,
-          shared_handle=shared.Shared())).with_outputs(
+          shared_handle=shared_handle)).with_outputs(
               _ExtractOutputDoFn.OUTPUT_TAG_PLOTS,
               main=_ExtractOutputDoFn.OUTPUT_TAG_METRICS)
 
 
+def PredictExtractor(eval_saved_model_path, add_metrics_callbacks,
+                     shared_handle, desired_batch_size):
+  # Map function which loads and runs the eval_saved_model against every
+  # example, yielding an types.ExampleAndExtracts containing a
+  # FeaturesPredictionsLabels value (where key is 'fpl').
+  return types.Extractor(
+      stage_name='Predict',
+      ptransform=predict_extractor.TFMAPredict(
+          eval_saved_model_path=eval_saved_model_path,
+          add_metrics_callbacks=add_metrics_callbacks,
+          shared_handle=shared_handle,
+          desired_batch_size=desired_batch_size))
+
+
+@beam.ptransform_fn
+def Extract(examples, extractors):
+  """Performs Extractions serially in provided order."""
+  augmented = examples
+
+  for extractor in extractors:
+    augmented = augmented | extractor.stage_name >> extractor.ptransform
+
+  return augmented
+
+
 @beam.ptransform_fn
 # No typehint for output type, since it's a multi-output DoFn result that
 # Beam doesn't support typehints for yet (BEAM-3280).
 def Evaluate(
     # pylint: disable=invalid-name
     examples,
     eval_saved_model_path,
+    extractors = None,
     add_metrics_callbacks = None,
     slice_spec = None,
     desired_batch_size = None,
 ):
   """Evaluate the given EvalSavedModel on the given examples.
 
   This is for TFMA use only. Users should call tfma.EvaluateAndWriteResults
   instead of this function.
 
   Args:
     examples: PCollection of input examples. Can be any format the model accepts
       (e.g. string containing CSV row, TensorFlow.Example, etc).
     eval_saved_model_path: Path to EvalSavedModel. This directory should contain
       the saved_model.pb file.
+    extractors: Optional list of Extractors to execute prior to slicing and
+      aggregating the metrics. If not provided, a default set will be run.
     add_metrics_callbacks: Optional list of callbacks for adding additional
       metrics to the graph. The names of the metrics added by the callbacks
       should not conflict with existing metrics, or metrics added by other
       callbacks. See below for more details about what each callback should do.
     slice_spec: Optional list of SingleSliceSpec specifying the slices to slice
       the data into. If None, defaults to the overall slice.
     desired_batch_size: Optional batch size for batching in Predict and
@@ -368,72 +371,83 @@
     DoOutputsTuple. The tuple entries are
     PCollection of (slice key, metrics) and
     PCollection of (slice key, plot metrics).
   """
   if slice_spec is None:
     slice_spec = [slicer.SingleSliceSpec()]
 
+  shared_handle = shared.Shared()
+
+  if not extractors:
+    extractors = [
+        PredictExtractor(eval_saved_model_path, add_metrics_callbacks,
+                         shared_handle, desired_batch_size),
+    ]
+
   # pylint: disable=no-value-for-parameter
   return (
       examples
       # Our diagnostic outputs, pass types.ExampleAndExtracts throughout,
       # however our aggregating functions do not use this interface.
-      | beam.Map(lambda x: types.ExampleAndExtracts(example=x, extracts={}))
-
-      # Map function which loads and runs the eval_saved_model against every
-      # example, yielding an types.ExampleAndExtracts containing a
-      # FeaturesPredictionsLabels value (where key is 'fpl').
-      | 'Predict' >> predict_extractor.TFMAPredict(
-          eval_saved_model_path=eval_saved_model_path,
-          desired_batch_size=desired_batch_size)
+      | 'ToExampleAndExtracts' >>
+      beam.Map(lambda x: types.ExampleAndExtracts(example=x, extracts={}))
+      | Extract(extractors=extractors)
 
-      # Unwrap the types.ExampleAndExtracts.
-      # The rest of this pipeline expects FeaturesPredictionsLabels
-      | beam.Map(lambda x:  # pylint: disable=g-long-lambda
-                 x.extracts[constants.FEATURES_PREDICTIONS_LABELS_KEY])
-
-      # Input: one example fpl at a time
+      # Input: one example at a time
       # Output: one fpl example per slice key (notice that the example turns
       #         into n, replicated once per applicable slice key)
-      | 'Slice' >> _Slice(slice_spec)
+      | 'Slice' >> slice_api.Slice(slice_spec)
 
       # Each slice key lands on one shard where metrics are computed for all
       # examples in that shard -- the "map" and "reduce" parts of the
       # computation happen within this shard.
       # Output: Tuple[slicer.SliceKeyType, MetricVariablesType]
       | 'Aggregate' >> _Aggregate(
           eval_saved_model_path=eval_saved_model_path,
           add_metrics_callbacks=add_metrics_callbacks,
+          shared_handle=shared_handle,
           desired_batch_size=desired_batch_size)
 
       # Different metrics for a given slice key are brought together.
-      | 'ExtractOutput' >> _ExtractOutput(eval_saved_model_path,
-                                          add_metrics_callbacks))
+      | 'ExtractOutput' >> _ExtractOutput(
+          eval_saved_model_path=eval_saved_model_path,
+          add_metrics_callbacks=add_metrics_callbacks,
+          shared_handle=shared_handle))
 
 
 @beam.ptransform_fn
 @beam.typehints.with_input_types(bytes)
 @beam.typehints.with_output_types(beam.typehints.Any)
 def BuildDiagnosticTable(
     # pylint: disable=invalid-name
     examples,
     eval_saved_model_path,
+    extractors = None,
     desired_batch_size = None):
   """Build diagnostics for the spacified EvalSavedModel and example collection.
 
   Args:
     examples: PCollection of input examples. Can be any format the model accepts
       (e.g. string containing CSV row, TensorFlow.Example, etc).
     eval_saved_model_path: Path to EvalSavedModel. This directory should contain
       the saved_model.pb file.
+    extractors: Optional list of Extractors to execute prior to slicing and
+      aggregating the metrics. If not provided, a default set will be run.
     desired_batch_size: Optional batch size for batching in Predict and
       Aggregate.
 
   Returns:
     PCollection of ExampleAndExtracts
   """
+
+  if not extractors:
+    extractors = [
+        PredictExtractor(eval_saved_model_path, None, shared.Shared(),
+                         desired_batch_size),
+        types.Extractor(
+            stage_name='ExtractFeatures',
+            ptransform=feature_extractor.ExtractFeatures()),
+    ]
   return (examples
           | 'ToExampleAndExtracts' >>
           beam.Map(lambda x: types.ExampleAndExtracts(example=x, extracts={}))
-          | 'Predict' >> predict_extractor.TFMAPredict(eval_saved_model_path,
-                                                       desired_batch_size)
-          | 'ExtractFeatures' >> feature_extractor.ExtractFeatures())
+          | Extract(extractors=extractors))
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/tfma_unit_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/tfma_unit_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/api/model_eval_lib.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/model_eval_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,17 @@
   return api_types.EvalResult(
       slicing_metrics=slicing_metrics, plots=plots, config=eval_config)
 
 
 def _assert_tensorflow_version():
   # Fail with a clear error in case we are not using a compatible TF version.
   major, minor, _ = tf.__version__.split('.')
-  if int(major) != 1 or int(minor) < 10:
+  if int(major) != 1 or int(minor) < 9:
     raise RuntimeError(
-        'Tensorflow version >= 1.10, < 2 is required. Found (%s). Please '
+        'Tensorflow version >= 1.9, < 2 is required. Found (%s). Please '
         'install the latest 1.x version from '
         'https://github.com/tensorflow/tensorflow. ' % tf.__version__)
 
 
 @beam.ptransform_fn
 @beam.typehints.with_output_types(beam.pvalue.PDone)
 def EvaluateAndWriteResults(  # pylint: disable=invalid-name
@@ -178,15 +178,16 @@
     slice_spec: Optional list of SingleSliceSpec specifying the slices to slice
       the data into. If None, defaults to the overall slice.
     example_weight_key: The key of the example weight column. If None, weight
       will be 1 for each example.
     add_metrics_callbacks: Optional list of callbacks for adding additional
       metrics to the graph. The names of the metrics added by the callbacks
       should not conflict with existing metrics, or metrics added by other
-      callbacks. See below for more details about what each callback should do.
+      callbacks. See docstring for Evaluate in api/impl/evaluate.py for more
+      details.
     desired_batch_size: Optional batch size for batching in Predict and
       Aggregate.
 
   Returns:
     PDone.
   """
 
@@ -264,16 +265,16 @@
         on slice "country:us".
       If None, defaults to the overall slice.
     example_weight_key: The key of the example weight column. If None, weight
       will be 1 for each example.
     add_metrics_callbacks: Optional list of callbacks for adding additional
       metrics to the graph. The names of the metrics added by the callbacks
       should not conflict with existing metrics, or metrics added by other
-      callbacks. See docstring for tensorflow_model_analysis.evaluate.Evaluate
-      for more details.
+      callbacks. See docstring for Evaluate in api/impl/evaluate.py for more
+      details.
     output_path: The directory to output metrics and results to. If None, we use
       a temporary directory.
 
   Returns:
     An EvalResult that can be used with the TFMA visualization functions.
 
   Raises:
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/types.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from __future__ import absolute_import
 from __future__ import division
 
 from __future__ import print_function
 
 import copy
 
+import apache_beam as beam
 import numpy as np
 import tensorflow as tf
 
 from tensorflow_model_analysis.types_compat import Any, Dict, List, Text, Tuple, Union, NamedTuple
 
 # pylint: disable=invalid-name
 TensorType = Union[tf.Tensor, tf.SparseTensor]
@@ -62,14 +63,18 @@
 
 # Used in building model diagnostics table, the ExampleAndExtracts holds an
 # example and all its "extractions." Extractions that should be emitted to file.
 # Each Extract has a name, stored as the key of the DictOfExtractedValues.
 DictOfExtractedValues = Dict[Text, Any]
 
 
+Extractor = NamedTuple('Extractor', [('stage_name', bytes),
+                                     ('ptransform', beam.PTransform)])
+
+
 class ExampleAndExtracts(
     NamedTuple('ExampleAndExtracts', [('example', bytes),
                                       ('extracts', DictOfExtractedValues)])):
   """Example and extracts."""
 
   def create_copy_with_shallow_copy_of_extracts(self):
     """Returns a new copy of this with a shallow copy of extracts.
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/types_compat.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/types_compat.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/constants.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/constants.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/version.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Contains the version string for this release of TFMA."""
 
 # Version string for this release of TFMA.
 # Note that setup.py reads and uses this version.
-VERSION_STRING = '0.9.1'
+VERSION_STRING = '0.9.2'
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/feature_extractor_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/feature_extractor_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/predict_extractor.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/predict_extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import apache_beam as beam
 
 from tensorflow_model_analysis import constants
 from tensorflow_model_analysis import types
 from tensorflow_model_analysis.eval_saved_model import dofn
 from tensorflow_transform.beam import shared
-from tensorflow_model_analysis.types_compat import Any, Callable, Dict, List, Optional, Tuple
+from tensorflow_model_analysis.types_compat import Any, Callable, Dict, Generator, List, Optional, Tuple
 
 MetricVariablesType = List[Any]  # pylint: disable=invalid-name
 
 # For use in Beam type annotations, because Beam's support for Python types
 # in Beam type annotations is not complete.
 _BeamSliceKeyType = beam.typehints.Tuple[  # pylint: disable=invalid-name
     beam.typehints.Tuple[bytes, beam.typehints.Union[bytes, int, float]], Ellipsis]
@@ -51,46 +51,64 @@
     self._predict_batch_size = beam.metrics.Metrics.distribution(
         _METRICS_NAMESPACE, 'predict_batch_size')
     self._num_instances = beam.metrics.Metrics.counter(_METRICS_NAMESPACE,
                                                        'num_instances')
 
   def process(self, element
              ):
-    result = []
     batch_size = len(element)
     self._predict_batch_size.update(batch_size)
     self._num_instances.inc(batch_size)
     serialized_examples = [x.example for x in element]
 
     # Compute FeaturesPredictionsLabels for each serialized_example
     for example_and_extracts, fpl in zip(
         element, self._eval_saved_model.predict_list(serialized_examples)):
 
       # Make a a shallow copy, so we don't mutate the original.
       element_copy = (
           example_and_extracts.create_copy_with_shallow_copy_of_extracts())
       element_copy.extracts[constants.FEATURES_PREDICTIONS_LABELS_KEY] = fpl
-
-      result.append(element_copy)
-
-    return result
+      yield element_copy
 
 
 @beam.ptransform_fn
-@beam.typehints.with_input_types(beam.typehints.List[types.ExampleAndExtracts])
+@beam.typehints.with_input_types(beam.typehints.Any)
 @beam.typehints.with_output_types(beam.typehints.Any)
 def TFMAPredict(  # pylint: disable=invalid-name
     examples,
     eval_saved_model_path,
+    add_metrics_callbacks,
+    shared_handle,
     desired_batch_size = None):
-  """A PTransform that adds predictions to ExamplesAndExtracts."""
+  """A PTransform that adds predictions to ExamplesAndExtracts.
+
+  Args:
+    examples: PCollection of serialized examples to be fed to the model
+    eval_saved_model_path: Path to the EvalSavedModle
+    add_metrics_callbacks: Optional list of add_metrics_callbacks. See docstring
+      for Evaluate in api/impl/evaluate.py for more details.
+    shared_handle: Handle to a shared.Shared object for sharing the in-memory
+      model within / between stages.
+    desired_batch_size: Optional. Desired batch size for prediction.
+
+  Returns:
+    PCollection of ExamplesAndExtracts, where the extracts contains the
+    features, predictions, labels retrieved.
+  """
   batch_args = {}
   if desired_batch_size:
     batch_args = dict(
         min_batch_size=desired_batch_size, max_batch_size=desired_batch_size)
+
+  # We don't actually need to add the add_metrics_callbacks to do Predict,
+  # but because if we want to share the model between Predict and subsequent
+  # stages (i.e. we use same shared handle for this and subsequent stages),
+  # then if we don't add the metrics callbacks here, they won't be present
+  # in the model in the later stages if we reuse the model from this stage.
   return (examples
           | 'Batch' >> beam.BatchElements(**batch_args)
-          | beam.ParDo(
+          | 'Predict' >> beam.ParDo(
               _TFMAPredictionDoFn(
                   eval_saved_model_path=eval_saved_model_path,
-                  add_metrics_callbacks=None,
-                  shared_handle=shared.Shared())))
+                  add_metrics_callbacks=add_metrics_callbacks,
+                  shared_handle=shared_handle)))
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/predict_extractor_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/predict_extractor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 import tensorflow as tf
 
 from tensorflow_model_analysis import types
 from tensorflow_model_analysis.eval_saved_model import testutil
 from tensorflow_model_analysis.eval_saved_model.example_trainers import linear_classifier
 from tensorflow_model_analysis.extractors import predict_extractor
+from tensorflow_transform.beam import shared
 
 
 class PredictExtractorTest(testutil.TensorflowModelAnalysisTest):
 
   def _getEvalExportDir(self):
     return os.path.join(self._getTempDir(), 'eval_export_dir')
 
@@ -59,15 +60,18 @@
               example3.SerializeToString(),
               example4.SerializeToString()
           ])
           # Our diagnostic outputs, pass types.ExampleAndExtracts throughout,
           # however our aggregating functions do not use this interface.
           | beam.Map(lambda x: types.ExampleAndExtracts(example=x, extracts={}))
           | 'Predict' >> predict_extractor.TFMAPredict(
-              eval_saved_model_path=eval_export_dir, desired_batch_size=3))
+              eval_saved_model_path=eval_export_dir,
+              add_metrics_callbacks=None,
+              shared_handle=shared.Shared(),
+              desired_batch_size=3))
 
       def check_result(got):
         try:
           self.assertEqual(4, len(got), 'got: %s' % got)
           for item in got:
             extracts_dict = item.extracts
             self.assertTrue(extracts_dict.has_key('fpl'))
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/extractors/feature_extractor.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/extractors/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/testutil.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/testutil.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/encoding.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/encoding.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/util.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/util.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/encoding_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/encoding_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/graph_ref.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/graph_ref.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/integration_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/integration_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/constants.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/constants.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metrics.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/post_export_metrics_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metric_keys.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/post_export_metrics/metric_keys.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/util_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/util_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/graph_ref_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/graph_ref_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/notebook/colab/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/load.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/load.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/exporter.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/exporter.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/export.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/export.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/dofn.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/dofn.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/multi_head.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/multi_head.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/util.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/util.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator_extra_fields.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator_extra_fields.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_classifier.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_classifier.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier_extra_fields.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier_extra_fields.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_estimator.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fixed_prediction_classifier.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/custom_estimator.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/custom_estimator.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier_multivalent.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_classifier_multivalent.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/fake_sequence_to_prediction.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/fake_sequence_to_prediction.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_regressor.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_regressor.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/dnn_regressor.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/eval_saved_model/example_trainers/csv_linear_classifier.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/eval_saved_model/example_trainers/csv_linear_classifier.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/extension.js` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/extension.js`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/vulcanized_template.html` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/vulcanized_template.html`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/index.js.map` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/index.js.map`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/static/index.js` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/static/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -183,15 +183,15 @@
             const _ = __webpack_require__(3);
 
             /**
              * Helper method to load the vulcanized templates.
              */
             function loadVulcanizedTemplate() {
                 const templateLocation =
-                    __webpack_require__.p + '/vulcanized_template.html';
+                    __webpack_require__.p + 'vulcanized_template.html';
 
                 // If the vulcanizes tempalets are not loaded yet, load it now.
                 if (!document.querySelector('link[href="' + templateLocation + '"]')) {
                     const link = document.createElement('link');
                     link.setAttribute('rel', 'import');
                     link.setAttribute('href', templateLocation);
                     document.head.appendChild(link);
```

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/proto/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slicer.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slicer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slice_accessor_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slice_accessor_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slicer_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slicer_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/slicer/slice_accessor.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/slicer/slice_accessor.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/util.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/util.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/widget_view.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/widget_view.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/util_test.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/util_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_model_analysis-0.9.1/tensorflow_model_analysis/view/__init__.py` & `tensorflow_model_analysis-0.9.2/tensorflow_model_analysis/view/__init__.py`

 * *Files identical despite different names*

