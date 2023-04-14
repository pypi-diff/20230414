# Comparing `tmp/mlprimitives-0.3.4.dev0.tar.gz` & `tmp/mlprimitives-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlprimitives-0.3.4.dev0.tar", last modified: Tue Jan 24 14:54:34 2023, max compression
+gzip compressed data, was "mlprimitives-0.3.5.tar", last modified: Fri Apr 14 21:55:05 2023, max compression
```

## Comparing `mlprimitives-0.3.4.dev0.tar` & `mlprimitives-0.3.5.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)    29688 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)     5337 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)    12497 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/HISTORY.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)      222 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/test_utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/tests/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)     1757 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/primitives/test_primitives.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/tests/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)     1966 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/adapters/test_statsmodels.py
--rw-r--r--   0 sarah      (501) staff       (20)     1841 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/adapters/test_keras.py
--rw-r--r--   0 sarah      (501) staff       (20)     5032 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/adapters/test_pandas.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/tests/custom/
--rw-r--r--   0 sarah      (501) staff       (20)    15173 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/custom/test_timeseries_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     2199 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/custom/test_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     1289 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/custom/test_text.py
--rw-r--r--   0 sarah      (501) staff       (20)     7366 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/custom/test_timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)     5620 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/tests/custom/test_feature_extraction.py
--rw-r--r--   0 sarah      (501) staff       (20)      304 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/MANIFEST.in
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      573 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      613 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/Makefile
--rwxr-xr-x   0 sarah      (501) staff       (20)     6015 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)      774 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/history.rst
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/authors.rst
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/readme.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/docs/community/
--rw-r--r--   0 sarah      (501) staff       (20)     7980 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/community/custom.rst
--rw-r--r--   0 sarah      (501) staff       (20)     7697 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/community/annotations.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5143 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/community/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8554 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/community/adapters.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3347 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/community/welcome.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/docs/getting_started/
--rw-r--r--   0 sarah      (501) staff       (20)     7656 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/docs/getting_started/concepts.rst
--rw-r--r--   0 sarah      (501) staff       (20)    11316 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/README.md
--rw-r--r--   0 sarah      (501) staff       (20)     3274 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/
--rw-r--r--   0 sarah      (501) staff       (20)     5451 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/dsp.py
--rw-r--r--   0 sarah      (501) staff       (20)     4806 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/audio_featurization.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/timeseries/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/timeseries/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    13260 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/timeseries/cyclegan.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)      735 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/candidates/audio_padding.py
--rw-r--r--   0 sarah      (501) staff       (20)     2535 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/evaluation.py
--rw-r--r--   0 sarah      (501) staff       (20)    21026 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/datasets.py
--rw-r--r--   0 sarah      (501) staff       (20)      484 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/
--rw-r--r--   0 sarah      (501) staff       (20)      262 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.Lars.json
--rw-r--r--   0 sarah      (501) staff       (20)      563 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_selection.LassoFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)     1680 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.LSTMTextClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      433 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.mode.json
--rw-r--r--   0 sarah      (501) staff       (20)      296 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.GradientBoostingRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      264 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.Lasso.json
--rw-r--r--   0 sarah      (501) staff       (20)      330 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.preprocessing.RobustScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1323 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/text.classification.lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)      435 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.median.json
--rw-r--r--   0 sarah      (501) staff       (20)      496 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.MLPBinaryClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      375 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.CategoricalEncoder.json
--rw-r--r--   0 sarah      (501) staff       (20)      373 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json
--rw-r--r--   0 sarah      (501) staff       (20)      771 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.LSTMBinaryTextClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      431 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.mean.json
--rw-r--r--   0 sarah      (501) staff       (20)      364 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.regression.resnet50.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      365 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.classification.resnet50.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      423 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.classification.hog.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      371 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.StringVectorizer.json
--rw-r--r--   0 sarah      (501) staff       (20)      284 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.ExtraTreesRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      836 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      264 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.Ridge.json
--rw-r--r--   0 sarah      (501) staff       (20)      330 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.preprocessing.MinMaxScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)      323 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.FastICA.json
--rw-r--r--   0 sarah      (501) staff       (20)      677 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.classification.text.json
--rw-r--r--   0 sarah      (501) staff       (20)      318 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.impute.SimpleImputer.json
--rw-r--r--   0 sarah      (501) staff       (20)      428 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      282 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.BaggingClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      284 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.AdaBoostClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      493 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.classification.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      286 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.LinearRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)      288 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.RandomForestRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      401 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)      345 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.RandomTreesEmbedding.json
--rw-r--r--   0 sarah      (501) staff       (20)      422 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.regression.hog.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      617 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.MLPMultiClassClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      345 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.DictionaryLearning.json
--rw-r--r--   0 sarah      (501) staff       (20)      587 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/graph.link_prediction.nx.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      333 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.TruncatedSVD.json
--rw-r--r--   0 sarah      (501) staff       (20)      337 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.FactorAnalysis.json
--rw-r--r--   0 sarah      (501) staff       (20)      406 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)      315 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.RandomForestClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      300 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.GradientBoostingClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      278 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.IsolationForest.json
--rw-r--r--   0 sarah      (501) staff       (20)      292 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.LogisticRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)      439 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.regression.hog.rf.json
--rw-r--r--   0 sarah      (501) staff       (20)      330 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.preprocessing.MaxAbsScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)      274 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.ElasticNet.json
--rw-r--r--   0 sarah      (501) staff       (20)      280 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.AdaBoostRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      440 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/image.classification.hog.rf.json
--rw-r--r--   0 sarah      (501) staff       (20)      278 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.BaggingRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      656 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/graph.graph_matching.nx.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      555 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.text.TextCleaner.json
--rw-r--r--   0 sarah      (501) staff       (20)      797 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.VGGCNNClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      368 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.regression.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      327 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.KernelPCA.json
--rw-r--r--   0 sarah      (501) staff       (20)      315 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.decomposition.PCA.json
--rw-r--r--   0 sarah      (501) staff       (20)      329 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.linear_model.MultiTaskLasso.json
--rw-r--r--   0 sarah      (501) staff       (20)      627 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.classification.json
--rw-r--r--   0 sarah      (501) staff       (20)      288 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/sklearn.ensemble.ExtraTreesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      667 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/multi_table.classification.dfs.xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)      437 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.regression.text.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)     3546 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Lars.json
--rw-r--r--   0 sarah      (501) staff       (20)     3663 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.LassoFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)     5340 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTextClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     5015 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.GradientBoostingRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.select_dtypes.json
--rw-r--r--   0 sarah      (501) staff       (20)      947 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.pop.json
--rw-r--r--   0 sarah      (501) staff       (20)     1198 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.resnet50.ResNet50.json
--rw-r--r--   0 sarah      (501) staff       (20)     5411 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Lasso.json
--rw-r--r--   0 sarah      (501) staff       (20)     2278 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.RobustScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1028 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.VocabularyCounter.json
--rw-r--r--   0 sarah      (501) staff       (20)     1204 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.mobilenet.MobileNet.json
--rw-r--r--   0 sarah      (501) staff       (20)     3002 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.entity_from_dataframe.json
--rw-r--r--   0 sarah      (501) staff       (20)     9451 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.SGDClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      911 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.preprocess_input.json
--rw-r--r--   0 sarah      (501) staff       (20)     1686 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.filter.json
--rw-r--r--   0 sarah      (501) staff       (20)     1201 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.xception.Xception.json
--rw-r--r--   0 sarah      (501) staff       (20)     1371 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/statsmodels.tsa.arima_model.Arima.json
--rw-r--r--   0 sarah      (501) staff       (20)     4125 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.MLPBinaryClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1609 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.CategoricalEncoder.json
--rw-r--r--   0 sarah      (501) staff       (20)     1211 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/community.CommunityBestPartition.json
--rw-r--r--   0 sarah      (501) staff       (20)     1294 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json
--rw-r--r--   0 sarah      (501) staff       (20)     3687 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.dfs.json
--rw-r--r--   0 sarah      (501) staff       (20)     1427 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.score_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     3742 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMBinaryTextClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2459 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1399 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.drop_duplicates.json
--rw-r--r--   0 sarah      (501) staff       (20)     2271 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/lightfm.LightFM.json
--rw-r--r--   0 sarah      (501) staff       (20)     1220 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.inception_v3.InceptionV3.json
--rw-r--r--   0 sarah      (501) staff       (20)     3791 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier_proba.json
--rw-r--r--   0 sarah      (501) staff       (20)     1262 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.StandardScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1912 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.find_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     1502 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.trivial.TrivialPredictor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1224 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.Series.filter.json
--rw-r--r--   0 sarah      (501) staff       (20)     1817 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.set_index.json
--rw-r--r--   0 sarah      (501) staff       (20)     2465 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/skimage.feature.hog.json
--rw-r--r--   0 sarah      (501) staff       (20)      911 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.resnet50.preprocess_input.json
--rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/xgboost.XGBRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1209 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/networkx.graph_feature_extraction.json
--rw-r--r--   0 sarah      (501) staff       (20)     1522 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.naive_bayes.MultinomialNB.json
--rw-r--r--   0 sarah      (501) staff       (20)     4504 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2134 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.StringVectorizer.json
--rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.to_numpy.json
--rw-r--r--   0 sarah      (501) staff       (20)     2401 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)      821 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.ravel.json
--rw-r--r--   0 sarah      (501) staff       (20)      924 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassDecoder.json
--rw-r--r--   0 sarah      (501) staff       (20)     3804 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.ExtraTreesRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     4533 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     4365 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Ridge.json
--rw-r--r--   0 sarah      (501) staff       (20)     1779 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/cv2.GaussianBlur.json
--rw-r--r--   0 sarah      (501) staff       (20)     2037 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences.json
--rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet201.json
--rw-r--r--   0 sarah      (501) staff       (20)     2226 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/xgboost.XGBClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1663 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.MinMaxScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1300 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.add_relationship.json
--rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet169.json
--rw-r--r--   0 sarah      (501) staff       (20)     2464 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.FastICA.json
--rw-r--r--   0 sarah      (501) staff       (20)     1352 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/networkx.link_prediction_feature_extraction.json
--rw-r--r--   0 sarah      (501) staff       (20)     1765 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.impute.SimpleImputer.json
--rw-r--r--   0 sarah      (501) staff       (20)     4482 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)    12064 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.CycleGAN.json
--rw-r--r--   0 sarah      (501) staff       (20)     1607 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.append.json
--rw-r--r--   0 sarah      (501) staff       (20)     2513 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.BaggingClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1890 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.AdaBoostClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.reshape.json
--rw-r--r--   0 sarah      (501) staff       (20)      914 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.mobilenet.preprocess_input.json
--rw-r--r--   0 sarah      (501) staff       (20)     2378 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.LinearRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)     1183 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences.json
--rw-r--r--   0 sarah      (501) staff       (20)      923 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.inception_v3.preprocess_input.json
--rw-r--r--   0 sarah      (501) staff       (20)      786 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.count_features.json
--rw-r--r--   0 sarah      (501) staff       (20)      847 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.argmax.json
--rw-r--r--   0 sarah      (501) staff       (20)     3909 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1451 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)     3202 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomTreesEmbedding.json
--rw-r--r--   0 sarah      (501) staff       (20)     1190 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.json
--rw-r--r--   0 sarah      (501) staff       (20)     4297 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.MLPMultiClassClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     3486 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.DictionaryLearning.json
--rw-r--r--   0 sarah      (501) staff       (20)     1887 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.TruncatedSVD.json
--rw-r--r--   0 sarah      (501) staff       (20)     1638 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.Imputer.json
--rw-r--r--   0 sarah      (501) staff       (20)     2344 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier_proba.json
--rw-r--r--   0 sarah      (501) staff       (20)     2368 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.FactorAnalysis.json
--rw-r--r--   0 sarah      (501) staff       (20)     1579 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.dropna.json
--rw-r--r--   0 sarah      (501) staff       (20)     1254 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.regression_errors.json
--rw-r--r--   0 sarah      (501) staff       (20)     1454 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json
--rw-r--r--   0 sarah      (501) staff       (20)     3721 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1660 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.preprocessing.sequence.pad_sequences.json
--rw-r--r--   0 sarah      (501) staff       (20)     4782 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.GradientBoostingClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2565 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.IsolationForest.json
--rw-r--r--   0 sarah      (501) staff       (20)     7498 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.LogisticRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)     2422 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.dsp.SpectralMask.json
--rw-r--r--   0 sarah      (501) staff       (20)     4688 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTextRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1534 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate.json
--rw-r--r--   0 sarah      (501) staff       (20)     1402 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.MaxAbsScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     2745 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.feature_extraction.text.CountVectorizer.json
--rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet121.json
--rw-r--r--   0 sarah      (501) staff       (20)     1621 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.drop.json
--rw-r--r--   0 sarah      (501) staff       (20)     5189 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.ElasticNet.json
--rw-r--r--   0 sarah      (501) staff       (20)     1914 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.AdaBoostRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     2510 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.BaggingRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1756 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.text.TextCleaner.json
--rw-r--r--   0 sarah      (501) staff       (20)      952 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.audio_padding.AudioPadder.json
--rw-r--r--   0 sarah      (501) staff       (20)     7933 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.VGGCNNClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      880 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.intervals_to_mask.json
--rw-r--r--   0 sarah      (501) staff       (20)     1321 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.OneHotEncoder.json
--rw-r--r--   0 sarah      (501) staff       (20)     1684 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.naive_bayes.GaussianNB.json
--rw-r--r--   0 sarah      (501) staff       (20)     5181 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     3369 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.KernelPCA.json
--rw-r--r--   0 sarah      (501) staff       (20)     1020 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.UniqueCounter.json
--rw-r--r--   0 sarah      (501) staff       (20)     2238 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.PCA.json
--rw-r--r--   0 sarah      (501) staff       (20)     1112 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeUnscaler.json
--rw-r--r--   0 sarah      (501) staff       (20)      901 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.audio_featurization.featurize_audio.json
--rw-r--r--   0 sarah      (501) staff       (20)     1948 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.join.json
--rw-r--r--   0 sarah      (501) staff       (20)     4290 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.MultiTaskLasso.json
--rw-r--r--   0 sarah      (501) staff       (20)     2278 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.resample.json
--rw-r--r--   0 sarah      (501) staff       (20)     1248 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     2041 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.preprocessing.text.Tokenizer.json
--rw-r--r--   0 sarah      (501) staff       (20)     1109 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_average.json
--rw-r--r--   0 sarah      (501) staff       (20)     5010 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     3098 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.normalize_entity.json
--rw-r--r--   0 sarah      (501) staff       (20)     1047 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.set.json
--rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.fillna.json
--rw-r--r--   0 sarah      (501) staff       (20)     1628 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.feature_extraction.text.TfidfTransformer.json
--rw-r--r--   0 sarah      (501) staff       (20)     1049 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassEncoder.json
--rw-r--r--   0 sarah      (501) staff       (20)     3885 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.ExtraTreesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      998 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.get.json
--rw-r--r--   0 sarah      (501) staff       (20)      911 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.xception.preprocess_input.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)      875 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/lightfm.py
--rw-r--r--   0 sarah      (501) staff       (20)     3458 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/pandas.py
--rw-r--r--   0 sarah      (501) staff       (20)     4093 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/keras.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     5693 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/featuretools.py
--rw-r--r--   0 sarah      (501) staff       (20)      571 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/skimage.py
--rw-r--r--   0 sarah      (501) staff       (20)      884 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/community.py
--rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/statsmodels.py
--rw-r--r--   0 sarah      (501) staff       (20)      524 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/cv2.py
--rw-r--r--   0 sarah      (501) staff       (20)     1737 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/adapters/networkx.py
--rw-r--r--   0 sarah      (501) staff       (20)     4191 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/cli.py
--rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/
--rw-r--r--   0 sarah      (501) staff       (20)     1641 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/counters.py
--rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)     1210 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/trivial.py
--rw-r--r--   0 sarah      (501) staff       (20)     3584 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/feature_selection.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     9242 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/feature_extraction.py
--rw-r--r--   0 sarah      (501) staff       (20)     1676 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     3606 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/text.py
--rw-r--r--   0 sarah      (501) staff       (20)     9481 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/mlprimitives/custom/timeseries_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)      480 2023-01-24 14:49:59.000000 mlprimitives-0.3.4.dev0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1137 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/setup.cfg
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    29688 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)    14510 2023-01-24 14:54:34.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)      220 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)      832 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)       13 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-24 14:54:33.000000 mlprimitives-0.3.4.dev0/mlprimitives.egg-info/dependency_links.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.416189 mlprimitives-0.3.5/
+-rw-r--r--   0 sarah      (501) staff       (20)      480 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5337 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)    12809 2023-04-14 21:55:00.000000 mlprimitives-0.3.5/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      304 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    25012 2023-04-14 21:55:05.416454 mlprimitives-0.3.5/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)    11316 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.211580 mlprimitives-0.3.5/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      613 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/Makefile
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/authors.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.215303 mlprimitives-0.3.5/docs/community/
+-rw-r--r--   0 sarah      (501) staff       (20)     8554 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/community/adapters.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7697 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/community/annotations.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5143 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/community/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7980 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/community/custom.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3347 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/community/welcome.rst
+-rwxr-xr-x   0 sarah      (501) staff       (20)     6015 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/conf.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.216005 mlprimitives-0.3.5/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)     7656 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/getting_started/concepts.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/history.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      573 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      774 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/make.bat
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/docs/readme.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.220808 mlprimitives-0.3.5/mlprimitives/
+-rw-r--r--   0 sarah      (501) staff       (20)      479 2023-04-14 21:55:00.000000 mlprimitives-0.3.5/mlprimitives/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.235287 mlprimitives-0.3.5/mlprimitives/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      884 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/community.py
+-rw-r--r--   0 sarah      (501) staff       (20)      524 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/cv2.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5693 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/featuretools.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4093 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)      875 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/lightfm.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1737 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/networkx.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3458 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)      571 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/skimage.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/adapters/statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.239524 mlprimitives-0.3.5/mlprimitives/candidates/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4806 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/audio_featurization.py
+-rw-r--r--   0 sarah      (501) staff       (20)      735 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/audio_padding.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5451 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/dsp.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.241279 mlprimitives-0.3.5/mlprimitives/candidates/timeseries/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/timeseries/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    13260 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/candidates/timeseries/cyclegan.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4191 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/cli.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.250181 mlprimitives-0.3.5/mlprimitives/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1641 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/counters.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9242 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/feature_extraction.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3584 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/feature_selection.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1676 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3606 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/text.py
+-rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9481 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/timeseries_preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1210 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/custom/trivial.py
+-rw-r--r--   0 sarah      (501) staff       (20)    21026 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/datasets.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2535 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/evaluation.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.308090 mlprimitives-0.3.5/mlprimitives/pipelines/
+-rw-r--r--   0 sarah      (501) staff       (20)      656 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/graph.graph_matching.nx.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      587 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/graph.link_prediction.nx.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      440 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.classification.hog.rf.json
+-rw-r--r--   0 sarah      (501) staff       (20)      423 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.classification.hog.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      365 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.classification.resnet50.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      439 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.regression.hog.rf.json
+-rw-r--r--   0 sarah      (501) staff       (20)      422 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.regression.hog.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      364 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/image.regression.resnet50.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      771 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.LSTMBinaryTextClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1680 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.LSTMTextClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      496 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.MLPBinaryClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      617 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.MLPMultiClassClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      836 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      428 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      797 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.VGGCNNClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      375 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.CategoricalEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)      373 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)      371 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_extraction.StringVectorizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)      406 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)      401 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)      563 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_selection.LassoFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)      555 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.text.TextCleaner.json
+-rw-r--r--   0 sarah      (501) staff       (20)      431 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.mean.json
+-rw-r--r--   0 sarah      (501) staff       (20)      435 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.median.json
+-rw-r--r--   0 sarah      (501) staff       (20)      433 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.trivial.TrivialPredictor.mode.json
+-rw-r--r--   0 sarah      (501) staff       (20)      667 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/multi_table.classification.dfs.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      627 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/single_table.classification.json
+-rw-r--r--   0 sarah      (501) staff       (20)      677 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/single_table.classification.text.json
+-rw-r--r--   0 sarah      (501) staff       (20)      493 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/single_table.classification.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      437 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/single_table.regression.text.json
+-rw-r--r--   0 sarah      (501) staff       (20)      368 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/single_table.regression.xgb.json
+-rw-r--r--   0 sarah      (501) staff       (20)      345 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.DictionaryLearning.json
+-rw-r--r--   0 sarah      (501) staff       (20)      337 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.FactorAnalysis.json
+-rw-r--r--   0 sarah      (501) staff       (20)      323 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.FastICA.json
+-rw-r--r--   0 sarah      (501) staff       (20)      327 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.KernelPCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)      315 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.PCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)      333 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.decomposition.TruncatedSVD.json
+-rw-r--r--   0 sarah      (501) staff       (20)      284 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.AdaBoostClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      280 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.AdaBoostRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      282 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.BaggingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      278 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.BaggingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      288 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.ExtraTreesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      284 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.ExtraTreesRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      300 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.GradientBoostingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      296 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.GradientBoostingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      278 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.IsolationForest.json
+-rw-r--r--   0 sarah      (501) staff       (20)      315 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.RandomForestClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      288 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.RandomForestRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      345 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.ensemble.RandomTreesEmbedding.json
+-rw-r--r--   0 sarah      (501) staff       (20)      318 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.impute.SimpleImputer.json
+-rw-r--r--   0 sarah      (501) staff       (20)      274 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.ElasticNet.json
+-rw-r--r--   0 sarah      (501) staff       (20)      262 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.Lars.json
+-rw-r--r--   0 sarah      (501) staff       (20)      264 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.Lasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)      286 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.LinearRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)      292 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.LogisticRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)      329 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.MultiTaskLasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)      264 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.linear_model.Ridge.json
+-rw-r--r--   0 sarah      (501) staff       (20)      330 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.preprocessing.MaxAbsScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)      330 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.preprocessing.MinMaxScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)      330 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/sklearn.preprocessing.RobustScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1323 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/pipelines/text.classification.lstm.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.409443 mlprimitives-0.3.5/mlprimitives/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     1211 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/community.CommunityBestPartition.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1779 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/cv2.GaussianBlur.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1300 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.add_relationship.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3002 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.entity_from_dataframe.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3098 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.normalize_entity.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3687 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/featuretools.dfs.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5010 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3742 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMBinaryTextClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5340 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTextClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4688 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTextRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4504 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5181 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4125 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.MLPBinaryClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4297 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.MLPMultiClassClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4533 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4482 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     7933 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.VGGCNNClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet121.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet169.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1205 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet201.json
+-rw-r--r--   0 sarah      (501) staff       (20)      911 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.preprocess_input.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1220 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.inception_v3.InceptionV3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      923 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.inception_v3.preprocess_input.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1204 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.mobilenet.MobileNet.json
+-rw-r--r--   0 sarah      (501) staff       (20)      914 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.mobilenet.preprocess_input.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1198 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.resnet50.ResNet50.json
+-rw-r--r--   0 sarah      (501) staff       (20)      911 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.resnet50.preprocess_input.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1201 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.xception.Xception.json
+-rw-r--r--   0 sarah      (501) staff       (20)      911 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.xception.preprocess_input.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1660 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.preprocessing.sequence.pad_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2041 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/keras.preprocessing.text.Tokenizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2271 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/lightfm.LightFM.json
+-rw-r--r--   0 sarah      (501) staff       (20)      901 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.audio_featurization.featurize_audio.json
+-rw-r--r--   0 sarah      (501) staff       (20)      952 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.audio_padding.AudioPadder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2422 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.dsp.SpectralMask.json
+-rw-r--r--   0 sarah      (501) staff       (20)    12064 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.CycleGAN.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1427 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.score_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1020 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.UniqueCounter.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1028 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.VocabularyCounter.json
+-rw-r--r--   0 sarah      (501) staff       (20)      786 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.count_features.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1609 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.CategoricalEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1294 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2134 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.StringVectorizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1454 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1451 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3663 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.LassoFeatureSelector.json
+-rw-r--r--   0 sarah      (501) staff       (20)      924 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassDecoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1049 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1190 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1112 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeUnscaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1756 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.text.TextCleaner.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1912 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.find_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1254 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.regression_errors.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1183 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)      880 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.intervals_to_mask.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2037 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1534 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1109 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_average.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1502 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.trivial.TrivialPredictor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1209 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/networkx.graph_feature_extraction.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1352 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/networkx.link_prediction_feature_extraction.json
+-rw-r--r--   0 sarah      (501) staff       (20)      847 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/numpy.argmax.json
+-rw-r--r--   0 sarah      (501) staff       (20)      821 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/numpy.ravel.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/numpy.reshape.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1607 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.append.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1621 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.drop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1399 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.drop_duplicates.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1579 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.dropna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.fillna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1686 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)      998 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.get.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1948 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.join.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.json
+-rw-r--r--   0 sarah      (501) staff       (20)      947 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.pop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2278 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.resample.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.select_dtypes.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1047 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.set.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1817 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.set_index.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.to_numpy.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1248 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1224 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/pandas.Series.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2465 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/skimage.feature.hog.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3486 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.DictionaryLearning.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2368 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.FactorAnalysis.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2464 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.FastICA.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3369 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.KernelPCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2238 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.PCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1887 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.TruncatedSVD.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1890 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.AdaBoostClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1914 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.AdaBoostRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2513 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.BaggingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2510 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.BaggingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3885 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.ExtraTreesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3804 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.ExtraTreesRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4782 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.GradientBoostingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5015 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.GradientBoostingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2565 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.IsolationForest.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3721 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3791 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier_proba.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3909 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3202 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomTreesEmbedding.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2745 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.feature_extraction.text.CountVectorizer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1628 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.feature_extraction.text.TfidfTransformer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1765 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.impute.SimpleImputer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5189 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.ElasticNet.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3546 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Lars.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5411 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Lasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2378 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.LinearRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     7498 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.LogisticRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4290 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.MultiTaskLasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4365 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Ridge.json
+-rw-r--r--   0 sarah      (501) staff       (20)     9451 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.SGDClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1684 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.naive_bayes.GaussianNB.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1522 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.naive_bayes.MultinomialNB.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2459 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2344 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier_proba.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2401 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1638 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.Imputer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1402 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.MaxAbsScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1663 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.MinMaxScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1321 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.OneHotEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2278 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.RobustScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1262 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.StandardScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1371 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/statsmodels.tsa.arima_model.Arima.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2226 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/xgboost.XGBClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/primitives/xgboost.XGBRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/mlprimitives/utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.225632 mlprimitives-0.3.5/mlprimitives.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    25012 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)    14510 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)      219 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      832 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       13 2023-04-14 21:55:05.000000 mlprimitives-0.3.5/mlprimitives.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1132 2023-04-14 21:55:05.418781 mlprimitives-0.3.5/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     3269 2023-04-14 21:55:00.000000 mlprimitives-0.3.5/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.410072 mlprimitives-0.3.5/tests/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.412123 mlprimitives-0.3.5/tests/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)     1841 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/adapters/test_keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5032 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/adapters/test_pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1966 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/adapters/test_statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.415211 mlprimitives-0.3.5/tests/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)     5620 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/custom/test_feature_extraction.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2199 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/custom/test_preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1289 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/custom/test_text.py
+-rw-r--r--   0 sarah      (501) staff       (20)     7366 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/custom/test_timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)    15173 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/custom/test_timeseries_preprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 21:55:05.415729 mlprimitives-0.3.5/tests/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     1757 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/primitives/test_primitives.py
+-rw-r--r--   0 sarah      (501) staff       (20)      222 2023-04-14 19:29:42.000000 mlprimitives-0.3.5/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mlprimitives-0.3.4.dev0/PKG-INFO` & `mlprimitives-0.3.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,648 +1,661 @@
 Metadata-Version: 2.1
 Name: mlprimitives
-Version: 0.3.4.dev0
+Version: 0.3.5
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLPrimitives
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
-Description: <p align="left">
-          <a href="https://dai.lids.mit.edu">
-            <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
-          </a>
-          <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
-        </p>
-        
-        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        [![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)](https://pypi.python.org/pypi/mlprimitives)
-        [![Tests](https://github.com/MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
-        [![Downloads](https://pepy.tech/badge/mlprimitives)](https://pepy.tech/project/mlprimitives)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
-        
-        # MLPrimitives
-        
-        Pipelines and primitives for machine learning and data science.
-        
-        * Documentation: https://MLBazaar.github.io/MLPrimitives
-        * Github: https://github.com/MLBazaar/MLPrimitives
-        * License: [MIT](https://github.com/MLBazaar/MLPrimitives/blob/master/LICENSE)
-        * Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        
-        # Overview
-        
-        This repository contains primitive annotations to be used by the MLBlocks library, as well as
-        the necessary Python code to make some of them fully compatible with the MLBlocks API requirements.
-        
-        There is also a collection of custom primitives contributed directly to this library, which either
-        combine third party tools or implement new functionalities from scratch.
-        
-        ## Why did we create this library?
-        
-        * Too many libraries in a fast growing field
-        * Huge societal need to build machine learning apps
-        * Domain expertise resides at several places (knowledge of math)
-        * No documented information about hyperparameters, behavior...
-        
-        # Installation
-        
-        ## Requirements
-        
-        **MLPrimitives** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
-        
-        Also, although it is not strictly required, the usage of a
-        [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
-        interfering with other software installed in the system where **MLPrimitives** is run.
-        
-        ## Install with pip
-        
-        The easiest and recommended way to install **MLPrimitives** is using [pip](https://pip.pypa.io/en/stable/):
-        
-        ```bash
-        pip install mlprimitives
-        ```
-        
-        This will pull and install the latest stable release from [PyPi](https://pypi.org/).
-        
-        If you want to install from source or contribute to the project please read the
-        [Contributing Guide](https://MLBazaar.github.io/MLPrimitives/community/welcome.html).
-        
-        # Quickstart
-        
-        This section is a short series of tutorials to help you getting started with MLPrimitives.
-        
-        In the following steps you will learn how to load and run a primitive on some data.
-        
-        Later on you will learn how to evaluate and improve the performance of a primitive by tuning
-        its hyperparameters.
-        
-        ## Running a Primitive
-        
-        In this first tutorial, we will be executing a single primitive for data transformation.
-        
-        ### 1. Load a Primitive
-        
-        The first step in order to run a primitive is to load it.
-        
-        This will be done using the `mlprimitives.load_primitive` function, which will
-        load the indicated primitive as an [MLBlock Object from MLBlocks](https://MLBazaar.github.io/MLBlocks/api/mlblocks.html#mlblocks.MLBlock)
-        
-        In this case, we will load the `mlprimitives.custom.feature_extraction.CategoricalEncoder`
-        primitive.
-        
-        ```python3
-        from mlprimitives import load_primitive
-        
-        primitive = load_primitive('mlprimitives.custom.feature_extraction.CategoricalEncoder')
-        ```
-        
-        ### 2. Load some data
-        
-        The CategoricalEncoder is a transformation primitive which applies one-hot encoding to all the
-        categorical columns of a `pandas.DataFrame`.
-        
-        So, in order to be able to run our primitive, we will first load some data that contains
-        categorical columns.
-        
-        This can be done with the `mlprimitives.datasets.load_census` function:
-        
-        ```python3
-        from mlprimitives.datasets import load_census
-        
-        dataset = load_census()
-        ```
-        
-        This dataset object has an attribute `data` which contains a table with several categorical
-        columns.
-        
-        We can have a look at this table by executing `dataset.data.head()`, which will return a
-        table like this:
-        
-        ```
-                                     0                    1                   2
-        age                         39                   50                  38
-        workclass            State-gov     Self-emp-not-inc             Private
-        fnlwgt                   77516                83311              215646
-        education            Bachelors            Bachelors             HS-grad
-        education-num               13                   13                   9
-        marital-status   Never-married   Married-civ-spouse            Divorced
-        occupation        Adm-clerical      Exec-managerial   Handlers-cleaners
-        relationship     Not-in-family              Husband       Not-in-family
-        race                     White                White               White
-        sex                       Male                 Male                Male
-        capital-gain              2174                    0                   0
-        capital-loss                 0                    0                   0
-        hours-per-week              40                   13                  40
-        native-country   United-States        United-States       United-States
-        ```
-        
-        ### 3. Fit the primitive
-        
-        In order to run our pipeline, we first need to fit it.
-        
-        This is the process where it analyzes the data to detect which columns are categorical
-        
-        This is done by calling its `fit` method and assing the `dataset.data` as `X`.
-        
-        ```python3
-        primitive.fit(X=dataset.data)
-        ```
-        
-        ### 4. Produce results
-        
-        Once the pipeline is fit, we can process the data by calling the `produce` method of the
-        primitive instance and passing agin the `data` as `X`.
-        
-        ```python3
-        transformed = primitive.produce(X=dataset.data)
-        ```
-        
-        After this is done, we can see how the transformed data contains the newly generated
-        one-hot vectors:
-        
-        ```
-                                                        0      1       2       3       4
-        age                                            39     50      38      53      28
-        fnlwgt                                      77516  83311  215646  234721  338409
-        education-num                                  13     13       9       7      13
-        capital-gain                                 2174      0       0       0       0
-        capital-loss                                    0      0       0       0       0
-        hours-per-week                                 40     13      40      40      40
-        workclass= Private                              0      0       1       1       1
-        workclass= Self-emp-not-inc                     0      1       0       0       0
-        workclass= Local-gov                            0      0       0       0       0
-        workclass= ?                                    0      0       0       0       0
-        workclass= State-gov                            1      0       0       0       0
-        workclass= Self-emp-inc                         0      0       0       0       0
-        ...                                             ...    ...     ...     ...     ...
-        ```
-        
-        ## Tuning a Primitive
-        
-        In this short tutorial we will teach you how to evaluate the performance of a primitive
-        and improve its performance by modifying its hyperparameters.
-        
-        To do so, we will load a primitive that can learn from the transformed data that we just
-        generated and later on make predictions based on new data.
-        
-        ### 1. Load another primitive
-        
-        Firs of all, we will load the `xgboost.XGBClassifier` primitive that we will use afterwards.
-        
-        ```python3
-        primitive = load_primitive('xgboost.XGBClassifier')
-        ```
-        
-        ### 2. Split the dataset
-        
-        Before being able to evaluate the primitive perfomance, we need to split the data in two
-        parts: train, which will be used for the primitive to learn, and test, which will be used
-        to make the predictions that later on will be evaluated.
-        
-        In order to do this, we will get the first 75% of rows from the transformed data that we
-        obtained above and call it `X_train`, and then set the next 25% of rows as `X_test`.
-        
-        ```python3
-        train_size = int(len(transformed) * 0.75)
-        X_train = transformed.iloc[:train_size]
-        X_test = transformed.iloc[train_size:]
-        ```
-        
-        Similarly, we need to obtain the `y_train` and `y_test` variables containing the corresponding
-        output values.
-        
-        ```python3
-        y_train = dataset.target[:train_size]
-        y_test = dataset.target[train_size:]
-        ```
-        
-        ### 3. Fit the new primitive
-        
-        Once we have have splitted the data, we can fit the primitive by passing `X_train` and `y_train`
-        to its `fit` method.
-        
-        ```python3
-        primitive.fit(X=X_train, y=y_train)
-        ```
-        
-        ### 4. Make predictions
-        
-        Once the primitive has been fitted, we can produce predictions using the `X_test` data as input.
-        
-        ```python3
-        predictions = primitive.produce(X=X_test)
-        ```
-        
-        ### 5. Evalute the performance
-        
-        We can now evaluate how good the predictions from our primitive are by using the `score`
-        method from the `dataset` object on both the expected output and the real output from the
-        primitive:
-        
-        ```python3
-        dataset.score(y_test, predictions)
-        ```
-        
-        This will output a float value between 0 and 1 indicating how good the predicitons are, being
-        0 the worst score possible and 1 the best one.
-        
-        In this case we will obtain a score around 0.866
-        
-        ### 6. Set new hyperparameter values
-        
-        In order to improve the performance of our primitive we will try to modify a couple of its
-        hyperparameters.
-        
-        First we will see which hyperparameter values the primitive has by calling its
-        `get_hyperparameters` method.
-        
-        ```python3
-        primitive.get_hyperparameters()
-        ```
-        
-        which will return a dictionary like this:
-        
-        ```python
-        {
-            "n_jobs": -1,
-            "n_estimators": 100,
-            "max_depth": 3,
-            "learning_rate": 0.1,
-            "gamma": 0,
-            "min_child_weight": 1
-        }
-        ```
-        
-        Next, we will see which are the valid values for each one of those hyperparameters by calling its
-        `get_tunable_hyperparameters` method:
-        
-        ```python3
-        primitive.get_tunable_hyperparameters()
-        ```
-        
-        For example, we will see that the `max_depth` hyperparameter has the following specification:
-        
-        ```python
-        {
-            "type": "int",
-            "default": 3,
-            "range": [
-                3,
-                10
-            ]
-        }
-        ```
-        
-        Next, we will choose a valid value, for example 7, and set it into the pipeline using the
-        `set_hyperparameters` method:
-        
-        ```python3
-        primitive.set_hyperparameters({'max_depth': 7})
-        ```
-        
-        ### 7. Re-evaluate the performance
-        
-        Once the new hyperparameter value has been set, we repeat the fit/train/score cycle to
-        evaluate the performance of this new hyperparameter value:
-        
-        ```python3
-        primitive.fit(X=X_train, y=y_train)
-        predictions = primitive.produce(X=X_test)
-        dataset.score(y_test, predictions)
-        ```
-        
-        This time we should see that the performance has improved to a value around 0.724
-        
-        ## What's Next?
-        
-        Do you want to [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/getting_started/concepts.html),
-        about [how to contribute to it](https://MLBazaar.github.io/MLPrimitives/community/contributing.html)
-        or browse the [API Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
-        Please check the corresponding sections of the [documentation](https://MLBazaar.github.io/MLPrimitives/)!
-        
-        
-        # History
-        
-        ## 0.3.3 - 2023-01-20
-        
-        ### General Imporvements
-        
-        * Update dependencies - [Issue #276](https://github.com/MLBazaar/MLPrimitives/issues/276) by @sarahmish
-        
-        ### Adapter Improvements
-        
-        * Building model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/MLPrimitives/issues/267) by @sarahmish
-        
-        ## 0.3.2 - 2021-11-09
-        
-        ### Adapter Improvements
-        
-        * Inferring data shapes with single dimension for keras adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
-        
-        ## 0.3.1 - 2021-10-07
-        
-        ### Adapter Improvements
-        
-        * Dynamic target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by @sarahmish
-        * Save keras primitives in Windows environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish
-        
-        ### General Imporvements
-        
-        * Update TensorFlow and NumPy dependency - [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish
-        
-        ## 0.3.0 - 2021-01-09
-        
-        ### New Primitives
-        
-        * Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish
-        * Add primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish
-        
-        ### Primitive Improvements
-        
-        * Add offset to rolling_window_sequence primitive - [Issue #251](https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz
-        * Rename the time_index column to time - [Issue #252](https://github.com/MLBazaar/MLPrimitives/issues/252) by @pvk-developer
-        * Update featuretools dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-developer
-        
-        ### General Improvements
-        
-        * Udpate dependencies and add python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala
-        * Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/244) by @csala
-        
-        ## 0.2.5 - 2020-07-29
-        
-        ### Primitive Improvements
-        
-        * Accept timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer
-        
-        ### Bug Fixes
-        
-        * ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer
-        
-        ### New Primitives
-        
-        * Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC
-        
-        ## 0.2.4 - 2020-01-30
-        
-        ### New Primitives
-        
-        * Add RangeScaler and RangeUnscaler primitives - [Issue #232](https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala
-        
-        ### Primitive Improvements
-        
-        * Extract input_shape from X in keras.Sequential - [Issue #223](https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala
-        
-        ### Bug Fixes
-        
-        * mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228](https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala
-        * Error when loading the reviews dataset - [Issue #230](https://github.com/MLBazaar/MLPrimitives/issues/230) by @csala
-        * Curate dependencies: specify an explicit prompt-toolkit version range - [Issue #224](https://github.com/MLBazaar/MLPrimitives/issues/224) by @csala
-        
-        ## 0.2.3 - 2019-11-14
-        
-        ### New Primitives
-        
-        * Add primitive to make window_sequences based on cutoff times - [Issue #217](https://github.com/MLBazaar/MLPrimitives/issues/217) by @csala
-        * Create a keras LSTM based TimeSeriesClassifier primitive - [Issue #218](https://github.com/MLBazaar/MLPrimitives/issues/218) by @csala
-        * Add pandas DataFrame primitives - [Issue #214](https://github.com/MLBazaar/MLPrimitives/issues/214) by @csala
-        * Add featuretools.EntitySet.normalize_entity primitive - [Issue #209](https://github.com/MLBazaar/MLPrimitives/issues/209) by @csala
-        
-        ### Primitive Improvements
-        
-        * Make featuretools.EntitySet.entity_from_dataframe entityset arg optional - [Issue #208](https://github.com/MLBazaar/MLPrimitives/issues/208) by @csala
-        
-        * Add text regression dataset - [Issue #206](https://github.com/MLBazaar/MLPrimitives/issues/206) by @csala
-        
-        ### Bug Fixes
-        
-        * pandas.DataFrame.resample crash when grouping by integer columns - [Issue #211](https://github.com/MLBazaar/MLPrimitives/issues/211) by @csala
-        
-        ## 0.2.2 - 2019-10-08
-        
-        ### New Primitives
-        
-        * Add primitives for GAN based time-series anomaly detection - [Issue #200](https://github.com/MLBazaar/MLPrimitives/issues/200) by @AlexanderGeiger
-        * Add `numpy.reshape` and `numpy.ravel` primitives - [Issue #197](https://github.com/MLBazaar/MLPrimitives/issues/197) by @AlexanderGeiger
-        * Add feature selection primitive based on Lasso - [Issue #194](https://github.com/MLBazaar/MLPrimitives/issues/194) by @csala
-        
-        ### Primitive Improvements
-        
-        * `feature_extraction.CategoricalEncoder` support dtype category - [Issue #196](https://github.com/MLBazaar/MLPrimitives/issues/196) by @csala
-        
-        ## 0.2.1 - 2019-09-09
-        
-        ### New Primitives
-        
-        * Timeseries Intervals to Mask Primitive - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
-        * Add new primitive: Arima model - [Issue #168](https://github.com/MLBazaar/MLPrimitives/issues/168) by @AlexanderGeiger
-        
-        ### Primitive Improvements
-        
-        * Curate PCA primitive hyperparameters - [Issue #190](https://github.com/MLBazaar/MLPrimitives/issues/190) by @AlexanderGeiger
-        * Add option to drop rolling window sequences - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
-        
-        ### Bug Fixes
-        
-        * scikit-image==0.14.3 crashes when installed on Mac - [Issue #188](https://github.com/MLBazaar/MLPrimitives/issues/188) by @csala
-        
-        ## 0.2.0
-        
-        ### New Features
-        
-        * Publish the pipelines as an `entry_point`
-        [Issue #175](https://github.com/MLBazaar/MLPrimitives/issues/175) by @csala
-        
-        ### Primitive Improvements
-        
-        * Improve pandas.DataFrame.resample primitive [Issue #177](https://github.com/MLBazaar/MLPrimitives/issues/177) by @csala
-        * Improve `feature_extractor` primitives [Issue #183](https://github.com/MLBazaar/MLPrimitives/issues/183) by @csala
-        * Improve `find_anomalies` primitive [Issue #180](https://github.com/MLBazaar/MLPrimitives/issues/180) by @AlexanderGeiger
-        
-        ### Bug Fixes
-        
-        * Typo in the primitive keras.Sequential.LSTMTimeSeriesRegressor [Issue #176](https://github.com/MLBazaar/MLPrimitives/issues/176) by @DanielCalvoCerezo
-        
-        
-        ## 0.1.10
-        
-        ### New Features
-        
-        * Add function to run primitives without a pipeline [Issue #43](https://github.com/MLBazaar/MLPrimitives/issues/43) by @csala
-        
-        ### New Pipelines
-        
-        * Add pipelines for all the MLBlocks examples [Issue #162](https://github.com/MLBazaar/MLPrimitives/issues/162) by @csala
-        
-        ### Primitive Improvements
-        
-        * Add Early Stopping to `keras.Sequential.LSTMTimeSeriesRegressor` primitive [Issue #156](https://github.com/MLBazaar/MLPrimitives/issues/156) by @csala
-        * Make FeatureExtractor primitives accept Numpy arrays [Issue #165](https://github.com/MLBazaar/MLPrimitives/issues/165) by @csala
-        * Add window size and pruning to the `timeseries_anomalies.find_anomalies` primitive [Issue #160](https://github.com/MLBazaar/MLPrimitives/issues/160) by @csala
-        
-        
-        ## 0.1.9
-        
-        ### New Features
-        
-        * Add a single table binary classification dataset [Issue #141](https://github.com/MLBazaar/MLPrimitives/issues/141) by @csala
-        
-        ### New Primitives
-        
-        * Add Multilayer Perceptron (MLP) primitive for binary classification [Issue #140](https://github.com/MLBazaar/MLPrimitives/issues/140) by @Hector-hedb12
-        * Add primitive for Sequence classification with LSTM [Issue #150](https://github.com/MLBazaar/MLPrimitives/issues/150) by @Hector-hedb12
-        * Add VGG-like convnet primitive [Issue #149](https://github.com/MLBazaar/MLPrimitives/issues/149) by @Hector-hedb12
-        * Add Multilayer Perceptron (MLP) primitive for multi-class softmax classification [Issue #139](https://github.com/MLBazaar/MLPrimitives/issues/139) by @Hector-hedb12
-        * Add primitive to count feature matrix columns [Issue #146](https://github.com/MLBazaar/MLPrimitives/issues/146) by @csala
-        
-        ### Primitive Improvements
-        
-        * Add additional fit and predict arguments to keras.Sequential [Issue #161](https://github.com/MLBazaar/MLPrimitives/issues/161) by @csala
-        * Add suport for keras.Sequential Callbacks [Issue #159](https://github.com/MLBazaar/MLPrimitives/issues/159) by @csala
-        * Add fixed hyperparam to control keras.Sequential verbosity [Issue #143](https://github.com/MLBazaar/MLPrimitives/issues/143) by @csala
-        
-        ## 0.1.8
-        
-        ### New Primitives
-        
-        * mlprimitives.custom.timeseries_preprocessing.time_segments_average - [Issue #137](https://github.com/MLBazaar/MLPrimitives/issues/137)
-        
-        ### New Features
-        
-        * Add target_index output in timseries_preprocessing.rolling_window_sequences - [Issue #136](https://github.com/MLBazaar/MLPrimitives/issues/136)
-        
-        ## 0.1.7
-        
-        ### General Improvements
-        
-        * Validate JSON format in `make lint` -  [Issue #133](https://github.com/MLBazaar/MLPrimitives/issues/133)
-        * Add demo datasets - [Issue #131](https://github.com/MLBazaar/MLPrimitives/issues/131)
-        * Improve featuretools.dfs primitive - [Issue #127](https://github.com/MLBazaar/MLPrimitives/issues/127)
-        
-        ### New Primitives
-        
-        * pandas.DataFrame.resample - [Issue #123](https://github.com/MLBazaar/MLPrimitives/issues/123)
-        * pandas.DataFrame.unstack - [Issue #124](https://github.com/MLBazaar/MLPrimitives/issues/124)
-        * featuretools.EntitySet.add_relationship - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
-        * featuretools.EntitySet.entity_from_dataframe - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
-        
-        ### Bug Fixes
-        
-        * Bug in timeseries_anomalies.py - [Issue #119](https://github.com/MLBazaar/MLPrimitives/issues/119)
-        
-        ## 0.1.6
-        
-        ### General Improvements
-        
-        * Add Contributing Documentation
-        * Remove upper bound in pandas version given new release of `featuretools` v0.6.1
-        * Improve LSTMTimeSeriesRegressor hyperparameters
-        
-        ### New Primitives
-        
-        * mlprimitives.candidates.dsp.SpectralMask
-        * mlprimitives.custom.timeseries_anomalies.find_anomalies
-        * mlprimitives.custom.timeseries_anomalies.regression_errors
-        * mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences
-        * mlprimitives.custom.timeseries_preprocessing.time_segments_average
-        * sklearn.linear_model.ElasticNet
-        * sklearn.linear_model.Lars
-        * sklearn.linear_model.Lasso
-        * sklearn.linear_model.MultiTaskLasso
-        * sklearn.linear_model.Ridge
-        
-        ## 0.1.5
-        
-        ### New Primitives
-        
-        * sklearn.impute.SimpleImputer
-        * sklearn.preprocessing.MinMaxScaler
-        * sklearn.preprocessing.MaxAbsScaler
-        * sklearn.preprocessing.RobustScaler
-        * sklearn.linear_model.LinearRegression
-        
-        ### General Improvements
-        
-        * Separate curated from candidate primitives
-        * Setup `entry_points` in setup.py to improve compaitibility with MLBlocks
-        * Add a test-pipelines command to test all the existing pipelines
-        * Clean sklearn example pipelines
-        * Change the `author` entry to a `contributors` list
-        * Change the name of `mlblocks_primitives` folder
-        * Pip install `requirements_dev.txt` fail documentation
-        
-        ### Bug Fixes
-        
-        * Fix LSTMTimeSeriesRegressor primitive. Issue #90
-        * Fix timeseries primitives. Issue #91
-        * Negative index anomalies in `timeseries_errors`. Issue #89
-        * Keep pandas version below 0.24.0. Issue #87
-        
-        ## 0.1.4
-        
-        ### New Primitives
-        
-        * mlprimitives.timeseries primitives for timeseries data preprocessing
-        * mlprimitives.timeseres_error primitives for timeseries anomaly detection
-        * keras.Sequential.LSTMTimeSeriesRegressor
-        * sklearn.neighbors.KNeighbors Classifier and Regressor
-        * several sklearn.decomposition primitives
-        * several sklearn.ensemble primitives
-        
-        ### Bug Fixes
-        
-        * Fix typo in mlprimitives.text.TextCleaner primitive
-        * Fix bug in index handling in featuretools.dfs primitive
-        * Fix bug in SingleLayerCNNImageClassifier annotation
-        * Remove old vlaidation tags from JSON annotations
-        
-        ## 0.1.3
-        
-        ### New Features
-        
-        * Fix and re-enable featuretools.dfs primitive.
-        
-        ## 0.1.2
-        
-        ### New Features
-        
-        * Add pipeline specification language and Evaluation utilities.
-        * Add pipelines for graph, text and tabular problems.
-        * New primitives ClassEncoder and ClassDecoder
-        * New primitives UniqueCounter and VocabularyCounter
-        
-        ### Bug Fixes
-        
-        * Fix TrivialPredictor bug when working with numpy arrays
-        * Change XGB default learning rate and number of estimators
-        
-        
-        ## 0.1.1
-        
-        ### New Features
-        
-        * Add more keras.applications primitives.
-        * Add a Text Cleanup primitive.
-        
-        ### Bug Fixes
-        
-        * Add keywords to `keras.preprocessing` primtives.
-        * Fix the `image_transform` method.
-        * Add `epoch` as a fixed hyperparameter for `keras.Sequential` primitives.
-        
-        ## 0.1.0
-        
-        * First release on PyPI.
-        
 Keywords: mlblocks mlprimitives pipelines primitives machine learning data science
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+<p align="left">
+  <a href="https://dai.lids.mit.edu">
+    <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
+  </a>
+  <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
+</p>
+
+[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+[![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)](https://pypi.python.org/pypi/mlprimitives)
+[![Tests](https://github.com/MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
+[![Downloads](https://pepy.tech/badge/mlprimitives)](https://pepy.tech/project/mlprimitives)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
+
+# MLPrimitives
+
+Pipelines and primitives for machine learning and data science.
+
+* Documentation: https://MLBazaar.github.io/MLPrimitives
+* Github: https://github.com/MLBazaar/MLPrimitives
+* License: [MIT](https://github.com/MLBazaar/MLPrimitives/blob/master/LICENSE)
+* Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+
+# Overview
+
+This repository contains primitive annotations to be used by the MLBlocks library, as well as
+the necessary Python code to make some of them fully compatible with the MLBlocks API requirements.
+
+There is also a collection of custom primitives contributed directly to this library, which either
+combine third party tools or implement new functionalities from scratch.
+
+## Why did we create this library?
+
+* Too many libraries in a fast growing field
+* Huge societal need to build machine learning apps
+* Domain expertise resides at several places (knowledge of math)
+* No documented information about hyperparameters, behavior...
+
+# Installation
+
+## Requirements
+
+**MLPrimitives** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+
+Also, although it is not strictly required, the usage of a
+[virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
+interfering with other software installed in the system where **MLPrimitives** is run.
+
+## Install with pip
+
+The easiest and recommended way to install **MLPrimitives** is using [pip](https://pip.pypa.io/en/stable/):
+
+```bash
+pip install mlprimitives
+```
+
+This will pull and install the latest stable release from [PyPi](https://pypi.org/).
+
+If you want to install from source or contribute to the project please read the
+[Contributing Guide](https://MLBazaar.github.io/MLPrimitives/community/welcome.html).
+
+# Quickstart
+
+This section is a short series of tutorials to help you getting started with MLPrimitives.
+
+In the following steps you will learn how to load and run a primitive on some data.
+
+Later on you will learn how to evaluate and improve the performance of a primitive by tuning
+its hyperparameters.
+
+## Running a Primitive
+
+In this first tutorial, we will be executing a single primitive for data transformation.
+
+### 1. Load a Primitive
+
+The first step in order to run a primitive is to load it.
+
+This will be done using the `mlprimitives.load_primitive` function, which will
+load the indicated primitive as an [MLBlock Object from MLBlocks](https://MLBazaar.github.io/MLBlocks/api/mlblocks.html#mlblocks.MLBlock)
+
+In this case, we will load the `mlprimitives.custom.feature_extraction.CategoricalEncoder`
+primitive.
+
+```python3
+from mlprimitives import load_primitive
+
+primitive = load_primitive('mlprimitives.custom.feature_extraction.CategoricalEncoder')
+```
+
+### 2. Load some data
+
+The CategoricalEncoder is a transformation primitive which applies one-hot encoding to all the
+categorical columns of a `pandas.DataFrame`.
+
+So, in order to be able to run our primitive, we will first load some data that contains
+categorical columns.
+
+This can be done with the `mlprimitives.datasets.load_census` function:
+
+```python3
+from mlprimitives.datasets import load_census
+
+dataset = load_census()
+```
+
+This dataset object has an attribute `data` which contains a table with several categorical
+columns.
+
+We can have a look at this table by executing `dataset.data.head()`, which will return a
+table like this:
+
+```
+                             0                    1                   2
+age                         39                   50                  38
+workclass            State-gov     Self-emp-not-inc             Private
+fnlwgt                   77516                83311              215646
+education            Bachelors            Bachelors             HS-grad
+education-num               13                   13                   9
+marital-status   Never-married   Married-civ-spouse            Divorced
+occupation        Adm-clerical      Exec-managerial   Handlers-cleaners
+relationship     Not-in-family              Husband       Not-in-family
+race                     White                White               White
+sex                       Male                 Male                Male
+capital-gain              2174                    0                   0
+capital-loss                 0                    0                   0
+hours-per-week              40                   13                  40
+native-country   United-States        United-States       United-States
+```
+
+### 3. Fit the primitive
+
+In order to run our pipeline, we first need to fit it.
+
+This is the process where it analyzes the data to detect which columns are categorical
+
+This is done by calling its `fit` method and assing the `dataset.data` as `X`.
+
+```python3
+primitive.fit(X=dataset.data)
+```
+
+### 4. Produce results
+
+Once the pipeline is fit, we can process the data by calling the `produce` method of the
+primitive instance and passing agin the `data` as `X`.
+
+```python3
+transformed = primitive.produce(X=dataset.data)
+```
+
+After this is done, we can see how the transformed data contains the newly generated
+one-hot vectors:
+
+```
+                                                0      1       2       3       4
+age                                            39     50      38      53      28
+fnlwgt                                      77516  83311  215646  234721  338409
+education-num                                  13     13       9       7      13
+capital-gain                                 2174      0       0       0       0
+capital-loss                                    0      0       0       0       0
+hours-per-week                                 40     13      40      40      40
+workclass= Private                              0      0       1       1       1
+workclass= Self-emp-not-inc                     0      1       0       0       0
+workclass= Local-gov                            0      0       0       0       0
+workclass= ?                                    0      0       0       0       0
+workclass= State-gov                            1      0       0       0       0
+workclass= Self-emp-inc                         0      0       0       0       0
+...                                             ...    ...     ...     ...     ...
+```
+
+## Tuning a Primitive
+
+In this short tutorial we will teach you how to evaluate the performance of a primitive
+and improve its performance by modifying its hyperparameters.
+
+To do so, we will load a primitive that can learn from the transformed data that we just
+generated and later on make predictions based on new data.
+
+### 1. Load another primitive
+
+Firs of all, we will load the `xgboost.XGBClassifier` primitive that we will use afterwards.
+
+```python3
+primitive = load_primitive('xgboost.XGBClassifier')
+```
+
+### 2. Split the dataset
+
+Before being able to evaluate the primitive perfomance, we need to split the data in two
+parts: train, which will be used for the primitive to learn, and test, which will be used
+to make the predictions that later on will be evaluated.
+
+In order to do this, we will get the first 75% of rows from the transformed data that we
+obtained above and call it `X_train`, and then set the next 25% of rows as `X_test`.
+
+```python3
+train_size = int(len(transformed) * 0.75)
+X_train = transformed.iloc[:train_size]
+X_test = transformed.iloc[train_size:]
+```
+
+Similarly, we need to obtain the `y_train` and `y_test` variables containing the corresponding
+output values.
+
+```python3
+y_train = dataset.target[:train_size]
+y_test = dataset.target[train_size:]
+```
+
+### 3. Fit the new primitive
+
+Once we have have splitted the data, we can fit the primitive by passing `X_train` and `y_train`
+to its `fit` method.
+
+```python3
+primitive.fit(X=X_train, y=y_train)
+```
+
+### 4. Make predictions
+
+Once the primitive has been fitted, we can produce predictions using the `X_test` data as input.
+
+```python3
+predictions = primitive.produce(X=X_test)
+```
+
+### 5. Evalute the performance
+
+We can now evaluate how good the predictions from our primitive are by using the `score`
+method from the `dataset` object on both the expected output and the real output from the
+primitive:
+
+```python3
+dataset.score(y_test, predictions)
+```
+
+This will output a float value between 0 and 1 indicating how good the predicitons are, being
+0 the worst score possible and 1 the best one.
+
+In this case we will obtain a score around 0.866
+
+### 6. Set new hyperparameter values
+
+In order to improve the performance of our primitive we will try to modify a couple of its
+hyperparameters.
+
+First we will see which hyperparameter values the primitive has by calling its
+`get_hyperparameters` method.
+
+```python3
+primitive.get_hyperparameters()
+```
+
+which will return a dictionary like this:
+
+```python
+{
+    "n_jobs": -1,
+    "n_estimators": 100,
+    "max_depth": 3,
+    "learning_rate": 0.1,
+    "gamma": 0,
+    "min_child_weight": 1
+}
+```
+
+Next, we will see which are the valid values for each one of those hyperparameters by calling its
+`get_tunable_hyperparameters` method:
+
+```python3
+primitive.get_tunable_hyperparameters()
+```
+
+For example, we will see that the `max_depth` hyperparameter has the following specification:
+
+```python
+{
+    "type": "int",
+    "default": 3,
+    "range": [
+        3,
+        10
+    ]
+}
+```
+
+Next, we will choose a valid value, for example 7, and set it into the pipeline using the
+`set_hyperparameters` method:
+
+```python3
+primitive.set_hyperparameters({'max_depth': 7})
+```
+
+### 7. Re-evaluate the performance
+
+Once the new hyperparameter value has been set, we repeat the fit/train/score cycle to
+evaluate the performance of this new hyperparameter value:
+
+```python3
+primitive.fit(X=X_train, y=y_train)
+predictions = primitive.produce(X=X_test)
+dataset.score(y_test, predictions)
+```
+
+This time we should see that the performance has improved to a value around 0.724
+
+## What's Next?
+
+Do you want to [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/getting_started/concepts.html),
+about [how to contribute to it](https://MLBazaar.github.io/MLPrimitives/community/contributing.html)
+or browse the [API Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
+Please check the corresponding sections of the [documentation](https://MLBazaar.github.io/MLPrimitives/)!
+
+
+# History
+
+## 0.3.5 - 2023-04-14
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #278](https://github.com/MLBazaar/MLPrimitives/issues/278) by @sarahmish
+
+## 0.3.4 - 2023-01-24
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #277](https://github.com/MLBazaar/MLPrimitives/issues/277) by @sarahmish
+
+## 0.3.3 - 2023-01-20
+
+### General Imporvements
+
+* Update dependencies - [Issue #276](https://github.com/MLBazaar/MLPrimitives/issues/276) by @sarahmish
+
+### Adapter Improvements
+
+* Building model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/MLPrimitives/issues/267) by @sarahmish
+
+## 0.3.2 - 2021-11-09
+
+### Adapter Improvements
+
+* Inferring data shapes with single dimension for keras adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
+
+## 0.3.1 - 2021-10-07
+
+### Adapter Improvements
+
+* Dynamic target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by @sarahmish
+* Save keras primitives in Windows environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish
+
+### General Imporvements
+
+* Update TensorFlow and NumPy dependency - [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish
+
+## 0.3.0 - 2021-01-09
+
+### New Primitives
+
+* Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish
+* Add primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish
+
+### Primitive Improvements
+
+* Add offset to rolling_window_sequence primitive - [Issue #251](https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz
+* Rename the time_index column to time - [Issue #252](https://github.com/MLBazaar/MLPrimitives/issues/252) by @pvk-developer
+* Update featuretools dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-developer
+
+### General Improvements
+
+* Udpate dependencies and add python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala
+* Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/244) by @csala
+
+## 0.2.5 - 2020-07-29
+
+### Primitive Improvements
+
+* Accept timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer
+
+### Bug Fixes
+
+* ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer
+
+### New Primitives
+
+* Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC
+
+## 0.2.4 - 2020-01-30
+
+### New Primitives
+
+* Add RangeScaler and RangeUnscaler primitives - [Issue #232](https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala
+
+### Primitive Improvements
+
+* Extract input_shape from X in keras.Sequential - [Issue #223](https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala
+
+### Bug Fixes
+
+* mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228](https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala
+* Error when loading the reviews dataset - [Issue #230](https://github.com/MLBazaar/MLPrimitives/issues/230) by @csala
+* Curate dependencies: specify an explicit prompt-toolkit version range - [Issue #224](https://github.com/MLBazaar/MLPrimitives/issues/224) by @csala
+
+## 0.2.3 - 2019-11-14
+
+### New Primitives
+
+* Add primitive to make window_sequences based on cutoff times - [Issue #217](https://github.com/MLBazaar/MLPrimitives/issues/217) by @csala
+* Create a keras LSTM based TimeSeriesClassifier primitive - [Issue #218](https://github.com/MLBazaar/MLPrimitives/issues/218) by @csala
+* Add pandas DataFrame primitives - [Issue #214](https://github.com/MLBazaar/MLPrimitives/issues/214) by @csala
+* Add featuretools.EntitySet.normalize_entity primitive - [Issue #209](https://github.com/MLBazaar/MLPrimitives/issues/209) by @csala
+
+### Primitive Improvements
+
+* Make featuretools.EntitySet.entity_from_dataframe entityset arg optional - [Issue #208](https://github.com/MLBazaar/MLPrimitives/issues/208) by @csala
+
+* Add text regression dataset - [Issue #206](https://github.com/MLBazaar/MLPrimitives/issues/206) by @csala
+
+### Bug Fixes
+
+* pandas.DataFrame.resample crash when grouping by integer columns - [Issue #211](https://github.com/MLBazaar/MLPrimitives/issues/211) by @csala
+
+## 0.2.2 - 2019-10-08
+
+### New Primitives
+
+* Add primitives for GAN based time-series anomaly detection - [Issue #200](https://github.com/MLBazaar/MLPrimitives/issues/200) by @AlexanderGeiger
+* Add `numpy.reshape` and `numpy.ravel` primitives - [Issue #197](https://github.com/MLBazaar/MLPrimitives/issues/197) by @AlexanderGeiger
+* Add feature selection primitive based on Lasso - [Issue #194](https://github.com/MLBazaar/MLPrimitives/issues/194) by @csala
+
+### Primitive Improvements
+
+* `feature_extraction.CategoricalEncoder` support dtype category - [Issue #196](https://github.com/MLBazaar/MLPrimitives/issues/196) by @csala
+
+## 0.2.1 - 2019-09-09
+
+### New Primitives
+
+* Timeseries Intervals to Mask Primitive - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
+* Add new primitive: Arima model - [Issue #168](https://github.com/MLBazaar/MLPrimitives/issues/168) by @AlexanderGeiger
+
+### Primitive Improvements
+
+* Curate PCA primitive hyperparameters - [Issue #190](https://github.com/MLBazaar/MLPrimitives/issues/190) by @AlexanderGeiger
+* Add option to drop rolling window sequences - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
+
+### Bug Fixes
+
+* scikit-image==0.14.3 crashes when installed on Mac - [Issue #188](https://github.com/MLBazaar/MLPrimitives/issues/188) by @csala
+
+## 0.2.0
+
+### New Features
+
+* Publish the pipelines as an `entry_point`
+[Issue #175](https://github.com/MLBazaar/MLPrimitives/issues/175) by @csala
+
+### Primitive Improvements
+
+* Improve pandas.DataFrame.resample primitive [Issue #177](https://github.com/MLBazaar/MLPrimitives/issues/177) by @csala
+* Improve `feature_extractor` primitives [Issue #183](https://github.com/MLBazaar/MLPrimitives/issues/183) by @csala
+* Improve `find_anomalies` primitive [Issue #180](https://github.com/MLBazaar/MLPrimitives/issues/180) by @AlexanderGeiger
+
+### Bug Fixes
+
+* Typo in the primitive keras.Sequential.LSTMTimeSeriesRegressor [Issue #176](https://github.com/MLBazaar/MLPrimitives/issues/176) by @DanielCalvoCerezo
+
+
+## 0.1.10
+
+### New Features
+
+* Add function to run primitives without a pipeline [Issue #43](https://github.com/MLBazaar/MLPrimitives/issues/43) by @csala
+
+### New Pipelines
+
+* Add pipelines for all the MLBlocks examples [Issue #162](https://github.com/MLBazaar/MLPrimitives/issues/162) by @csala
+
+### Primitive Improvements
+
+* Add Early Stopping to `keras.Sequential.LSTMTimeSeriesRegressor` primitive [Issue #156](https://github.com/MLBazaar/MLPrimitives/issues/156) by @csala
+* Make FeatureExtractor primitives accept Numpy arrays [Issue #165](https://github.com/MLBazaar/MLPrimitives/issues/165) by @csala
+* Add window size and pruning to the `timeseries_anomalies.find_anomalies` primitive [Issue #160](https://github.com/MLBazaar/MLPrimitives/issues/160) by @csala
+
+
+## 0.1.9
+
+### New Features
+
+* Add a single table binary classification dataset [Issue #141](https://github.com/MLBazaar/MLPrimitives/issues/141) by @csala
+
+### New Primitives
+
+* Add Multilayer Perceptron (MLP) primitive for binary classification [Issue #140](https://github.com/MLBazaar/MLPrimitives/issues/140) by @Hector-hedb12
+* Add primitive for Sequence classification with LSTM [Issue #150](https://github.com/MLBazaar/MLPrimitives/issues/150) by @Hector-hedb12
+* Add VGG-like convnet primitive [Issue #149](https://github.com/MLBazaar/MLPrimitives/issues/149) by @Hector-hedb12
+* Add Multilayer Perceptron (MLP) primitive for multi-class softmax classification [Issue #139](https://github.com/MLBazaar/MLPrimitives/issues/139) by @Hector-hedb12
+* Add primitive to count feature matrix columns [Issue #146](https://github.com/MLBazaar/MLPrimitives/issues/146) by @csala
+
+### Primitive Improvements
+
+* Add additional fit and predict arguments to keras.Sequential [Issue #161](https://github.com/MLBazaar/MLPrimitives/issues/161) by @csala
+* Add suport for keras.Sequential Callbacks [Issue #159](https://github.com/MLBazaar/MLPrimitives/issues/159) by @csala
+* Add fixed hyperparam to control keras.Sequential verbosity [Issue #143](https://github.com/MLBazaar/MLPrimitives/issues/143) by @csala
+
+## 0.1.8
+
+### New Primitives
+
+* mlprimitives.custom.timeseries_preprocessing.time_segments_average - [Issue #137](https://github.com/MLBazaar/MLPrimitives/issues/137)
+
+### New Features
+
+* Add target_index output in timseries_preprocessing.rolling_window_sequences - [Issue #136](https://github.com/MLBazaar/MLPrimitives/issues/136)
+
+## 0.1.7
+
+### General Improvements
+
+* Validate JSON format in `make lint` -  [Issue #133](https://github.com/MLBazaar/MLPrimitives/issues/133)
+* Add demo datasets - [Issue #131](https://github.com/MLBazaar/MLPrimitives/issues/131)
+* Improve featuretools.dfs primitive - [Issue #127](https://github.com/MLBazaar/MLPrimitives/issues/127)
+
+### New Primitives
+
+* pandas.DataFrame.resample - [Issue #123](https://github.com/MLBazaar/MLPrimitives/issues/123)
+* pandas.DataFrame.unstack - [Issue #124](https://github.com/MLBazaar/MLPrimitives/issues/124)
+* featuretools.EntitySet.add_relationship - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
+* featuretools.EntitySet.entity_from_dataframe - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
+
+### Bug Fixes
+
+* Bug in timeseries_anomalies.py - [Issue #119](https://github.com/MLBazaar/MLPrimitives/issues/119)
+
+## 0.1.6
+
+### General Improvements
+
+* Add Contributing Documentation
+* Remove upper bound in pandas version given new release of `featuretools` v0.6.1
+* Improve LSTMTimeSeriesRegressor hyperparameters
+
+### New Primitives
+
+* mlprimitives.candidates.dsp.SpectralMask
+* mlprimitives.custom.timeseries_anomalies.find_anomalies
+* mlprimitives.custom.timeseries_anomalies.regression_errors
+* mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences
+* mlprimitives.custom.timeseries_preprocessing.time_segments_average
+* sklearn.linear_model.ElasticNet
+* sklearn.linear_model.Lars
+* sklearn.linear_model.Lasso
+* sklearn.linear_model.MultiTaskLasso
+* sklearn.linear_model.Ridge
+
+## 0.1.5
+
+### New Primitives
+
+* sklearn.impute.SimpleImputer
+* sklearn.preprocessing.MinMaxScaler
+* sklearn.preprocessing.MaxAbsScaler
+* sklearn.preprocessing.RobustScaler
+* sklearn.linear_model.LinearRegression
+
+### General Improvements
+
+* Separate curated from candidate primitives
+* Setup `entry_points` in setup.py to improve compaitibility with MLBlocks
+* Add a test-pipelines command to test all the existing pipelines
+* Clean sklearn example pipelines
+* Change the `author` entry to a `contributors` list
+* Change the name of `mlblocks_primitives` folder
+* Pip install `requirements_dev.txt` fail documentation
+
+### Bug Fixes
+
+* Fix LSTMTimeSeriesRegressor primitive. Issue #90
+* Fix timeseries primitives. Issue #91
+* Negative index anomalies in `timeseries_errors`. Issue #89
+* Keep pandas version below 0.24.0. Issue #87
+
+## 0.1.4
+
+### New Primitives
+
+* mlprimitives.timeseries primitives for timeseries data preprocessing
+* mlprimitives.timeseres_error primitives for timeseries anomaly detection
+* keras.Sequential.LSTMTimeSeriesRegressor
+* sklearn.neighbors.KNeighbors Classifier and Regressor
+* several sklearn.decomposition primitives
+* several sklearn.ensemble primitives
+
+### Bug Fixes
+
+* Fix typo in mlprimitives.text.TextCleaner primitive
+* Fix bug in index handling in featuretools.dfs primitive
+* Fix bug in SingleLayerCNNImageClassifier annotation
+* Remove old vlaidation tags from JSON annotations
+
+## 0.1.3
+
+### New Features
+
+* Fix and re-enable featuretools.dfs primitive.
+
+## 0.1.2
+
+### New Features
+
+* Add pipeline specification language and Evaluation utilities.
+* Add pipelines for graph, text and tabular problems.
+* New primitives ClassEncoder and ClassDecoder
+* New primitives UniqueCounter and VocabularyCounter
+
+### Bug Fixes
+
+* Fix TrivialPredictor bug when working with numpy arrays
+* Change XGB default learning rate and number of estimators
+
+
+## 0.1.1
+
+### New Features
+
+* Add more keras.applications primitives.
+* Add a Text Cleanup primitive.
+
+### Bug Fixes
+
+* Add keywords to `keras.preprocessing` primtives.
+* Fix the `image_transform` method.
+* Add `epoch` as a fixed hyperparameter for `keras.Sequential` primitives.
+
+## 0.1.0
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,11 +1,19 @@
-Metadata-Version: 2.1 Name: mlprimitives Version: 0.3.4.dev0 Summary: Pipelines
-and primitives for machine learning and data science. Home-page: https://
+Metadata-Version: 2.1 Name: mlprimitives Version: 0.3.5 Summary: Pipelines and
+primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLPrimitives Author: MIT Data To AI Lab Author-email:
-dailabmit@gmail.com License: MIT license Description:
+dailabmit@gmail.com License: MIT license Keywords: mlblocks mlprimitives
+pipelines primitives machine learning data science Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+dev License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)]
 (https://pypi.python.org/pypi/mlprimitives) [![Tests](https://github.com/
 MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/
 MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
@@ -125,46 +133,51 @@
 dataset.score(y_test, predictions) ``` This time we should see that the
 performance has improved to a value around 0.724 ## What's Next? Do you want to
 [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/
 getting_started/concepts.html), about [how to contribute to it](https://
 MLBazaar.github.io/MLPrimitives/community/contributing.html) or browse the [API
 Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
 Please check the corresponding sections of the [documentation](https://
-MLBazaar.github.io/MLPrimitives/)! # History ## 0.3.3 - 2023-01-20 ### General
-Imporvements * Update dependencies - [Issue #276](https://github.com/MLBazaar/
-MLPrimitives/issues/276) by @sarahmish ### Adapter Improvements * Building
-model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/
-MLPrimitives/issues/267) by @sarahmish ## 0.3.2 - 2021-11-09 ### Adapter
-Improvements * Inferring data shapes with single dimension for keras adapter -
-[Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
-## 0.3.1 - 2021-10-07 ### Adapter Improvements * Dynamic target_shape in keras
-adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by
-@sarahmish * Save keras primitives in Windows environment - [Issue #261](https:
-//github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish ### General
-Imporvements * Update TensorFlow and NumPy dependency - [Issue #259](https://
-github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish ## 0.3.0 - 2021-01-
-09 ### New Primitives * Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue
-#242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish * Add
-primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://
-github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish ### Primitive
-Improvements * Add offset to rolling_window_sequence primitive - [Issue #251]
-(https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz *
-Rename the time_index column to time - [Issue #252](https://github.com/
-MLBazaar/MLPrimitives/issues/252) by @pvk-developer * Update featuretools
-dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250)
-by @pvk-developer ### General Improvements * Udpate dependencies and add
-python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246)
-by @csala * Drop Python35 - [Issue #244](https://github.com/MLBazaar/
-MLPrimitives/issues/244) by @csala ## 0.2.5 - 2020-07-29 ### Primitive
-Improvements * Accept timedelta `window_size` in `cutoff_window_sequences` -
-[Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by
-@joanvaquer ### Bug Fixes * ImportError: Keras requires TensorFlow 2.2 or
-higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://
-github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer ### New Primitives
-* Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/
+MLBazaar.github.io/MLPrimitives/)! # History ## 0.3.5 - 2023-04-14 ### General
+Imporvements * Update `mlblocks` cap - [Issue #278](https://github.com/
+MLBazaar/MLPrimitives/issues/278) by @sarahmish ## 0.3.4 - 2023-01-24 ###
+General Imporvements * Update `mlblocks` cap - [Issue #277](https://github.com/
+MLBazaar/MLPrimitives/issues/277) by @sarahmish ## 0.3.3 - 2023-01-20 ###
+General Imporvements * Update dependencies - [Issue #276](https://github.com/
+MLBazaar/MLPrimitives/issues/276) by @sarahmish ### Adapter Improvements *
+Building model within fit in keras adapter- [Issue #267](https://github.com/
+MLBazaar/MLPrimitives/issues/267) by @sarahmish ## 0.3.2 - 2021-11-09 ###
+Adapter Improvements * Inferring data shapes with single dimension for keras
+adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by
+@sarahmish ## 0.3.1 - 2021-10-07 ### Adapter Improvements * Dynamic
+target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/
+MLPrimitives/issues/263) by @sarahmish * Save keras primitives in Windows
+environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261)
+by @sarahmish ### General Imporvements * Update TensorFlow and NumPy dependency
+- [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by
+@sarahmish ## 0.3.0 - 2021-01-09 ### New Primitives * Add primitive
+`sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/
+MLPrimitives/issues/242) by @sarahmish * Add primitive
+`sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/
+MLBazaar/MLPrimitives/issues/241) by @sarahmish ### Primitive Improvements *
+Add offset to rolling_window_sequence primitive - [Issue #251](https://
+github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz * Rename the
+time_index column to time - [Issue #252](https://github.com/MLBazaar/
+MLPrimitives/issues/252) by @pvk-developer * Update featuretools dependency -
+[Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-
+developer ### General Improvements * Udpate dependencies and add python3.8 -
+[Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala *
+Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/
+244) by @csala ## 0.2.5 - 2020-07-29 ### Primitive Improvements * Accept
+timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://
+github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer ### Bug Fixes *
+ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via
+`pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/
+MLPrimitives/issues/237) by @joanvaquer ### New Primitives * Add
+`pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/
 MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC ## 0.2.4 - 2020-01-30 ###
 New Primitives * Add RangeScaler and RangeUnscaler primitives - [Issue #232]
 (https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala ### Primitive
 Improvements * Extract input_shape from X in keras.Sequential - [Issue #223]
 (https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala ### Bug Fixes *
 mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228]
 (https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala * Error when
@@ -291,16 +304,8 @@
 pipelines for graph, text and tabular problems. * New primitives ClassEncoder
 and ClassDecoder * New primitives UniqueCounter and VocabularyCounter ### Bug
 Fixes * Fix TrivialPredictor bug when working with numpy arrays * Change XGB
 default learning rate and number of estimators ## 0.1.1 ### New Features * Add
 more keras.applications primitives. * Add a Text Cleanup primitive. ### Bug
 Fixes * Add keywords to `keras.preprocessing` primtives. * Fix the
 `image_transform` method. * Add `epoch` as a fixed hyperparameter for
-`keras.Sequential` primitives. ## 0.1.0 * First release on PyPI. Keywords:
-mlblocks mlprimitives pipelines primitives machine learning data science
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev
+`keras.Sequential` primitives. ## 0.1.0 * First release on PyPI.
```

### Comparing `mlprimitives-0.3.4.dev0/LICENSE` & `mlprimitives-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/CONTRIBUTING.rst` & `mlprimitives-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/HISTORY.md` & `mlprimitives-0.3.5/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # History
 
+## 0.3.5 - 2023-04-14
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #278](https://github.com/MLBazaar/MLPrimitives/issues/278) by @sarahmish
+
+## 0.3.4 - 2023-01-24
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #277](https://github.com/MLBazaar/MLPrimitives/issues/277) by @sarahmish
+
 ## 0.3.3 - 2023-01-20
 
 ### General Imporvements
 
 * Update dependencies - [Issue #276](https://github.com/MLBazaar/MLPrimitives/issues/276) by @sarahmish
 
 ### Adapter Improvements
```

### Comparing `mlprimitives-0.3.4.dev0/tests/primitives/test_primitives.py` & `mlprimitives-0.3.5/tests/primitives/test_primitives.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/adapters/test_statsmodels.py` & `mlprimitives-0.3.5/tests/adapters/test_statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/adapters/test_keras.py` & `mlprimitives-0.3.5/tests/adapters/test_keras.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/adapters/test_pandas.py` & `mlprimitives-0.3.5/tests/adapters/test_pandas.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/custom/test_timeseries_preprocessing.py` & `mlprimitives-0.3.5/tests/custom/test_timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/custom/test_preprocessing.py` & `mlprimitives-0.3.5/tests/custom/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/custom/test_text.py` & `mlprimitives-0.3.5/tests/custom/test_text.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/custom/test_timeseries_anomalies.py` & `mlprimitives-0.3.5/tests/custom/test_timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/tests/custom/test_feature_extraction.py` & `mlprimitives-0.3.5/tests/custom/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/index.rst` & `mlprimitives-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/Makefile` & `mlprimitives-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/conf.py` & `mlprimitives-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/make.bat` & `mlprimitives-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/community/custom.rst` & `mlprimitives-0.3.5/docs/community/custom.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/community/annotations.rst` & `mlprimitives-0.3.5/docs/community/annotations.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/community/contributing.rst` & `mlprimitives-0.3.5/docs/community/contributing.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/community/adapters.rst` & `mlprimitives-0.3.5/docs/community/adapters.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/community/welcome.rst` & `mlprimitives-0.3.5/docs/community/welcome.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/docs/getting_started/concepts.rst` & `mlprimitives-0.3.5/docs/getting_started/concepts.rst`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/README.md` & `mlprimitives-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/setup.py` & `mlprimitives-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 install_requires = [
     'Keras>=2.4,<2.5',
     'featuretools>=0.6.1,<0.23',
     'iso639>=0.1.4,<0.2',
     'langdetect>=1.0.7,<2',
     'lightfm>=1.15,<2',
-    'mlblocks>=0.4.0.dev0,<0.6',
+    'mlblocks>=0.4.0.dev0,<0.7',
     'networkx>=2.0,<3',
     'nltk>=3.3,<4',
     'numpy<1.21.0,>=1.16.0',
     'opencv-python>=3.4.0.12,<4.7',
     'pandas>=1,<2',
     'python-louvain>=0.10,<0.14',   # community
     'scikit-image>=0.15',
@@ -118,10 +118,10 @@
     name='mlprimitives',
     packages=find_packages(include=['mlprimitives', 'mlprimitives.*']),
     python_requires='>=3.6,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/MLBazaar/MLPrimitives',
-    version='0.3.4.dev0',
+    version='0.3.5',
     zip_safe=False,
 )
```

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/candidates/dsp.py` & `mlprimitives-0.3.5/mlprimitives/candidates/dsp.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/candidates/audio_featurization.py` & `mlprimitives-0.3.5/mlprimitives/candidates/audio_featurization.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/candidates/timeseries/cyclegan.py` & `mlprimitives-0.3.5/mlprimitives/candidates/timeseries/cyclegan.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/candidates/audio_padding.py` & `mlprimitives-0.3.5/mlprimitives/candidates/audio_padding.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/evaluation.py` & `mlprimitives-0.3.5/mlprimitives/evaluation.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/datasets.py` & `mlprimitives-0.3.5/mlprimitives/datasets.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.feature_selection.LassoFeatureSelector.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.feature_selection.LassoFeatureSelector.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.LSTMTextClassifier.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.LSTMTextClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/text.classification.lstm.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/text.classification.lstm.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.LSTMBinaryTextClassifier.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.LSTMBinaryTextClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageClassifier.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.SingleLayerCNNImageClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.classification.text.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/single_table.classification.text.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.MLPMultiClassClassifier.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.MLPMultiClassClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/graph.link_prediction.nx.xgb.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/graph.link_prediction.nx.xgb.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/graph.graph_matching.nx.xgb.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/graph.graph_matching.nx.xgb.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/mlprimitives.custom.text.TextCleaner.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/mlprimitives.custom.text.TextCleaner.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/keras.Sequential.VGGCNNClassifier.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/keras.Sequential.VGGCNNClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/single_table.classification.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/single_table.classification.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/pipelines/multi_table.classification.dfs.xgb.json` & `mlprimitives-0.3.5/mlprimitives/pipelines/multi_table.classification.dfs.xgb.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Lars.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Lars.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.LassoFeatureSelector.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.LassoFeatureSelector.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTextClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTextClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.GradientBoostingRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.GradientBoostingRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.select_dtypes.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.select_dtypes.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.pop.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.pop.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.resnet50.ResNet50.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.resnet50.ResNet50.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Lasso.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Lasso.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.RobustScaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.RobustScaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.VocabularyCounter.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.VocabularyCounter.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.mobilenet.MobileNet.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.mobilenet.MobileNet.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.entity_from_dataframe.json` & `mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.entity_from_dataframe.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.SGDClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.SGDClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.preprocess_input.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.preprocess_input.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.filter.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.filter.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.xception.Xception.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.xception.Xception.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/statsmodels.tsa.arima_model.Arima.json` & `mlprimitives-0.3.5/mlprimitives/primitives/statsmodels.tsa.arima_model.Arima.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.MLPBinaryClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.MLPBinaryClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.CategoricalEncoder.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.CategoricalEncoder.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/community.CommunityBestPartition.json` & `mlprimitives-0.3.5/mlprimitives/primitives/community.CommunityBestPartition.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.DatetimeFeaturizer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.dfs.json` & `mlprimitives-0.3.5/mlprimitives/primitives/featuretools.dfs.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.score_anomalies.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.score_anomalies.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMBinaryTextClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMBinaryTextClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.drop_duplicates.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.drop_duplicates.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/lightfm.LightFM.json` & `mlprimitives-0.3.5/mlprimitives/primitives/lightfm.LightFM.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.inception_v3.InceptionV3.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.inception_v3.InceptionV3.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier_proba.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier_proba.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.StandardScaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.StandardScaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.find_anomalies.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.find_anomalies.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.trivial.TrivialPredictor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.trivial.TrivialPredictor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.Series.filter.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.Series.filter.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.set_index.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.set_index.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/skimage.feature.hog.json` & `mlprimitives-0.3.5/mlprimitives/primitives/skimage.feature.hog.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.resnet50.preprocess_input.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.resnet50.preprocess_input.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/xgboost.XGBRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/xgboost.XGBRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/networkx.graph_feature_extraction.json` & `mlprimitives-0.3.5/mlprimitives/primitives/networkx.graph_feature_extraction.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.naive_bayes.MultinomialNB.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.naive_bayes.MultinomialNB.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_extraction.StringVectorizer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_extraction.StringVectorizer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.to_numpy.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.to_numpy.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.ravel.json` & `mlprimitives-0.3.5/mlprimitives/primitives/numpy.ravel.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassDecoder.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassDecoder.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.ExtraTreesRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.ExtraTreesRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.Ridge.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.Ridge.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/cv2.GaussianBlur.json` & `mlprimitives-0.3.5/mlprimitives/primitives/cv2.GaussianBlur.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet201.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet201.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/xgboost.XGBClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/xgboost.XGBClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.MinMaxScaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.MinMaxScaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.add_relationship.json` & `mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.add_relationship.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet169.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet169.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.FastICA.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.FastICA.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/networkx.link_prediction_feature_extraction.json` & `mlprimitives-0.3.5/mlprimitives/primitives/networkx.link_prediction_feature_extraction.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.impute.SimpleImputer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.impute.SimpleImputer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.SingleLayerCNNImageRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.CycleGAN.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.timeseries.cyclegan.CycleGAN.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.append.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.append.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.BaggingClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.BaggingClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.AdaBoostClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.AdaBoostClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.reshape.json` & `mlprimitives-0.3.5/mlprimitives/primitives/numpy.reshape.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.mobilenet.preprocess_input.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.mobilenet.preprocess_input.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.LinearRegression.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.LinearRegression.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.inception_v3.preprocess_input.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.inception_v3.preprocess_input.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.count_features.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.count_features.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/numpy.argmax.json` & `mlprimitives-0.3.5/mlprimitives/primitives/numpy.argmax.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesRegressorFeatureSelector.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomTreesEmbedding.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomTreesEmbedding.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeScaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeScaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.MLPMultiClassClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.MLPMultiClassClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.DictionaryLearning.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.DictionaryLearning.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.TruncatedSVD.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.TruncatedSVD.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.Imputer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.Imputer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier_proba.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.neighbors.KNeighborsClassifier_proba.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.FactorAnalysis.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.FactorAnalysis.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.dropna.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.dropna.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.regression_errors.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_anomalies.regression_errors.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.feature_selection.ExtraTreesClassifierFeatureSelector.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.RandomForestClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.preprocessing.sequence.pad_sequences.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.preprocessing.sequence.pad_sequences.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.GradientBoostingClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.GradientBoostingClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.IsolationForest.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.IsolationForest.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.LogisticRegression.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.LogisticRegression.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.dsp.SpectralMask.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.dsp.SpectralMask.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTextRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTextRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.MaxAbsScaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.MaxAbsScaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.feature_extraction.text.CountVectorizer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.feature_extraction.text.CountVectorizer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.densenet.DenseNet121.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.densenet.DenseNet121.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.drop.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.drop.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.ElasticNet.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.ElasticNet.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.AdaBoostRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.AdaBoostRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.BaggingRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.BaggingRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.text.TextCleaner.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.text.TextCleaner.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.audio_padding.AudioPadder.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.audio_padding.AudioPadder.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.VGGCNNClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.VGGCNNClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.intervals_to_mask.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.intervals_to_mask.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.preprocessing.OneHotEncoder.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.preprocessing.OneHotEncoder.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.naive_bayes.GaussianNB.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.naive_bayes.GaussianNB.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.KernelPCA.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.KernelPCA.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.counters.UniqueCounter.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.counters.UniqueCounter.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.decomposition.PCA.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.decomposition.PCA.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeUnscaler.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.RangeUnscaler.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.candidates.audio_featurization.featurize_audio.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.candidates.audio_featurization.featurize_audio.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.join.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.join.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.linear_model.MultiTaskLasso.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.linear_model.MultiTaskLasso.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.resample.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.resample.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.unstack.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.unstack.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.preprocessing.text.Tokenizer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.preprocessing.text.Tokenizer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_average.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_average.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/featuretools.EntitySet.normalize_entity.json` & `mlprimitives-0.3.5/mlprimitives/primitives/featuretools.EntitySet.normalize_entity.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.set.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.set.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.fillna.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.fillna.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.feature_extraction.text.TfidfTransformer.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.feature_extraction.text.TfidfTransformer.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassEncoder.json` & `mlprimitives-0.3.5/mlprimitives/primitives/mlprimitives.custom.preprocessing.ClassEncoder.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/sklearn.ensemble.ExtraTreesClassifier.json` & `mlprimitives-0.3.5/mlprimitives/primitives/sklearn.ensemble.ExtraTreesClassifier.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/pandas.DataFrame.get.json` & `mlprimitives-0.3.5/mlprimitives/primitives/pandas.DataFrame.get.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/primitives/keras.applications.xception.preprocess_input.json` & `mlprimitives-0.3.5/mlprimitives/primitives/keras.applications.xception.preprocess_input.json`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/lightfm.py` & `mlprimitives-0.3.5/mlprimitives/adapters/lightfm.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/pandas.py` & `mlprimitives-0.3.5/mlprimitives/adapters/pandas.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/keras.py` & `mlprimitives-0.3.5/mlprimitives/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/featuretools.py` & `mlprimitives-0.3.5/mlprimitives/adapters/featuretools.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/skimage.py` & `mlprimitives-0.3.5/mlprimitives/adapters/skimage.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/community.py` & `mlprimitives-0.3.5/mlprimitives/adapters/community.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/statsmodels.py` & `mlprimitives-0.3.5/mlprimitives/adapters/statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/cv2.py` & `mlprimitives-0.3.5/mlprimitives/adapters/cv2.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/adapters/networkx.py` & `mlprimitives-0.3.5/mlprimitives/adapters/networkx.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/cli.py` & `mlprimitives-0.3.5/mlprimitives/cli.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/utils.py` & `mlprimitives-0.3.5/mlprimitives/utils.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/counters.py` & `mlprimitives-0.3.5/mlprimitives/custom/counters.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/timeseries_anomalies.py` & `mlprimitives-0.3.5/mlprimitives/custom/timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/trivial.py` & `mlprimitives-0.3.5/mlprimitives/custom/trivial.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/feature_selection.py` & `mlprimitives-0.3.5/mlprimitives/custom/feature_selection.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/feature_extraction.py` & `mlprimitives-0.3.5/mlprimitives/custom/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/preprocessing.py` & `mlprimitives-0.3.5/mlprimitives/custom/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/text.py` & `mlprimitives-0.3.5/mlprimitives/custom/text.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives/custom/timeseries_preprocessing.py` & `mlprimitives-0.3.5/mlprimitives/custom/timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/setup.cfg` & `mlprimitives-0.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.4.dev0
+current_version = 0.3.5
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives.egg-info/PKG-INFO` & `mlprimitives-0.3.5/mlprimitives.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,648 +1,661 @@
 Metadata-Version: 2.1
 Name: mlprimitives
-Version: 0.3.4.dev0
+Version: 0.3.5
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLPrimitives
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
-Description: <p align="left">
-          <a href="https://dai.lids.mit.edu">
-            <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
-          </a>
-          <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
-        </p>
-        
-        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        [![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)](https://pypi.python.org/pypi/mlprimitives)
-        [![Tests](https://github.com/MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
-        [![Downloads](https://pepy.tech/badge/mlprimitives)](https://pepy.tech/project/mlprimitives)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
-        
-        # MLPrimitives
-        
-        Pipelines and primitives for machine learning and data science.
-        
-        * Documentation: https://MLBazaar.github.io/MLPrimitives
-        * Github: https://github.com/MLBazaar/MLPrimitives
-        * License: [MIT](https://github.com/MLBazaar/MLPrimitives/blob/master/LICENSE)
-        * Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        
-        # Overview
-        
-        This repository contains primitive annotations to be used by the MLBlocks library, as well as
-        the necessary Python code to make some of them fully compatible with the MLBlocks API requirements.
-        
-        There is also a collection of custom primitives contributed directly to this library, which either
-        combine third party tools or implement new functionalities from scratch.
-        
-        ## Why did we create this library?
-        
-        * Too many libraries in a fast growing field
-        * Huge societal need to build machine learning apps
-        * Domain expertise resides at several places (knowledge of math)
-        * No documented information about hyperparameters, behavior...
-        
-        # Installation
-        
-        ## Requirements
-        
-        **MLPrimitives** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
-        
-        Also, although it is not strictly required, the usage of a
-        [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
-        interfering with other software installed in the system where **MLPrimitives** is run.
-        
-        ## Install with pip
-        
-        The easiest and recommended way to install **MLPrimitives** is using [pip](https://pip.pypa.io/en/stable/):
-        
-        ```bash
-        pip install mlprimitives
-        ```
-        
-        This will pull and install the latest stable release from [PyPi](https://pypi.org/).
-        
-        If you want to install from source or contribute to the project please read the
-        [Contributing Guide](https://MLBazaar.github.io/MLPrimitives/community/welcome.html).
-        
-        # Quickstart
-        
-        This section is a short series of tutorials to help you getting started with MLPrimitives.
-        
-        In the following steps you will learn how to load and run a primitive on some data.
-        
-        Later on you will learn how to evaluate and improve the performance of a primitive by tuning
-        its hyperparameters.
-        
-        ## Running a Primitive
-        
-        In this first tutorial, we will be executing a single primitive for data transformation.
-        
-        ### 1. Load a Primitive
-        
-        The first step in order to run a primitive is to load it.
-        
-        This will be done using the `mlprimitives.load_primitive` function, which will
-        load the indicated primitive as an [MLBlock Object from MLBlocks](https://MLBazaar.github.io/MLBlocks/api/mlblocks.html#mlblocks.MLBlock)
-        
-        In this case, we will load the `mlprimitives.custom.feature_extraction.CategoricalEncoder`
-        primitive.
-        
-        ```python3
-        from mlprimitives import load_primitive
-        
-        primitive = load_primitive('mlprimitives.custom.feature_extraction.CategoricalEncoder')
-        ```
-        
-        ### 2. Load some data
-        
-        The CategoricalEncoder is a transformation primitive which applies one-hot encoding to all the
-        categorical columns of a `pandas.DataFrame`.
-        
-        So, in order to be able to run our primitive, we will first load some data that contains
-        categorical columns.
-        
-        This can be done with the `mlprimitives.datasets.load_census` function:
-        
-        ```python3
-        from mlprimitives.datasets import load_census
-        
-        dataset = load_census()
-        ```
-        
-        This dataset object has an attribute `data` which contains a table with several categorical
-        columns.
-        
-        We can have a look at this table by executing `dataset.data.head()`, which will return a
-        table like this:
-        
-        ```
-                                     0                    1                   2
-        age                         39                   50                  38
-        workclass            State-gov     Self-emp-not-inc             Private
-        fnlwgt                   77516                83311              215646
-        education            Bachelors            Bachelors             HS-grad
-        education-num               13                   13                   9
-        marital-status   Never-married   Married-civ-spouse            Divorced
-        occupation        Adm-clerical      Exec-managerial   Handlers-cleaners
-        relationship     Not-in-family              Husband       Not-in-family
-        race                     White                White               White
-        sex                       Male                 Male                Male
-        capital-gain              2174                    0                   0
-        capital-loss                 0                    0                   0
-        hours-per-week              40                   13                  40
-        native-country   United-States        United-States       United-States
-        ```
-        
-        ### 3. Fit the primitive
-        
-        In order to run our pipeline, we first need to fit it.
-        
-        This is the process where it analyzes the data to detect which columns are categorical
-        
-        This is done by calling its `fit` method and assing the `dataset.data` as `X`.
-        
-        ```python3
-        primitive.fit(X=dataset.data)
-        ```
-        
-        ### 4. Produce results
-        
-        Once the pipeline is fit, we can process the data by calling the `produce` method of the
-        primitive instance and passing agin the `data` as `X`.
-        
-        ```python3
-        transformed = primitive.produce(X=dataset.data)
-        ```
-        
-        After this is done, we can see how the transformed data contains the newly generated
-        one-hot vectors:
-        
-        ```
-                                                        0      1       2       3       4
-        age                                            39     50      38      53      28
-        fnlwgt                                      77516  83311  215646  234721  338409
-        education-num                                  13     13       9       7      13
-        capital-gain                                 2174      0       0       0       0
-        capital-loss                                    0      0       0       0       0
-        hours-per-week                                 40     13      40      40      40
-        workclass= Private                              0      0       1       1       1
-        workclass= Self-emp-not-inc                     0      1       0       0       0
-        workclass= Local-gov                            0      0       0       0       0
-        workclass= ?                                    0      0       0       0       0
-        workclass= State-gov                            1      0       0       0       0
-        workclass= Self-emp-inc                         0      0       0       0       0
-        ...                                             ...    ...     ...     ...     ...
-        ```
-        
-        ## Tuning a Primitive
-        
-        In this short tutorial we will teach you how to evaluate the performance of a primitive
-        and improve its performance by modifying its hyperparameters.
-        
-        To do so, we will load a primitive that can learn from the transformed data that we just
-        generated and later on make predictions based on new data.
-        
-        ### 1. Load another primitive
-        
-        Firs of all, we will load the `xgboost.XGBClassifier` primitive that we will use afterwards.
-        
-        ```python3
-        primitive = load_primitive('xgboost.XGBClassifier')
-        ```
-        
-        ### 2. Split the dataset
-        
-        Before being able to evaluate the primitive perfomance, we need to split the data in two
-        parts: train, which will be used for the primitive to learn, and test, which will be used
-        to make the predictions that later on will be evaluated.
-        
-        In order to do this, we will get the first 75% of rows from the transformed data that we
-        obtained above and call it `X_train`, and then set the next 25% of rows as `X_test`.
-        
-        ```python3
-        train_size = int(len(transformed) * 0.75)
-        X_train = transformed.iloc[:train_size]
-        X_test = transformed.iloc[train_size:]
-        ```
-        
-        Similarly, we need to obtain the `y_train` and `y_test` variables containing the corresponding
-        output values.
-        
-        ```python3
-        y_train = dataset.target[:train_size]
-        y_test = dataset.target[train_size:]
-        ```
-        
-        ### 3. Fit the new primitive
-        
-        Once we have have splitted the data, we can fit the primitive by passing `X_train` and `y_train`
-        to its `fit` method.
-        
-        ```python3
-        primitive.fit(X=X_train, y=y_train)
-        ```
-        
-        ### 4. Make predictions
-        
-        Once the primitive has been fitted, we can produce predictions using the `X_test` data as input.
-        
-        ```python3
-        predictions = primitive.produce(X=X_test)
-        ```
-        
-        ### 5. Evalute the performance
-        
-        We can now evaluate how good the predictions from our primitive are by using the `score`
-        method from the `dataset` object on both the expected output and the real output from the
-        primitive:
-        
-        ```python3
-        dataset.score(y_test, predictions)
-        ```
-        
-        This will output a float value between 0 and 1 indicating how good the predicitons are, being
-        0 the worst score possible and 1 the best one.
-        
-        In this case we will obtain a score around 0.866
-        
-        ### 6. Set new hyperparameter values
-        
-        In order to improve the performance of our primitive we will try to modify a couple of its
-        hyperparameters.
-        
-        First we will see which hyperparameter values the primitive has by calling its
-        `get_hyperparameters` method.
-        
-        ```python3
-        primitive.get_hyperparameters()
-        ```
-        
-        which will return a dictionary like this:
-        
-        ```python
-        {
-            "n_jobs": -1,
-            "n_estimators": 100,
-            "max_depth": 3,
-            "learning_rate": 0.1,
-            "gamma": 0,
-            "min_child_weight": 1
-        }
-        ```
-        
-        Next, we will see which are the valid values for each one of those hyperparameters by calling its
-        `get_tunable_hyperparameters` method:
-        
-        ```python3
-        primitive.get_tunable_hyperparameters()
-        ```
-        
-        For example, we will see that the `max_depth` hyperparameter has the following specification:
-        
-        ```python
-        {
-            "type": "int",
-            "default": 3,
-            "range": [
-                3,
-                10
-            ]
-        }
-        ```
-        
-        Next, we will choose a valid value, for example 7, and set it into the pipeline using the
-        `set_hyperparameters` method:
-        
-        ```python3
-        primitive.set_hyperparameters({'max_depth': 7})
-        ```
-        
-        ### 7. Re-evaluate the performance
-        
-        Once the new hyperparameter value has been set, we repeat the fit/train/score cycle to
-        evaluate the performance of this new hyperparameter value:
-        
-        ```python3
-        primitive.fit(X=X_train, y=y_train)
-        predictions = primitive.produce(X=X_test)
-        dataset.score(y_test, predictions)
-        ```
-        
-        This time we should see that the performance has improved to a value around 0.724
-        
-        ## What's Next?
-        
-        Do you want to [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/getting_started/concepts.html),
-        about [how to contribute to it](https://MLBazaar.github.io/MLPrimitives/community/contributing.html)
-        or browse the [API Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
-        Please check the corresponding sections of the [documentation](https://MLBazaar.github.io/MLPrimitives/)!
-        
-        
-        # History
-        
-        ## 0.3.3 - 2023-01-20
-        
-        ### General Imporvements
-        
-        * Update dependencies - [Issue #276](https://github.com/MLBazaar/MLPrimitives/issues/276) by @sarahmish
-        
-        ### Adapter Improvements
-        
-        * Building model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/MLPrimitives/issues/267) by @sarahmish
-        
-        ## 0.3.2 - 2021-11-09
-        
-        ### Adapter Improvements
-        
-        * Inferring data shapes with single dimension for keras adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
-        
-        ## 0.3.1 - 2021-10-07
-        
-        ### Adapter Improvements
-        
-        * Dynamic target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by @sarahmish
-        * Save keras primitives in Windows environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish
-        
-        ### General Imporvements
-        
-        * Update TensorFlow and NumPy dependency - [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish
-        
-        ## 0.3.0 - 2021-01-09
-        
-        ### New Primitives
-        
-        * Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish
-        * Add primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish
-        
-        ### Primitive Improvements
-        
-        * Add offset to rolling_window_sequence primitive - [Issue #251](https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz
-        * Rename the time_index column to time - [Issue #252](https://github.com/MLBazaar/MLPrimitives/issues/252) by @pvk-developer
-        * Update featuretools dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-developer
-        
-        ### General Improvements
-        
-        * Udpate dependencies and add python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala
-        * Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/244) by @csala
-        
-        ## 0.2.5 - 2020-07-29
-        
-        ### Primitive Improvements
-        
-        * Accept timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer
-        
-        ### Bug Fixes
-        
-        * ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer
-        
-        ### New Primitives
-        
-        * Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC
-        
-        ## 0.2.4 - 2020-01-30
-        
-        ### New Primitives
-        
-        * Add RangeScaler and RangeUnscaler primitives - [Issue #232](https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala
-        
-        ### Primitive Improvements
-        
-        * Extract input_shape from X in keras.Sequential - [Issue #223](https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala
-        
-        ### Bug Fixes
-        
-        * mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228](https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala
-        * Error when loading the reviews dataset - [Issue #230](https://github.com/MLBazaar/MLPrimitives/issues/230) by @csala
-        * Curate dependencies: specify an explicit prompt-toolkit version range - [Issue #224](https://github.com/MLBazaar/MLPrimitives/issues/224) by @csala
-        
-        ## 0.2.3 - 2019-11-14
-        
-        ### New Primitives
-        
-        * Add primitive to make window_sequences based on cutoff times - [Issue #217](https://github.com/MLBazaar/MLPrimitives/issues/217) by @csala
-        * Create a keras LSTM based TimeSeriesClassifier primitive - [Issue #218](https://github.com/MLBazaar/MLPrimitives/issues/218) by @csala
-        * Add pandas DataFrame primitives - [Issue #214](https://github.com/MLBazaar/MLPrimitives/issues/214) by @csala
-        * Add featuretools.EntitySet.normalize_entity primitive - [Issue #209](https://github.com/MLBazaar/MLPrimitives/issues/209) by @csala
-        
-        ### Primitive Improvements
-        
-        * Make featuretools.EntitySet.entity_from_dataframe entityset arg optional - [Issue #208](https://github.com/MLBazaar/MLPrimitives/issues/208) by @csala
-        
-        * Add text regression dataset - [Issue #206](https://github.com/MLBazaar/MLPrimitives/issues/206) by @csala
-        
-        ### Bug Fixes
-        
-        * pandas.DataFrame.resample crash when grouping by integer columns - [Issue #211](https://github.com/MLBazaar/MLPrimitives/issues/211) by @csala
-        
-        ## 0.2.2 - 2019-10-08
-        
-        ### New Primitives
-        
-        * Add primitives for GAN based time-series anomaly detection - [Issue #200](https://github.com/MLBazaar/MLPrimitives/issues/200) by @AlexanderGeiger
-        * Add `numpy.reshape` and `numpy.ravel` primitives - [Issue #197](https://github.com/MLBazaar/MLPrimitives/issues/197) by @AlexanderGeiger
-        * Add feature selection primitive based on Lasso - [Issue #194](https://github.com/MLBazaar/MLPrimitives/issues/194) by @csala
-        
-        ### Primitive Improvements
-        
-        * `feature_extraction.CategoricalEncoder` support dtype category - [Issue #196](https://github.com/MLBazaar/MLPrimitives/issues/196) by @csala
-        
-        ## 0.2.1 - 2019-09-09
-        
-        ### New Primitives
-        
-        * Timeseries Intervals to Mask Primitive - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
-        * Add new primitive: Arima model - [Issue #168](https://github.com/MLBazaar/MLPrimitives/issues/168) by @AlexanderGeiger
-        
-        ### Primitive Improvements
-        
-        * Curate PCA primitive hyperparameters - [Issue #190](https://github.com/MLBazaar/MLPrimitives/issues/190) by @AlexanderGeiger
-        * Add option to drop rolling window sequences - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
-        
-        ### Bug Fixes
-        
-        * scikit-image==0.14.3 crashes when installed on Mac - [Issue #188](https://github.com/MLBazaar/MLPrimitives/issues/188) by @csala
-        
-        ## 0.2.0
-        
-        ### New Features
-        
-        * Publish the pipelines as an `entry_point`
-        [Issue #175](https://github.com/MLBazaar/MLPrimitives/issues/175) by @csala
-        
-        ### Primitive Improvements
-        
-        * Improve pandas.DataFrame.resample primitive [Issue #177](https://github.com/MLBazaar/MLPrimitives/issues/177) by @csala
-        * Improve `feature_extractor` primitives [Issue #183](https://github.com/MLBazaar/MLPrimitives/issues/183) by @csala
-        * Improve `find_anomalies` primitive [Issue #180](https://github.com/MLBazaar/MLPrimitives/issues/180) by @AlexanderGeiger
-        
-        ### Bug Fixes
-        
-        * Typo in the primitive keras.Sequential.LSTMTimeSeriesRegressor [Issue #176](https://github.com/MLBazaar/MLPrimitives/issues/176) by @DanielCalvoCerezo
-        
-        
-        ## 0.1.10
-        
-        ### New Features
-        
-        * Add function to run primitives without a pipeline [Issue #43](https://github.com/MLBazaar/MLPrimitives/issues/43) by @csala
-        
-        ### New Pipelines
-        
-        * Add pipelines for all the MLBlocks examples [Issue #162](https://github.com/MLBazaar/MLPrimitives/issues/162) by @csala
-        
-        ### Primitive Improvements
-        
-        * Add Early Stopping to `keras.Sequential.LSTMTimeSeriesRegressor` primitive [Issue #156](https://github.com/MLBazaar/MLPrimitives/issues/156) by @csala
-        * Make FeatureExtractor primitives accept Numpy arrays [Issue #165](https://github.com/MLBazaar/MLPrimitives/issues/165) by @csala
-        * Add window size and pruning to the `timeseries_anomalies.find_anomalies` primitive [Issue #160](https://github.com/MLBazaar/MLPrimitives/issues/160) by @csala
-        
-        
-        ## 0.1.9
-        
-        ### New Features
-        
-        * Add a single table binary classification dataset [Issue #141](https://github.com/MLBazaar/MLPrimitives/issues/141) by @csala
-        
-        ### New Primitives
-        
-        * Add Multilayer Perceptron (MLP) primitive for binary classification [Issue #140](https://github.com/MLBazaar/MLPrimitives/issues/140) by @Hector-hedb12
-        * Add primitive for Sequence classification with LSTM [Issue #150](https://github.com/MLBazaar/MLPrimitives/issues/150) by @Hector-hedb12
-        * Add VGG-like convnet primitive [Issue #149](https://github.com/MLBazaar/MLPrimitives/issues/149) by @Hector-hedb12
-        * Add Multilayer Perceptron (MLP) primitive for multi-class softmax classification [Issue #139](https://github.com/MLBazaar/MLPrimitives/issues/139) by @Hector-hedb12
-        * Add primitive to count feature matrix columns [Issue #146](https://github.com/MLBazaar/MLPrimitives/issues/146) by @csala
-        
-        ### Primitive Improvements
-        
-        * Add additional fit and predict arguments to keras.Sequential [Issue #161](https://github.com/MLBazaar/MLPrimitives/issues/161) by @csala
-        * Add suport for keras.Sequential Callbacks [Issue #159](https://github.com/MLBazaar/MLPrimitives/issues/159) by @csala
-        * Add fixed hyperparam to control keras.Sequential verbosity [Issue #143](https://github.com/MLBazaar/MLPrimitives/issues/143) by @csala
-        
-        ## 0.1.8
-        
-        ### New Primitives
-        
-        * mlprimitives.custom.timeseries_preprocessing.time_segments_average - [Issue #137](https://github.com/MLBazaar/MLPrimitives/issues/137)
-        
-        ### New Features
-        
-        * Add target_index output in timseries_preprocessing.rolling_window_sequences - [Issue #136](https://github.com/MLBazaar/MLPrimitives/issues/136)
-        
-        ## 0.1.7
-        
-        ### General Improvements
-        
-        * Validate JSON format in `make lint` -  [Issue #133](https://github.com/MLBazaar/MLPrimitives/issues/133)
-        * Add demo datasets - [Issue #131](https://github.com/MLBazaar/MLPrimitives/issues/131)
-        * Improve featuretools.dfs primitive - [Issue #127](https://github.com/MLBazaar/MLPrimitives/issues/127)
-        
-        ### New Primitives
-        
-        * pandas.DataFrame.resample - [Issue #123](https://github.com/MLBazaar/MLPrimitives/issues/123)
-        * pandas.DataFrame.unstack - [Issue #124](https://github.com/MLBazaar/MLPrimitives/issues/124)
-        * featuretools.EntitySet.add_relationship - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
-        * featuretools.EntitySet.entity_from_dataframe - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
-        
-        ### Bug Fixes
-        
-        * Bug in timeseries_anomalies.py - [Issue #119](https://github.com/MLBazaar/MLPrimitives/issues/119)
-        
-        ## 0.1.6
-        
-        ### General Improvements
-        
-        * Add Contributing Documentation
-        * Remove upper bound in pandas version given new release of `featuretools` v0.6.1
-        * Improve LSTMTimeSeriesRegressor hyperparameters
-        
-        ### New Primitives
-        
-        * mlprimitives.candidates.dsp.SpectralMask
-        * mlprimitives.custom.timeseries_anomalies.find_anomalies
-        * mlprimitives.custom.timeseries_anomalies.regression_errors
-        * mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences
-        * mlprimitives.custom.timeseries_preprocessing.time_segments_average
-        * sklearn.linear_model.ElasticNet
-        * sklearn.linear_model.Lars
-        * sklearn.linear_model.Lasso
-        * sklearn.linear_model.MultiTaskLasso
-        * sklearn.linear_model.Ridge
-        
-        ## 0.1.5
-        
-        ### New Primitives
-        
-        * sklearn.impute.SimpleImputer
-        * sklearn.preprocessing.MinMaxScaler
-        * sklearn.preprocessing.MaxAbsScaler
-        * sklearn.preprocessing.RobustScaler
-        * sklearn.linear_model.LinearRegression
-        
-        ### General Improvements
-        
-        * Separate curated from candidate primitives
-        * Setup `entry_points` in setup.py to improve compaitibility with MLBlocks
-        * Add a test-pipelines command to test all the existing pipelines
-        * Clean sklearn example pipelines
-        * Change the `author` entry to a `contributors` list
-        * Change the name of `mlblocks_primitives` folder
-        * Pip install `requirements_dev.txt` fail documentation
-        
-        ### Bug Fixes
-        
-        * Fix LSTMTimeSeriesRegressor primitive. Issue #90
-        * Fix timeseries primitives. Issue #91
-        * Negative index anomalies in `timeseries_errors`. Issue #89
-        * Keep pandas version below 0.24.0. Issue #87
-        
-        ## 0.1.4
-        
-        ### New Primitives
-        
-        * mlprimitives.timeseries primitives for timeseries data preprocessing
-        * mlprimitives.timeseres_error primitives for timeseries anomaly detection
-        * keras.Sequential.LSTMTimeSeriesRegressor
-        * sklearn.neighbors.KNeighbors Classifier and Regressor
-        * several sklearn.decomposition primitives
-        * several sklearn.ensemble primitives
-        
-        ### Bug Fixes
-        
-        * Fix typo in mlprimitives.text.TextCleaner primitive
-        * Fix bug in index handling in featuretools.dfs primitive
-        * Fix bug in SingleLayerCNNImageClassifier annotation
-        * Remove old vlaidation tags from JSON annotations
-        
-        ## 0.1.3
-        
-        ### New Features
-        
-        * Fix and re-enable featuretools.dfs primitive.
-        
-        ## 0.1.2
-        
-        ### New Features
-        
-        * Add pipeline specification language and Evaluation utilities.
-        * Add pipelines for graph, text and tabular problems.
-        * New primitives ClassEncoder and ClassDecoder
-        * New primitives UniqueCounter and VocabularyCounter
-        
-        ### Bug Fixes
-        
-        * Fix TrivialPredictor bug when working with numpy arrays
-        * Change XGB default learning rate and number of estimators
-        
-        
-        ## 0.1.1
-        
-        ### New Features
-        
-        * Add more keras.applications primitives.
-        * Add a Text Cleanup primitive.
-        
-        ### Bug Fixes
-        
-        * Add keywords to `keras.preprocessing` primtives.
-        * Fix the `image_transform` method.
-        * Add `epoch` as a fixed hyperparameter for `keras.Sequential` primitives.
-        
-        ## 0.1.0
-        
-        * First release on PyPI.
-        
 Keywords: mlblocks mlprimitives pipelines primitives machine learning data science
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+<p align="left">
+  <a href="https://dai.lids.mit.edu">
+    <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
+  </a>
+  <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
+</p>
+
+[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+[![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)](https://pypi.python.org/pypi/mlprimitives)
+[![Tests](https://github.com/MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
+[![Downloads](https://pepy.tech/badge/mlprimitives)](https://pepy.tech/project/mlprimitives)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
+
+# MLPrimitives
+
+Pipelines and primitives for machine learning and data science.
+
+* Documentation: https://MLBazaar.github.io/MLPrimitives
+* Github: https://github.com/MLBazaar/MLPrimitives
+* License: [MIT](https://github.com/MLBazaar/MLPrimitives/blob/master/LICENSE)
+* Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+
+# Overview
+
+This repository contains primitive annotations to be used by the MLBlocks library, as well as
+the necessary Python code to make some of them fully compatible with the MLBlocks API requirements.
+
+There is also a collection of custom primitives contributed directly to this library, which either
+combine third party tools or implement new functionalities from scratch.
+
+## Why did we create this library?
+
+* Too many libraries in a fast growing field
+* Huge societal need to build machine learning apps
+* Domain expertise resides at several places (knowledge of math)
+* No documented information about hyperparameters, behavior...
+
+# Installation
+
+## Requirements
+
+**MLPrimitives** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+
+Also, although it is not strictly required, the usage of a
+[virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
+interfering with other software installed in the system where **MLPrimitives** is run.
+
+## Install with pip
+
+The easiest and recommended way to install **MLPrimitives** is using [pip](https://pip.pypa.io/en/stable/):
+
+```bash
+pip install mlprimitives
+```
+
+This will pull and install the latest stable release from [PyPi](https://pypi.org/).
+
+If you want to install from source or contribute to the project please read the
+[Contributing Guide](https://MLBazaar.github.io/MLPrimitives/community/welcome.html).
+
+# Quickstart
+
+This section is a short series of tutorials to help you getting started with MLPrimitives.
+
+In the following steps you will learn how to load and run a primitive on some data.
+
+Later on you will learn how to evaluate and improve the performance of a primitive by tuning
+its hyperparameters.
+
+## Running a Primitive
+
+In this first tutorial, we will be executing a single primitive for data transformation.
+
+### 1. Load a Primitive
+
+The first step in order to run a primitive is to load it.
+
+This will be done using the `mlprimitives.load_primitive` function, which will
+load the indicated primitive as an [MLBlock Object from MLBlocks](https://MLBazaar.github.io/MLBlocks/api/mlblocks.html#mlblocks.MLBlock)
+
+In this case, we will load the `mlprimitives.custom.feature_extraction.CategoricalEncoder`
+primitive.
+
+```python3
+from mlprimitives import load_primitive
+
+primitive = load_primitive('mlprimitives.custom.feature_extraction.CategoricalEncoder')
+```
+
+### 2. Load some data
+
+The CategoricalEncoder is a transformation primitive which applies one-hot encoding to all the
+categorical columns of a `pandas.DataFrame`.
+
+So, in order to be able to run our primitive, we will first load some data that contains
+categorical columns.
+
+This can be done with the `mlprimitives.datasets.load_census` function:
+
+```python3
+from mlprimitives.datasets import load_census
+
+dataset = load_census()
+```
+
+This dataset object has an attribute `data` which contains a table with several categorical
+columns.
+
+We can have a look at this table by executing `dataset.data.head()`, which will return a
+table like this:
+
+```
+                             0                    1                   2
+age                         39                   50                  38
+workclass            State-gov     Self-emp-not-inc             Private
+fnlwgt                   77516                83311              215646
+education            Bachelors            Bachelors             HS-grad
+education-num               13                   13                   9
+marital-status   Never-married   Married-civ-spouse            Divorced
+occupation        Adm-clerical      Exec-managerial   Handlers-cleaners
+relationship     Not-in-family              Husband       Not-in-family
+race                     White                White               White
+sex                       Male                 Male                Male
+capital-gain              2174                    0                   0
+capital-loss                 0                    0                   0
+hours-per-week              40                   13                  40
+native-country   United-States        United-States       United-States
+```
+
+### 3. Fit the primitive
+
+In order to run our pipeline, we first need to fit it.
+
+This is the process where it analyzes the data to detect which columns are categorical
+
+This is done by calling its `fit` method and assing the `dataset.data` as `X`.
+
+```python3
+primitive.fit(X=dataset.data)
+```
+
+### 4. Produce results
+
+Once the pipeline is fit, we can process the data by calling the `produce` method of the
+primitive instance and passing agin the `data` as `X`.
+
+```python3
+transformed = primitive.produce(X=dataset.data)
+```
+
+After this is done, we can see how the transformed data contains the newly generated
+one-hot vectors:
+
+```
+                                                0      1       2       3       4
+age                                            39     50      38      53      28
+fnlwgt                                      77516  83311  215646  234721  338409
+education-num                                  13     13       9       7      13
+capital-gain                                 2174      0       0       0       0
+capital-loss                                    0      0       0       0       0
+hours-per-week                                 40     13      40      40      40
+workclass= Private                              0      0       1       1       1
+workclass= Self-emp-not-inc                     0      1       0       0       0
+workclass= Local-gov                            0      0       0       0       0
+workclass= ?                                    0      0       0       0       0
+workclass= State-gov                            1      0       0       0       0
+workclass= Self-emp-inc                         0      0       0       0       0
+...                                             ...    ...     ...     ...     ...
+```
+
+## Tuning a Primitive
+
+In this short tutorial we will teach you how to evaluate the performance of a primitive
+and improve its performance by modifying its hyperparameters.
+
+To do so, we will load a primitive that can learn from the transformed data that we just
+generated and later on make predictions based on new data.
+
+### 1. Load another primitive
+
+Firs of all, we will load the `xgboost.XGBClassifier` primitive that we will use afterwards.
+
+```python3
+primitive = load_primitive('xgboost.XGBClassifier')
+```
+
+### 2. Split the dataset
+
+Before being able to evaluate the primitive perfomance, we need to split the data in two
+parts: train, which will be used for the primitive to learn, and test, which will be used
+to make the predictions that later on will be evaluated.
+
+In order to do this, we will get the first 75% of rows from the transformed data that we
+obtained above and call it `X_train`, and then set the next 25% of rows as `X_test`.
+
+```python3
+train_size = int(len(transformed) * 0.75)
+X_train = transformed.iloc[:train_size]
+X_test = transformed.iloc[train_size:]
+```
+
+Similarly, we need to obtain the `y_train` and `y_test` variables containing the corresponding
+output values.
+
+```python3
+y_train = dataset.target[:train_size]
+y_test = dataset.target[train_size:]
+```
+
+### 3. Fit the new primitive
+
+Once we have have splitted the data, we can fit the primitive by passing `X_train` and `y_train`
+to its `fit` method.
+
+```python3
+primitive.fit(X=X_train, y=y_train)
+```
+
+### 4. Make predictions
+
+Once the primitive has been fitted, we can produce predictions using the `X_test` data as input.
+
+```python3
+predictions = primitive.produce(X=X_test)
+```
+
+### 5. Evalute the performance
+
+We can now evaluate how good the predictions from our primitive are by using the `score`
+method from the `dataset` object on both the expected output and the real output from the
+primitive:
+
+```python3
+dataset.score(y_test, predictions)
+```
+
+This will output a float value between 0 and 1 indicating how good the predicitons are, being
+0 the worst score possible and 1 the best one.
+
+In this case we will obtain a score around 0.866
+
+### 6. Set new hyperparameter values
+
+In order to improve the performance of our primitive we will try to modify a couple of its
+hyperparameters.
+
+First we will see which hyperparameter values the primitive has by calling its
+`get_hyperparameters` method.
+
+```python3
+primitive.get_hyperparameters()
+```
+
+which will return a dictionary like this:
+
+```python
+{
+    "n_jobs": -1,
+    "n_estimators": 100,
+    "max_depth": 3,
+    "learning_rate": 0.1,
+    "gamma": 0,
+    "min_child_weight": 1
+}
+```
+
+Next, we will see which are the valid values for each one of those hyperparameters by calling its
+`get_tunable_hyperparameters` method:
+
+```python3
+primitive.get_tunable_hyperparameters()
+```
+
+For example, we will see that the `max_depth` hyperparameter has the following specification:
+
+```python
+{
+    "type": "int",
+    "default": 3,
+    "range": [
+        3,
+        10
+    ]
+}
+```
+
+Next, we will choose a valid value, for example 7, and set it into the pipeline using the
+`set_hyperparameters` method:
+
+```python3
+primitive.set_hyperparameters({'max_depth': 7})
+```
+
+### 7. Re-evaluate the performance
+
+Once the new hyperparameter value has been set, we repeat the fit/train/score cycle to
+evaluate the performance of this new hyperparameter value:
+
+```python3
+primitive.fit(X=X_train, y=y_train)
+predictions = primitive.produce(X=X_test)
+dataset.score(y_test, predictions)
+```
+
+This time we should see that the performance has improved to a value around 0.724
+
+## What's Next?
+
+Do you want to [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/getting_started/concepts.html),
+about [how to contribute to it](https://MLBazaar.github.io/MLPrimitives/community/contributing.html)
+or browse the [API Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
+Please check the corresponding sections of the [documentation](https://MLBazaar.github.io/MLPrimitives/)!
+
+
+# History
+
+## 0.3.5 - 2023-04-14
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #278](https://github.com/MLBazaar/MLPrimitives/issues/278) by @sarahmish
+
+## 0.3.4 - 2023-01-24
+
+### General Imporvements
+
+* Update `mlblocks` cap - [Issue #277](https://github.com/MLBazaar/MLPrimitives/issues/277) by @sarahmish
+
+## 0.3.3 - 2023-01-20
+
+### General Imporvements
+
+* Update dependencies - [Issue #276](https://github.com/MLBazaar/MLPrimitives/issues/276) by @sarahmish
+
+### Adapter Improvements
+
+* Building model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/MLPrimitives/issues/267) by @sarahmish
+
+## 0.3.2 - 2021-11-09
+
+### Adapter Improvements
+
+* Inferring data shapes with single dimension for keras adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
+
+## 0.3.1 - 2021-10-07
+
+### Adapter Improvements
+
+* Dynamic target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by @sarahmish
+* Save keras primitives in Windows environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish
+
+### General Imporvements
+
+* Update TensorFlow and NumPy dependency - [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish
+
+## 0.3.0 - 2021-01-09
+
+### New Primitives
+
+* Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish
+* Add primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish
+
+### Primitive Improvements
+
+* Add offset to rolling_window_sequence primitive - [Issue #251](https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz
+* Rename the time_index column to time - [Issue #252](https://github.com/MLBazaar/MLPrimitives/issues/252) by @pvk-developer
+* Update featuretools dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-developer
+
+### General Improvements
+
+* Udpate dependencies and add python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala
+* Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/244) by @csala
+
+## 0.2.5 - 2020-07-29
+
+### Primitive Improvements
+
+* Accept timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer
+
+### Bug Fixes
+
+* ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer
+
+### New Primitives
+
+* Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC
+
+## 0.2.4 - 2020-01-30
+
+### New Primitives
+
+* Add RangeScaler and RangeUnscaler primitives - [Issue #232](https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala
+
+### Primitive Improvements
+
+* Extract input_shape from X in keras.Sequential - [Issue #223](https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala
+
+### Bug Fixes
+
+* mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228](https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala
+* Error when loading the reviews dataset - [Issue #230](https://github.com/MLBazaar/MLPrimitives/issues/230) by @csala
+* Curate dependencies: specify an explicit prompt-toolkit version range - [Issue #224](https://github.com/MLBazaar/MLPrimitives/issues/224) by @csala
+
+## 0.2.3 - 2019-11-14
+
+### New Primitives
+
+* Add primitive to make window_sequences based on cutoff times - [Issue #217](https://github.com/MLBazaar/MLPrimitives/issues/217) by @csala
+* Create a keras LSTM based TimeSeriesClassifier primitive - [Issue #218](https://github.com/MLBazaar/MLPrimitives/issues/218) by @csala
+* Add pandas DataFrame primitives - [Issue #214](https://github.com/MLBazaar/MLPrimitives/issues/214) by @csala
+* Add featuretools.EntitySet.normalize_entity primitive - [Issue #209](https://github.com/MLBazaar/MLPrimitives/issues/209) by @csala
+
+### Primitive Improvements
+
+* Make featuretools.EntitySet.entity_from_dataframe entityset arg optional - [Issue #208](https://github.com/MLBazaar/MLPrimitives/issues/208) by @csala
+
+* Add text regression dataset - [Issue #206](https://github.com/MLBazaar/MLPrimitives/issues/206) by @csala
+
+### Bug Fixes
+
+* pandas.DataFrame.resample crash when grouping by integer columns - [Issue #211](https://github.com/MLBazaar/MLPrimitives/issues/211) by @csala
+
+## 0.2.2 - 2019-10-08
+
+### New Primitives
+
+* Add primitives for GAN based time-series anomaly detection - [Issue #200](https://github.com/MLBazaar/MLPrimitives/issues/200) by @AlexanderGeiger
+* Add `numpy.reshape` and `numpy.ravel` primitives - [Issue #197](https://github.com/MLBazaar/MLPrimitives/issues/197) by @AlexanderGeiger
+* Add feature selection primitive based on Lasso - [Issue #194](https://github.com/MLBazaar/MLPrimitives/issues/194) by @csala
+
+### Primitive Improvements
+
+* `feature_extraction.CategoricalEncoder` support dtype category - [Issue #196](https://github.com/MLBazaar/MLPrimitives/issues/196) by @csala
+
+## 0.2.1 - 2019-09-09
+
+### New Primitives
+
+* Timeseries Intervals to Mask Primitive - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
+* Add new primitive: Arima model - [Issue #168](https://github.com/MLBazaar/MLPrimitives/issues/168) by @AlexanderGeiger
+
+### Primitive Improvements
+
+* Curate PCA primitive hyperparameters - [Issue #190](https://github.com/MLBazaar/MLPrimitives/issues/190) by @AlexanderGeiger
+* Add option to drop rolling window sequences - [Issue #186](https://github.com/MLBazaar/MLPrimitives/issues/186) by @AlexanderGeiger
+
+### Bug Fixes
+
+* scikit-image==0.14.3 crashes when installed on Mac - [Issue #188](https://github.com/MLBazaar/MLPrimitives/issues/188) by @csala
+
+## 0.2.0
+
+### New Features
+
+* Publish the pipelines as an `entry_point`
+[Issue #175](https://github.com/MLBazaar/MLPrimitives/issues/175) by @csala
+
+### Primitive Improvements
+
+* Improve pandas.DataFrame.resample primitive [Issue #177](https://github.com/MLBazaar/MLPrimitives/issues/177) by @csala
+* Improve `feature_extractor` primitives [Issue #183](https://github.com/MLBazaar/MLPrimitives/issues/183) by @csala
+* Improve `find_anomalies` primitive [Issue #180](https://github.com/MLBazaar/MLPrimitives/issues/180) by @AlexanderGeiger
+
+### Bug Fixes
+
+* Typo in the primitive keras.Sequential.LSTMTimeSeriesRegressor [Issue #176](https://github.com/MLBazaar/MLPrimitives/issues/176) by @DanielCalvoCerezo
+
+
+## 0.1.10
+
+### New Features
+
+* Add function to run primitives without a pipeline [Issue #43](https://github.com/MLBazaar/MLPrimitives/issues/43) by @csala
+
+### New Pipelines
+
+* Add pipelines for all the MLBlocks examples [Issue #162](https://github.com/MLBazaar/MLPrimitives/issues/162) by @csala
+
+### Primitive Improvements
+
+* Add Early Stopping to `keras.Sequential.LSTMTimeSeriesRegressor` primitive [Issue #156](https://github.com/MLBazaar/MLPrimitives/issues/156) by @csala
+* Make FeatureExtractor primitives accept Numpy arrays [Issue #165](https://github.com/MLBazaar/MLPrimitives/issues/165) by @csala
+* Add window size and pruning to the `timeseries_anomalies.find_anomalies` primitive [Issue #160](https://github.com/MLBazaar/MLPrimitives/issues/160) by @csala
+
+
+## 0.1.9
+
+### New Features
+
+* Add a single table binary classification dataset [Issue #141](https://github.com/MLBazaar/MLPrimitives/issues/141) by @csala
+
+### New Primitives
+
+* Add Multilayer Perceptron (MLP) primitive for binary classification [Issue #140](https://github.com/MLBazaar/MLPrimitives/issues/140) by @Hector-hedb12
+* Add primitive for Sequence classification with LSTM [Issue #150](https://github.com/MLBazaar/MLPrimitives/issues/150) by @Hector-hedb12
+* Add VGG-like convnet primitive [Issue #149](https://github.com/MLBazaar/MLPrimitives/issues/149) by @Hector-hedb12
+* Add Multilayer Perceptron (MLP) primitive for multi-class softmax classification [Issue #139](https://github.com/MLBazaar/MLPrimitives/issues/139) by @Hector-hedb12
+* Add primitive to count feature matrix columns [Issue #146](https://github.com/MLBazaar/MLPrimitives/issues/146) by @csala
+
+### Primitive Improvements
+
+* Add additional fit and predict arguments to keras.Sequential [Issue #161](https://github.com/MLBazaar/MLPrimitives/issues/161) by @csala
+* Add suport for keras.Sequential Callbacks [Issue #159](https://github.com/MLBazaar/MLPrimitives/issues/159) by @csala
+* Add fixed hyperparam to control keras.Sequential verbosity [Issue #143](https://github.com/MLBazaar/MLPrimitives/issues/143) by @csala
+
+## 0.1.8
+
+### New Primitives
+
+* mlprimitives.custom.timeseries_preprocessing.time_segments_average - [Issue #137](https://github.com/MLBazaar/MLPrimitives/issues/137)
+
+### New Features
+
+* Add target_index output in timseries_preprocessing.rolling_window_sequences - [Issue #136](https://github.com/MLBazaar/MLPrimitives/issues/136)
+
+## 0.1.7
+
+### General Improvements
+
+* Validate JSON format in `make lint` -  [Issue #133](https://github.com/MLBazaar/MLPrimitives/issues/133)
+* Add demo datasets - [Issue #131](https://github.com/MLBazaar/MLPrimitives/issues/131)
+* Improve featuretools.dfs primitive - [Issue #127](https://github.com/MLBazaar/MLPrimitives/issues/127)
+
+### New Primitives
+
+* pandas.DataFrame.resample - [Issue #123](https://github.com/MLBazaar/MLPrimitives/issues/123)
+* pandas.DataFrame.unstack - [Issue #124](https://github.com/MLBazaar/MLPrimitives/issues/124)
+* featuretools.EntitySet.add_relationship - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
+* featuretools.EntitySet.entity_from_dataframe - [Issue #126](https://github.com/MLBazaar/MLPrimitives/issues/126)
+
+### Bug Fixes
+
+* Bug in timeseries_anomalies.py - [Issue #119](https://github.com/MLBazaar/MLPrimitives/issues/119)
+
+## 0.1.6
+
+### General Improvements
+
+* Add Contributing Documentation
+* Remove upper bound in pandas version given new release of `featuretools` v0.6.1
+* Improve LSTMTimeSeriesRegressor hyperparameters
+
+### New Primitives
+
+* mlprimitives.candidates.dsp.SpectralMask
+* mlprimitives.custom.timeseries_anomalies.find_anomalies
+* mlprimitives.custom.timeseries_anomalies.regression_errors
+* mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences
+* mlprimitives.custom.timeseries_preprocessing.time_segments_average
+* sklearn.linear_model.ElasticNet
+* sklearn.linear_model.Lars
+* sklearn.linear_model.Lasso
+* sklearn.linear_model.MultiTaskLasso
+* sklearn.linear_model.Ridge
+
+## 0.1.5
+
+### New Primitives
+
+* sklearn.impute.SimpleImputer
+* sklearn.preprocessing.MinMaxScaler
+* sklearn.preprocessing.MaxAbsScaler
+* sklearn.preprocessing.RobustScaler
+* sklearn.linear_model.LinearRegression
+
+### General Improvements
+
+* Separate curated from candidate primitives
+* Setup `entry_points` in setup.py to improve compaitibility with MLBlocks
+* Add a test-pipelines command to test all the existing pipelines
+* Clean sklearn example pipelines
+* Change the `author` entry to a `contributors` list
+* Change the name of `mlblocks_primitives` folder
+* Pip install `requirements_dev.txt` fail documentation
+
+### Bug Fixes
+
+* Fix LSTMTimeSeriesRegressor primitive. Issue #90
+* Fix timeseries primitives. Issue #91
+* Negative index anomalies in `timeseries_errors`. Issue #89
+* Keep pandas version below 0.24.0. Issue #87
+
+## 0.1.4
+
+### New Primitives
+
+* mlprimitives.timeseries primitives for timeseries data preprocessing
+* mlprimitives.timeseres_error primitives for timeseries anomaly detection
+* keras.Sequential.LSTMTimeSeriesRegressor
+* sklearn.neighbors.KNeighbors Classifier and Regressor
+* several sklearn.decomposition primitives
+* several sklearn.ensemble primitives
+
+### Bug Fixes
+
+* Fix typo in mlprimitives.text.TextCleaner primitive
+* Fix bug in index handling in featuretools.dfs primitive
+* Fix bug in SingleLayerCNNImageClassifier annotation
+* Remove old vlaidation tags from JSON annotations
+
+## 0.1.3
+
+### New Features
+
+* Fix and re-enable featuretools.dfs primitive.
+
+## 0.1.2
+
+### New Features
+
+* Add pipeline specification language and Evaluation utilities.
+* Add pipelines for graph, text and tabular problems.
+* New primitives ClassEncoder and ClassDecoder
+* New primitives UniqueCounter and VocabularyCounter
+
+### Bug Fixes
+
+* Fix TrivialPredictor bug when working with numpy arrays
+* Change XGB default learning rate and number of estimators
+
+
+## 0.1.1
+
+### New Features
+
+* Add more keras.applications primitives.
+* Add a Text Cleanup primitive.
+
+### Bug Fixes
+
+* Add keywords to `keras.preprocessing` primtives.
+* Fix the `image_transform` method.
+* Add `epoch` as a fixed hyperparameter for `keras.Sequential` primitives.
+
+## 0.1.0
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,11 +1,19 @@
-Metadata-Version: 2.1 Name: mlprimitives Version: 0.3.4.dev0 Summary: Pipelines
-and primitives for machine learning and data science. Home-page: https://
+Metadata-Version: 2.1 Name: mlprimitives Version: 0.3.5 Summary: Pipelines and
+primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLPrimitives Author: MIT Data To AI Lab Author-email:
-dailabmit@gmail.com License: MIT license Description:
+dailabmit@gmail.com License: MIT license Keywords: mlblocks mlprimitives
+pipelines primitives machine learning data science Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+dev License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/mlprimitives.svg)]
 (https://pypi.python.org/pypi/mlprimitives) [![Tests](https://github.com/
 MLBazaar/MLPrimitives/workflows/Run%20Tests/badge.svg)](https://github.com/
 MLBazaar/MLPrimitives/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
@@ -125,46 +133,51 @@
 dataset.score(y_test, predictions) ``` This time we should see that the
 performance has improved to a value around 0.724 ## What's Next? Do you want to
 [learn more about how the project](https://MLBazaar.github.io/MLPrimitives/
 getting_started/concepts.html), about [how to contribute to it](https://
 MLBazaar.github.io/MLPrimitives/community/contributing.html) or browse the [API
 Reference](https://MLBazaar.github.io/MLPrimitives/api/mlprimitives.html)?
 Please check the corresponding sections of the [documentation](https://
-MLBazaar.github.io/MLPrimitives/)! # History ## 0.3.3 - 2023-01-20 ### General
-Imporvements * Update dependencies - [Issue #276](https://github.com/MLBazaar/
-MLPrimitives/issues/276) by @sarahmish ### Adapter Improvements * Building
-model within fit in keras adapter- [Issue #267](https://github.com/MLBazaar/
-MLPrimitives/issues/267) by @sarahmish ## 0.3.2 - 2021-11-09 ### Adapter
-Improvements * Inferring data shapes with single dimension for keras adapter -
-[Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by @sarahmish
-## 0.3.1 - 2021-10-07 ### Adapter Improvements * Dynamic target_shape in keras
-adapter - [Issue #263](https://github.com/MLBazaar/MLPrimitives/issues/263) by
-@sarahmish * Save keras primitives in Windows environment - [Issue #261](https:
-//github.com/MLBazaar/MLPrimitives/issues/261) by @sarahmish ### General
-Imporvements * Update TensorFlow and NumPy dependency - [Issue #259](https://
-github.com/MLBazaar/MLPrimitives/issues/259) by @sarahmish ## 0.3.0 - 2021-01-
-09 ### New Primitives * Add primitive `sklearn.naive_bayes.GaussianNB` - [Issue
-#242](https://github.com/MLBazaar/MLPrimitives/issues/242) by @sarahmish * Add
-primitive `sklearn.linear_model.SGDClassifier` - [Issue #241](https://
-github.com/MLBazaar/MLPrimitives/issues/241) by @sarahmish ### Primitive
-Improvements * Add offset to rolling_window_sequence primitive - [Issue #251]
-(https://github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz *
-Rename the time_index column to time - [Issue #252](https://github.com/
-MLBazaar/MLPrimitives/issues/252) by @pvk-developer * Update featuretools
-dependency - [Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250)
-by @pvk-developer ### General Improvements * Udpate dependencies and add
-python3.8 - [Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246)
-by @csala * Drop Python35 - [Issue #244](https://github.com/MLBazaar/
-MLPrimitives/issues/244) by @csala ## 0.2.5 - 2020-07-29 ### Primitive
-Improvements * Accept timedelta `window_size` in `cutoff_window_sequences` -
-[Issue #239](https://github.com/MLBazaar/MLPrimitives/issues/239) by
-@joanvaquer ### Bug Fixes * ImportError: Keras requires TensorFlow 2.2 or
-higher. Install TensorFlow via `pip install tensorflow` - [Issue #237](https://
-github.com/MLBazaar/MLPrimitives/issues/237) by @joanvaquer ### New Primitives
-* Add `pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/
+MLBazaar.github.io/MLPrimitives/)! # History ## 0.3.5 - 2023-04-14 ### General
+Imporvements * Update `mlblocks` cap - [Issue #278](https://github.com/
+MLBazaar/MLPrimitives/issues/278) by @sarahmish ## 0.3.4 - 2023-01-24 ###
+General Imporvements * Update `mlblocks` cap - [Issue #277](https://github.com/
+MLBazaar/MLPrimitives/issues/277) by @sarahmish ## 0.3.3 - 2023-01-20 ###
+General Imporvements * Update dependencies - [Issue #276](https://github.com/
+MLBazaar/MLPrimitives/issues/276) by @sarahmish ### Adapter Improvements *
+Building model within fit in keras adapter- [Issue #267](https://github.com/
+MLBazaar/MLPrimitives/issues/267) by @sarahmish ## 0.3.2 - 2021-11-09 ###
+Adapter Improvements * Inferring data shapes with single dimension for keras
+adapter - [Issue #265](https://github.com/MLBazaar/MLPrimitives/issues/265) by
+@sarahmish ## 0.3.1 - 2021-10-07 ### Adapter Improvements * Dynamic
+target_shape in keras adapter - [Issue #263](https://github.com/MLBazaar/
+MLPrimitives/issues/263) by @sarahmish * Save keras primitives in Windows
+environment - [Issue #261](https://github.com/MLBazaar/MLPrimitives/issues/261)
+by @sarahmish ### General Imporvements * Update TensorFlow and NumPy dependency
+- [Issue #259](https://github.com/MLBazaar/MLPrimitives/issues/259) by
+@sarahmish ## 0.3.0 - 2021-01-09 ### New Primitives * Add primitive
+`sklearn.naive_bayes.GaussianNB` - [Issue #242](https://github.com/MLBazaar/
+MLPrimitives/issues/242) by @sarahmish * Add primitive
+`sklearn.linear_model.SGDClassifier` - [Issue #241](https://github.com/
+MLBazaar/MLPrimitives/issues/241) by @sarahmish ### Primitive Improvements *
+Add offset to rolling_window_sequence primitive - [Issue #251](https://
+github.com/MLBazaar/MLPrimitives/issues/251) by @skyeeiskowitz * Rename the
+time_index column to time - [Issue #252](https://github.com/MLBazaar/
+MLPrimitives/issues/252) by @pvk-developer * Update featuretools dependency -
+[Issue #250](https://github.com/MLBazaar/MLPrimitives/issues/250) by @pvk-
+developer ### General Improvements * Udpate dependencies and add python3.8 -
+[Issue #246](https://github.com/MLBazaar/MLPrimitives/issues/246) by @csala *
+Drop Python35 - [Issue #244](https://github.com/MLBazaar/MLPrimitives/issues/
+244) by @csala ## 0.2.5 - 2020-07-29 ### Primitive Improvements * Accept
+timedelta `window_size` in `cutoff_window_sequences` - [Issue #239](https://
+github.com/MLBazaar/MLPrimitives/issues/239) by @joanvaquer ### Bug Fixes *
+ImportError: Keras requires TensorFlow 2.2 or higher. Install TensorFlow via
+`pip install tensorflow` - [Issue #237](https://github.com/MLBazaar/
+MLPrimitives/issues/237) by @joanvaquer ### New Primitives * Add
+`pandas.DataFrame.set_index` primitive - [Issue #222](https://github.com/
 MLBazaar/MLPrimitives/issues/222) by @JDTheRipperPC ## 0.2.4 - 2020-01-30 ###
 New Primitives * Add RangeScaler and RangeUnscaler primitives - [Issue #232]
 (https://github.com/MLBazaar/MLPrimitives/issues/232) by @csala ### Primitive
 Improvements * Extract input_shape from X in keras.Sequential - [Issue #223]
 (https://github.com/MLBazaar/MLPrimitives/issues/223) by @csala ### Bug Fixes *
 mlprimitives.custom.text.TextCleaner fails if text is empty - [Issue #228]
 (https://github.com/MLBazaar/MLPrimitives/issues/228) by @csala * Error when
@@ -291,16 +304,8 @@
 pipelines for graph, text and tabular problems. * New primitives ClassEncoder
 and ClassDecoder * New primitives UniqueCounter and VocabularyCounter ### Bug
 Fixes * Fix TrivialPredictor bug when working with numpy arrays * Change XGB
 default learning rate and number of estimators ## 0.1.1 ### New Features * Add
 more keras.applications primitives. * Add a Text Cleanup primitive. ### Bug
 Fixes * Add keywords to `keras.preprocessing` primtives. * Fix the
 `image_transform` method. * Add `epoch` as a fixed hyperparameter for
-`keras.Sequential` primitives. ## 0.1.0 * First release on PyPI. Keywords:
-mlblocks mlprimitives pipelines primitives machine learning data science
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev
+`keras.Sequential` primitives. ## 0.1.0 * First release on PyPI.
```

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives.egg-info/SOURCES.txt` & `mlprimitives-0.3.5/mlprimitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlprimitives-0.3.4.dev0/mlprimitives.egg-info/requires.txt` & `mlprimitives-0.3.5/mlprimitives.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Keras<2.5,>=2.4
 featuretools<0.23,>=0.6.1
 iso639<0.2,>=0.1.4
 langdetect<2,>=1.0.7
 lightfm<2,>=1.15
-mlblocks<0.6,>=0.4.0.dev0
+mlblocks<0.7,>=0.4.0.dev0
 networkx<3,>=2.0
 nltk<4,>=3.3
 numpy<1.21.0,>=1.16.0
 opencv-python<4.7,>=3.4.0.12
 pandas<2,>=1
 python-louvain<0.14,>=0.10
 scikit-image>=0.15
```

