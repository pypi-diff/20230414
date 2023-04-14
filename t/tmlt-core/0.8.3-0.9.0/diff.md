# Comparing `tmp/tmlt_core-0.8.3.tar.gz` & `tmp/tmlt_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_core-0.8.3.tar", max compression
+gzip compressed data, was "tmlt_core-0.9.0.tar", max compression
```

## Comparing `tmlt_core-0.8.3.tar` & `tmlt_core-0.9.0.tar`

### file list

```diff
@@ -1,184 +1,186 @@
--rw-r--r--   0        0        0     9391 2023-03-08 15:46:12.794374 tmlt_core-0.8.3/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-03-08 15:46:12.794374 tmlt_core-0.8.3/LICENSE
--rw-r--r--   0        0        0    20138 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/LICENSE.docs
--rw-r--r--   0        0        0      116 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/NOTICE
--rw-r--r--   0        0        0     1868 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/README.md
--rw-r--r--   0        0        0    11490 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_count_sum.py
--rw-r--r--   0        0        0     3838 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_noise_mechanism.py
--rw-r--r--   0        0        0     8652 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_private_join.py
--rw-r--r--   0        0        0    15620 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_public_join.py
--rw-r--r--   0        0        0     8873 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_quantile.py
--rw-r--r--   0        0        0    10207 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_sparkflatmap.py
--rw-r--r--   0        0        0     9446 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmark_sparkmap.py
--rw-r--r--   0        0        0      731 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/benchmark/benchmarking_utils.py
--rw-r--r--   0        0        0      951 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-03-08 15:46:12.795374 tmlt_core-0.8.3/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/_templates/package-name.html
--rw-r--r--   0        0        0      210 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/additional-resources/index.rst
--rw-r--r--   0        0        0      660 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/additional-resources/license.rst
--rw-r--r--   0        0        0     3159 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/additional-resources/privacy_policy.rst
--rw-r--r--   0        0        0     6889 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/conf.py
--rw-r--r--   0        0        0     1836 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/images/index_api.svg
--rw-r--r--   0        0        0     1186 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/images/index_more.svg
--rw-r--r--   0        0        0      596 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1363 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    30903 2023-03-08 15:46:12.796374 tmlt_core-0.8.3/doc/images/logo.png
--rw-r--r--   0        0        0     3186 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/index.rst
--rw-r--r--   0        0        0     4541 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/installation.rst
--rw-r--r--   0        0        0     6510 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/ref.bib
--rw-r--r--   0        0        0     2006 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3244 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/templates/python/module.rst
--rw-r--r--   0        0        0    16713 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/architecture.rst
--rw-r--r--   0        0        0      345 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/index.rst
--rw-r--r--   0        0        0     1424 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/known-vulnerabilities.rst
--rw-r--r--   0        0        0     6510 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/privacy-guarantee.rst
--rw-r--r--   0        0        0     2289 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/real-numbers.rst
--rw-r--r--   0        0        0     6151 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0     8100 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/topic-guides/special-values.rst
--rw-r--r--   0        0        0     7334 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/tutorials/first-tutorial.rst
--rw-r--r--   0        0        0      231 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/tutorials/index.rst
--rw-r--r--   0        0        0       88 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/doc/zcitations.rst
--rw-r--r--   0        0        0      363 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/ext/build.py
--rw-r--r--   0        0        0     3175 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/ext/build.sh
--rw-r--r--   0        0        0      150 2023-03-08 15:46:12.797374 tmlt_core-0.8.3/ext/dependency_versions.sh
--rw-r--r--   0        0        0     4889 2023-03-08 15:47:02.807316 tmlt_core-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      103 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/__init__.py
--rw-r--r--   0        0        0      110 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/__init__.py
--rw-r--r--   0        0        0     3889 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0      654 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/__init__.py
--rw-r--r--   0        0        0     5468 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_average.py
--rw-r--r--   0        0        0    11426 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_base_mechanisms.py
--rw-r--r--   0        0        0     4671 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_count.py
--rw-r--r--   0        0        0     4849 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_count_distinct.py
--rw-r--r--   0        0        0     5670 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_quantile.py
--rw-r--r--   0        0        0      844 2023-03-08 15:46:12.799374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_samplers.py
--rw-r--r--   0        0        0     6712 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_standard_deviation.py
--rw-r--r--   0        0        0     5197 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_sum.py
--rw-r--r--   0        0        0     7073 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/system/noise_distribution_tests/test_variance.py
--rw-r--r--   0        0        0      108 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/__init__.py
--rw-r--r--   0        0        0      116 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/__init__.py
--rw-r--r--   0        0        0     1176 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/test_base.py
--rw-r--r--   0        0        0     6460 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/test_collections.py
--rw-r--r--   0        0        0     8866 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/test_numpy_domains.py
--rw-r--r--   0        0        0     9777 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/test_pandas_domains.py
--rw-r--r--   0        0        0    26395 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/domains/test_spark_domains.py
--rw-r--r--   0        0        0      121 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/measurements/__init__.py
--rw-r--r--   0        0        0      141 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    13590 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/measurements/pandas_measurements/test_dataframe.py
--rw-r--r--   0        0        0    10159 2023-03-08 15:46:12.800374 tmlt_core-0.8.3/test/unit/measurements/pandas_measurements/test_series.py
--rw-r--r--   0        0        0    42272 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_aggregations.py
--rw-r--r--   0        0        0     7381 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_chaining.py
--rw-r--r--   0        0        0    17665 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_composition.py
--rw-r--r--   0        0        0     8003 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_converters.py
--rw-r--r--   0        0        0    79225 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0    13139 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_noise_mechanisms.py
--rw-r--r--   0        0        0     9458 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_postprocess.py
--rw-r--r--   0        0        0    17410 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/measurements/test_spark_measurements.py
--rw-r--r--   0        0        0      115 2023-03-08 15:46:12.801374 tmlt_core-0.8.3/test/unit/random/__init__.py
--rw-r--r--   0        0        0     1833 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_continuous_gaussian.py
--rw-r--r--   0        0        0     1236 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_discrete_gaussian.py
--rw-r--r--   0        0        0      707 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_inverse_cdf.py
--rw-r--r--   0        0        0     1957 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_laplace.py
--rw-r--r--   0        0        0     1590 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_rng.py
--rw-r--r--   0        0        0      753 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/random/test_uniform.py
--rw-r--r--   0        0        0    15212 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/test_measures.py
--rw-r--r--   0        0        0    90933 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/test_metrics.py
--rw-r--r--   0        0        0      124 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/transformations/__init__.py
--rw-r--r--   0        0        0      146 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    19370 2023-03-08 15:46:12.802374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_add_remove_keys.py
--rw-r--r--   0        0        0    37113 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_agg.py
--rw-r--r--   0        0        0     4748 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_filter.py
--rw-r--r--   0        0        0    16338 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_groupby.py
--rw-r--r--   0        0        0     6832 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_id.py
--rw-r--r--   0        0        0    42138 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_join.py
--rw-r--r--   0        0        0    27193 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_map.py
--rw-r--r--   0        0        0    34028 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_nan.py
--rw-r--r--   0        0        0    12634 2023-03-08 15:46:12.803374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_partition.py
--rw-r--r--   0        0        0     3283 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_persist.py
--rw-r--r--   0        0        0     6053 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_rename.py
--rw-r--r--   0        0        0     4811 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_select.py
--rw-r--r--   0        0        0    17751 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_truncation.py
--rw-r--r--   0        0        0     7952 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/test_chaining.py
--rw-r--r--   0        0        0     3922 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/test_converters.py
--rw-r--r--   0        0        0    39668 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/test_dictionary.py
--rw-r--r--   0        0        0     1936 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/transformations/test_identity.py
--rw-r--r--   0        0        0      114 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/__init__.py
--rw-r--r--   0        0        0     8418 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_arb.py
--rw-r--r--   0        0        0     5700 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_cleanup.py
--rw-r--r--   0        0        0     9909 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_configuration.py
--rw-r--r--   0        0        0     8733 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_distributions.py
--rw-r--r--   0        0        0     6032 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_exact_number.py
--rw-r--r--   0        0        0     9346 2023-03-08 15:46:12.804374 tmlt_core-0.8.3/test/unit/utils/test_grouped_dataframe.py
--rw-r--r--   0        0        0     2380 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/test/unit/utils/test_misc.py
--rw-r--r--   0        0        0     1054 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/test/unit/utils/test_testing.py
--rw-r--r--   0        0        0     3676 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/test/unit/utils/test_truncation.py
--rw-r--r--   0        0        0     1837 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/test/unit/utils/test_type_utils.py
--rw-r--r--   0        0        0       37 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/test_requirements.txt
--rw-r--r--   0        0        0      376 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/__init__.py
--rw-r--r--   0        0        0       83 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/__init__.py
--rw-r--r--   0        0        0     1004 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/base.py
--rw-r--r--   0        0        0     3281 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/collections.py
--rw-r--r--   0        0        0     3926 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/numpy_domains.py
--rw-r--r--   0        0        0     4425 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/pandas_domains.py
--rw-r--r--   0        0        0    25471 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/domains/spark_domains.py
--rw-r--r--   0        0        0       88 2023-03-08 15:46:12.805374 tmlt_core-0.8.3/tmlt/core/measurements/__init__.py
--rw-r--r--   0        0        0    82707 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/aggregations.py
--rw-r--r--   0        0        0     2943 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/base.py
--rw-r--r--   0        0        0     5013 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/chaining.py
--rw-r--r--   0        0        0     6708 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/composition.py
--rw-r--r--   0        0        0     8465 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/converters.py
--rw-r--r--   0        0        0    73806 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/interactive_measurements.py
--rw-r--r--   0        0        0    16951 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/noise_mechanisms.py
--rw-r--r--   0        0        0      120 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    10140 2023-03-08 15:46:12.806374 tmlt_core-0.8.3/tmlt/core/measurements/pandas_measurements/dataframe.py
--rw-r--r--   0        0        0    15946 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/measurements/pandas_measurements/series.py
--rw-r--r--   0        0        0     7411 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/measurements/postprocess.py
--rw-r--r--   0        0        0    22751 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/measurements/spark_measurements.py
--rw-r--r--   0        0        0    13275 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/measures.py
--rw-r--r--   0        0        0    54816 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/metrics.py
--rw-r--r--   0        0        0        0 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/py.typed
--rw-r--r--   0        0        0      119 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/__init__.py
--rw-r--r--   0        0        0     2551 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/continuous_gaussian.py
--rw-r--r--   0        0        0    16943 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/discrete_gaussian.py
--rw-r--r--   0        0        0     1499 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/inverse_cdf.py
--rw-r--r--   0        0        0     2134 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/laplace.py
--rw-r--r--   0        0        0      619 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/rng.py
--rw-r--r--   0        0        0     1675 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/random/uniform.py
--rw-r--r--   0        0        0       91 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/transformations/__init__.py
--rw-r--r--   0        0        0     4041 2023-03-08 15:46:12.807374 tmlt_core-0.8.3/tmlt/core/transformations/base.py
--rw-r--r--   0        0        0     4646 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/chaining.py
--rw-r--r--   0        0        0     3279 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/converters.py
--rw-r--r--   0        0        0    27820 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/dictionary.py
--rw-r--r--   0        0        0     1160 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/identity.py
--rw-r--r--   0        0        0      125 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    35021 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/add_remove_keys.py
--rw-r--r--   0        0        0    44309 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/agg.py
--rw-r--r--   0        0        0     5838 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/filter.py
--rw-r--r--   0        0        0    16867 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/groupby.py
--rw-r--r--   0        0        0     5680 2023-03-08 15:46:12.808374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/id.py
--rw-r--r--   0        0        0    45174 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/join.py
--rw-r--r--   0        0        0    38149 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/map.py
--rw-r--r--   0        0        0    40461 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/nan.py
--rw-r--r--   0        0        0     9704 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/partition.py
--rw-r--r--   0        0        0     3862 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/persist.py
--rw-r--r--   0        0        0     6769 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/rename.py
--rw-r--r--   0        0        0     5800 2023-03-08 15:46:12.809374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/select.py
--rw-r--r--   0        0        0    22134 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/truncation.py
--rw-r--r--   0        0        0       85 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/__init__.py
--rw-r--r--   0        0        0    16306 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/arb.py
--rw-r--r--   0        0        0     1147 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/cleanup.py
--rw-r--r--   0        0        0     5899 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/configuration.py
--rw-r--r--   0        0        0     9286 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/distributions.py
--rw-r--r--   0        0        0    15002 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/exact_number.py
--rw-r--r--   0        0        0    10554 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/grouped_dataframe.py
--rw-r--r--   0        0        0     3194 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/misc.py
--rw-r--r--   0        0        0     3551 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/parameters.py
--rw-r--r--   0        0        0    32356 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/testing.py
--rw-r--r--   0        0        0     7359 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/truncation.py
--rw-r--r--   0        0        0     2804 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/type_utils.py
--rw-r--r--   0        0        0     6215 2023-03-08 15:46:12.810374 tmlt_core-0.8.3/tmlt/core/utils/validation.py
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    10069 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0    20138 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/LICENSE.docs
+-rw-r--r--   0        0        0      116 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/NOTICE
+-rw-r--r--   0        0        0     1868 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/README.md
+-rw-r--r--   0        0        0    11481 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/benchmark/benchmark_count_sum.py
+-rw-r--r--   0        0        0     3838 2023-04-14 16:44:30.148892 tmlt_core-0.9.0/benchmark/benchmark_noise_mechanism.py
+-rw-r--r--   0        0        0     8652 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_private_join.py
+-rw-r--r--   0        0        0    15676 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_public_join.py
+-rw-r--r--   0        0        0     8873 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_quantile.py
+-rw-r--r--   0        0        0    10207 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_sparkflatmap.py
+-rw-r--r--   0        0        0     9446 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmark_sparkmap.py
+-rw-r--r--   0        0        0      731 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/benchmark/benchmarking_utils.py
+-rw-r--r--   0        0        0      951 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-04-14 16:44:30.149892 tmlt_core-0.9.0/doc/_templates/package-name.html
+-rw-r--r--   0        0        0      210 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/index.rst
+-rw-r--r--   0        0        0      660 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/license.rst
+-rw-r--r--   0        0        0     3159 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/additional-resources/privacy_policy.rst
+-rw-r--r--   0        0        0     6889 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/conf.py
+-rw-r--r--   0        0        0     1836 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_api.svg
+-rw-r--r--   0        0        0     1186 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_more.svg
+-rw-r--r--   0        0        0      596 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1363 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    30903 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/images/logo.png
+-rw-r--r--   0        0        0     3186 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/index.rst
+-rw-r--r--   0        0        0     4541 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/installation.rst
+-rw-r--r--   0        0        0     6510 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/ref.bib
+-rw-r--r--   0        0        0     2006 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3244 2023-04-14 16:44:30.150892 tmlt_core-0.9.0/doc/templates/python/module.rst
+-rw-r--r--   0        0        0    16713 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/architecture.rst
+-rw-r--r--   0        0        0      345 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0     1424 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/known-vulnerabilities.rst
+-rw-r--r--   0        0        0     6510 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/privacy-guarantee.rst
+-rw-r--r--   0        0        0     2289 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/real-numbers.rst
+-rw-r--r--   0        0        0     6151 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0     8100 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/topic-guides/special-values.rst
+-rw-r--r--   0        0        0     7334 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/tutorials/first-tutorial.rst
+-rw-r--r--   0        0        0      231 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/tutorials/index.rst
+-rw-r--r--   0        0        0       88 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/doc/zcitations.rst
+-rw-r--r--   0        0        0      363 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/build.py
+-rw-r--r--   0        0        0     3175 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/build.sh
+-rw-r--r--   0        0        0      150 2023-04-14 16:44:30.151892 tmlt_core-0.9.0/ext/dependency_versions.sh
+-rw-r--r--   0        0        0     4909 2023-04-14 16:45:17.001831 tmlt_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-04-14 16:44:30.152892 tmlt_core-0.9.0/test/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-14 16:44:30.152892 tmlt_core-0.9.0/test/system/__init__.py
+-rw-r--r--   0        0        0     3889 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0      654 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/__init__.py
+-rw-r--r--   0        0        0     5468 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_average.py
+-rw-r--r--   0        0        0    11426 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_base_mechanisms.py
+-rw-r--r--   0        0        0     4671 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count.py
+-rw-r--r--   0        0        0     4849 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count_distinct.py
+-rw-r--r--   0        0        0     5670 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_quantile.py
+-rw-r--r--   0        0        0      844 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_samplers.py
+-rw-r--r--   0        0        0     6706 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_standard_deviation.py
+-rw-r--r--   0        0        0     5197 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_sum.py
+-rw-r--r--   0        0        0     7067 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/system/noise_distribution_tests/test_variance.py
+-rw-r--r--   0        0        0      108 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/__init__.py
+-rw-r--r--   0        0        0     1176 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_base.py
+-rw-r--r--   0        0        0     6558 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_collections.py
+-rw-r--r--   0        0        0     8866 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_numpy_domains.py
+-rw-r--r--   0        0        0     9857 2023-04-14 16:44:30.153892 tmlt_core-0.9.0/test/unit/domains/test_pandas_domains.py
+-rw-r--r--   0        0        0    26425 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/domains/test_spark_domains.py
+-rw-r--r--   0        0        0      121 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    13818 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_dataframe.py
+-rw-r--r--   0        0        0    10203 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_series.py
+-rw-r--r--   0        0        0    42343 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_aggregations.py
+-rw-r--r--   0        0        0     7429 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_chaining.py
+-rw-r--r--   0        0        0    17787 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_composition.py
+-rw-r--r--   0        0        0     8003 2023-04-14 16:44:30.154892 tmlt_core-0.9.0/test/unit/measurements/test_converters.py
+-rw-r--r--   0        0        0    80698 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0    13139 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_noise_mechanisms.py
+-rw-r--r--   0        0        0     9458 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_postprocess.py
+-rw-r--r--   0        0        0    17510 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/measurements/test_spark_measurements.py
+-rw-r--r--   0        0        0      115 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/__init__.py
+-rw-r--r--   0        0        0     1833 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_continuous_gaussian.py
+-rw-r--r--   0        0        0     1235 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_discrete_gaussian.py
+-rw-r--r--   0        0        0      707 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_inverse_cdf.py
+-rw-r--r--   0        0        0     1957 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_laplace.py
+-rw-r--r--   0        0        0     1590 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_rng.py
+-rw-r--r--   0        0        0      753 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/random/test_uniform.py
+-rw-r--r--   0        0        0    15212 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/test_measures.py
+-rw-r--r--   0        0        0    91233 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/test_metrics.py
+-rw-r--r--   0        0        0      124 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/transformations/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-14 16:44:30.155892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    22382 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_add_remove_keys.py
+-rw-r--r--   0        0        0    37109 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_agg.py
+-rw-r--r--   0        0        0     4748 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_filter.py
+-rw-r--r--   0        0        0    16386 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_groupby.py
+-rw-r--r--   0        0        0     6832 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_id.py
+-rw-r--r--   0        0        0    50620 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_join.py
+-rw-r--r--   0        0        0    27295 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_map.py
+-rw-r--r--   0        0        0    34292 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_nan.py
+-rw-r--r--   0        0        0    12670 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_partition.py
+-rw-r--r--   0        0        0     3331 2023-04-14 16:44:30.156892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_persist.py
+-rw-r--r--   0        0        0     6053 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_rename.py
+-rw-r--r--   0        0        0     4811 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_select.py
+-rw-r--r--   0        0        0    17751 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_truncation.py
+-rw-r--r--   0        0        0     8000 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_chaining.py
+-rw-r--r--   0        0        0     3922 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_converters.py
+-rw-r--r--   0        0        0    39837 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_dictionary.py
+-rw-r--r--   0        0        0     1936 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/transformations/test_identity.py
+-rw-r--r--   0        0        0      114 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/__init__.py
+-rw-r--r--   0        0        0     8396 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_arb.py
+-rw-r--r--   0        0        0     5700 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_cleanup.py
+-rw-r--r--   0        0        0    10005 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_configuration.py
+-rw-r--r--   0        0        0     8733 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_distributions.py
+-rw-r--r--   0        0        0     6032 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_exact_number.py
+-rw-r--r--   0        0        0    13458 2023-04-14 16:44:30.157892 tmlt_core-0.9.0/test/unit/utils/test_grouped_dataframe.py
+-rw-r--r--   0        0        0    37873 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_join.py
+-rw-r--r--   0        0        0     2424 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_misc.py
+-rw-r--r--   0        0        0     1054 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_testing.py
+-rw-r--r--   0        0        0     4466 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_truncation.py
+-rw-r--r--   0        0        0     1837 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test/unit/utils/test_type_utils.py
+-rw-r--r--   0        0        0       37 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/test_requirements.txt
+-rw-r--r--   0        0        0      376 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/__init__.py
+-rw-r--r--   0        0        0       83 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/__init__.py
+-rw-r--r--   0        0        0      992 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/base.py
+-rw-r--r--   0        0        0     3425 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/collections.py
+-rw-r--r--   0        0        0     3926 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/numpy_domains.py
+-rw-r--r--   0        0        0     4489 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/pandas_domains.py
+-rw-r--r--   0        0        0    25759 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/domains/spark_domains.py
+-rw-r--r--   0        0        0       88 2023-04-14 16:44:30.158892 tmlt_core-0.9.0/tmlt/core/measurements/__init__.py
+-rw-r--r--   0        0        0    83528 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/aggregations.py
+-rw-r--r--   0        0        0     2931 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/base.py
+-rw-r--r--   0        0        0     5020 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/chaining.py
+-rw-r--r--   0        0        0     6728 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/composition.py
+-rw-r--r--   0        0        0     8463 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/converters.py
+-rw-r--r--   0        0        0    73838 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/interactive_measurements.py
+-rw-r--r--   0        0        0    17009 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/noise_mechanisms.py
+-rw-r--r--   0        0        0      120 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    10135 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/dataframe.py
+-rw-r--r--   0        0        0    15934 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/series.py
+-rw-r--r--   0        0        0     7411 2023-04-14 16:44:30.159892 tmlt_core-0.9.0/tmlt/core/measurements/postprocess.py
+-rw-r--r--   0        0        0    22812 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/measurements/spark_measurements.py
+-rw-r--r--   0        0        0    13254 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/measures.py
+-rw-r--r--   0        0        0    54917 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/metrics.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/py.typed
+-rw-r--r--   0        0        0      119 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/continuous_gaussian.py
+-rw-r--r--   0        0        0    16941 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/discrete_gaussian.py
+-rw-r--r--   0        0        0     1497 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/inverse_cdf.py
+-rw-r--r--   0        0        0     2132 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/laplace.py
+-rw-r--r--   0        0        0      619 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/rng.py
+-rw-r--r--   0        0        0     1673 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/random/uniform.py
+-rw-r--r--   0        0        0       91 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/__init__.py
+-rw-r--r--   0        0        0     4029 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/base.py
+-rw-r--r--   0        0        0     4653 2023-04-14 16:44:30.160892 tmlt_core-0.9.0/tmlt/core/transformations/chaining.py
+-rw-r--r--   0        0        0     3277 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/converters.py
+-rw-r--r--   0        0        0    27820 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/dictionary.py
+-rw-r--r--   0        0        0     1160 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/identity.py
+-rw-r--r--   0        0        0      125 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    34915 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/add_remove_keys.py
+-rw-r--r--   0        0        0    44303 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/agg.py
+-rw-r--r--   0        0        0     5860 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/filter.py
+-rw-r--r--   0        0        0    16865 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/groupby.py
+-rw-r--r--   0        0        0     5680 2023-04-14 16:44:30.161892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/id.py
+-rw-r--r--   0        0        0    39943 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/join.py
+-rw-r--r--   0        0        0    40011 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/map.py
+-rw-r--r--   0        0        0    40713 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/nan.py
+-rw-r--r--   0        0        0     9724 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/partition.py
+-rw-r--r--   0        0        0     3862 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/persist.py
+-rw-r--r--   0        0        0     6769 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/rename.py
+-rw-r--r--   0        0        0     5800 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/select.py
+-rw-r--r--   0        0        0    22134 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/truncation.py
+-rw-r--r--   0        0        0       85 2023-04-14 16:44:30.162892 tmlt_core-0.9.0/tmlt/core/utils/__init__.py
+-rw-r--r--   0        0        0    16349 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/arb.py
+-rw-r--r--   0        0        0     1181 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/cleanup.py
+-rw-r--r--   0        0        0     6030 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/configuration.py
+-rw-r--r--   0        0        0     9303 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/distributions.py
+-rw-r--r--   0        0        0    15026 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/exact_number.py
+-rw-r--r--   0        0        0     9403 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/grouped_dataframe.py
+-rw-r--r--   0        0        0    20371 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/join.py
+-rw-r--r--   0        0        0     3190 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/misc.py
+-rw-r--r--   0        0        0     3551 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/parameters.py
+-rw-r--r--   0        0        0    32413 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/testing.py
+-rw-r--r--   0        0        0     7707 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/truncation.py
+-rw-r--r--   0        0        0     2796 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/type_utils.py
+-rw-r--r--   0        0        0     6215 2023-04-14 16:44:30.163892 tmlt_core-0.9.0/tmlt/core/utils/validation.py
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.9.0/PKG-INFO
```

### Comparing `tmlt_core-0.8.3/CHANGELOG.rst` & `tmlt_core-0.9.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 .. _core-changelog:
 
 Changelog
 =========
 
+0.9.0 - 2023-04-14
+------------------
+
+Added
+~~~~~
+
+- :mod:`~.utils.join`, which contains utilities for validating join parameters, propogating domains through joins, and joining dataframes.
+
+Changed
+~~~~~~~
+
+- :func:`~.truncate_large_groups` does not clump identical records together in hash-based ordering.
+- :class:`~.TransformValue` no longer fails when renaming the id column using :class:`~.RenameValue`.
+
+Fixed
+~~~~~
+
+- groupby no longer outputs nan values when both tables are views on the same original table
+- private join no longer drops Nulls on non-join columns when join_on_nulls=False
+- groupby average and variance no longer drops groups containing null values
+
 0.8.3 - 2023-03-08
 ------------------
 
 Changed
 ~~~~~~~
 
 - Functions in :mod:`~.aggregations` now support :class:`~.ApproxDP`.
```

### Comparing `tmlt_core-0.8.3/LICENSE` & `tmlt_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/LICENSE.docs` & `tmlt_core-0.9.0/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/README.md` & `tmlt_core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_count_sum.py` & `tmlt_core-0.9.0/benchmark/benchmark_count_sum.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from pyspark.sql import SparkSession
 from pyspark.sql import functions as sf
 from pyspark.sql.dataframe import DataFrame
-from pyspark.sql.types import IntegerType, StructField, StructType
+from pyspark.sql.types import LongType, StructField, StructType
 
 from benchmarking_utils import Timer, write_as_html
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkIntegerColumnDescriptor,
 )
 from tmlt.core.metrics import SymmetricDifference
@@ -236,15 +236,15 @@
         groupby_columns = ["Col_{}".format(i) for i in range(num_cols)]
         columns = groupby_columns + ["X"]
         input_domain = SparkDataFrameDomain(
             dict.fromkeys(columns, SparkIntegerColumnDescriptor())
         )
         schema = StructType(
             [
-                StructField("Col_{}".format(i), IntegerType(), True)
+                StructField("Col_{}".format(i), LongType(), True)
                 for i in range(num_cols)
             ]
         )
         sdf = spark.createDataFrame(  # pylint: disable=no-member
             spark.sparkContext.parallelize(
                 np.repeat(
                     np.transpose(
@@ -288,15 +288,15 @@
         groupby_columns = ["Col_{}".format(i) for i in range(num_cols)]
         columns = groupby_columns + ["X"]
         input_domain = SparkDataFrameDomain(
             dict.fromkeys(columns, SparkIntegerColumnDescriptor())
         )
         schema = StructType(
             [
-                StructField("Col_{}".format(i), IntegerType(), True)
+                StructField("Col_{}".format(i), LongType(), True)
                 for i in range(num_cols)
             ]
         )
         sdf = spark.createDataFrame(  # pylint: disable=no-member
             spark.sparkContext.parallelize(
                 np.repeat(
                     np.transpose(
```

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_noise_mechanism.py` & `tmlt_core-0.9.0/benchmark/benchmark_noise_mechanism.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_private_join.py` & `tmlt_core-0.9.0/benchmark/benchmark_private_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_public_join.py` & `tmlt_core-0.9.0/benchmark/benchmark_public_join.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from random import randint
 from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 from pyspark.sql import SparkSession
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql.functions import lit
+from pyspark.sql.types import LongType
 from benchmarking_utils import write_as_html
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
@@ -205,15 +206,15 @@
             for cols in columns_private:
                 schema = {f"Col_{i}": SparkFloatColumnDescriptor() for i in range(cols)}
                 private_df = self.spark.createDataFrame(  # pylint: disable=no-member
                     pd.DataFrame(
                         [tuple(range(cols))] * rows_in_private, columns=schema.keys()
                     )
                 )
-                private_df = private_df.withColumn("B", lit(randint(0, 1)))
+                private_df = private_df.withColumn("B", lit(randint(0, 1)).cast(LongType()))
                 schema["B"] = SparkIntegerColumnDescriptor()
                 input_domain = SparkDataFrameDomain(schema=schema)
                 metric = IfGroupedBy("B", SumOf(SymmetricDifference()))
                 join_cols = ["B"]
                 transform_time, running_time = self.evaluate_runtime(
                     input_domain=input_domain,
                     public_df=self.spark.createDataFrame(public_df),
```

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_quantile.py` & `tmlt_core-0.9.0/benchmark/benchmark_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_sparkflatmap.py` & `tmlt_core-0.9.0/benchmark/benchmark_sparkflatmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmark_sparkmap.py` & `tmlt_core-0.9.0/benchmark/benchmark_sparkmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/benchmark/benchmarking_utils.py` & `tmlt_core-0.9.0/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/_static/css/custom.css` & `tmlt_core-0.9.0/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/_static/favicon.ico` & `tmlt_core-0.9.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/_static/js/version-banner.js` & `tmlt_core-0.9.0/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/_static/logo.png` & `tmlt_core-0.9.0/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/additional-resources/license.rst` & `tmlt_core-0.9.0/doc/additional-resources/license.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/additional-resources/privacy_policy.rst` & `tmlt_core-0.9.0/doc/additional-resources/privacy_policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/conf.py` & `tmlt_core-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/images/index_api.svg` & `tmlt_core-0.9.0/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/images/index_more.svg` & `tmlt_core-0.9.0/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/images/index_topic_guides.svg` & `tmlt_core-0.9.0/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/images/index_tutorials.svg` & `tmlt_core-0.9.0/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/images/logo.png` & `tmlt_core-0.9.0/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/index.rst` & `tmlt_core-0.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/installation.rst` & `tmlt_core-0.9.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/ref.bib` & `tmlt_core-0.9.0/doc/ref.bib`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/templates/python/class.rst` & `tmlt_core-0.9.0/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/templates/python/module.rst` & `tmlt_core-0.9.0/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/architecture.rst` & `tmlt_core-0.9.0/doc/topic-guides/architecture.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/known-vulnerabilities.rst` & `tmlt_core-0.9.0/doc/topic-guides/known-vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/privacy-guarantee.rst` & `tmlt_core-0.9.0/doc/topic-guides/privacy-guarantee.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/real-numbers.rst` & `tmlt_core-0.9.0/doc/topic-guides/real-numbers.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/spark.rst` & `tmlt_core-0.9.0/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/topic-guides/special-values.rst` & `tmlt_core-0.9.0/doc/topic-guides/special-values.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/doc/tutorials/first-tutorial.rst` & `tmlt_core-0.9.0/doc/tutorials/first-tutorial.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/ext/build.sh` & `tmlt_core-0.9.0/ext/build.sh`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/pyproject.toml` & `tmlt_core-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Tumult's differential privacy primitives"
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 repository = "https://gitlab.com/tumult-labs/core"
 documentation = "https://docs.tmlt.dev/core/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.8.3"
+version = "0.9.0"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
    "Topic :: Software Development :: Libraries",
@@ -62,19 +62,19 @@
 
 [tool.poetry.dev-dependencies]
 # Build scripting
 nox = "2022.8.7"
 nox_poetry = "1.0.1"
 
 # Linters, formatters
-black = "21.9b0"
-isort = { version = "4.3.21", extras = ["pyproject"] }
-mypy = "0.940"
-pydocstyle = { version = "6.1.1", extras = ["toml"] }
-pylint = "2.5.3"
+black = "^23"
+isort = { version = "^5.11", extras = ["pyproject"] }
+mypy = "^1.2"
+pydocstyle = { version = "^6.3", extras = ["toml"] }
+pylint = "^2.13"
 
 # Testing
 coverage = "^6.5"
 nose = "^1.3.7"
 parameterized = "^0.7.4"
 
 # Docs
@@ -111,14 +111,15 @@
 line_length = 88
 
 [tool.mypy]
 explicit_package_bases = true
 follow_imports = "silent"
 ignore_missing_imports = true
 namespace_packages = true
+check_untyped_defs = true
 
 [tool.pylint.master]
 # See https://github.com/PyCQA/pylint/issues/1975#issuecomment-387924981
 extension-pkg-whitelist = ['numpy']
 load-plugins = ['pylint.extensions.docparams']
 # Only check param docs in docstrings that contain an Args: section.
 # Set to "no" to show docstrings missing argument documentation.
```

### Comparing `tmlt_core-0.8.3/test/system/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.0/test/system/measurements/test_interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/__init__.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_average.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_average.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_base_mechanisms.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_base_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_count.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_count_distinct.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_count_distinct.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_quantile.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_samplers.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_standard_deviation.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_standard_deviation.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,24 +88,24 @@
             sum_of_squared_deviations_column="sos",
             count_column="count",
         )
 
         true_answers: Dict[str, Union[float, int]] = {
             "count": len(dataset.group_vals),
             "sum": sum(dataset.group_vals),
-            "sum_of_squares": sum(val ** 2 for val in dataset.group_vals),
+            "sum_of_squares": sum(val**2 for val in dataset.group_vals),
         }
         midpoint_sod, _ = get_midpoint(
             dataset.lower,
             dataset.upper,
             integer_midpoint=not dataset.float_measure_column,
         )
         midpoint_sos, _ = get_midpoint(
-            0 if dataset.lower <= 0 <= dataset.upper else dataset.lower ** 2,
-            dataset.upper ** 2,
+            0 if dataset.lower <= 0 <= dataset.upper else dataset.lower**2,
+            dataset.upper**2,
             integer_midpoint=not dataset.float_measure_column,
         )
 
         def postprocessor(
             df: DataFrame,
             count: int = count_loc,
             midpoint_sod: float = midpoint_sod,
```

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_sum.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/system/noise_distribution_tests/test_variance.py` & `tmlt_core-0.9.0/test/system/noise_distribution_tests/test_variance.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,24 +88,24 @@
             sum_of_squared_deviations_column="sos",
             count_column="count",
         )
 
         true_answers: Dict[str, Union[float, int]] = {
             "count": len(dataset.group_vals),
             "sum": sum(dataset.group_vals),
-            "sum_of_squares": sum(val ** 2 for val in dataset.group_vals),
+            "sum_of_squares": sum(val**2 for val in dataset.group_vals),
         }
         midpoint_sod, _ = get_midpoint(
             dataset.lower,
             dataset.upper,
             integer_midpoint=not dataset.float_measure_column,
         )
         midpoint_sos, _ = get_midpoint(
-            0 if dataset.lower <= 0 <= dataset.upper else dataset.lower ** 2,
-            dataset.upper ** 2,
+            0 if dataset.lower <= 0 <= dataset.upper else dataset.lower**2,
+            dataset.upper**2,
             integer_midpoint=not dataset.float_measure_column,
         )
 
         def postprocessor(
             df: DataFrame,
             count: int = count_loc,
             midpoint_sod: float = midpoint_sod,
```

### Comparing `tmlt_core-0.8.3/test/unit/domains/test_base.py` & `tmlt_core-0.9.0/test/unit/domains/test_base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/domains/test_collections.py` & `tmlt_core-0.9.0/test/unit/domains/test_collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 import numpy as np
 from parameterized import parameterized
 from pyspark.sql.types import StringType
 
 from tmlt.core.domains.base import Domain, OutOfDomainError
 from tmlt.core.domains.collections import DictDomain, ListDomain
-from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
+from tmlt.core.domains.numpy_domains import (
+    NumpyDomain,
+    NumpyFloatDomain,
+    NumpyIntegerDomain,
+)
 from tmlt.core.utils.testing import assert_property_immutability, get_all_props
 
 
 class TestListDomain(TestCase):
     """Tests for :class:`~tmlt.core.domains.collections.ListDomain`."""
 
     def setUp(self):
@@ -42,16 +46,18 @@
 
     @parameterized.expand(
         [
             ([np.int64(1)], None),
             ("Not a list", f"Value must be {list}, instead it is {str}."),
             (
                 ["invalid"],
-                f"Found invalid value in list: Value must be {np.int64}, "
-                f"instead it is {str}.",
+                (
+                    f"Found invalid value in list: Value must be {np.int64}, "
+                    f"instead it is {str}."
+                ),
             ),
         ]
     )
     def test_validate(self, candidate: Any, exception: Optional[str]):
         """Tests that validate works correctly."""
         if exception is not None:
             with self.assertRaisesRegex(OutOfDomainError, exception):
@@ -67,15 +73,15 @@
         """Setup."""
         self.domain_a = create_autospec(spec=Domain, instance=True)
         self.domain_b = create_autospec(spec=Domain, instance=True)
         self.dict_domain = DictDomain({"A": self.domain_a, "B": self.domain_b})
 
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
-        domain_map = {"A": NumpyIntegerDomain()}
+        domain_map: Dict[str, NumpyDomain] = {"A": NumpyIntegerDomain()}
         domain = DictDomain(key_to_domain=domain_map)
         domain_map["A"] = NumpyFloatDomain()
         self.assertDictEqual(domain.key_to_domain, {"A": NumpyIntegerDomain()})
 
     @parameterized.expand(get_all_props(DictDomain))
     def test_property_immutability(self, prop_name: str):
         """Tests that given property is immutable."""
@@ -109,15 +115,15 @@
             self.dict_domain.validate(candidate)
         else:
             issue_object = "'B'" if in_A else "'A'"
             exception = f"Found invalid value at {issue_object}: Test"
             if set(candidate) != {"A", "B"}:
                 exception = (
                     "Keys are not as expected, value must match domain.\n"
-                    fr"Value keys: \[{str(sorted(set(candidate)))[1:-1]}\]"
+                    rf"Value keys: \[{str(sorted(set(candidate)))[1:-1]}\]"
                     "\n"
                     r"Domain keys: \['A', 'B'\]"
                 )
             with self.assertRaisesRegex(OutOfDomainError, exception):
                 self.dict_domain.validate(candidate)
 
         if set(candidate) == {"A", "B"}:
```

### Comparing `tmlt_core-0.8.3/test/unit/domains/test_numpy_domains.py` & `tmlt_core-0.9.0/test/unit/domains/test_numpy_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/domains/test_pandas_domains.py` & `tmlt_core-0.9.0/test/unit/domains/test_pandas_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,37 +153,39 @@
             }
         )
 
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
         schema = {"A": PandasSeriesDomain(NumpyIntegerDomain())}
         domain = PandasDataFrameDomain(schema=schema)
-        schema["A"] = NumpyFloatDomain()
+        schema["A"] = PandasSeriesDomain(NumpyFloatDomain())
         self.assertDictEqual(
             domain.schema, {"A": PandasSeriesDomain(NumpyIntegerDomain())}
         )
 
     @parameterized.expand(get_all_props(PandasDataFrameDomain))
     def test_property_immutability(self, prop_name: str):
         """Tests that given property is immutable."""
         assert_property_immutability(self.pdfd, prop_name)
 
     def test_bad_init(self):
         """Test that PandasDataFrameDomain raises error when create with wrong type."""
         with self.assertRaises(TypeError):
-            PandasDataFrameDomain(schema="incorrect type")
+            PandasDataFrameDomain(schema="incorrect type")  # type: ignore
 
     @parameterized.expand(
         [
             (pd.DataFrame({"A": [1, 2], "B": [1.0, 2.0], "C": ["1", "2"]}), None),
             # wrong column type
             (
                 pd.DataFrame({"A": [1, 2], "B": [1, 2], "C": ["1", "2"]}),
-                "Found invalid value in column 'B': Found invalid value in Series: "
-                f"Value must be {np.float64}, instead it is {np.int64}.",
+                (
+                    "Found invalid value in column 'B': Found invalid value in Series: "
+                    f"Value must be {np.float64}, instead it is {np.int64}."
+                ),
             ),
             # missing column
             (
                 pd.DataFrame({"A": [1, 2], "B": [1.0, 2.0]}),
                 "Columns are not as expected. DataFrame and Domain must contain the "
                 r"same columns in the same order.\nDataFrame columns: \['A', 'B'\]\n"
                 r"Domain columns: \['A', 'B', 'C'\]",
```

### Comparing `tmlt_core-0.8.3/test/unit/domains/test_spark_domains.py` & `tmlt_core-0.9.0/test/unit/domains/test_spark_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
         schema = {
             "A": SparkIntegerColumnDescriptor(),
             "B": SparkStringColumnDescriptor(),
         }
         domain = SparkDataFrameDomain(schema=schema)
-        schema["A"] = NumpyFloatDomain()
+        schema["A"] = SparkFloatColumnDescriptor()
         self.assertDictEqual(
             domain.schema,
             {"A": SparkIntegerColumnDescriptor(), "B": SparkStringColumnDescriptor()},
         )
 
     @parameterized.expand(get_all_props(SparkDataFrameDomain))
     def test_property_immutability(self, prop_name: str):
@@ -102,15 +102,15 @@
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
         schema = {
             "A": SparkIntegerColumnDescriptor(),
             "B": SparkStringColumnDescriptor(),
         }
         domain = SparkRowDomain(schema=schema)
-        schema["A"] = NumpyFloatDomain()
+        schema["A"] = SparkFloatColumnDescriptor()
         self.assertDictEqual(
             domain.schema,
             {"A": SparkIntegerColumnDescriptor(), "B": SparkStringColumnDescriptor()},
         )
 
     @parameterized.expand(get_all_props(SparkRowDomain))
     def test_property_immutability(self, prop_name: str):
@@ -291,15 +291,15 @@
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
         schema = {
             "A": SparkIntegerColumnDescriptor(),
             "B": SparkStringColumnDescriptor(),
         }
         domain = SparkGroupedDataFrameDomain(schema=schema, group_keys=self.group_keys)
-        schema["A"] = NumpyFloatDomain()
+        schema["A"] = SparkFloatColumnDescriptor()
         self.assertDictEqual(
             domain.schema,
             {"A": SparkIntegerColumnDescriptor(), "B": SparkStringColumnDescriptor()},
         )
 
     @parameterized.expand(get_all_props(SparkGroupedDataFrameDomain))
     def test_property_immutability(self, prop_name: str):
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/pandas_measurements/test_dataframe.py` & `tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class TestAggregateByColumn(unittest.TestCase):
     """Tests measurements on pandas dataframes.
 
     Tests :class:`~tmlt.core.measurements.pandas_measurements.dataframe.Aggregate`.
     """
 
     @parameterized.expand(get_all_props(AggregateByColumn))
-    def test_property_immutability(self, prop_name: str):
+    def test_property_immutability(self, prop_name: str) -> None:
         """Tests that given property is immutable."""
         quantile_measurement = NoisyQuantile(
             PandasSeriesDomain(NumpyIntegerDomain()),
             output_measure=PureDP(),
             quantile=0.5,
             lower=22,
             upper=29,
@@ -90,15 +90,15 @@
                     "C": PandasSeriesDomain(NumpyStringDomain()),
                 }
             ),
             column_to_aggregation=column_to_aggregation,
         )
         assert_property_immutability(measurement, prop_name)
 
-    def test_properties(self):
+    def test_properties(self) -> None:
         """AggregateByColumn's properties have the expected values."""
         quantile_measurement = NoisyQuantile(
             PandasSeriesDomain(NumpyIntegerDomain()),
             output_measure=PureDP(),
             quantile=0.5,
             lower=22,
             upper=29,
@@ -120,15 +120,15 @@
         )
         self.assertEqual(measurement.input_domain, input_domain)
         self.assertEqual(measurement.input_metric, SymmetricDifference())
         self.assertEqual(measurement.output_measure, PureDP())
         self.assertEqual(measurement.is_interactive, False)
         self.assertEqual(measurement.column_to_aggregation, column_to_aggregation)
 
-    def test_output_schema(self):
+    def test_output_schema(self) -> None:
         """Test that the output schema is constructed correctly."""
         quantile_measurement = NoisyQuantile(
             PandasSeriesDomain(NumpyIntegerDomain()),
             output_measure=PureDP(),
             quantile=0.5,
             lower=22,
             upper=29,
@@ -164,27 +164,31 @@
             (  # mismatching input domains
                 {
                     "A": _create_mock_aggregate(
                         input_domain=PandasSeriesDomain(NumpyFloatDomain())
                     )
                 },
                 {"A": PandasSeriesDomain(NumpyIntegerDomain())},
-                "The input domain is not compatible with the input domains of the"
-                " aggregation functions.",
+                (
+                    "The input domain is not compatible with the input domains of the"
+                    " aggregation functions."
+                ),
             ),
             (  # mismatching column names
                 {"A": _create_mock_aggregate()},
                 {"B": PandasSeriesDomain(NumpyIntegerDomain())},
                 "Column 'A' is not in the input schema.",
             ),
             (  # invalid input metric
                 {"A": _create_mock_aggregate(input_metric=AbsoluteDifference())},
                 {"A": PandasSeriesDomain(NumpyIntegerDomain())},
-                "The input metric of the aggregation function must be either "
-                "SymmetricDifference or HammingDistance.",
+                (
+                    "The input metric of the aggregation function must be either "
+                    "SymmetricDifference or HammingDistance."
+                ),
             ),
             (  # inconsistent input metrics
                 {
                     "A": _create_mock_aggregate(input_metric=SymmetricDifference()),
                     "B": _create_mock_aggregate(input_metric=HammingDistance()),
                 },
                 {
@@ -192,16 +196,18 @@
                     "B": PandasSeriesDomain(NumpyIntegerDomain()),
                 },
                 "All of the aggregation functions must have the same input metric.",
             ),
             (  # invalid output measure
                 {"A": _create_mock_aggregate(output_measure=ApproxDP())},
                 {"A": PandasSeriesDomain(NumpyIntegerDomain())},
-                "The output measure of the aggregation function must be either PureDP "
-                "or RhoZCDP.",
+                (
+                    "The output measure of the aggregation function must be either"
+                    " PureDP or RhoZCDP."
+                ),
             ),
             (  # inconsistent output measures
                 {
                     "A": _create_mock_aggregate(output_measure=PureDP()),
                     "B": _create_mock_aggregate(output_measure=RhoZCDP()),
                 },
                 {
@@ -213,23 +219,23 @@
         ]
     )
     def test_input_validation(
         self,
         column_to_aggregation: Dict[str, Aggregate],
         schema: Dict[str, PandasSeriesDomain],
         expected_error_message: str,
-    ):
+    ) -> None:
         """Init correctly validates aggregation functions."""
         with self.assertRaisesRegex(ValueError, expected_error_message):
             AggregateByColumn(
                 input_domain=PandasDataFrameDomain(schema),
                 column_to_aggregation=column_to_aggregation,
             )
 
-    def test_correctness_quantile(self):
+    def test_correctness_quantile(self) -> None:
         """Test correctness for a quantile aggregation and infinite budget."""
         df = pd.DataFrame([[28, 23], [26, 22], [27, 24], [29, 25]], columns=["F", "M"])
         qs = [0, 1]
         quantile_measurements = [
             NoisyQuantile(
                 PandasSeriesDomain(NumpyIntegerDomain()),
                 output_measure=PureDP(),
@@ -282,15 +288,15 @@
         privacy_function_return_value1: ExactNumber,
         privacy_relation_return_value1: bool,
         privacy_function_implemented2: bool,
         privacy_function_return_value2: ExactNumber,
         privacy_relation_return_value2: bool,
         input_metric: Union[SymmetricDifference, HammingDistance],
         use_hint: bool,
-    ):
+    ) -> None:
         """Tests that the privacy function and relation work correctly."""
         mock_measurement1 = create_mock_measurement(
             input_domain=PandasSeriesDomain(element_domain=NumpyFloatDomain()),
             input_metric=input_metric,
             privacy_function_implemented=privacy_function_implemented1,
             privacy_function_return_value=privacy_function_return_value1,
             privacy_relation_return_value=privacy_relation_return_value1,
@@ -325,17 +331,19 @@
             )
         if (
             not (privacy_function_implemented1 and privacy_function_implemented2)
             and not use_hint
         ):
             self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "privacy_relation from one of self.column_to_aggregation.values() "
-                "raised a NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "privacy_relation from one of self.column_to_aggregation.values() "
+                    "raised a NotImplementedError: TEST"
+                ),
             )
         else:
             self.assertEqual(
                 measurement.privacy_relation(1, 2),
                 mock_measurement1.privacy_relation(1, 1)
                 and mock_measurement2.privacy_relation(1, 1),
             )
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/pandas_measurements/test_series.py` & `tmlt_core-0.9.0/test/unit/measurements/pandas_measurements/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,16 +121,18 @@
             (
                 {"upper": 0, "lower": 1},
                 "Lower bound (1) can not be greater than the upper bound (0).",
             ),
             ({"epsilon": -1}, "Invalid PureDP measure value (epsilon) -1"),
             (
                 {"input_domain": PandasSeriesDomain(NumpyStringDomain())},
-                "input_domain.element_domain must be NumpyIntegerDomain or "
-                "NumpyFloatDomain, not NumpyStringDomain",
+                (
+                    "input_domain.element_domain must be NumpyIntegerDomain or "
+                    "NumpyFloatDomain, not NumpyStringDomain"
+                ),
             ),
             (
                 {"input_domain": PandasSeriesDomain(NumpyFloatDomain(allow_nan=True))},
                 "Input domain must disallow NaNs",
             ),
         ]
     )
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_aggregations.py` & `tmlt_core-0.9.0/test/unit/measurements/test_aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from tmlt.core.utils.testing import PySparkTest
 
 
 @parameterized_class(
     [
         {"group_keys_list": [], "struct_fields": [], "groupby_columns": []},
         {
-            "group_keys_list": [("x1",), ("x2",), ("x3",)],
+            "group_keys_list": [("x1",), ("x2",), ("x3",), (None,)],
             "struct_fields": [StructField("A", StringType())],
             "groupby_columns": ["A"],
         },
     ]
 )
 class TestGroupByAggregationMeasurements(PySparkTest):
     """Tests for :mod:`tmlt.core.measurements.aggregations`."""
@@ -57,15 +57,18 @@
     group_keys_list: List[Tuple[str, ...]]
     struct_fields: List[StructField]
     groupby_columns: List[str]
 
     def setUp(self):
         """Test setup."""
         self.input_domain = SparkDataFrameDomain(
-            {"A": SparkStringColumnDescriptor(), "B": SparkIntegerColumnDescriptor()}
+            {
+                "A": SparkStringColumnDescriptor(allow_null=True),
+                "B": SparkIntegerColumnDescriptor(),
+            }
         )
         self.group_keys = self.spark.createDataFrame(
             self.group_keys_list, schema=StructType(self.struct_fields.copy())
         )
         self.sdf = self.spark.createDataFrame(
             [("x1", 2), ("x1", 2), ("x2", 4)], schema=["A", "B"]
         )
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_chaining.py` & `tmlt_core-0.9.0/test/unit/measurements/test_chaining.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,19 @@
             self.assertEqual(
                 measurement.privacy_function(sp.Integer(1)),
                 privacy_function_return_value,
             )
         if not stability_function_implemented and not use_hint:
             with self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "stability_relation of self.transformation raised a "
-                "NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "stability_relation of self.transformation raised a "
+                    "NotImplementedError: TEST"
+                ),
             ):
                 measurement.privacy_relation(sp.Integer(1), sp.Integer(1))
         else:
             self.assertEqual(
                 measurement.privacy_relation(sp.Integer(1), sp.Integer(1)),
                 mock_transformation.stability_relation(sp.Integer(1), sp.Integer(1))
                 and mock_measurement.privacy_relation(sp.Integer(1), sp.Integer(1)),
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_composition.py` & `tmlt_core-0.9.0/test/unit/measurements/test_composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,17 +174,19 @@
             )
         if (
             not (privacy_function_implemented1 and privacy_function_implemented2)
             and not use_hint
         ):
             self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "privacy_relation from one of self.measurements raised a "
-                "NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "privacy_relation from one of self.measurements raised a "
+                    "NotImplementedError: TEST"
+                ),
             )
         else:
             self.assertEqual(
                 measurement.privacy_relation(d_in, d_in * 2),
                 mock_measurement1.privacy_relation(d_in, d_in * 1)
                 and mock_measurement2.privacy_relation(d_in, d_in * 1),
             )
@@ -196,18 +198,18 @@
 
     @parameterized.expand(
         [
             (d_in, *params1, *params2, use_hint)
             for d_in in [1, 2]
             for params1, params2 in itertools.combinations(
                 [
-                    (True, d_in ** 2 * 1, True),
-                    (True, d_in ** 2 * 2, False),
-                    (False, d_in ** 2 * 1, True),
-                    (False, d_in ** 2 * 2, False),
+                    (True, d_in**2 * 1, True),
+                    (True, d_in**2 * 2, False),
+                    (False, d_in**2 * 1, True),
+                    (False, d_in**2 * 2, False),
                 ],
                 2,
             )
             for use_hint in [True, False]
         ]
     )
     def test_privacy_function_and_relation_rho_zcdp(
@@ -233,15 +235,15 @@
         )
         mock_measurement2 = create_mock_measurement(
             privacy_function_implemented=privacy_function_implemented2,
             privacy_function_return_value=privacy_function_return_value2,
             privacy_relation_return_value=privacy_relation_return_value2,
             output_measure=RhoZCDP(),
         )
-        mock_hint = MagicMock(return_value=(d_in ** 2 * 1, d_in ** 2 * 1))
+        mock_hint = MagicMock(return_value=(d_in**2 * 1, d_in**2 * 1))
 
         measurement = Composition(
             [mock_measurement1, mock_measurement2], hint=mock_hint if use_hint else None
         )
         if not (privacy_function_implemented1 and privacy_function_implemented2):
             with self.assertRaisesRegex(NotImplementedError, "TEST"):
                 measurement.privacy_function(d_in)
@@ -252,28 +254,30 @@
             )
         if (
             not (privacy_function_implemented1 and privacy_function_implemented2)
             and not use_hint
         ):
             self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "privacy_relation from one of self.measurements raised a "
-                "NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "privacy_relation from one of self.measurements raised a "
+                    "NotImplementedError: TEST"
+                ),
             )
         else:
             self.assertEqual(
-                measurement.privacy_relation(d_in, d_in ** 2 * 2),
-                mock_measurement1.privacy_relation(d_in, d_in ** 2 * 1)
-                and mock_measurement2.privacy_relation(d_in, d_in ** 2 * 1),
+                measurement.privacy_relation(d_in, d_in**2 * 2),
+                mock_measurement1.privacy_relation(d_in, d_in**2 * 1)
+                and mock_measurement2.privacy_relation(d_in, d_in**2 * 1),
             )
             if mock_hint.called:
-                mock_hint.assert_called_with(d_in, d_in ** 2 * 2)
+                mock_hint.assert_called_with(d_in, d_in**2 * 2)
             self.assertFalse(
-                measurement.privacy_relation(d_in, d_in ** 2 * sp.Rational("1.99"))
+                measurement.privacy_relation(d_in, d_in**2 * sp.Rational("1.99"))
             )
 
     @parameterized.expand(
         [
             (d_in, *params1, *params2, use_hint)
             for d_in in [1, 2]
             for params1, params2 in itertools.combinations(
@@ -347,17 +351,19 @@
             )
         if (
             not (privacy_function_implemented1 and privacy_function_implemented2)
             and not use_hint
         ):
             self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "privacy_relation from one of self.measurements raised a "
-                "NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "privacy_relation from one of self.measurements raised a "
+                    "NotImplementedError: TEST"
+                ),
             )
         else:
             self.assertEqual(
                 measurement.privacy_relation(d_in, (d_in * 2, sp.Rational("0.4"))),
                 mock_measurement1.privacy_relation(d_in, (d_in * 1, sp.Rational("0.2")))
                 and mock_measurement2.privacy_relation(
                     d_in, (d_in * 1, sp.Rational("0.2"))
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_converters.py` & `tmlt_core-0.9.0/test/unit/measurements/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.0/test/unit/measurements/test_interactive_measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,16 +268,18 @@
                 r" measurements \(1\)",
             ),
             (
                 ListDomain(NumpyIntegerDomain(), length=2),
                 RootSumOfSquared(AbsoluteDifference()),
                 ApproxDP(),
                 [create_mock_measurement(is_interactive=True)],
-                f"Input metric {RootSumOfSquared} is incompatible with output measure"
-                f" {ApproxDP}",
+                (
+                    f"Input metric {RootSumOfSquared} is incompatible with output"
+                    f" measure {ApproxDP}"
+                ),
             ),
             (
                 ListDomain(NumpyIntegerDomain(), length=1),
                 SumOf(AbsoluteDifference()),
                 RhoZCDP(),
                 [create_mock_measurement(is_interactive=True)],
                 f"Input metric {SumOf} is incompatible with output measure {RhoZCDP}",
@@ -289,24 +291,28 @@
                 [
                     create_mock_measurement(
                         is_interactive=True,
                         output_measure=RhoZCDP(),
                         input_metric=SymmetricDifference(),
                     )
                 ],
-                "Input metric for each supplied measurement must match inner metric of"
-                " input metric for ParallelComposition",
+                (
+                    "Input metric for each supplied measurement must match inner metric"
+                    " of input metric for ParallelComposition"
+                ),
             ),
             (
                 ListDomain(NumpyIntegerDomain(), length=1),
                 RootSumOfSquared(AbsoluteDifference()),
                 RhoZCDP(),
                 [create_mock_measurement(is_interactive=True, output_measure=PureDP())],
-                "Output measure for each supplied measurement must match output measure"
-                " for ParallelComposition",
+                (
+                    "Output measure for each supplied measurement must match output"
+                    " measure for ParallelComposition"
+                ),
             ),
         ]
     )
     def test_invalid_constructor_arguments(
         self,
         input_domain: ListDomain,
         input_metric: Union[SumOf, RootSumOfSquared],
@@ -565,30 +571,36 @@
 
     @parameterized.expand(
         [
             (
                 NumpyFloatDomain(),
                 AbsoluteDifference(),
                 PureDP(),
-                "Input domain of measurement query does not match the input domain of"
-                " SequentialQueryable.",
+                (
+                    "Input domain of measurement query does not match the input domain"
+                    " of SequentialQueryable."
+                ),
             ),
             (
                 NumpyIntegerDomain(),
                 SymmetricDifference(),
                 PureDP(),
-                "Input metric of measurement query does not match the input metric of"
-                " SequentialQueryable.",
+                (
+                    "Input metric of measurement query does not match the input metric"
+                    " of SequentialQueryable."
+                ),
             ),
             (
                 NumpyIntegerDomain(),
                 AbsoluteDifference(),
                 RhoZCDP(),
-                "Output measure of measurement query does not match the output measure"
-                " of SequentialQueryable.",
+                (
+                    "Output measure of measurement query does not match the output"
+                    " measure of SequentialQueryable."
+                ),
             ),
         ]
     )
     def test_incompatible_measurement_query(
         self,
         input_domain: Domain,
         input_metric: Metric,
@@ -696,39 +708,43 @@
             )
 
     def test_transformation_query(self):
         """SequentialQueryable processes TransformationQuery correctly."""
         # pylint: disable=protected-access
         queryable = self.construct_queryable()
         transformation = create_mock_transformation(
-            return_value=np.float(100.0),
+            return_value=np.float64(100.0),
             stability_function_implemented=True,
             output_domain=NumpyFloatDomain(),
             output_metric=SymmetricDifference(),
             stability_function_return_value=20,
         )
         queryable(TransformationQuery(transformation=transformation))
         self.assertEqual(queryable._d_in, 20)
         self.assertEqual(queryable._input_domain, NumpyFloatDomain())
         self.assertEqual(queryable._input_metric, SymmetricDifference())
-        self.assertEqual(queryable._data, np.float(100.0))
+        self.assertEqual(queryable._data, np.float64(100.0))
 
     @parameterized.expand(
         [
             (
                 NumpyIntegerDomain(),
                 SymmetricDifference(),
-                "Input metric of transformation query does not match the input metric"
-                " of SequentialQueryable.",
+                (
+                    "Input metric of transformation query does not match the input"
+                    " metric of SequentialQueryable."
+                ),
             ),
             (
                 NumpyFloatDomain(),
                 AbsoluteDifference(),
-                "Input domain of transformation query does not match the input domain"
-                " of SequentialQueryable.",
+                (
+                    "Input domain of transformation query does not match the input"
+                    " domain of SequentialQueryable."
+                ),
             ),
         ]
     )
     def test_invalid_transformation_query(
         self, input_domain: Domain, input_metric: Metric, error_message: str
     ):
         """SequentialQueryable raises error when TransformationQuery is incompatible."""
@@ -989,22 +1005,26 @@
         self.assertNotEqual(children, accountant.children)
 
     @parameterized.expand(
         [
             (
                 None,
                 None,
-                "PrivacyAccountant cannot be initialized with no parent and no"
-                " queryable",
+                (
+                    "PrivacyAccountant cannot be initialized with no parent and no"
+                    " queryable"
+                ),
             ),
             (
                 Mock(PrivacyAccountant),
                 Mock(SequentialQueryable),
-                "PrivacyAccountant can be initialized with only parent or only"
-                " queryable but not both",
+                (
+                    "PrivacyAccountant can be initialized with only parent or only"
+                    " queryable but not both"
+                ),
             ),
         ]
     )
     def test_init_invalid_arguments(
         self,
         parent: Optional[PrivacyAccountant],
         queryable: Optional[Queryable],
@@ -1061,27 +1081,31 @@
         self.assertEqual(accountant.privacy_budget, self.measurement.privacy_budget)
         self.assertEqual(accountant.d_in, self.measurement.d_in)
         self.assertEqual(accountant.children, [])
 
     @parameterized.expand(
         [
             (
-                "Transformation's input domain does not match PrivacyAccountant's input"
-                " domain",
+                (
+                    "Transformation's input domain does not match PrivacyAccountant's"
+                    " input domain"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {"A": SparkIntegerColumnDescriptor()}
                     ),
                     input_metric=SymmetricDifference(),
                     stability_function_implemented=True,
                 ),
             ),
             (
-                "Transformation's input metric does not match PrivacyAccountant's input"
-                " metric",
+                (
+                    "Transformation's input metric does not match PrivacyAccountant's"
+                    " input metric"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {
                             "A": SparkIntegerColumnDescriptor(),
                             "B": SparkStringColumnDescriptor(),
                         }
                     ),
@@ -1124,15 +1148,17 @@
             return_value=np.int64(2),
         )
         accountant.transform_in_place(transformation=transformation)
         self.assertEqual(accountant.input_domain, NumpyIntegerDomain())
         self.assertEqual(accountant.input_metric, AbsoluteDifference())
         self.assertEqual(accountant.d_in, 10)
         # pylint: disable=protected-access
-        self.assertEqual(accountant._queryable._data, np.int64(2))
+        self.assertIsNotNone(accountant._queryable)
+        self.assertEqual(accountant._queryable._data, np.int64(2))  # type: ignore
+        # pylint: enable=protected-access
 
     def test_transform_with_explicit_d_out(self):
         """PrivacyAccountant.transform_in_place works with a d_out provided."""
         accountant = PrivacyAccountant.launch(
             measurement=self.measurement, data=self.data
         )
         transformation = create_mock_transformation(
@@ -1150,21 +1176,24 @@
             return_value=np.int64(2),
         )
         accountant.transform_in_place(transformation=transformation, d_out=10)
         self.assertEqual(accountant.input_domain, NumpyIntegerDomain())
         self.assertEqual(accountant.input_metric, AbsoluteDifference())
         self.assertEqual(accountant.d_in, 10)
         # pylint: disable=protected-access
-        self.assertEqual(accountant._queryable._data, np.int64(2))
+        self.assertIsNotNone(accountant._queryable)
+        self.assertEqual(accountant._queryable._data, np.int64(2))  # type: ignore
 
     @parameterized.expand(
         [
             (
-                "Measurement's output measure does not match PrivacyAccountant's output"
-                " measure",
+                (
+                    "Measurement's output measure does not match PrivacyAccountant's"
+                    " output measure"
+                ),
                 create_mock_measurement(
                     input_domain=SparkDataFrameDomain(
                         {
                             "A": SparkIntegerColumnDescriptor(),
                             "B": SparkStringColumnDescriptor(),
                         }
                     ),
@@ -1255,26 +1284,30 @@
                 SumOf(AbsoluteDifference()),
                 PureDP(),
                 8,
                 False,
                 1,
             ),
             (
-                "Transformation's input domain does not match PrivacyAccountant's input"
-                " domain",
+                (
+                    "Transformation's input domain does not match PrivacyAccountant's"
+                    " input domain"
+                ),
                 NumpyStringDomain(),
                 AbsoluteDifference(),
                 ListDomain(NumpyIntegerDomain(), length=2),
                 SumOf(AbsoluteDifference()),
                 PureDP(),
                 8,
             ),
             (
-                "Transformation's input metric does not match PrivacyAccountant's"
-                " input metric",
+                (
+                    "Transformation's input metric does not match PrivacyAccountant's"
+                    " input metric"
+                ),
                 NumpyIntegerDomain(),
                 SymmetricDifference(),
                 ListDomain(NumpyIntegerDomain(), length=2),
                 SumOf(AbsoluteDifference()),
                 PureDP(),
                 8,
             ),
@@ -1293,26 +1326,30 @@
                 AbsoluteDifference(),
                 ListDomain(NumpyIntegerDomain()),
                 SumOf(AbsoluteDifference()),
                 PureDP(),
                 8,
             ),
             (
-                "Splitting transformation's output metric must be"
-                f" {SumOf} for output measure PureDP",
+                (
+                    "Splitting transformation's output metric must be"
+                    f" {SumOf} for output measure PureDP"
+                ),
                 NumpyIntegerDomain(),
                 AbsoluteDifference(),
                 ListDomain(NumpyIntegerDomain(), length=2),
                 RootSumOfSquared(AbsoluteDifference()),
                 PureDP(),
                 8,
             ),
             (
-                "Splitting transformation's output metric must be"
-                f" {RootSumOfSquared} for output measure RhoZCDP",
+                (
+                    "Splitting transformation's output metric must be"
+                    f" {RootSumOfSquared} for output measure RhoZCDP"
+                ),
                 NumpyIntegerDomain(),
                 AbsoluteDifference(),
                 ListDomain(NumpyIntegerDomain(), length=2),
                 SumOf(AbsoluteDifference()),
                 RhoZCDP(),
                 8,
             ),
@@ -1431,16 +1468,18 @@
             return_value=np.int64(2),
         )
         accountant.queue_transformation(transformation=transformation)
         self.assertEqual(accountant.input_domain, NumpyIntegerDomain())
         self.assertEqual(accountant.input_metric, AbsoluteDifference())
         self.assertEqual(accountant.d_in, 10)
         # pylint: disable=protected-access
-        self.assertEqual(accountant._queryable._data, np.int64(2))
+        self.assertIsNotNone(accountant._queryable)
+        self.assertEqual(accountant._queryable._data, np.int64(2))  # type: ignore
         self.assertIsNone(accountant._pending_transformation)
+        # pylint: enable=protected-access
 
     def test_queue_transformation_on_inactive_accountant(self):
         """queue_transformation queues transformations on inactive account"""
         accountant = PrivacyAccountant.launch(
             measurement=self.measurement, data=self.data
         )
         split_transformation = create_mock_transformation(
@@ -1490,33 +1529,39 @@
         # Once the accountant is active again, the transformation should
         # have been run
         self.assertEqual(accountant.state, PrivacyAccountantState.ACTIVE)
         self.assertEqual(accountant.input_domain, NumpyIntegerDomain())
         self.assertEqual(accountant.input_metric, AbsoluteDifference())
         self.assertEqual(accountant.d_in, 10)
         # pylint: disable=protected-access
-        self.assertEqual(accountant._queryable._data, np.int64(2))
+        self.assertIsNotNone(accountant._queryable)
+        self.assertEqual(accountant._queryable._data, np.int64(2))  # type: ignore
         self.assertIsNone(accountant._pending_transformation)
+        # pylint: enable=protected-access
 
     @parameterized.expand(
         [
             (
-                "Transformation's input domain does not match PrivacyAccountant's input"
-                " domain",
+                (
+                    "Transformation's input domain does not match PrivacyAccountant's"
+                    " input domain"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {"A": SparkIntegerColumnDescriptor()}
                     ),
                     input_metric=SymmetricDifference(),
                     stability_function_implemented=True,
                 ),
             ),
             (
-                "Transformation's input metric does not match PrivacyAccountant's input"
-                " metric",
+                (
+                    "Transformation's input metric does not match PrivacyAccountant's"
+                    " input metric"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {
                             "A": SparkIntegerColumnDescriptor(),
                             "B": SparkStringColumnDescriptor(),
                         }
                     ),
@@ -1557,27 +1602,31 @@
         self.assertEqual(accountant.state, PrivacyAccountantState.WAITING_FOR_CHILDREN)
         with self.assertRaisesRegex(ValueError, error_message):
             accountant.queue_transformation(transformation=transformation, d_out=d_out)
 
     @parameterized.expand(
         [
             (
-                "Transformation's input domain does not match the output domain"
-                " of the last transformation",
+                (
+                    "Transformation's input domain does not match the output domain"
+                    " of the last transformation"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {"A": SparkIntegerColumnDescriptor()}
                     ),
                     input_metric=SymmetricDifference(),
                     stability_function_implemented=True,
                 ),
             ),
             (
-                "Transformation's input metric does not match the output metric"
-                " of the last transformation",
+                (
+                    "Transformation's input metric does not match the output metric"
+                    " of the last transformation"
+                ),
                 create_mock_transformation(
                     input_domain=SparkDataFrameDomain(
                         {
                             "A": SparkIntegerColumnDescriptor(),
                             "B": SparkStringColumnDescriptor(),
                         }
                     ),
@@ -1714,16 +1763,18 @@
                 return_value=[np.int64(0) for _ in range(4)],
                 stability_function_implemented=True,
             ),
             privacy_budget=self.budget_quarters[1],
         )
         with self.assertWarnsRegex(
             RuntimeWarning,
-            "Retiring an unused PrivacyAccountant that is"
-            " PrivacyAccountantState.WAITING_FOR_SIBLING",
+            (
+                "Retiring an unused PrivacyAccountant that is"
+                " PrivacyAccountantState.WAITING_FOR_SIBLING"
+            ),
         ):
             children[1].retire()
 
     def test_retire_accountant_waiting_for_sibling(self):
         """Retiring an unused sibling retires all prior siblings and activates next."""
         accountant = PrivacyAccountant.launch(
             measurement=self.measurement, data=self.data
@@ -1931,18 +1982,20 @@
         self.assertIsInstance(adaptive_composition.measurement, SequentialComposition)
         self.assertEqual(
             adaptive_composition.measurement.input_domain, NumpyIntegerDomain()
         )
         self.assertEqual(
             adaptive_composition.measurement.input_metric, AbsoluteDifference()
         )
-        self.assertEqual(adaptive_composition.measurement.d_in, 1)
+        self.assertEqual(adaptive_composition.measurement.d_in, 1)  # type: ignore
+        # pylint: disable=line-too-long
         self.assertEqual(
-            adaptive_composition.measurement.privacy_budget, self.privacy_budget
+            adaptive_composition.measurement.privacy_budget, self.privacy_budget  # type: ignore
         )
+        # pylint: enable=line-too-long
         self.assertEqual(
             adaptive_composition.measurement.output_measure, self.output_measure
         )
         self.assertIsInstance(adaptive_composition(np.int64(10)), DecoratedQueryable)
 
     def test_correctness(self):
         """Queryable works as expected."""
```

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_noise_mechanisms.py` & `tmlt_core-0.9.0/test/unit/measurements/test_noise_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_postprocess.py` & `tmlt_core-0.9.0/test/unit/measurements/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/measurements/test_spark_measurements.py` & `tmlt_core-0.9.0/test/unit/measurements/test_spark_measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,16 @@
             input_domain=self.input_domain,
             alpha=1,
             threshold=-1,
             count_column=self.count_column,
         )
         actual = measurement(sdf).toPandas()
         expected_without_count = pd.DataFrame({"A": ["a1"], "B": [1]})
+        self.assertIsInstance(actual, pd.DataFrame)
+        assert isinstance(actual, pd.DataFrame)
         self.assert_frame_equal_with_sort(actual[["A", "B"]], expected_without_count)
         # Threshold -1 should give worse guarantee than for threshold of 0 or 1
         measurement_threshold_0 = GeometricPartitionSelection(
             input_domain=self.input_domain,
             alpha=1,
             threshold=0,
             count_column=self.count_column,
```

### Comparing `tmlt_core-0.8.3/test/unit/random/test_continuous_gaussian.py` & `tmlt_core-0.9.0/test/unit/random/test_continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/random/test_discrete_gaussian.py` & `tmlt_core-0.9.0/test/unit/random/test_discrete_gaussian.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,11 +27,9 @@
 
     def test_invalid_rng_raises_error(self):
         """Tests that sample_dgauss raises error if rng does not support randrange."""
 
         class BadRNG:
             """Does not support randrange."""
 
-            ...
-
         with self.assertRaisesRegex(TypeError, 'type of argument "rng" must be'):
-            sample_dgauss(sigma_squared=1, rng=BadRNG())
+            sample_dgauss(sigma_squared=1, rng=BadRNG())  # type: ignore
```

### Comparing `tmlt_core-0.8.3/test/unit/random/test_inverse_cdf.py` & `tmlt_core-0.9.0/test/unit/random/test_inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/random/test_laplace.py` & `tmlt_core-0.9.0/test/unit/random/test_laplace.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/random/test_rng.py` & `tmlt_core-0.9.0/test/unit/random/test_rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/random/test_uniform.py` & `tmlt_core-0.9.0/test/unit/random/test_uniform.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/test_measures.py` & `tmlt_core-0.9.0/test/unit/test_measures.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/test_metrics.py` & `tmlt_core-0.9.0/test/unit/test_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Unit tests for :mod:`tmlt.core.metrics`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 # pylint: disable=no-self-use
 import datetime
-from typing import Any, Union
+from typing import Any, Dict, Union
 from unittest import TestCase
 from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
 import sympy as sp
 from parameterized import parameterized
@@ -1259,21 +1259,25 @@
         """Tests that the metric is equal to itself and not other metrics."""
         self.assertEqual(value1 == value2, expected)
 
     def test_repr(self):
         """Tests that the string representation is as expected."""
         self.assertEqual(
             repr(OnColumn(column="A", metric=RootSumOfSquared(SymmetricDifference()))),
-            "OnColumn(column='A', "
-            "metric=RootSumOfSquared(inner_metric=SymmetricDifference()))",
+            (
+                "OnColumn(column='A', "
+                "metric=RootSumOfSquared(inner_metric=SymmetricDifference()))"
+            ),
         )
         self.assertEqual(
             repr(OnColumn(column="A", metric=RootSumOfSquared(AbsoluteDifference()))),
-            "OnColumn(column='A', "
-            "metric=RootSumOfSquared(inner_metric=AbsoluteDifference()))",
+            (
+                "OnColumn(column='A', "
+                "metric=RootSumOfSquared(inner_metric=AbsoluteDifference()))"
+            ),
         )
         self.assertEqual(
             repr(OnColumn(column="A", metric=SumOf(AbsoluteDifference()))),
             "OnColumn(column='A', metric=SumOf(inner_metric=AbsoluteDifference()))",
         )
 
     @parameterized.expand(
@@ -1489,17 +1493,20 @@
                         OnColumn(
                             column="A", metric=RootSumOfSquared(SymmetricDifference())
                         ),
                         OnColumn(column="B", metric=SumOf(AbsoluteDifference())),
                     ]
                 )
             ),
-            "OnColumns(on_columns=[OnColumn(column='A', metric=RootSumOfSquared("
-            "inner_metric=SymmetricDifference())), OnColumn(column='B', metric=SumOf("
-            "inner_metric=AbsoluteDifference()))])",
+            (
+                "OnColumns(on_columns=[OnColumn(column='A',"
+                " metric=RootSumOfSquared(inner_metric=SymmetricDifference())),"
+                " OnColumn(column='B',"
+                " metric=SumOf(inner_metric=AbsoluteDifference()))])"
+            ),
         )
 
     @parameterized.expand(
         [
             (
                 OnColumns(
                     [
@@ -1695,30 +1702,36 @@
         """Tests that the string representation is as expected."""
         self.assertEqual(
             repr(
                 IfGroupedBy(
                     column="A", inner_metric=RootSumOfSquared(SymmetricDifference())
                 )
             ),
-            "IfGroupedBy(column='A', "
-            "inner_metric=RootSumOfSquared(inner_metric=SymmetricDifference()))",
+            (
+                "IfGroupedBy(column='A', "
+                "inner_metric=RootSumOfSquared(inner_metric=SymmetricDifference()))"
+            ),
         )
         self.assertEqual(
             repr(
                 IfGroupedBy(
                     column="A", inner_metric=RootSumOfSquared(AbsoluteDifference())
                 )
             ),
-            "IfGroupedBy(column='A', "
-            "inner_metric=RootSumOfSquared(inner_metric=AbsoluteDifference()))",
+            (
+                "IfGroupedBy(column='A', "
+                "inner_metric=RootSumOfSquared(inner_metric=AbsoluteDifference()))"
+            ),
         )
         self.assertEqual(
             repr(IfGroupedBy(column="A", inner_metric=SumOf(AbsoluteDifference()))),
-            "IfGroupedBy(column='A', "
-            "inner_metric=SumOf(inner_metric=AbsoluteDifference()))",
+            (
+                "IfGroupedBy(column='A', "
+                "inner_metric=SumOf(inner_metric=AbsoluteDifference()))"
+            ),
         )
 
     @parameterized.expand(
         [
             (
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
                 NumpyIntegerDomain(),
@@ -1852,15 +1865,15 @@
 
 
 class TestDictMetric(TestCase):
     """TestCase for DictMetric"""
 
     def test_constructor_mutable_arguments(self):
         """Tests that mutable constructor arguments are copied."""
-        metric_map = {"A": SymmetricDifference()}
+        metric_map: Dict[str, Metric] = {"A": SymmetricDifference()}
         metric = DictMetric(key_to_metric=metric_map)
         metric_map["A"] = HammingDistance()
         self.assertDictEqual(metric.key_to_metric, {"A": SymmetricDifference()})
 
     @parameterized.expand(get_all_props(DictMetric))
     def test_property_immutability(self, prop_name: str):
         """Tests that given property is immutable."""
@@ -1952,16 +1965,18 @@
         """Tests that the metric is equal to itself and not other metrics."""
         self.assertEqual(value1 == value2, expected)
 
     def test_repr(self):
         """Tests that the string representation is as expected."""
         self.assertEqual(
             repr(DictMetric({"A": SymmetricDifference(), "B": AbsoluteDifference()})),
-            "DictMetric(key_to_metric={'A': SymmetricDifference(), 'B': "
-            "AbsoluteDifference()})",
+            (
+                "DictMetric(key_to_metric={'A': SymmetricDifference(), 'B': "
+                "AbsoluteDifference()})"
+            ),
         )
 
     @parameterized.expand(
         [
             (
                 DictMetric({"A": AbsoluteDifference(), "B": SymmetricDifference()}),
                 DictDomain(
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_add_remove_keys.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_add_remove_keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     ]
 )
 class TestTransformValueSubclasses(PySparkTest):
     """Tests for subclasses of :class:`~.TransformValue`."""
 
     def test_smoke(self):
         """Tests that the transformation can be constructed and applied to data."""
-        kwargs = self.extra_kwargs.copy()
+        kwargs = self.extra_kwargs.copy()  # type: ignore
         input_data = {
             "key1": self.spark.createDataFrame(
                 pd.DataFrame(
                     [["X", 1.2, "c1"], ["Y", 0.9, "c2"]], columns=["A", "B", "C"]
                 )
             ),
             "key2": self.spark.createDataFrame(
@@ -245,18 +245,18 @@
                     }
                 ),
             }
         )
         kwargs["input_metric"] = AddRemoveKeys({"key1": "A", "key2": "A"})
         kwargs["key"] = "key1"
         kwargs["new_key"] = "key3"
-        kwargs.update(self.extra_kwargs)
-        for key, value in self.pandas_to_spark_kwargs.items():
+        kwargs.update(self.extra_kwargs)  # type: ignore
+        for key, value in self.pandas_to_spark_kwargs.items():  # type: ignore
             kwargs[key] = self.spark.createDataFrame(value)
-        transformation = self.test_class(**kwargs)
+        transformation = self.test_class(**kwargs)  # type: ignore
         transformation(input_data)
 
 
 class MockValue(TransformValue):
     """Subclass of :class:`~.TransformValue` with flexible behavior for testing."""
 
     def __init__(
@@ -305,15 +305,15 @@
                         "E": SparkIntegerColumnDescriptor(),
                     }
                 ),
             }
         )
         self.input_metric = AddRemoveKeys({"key1": "A", "key2": "D"})
         self.filter_transformation = Filter(
-            domain=self.input_domain.key_to_domain["key1"],
+            domain=self.input_domain.key_to_domain["key1"],  # type: ignore
             metric=IfGroupedBy("A", SymmetricDifference()),
             filter_expr="B < 1",
         )
         self.mock_filter_value = MockValue(
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             transformation=self.filter_transformation,
@@ -416,74 +416,75 @@
             (
                 "'key2' is already a key in the input domain",
                 ValueError,
                 {"new_key": "key2"},
                 {},
             ),
             (
-                "Input domain's value for 'key1' does not match transformation's input"
-                " domain",
+                (
+                    "Input domain's value for 'key1' does not match transformation's"
+                    " input domain"
+                ),
                 ValueError,
                 {},
                 {
                     "input_domain": SparkDataFrameDomain(
                         {"D": SparkStringColumnDescriptor()}
                     )
                 },
             ),
             (
-                "Output metric AddRemoveKeys(df_to_key_column={'key1': 'A', 'key2':"
-                " 'D', 'key3': 'A'}) and output domain"
-                " DictDomain(key_to_domain={'key1': SparkDataFrameDomain(schema={'A':"
-                " SparkStringColumnDescriptor(allow_null=False), 'B':"
-                " SparkFloatColumnDescriptor(allow_nan=True, allow_inf=True,"
-                " allow_null=True, size=64), 'C':"
-                " SparkStringColumnDescriptor(allow_null=False)}), 'key2':"
-                " SparkDataFrameDomain(schema={'D':"
-                " SparkStringColumnDescriptor(allow_null=False), 'E':"
-                " SparkIntegerColumnDescriptor(allow_null=False, size=64)}), 'key3':"
-                " NumpyIntegerDomain(size=64)}) are not compatible.",
+                (
+                    "Output metric AddRemoveKeys(df_to_key_column={'key1': 'A', 'key2':"
+                    " 'D', 'key3': 'A'}) and output domain"
+                    " DictDomain(key_to_domain={'key1':"
+                    " SparkDataFrameDomain(schema={'A':"
+                    " SparkStringColumnDescriptor(allow_null=False), 'B':"
+                    " SparkFloatColumnDescriptor(allow_nan=True, allow_inf=True,"
+                    " allow_null=True, size=64), 'C':"
+                    " SparkStringColumnDescriptor(allow_null=False)}), 'key2':"
+                    " SparkDataFrameDomain(schema={'D':"
+                    " SparkStringColumnDescriptor(allow_null=False), 'E':"
+                    " SparkIntegerColumnDescriptor(allow_null=False, size=64)}),"
+                    " 'key3': NumpyIntegerDomain(size=64)}) are not compatible."
+                ),
                 ValueError,
                 {},
                 {"output_domain": NumpyIntegerDomain()},
             ),
             (
-                "Transformation's input metric must be IfGroupedBy(column,"
-                " SymmetricDifference())",
+                (
+                    "Transformation's input metric must be IfGroupedBy(column,"
+                    " SymmetricDifference())"
+                ),
                 ValueError,
                 {},
                 {"input_metric": SymmetricDifference()},
             ),
             (
-                "Transformation's output metric must be IfGroupedBy(column,"
-                " SymmetricDifference())",
+                (
+                    "Transformation's output metric must be IfGroupedBy(column,"
+                    " SymmetricDifference())"
+                ),
                 ValueError,
                 {},
                 {"output_metric": SymmetricDifference()},
             ),
             (
-                "Transformation's input metric grouping column, B, does not"
-                " match the dataframe's key column, A.",
+                (
+                    "Transformation's input metric grouping column, B, does not"
+                    " match the dataframe's key column, A."
+                ),
                 ValueError,
                 {},
                 {
                     "input_metric": IfGroupedBy("B", SymmetricDifference()),
                     "output_metric": IfGroupedBy("B", SymmetricDifference()),
                 },
             ),
-            (
-                "Transformation's input and output metric must group by the same"
-                " column",
-                ValueError,
-                {},
-                {
-                    "input_metric": IfGroupedBy("A", SymmetricDifference()),
-                    "output_metric": IfGroupedBy("B", SymmetricDifference()),
-                },
-            ),
         ]
     )
     def test_invalid_parameters(
         self,
         error_msg: str,
         error_type: Type[Exception],
         updated_mock_value_args: Dict,
@@ -501,11 +502,92 @@
             "output_domain": self.input_domain.key_to_domain["key1"],
             "input_metric": IfGroupedBy("A", SymmetricDifference()),
             "output_metric": IfGroupedBy("A", SymmetricDifference()),
         }
         mock_transformation_args.update(updated_mock_transformation_args)
         mock_value_args.update(updated_mock_value_args)
         mock_value_args["transformation"] = create_mock_transformation(
-            **mock_transformation_args
+            **mock_transformation_args  # type: ignore
         )
         with self.assertRaisesRegex(error_type, re.escape(error_msg)):
             MockValue(**mock_value_args)  # type: ignore
+
+
+class TestRenameValue(PySparkTest):
+    """Tests for :class:`~.RenameValue`."""
+
+    def setUp(self):
+        """Setup."""
+        self.input_domain = DictDomain(
+            {
+                "key1": SparkDataFrameDomain(
+                    {
+                        "A": SparkStringColumnDescriptor(),
+                        "B": SparkFloatColumnDescriptor(
+                            allow_nan=True, allow_inf=True, allow_null=True
+                        ),
+                        "C": SparkStringColumnDescriptor(),
+                    }
+                ),
+                "key2": SparkDataFrameDomain(
+                    {
+                        "D": SparkStringColumnDescriptor(),
+                        "E": SparkIntegerColumnDescriptor(),
+                    }
+                ),
+            }
+        )
+        self.input_metric = AddRemoveKeys({"key1": "A", "key2": "D"})
+        self.input_data = {
+            "key1": self.spark.createDataFrame(
+                pd.DataFrame(
+                    [["X", 1.2, "c1"], ["Y", 0.9, "c2"]], columns=["A", "B", "C"]
+                )
+            ),
+            "key2": self.spark.createDataFrame(
+                pd.DataFrame([["X", 1], ["X", 2]], columns=["D", "E"])
+            ),
+        }
+        self.expected_output = {
+            "key1": self.spark.createDataFrame(
+                pd.DataFrame(
+                    [["X", 1.2, "c1"], ["Y", 0.9, "c2"]], columns=["A", "B", "C"]
+                )
+            ),
+            "key2": self.spark.createDataFrame(
+                pd.DataFrame([["X", 1], ["X", 2]], columns=["D", "E"])
+            ),
+        }
+
+    @parameterized.expand(
+        [
+            ("key1", "key3", {"A": "D"}),
+            ("key2", "key4", {"D": "F"}),
+            ("key1", "key5", {"B": "D", "C": "E"}),
+            ("key2", "key6", {"E": "F", "D": "G"}),
+        ]
+    )
+    def test_value_rename(self, key: str, new_key: str, rename_mapping: Dict[str, str]):
+        """Testing renaming values."""
+        expected_value = self.input_data[key].alias(new_key)
+        for k, v in rename_mapping.items():
+            expected_value = expected_value.withColumnRenamed(k, v)
+        expected_output = self.expected_output.copy()
+        expected_output[new_key] = expected_value
+
+        actual_output = RenameValue(
+            self.input_domain, self.input_metric, key, new_key, rename_mapping
+        )(self.input_data)
+
+        self.assertEqual(list(actual_output), ["key1", "key2", new_key])
+        self.assertEqual(
+            list(actual_output[new_key].columns), expected_output[new_key].columns
+        )
+        self.assert_frame_equal_with_sort(
+            actual_output["key1"].toPandas(), expected_output["key1"].toPandas()
+        )
+        self.assert_frame_equal_with_sort(
+            actual_output["key2"].toPandas(), expected_output["key2"].toPandas()
+        )
+        self.assert_frame_equal_with_sort(
+            actual_output[new_key].toPandas(), expected_output[new_key].toPandas()
+        )
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_agg.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_agg.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,18 +572,18 @@
             (  # measure column permits nulls
                 "D",
                 1,
                 40,
                 r"Input domain must not allow nulls or NaNs on the measure column"
                 r" \(D\)",
             ),
-            ("E", 0, 2 ** 970 + 1, r"Upper clipping bound should be at most 2\^970."),
+            ("E", 0, 2**970 + 1, r"Upper clipping bound should be at most 2\^970."),
             (
                 "E",
-                -(2 ** 970) - 1,
+                -(2**970) - 1,
                 0,
                 r"Lower clipping bound should be at least -2\^970.",
             ),
         ]
     )
     def test_invalid_inputs(
         self,
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_filter.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_filter.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_groupby.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,17 +108,19 @@
                 r"Column must be LongType(\(\))?, instead it is StringType(\(\))?.",
                 OutOfDomainError,
             ),
             (
                 IfGroupedBy("A", RootSumOfSquared(SymmetricDifference())),
                 [(1,), (2,), (3,)],
                 StructType([StructField("A", LongType())]),
-                "Input metric does not have the expected inner metric. Maybe "
-                "IfGroupedBy(column='A', inner_metric=SumOf("
-                "inner_metric=SymmetricDifference()))?",
+                (
+                    "Input metric does not have the expected inner metric. Maybe "
+                    "IfGroupedBy(column='A', inner_metric=SumOf("
+                    "inner_metric=SymmetricDifference()))?"
+                ),
             ),
             (
                 SymmetricDifference(),
                 [],
                 StructType([StructField("A", LongType())]),
                 "Group keys cannot have no rows, unless it also has no columns",
             ),
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_id.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_join.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_join.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Unit tests for :mod:`~tmlt.core.transformations.spark_transformations.join`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
+import re
 from typing import List, Optional, Union, cast
 
 import pandas as pd
 from parameterized import parameterized
 from pyspark.sql import types as st
 
 from tmlt.core.domains.collections import DictDomain
@@ -118,14 +119,102 @@
         pd.testing.assert_frame_equal(
             transformation.public_df.toPandas(), self.public_df.toPandas()
         )
         self.assertEqual(transformation.stability, 2)
 
     @parameterized.expand(
         [
+            (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                    }
+                ),
+                pd.DataFrame({"B": ["X", "X", None], "C": [10.0, 11.0, 3.0]}),
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+                ["B"],
+                False,
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+            ),
+            (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=True
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                    }
+                ),
+                pd.DataFrame({"A": [1.2, 1.3], "B": ["X", "X"]}),
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+                ["A"],
+                True,
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                        "B_left": SparkStringColumnDescriptor(allow_null=True),
+                        "B_right": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+            ),
+        ]
+    )
+    def test_output_domain_special_values(
+        self,
+        input_domain: SparkDataFrameDomain,
+        public_df: pd.DataFrame,
+        public_df_domain: SparkDataFrameDomain,
+        join_cols: List[str],
+        join_on_nulls: bool,
+        expected_domain: SparkDataFrameDomain,
+    ):
+        """Tests special values in output domain."""
+        transformation = PublicJoin(
+            input_domain=input_domain,
+            metric=SymmetricDifference(),
+            public_df=self.spark.createDataFrame(
+                public_df, schema=public_df_domain.spark_schema
+            ),
+            public_df_domain=public_df_domain,
+            join_cols=join_cols,
+            join_on_nulls=join_on_nulls,
+        )
+        self.assertEqual(transformation.output_domain, expected_domain)
+
+    @parameterized.expand(
+        [
             (SymmetricDifference(), 2),
             (IfGroupedBy("B", SumOf(SymmetricDifference())), 2),
             (IfGroupedBy("B", RootSumOfSquared(SymmetricDifference())), 2),
             (IfGroupedBy("B", SymmetricDifference()), 1),
         ]
     )
     def test_public_join_correctness(
@@ -180,15 +269,15 @@
 
     @parameterized.expand(
         [
             (
                 ["B", "C"],
                 ["B"],
                 "C",
-                "C is an overlapping column but not a join key",
+                "'C' is an overlapping column but not a join key",
                 SymmetricDifference(),
             ),
             (
                 ["A", "B"],
                 ["B"],
                 "D",
                 "Input metric .* and input domain .* are not compatible",
@@ -713,15 +802,15 @@
                             {"A": SparkIntegerColumnDescriptor()}
                         ),
                     }
                 ),
                 "df1",
                 "df2",
                 None,
-                "No common columns",
+                "Join must involve at least one column.",
             ),
             (  # Mismatching column types
                 DictDomain(
                     {
                         "df1": SparkDataFrameDomain(
                             {"A": SparkStringColumnDescriptor()}
                         ),
@@ -729,15 +818,16 @@
                             {"A": SparkIntegerColumnDescriptor()}
                         ),
                     }
                 ),
                 "df1",
                 "df2",
                 ["A"],
-                "mismatching types on join column A",
+                "'A' has different data types in left (StringType) and right "
+                "(LongType) domains.",
             ),
             (  # _right column already exists
                 DictDomain(
                     {
                         "df1": SparkDataFrameDomain(
                             {
                                 "A": SparkStringColumnDescriptor(),
@@ -752,84 +842,39 @@
                             }
                         ),
                     }
                 ),
                 "df1",
                 "df2",
                 ["A"],
-                "Join would rename overlapping column 'B' to an existing column name",
+                "Name collision, 'B_right' would appear more than once in the output.",
             ),
         ]
     )
     def test_invalid_arguments_rejected(
         self,
         input_domain: DictDomain,
         left: str,
         right: str,
         join_cols: Optional[List[str]],
         error_msg: str,
     ):
         """Tests that PrivateJoin cannot be constructed with invalid arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex(ValueError, re.escape(error_msg)):
             PrivateJoin(
                 input_domain=input_domain,
                 left_key=left,
                 right_key=right,
                 left_truncation_strategy=TruncationStrategy.TRUNCATE,
                 right_truncation_strategy=TruncationStrategy.TRUNCATE,
                 left_truncation_threshold=1,
                 right_truncation_threshold=1,
                 join_cols=join_cols,
             )
 
-    def test_join_drops_invalid_rows(self):
-        """Tests nans are dropped from the right-hand DataFrame when disallowed.
-
-        Infinity should still be allowed.
-        """
-        left = pd.DataFrame([(1, 2), (1, 3), (2, 4)], columns=["A", "B"])
-        right_sdf = self.spark.createDataFrame(
-            [(1, 2, float("nan")), (1, 3, float("inf")), (2, 4, float(0))],
-            schema=st.StructType(
-                [
-                    st.StructField("A", st.IntegerType(), nullable=False),
-                    st.StructField("B", st.IntegerType(), nullable=False),
-                    st.StructField("C", st.DoubleType(), nullable=False),
-                ]
-            ),
-        )
-        left_domain = SparkDataFrameDomain(
-            {col: SparkIntegerColumnDescriptor() for col in left.columns}
-        )
-        right_domain = SparkDataFrameDomain(
-            {
-                "A": SparkIntegerColumnDescriptor(),
-                "B": SparkIntegerColumnDescriptor(),
-                "C": SparkFloatColumnDescriptor(allow_inf=True),
-            }
-        )
-        join_cols = ["A", "B"]
-        private_join = PrivateJoin(
-            input_domain=DictDomain({"left": left_domain, "right": right_domain}),
-            left_key="left",
-            right_key="right",
-            left_truncation_strategy=TruncationStrategy.TRUNCATE,
-            right_truncation_strategy=TruncationStrategy.TRUNCATE,
-            left_truncation_threshold=1,
-            right_truncation_threshold=1,
-            join_cols=join_cols,
-            join_on_nulls=False,
-        )
-        left_sdf = self.spark.createDataFrame(left)
-        actual = private_join({"left": left_sdf, "right": right_sdf}).toPandas()
-        expected = pd.DataFrame(
-            [[2, 4, float(0)], [1, 3, float("inf")]], columns=["A", "B", "C"]
-        )
-        self.assert_frame_equal_with_sort(actual, expected)
-
     def test_join_without_nulls_changes_domain(self):
         """Test that when join_on_null=False, output domain does not allow null."""
         left_domain = SparkDataFrameDomain(
             {
                 "A": SparkFloatColumnDescriptor(),
                 "B": SparkStringColumnDescriptor(allow_null=True),
             }
@@ -854,21 +899,109 @@
             {
                 "A": SparkFloatColumnDescriptor(),
                 "B": SparkStringColumnDescriptor(allow_null=False),
                 "C": SparkFloatColumnDescriptor(allow_null=True),
             }
         )
         actual = private_join.output_domain
+        self.assertIsInstance(actual, SparkDataFrameDomain)
+        assert isinstance(actual, SparkDataFrameDomain)
         self.assertEqual(expected_output_domain["A"], actual["A"])
         self.assertEqual(expected_output_domain["B"], actual["B"])
         self.assertEqual(expected_output_domain["C"], actual["C"])
 
     @parameterized.expand(
         [
             (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+                ["B"],
+                True,
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+            ),
+            (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=True
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                    }
+                ),
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+                ["A"],
+                True,
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                        "B_left": SparkStringColumnDescriptor(allow_null=True),
+                        "B_right": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+            ),
+        ]
+    )
+    def test_output_domain_special_values(
+        self,
+        left_domain: SparkDataFrameDomain,
+        right_domain: SparkDataFrameDomain,
+        join_cols: List[str],
+        join_on_nulls: bool,
+        expected_domain: SparkDataFrameDomain,
+    ):
+        """Tests special values in output domain."""
+        transformation = PrivateJoin(
+            input_domain=DictDomain({"left": left_domain, "right": right_domain}),
+            left_key="left",
+            right_key="right",
+            left_truncation_strategy=TruncationStrategy.TRUNCATE,
+            right_truncation_strategy=TruncationStrategy.TRUNCATE,
+            left_truncation_threshold=10,
+            right_truncation_threshold=10,
+            join_cols=join_cols,
+            join_on_nulls=join_on_nulls,
+        )
+        self.assertEqual(transformation.output_domain, expected_domain)
+
+    @parameterized.expand(
+        [
+            (
                 True,
                 pd.DataFrame(
                     [["X", 1.2, 1.1], [None, 0.1, 1.2], [None, 0.1, 2.1]],
                     columns=["B", "A", "C"],
                 ),
             ),
             (False, pd.DataFrame([["X", 1.2, 1.1]], columns=["B", "A", "C"])),
@@ -1083,7 +1216,96 @@
             left_key="left",
             right_key="right",
             new_key="new",
             join_cols=["B"],
         )
         self.assertEqual(private_join.stability_relation(d_in, d_out), expected)
         self.assertEqual(private_join.stability_function(d_in) <= d_out, expected)
+
+    @parameterized.expand(
+        [
+            (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                    }
+                ),
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+                ["B"],
+                True,
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=True),
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=False, allow_inf=True, allow_nan=False
+                        ),
+                        "C": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=False, allow_nan=True
+                        ),
+                    }
+                ),
+            ),
+            (
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=True
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+                SparkDataFrameDomain(
+                    {
+                        "A": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                    }
+                ),
+                ["B"],
+                True,
+                SparkDataFrameDomain(
+                    {
+                        "B": SparkStringColumnDescriptor(allow_null=False),
+                        "A_left": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=True
+                        ),
+                        "A_right": SparkFloatColumnDescriptor(
+                            allow_null=True, allow_inf=True, allow_nan=False
+                        ),
+                    }
+                ),
+            ),
+        ]
+    )
+    def test_output_domain_special_values(
+        self,
+        left_domain: SparkDataFrameDomain,
+        right_domain: SparkDataFrameDomain,
+        join_cols: List[str],
+        join_on_nulls: bool,
+        expected_domain: SparkDataFrameDomain,
+    ):
+        """Tests that special values in output domain."""
+        transformation = PrivateJoinOnKey(
+            input_domain=DictDomain({"left": left_domain, "right": right_domain}),
+            input_metric=AddRemoveKeys({"left": "B", "right": "B"}),
+            left_key="left",
+            right_key="right",
+            new_key="joined",
+            join_cols=join_cols,
+            join_on_nulls=join_on_nulls,
+        )
+        self.assertEqual(
+            cast(DictDomain, transformation.output_domain).key_to_domain["joined"],
+            expected_domain,
+        )
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_map.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Unit tests for :mod:`~tmlt.core.transformations.spark_transformations.map`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-from typing import Callable, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
 import sympy as sp
 from parameterized import parameterized
 from pyspark import Row
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import ListDomain
 from tmlt.core.domains.spark_domains import (
+    SparkColumnDescriptor,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkRowDomain,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.metrics import (
@@ -542,15 +543,18 @@
             max_num_rows=2,
         )
         assert_property_immutability(t, prop_name)
 
     def test_properties(self):
         """GroupingFlatMap's properties have the expected values."""
         duplicate = lambda row: [{**row.asDict(), "G": 1}, {**row.asDict(), "G": 2}]
-        output_schema = {**self.schema_a, "G": SparkIntegerColumnDescriptor()}
+        output_schema: Dict[str, SparkColumnDescriptor] = {
+            **self.schema_a,
+            "G": SparkIntegerColumnDescriptor(),
+        }
         row_transformer = RowToRowsTransformation(
             input_domain=SparkRowDomain(self.schema_a),
             output_domain=ListDomain(SparkRowDomain(output_schema)),
             trusted_f=duplicate,
             augment=True,
         )
         transformation = GroupingFlatMap(
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_nan.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_nan.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,18 @@
             (
                 "One or more columns do not exist in the input domain",
                 ["column_that_does_not_exist"],
             ),
             ("At least one column must be specified", []),
             (re.escape("`columns` must not contain duplicate names"), ["B", "B"]),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 ["B"],
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
         ]
     )
     def test_invalid_constructor_args(
         self,
@@ -245,16 +247,18 @@
     @parameterized.expand(
         [
             ("Cannot drop NaNs from .* Only float columns can contain NaNs", ["A"]),
             ("One or more columns do not exist in the input domain", ["C"]),
             ("At least one column must be specified", []),
             ("`columns` must not contain duplicate names", ["B", "B"]),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 ["B"],
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
         ]
     )
     def test_invalid_constructor_args(
         self,
@@ -382,16 +386,18 @@
 
     @parameterized.expand(
         [
             ("One or more columns do not exist in the input domain", ["C"]),
             ("At least one column must be specified", []),
             ("`columns` must not contain duplicate names", ["B", "B"]),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 ["B"],
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
         ]
     )
     def test_invalid_constructor_args(
         self,
@@ -541,16 +547,18 @@
             ),
             (
                 "Column of type .* cannot contain values of "
                 + re.escape("infinity or -infinity"),
                 {"A": (-23, 45)},
             ),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 {"B": (1.0, 23.0)},
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
             (
                 # if this was supported, it would still not be allowed, because
                 # you can't replace on grouping column. See ReplaceNulls
                 "Can not group by a floating point column: B",
@@ -696,16 +704,18 @@
 
     @parameterized.expand(
         [
             ("One or more columns do not exist in the input domain", {"C": 0.1}),
             ("At least one column must be specified", {}),
             (r"Replacement value .* is invalid for column \(B\)", {"B": float("nan")}),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 {"B": 1.0},
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
             (
                 # if this was supported, it would still not be allowed, because
                 # you can't replace on grouping column. See ReplaceNulls
                 "Can not group by a floating point column: B",
@@ -853,16 +863,18 @@
     @parameterized.expand(
         [
             ("One or more columns do not exist in the input domain", {"C": 0.1}),
             ("At least one column must be specified", {}),
             (r"Replacement value .* is invalid for column \(B\)", {"B": None}),
             (r"Replacement value .* is invalid for column \(B\)", {"B": "X"}),
             (
-                "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
-                "or L1 or L2 over SymmetricDifference.",
+                (
+                    "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
+                    "or L1 or L2 over SymmetricDifference."
+                ),
                 {"B": 1.0},
                 IfGroupedBy("A", SumOf(AbsoluteDifference())),
             ),
             (
                 "Cannot replace values in the grouping column for IfGroupedBy.",
                 {"A": 1},
                 IfGroupedBy("A", SumOf(SymmetricDifference())),
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_partition.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         )
         partitions = transformation(sdf)
         for key, partition in zip(key_values, partitions):
             actual_rows = partition.collect()
             self.assertEqual(len(actual_rows), 1)
             assert (
                 actual_rows[0].A == key
-                or math.isnan(actual_rows[0].A)
+                or key is not None
+                and math.isnan(actual_rows[0].A)
                 and math.isnan(key)
             )
             assert actual_rows[0].B == 1
 
     @parameterized.expand(
         [
             (SymmetricDifference(), SumOf(SymmetricDifference()), 2, 2),
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_persist.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_persist.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,13 +86,14 @@
         assert_property_immutability(self.transformation, prop_name)
 
     def test_correctness(self):
         """SparkAction makes Spark evaluate and persist a DataFrame immediately."""
         # pylint: disable=protected-access
         df = self.spark.createDataFrame([(1,)], schema=["A"]).persist()
         assert df.is_cached
-        assert list(self.spark.sparkContext._jsc.sc().getRDDStorageInfo()) == []
+        # this will assert that the list is empty
+        assert not list(self.spark.sparkContext._jsc.sc().getRDDStorageInfo())
         df = self.transformation(df)
         self.assertEqual(
             len(list(self.spark.sparkContext._jsc.sc().getRDDStorageInfo())), 1
         )
         df.unpersist()
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_rename.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_rename.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_select.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_select.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/spark_transformations/test_truncation.py` & `tmlt_core-0.9.0/test/unit/transformations/spark_transformations/test_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/test_chaining.py` & `tmlt_core-0.9.0/test/unit/transformations/test_chaining.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,17 +171,19 @@
         else:
             self.assertEqual(
                 transformation.stability_function(1), stability_function_return_value2
             )
         if not stability_function_implemented1 and not use_hint:
             self.assertRaisesRegex(
                 ValueError,
-                "A hint is needed to check this privacy relation, because the "
-                "stability_relation of self.transformation1 raised  a "
-                "NotImplementedError: TEST",
+                (
+                    "A hint is needed to check this privacy relation, because the "
+                    "stability_relation of self.transformation1 raised  a "
+                    "NotImplementedError: TEST"
+                ),
             )
         else:
             self.assertEqual(
                 transformation.stability_relation(1, 1),
                 mock_transformation1.stability_relation(1, 1)
                 and mock_transformation2.stability_relation(1, 1),
             )
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/test_converters.py` & `tmlt_core-0.9.0/test/unit/transformations/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/transformations/test_dictionary.py` & `tmlt_core-0.9.0/test/unit/transformations/test_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,24 +146,25 @@
             ),
             stability_relation_return_value,
         )
 
     def test_correctness(self):
         """Tests that AugmentDictTransformation works correctly."""
         inner_transformation = self.get_mock_transformation(
-            return_value={"K": np.int(2)}
+            return_value={"K": np.int64(2)}
         )
         transformation = AugmentDictTransformation(transformation=inner_transformation)
-        input_dict = {"A": np.int(20), "B": np.int(123)}
+        input_dict = {"A": np.int64(20), "B": np.int64(123)}
 
         actual = transformation(input_dict)
         self.assertEqual(
-            inner_transformation.mock_calls, [call({"A": np.int(20), "B": np.int(123)})]
+            inner_transformation.mock_calls,
+            [call({"A": np.int64(20), "B": np.int64(123)})],
         )
-        self.assertEqual(actual, {**input_dict, "K": np.int(2)})
+        self.assertEqual(actual, {**input_dict, "K": np.int64(2)})
 
     @parameterized.expand(
         [
             (
                 "Invalid transformation input domain: Must be a DictDomain",
                 NumpyIntegerDomain(),
                 AbsoluteDifference(),
@@ -293,17 +294,19 @@
         )
         actual = transformation({"A": np.int_(20), ("B", "B"): np.int_(123)})
         self.assertEqual(actual, expected)
 
     @parameterized.expand(
         [
             (
-                "Input metric DictMetric(key_to_metric={'B': AbsoluteDifference()}) and"
-                " input domain DictDomain(key_to_domain={'A':"
-                " NumpyIntegerDomain(size=64)}) are not compatible.",
+                (
+                    "Input metric DictMetric(key_to_metric={'B': AbsoluteDifference()})"
+                    " and input domain DictDomain(key_to_domain={'A':"
+                    " NumpyIntegerDomain(size=64)}) are not compatible."
+                ),
                 DictDomain({"A": NumpyIntegerDomain()}),
                 DictMetric({"B": AbsoluteDifference()}),
                 "A",
             ),
             (
                 "'B' is not one of the input domain's keys",
                 DictDomain({"A": NumpyIntegerDomain()}),
@@ -503,17 +506,19 @@
             (
                 "No keys provided",
                 DictDomain({"A": NumpyIntegerDomain()}),
                 DictMetric({"A": AbsoluteDifference()}),
                 [],
             ),
             (
-                "Input metric AddRemoveKeys(df_to_key_column={'A': 'B'}) and input"
-                " domain DictDomain(key_to_domain={'A': NumpyIntegerDomain(size=64)})"
-                " are not compatible.",
+                (
+                    "Input metric AddRemoveKeys(df_to_key_column={'A': 'B'}) and input"
+                    " domain DictDomain(key_to_domain={'A':"
+                    " NumpyIntegerDomain(size=64)}) are not compatible."
+                ),
                 DictDomain({"A": NumpyIntegerDomain()}),
                 AddRemoveKeys({"A": "B"}),
                 ["A"],
             ),
         ]
     )
     def test_invalid_arguments_raises_error(
@@ -603,16 +608,16 @@
     def test_correctness(self):
         """Tests that CreateDictFromValue correctly applies transformation."""
         transformation = CreateDictFromValue(
             input_domain=NumpyIntegerDomain(),
             input_metric=AbsoluteDifference(),
             key="X",
         )
-        actual = transformation(np.int(20))
-        expected = {"X": np.int(20)}
+        actual = transformation(np.int64(20))
+        expected = {"X": np.int64(20)}
         self.assertEqual(actual, expected)
 
     @parameterized.expand([(False, 3, {"X": 3}), (True, 4, 4)])
     def test_stability_function_and_relation(
         self, use_add_remove_keys: bool, d_in: Any, d_out: Any
     ):
         """Tests that the stability function and relation are correct."""
@@ -633,16 +638,18 @@
         )
         self.assertEqual(transformation.stability_function(d_in), d_out)
         self.assertTrue(transformation.stability_relation(d_in, d_out))
 
     @parameterized.expand(
         [
             (
-                "Input metric must be IfGroupedBy with an inner metric of"
-                " SymmetricDifference to use AddRemoveKeys as the output metric",
+                (
+                    "Input metric must be IfGroupedBy with an inner metric of"
+                    " SymmetricDifference to use AddRemoveKeys as the output metric"
+                ),
                 NumpyIntegerDomain(),
                 AbsoluteDifference(),
                 "A",
                 True,
             )
         ]
     )
```

### Comparing `tmlt_core-0.8.3/test/unit/transformations/test_identity.py` & `tmlt_core-0.9.0/test/unit/transformations/test_identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_arb.py` & `tmlt_core-0.9.0/test/unit/utils/test_arb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,53 +26,53 @@
 
 
 class TestArb(TestCase):
     """Tests for :class:`tmlt.core.utils.arb.Arb`."""
 
     @parameterized.expand(
         [
-            (-42 * 10 ** 9,),
-            (-42 * 10 ** 7,),
+            (-42 * 10**9,),
+            (-42 * 10**7,),
             (-42,),
             (0,),
             (42,),
-            (42 * 10 ** 7,),
-            (42 * 10 ** 9,),
-            (42 * 10 ** 11,),
+            (42 * 10**7,),
+            (42 * 10**9,),
+            (42 * 10**11,),
         ]
     )
     def test_from_int(self, val: int):
         """Tests `Arb.from_int`."""
         x = Arb.from_int(val)
         man, exp = x.man_exp()
-        self.assertEqual(man * 2 ** exp, val)
+        self.assertEqual(man * 2**exp, val)
 
     @parameterized.expand([(0.0,), (1.1,), (-1.1,), (9.9 * 0.123,), (99.12,)])
     def test_from_float(self, val: float):
         """Tests `Arb.from_float`."""
         x = Arb.from_float(val)
         man, exp = x.man_exp()
-        self.assertEqual(man * 2 ** exp, val)
+        self.assertEqual(man * 2**exp, val)
 
     def test_from_float_inf(self):
         """Tests `Arb.from_float` works with +/- inf."""
         posinf = Arb.from_float(float("inf"))
         neginf = Arb.from_float(float("-inf"))
 
         self.assertFalse(posinf.is_finite())
         self.assertFalse(neginf.is_finite())
         self.assertEqual(float(posinf), float("inf"))
         self.assertEqual(float(neginf), float("-inf"))
 
-    @parameterized.expand([(2, 30), (4, 300), (5 * 10 ** 2, 7 ** 8)])
+    @parameterized.expand([(2, 30), (4, 300), (5 * 10**2, 7**8)])
     def test_from_man_exp(self, man: int, exp: int):
         """Tests `Arb.from_man_exp`."""
         x = Arb.from_man_exp(man, exp)
         m, e = x.man_exp()
-        self.assertEqual(m * 2 ** e, man * 2 ** exp)
+        self.assertEqual(m * 2**e, man * 2**exp)
 
     @parameterized.expand([(10, 1), (10000, 5), (10, 1), (10, 1)])
     def test_from_midpoint_radius(self, mid: int, rad: int):
         """Tests `Arb.from_midpoint_radius`."""
         mid_arb = Arb.from_int(mid)
         rad_arb = Arb.from_int(rad)
         x = Arb.from_midpoint_radius(mid_arb, rad_arb)
```

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_cleanup.py` & `tmlt_core-0.9.0/test/unit/utils/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_configuration.py` & `tmlt_core-0.9.0/test/unit/utils/test_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,19 @@
         self.assertTrue(len(Config.temp_db_name()) > 0)
         self.assertIn(Config.temp_db_name()[0], ascii_letters + digits)
 
     # pylint: disable=protected-access
     @parameterized.expand(
         [
             (
-                'openjdk version "1.8.0_292"\nOpenJDK Runtime Environment'
-                " (AdoptOpenJDK)(build 1.8.0_292-b10)\nOpenJDK 64-Bit Server VM"
-                " (AdoptOpenJDK)(build 25.292-b10, mixed mode)",
+                (
+                    'openjdk version "1.8.0_292"\nOpenJDK Runtime Environment'
+                    " (AdoptOpenJDK)(build 1.8.0_292-b10)\nOpenJDK 64-Bit Server VM"
+                    " (AdoptOpenJDK)(build 25.292-b10, mixed mode)"
+                ),
                 8,
             ),
             ("1.2.345_678", 2),
             ('un-open jdk version "11.987.654_321"', 11),
             ("15.43.21", 15),
             ("totally bogus version string", None),
         ]
@@ -137,17 +139,19 @@
                 self.assertEqual(_get_java_version(), expected)
         else:
             self.assertEqual(_get_java_version(), expected)
 
     @parameterized.expand(
         [
             (
-                'openjdk version "1.8.0_292"\nOpenJDK Runtime Environment'
-                " (AdoptOpenJDK)(build 1.8.0_292-b10)\nOpenJDK 64-Bit Server VM"
-                " (AdoptOpenJDK)(build 25.292-b10, mixed mode)",
+                (
+                    'openjdk version "1.8.0_292"\nOpenJDK Runtime Environment'
+                    " (AdoptOpenJDK)(build 1.8.0_292-b10)\nOpenJDK 64-Bit Server VM"
+                    " (AdoptOpenJDK)(build 25.292-b10, mixed mode)"
+                ),
                 8,
             ),
             ('Artisanal Handmade Java "1.2.345_678"', 2),
             ('un-open jdk version "11.987.654_321"', 11),
             ('some other kind of java "15.43.21"', 15),
             ("totally bogus version string", None),
         ]
```

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_distributions.py` & `tmlt_core-0.9.0/test/unit/utils/test_distributions.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_exact_number.py` & `tmlt_core-0.9.0/test/unit/utils/test_exact_number.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_grouped_dataframe.py` & `tmlt_core-0.9.0/test/unit/utils/test_grouped_dataframe.py`

 * *Files 25% similar despite different names*

```diff
@@ -71,30 +71,67 @@
         )
         expected = pd.DataFrame({"A": [1], "B": [2]})
         actual = grouped_dataframe.select(  # pylint:disable=protected-access
             ["A", "B"]
         )._dataframe.toPandas()
         self.assert_frame_equal_with_sort(actual, expected)
 
-    def test_null_safe_join(self) -> None:
-        """Test that _null_safe_join works correctly."""
-        data = pd.DataFrame({"A": [None, "a0", "a1"], "B": [1, 2, 3]})
+    def test_agg_with_nulls(self) -> None:
+        """Test that .agg works correctly with nulls."""
+        data = pd.DataFrame({"A": [None, "a0", "a0", "a1"], "B": [1, 2, 2, 3]})
         grouped_dataframe = GroupedDataFrame(
             dataframe=self.spark.createDataFrame(data),
-            group_keys=self.spark.createDataFrame(pd.DataFrame({"A": [None, "a999"]})),
+            group_keys=self.spark.createDataFrame(
+                pd.DataFrame({"A": [None, "a0", "a999"]})
+            ),
         )
-        expected_join_result = pd.DataFrame({"A": [None, "a999"], "B": [1, None]})
-        # pylint: disable=protected-access
-        self.assert_frame_equal_with_sort(
-            grouped_dataframe._null_safe_join(
-                self.spark.createDataFrame(data)
-            ).toPandas(),
-            expected_join_result,
+        expected = pd.DataFrame({"A": [None, "a0", "a999"], "sum(B)": [1, 4, 0]})
+        actual = grouped_dataframe.agg(sf.sum("B"), fill_value=0).toPandas()
+        self.assert_frame_equal_with_sort(actual, expected)
+
+    def test_apply_in_pandas_with_nulls(self) -> None:
+        """Test that .apply_in_pandas works correctly with nulls."""
+        data = pd.DataFrame({"A": [None, "a0", "a0", "a1"], "B": [1, 2, 2, 3]})
+        grouped_dataframe = GroupedDataFrame(
+            dataframe=self.spark.createDataFrame(data),
+            group_keys=self.spark.createDataFrame(
+                pd.DataFrame({"A": [None, "a0", "a999"]})
+            ),
         )
-        # pylint: enable=protected-access
+        expected = pd.DataFrame({"A": [None, "a0", "a999"], "sum(B)": [1, 4, 0]})
+        actual = grouped_dataframe.apply_in_pandas(
+            lambda df: pd.DataFrame({"sum(B)": [df["B"].sum()]}),
+            StructType([StructField("sum(B)", IntegerType())]),
+        ).toPandas()
+        self.assert_frame_equal_with_sort(actual, expected)
+
+    def test_agg_from_same_source(self) -> None:
+        """Previous implementations would fail when using the same source twice."""
+        data = self.spark.createDataFrame(
+            [("0", 1), ("1", 0), ("1", 2)], schema=["A", "B"]
+        )
+        group_keys = data.filter("B = 2")
+        grouped_dataframe = GroupedDataFrame(dataframe=data, group_keys=group_keys)
+        expected = pd.DataFrame({"A": ["1"], "B": [2], "count(1)": [1]})
+        actual = grouped_dataframe.agg(sf.count("*"), fill_value=0).toPandas()
+        self.assert_frame_equal_with_sort(actual, expected)
+
+    def test_apply_in_pandas_from_same_source(self) -> None:
+        """Previous implementations would fail when using the same source twice."""
+        data = self.spark.createDataFrame(
+            [("0", 1), ("1", 0), ("1", 2)], schema=["A", "B"]
+        )
+        group_keys = data.filter("B = 2")
+        grouped_dataframe = GroupedDataFrame(dataframe=data, group_keys=group_keys)
+        expected = pd.DataFrame({"A": ["1"], "B": [2], "count": [1]})
+        actual = grouped_dataframe.apply_in_pandas(
+            lambda df: pd.DataFrame({"count": [len(df)]}),
+            StructType([StructField("count", IntegerType())]),
+        ).toPandas()
+        self.assert_frame_equal_with_sort(actual, expected)
 
     def test_group_keys_no_rows_one_column(self):
         """Tests that group keys must have no columns it is empty."""
 
         with self.assertRaisesRegex(
             ValueError, "Group keys cannot have no rows, unless it also has no columns"
         ):
@@ -165,14 +202,50 @@
                 group_keys=self.spark.createDataFrame(group_keys),
             )
             .agg(sum_func, fill_value=0)
             .toPandas(),
             expected,
         )
 
+    @parameterized.expand(
+        [
+            (
+                pd.DataFrame([("A", 1), ("B", 4), ("B", 5)], columns=["X", "Y"]),
+                pd.DataFrame([("A",), ("B",)], columns=["X"]),
+                pd.DataFrame([("A", 1), ("B", 9)], columns=["X", "sum(Y)"]),
+            ),
+            (
+                pd.DataFrame([("A", 1), ("B", 4), ("C", 5)], columns=["X", "Y"]),
+                pd.DataFrame([("A",), ("B",)], columns=["X"]),
+                pd.DataFrame([("A", 1), ("B", 4)], columns=["X", "sum(Y)"]),
+            ),
+            (
+                pd.DataFrame([("A", 1), ("B", 4)], columns=["X", "Y"]),
+                pd.DataFrame([("A",), ("B",), ("C",)], columns=["X"]),
+                pd.DataFrame([("A", 1), ("B", 4), ("C", 0)], columns=["X", "sum(Y)"]),
+            ),
+        ]
+    )
+    def test_sum_apply_in_pandas(
+        self, df: pd.DataFrame, group_keys: pd.DataFrame, expected: pd.DataFrame
+    ):
+        """Tests that apply_in_pandas works as expected."""
+        self.assert_frame_equal_with_sort(
+            GroupedDataFrame(
+                dataframe=self.spark.createDataFrame(df),
+                group_keys=self.spark.createDataFrame(group_keys),
+            )
+            .apply_in_pandas(
+                lambda df: pd.DataFrame({"sum(Y)": [df["Y"].sum()]}),
+                StructType([StructField("sum(Y)", IntegerType())]),
+            )
+            .toPandas(),
+            expected,
+        )
+
     def test_empty_agg(self):
         """Tests that agg works for empty group keys."""
         sum_func = sf.sum(sf.col("Y")).alias("sum(Y)")
         self.assert_frame_equal_with_sort(
             GroupedDataFrame(
                 dataframe=self.spark.createDataFrame(
                     pd.DataFrame([("A", 1), ("B", 4)], columns=["X", "Y"])
@@ -180,14 +253,29 @@
                 group_keys=self.spark.createDataFrame([], schema=StructType()),
             )
             .agg(sum_func, fill_value=0)
             .toPandas(),
             pd.DataFrame({"sum(Y)": [5]}),
         )
 
+    def test_empty_apply_in_pandas(self):
+        """Tests that apply_in_pandas works for empty group keys."""
+        grouped_dataframe = GroupedDataFrame(
+            dataframe=self.spark.createDataFrame(
+                pd.DataFrame([("A", 1), ("B", 4)], columns=["X", "Y"])
+            ),
+            group_keys=self.spark.createDataFrame([], schema=StructType()),
+        )
+        actual = grouped_dataframe.apply_in_pandas(
+            lambda df: pd.DataFrame({"sum(Y)": [df["Y"].sum()]}),
+            StructType([StructField("sum(Y)", IntegerType())]),
+        ).toPandas()
+        expected = pd.DataFrame({"sum(Y)": [5]})
+        self.assert_frame_equal_with_sort(actual, expected)
+
     def test_agg_fill_value(self):
         """Tests that agg fills correct value for missing keys."""
         expected = pd.DataFrame({"X": ["A", "B"], "sum(Y)": [1, 10]})
         actual = (
             GroupedDataFrame(
                 dataframe=self.spark.createDataFrame([("A", 1)], schema=["X", "Y"]),
                 group_keys=self.spark.createDataFrame([("A",), ("B",)], schema=["X"]),
```

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_misc.py` & `tmlt_core-0.9.0/test/unit/utils/test_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test for :mod:`tmlt.core.utils.misc`"""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-from typing import Any, Callable
+from typing import Any, Callable, Dict
 
 import pandas as pd
 from parameterized import parameterized
 
 from tmlt.core.utils.misc import copy_if_mutable
 from tmlt.core.utils.testing import PySparkTest
 
@@ -41,15 +41,17 @@
         mutator(original)
         self.assertNotEqual(copied_item, original)
         self.assertNotEqual(reference_copy, original)
         self.assertEqual(copied_item, reference_copy)
 
     def test_no_deepcopy(self):
         """Still works for containers of immutable items that can't be deep-copied."""
-        original = {"key1": self.spark.createDataFrame(pd.DataFrame({"A": [1, 2, 3]}))}
+        original: Dict[str, Any] = {
+            "key1": self.spark.createDataFrame(pd.DataFrame({"A": [1, 2, 3]}))
+        }
         reference_copy = {
             "key1": self.spark.createDataFrame(pd.DataFrame({"A": [1, 2, 3]}))
         }
 
         copied_item = copy_if_mutable(original)
         self.assertEqual(list(copied_item), ["key1"])
         self.assertEqual(list(original), ["key1"])
```

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_testing.py` & `tmlt_core-0.9.0/test/unit/utils/test_testing.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_truncation.py` & `tmlt_core-0.9.0/test/unit/utils/test_truncation.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,32 +19,34 @@
     @parameterized.expand(
         [
             (2, [(1, "x"), (1, "y"), (1, "z"), (1, "w")], 2),
             (2, [(1, "x")], 1),
             (0, [(1, "x"), (1, "y"), (1, "z"), (1, "w")], 0),
         ]
     )
-    def test_correctness(self, threshold: int, rows: List[Tuple], expected_count: int):
+    def test_correctness(
+        self, threshold: int, rows: List[Tuple], expected_count: int
+    ) -> None:
         """Tests that truncate_large_groups works correctly."""
         df = self.spark.createDataFrame(rows, schema=["A", "B"])
         self.assertEqual(
             truncate_large_groups(df, ["A"], threshold).count(), expected_count
         )
 
-    def test_consistency(self):
+    def test_consistency(self) -> None:
         """Tests that truncate_large_groups does not truncate randomly across calls."""
         df = self.spark.createDataFrame([(i,) for i in range(1000)], schema=["A"])
 
         expected_output = truncate_large_groups(df, ["A"], 5).toPandas()
         for _ in range(5):
             self.assert_frame_equal_with_sort(
                 truncate_large_groups(df, ["A"], 5).toPandas(), expected_output
             )
 
-    def test_rows_dropped_consistently(self):
+    def test_rows_dropped_consistently(self) -> None:
         """Tests that truncate_large_groups drops that same rows for unchanged keys."""
         df1 = self.spark.createDataFrame(
             [("A", 1), ("B", 2), ("B", 3)], schema=["W", "X"]
         )
         df2 = self.spark.createDataFrame(
             [("A", 0), ("A", 1), ("B", 2), ("B", 3)], schema=["W", "X"]
         )
@@ -52,25 +54,46 @@
         df1_truncated = truncate_large_groups(df1, ["W"], 1)
         df2_truncated = truncate_large_groups(df2, ["W"], 1)
         self.assert_frame_equal_with_sort(
             df1_truncated.filter("W='B'").toPandas(),
             df2_truncated.filter("W='B'").toPandas(),
         )
 
-    def test_hash_truncation_order_agnostic(self):
+    def test_hash_truncation_order_agnostic(self) -> None:
         """Tests that truncate_large_groups doesn't depend on row order."""
         df_rows = [(1, 2, "A"), (3, 4, "A"), (5, 6, "A"), (7, 8, "B")]
 
         truncated_dfs: List[pd.DataFrame] = []
         for permutation in itertools.permutations(df_rows, 4):
             df = self.spark.createDataFrame(list(permutation), schema=["W", "X", "Y"])
             truncated_dfs.append(truncate_large_groups(df, ["Y"], 1).toPandas())
         for df in truncated_dfs[1:]:
             self.assert_frame_equal_with_sort(first_df=truncated_dfs[0], second_df=df)
 
+    def test_hash_truncation_duplicate_rows_not_clumped(self) -> None:
+        """Tests that truncate_large_groups doesn't clump duplicate rows together."""
+        df = self.spark.createDataFrame(
+            [
+                (1, 2, "A"),
+                (1, 2, "A"),
+                (1, 2, "A"),
+                (1, 2, "A"),
+                (1, 2, "A"),
+                (2, 4, "A"),
+                (2, 4, "A"),
+                (2, 4, "A"),
+                (2, 4, "A"),
+                (2, 4, "A"),
+            ],
+            schema=["X", "Y", "Z"],
+        )
+        actual = truncate_large_groups(df, ["Z"], threshold=5).toPandas()
+        assert isinstance(actual, pd.DataFrame)
+        assert len(actual.drop_duplicates()) == 2
+
 
 class TestDropLargeGroups(PySparkTest):
     """Tests for :meth:`~tmlt.core.utils.truncation.drop_large_groups`."""
 
     @parameterized.expand(
         [
             (1, [(1, "A"), (1, "B"), (2, "C")], [(2, "C")]),
@@ -78,13 +101,13 @@
             (2, [(1, "A"), (2, "C"), (2, "D"), (2, "E")], [(1, "A")]),
             (1, [(1, "A"), (1, "B"), (2, "C"), (2, "D"), (2, "E")], []),
             (0, [(1, "x"), (2, "y"), (3, "z"), (3, "w")], []),
         ]
     )
     def test_correctness(
         self, threshold: int, input_rows: List[Tuple], expected: List[Tuple]
-    ):
+    ) -> None:
         """Tests that drop_large_groups works correctly."""
         df = self.spark.createDataFrame(input_rows, schema=["A", "B"])
         actual = drop_large_groups(df, ["A"], threshold).toPandas()
         expected = pd.DataFrame.from_records(expected, columns=["A", "B"])
         self.assert_frame_equal_with_sort(actual, expected)
```

### Comparing `tmlt_core-0.8.3/test/unit/utils/test_type_utils.py` & `tmlt_core-0.9.0/test/unit/utils/test_type_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/domains/base.py` & `tmlt_core-0.9.0/tmlt/core/domains/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 class Domain(ABC):
     """Base class for input/output domains."""
 
     @property
     @abstractmethod
     def carrier_type(self) -> type:
         """Returns the type of elements in the domain."""
-        ...
 
     def validate(self, value: Any):
         """Raises an error if value is not in the domain."""
         if value.__class__ is not self.carrier_type:
             raise OutOfDomainError(
                 f"Value must be {self.carrier_type}, instead it is {value.__class__}."
             )
```

### Comparing `tmlt_core-0.8.3/tmlt/core/domains/collections.py` & `tmlt_core-0.9.0/tmlt/core/domains/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Domains for common python collections such as lists and dictionaries."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 from dataclasses import dataclass
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Mapping, Optional
 
 from typeguard import check_type, typechecked
 
 from tmlt.core.domains.base import Domain, OutOfDomainError
 
 
 @dataclass(frozen=True, eq=True)
@@ -34,28 +34,30 @@
     def validate(self, value: Any):
         """Raises error if value is not a row with matching schema."""
         super().validate(value)
         for elem in value:
             try:
                 self.element_domain.validate(elem)
             except OutOfDomainError as exception:
-                raise OutOfDomainError(f"Found invalid value in list: {exception}")
+                raise OutOfDomainError(
+                    f"Found invalid value in list: {exception}"
+                ) from exception
 
 
 class DictDomain(Domain):
     """Domain of dictionaries."""
 
     @typechecked
-    def __init__(self, key_to_domain: Dict[Any, Domain]):
+    def __init__(self, key_to_domain: Mapping[Any, Domain]):
         """Constructor.
 
         Args:
             key_to_domain: Mapping from key to domain.
         """
-        self._key_to_domain = key_to_domain.copy()
+        self._key_to_domain: Dict[Any, Domain] = dict(key_to_domain.items())
 
     def __repr__(self) -> str:
         """Return string representation of the object."""
         return f"{self.__class__.__name__}(key_to_domain={self.key_to_domain})"
 
     def __eq__(self, other: Any) -> bool:
         """Returns True if both domains are identical."""
@@ -92,8 +94,10 @@
                 f"keys: {value_keys}\nDomain keys: {domain_keys}"
             )
 
         for key in value:
             try:
                 self.key_to_domain[key].validate(value[key])
             except OutOfDomainError as exception:
-                raise OutOfDomainError(f"Found invalid value at '{key}': {exception}")
+                raise OutOfDomainError(
+                    f"Found invalid value at '{key}': {exception}"
+                ) from exception
```

### Comparing `tmlt_core-0.8.3/tmlt/core/domains/numpy_domains.py` & `tmlt_core-0.9.0/tmlt/core/domains/numpy_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/domains/pandas_domains.py` & `tmlt_core-0.9.0/tmlt/core/domains/pandas_domains.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         # iterating over a Series implicitly calls item() on the NumPy values
         # retrieving the corresponding python object
         super().validate(value)
         for i in range(len(value)):  # pylint: disable=consider-using-enumerate
             try:
                 self.element_domain.validate(value[i])
             except OutOfDomainError as exception:
-                raise OutOfDomainError(f"Found invalid value in Series: {exception}")
+                raise OutOfDomainError(
+                    f"Found invalid value in Series: {exception}"
+                ) from exception
 
     @classmethod
     def from_numpy_type(cls, dtype: np.dtype) -> "PandasSeriesDomain":
         """Returns a Pandas Series from a NumPy type."""
         return PandasSeriesDomain(NumpyDomain.from_np_type(dtype))
 
 
@@ -103,22 +105,22 @@
 
         for column in self.schema:
             try:
                 self.schema[column].validate(value[column])
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
                     f"Found invalid value in column '{column}': {exception}"
-                )
+                ) from exception
 
     def __eq__(self, other: Any) -> bool:
         """Return True if the classes are equivalent."""
         if self.__class__ != other.__class__:
             return False
         return OrderedDict(self.schema) == OrderedDict(other.schema)
 
     @classmethod
     def from_numpy_types(cls, dtypes: Dict[str, np.dtype]) -> "PandasDataFrameDomain":
         """Returns a Pandas DataFrame domain from a dictionary of NumPy types."""
-        col_to_desc = dict()
+        col_to_desc = {}
         for col in dtypes:
             col_to_desc[col] = PandasSeriesDomain.from_numpy_type(dtypes[col])
         return PandasDataFrameDomain(col_to_desc)
```

### Comparing `tmlt_core-0.8.3/tmlt/core/domains/spark_domains.py` & `tmlt_core-0.9.0/tmlt/core/domains/spark_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 import datetime
 import warnings
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from dataclasses import dataclass
-from typing import Any, Dict, Mapping, Optional, Sequence
+from typing import Any, Mapping, Optional, Sequence
 
 import numpy as np
 from pyspark import Row
 from pyspark.sql import DataFrame
 from pyspark.sql.types import (
     DataType,
     DateType,
@@ -31,30 +31,28 @@
 from tmlt.core.domains.numpy_domains import (
     NumpyDomain,
     NumpyFloatDomain,
     NumpyIntegerDomain,
     NumpyStringDomain,
 )
 from tmlt.core.domains.pandas_domains import PandasDataFrameDomain
-from tmlt.core.utils.grouped_dataframe import GroupedDataFrame
 
 
 class SparkColumnDescriptor(ABC):
     """Base class for describing Spark column types.
 
     Attributes:
         allow_null: If True, null values are permitted in the domain.
     """
 
     allow_null: bool
 
     @abstractmethod
     def to_numpy_domain(self) -> NumpyDomain:
         """Returns corresponding NumPy domain."""
-        ...
 
     def validate_column(self, sdf: DataFrame, col_name: str):
         """Raises error if not all values in given DataFrame column match descriptor.
 
         Args:
             sdf: Spark DataFrame to check.
             col_name: Name of column in sdf to be checked.
@@ -69,24 +67,22 @@
         if not self.allow_null:
             if sdf.filter(sdf[col_name].isNull()).first():
                 raise OutOfDomainError("Column contains null values.")
 
     @abstractmethod
     def valid_py_value(self, val: Any) -> bool:
         """Returns True if `val` is valid for described Spark column."""
-        ...
 
     @property
     @abstractmethod
     def data_type(self) -> DataType:
         """Returns data type associated with Spark column."""
-        ...
 
 
-SparkColumnsDescriptor = Dict[str, SparkColumnDescriptor]
+SparkColumnsDescriptor = Mapping[str, SparkColumnDescriptor]
 """Mapping from column name to SparkColumnDescriptor."""
 
 
 @dataclass(frozen=True)
 class SparkIntegerColumnDescriptor(SparkColumnDescriptor):
     """Describes an integer attribute in Spark."""
 
@@ -305,15 +301,15 @@
     @typechecked
     def __init__(self, schema: SparkColumnsDescriptor):
         """Constructor.
 
         Args:
             schema: Mapping from column names to column descriptors.
         """
-        self._schema = schema.copy()
+        self._schema = dict(schema.items())
 
     def __repr__(self) -> str:
         """Return string representation of the object."""
         return f"{self.__class__.__name__}(schema={self.schema})"
 
     @property
     def schema(self) -> SparkColumnsDescriptor:
@@ -346,15 +342,15 @@
     @typechecked
     def __init__(self, schema: SparkColumnsDescriptor):
         """Constructor.
 
         Args:
             schema: Mapping from column names to column descriptors.
         """
-        self._schema = schema.copy()
+        self._schema = dict(schema.items())
 
     def __repr__(self) -> str:
         """Return string representation of the object."""
         return f"{self.__class__.__name__}(schema={self.schema})"
 
     @property
     def schema(self) -> SparkColumnsDescriptor:
@@ -381,15 +377,15 @@
 
         for column in self.schema:
             try:
                 self.schema[column].validate_column(value, column)
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
                     f"Found invalid value in column '{column}': {exception}"
-                )
+                ) from exception
 
     def __eq__(self, other: Any) -> bool:
         """Return True if the classes are equivalent."""
         if self.__class__ != other.__class__:
             return False
         return OrderedDict(self.schema) == OrderedDict(other.schema)
 
@@ -495,15 +491,15 @@
             raise ValueError(f"Invalid groupby column: {invalid_groupby_column}")
 
         for column in group_keys.columns:
             if isinstance(schema[column], SparkFloatColumnDescriptor):
                 raise ValueError(f"Can not group by a floating point column: {column}")
             schema[column].validate_column(sdf=group_keys, col_name=column)
 
-        self._schema = schema.copy()
+        self._schema = dict(schema.items())
         self._group_keys = group_keys.distinct()
 
     @property
     def group_keys(self) -> DataFrame:
         """Returns DataFrame containing group keys as rows."""
         return self._group_keys
 
@@ -518,14 +514,19 @@
             f"{self.__class__.__name__}(schema={self.schema},"
             f" group_keys={self.group_keys})"
         )
 
     @property
     def carrier_type(self) -> type:
         """Returns carrier type for the domain."""
+        # avoid circular import
+        from tmlt.core.utils.grouped_dataframe import (  # pylint: disable=import-outside-toplevel
+            GroupedDataFrame,
+        )
+
         return GroupedDataFrame
 
     @property
     def spark_schema(self) -> StructType:
         """Returns Spark schema object according to domain.
 
         Note:
@@ -540,16 +541,20 @@
                 StructField(col, desc.data_type, desc.allow_null)
                 for col, desc in self.schema.items()
             ]
         )
 
     def validate(self, value: Any):
         """Raises error if value is not a GroupedDataFrame with matching group_keys."""
-        super().validate(value)
+        # avoid circular import
+        from tmlt.core.utils.grouped_dataframe import (  # pylint: disable=import-outside-toplevel
+            GroupedDataFrame,
+        )
 
+        super().validate(value)
         assert isinstance(value, GroupedDataFrame)
         if value.group_keys.schema != self.group_keys.schema:
             raise OutOfDomainError(
                 "Group keys dataframe does not have expected schema."
                 f"Expected: {self.group_keys.schema}. Got: {value.group_keys.schema}"
             )
 
@@ -593,15 +598,15 @@
             try:
                 self.schema[column].validate_column(
                     value._dataframe, column  # pylint: disable=protected-access
                 )
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
                     f"Found invalid value in column '{column}': {exception}"
-                )
+                ) from exception
 
     def get_group_domain(self) -> SparkDataFrameDomain:
         """Return the domain for one of the groups."""
         groupby_columns = self.group_keys.columns
         group_schema = {
             column: v
             for column, v in self.schema.items()
@@ -653,15 +658,15 @@
     """Returns mapping from column name to SparkColumnDescriptor."""
     spark_type_to_size: Mapping[DataType, int] = {
         IntegerType(): 32,
         LongType(): 64,
         FloatType(): 32,
         DoubleType(): 64,
     }
-    column_to_descriptor = dict()
+    column_to_descriptor = {}
     for field in spark_schema:
         if field.name in column_to_descriptor:
             raise ValueError(f"Schema contains duplicate column name {field.name}.")
         column_to_descriptor[field.name] = _spark_type_to_descriptor(
             field.dataType, field.nullable, spark_type_to_size.get(field.dataType)
         )
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/aggregations.py` & `tmlt_core-0.9.0/tmlt/core/measurements/aggregations.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from tmlt.core.transformations.spark_transformations.groupby import GroupBy
 from tmlt.core.transformations.spark_transformations.map import (
     Map,
     RowToRowTransformation,
 )
 from tmlt.core.utils.distributions import double_sided_geometric_inverse_cmf
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
+from tmlt.core.utils.join import join
 from tmlt.core.utils.misc import get_nonconflicting_string
 from tmlt.core.utils.parameters import calculate_noise_scale
 
 
 class NoiseMechanism(Enum):
     """Enumerating noise mechanisms."""
 
@@ -230,19 +231,19 @@
             add_noise_to_number = AddLaplaceNoise(
                 scale=noise_scale, input_domain=NumpyIntegerDomain()
             )
         elif noise_mechanism == NoiseMechanism.GEOMETRIC:
             add_noise_to_number = AddGeometricNoise(alpha=noise_scale)
         elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
             add_noise_to_number = AddDiscreteGaussianNoise(
-                sigma_squared=noise_scale ** 2
+                sigma_squared=noise_scale**2
             )
         elif noise_mechanism == NoiseMechanism.GAUSSIAN:
             add_noise_to_number = AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=NumpyIntegerDomain()
+                sigma_squared=noise_scale**2, input_domain=NumpyIntegerDomain()
             )
         else:
             raise ValueError(
                 f"Unrecognized noise mechanism {noise_mechanism}. "
                 "Supported noise mechanisms are LAPLACE, "
                 "GEOMETRIC, GAUSSIAN, and DISCRETE_GAUSSIAN."
             )
@@ -273,20 +274,20 @@
         add_noise_to_series = AddNoiseToSeries(
             AddLaplaceNoise(scale=noise_scale, input_domain=NumpyIntegerDomain())
         )
     elif noise_mechanism == NoiseMechanism.GEOMETRIC:
         add_noise_to_series = AddNoiseToSeries(AddGeometricNoise(alpha=noise_scale))
     elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
-            AddDiscreteGaussianNoise(sigma_squared=noise_scale ** 2)
+            AddDiscreteGaussianNoise(sigma_squared=noise_scale**2)
         )
     elif noise_mechanism == NoiseMechanism.GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
             AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=NumpyIntegerDomain()
+                sigma_squared=noise_scale**2, input_domain=NumpyIntegerDomain()
             )
         )
 
     else:
         raise ValueError(
             f"Unrecognized noise mechanism {noise_mechanism}. "
             "Supported noise mechanisms are LAPLACE, "
@@ -429,19 +430,19 @@
             add_noise_to_number = AddLaplaceNoise(
                 scale=noise_scale, input_domain=NumpyIntegerDomain()
             )
         elif noise_mechanism == NoiseMechanism.GEOMETRIC:
             add_noise_to_number = AddGeometricNoise(alpha=noise_scale)
         elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
             add_noise_to_number = AddDiscreteGaussianNoise(
-                sigma_squared=noise_scale ** 2
+                sigma_squared=noise_scale**2
             )
         elif noise_mechanism == NoiseMechanism.GAUSSIAN:
             add_noise_to_number = AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=NumpyIntegerDomain()
+                sigma_squared=noise_scale**2, input_domain=NumpyIntegerDomain()
             )
         else:
             raise ValueError(
                 f"Unrecognized noise mechanism {noise_mechanism}. "
                 "Supported noise mechanisms are LAPLACE, "
                 "GEOMETRIC, GAUSSIAN, and DISCRETE_GAUSSIAN."
             )
@@ -485,20 +486,20 @@
         add_noise_to_series = AddNoiseToSeries(
             AddLaplaceNoise(scale=noise_scale, input_domain=NumpyIntegerDomain())
         )
     elif noise_mechanism == NoiseMechanism.GEOMETRIC:
         add_noise_to_series = AddNoiseToSeries(AddGeometricNoise(alpha=noise_scale))
     elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
-            AddDiscreteGaussianNoise(sigma_squared=noise_scale ** 2)
+            AddDiscreteGaussianNoise(sigma_squared=noise_scale**2)
         )
     elif noise_mechanism == NoiseMechanism.GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
             AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=NumpyIntegerDomain()
+                sigma_squared=noise_scale**2, input_domain=NumpyIntegerDomain()
             )
         )
     else:
         raise ValueError(
             f"Unrecognized noise mechanism {noise_mechanism}. "
             "Supported noise mechanisms are LAPLACE, "
             "GEOMETRIC, GAUSSIAN, and DISCRETE_GAUSSIAN."
@@ -655,19 +656,19 @@
                 scale=noise_scale, input_domain=measure_column_domain
             )
         elif noise_mechanism == NoiseMechanism.GEOMETRIC:
             add_noise_to_number = AddGeometricNoise(alpha=noise_scale)
 
         elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
             add_noise_to_number = AddDiscreteGaussianNoise(
-                sigma_squared=noise_scale ** 2
+                sigma_squared=noise_scale**2
             )
         elif noise_mechanism == NoiseMechanism.GAUSSIAN:
             add_noise_to_number = AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=measure_column_domain
+                sigma_squared=noise_scale**2, input_domain=measure_column_domain
             )
         else:
             raise ValueError(
                 f"Unrecognized noise mechanism d P {noise_mechanism}. "
                 "Supported noise mechanisms are LAPLACE, "
                 "GEOMETRIC, GAUSSIAN, and DISCRETE_GAUSSIAN."
             )
@@ -701,20 +702,20 @@
         add_noise_to_series = AddNoiseToSeries(
             AddLaplaceNoise(scale=noise_scale, input_domain=measure_column_domain)
         )
     elif noise_mechanism == NoiseMechanism.GEOMETRIC:
         add_noise_to_series = AddNoiseToSeries(AddGeometricNoise(alpha=noise_scale))
     elif noise_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
-            AddDiscreteGaussianNoise(sigma_squared=noise_scale ** 2)
+            AddDiscreteGaussianNoise(sigma_squared=noise_scale**2)
         )
     elif noise_mechanism == NoiseMechanism.GAUSSIAN:
         add_noise_to_series = AddNoiseToSeries(
             AddGaussianNoise(
-                sigma_squared=noise_scale ** 2, input_domain=measure_column_domain
+                sigma_squared=noise_scale**2, input_domain=measure_column_domain
             )
         )
     else:
         raise ValueError(
             f"Unrecognized noise mechanism {noise_mechanism}. "
             "Supported noise mechanisms are LAPLACE, "
             "GEOMETRIC, GAUSSIAN, and DISCRETE_GAUSSIAN."
@@ -924,15 +925,15 @@
         ) -> Union[
             np.int64,
             np.float64,
             Dict[str, Union[Union[float, np.int64], Union[int, np.float64]]],
         ]:
             """Computes average from noisy count and sum of deviations."""
             sod, count = answers
-            average = sod / max(1, count) + midpoint_of_measure_column
+            average = sod / max(1, count) + midpoint_of_measure_column  # type: ignore
             if keep_intermediates:
                 return {
                     "average": average,
                     "sum_of_deviations": sod,
                     "count": count,
                     "midpoint_of_deviations": midpoint_of_measure_column,
                 }
@@ -984,22 +985,30 @@
         assert (
             average_column is not None
             and sum_column is not None
             and count_column is not None
         )
         sod_df, count_df = answers
         if groupby.groupby_columns:
-            df_with_sod_and_count = sod_df.join(count_df, on=groupby.groupby_columns)
+            df_with_sod_and_count = join(
+                left=sod_df,
+                right=count_df,
+                on=groupby.groupby_columns,
+                how="inner",  # same groups
+                nulls_are_equal=True,
+            )
         else:
             temp_column = get_nonconflicting_string(sod_df.columns + count_df.columns)
-            df_with_sod_and_count = (
-                sod_df.withColumn(temp_column, sf.lit(1))
-                .join(count_df.withColumn(temp_column, sf.lit(1)), on=[temp_column])
-                .drop(temp_column)
-            )
+            df_with_sod_and_count = join(
+                left=sod_df.withColumn(temp_column, sf.lit(1)),
+                right=count_df.withColumn(temp_column, sf.lit(1)),
+                on=[temp_column],
+                how="inner",  # only one row
+                nulls_are_equal=False,  # no nulls
+            ).drop(temp_column)
 
         df_with_all_columns = df_with_sod_and_count.withColumn(
             average_column,
             (sf.col(sum_column) / sf.greatest(sf.lit(1), sf.col(count_column)))
             + sf.lit(midpoint_of_measure_column),
         )
         if keep_intermediates:
@@ -1157,17 +1166,17 @@
         upper,
         integer_midpoint=isinstance(
             input_domain[measure_column], SparkIntegerColumnDescriptor
         ),
     )
 
     lower_after_squaring: ExactNumber = (
-        ExactNumber(0) if lower <= 0 <= upper else min(lower ** 2, upper ** 2)
+        ExactNumber(0) if lower <= 0 <= upper else min(lower**2, upper**2)
     )
-    upper_after_squaring: ExactNumber = max(lower ** 2, upper ** 2)
+    upper_after_squaring: ExactNumber = max(lower**2, upper**2)
     (
         midpoint_of_squared_measure_column,
         exact_midpoint_of_squared_measure_column,
     ) = get_midpoint(
         lower_after_squaring,
         upper_after_squaring,
         integer_midpoint=isinstance(
@@ -1239,15 +1248,15 @@
             Dict[str, Union[Union[float, np.int64], Union[int, np.float64]]],
         ]:
             """Computes variance from noisy count and sums of deviations."""
             sod, sos, count = answers
             variance: Any
             if count <= 1:
                 variance = (
-                    midpoint_of_squared_measure_column - midpoint_of_measure_column ** 2
+                    midpoint_of_squared_measure_column - midpoint_of_measure_column**2
                 )
             else:
                 variance = (sos / count + midpoint_of_squared_measure_column) - (
                     sod / count + midpoint_of_measure_column
                 ) ** 2
                 if variance < 0:
                     variance = 0
@@ -1338,25 +1347,43 @@
             and sum_of_deviations_column is not None
             and sum_of_squared_deviations_column is not None
             and count_column is not None
         )
         sod_df, sos_df, count_df = answers
         assert groupby_transformation is not None
         if groupby.groupby_columns:
-            df_with_sums_and_count = sod_df.join(
-                sos_df, on=groupby.groupby_columns
-            ).join(count_df, on=groupby.groupby_columns)
-        else:
-            temp_column = get_nonconflicting_string(sod_df.columns + count_df.columns)
-            df_with_sums_and_count = (
-                sod_df.withColumn(temp_column, sf.lit(1))
-                .join(sos_df.withColumn(temp_column, sf.lit(1)), on=[temp_column])
-                .join(count_df.withColumn(temp_column, sf.lit(1)), on=[temp_column])
-                .drop(temp_column)
+            df_with_sums_and_count = join(
+                left=join(
+                    left=sod_df,
+                    right=sos_df,
+                    on=groupby.groupby_columns,
+                    how="inner",  # same groups
+                    nulls_are_equal=True,
+                ),
+                right=count_df,
+                on=groupby.groupby_columns,
+                how="inner",
+                nulls_are_equal=True,
             )
+        else:
+            temp_column = get_nonconflicting_string(sod_df.columns + sos_df.columns)
+            df_with_sums_and_count = join(
+                left=join(
+                    left=sod_df.withColumn(temp_column, sf.lit(1)),
+                    right=sos_df.withColumn(temp_column, sf.lit(1)),
+                    on=[temp_column],
+                    how="inner",  # only one row
+                    nulls_are_equal=False,  # no nulls
+                ),
+                right=count_df.withColumn(temp_column, sf.lit(1)),
+                on=[temp_column],
+                how="inner",
+                nulls_are_equal=False,
+            ).drop(temp_column)
+
         df_with_all_columns = df_with_sums_and_count.withColumn(
             variance_column,
             sf.when(
                 sf.col(count_column) <= 1,
                 sf.lit(midpoint_of_squared_measure_column)
                 - sf.lit(midpoint_of_measure_column) ** 2,
             ).otherwise(
@@ -1780,17 +1807,17 @@
         upper,
         integer_midpoint=isinstance(
             input_domain[measure_column], SparkIntegerColumnDescriptor
         ),
     )
 
     lower_after_squaring: ExactNumber = (
-        ExactNumber(0) if lower <= 0 <= upper else min(lower ** 2, upper ** 2)
+        ExactNumber(0) if lower <= 0 <= upper else min(lower**2, upper**2)
     )
-    upper_after_squaring: ExactNumber = max(lower ** 2, upper ** 2)
+    upper_after_squaring: ExactNumber = max(lower**2, upper**2)
     (midpoint_of_squared_measure_column, _) = get_midpoint(
         lower_after_squaring,
         upper_after_squaring,
         integer_midpoint=isinstance(
             input_domain[measure_column], SparkIntegerColumnDescriptor
         ),
     )
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/base.py` & `tmlt_core-0.9.0/tmlt/core/measurements/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,8 +89,7 @@
             d_out: Distance between outputs under `output_measure`.
         """
         return self.output_measure.compare(self.privacy_function(d_in), d_out)
 
     @abstractmethod
     def __call__(self, data: Any) -> Any:
         """Performs measurement."""
-        ...
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/chaining.py` & `tmlt_core-0.9.0/tmlt/core/measurements/chaining.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             d_mid = self.transformation.stability_function(d_in)
         except NotImplementedError as e:
             if self._hint is None:
                 raise ValueError(
                     "A hint is needed to check this privacy relation, because the "
                     "stability_relation of self.transformation raised a "
                     f"NotImplementedError: {e}"
-                )
+                ) from e
             d_mid = self._hint(d_in, d_out)
         return self.transformation.stability_relation(
             d_in, d_mid
         ) and self.measurement.privacy_relation(d_mid, d_out)
 
     def __call__(self, data: Any) -> Any:
         """Computes measurement after applying transformation on input data."""
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/composition.py` & `tmlt_core-0.9.0/tmlt/core/measurements/composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Measurement for combining multiple measurements into a single measurement."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable, List, Optional, Sequence, Tuple
 
 from typeguard import typechecked
 
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
 
 
 class Composition(Measurement):
     """Describes a measurement constructed by composing two or more Measurements."""
 
     @typechecked
     def __init__(
         self,
-        measurements: List[Measurement],
+        measurements: Sequence[Measurement],
         hint: Optional[Callable[[Any, Any], Tuple[Any, ...]]] = None,
     ):
         """Constructor.
 
         It supports PureDP, ApproxDP, and RhoZCDP. Input metrics, domains, and
         output measures must be identical across all supplied measurements.
 
@@ -69,15 +69,15 @@
 
         super().__init__(
             input_domain=input_domain,
             input_metric=input_metric,
             output_measure=output_measure,
             is_interactive=False,
         )
-        self._measurements = measurements.copy()
+        self._measurements = list(measurements)
         self._hint = hint
 
     @property
     def measurements(self) -> List[Measurement]:
         """Returns the list of measurements being composed."""
         return self._measurements.copy()
 
@@ -132,15 +132,15 @@
             return super().privacy_relation(d_in, d_out)
         except NotImplementedError as e:
             if self._hint is None:
                 raise ValueError(
                     "A hint is needed to check this privacy relation, because the "
                     "privacy_relation from one of self.measurements raised a "
                     f"NotImplementedError: {e}"
-                )
+                ) from e
         d_outs = self._hint(d_in, d_out)
         if len(d_outs) != len(self.measurements):
             raise RuntimeError(
                 f"Hint function produced {len(d_outs)} output measure values,"
                 f" expected {len(self.measurements)}."
             )
         if not all(
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/converters.py` & `tmlt_core-0.9.0/tmlt/core/measurements/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         Raises:
             NotImplementedError: If self.pure_dp_measurement.privacy_function(d_in)
                 raises :class:`NotImplementedError`.
         """
         epsilon = self.pure_dp_measurement.privacy_function(d_in)
         assert isinstance(epsilon, ExactNumber)
-        rho = (epsilon ** 2) / 2
+        rho = (epsilon**2) / 2
         self.output_measure.validate(rho)
         return rho
 
     @typechecked
     def privacy_relation(self, d_in: Any, d_out: ExactNumberInput) -> bool:
         r"""Return True if close inputs produce close outputs.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/interactive_measurements.py` & `tmlt_core-0.9.0/tmlt/core/measurements/interactive_measurements.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         All subclasses of Queryable should have exactly one public
         method: `__call__`.
     """
 
     @abstractmethod
     def __call__(self, query: Any):
         """Returns answer to given query."""
-        ...
 
 
 @dataclass
 class MeasurementQuery:
     """Contains a Measurement and the `d_out` it satisfies.
 
     Note:
@@ -1638,16 +1637,18 @@
             raise RuntimeError(
                 "Can not retire PrivacyAccountant in WAITING_FOR_CHILDREN state."
                 " Set the `force` flag to retire this PrivacyAccountant and all"
                 " its children."
             )
         if self.state == PrivacyAccountantState.WAITING_FOR_SIBLING:
             warn(
-                "Retiring an unused PrivacyAccountant that is"
-                " PrivacyAccountantState.WAITING_FOR_SIBLING.",
+                (
+                    "Retiring an unused PrivacyAccountant that is"
+                    " PrivacyAccountantState.WAITING_FOR_SIBLING."
+                ),
                 RuntimeWarning,
             )
 
         if self.state != PrivacyAccountantState.ACTIVE:
             # If this PrivacyAccountant is WAITING_FOR_CHILDREN, this retires all child
             # accountants and their descendants. If it is WAITING_FOR_SIBLINGS, this
             # retires all preceding siblings.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/noise_mechanisms.py` & `tmlt_core-0.9.0/tmlt/core/measurements/noise_mechanisms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Copyright Tumult Labs 2022
 
 import random
 from fractions import Fraction
 from typing import Union, cast
 
 import numpy as np
-import scipy.stats as stats
 from pyspark.sql.types import DataType, DoubleType, LongType
+from scipy import stats
 from typeguard import typechecked
 
 from tmlt.core.domains.numpy_domains import (
     NumpyDomain,
     NumpyFloatDomain,
     NumpyIntegerDomain,
 )
@@ -106,15 +106,17 @@
             d_in: Distance between inputs under input_metric.
         """
         self.input_metric.validate(d_in)
         if self.scale == 0:
             return ExactNumber(float("inf"))
         return d_in / self.scale
 
-    def __call__(self, val: Union[np.int32, np.int64, np.float32, np.float64]) -> float:
+    def __call__(
+        self, val: Union[np.int32, np.int64, np.float32, np.float64, float, int]
+    ) -> float:
         r"""Returns the value with laplace noise added.
 
         The added laplace noise has the probability density function
 
         :math:`f(x) = \frac{1}{2 b} e ^ {\frac{-\mid x \mid}{b}}`
 
         where:
@@ -220,15 +222,15 @@
             d_in: Distance between inputs under input_metric.
         """
         self.input_metric.validate(d_in)
         if self.alpha == 0:
             return ExactNumber(float("inf"))
         return d_in / self.alpha
 
-    def __call__(self, value: Union[np.int32, np.int64]) -> int:
+    def __call__(self, value: Union[np.int32, np.int64, float, int]) -> int:
         r"""Returns the value with double sided geometric noise added.
 
         The added noise has the probability mass function
 
         .. math::
 
             f(k)=
@@ -364,15 +366,15 @@
             d_in: Distance between inputs under input_metric.
         """
         self.input_metric.validate(d_in)
         if self.sigma_squared == 0:
             return ExactNumber(float("inf"))
         return (ExactNumber(d_in) ** 2) / (2 * self._sigma_squared)
 
-    def __call__(self, value: Union[np.int32, np.int64]) -> int:
+    def __call__(self, value: Union[np.int32, np.int64, float, int]) -> int:
         r"""Adds discrete Gaussian noise with specified scale.
 
         The added noise has the probability mass function
 
         .. math::
 
             f(k) = \frac
@@ -490,15 +492,15 @@
         """
         self.input_metric.validate(d_in)
         if self.sigma_squared == 0:
             return ExactNumber(float("inf"))
         return (ExactNumber(d_in) ** 2) / (2 * self._sigma_squared)
 
     def __call__(
-        self, value: Union[np.int32, np.int64, np.float32, np.float64]
+        self, value: Union[np.int32, np.int64, np.float32, np.float64, float, int]
     ) -> float:
         r"""Adds Gaussian noise with specified scale.
 
         The added noise has the probability density function
 
         .. math::
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/pandas_measurements/dataframe.py` & `tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     def output_schema(self) -> StructType:
         """Return the output schema."""
         return self._output_schema
 
     @abstractmethod
     def __call__(self, df: pd.DataFrame) -> pd.DataFrame:
         """Perform measurement."""
-        ...
 
 
 class AggregateByColumn(Aggregate):
     """Apply Aggregate measurements to columns of a Pandas DataFrame."""
 
     @typechecked
     def __init__(
@@ -224,15 +223,15 @@
             return super().privacy_relation(d_in, d_out)
         except NotImplementedError as e:
             if self._hint is None:
                 raise ValueError(
                     "A hint is needed to check this privacy relation, because the "
                     "privacy_relation from one of self.column_to_aggregation.values() "
                     f"raised a NotImplementedError: {e}"
-                )
+                ) from e
         assert self._hint is not None
         d_outs = self._hint(d_in, d_out)
         if set(d_outs) != set(self.column_to_aggregation):
             raise ValueError(
                 "The columns produced by the hint function don't match"
                 " the columns to be aggregated."
             )
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/pandas_measurements/series.py` & `tmlt_core-0.9.0/tmlt/core/measurements/pandas_measurements/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def output_spark_type(self) -> DataType:
         """Return the Spark type of the aggregated value."""
         return self._output_spark_type
 
     @abstractmethod
     def __call__(self, data: pd.Series) -> Union[float, int]:
         """Perform measurement."""
-        ...
 
 
 class NoisyQuantile(Aggregate):
     """Estimates the quantile of a Pandas Series."""
 
     @typechecked
     def __init__(
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/postprocess.py` & `tmlt_core-0.9.0/tmlt/core/measurements/postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/measurements/spark_measurements.py` & `tmlt_core-0.9.0/tmlt/core/measurements/spark_measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,17 +210,18 @@
         Raises:
             NotImplementedError: If the :meth:`~.Measurement.privacy_function` of the
                 :class:`~.AddNoiseToSeries` measurement raises :class:`NotImplementedError`.
         """
         self.input_metric.validate(d_in)
         return self.measurement.privacy_function(d_in)
 
-    def call(self, sdf: DataFrame) -> DataFrame:
+    def call(self, val: DataFrame) -> DataFrame:
         """Applies measurement to measure column."""
         # TODO(#2107): Fix typing once pd.Series is a usable type
+        sdf = val
         udf = sf.pandas_udf(  # type: ignore
             self.measurement, self.measurement.output_type, sf.PandasUDFType.SCALAR
         ).asNondeterministic()
         sdf = sdf.withColumn(self.measure_column, udf(sdf[self.measure_column]))
         return sdf
 
 
@@ -312,16 +313,17 @@
 
         Raises:
             NotImplementedError: If self.aggregation_function.privacy_function(d_in)
                 raises :class:`NotImplementedError`.
         """
         return self.aggregation_function.privacy_function(d_in)
 
-    def call(self, grouped_dataframe: GroupedDataFrame) -> DataFrame:
+    def call(self, val: GroupedDataFrame) -> DataFrame:
         """Returns DataFrame obtained by applying pandas aggregation to each group."""
+        grouped_dataframe = val
         return grouped_dataframe.select(
             grouped_dataframe.groupby_columns
             + list(self.aggregation_function.input_domain.schema)
         ).apply_in_pandas(
             aggregation_function=self.aggregation_function,
             aggregation_output_schema=self.aggregation_function.output_schema,
         )
@@ -457,15 +459,15 @@
             validate_exact_number(
                 value=alpha,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid alpha: {e}")
+            raise ValueError(f"Invalid alpha: {e}") from e
         if count_column is None:
             count_column = "count"
         if count_column in set(input_domain.schema):
             raise ValueError(
                 f"Invalid count column name: ({count_column}) column already exists"
             )
         self._alpha = ExactNumber(alpha)
@@ -522,16 +524,17 @@
             d_in * base_epsilon,
             min(
                 ExactNumber(1),
                 d_in * ExactNumber(sp.E) ** (d_in * base_epsilon) * base_delta,
             ),
         )
 
-    def call(self, sdf: DataFrame) -> DataFrame:
+    def call(self, val: DataFrame) -> DataFrame:
         """Return the noisy counts for common rows."""
+        sdf = val
         count_df = sdf.groupBy(sdf.columns).agg(sf.count("*").alias(self.count_column))
         internal_measurement = AddNoiseToColumn(
             input_domain=SparkDataFrameDomain(
                 schema={
                     **cast(SparkDataFrameDomain, self.input_domain).schema,
                     self.count_column: SparkIntegerColumnDescriptor(),
                 }
```

### Comparing `tmlt_core-0.8.3/tmlt/core/measures.py` & `tmlt_core-0.9.0/tmlt/core/measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,18 @@
     @abstractmethod
     def validate(self, value: Any):
         """Raises an error if `value` not a valid distance.
 
         Args:
             value: A distance between two probability distributions under this measure.
         """
-        ...
 
     @abstractmethod
     def compare(self, value1: Any, value2: Any) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
-        ...
 
     def __repr__(self) -> str:
         """Returns string representation."""
         return f"{self.__class__.__name__}()"
 
 
 class PureDP(Measure):
@@ -56,15 +54,15 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid PureDP measure value (epsilon) {e}")
+            raise ValueError(f"Invalid PureDP measure value (epsilon) {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
@@ -96,15 +94,17 @@
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
                 maximum=1,
                 maximum_is_inclusive=True,
             )
         except (ValueError, TypeError) as e:
-            raise ValueError(f"Invalid ApproxDP measure value (epsilon,delta): {e}")
+            raise ValueError(
+                f"Invalid ApproxDP measure value (epsilon,delta): {e}"
+            ) from e
 
     def compare(
         self,
         value1: Tuple[ExactNumberInput, ExactNumberInput],
         value2: Tuple[ExactNumberInput, ExactNumberInput],
     ) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
@@ -137,15 +137,15 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid RhoZCDP measure value (rho): {e}")
+            raise ValueError(f"Invalid RhoZCDP measure value (rho): {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
@@ -190,43 +190,39 @@
         assert isinstance(measure, RhoZCDP)
         return RhoZCDPBudget(value)
 
     @property
     @abstractmethod
     def value(self) -> PrivacyBudgetValue:
         """Return the value of the privacy budget."""
-        ...
 
     @abstractmethod
     def is_finite(self) -> bool:
         """Return true iff the budget is finite."""
-        ...
 
     @abstractmethod
     def can_spend_budget(self, other: PrivacyBudgetInput) -> bool:
         """Return true iff we can spend budget `other`.
 
         Args:
             other: The privacy budget we would like to spend.
         """
-        ...
 
     @abstractmethod
     def subtract(self, other: PrivacyBudgetInput) -> "PrivacyBudget":
         """Return a new budget after subtracting `other`.
 
         If the budget represented by this class is infinite, return the current budget.
 
         Args:
             other: The privacy budget to subtract.
 
         Raises:
             ValueError: If there is not enough privacy budget to subtract other.
         """
-        ...
 
     def __eq__(self, other: Any) -> bool:
         """Check is this instance is equal to `other`.
 
         Args:
             other: The other instance.
         """
```

### Comparing `tmlt_core-0.8.3/tmlt/core/metrics.py` & `tmlt_core-0.9.0/tmlt/core/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 # pylint: disable=no-member
 
 from abc import ABC, abstractmethod
 from collections import Counter
 from functools import reduce
-from typing import Any, Dict, Iterable, List, Tuple, Union, cast
+from typing import Any, Dict, Iterable, List, Mapping, Tuple, Union, cast
 
 import numpy as np  # pylint: disable=unused-import
 import pandas as pd
 import sympy as sp
 from pyspark.sql import functions as sf
 from pyspark.sql.session import SparkSession
 from typeguard import typechecked
@@ -37,30 +37,26 @@
     @abstractmethod
     def validate(self, value: Any):
         """Raises an error if `value` not a valid distance.
 
         Args:
             value: A distance between two datasets under this metric.
         """
-        ...
 
     @abstractmethod
     def compare(self, value1: Any, value2: Any) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
-        ...
 
     @abstractmethod
     def supports_domain(self, domain: Domain) -> bool:
         """Return True if the metric is implemented for the passed domain."""
-        ...
 
     @abstractmethod
     def distance(self, value1: Any, value2: Any, domain: Domain) -> Any:
         """Returns the metric distance between two elements of a supported domain."""
-        ...
 
     def _validate_distance_arguments(
         self, value1: Any, value2: Any, domain: Domain
     ) -> None:
         """Raise an exception if the arguments to a distance method aren't valid."""
         if not self.supports_domain(domain):
             raise ValueError(f"{repr(self)} does not support domain {repr(domain)}.")
@@ -133,15 +129,14 @@
         """Return the metric distance between two elements of a supported domain.
 
         Args:
             value1: An element of the domain.
             value2: An element of the domain.
             domain: A domain compatible with the metric.
         """
-        ...
 
 
 class AbsoluteDifference(ExactNumberMetric):
     """The absolute value of the difference of two values.
 
     Example:
         >>> AbsoluteDifference().distance(
@@ -167,15 +162,15 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid value for metric AbsoluteDifference: {e}")
+            raise ValueError(f"Invalid value for metric AbsoluteDifference: {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
@@ -273,15 +268,17 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid value for metric SymmetricDifference: {e}")
+            raise ValueError(
+                f"Invalid value for metric SymmetricDifference: {e}"
+            ) from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
@@ -397,15 +394,15 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=False,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid value for metric HammingDistance: {e}")
+            raise ValueError(f"Invalid value for metric HammingDistance: {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
 
@@ -593,15 +590,14 @@
     @abstractmethod
     def _aggregate(self, distances: Iterable[ExactNumber]) -> ExactNumber:
         """Aggregate the component distances.
 
         Args:
             distances: The list of distances to aggregate.
         """
-        ...
 
 
 class SumOf(AggregationMetric):
     """Distances resulting from summing distances of its components.
 
     These components may be elements of a series, groups of a grouped dataframe, or
     elements of a list. This metric is parameterized by an `inner_metric` that is used
@@ -661,15 +657,15 @@
 
         Args:
             value: A distance between two datasets under this metric.
         """
         try:
             self.inner_metric.validate(value)
         except ValueError as e:
-            raise ValueError(f"Invalid metric value for SumOf metric: {e}")
+            raise ValueError(f"Invalid metric value for SumOf metric: {e}") from e
 
     def _aggregate(self, distances: Iterable[ExactNumber]) -> ExactNumber:
         """Aggregate the component distances.
 
         Args:
             distances: The list of distances to aggregate.
         """
@@ -734,24 +730,24 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid value for metric RootSumOfSquared: {e}")
+            raise ValueError(f"Invalid value for metric RootSumOfSquared: {e}") from e
 
     def _aggregate(self, distances: Iterable[ExactNumber]) -> ExactNumber:
         """Aggregate the component distances.
 
         Args:
             distances: The list of distances to aggregate.
         """
         return ExactNumber(
-            sp.sqrt(sum((d ** 2 for d in distances), ExactNumber(0)).expr)
+            sp.sqrt(sum((d**2 for d in distances), ExactNumber(0)).expr)
         )
 
 
 class OnColumn(ExactNumberMetric):
     """The value of a metric applied to a single column treated as a vector.
 
     Example:
@@ -810,15 +806,17 @@
 
         Args:
             value: A distance between two datasets under this metric.
         """
         try:
             self.metric.validate(value)
         except ValueError as e:
-            raise ValueError(f"Invalid value for OnColumn metric on {self.column}: {e}")
+            raise ValueError(
+                f"Invalid value for OnColumn metric on {self.column}: {e}"
+            ) from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         return self.metric.compare(value1, value2)
 
     def supports_domain(self, domain: Domain) -> bool:
         """Return True if the metric is implemented for the passed domain.
@@ -922,15 +920,15 @@
             raise ValueError(
                 f"Expecting a tuple of length {len(self._on_columns)}. Not {value}"
             )
         for column_value, on_column in zip(value, self.on_columns):
             try:
                 on_column.validate(column_value)
             except ValueError as e:
-                raise ValueError(f"Invalid value for OnColumns metric: {e}")
+                raise ValueError(f"Invalid value for OnColumns metric: {e}") from e
 
     def compare(
         self, value1: Tuple[ExactNumberInput, ...], value2: Tuple[ExactNumberInput, ...]
     ) -> bool:
         """Returns True if `value1` is less than or equal to `value2`.
 
         Args:
@@ -1060,15 +1058,15 @@
 
         Args:
             value: A distance between two datasets under this metric.
         """
         try:
             self.inner_metric.validate(value)
         except ValueError as e:
-            raise ValueError(f"Invalid value for IfGroupedBy metric: {e}")
+            raise ValueError(f"Invalid value for IfGroupedBy metric: {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`.
 
         Args:
             value1: A distance between two datasets under this metric.
             value2: A distance between two datasets under this metric.
@@ -1168,21 +1166,21 @@
         >>> value1 = {"x": np.int64(1), "y": df1}
         >>> value2 = {"x": np.int64(10), "y": df2}
         >>> metric.distance(value1, value2, domain)
         {'x': 9, 'y': 3}
     """
 
     @typechecked
-    def __init__(self, key_to_metric: Dict[Any, Metric]):
+    def __init__(self, key_to_metric: Mapping[Any, Metric]):
         """Constructor.
 
         Args:
             key_to_metric: Mapping from dictionary key to metric.
         """
-        self._key_to_metric = key_to_metric.copy()
+        self._key_to_metric: Dict[Any, Metric] = dict(key_to_metric.items()).copy()
 
     @property
     def key_to_metric(self) -> Dict[Any, Metric]:
         """Returns mapping from keys to metrics."""
         return self._key_to_metric.copy()
 
     def validate(self, value: Dict[Any, Any]):
@@ -1202,15 +1200,15 @@
                 f"Invalid DictMetric value: Expected keys: {set(self._key_to_metric)}"
                 f" not: {set(value)}"
             )
         for key, metric_value in value.items():
             try:
                 self._key_to_metric[key].validate(metric_value)
             except ValueError as e:
-                raise ValueError(f"Invalid value for DictMetric: {e}")
+                raise ValueError(f"Invalid value for DictMetric: {e}") from e
 
     def compare(self, value1: Dict[Any, Any], value2: Dict[Any, Any]) -> bool:
         """Returns True if `value1` is less than or equal to `value2`.
 
         Args:
             value1: A distance between two datasets under this metric.
             value2: A distance between two datasets under this metric.
@@ -1389,15 +1387,15 @@
             validate_exact_number(
                 value=value,
                 allow_nonintegral=True,
                 minimum=0,
                 minimum_is_inclusive=True,
             )
         except ValueError as e:
-            raise ValueError(f"Invalid value for metric AbsoluteDifference: {e}")
+            raise ValueError(f"Invalid value for metric AbsoluteDifference: {e}") from e
 
     def compare(self, value1: ExactNumberInput, value2: ExactNumberInput) -> bool:
         """Returns True if `value1` is less than or equal to `value2`."""
         self.validate(value1)
         self.validate(value2)
         return ExactNumber(value1) <= ExactNumber(value2)
```

### Comparing `tmlt_core-0.8.3/tmlt/core/random/continuous_gaussian.py` & `tmlt_core-0.9.0/tmlt/core/random/continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/random/discrete_gaussian.py` & `tmlt_core-0.9.0/tmlt/core/random/discrete_gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 @runtime_checkable
 class SupportsRandRange(Protocol):
     """Protocol class defining randrange."""
 
     def randrange(self, high: int) -> int:
         """Returns an integer sampled uniformly from [0, high)."""
-        ...
 
 
 def _sample_uniform(m: int, rng: SupportsRandRange) -> int:
     """Returns an integer sampled uniformly from [0, m).
 
     Args:
         m: Upper bound (exclusive) for sampling.
@@ -175,15 +174,15 @@
         else:
             b = c
     return a
 
 
 @typechecked
 def sample_dgauss(
-    sigma_squared: Union[float, Fraction, int], rng: SupportsRandRange = None
+    sigma_squared: Union[float, Fraction, int], rng: Optional[SupportsRandRange] = None
 ) -> int:
     r"""Returns a sample from a discrete Gaussian distribution.
 
     In particular, this returns a sample from discrete Gaussian
         :math:`\mathcal{N}_{\mathbb{Z}}(sigma\_squared)`
 
     Args:
```

### Comparing `tmlt_core-0.8.3/tmlt/core/random/inverse_cdf.py` & `tmlt_core-0.9.0/tmlt/core/random/inverse_cdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for inverse transform sampling."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 from typing import Callable
 
-import tmlt.core.utils.arb as arb
 from tmlt.core.random.rng import prng
+from tmlt.core.utils import arb
 
 
 def construct_inverse_sampler(
     inverse_cdf: Callable[[arb.Arb, int], arb.Arb], step_size: int = 63
 ) -> Callable[[], float]:
     """Returns a sampler for the distribution corresponding to `inverse_cdf`.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/random/laplace.py` & `tmlt_core-0.9.0/tmlt/core/random/laplace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for sampling from a Laplace distribution."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 import math
 
-import tmlt.core.utils.arb as arb
 from tmlt.core.random.inverse_cdf import construct_inverse_sampler
+from tmlt.core.utils import arb
 
 
 def laplace_inverse_cdf(u: float, b: float, p: arb.Arb, prec: int) -> arb.Arb:
     """Returns inverse CDF for Lap(u,b) at p.
 
     Args:
         u: The mean of the distribution. Must be finite and non-nan.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/random/rng.py` & `tmlt_core-0.9.0/tmlt/core/random/rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/random/uniform.py` & `tmlt_core-0.9.0/tmlt/core/random/uniform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for sampling uniformly from an interval."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-import tmlt.core.utils.arb as arb
 from tmlt.core.random.inverse_cdf import construct_inverse_sampler
+from tmlt.core.utils import arb
 
 
 def uniform_inverse_cdf(l: float, u: float, p: arb.Arb, prec: int) -> arb.Arb:
     """Returns the value of inverse CDF of the uniform distribution from `l` to `u`.
 
     Args:
         l: Lower bound for the uniform distribution.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/base.py` & `tmlt_core-0.9.0/tmlt/core/transformations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,8 +117,7 @@
         from tmlt.core.transformations.chaining import ChainTT
 
         return ChainTT(transformation1=self, transformation2=other)
 
     @abstractmethod
     def __call__(self, data: Any) -> Any:
         """Perform transformation."""
-        ...
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/chaining.py` & `tmlt_core-0.9.0/tmlt/core/transformations/chaining.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             d_mid = self.transformation1.stability_function(d_in)
         except NotImplementedError as e:
             if self._hint is None:
                 raise ValueError(
                     "A hint is needed to check this privacy relation, because the "
                     "stability_relation of self.transformation1 raised a "
                     f"NotImplementedError: {e}"
-                )
+                ) from e
             d_mid = self._hint(d_in, d_out)
         return self.transformation1.stability_relation(
             d_in, d_mid
         ) and self.transformation2.stability_relation(d_mid, d_out)
 
     @property
     def transformation1(self) -> Transformation:
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/converters.py` & `tmlt_core-0.9.0/tmlt/core/transformations/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         Args:
             d_in: Distance between inputs under input_metric.
         """
         self.input_metric.validate(d_in)
         d_in = ExactNumber(d_in)
         if self._is_l2:
-            return d_in ** 2
+            return d_in**2
         return d_in
 
     def __call__(self, sdf: DataFrame) -> DataFrame:
         """Returns DataFrame unchanged."""
         return sdf
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/dictionary.py` & `tmlt_core-0.9.0/tmlt/core/transformations/dictionary.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/identity.py` & `tmlt_core-0.9.0/tmlt/core/transformations/identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/add_remove_keys.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/add_remove_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,27 +211,24 @@
                 transformation.output_metric.inner_metric, SymmetricDifference
             )
         ):
             raise ValueError(
                 "Transformation's output metric must be "
                 "IfGroupedBy(column, SymmetricDifference())"
             )
-        column = transformation.input_metric.column
-        if column != transformation.output_metric.column:
+        input_column = transformation.input_metric.column
+        if input_metric.df_to_key_column[key] != input_column:
             raise ValueError(
-                "Transformation's input and output metric must group by the same column"
-            )
-        if input_metric.df_to_key_column[key] != column:
-            raise ValueError(
-                f"Transformation's input metric grouping column, {column}, does not"
-                " match the dataframe's key column,"
+                f"Transformation's input metric grouping column, {input_column}, does"
+                " not match the dataframe's key column,"
                 f" {input_metric.df_to_key_column[key]}."
             )
+        output_column = transformation.output_metric.column
         output_metric = AddRemoveKeys(
-            {**input_metric.df_to_key_column, new_key: column}
+            {**input_metric.df_to_key_column, new_key: output_column}
         )
         output_domain = DictDomain(
             {**input_domain.key_to_domain, new_key: transformation.output_domain}
         )
         self._transformation = transformation
         self._key = key
         self._new_key = new_key
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/agg.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/agg.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Optional, Union, cast, overload
 
 import numpy as np
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
-import tmlt.core.transformations.spark_transformations.nan as nan
 from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
 )
@@ -24,14 +23,15 @@
     HammingDistance,
     OnColumn,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.spark_transformations import nan
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
 from tmlt.core.utils.grouped_dataframe import GroupedDataFrame
 
 
 class Count(Transformation):
     r"""Counts the number of records in a spark DataFrame.
 
@@ -721,17 +721,17 @@
                 raise ValueError("Clipping bounds must be integral")
         if not self._lower.is_finite or not self._upper.is_finite:
             raise ValueError("Clipping bounds must be finite")
         if self._lower > self._upper:
             raise ValueError(
                 "Lower clipping bound is larger than upper clipping bound."
             )
-        if self._upper > 2 ** 970:
+        if self._upper > 2**970:
             raise ValueError("Upper clipping bound should be at most 2^970.")
-        if self._lower < -(2 ** 970):
+        if self._lower < -(2**970):
             raise ValueError("Lower clipping bound should be at least -2^970.")
 
         self._measure_column = measure_column
         output_domain = output_domain = (
             NumpyFloatDomain() if measure_column_nonintegral else NumpyIntegerDomain()
         )
         super().__init__(
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/filter.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
                 )
             if metric.column not in domain.schema:
                 raise ValueError(
                     f"Invalid IfGroupedBy metric: {metric.column} not in domain."
                 )
         try:
             test_df.filter(filter_expr)
-        except:
-            raise ValueError(f"Invalid filter_expr: {filter_expr}.")
+        except Exception as e:
+            raise ValueError(f"Invalid filter_expr: {filter_expr}.") from e
         super().__init__(
             input_domain=domain,
             input_metric=metric,
             output_domain=domain,
             output_metric=metric,
         )
         self._filter_expr = filter_expr
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/groupby.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
     if not column_domains:
         return SparkSession.builder.getOrCreate().createDataFrame([], StructType())
     full_domain_size = reduce(lambda acc, x: acc * len(x), column_domains.values(), 1)
 
     domain_spark_types = {
         column: _spark_type(values) for column, values in column_domains.items()
     }
-    if full_domain_size <= 10 ** 6:
+    if full_domain_size <= 10**6:
         # Perform in-memory crossjoin using itertools if fewer than 1m rows
         return spark.createDataFrame(
             spark.sparkContext.parallelize(
                 itertools.product(*column_domains.values()),
                 numSlices=2 + full_domain_size // 10000,
             ),
             schema=StructType(
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/id.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/join.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/join.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Transformations for joining Spark DataFrames."""
 # TODO(#1320): Add links to privacy and stability tutorial
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-from dataclasses import replace
 from enum import Enum
-from functools import reduce
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
@@ -24,14 +22,15 @@
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
+from tmlt.core.utils.join import domain_after_join, join, natural_join_columns
 from tmlt.core.utils.truncation import drop_large_groups, truncate_large_groups
 
 
 class PublicJoin(Transformation):
     """Join a Spark DataFrame with a public Pandas DataFrame.
 
     Examples:
@@ -268,71 +267,51 @@
             ):
                 raise ValueError(
                     "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
                     "SumOf(SymmetricDifference()), or "
                     "RootSumOfSquared(SymmetricDifference())"
                 )
 
-        common_cols = set(input_domain.schema) & set(public_df.columns)
-        if not join_cols:
-            if not common_cols:
-                raise ValueError("Can not join: No common columns.")
-            join_cols = sorted(common_cols, key=list(input_domain.schema).index)
-        else:
-            join_cols = join_cols.copy()
-
-        if not set(join_cols) <= set(common_cols):
-            raise ValueError("Join columns must be common to both DataFrames.")
-
         if public_df_domain:
             if public_df.schema != public_df_domain.spark_schema:
                 raise ValueError(
                     "public_df's Spark schema does not match public_df_domain"
                 )
             for col, descriptor in public_df_domain.schema.items():
                 if isinstance(descriptor, SparkFloatColumnDescriptor):
                     if not descriptor.allow_inf:
                         public_df = public_df.filter(
                             ~public_df[col].isin([float("inf"), -float("inf")])
                         )
                     if not descriptor.allow_nan:
                         public_df = public_df.filter(~sf.isnan(public_df[col]))
-
         else:
             public_df_domain = SparkDataFrameDomain.from_spark_schema(public_df.schema)
-        for col in join_cols:
-            if input_domain[col].data_type != public_df_domain[col].data_type:
-                raise ValueError(
-                    "Join columns must have identical types on both "
-                    f"DataFrames. {input_domain[col].data_type} and "
-                    f"{public_df_domain[col].data_type} are incompatible."
-                )
-
-        join_cols_schema = {col: input_domain[col] for col in join_cols}
-        overlapping_cols = common_cols - set(join_cols)
-        left_schema = {
-            col + ("_left" if col in overlapping_cols else ""): input_domain[col]
-            for col in input_domain.schema
-            if col not in join_cols
-        }
-        right_schema = {
-            col + ("_right" if col in overlapping_cols else ""): public_df_domain[col]
-            for col in public_df_domain.schema
-            if col not in join_cols
-        }
-        output_domain = SparkDataFrameDomain(
-            {**join_cols_schema, **left_schema, **right_schema}
+        if join_cols is None:
+            join_cols = natural_join_columns(
+                left_columns=list(input_domain.schema),
+                right_columns=list(public_df_domain.schema),
+            )
+        output_domain = domain_after_join(
+            left_domain=input_domain,
+            right_domain=public_df_domain,
+            on=join_cols,
+            how="inner",
+            nulls_are_equal=join_on_nulls,
         )
-        if isinstance(metric, IfGroupedBy) and metric.column in overlapping_cols:
+        if (
+            isinstance(metric, IfGroupedBy)
+            and metric.column not in join_cols
+            and metric.column in input_domain.schema
+            and metric.column in public_df_domain.schema
+        ):
             raise ValueError(
-                f"IfGroupedBy column {metric.column} is an overlapping"
+                f"IfGroupedBy column '{metric.column}' is an overlapping"
                 " column but not a join key."
             )
-        for col in overlapping_cols:
-            public_df = public_df.withColumnRenamed(col, f"{col}_right")
 
         public_df_join_columns = public_df.select(*join_cols)
         if not join_on_nulls:
             public_df_join_columns = public_df_join_columns.dropna()
         if (
             isinstance(metric, IfGroupedBy)
             and metric.inner_metric == SymmetricDifference()
@@ -351,18 +330,28 @@
         super().__init__(
             input_domain=input_domain,
             input_metric=metric,
             output_domain=output_domain,
             output_metric=metric,
         )
         self._join_on_nulls = join_on_nulls
-        self._overlapping_cols = overlapping_cols
         self._public_df = public_df
         self._public_df = public_df
-        self._join_cols = join_cols
+        self._join_cols = (
+            join_cols.copy()
+            if join_cols is not None
+            else natural_join_columns(
+                list(input_domain.schema), list(public_df_domain.schema)
+            )
+        )
+
+    @property
+    def join_on_nulls(self) -> bool:
+        """Returns whether nulls are considered equal in join."""
+        return self._join_on_nulls
 
     @property
     def join_cols(self) -> List[str]:
         """Returns list of columns to be joined on."""
         return self._join_cols.copy()
 
     @property
@@ -393,34 +382,21 @@
 
     def __call__(self, sdf: DataFrame) -> DataFrame:
         """Perform public join.
 
         Args:
             sdf: Private DataFrame to join public DataFrame with.
         """
-        output_columns_order = list(
-            (cast(SparkDataFrameDomain, self.output_domain)).schema
-        )
-        for col in self._overlapping_cols:
-            sdf = sdf.withColumnRenamed(col, f"{col}_left")
-        if not self._join_on_nulls:
-            return sdf.join(self.public_df, on=self.join_cols, how="inner").select(
-                output_columns_order
-            )
-        joined_df = sdf.join(
-            self.public_df,
-            on=reduce(
-                lambda exp, col: exp & sdf[col].eqNullSafe(self.public_df[col]),
-                self.join_cols,
-                sf.lit(True),  # pylint: disable=no-member
-            ),
+        return join(
+            left=sdf,
+            right=self.public_df,
+            how="inner",
+            on=self.join_cols,
+            nulls_are_equal=self.join_on_nulls,
         )
-        for col in self.join_cols:
-            joined_df = joined_df.drop(self.public_df[col])
-        return joined_df.select(output_columns_order)
 
 
 class TruncationStrategy(Enum):
     """Enumerating truncation strategies for PrivateJoin.
 
     See :meth:`~.PrivateJoin.stability_function` for the stability of each strategy.
     """
@@ -511,16 +487,16 @@
         ...     "left": left_spark_dataframe,
         ...     "right": right_spark_dataframe
         ... }
         >>> # Apply transformation to data
         >>> joined_dataframe = private_join(input_dictionary)
         >>> print_sdf(joined_dataframe)
             B   A  X   C
-        0  b1  a1  5  c1
-        1  b1  a2 -5  c1
+        0  b1  a1  2  c1
+        1  b1  a1  3  c1
         2  b2  a1 -1  c2
         3  b2  a1 -1  c3
         4  b2  a1  4  c2
         5  b2  a1  4  c3
 
     .. Note:
         This join works similarly to :class:`~.PublicJoin`, see it for more examples.
@@ -608,15 +584,15 @@
                 truncating the left DataFrame.
             right_truncation_strategy:  :class:`~.TruncationStrategy` to use for
                 truncating the right DataFrame.
             left_truncation_threshold: The maximum number of rows to allow for each
                 combination of values of `join_cols` in the left DataFrame.
             right_truncation_threshold: The maximum number of rows to allow for each
                 combination of values of `join_cols` in the right DataFrame.
-            join_cols: Columns to perform join on. If None, or empty, natural join is
+            join_cols: Columns to perform join on. If None, a natural join is
                 computed.
             join_on_nulls: If True, null values on corresponding join columns of
                 both dataframes will be considered to be equal.
         """
         if input_domain.length != 2:
             raise ValueError("Input domain must be a DictDomain with 2 keys.")
         if left_key == right_key:
@@ -626,57 +602,22 @@
         if right_key not in input_domain.key_to_domain:
             raise ValueError(f"Invalid key: Key '{right_key}' not in input domain.")
 
         left_domain, right_domain = input_domain[left_key], input_domain[right_key]
         if not isinstance(left_domain, SparkDataFrameDomain) or not isinstance(
             right_domain, SparkDataFrameDomain
         ):
-            raise ValueError("Input domain must be SparkDataFrameDomin for both keys.")
+            raise ValueError("Input domain must be SparkDataFrameDomain for both keys.")
 
-        common_cols = set(left_domain.schema) & set(right_domain.schema)
-        if not join_cols:
-            if not common_cols:
-                raise ValueError("Can not join: No common columns.")
-            join_cols = sorted(common_cols, key=list(left_domain.schema).index)
-        else:
-            join_cols = join_cols.copy()
-
-        join_cols_schema = {}
-        for key in join_cols:
-            if left_domain[key] != right_domain[key]:
-                raise ValueError(
-                    "Left and right DataFrame domains have mismatching types on"
-                    f" join column {key}."
-                )
-            if join_on_nulls:
-                join_cols_schema[key] = left_domain[key]
-            else:
-                join_cols_schema[key] = replace(left_domain[key], allow_null=False)
-        overlapping_cols = common_cols - set(join_cols)
-        all_input_cols = set(left_domain.schema) | set(right_domain.schema)
-        for col in overlapping_cols:
-            if f"{col}_left" in all_input_cols or f"{col}_right" in all_input_cols:
-                raise ValueError(
-                    f"Join would rename overlapping column '{col}' to an existing"
-                    " column name."
-                )
-
-        left_schema = {
-            col + ("_left" if col in overlapping_cols else ""): left_domain[col]
-            for col in left_domain.schema
-            if col not in join_cols
-        }
-        right_schema = {
-            col + ("_right" if col in overlapping_cols else ""): right_domain[col]
-            for col in right_domain.schema
-            if col not in join_cols
-        }
-
-        output_domain = SparkDataFrameDomain(
-            {**join_cols_schema, **left_schema, **right_schema}
+        output_domain = domain_after_join(
+            left_domain=left_domain,
+            right_domain=right_domain,
+            on=join_cols,
+            how="inner",
+            nulls_are_equal=join_on_nulls,
         )
 
         super().__init__(
             input_domain=input_domain,
             input_metric=DictMetric(
                 {left_key: SymmetricDifference(), right_key: SymmetricDifference()}
             ),
@@ -685,16 +626,21 @@
         )
         self._left_key = left_key
         self._right_key = right_key
         self._left_truncation_strategy = left_truncation_strategy
         self._right_truncation_strategy = right_truncation_strategy
         self._left_truncation_threshold = left_truncation_threshold
         self._right_truncation_threshold = right_truncation_threshold
-        self._join_cols = join_cols
-        self._overlapping_cols = set(common_cols) - set(join_cols)
+        self._join_cols = (
+            join_cols.copy()
+            if join_cols is not None
+            else natural_join_columns(
+                list(left_domain.schema), list(right_domain.schema)
+            )
+        )
         self._join_on_nulls = join_on_nulls
 
     @property
     def left_key(self) -> Any:
         """Returns key to left DataFrame."""
         return self._left_key
 
@@ -777,32 +723,21 @@
             self.left_truncation_threshold,
         )
         right = truncate(
             dfs[self.right_key],
             self.right_truncation_strategy,
             self.right_truncation_threshold,
         )
-
-        for col in self._overlapping_cols:
-            left = left.withColumnRenamed(col, f"{col}_left")
-            right = right.withColumnRenamed(col, f"{col}_right")
-
-        if not self._join_on_nulls:
-            right = right.dropna()
-            return left.join(right, on=self.join_cols, how="inner")
-
-        joined_df = left.join(
-            right, on=[left[col].eqNullSafe(right[col]) for col in self.join_cols]
+        return join(
+            left=left,
+            right=right,
+            how="inner",
+            on=self.join_cols,
+            nulls_are_equal=self.join_on_nulls,
         )
-        for col in self.join_cols:
-            joined_df = joined_df.drop(right[col])
-        output_columns_order = list(
-            (cast(SparkDataFrameDomain, self.output_domain)).schema
-        )
-        return joined_df.select(output_columns_order)
 
 
 class PrivateJoinOnKey(Transformation):
     r"""Join two private SparkDataFrames including a key column.
 
     Example:
         ..
@@ -968,18 +903,18 @@
         new_key: Any,
         join_cols: Optional[List[str]] = None,
         join_on_nulls: bool = False,
     ):
         """Constructor.
 
         Args:
-            input_domain: Domain of the input dictionaries. Must contain `left_key` and `right_key`,
-                but may also contain other keys.
-            input_metric: AddRemoveKeys metric for the input dictionaries. The left and right dataframes
-                must use the same key column.
+            input_domain: Domain of the input dictionaries. Must contain `left_key` and
+                `right_key`, but may also contain other keys.
+            input_metric: AddRemoveKeys metric for the input dictionaries. The left and
+                right dataframes must use the same key column.
             left_key: Key for the left DataFrame.
             right_key: Key for the right DataFrame.
             new_key: Key for the output DataFrame.
             join_cols: Columns to perform join on. If None, or empty, natural join is
                 computed.
             join_on_nulls: If True, null values on corresponding join columns of
                 both dataframes will be considered to be equal.
@@ -988,65 +923,33 @@
             raise ValueError("Left and right keys must be distinct.")
         if left_key not in input_domain.key_to_domain:
             raise ValueError(f"Invalid key: Key '{left_key}' not in input domain.")
         if right_key not in input_domain.key_to_domain:
             raise ValueError(f"Invalid key: Key '{right_key}' not in input domain.")
 
         left_domain, right_domain = input_domain[left_key], input_domain[right_key]
-        if not isinstance(left_domain, SparkDataFrameDomain) or not isinstance(
-            right_domain, SparkDataFrameDomain
-        ):
-            raise ValueError("Input domain must be SparkDataFrameDomin for both keys.")
-
-        common_cols = set(left_domain.schema) & set(right_domain.schema)
-        if not join_cols:
-            if not common_cols:
-                raise ValueError("Can not join: No common columns.")
-            join_cols = sorted(common_cols, key=list(left_domain.schema).index)
-        else:
-            join_cols = join_cols.copy()
 
-        join_cols_schema = {}
-        for key in join_cols:
-            if left_domain[key] != right_domain[key]:
-                raise ValueError(
-                    "Left and right DataFrame domains have mismatching types on"
-                    f" join column {key}."
-                )
-            if join_on_nulls:
-                join_cols_schema[key] = left_domain[key]
-            else:
-                join_cols_schema[key] = replace(left_domain[key], allow_null=False)
-        overlapping_cols = common_cols - set(join_cols)
-        all_input_cols = set(left_domain.schema) | set(right_domain.schema)
-        for col in overlapping_cols:
-            if f"{col}_left" in all_input_cols or f"{col}_right" in all_input_cols:
-                raise ValueError(
-                    f"Join would rename overlapping column '{col}' to an existing"
-                    " column name."
-                )
-
-        left_schema = {
-            col + ("_left" if col in overlapping_cols else ""): left_domain[col]
-            for col in left_domain.schema
-            if col not in join_cols
-        }
-        right_schema = {
-            col + ("_right" if col in overlapping_cols else ""): right_domain[col]
-            for col in right_domain.schema
-            if col not in join_cols
-        }
-
-        new_df_domain = SparkDataFrameDomain(
-            {**join_cols_schema, **left_schema, **right_schema}
-        )
         output_domain = DictDomain(
-            {**input_domain.key_to_domain, new_key: new_df_domain}
+            {
+                **input_domain.key_to_domain,
+                new_key: domain_after_join(
+                    left_domain=left_domain,
+                    right_domain=right_domain,
+                    on=join_cols,
+                    how="inner",
+                    nulls_are_equal=join_on_nulls,
+                ),
+            }
         )
-
+        assert isinstance(left_domain, SparkDataFrameDomain)
+        assert isinstance(right_domain, SparkDataFrameDomain)
+        if join_cols is None:
+            join_cols = natural_join_columns(
+                list(left_domain.schema), list(right_domain.schema)
+            )
         if left_key not in input_metric.df_to_key_column:
             raise ValueError(f"Invalid key: Key '{left_key}' not in input metric.")
         if right_key not in input_metric.df_to_key_column:
             raise ValueError(f"Invalid key: Key '{right_key}' not in input metric.")
         if (
             input_metric.df_to_key_column[left_key]
             != input_metric.df_to_key_column[right_key]
@@ -1065,16 +968,21 @@
             input_metric=input_metric,
             output_domain=output_domain,
             output_metric=output_metric,
         )
         self._left_key = left_key
         self._right_key = right_key
         self._new_key = new_key
-        self._join_cols = join_cols
-        self._overlapping_cols = overlapping_cols
+        self._join_cols = (
+            join_cols.copy()
+            if join_cols is not None
+            else natural_join_columns(
+                list(left_domain.schema), list(right_domain.schema)
+            )
+        )
         self._join_on_nulls = join_on_nulls
 
     @property
     def left_key(self) -> Any:
         """Returns key to left DataFrame."""
         return self._left_key
 
@@ -1110,31 +1018,16 @@
         self.input_metric.validate(d_in)
         return ExactNumber(d_in)
 
     def __call__(self, dfs: Dict[Any, DataFrame]):
         """Perform join."""
         left = dfs[self.left_key]
         right = dfs[self.right_key]
-        for col in self._overlapping_cols:
-            left = left.withColumnRenamed(col, f"{col}_left")
-            right = right.withColumnRenamed(col, f"{col}_right")
-
-        if not self._join_on_nulls:
-            right = right.dropna()
-            joined_df = left.join(right, on=self.join_cols, how="inner")
-        else:
-            joined_df = left.join(
-                right, on=[left[col].eqNullSafe(right[col]) for col in self.join_cols]
-            )
-            for col in self.join_cols:
-                joined_df = joined_df.drop(right[col])
-        output_columns_order = list(
-            (
-                cast(
-                    SparkDataFrameDomain,
-                    cast(DictDomain, self.output_domain).key_to_domain[self.new_key],
-                )
-            ).schema
-        )
         new_dfs = dfs.copy()
-        new_dfs[self.new_key] = joined_df.select(output_columns_order)
+        new_dfs[self.new_key] = join(
+            left,
+            right,
+            on=self.join_cols,
+            how="inner",
+            nulls_are_equal=self.join_on_nulls,
+        )
         return new_dfs
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/map.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
 
 
 class RowToRowTransformation(Transformation):
     """Transforms a single row into a different row using a user defined function.
 
+    .. note::
+        The transformation function must not contain any objects that
+        directly or indirectly reference Spark DataFrames or Spark contexts.
+        If the function does contain an object that directly or indirectly
+        references a Spark DataFrame or a Spark context, an
+        error will occur when the RowToRowTransformation is called on a row.
+
     Examples:
         ..
             >>> from tmlt.core.domains.spark_domains import (
             ...     SparkRowDomain,
             ...     SparkStringColumnDescriptor,
             ... )
             >>> spark_row = Row(A='a1', B='b1')
@@ -185,14 +192,21 @@
             return Row(**augmented_row_dict)
         return Row(**mapped_row_dict)
 
 
 class RowToRowsTransformation(Transformation):
     """Transforms a single row into multiple rows using a user defined function.
 
+    .. note::
+        The transformation function must not contain any objects that
+        directly or indirectly reference Spark DataFrames or Spark contexts.
+        If the function does contain an object that directly or indirectly
+        references a Spark DataFrame or a Spark context, an
+        error will occur when the RowToRowTransformation is called on a row
+
     Examples:
         ..
             >>> from tmlt.core.domains.spark_domains import (
             ...     SparkRowDomain,
             ...     SparkIntegerColumnDescriptor,
             ...     SparkStringColumnDescriptor,
             ... )
@@ -351,28 +365,35 @@
 
     def __call__(self, row: Row) -> List[Row]:
         """Map row."""
         mapped = self._trusted_f(row)
         assert all(isinstance(r, (Row, dict)) for r in mapped)
         mapped_rows = [r if isinstance(r, Row) else Row(**r) for r in mapped]
         if self._augment:
-            augmented_rows: List[Row] = list()
+            augmented_rows: List[Row] = []
             for r in mapped_rows:
-                # NOTE: .asDict() doesn't work with emtpy row.
+                # NOTE: .asDict() doesn't work with empty row.
                 r_dict = r.asDict() if len(r) > 0 else {}
                 augmented_row_dict = {**row.asDict(), **r_dict}
                 augmented_row_dict.update(row.asDict())
                 augmented_rows.append(Row(**augmented_row_dict))
             return augmented_rows
         return mapped_rows
 
 
 class FlatMap(Transformation):
     """Applies a :class:`~.RowToRowsTransformation` to each row and flattens the result.
 
+    .. note::
+        The transformation function must not contain any objects that
+        directly or indirectly reference Spark DataFrames or Spark contexts.
+        If the function does contain an object that directly or indirectly
+        references a Spark DataFrame or a Spark context, an
+        error will occur when the RowToRowTransformation is called on a row
+
     Example:
         ..
             >>> import pandas as pd
             >>> from tmlt.core.domains.spark_domains import (
             ...     SparkRowDomain,
             ...     SparkStringColumnDescriptor,
             ... )
@@ -591,14 +612,21 @@
 
     The requirements are that
 
     1. The `row_transformer` creates a single column that is augmented to the input
     2. For each input row, the values in the created column are distinct (This is
        enforced by the implementation).
 
+    .. note::
+        The transformation function must not contain any objects that
+        directly or indirectly reference Spark DataFrames or Spark contexts.
+        If the function does contain an object that directly or indirectly
+        references a Spark DataFrame or a Spark context, an
+        error will occur when the RowToRowTransformation is called on a row
+
     Example:
         ..
             >>> import pandas as pd
             >>> from tmlt.core.domains.spark_domains import (
             ...     SparkRowDomain,
             ...     SparkIntegerColumnDescriptor,
             ...     SparkStringColumnDescriptor,
@@ -805,14 +833,21 @@
         mapped_sdf = spark.createDataFrame(mapped_rdd, self._output_domain.spark_schema)
         return mapped_sdf
 
 
 class Map(Transformation):
     """Applies a :class:`~.RowToRowTransformation` to each row in a Spark DataFrame.
 
+    .. note::
+        The transformation function must not contain any objects that
+        directly or indirectly reference Spark DataFrames or Spark contexts.
+        If the function does contain an object that directly or indirectly
+        references a Spark DataFrame or a Spark context, an
+        error will occur when the RowToRowTransformation is called on a row
+
     Example:
         ..
             >>> import pandas as pd
             >>> from tmlt.core.domains.spark_domains import (
             ...     SparkRowDomain,
             ...     SparkIntegerColumnDescriptor,
             ...     SparkStringColumnDescriptor,
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/nan.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/nan.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 raise ValueError(
                     f"Cannot drop +inf and -inf from {input_domain[column]}. Only float"
                     " columns can contain +inf or -inf."
                 )
 
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_inf=False)
+                column: replace(descriptor, allow_inf=False)  # type: ignore
                 if column in columns
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         super().__init__(
             input_domain=input_domain,
@@ -315,15 +315,15 @@
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Cannot drop NaNs from {input_domain[column]}. Only float columns"
                     " can contain NaNs."
                 )
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_nan=False)
+                column: replace(descriptor, allow_nan=False)  # type: ignore
                 if column in columns
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         super().__init__(
             input_domain=input_domain,
@@ -474,15 +474,15 @@
         if not set(columns) <= set(input_domain.schema):
             raise ValueError(
                 "One or more columns do not exist in the input domain"
                 f" {set(columns)-set(input_domain.schema)}"
             )
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_null=False)
+                column: replace(descriptor, allow_null=False)  # type: ignore
                 if column in columns
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         super().__init__(
             input_domain=input_domain,
@@ -639,21 +639,23 @@
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Column of type {input_domain[column]} cannot contain values of"
                     " infinity or -infinity."
                 )
             if not cast(SparkFloatColumnDescriptor, input_domain[column]).allow_inf:
                 warnings.warn(
-                    f"Column ({column}) already disallows infinite values. This"
-                    " transformation will have no effect on this column.",
+                    (
+                        f"Column ({column}) already disallows infinite values. This"
+                        " transformation will have no effect on this column."
+                    ),
                     RuntimeWarning,
                 )
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_inf=False)
+                column: replace(descriptor, allow_inf=False)  # type: ignore
                 if column in replace_map
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         for column, values in replace_map.items():
             for value in values:
@@ -816,21 +818,23 @@
         for column, value in replace_map.items():
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Column of type {input_domain[column]} can not contain NaNs."
                 )
             if not cast(SparkFloatColumnDescriptor, input_domain[column]).allow_nan:
                 warnings.warn(
-                    f"Column ({column}) already disallows NaNs. This transformation"
-                    " will have no effect on this column.",
+                    (
+                        f"Column ({column}) already disallows NaNs. This transformation"
+                        " will have no effect on this column."
+                    ),
                     RuntimeWarning,
                 )
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_nan=False)
+                column: replace(descriptor, allow_nan=False)  # type: ignore
                 if column in replace_map
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         for column, value in replace_map.items():
             if not output_domain[column].valid_py_value(value):
@@ -979,29 +983,31 @@
         if not set(replace_map) <= set(input_domain.schema):
             raise ValueError(
                 "One or more columns do not exist in the input domain"
                 f" {set(replace_map)-set(input_domain.schema)}"
             )
         output_domain = SparkDataFrameDomain(
             {
-                column: replace(descriptor, allow_null=False)
+                column: replace(descriptor, allow_null=False)  # type: ignore
                 if column in replace_map
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
             }
         )
         for column, value in replace_map.items():
             if not output_domain[column].valid_py_value(value):
                 raise ValueError(
                     f"Replacement value ({value}) is invalid for column ({column})"
                 )
             if not input_domain[column].allow_null:
                 warnings.warn(
-                    f"Column ({column}) already disallows nulls. This transformation"
-                    " will have no effect on this column.",
+                    (
+                        f"Column ({column}) already disallows nulls. This"
+                        " transformation will have no effect on this column."
+                    ),
                     RuntimeWarning,
                 )
         if isinstance(metric, IfGroupedBy):
             if metric.column in replace_map:
                 raise ValueError(
                     "Cannot replace values in the grouping column for IfGroupedBy."
                 )
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/partition.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Transformations for partitioning Spark DataFrames."""
 # TODO(#1320): Add links to privacy and stability tutorial
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Sequence, Tuple, Union
 
 from pyspark.sql import Column, DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import ListDomain
@@ -163,15 +163,15 @@
     @typechecked
     def __init__(
         self,
         input_domain: SparkDataFrameDomain,
         input_metric: Union[IfGroupedBy, SymmetricDifference],
         use_l2: bool,
         keys: List[str],
-        list_values: List[Tuple],
+        list_values: Sequence[Tuple],
     ):
         """Constructor.
 
         Args:
             input_domain: Domain of input DataFrames.
             input_metric: Distance metric for input DataFrames.
             use_l2: If True, use :class:`~.RootSumOfSquared` instead of :class:`~.SumOf`
@@ -214,15 +214,15 @@
         else:
             output_metric = (
                 RootSumOfSquared(SymmetricDifference())
                 if use_l2
                 else SumOf(SymmetricDifference())
             )
         self._partition_keys = keys.copy()
-        self._list_values = list_values.copy()
+        self._list_values = list(list_values).copy()
         super().__init__(
             input_domain, input_metric, output_metric, num_partitions=len(list_values)
         )
 
     @property
     def keys(self) -> List[str]:
         """Returns list of column names to partition on."""
```

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/persist.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/persist.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/rename.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/rename.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/select.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/select.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/transformations/spark_transformations/truncation.py` & `tmlt_core-0.9.0/tmlt/core/transformations/spark_transformations/truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/arb.py` & `tmlt_core-0.9.0/tmlt/core/utils/arb.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,15 +495,15 @@
 def _int_to_fmpz_t(val: int) -> "ctypes._PointerLike":
     """Returns pointer to a C arbitrary precision integer from a python integer.
 
     Args:
         val: Integer to convert.
     """
     fmpz_pointer = ctypes.pointer(ctypes.c_long())
-    s = "%x" % int(val)
+    s = "%x" % int(val)  # pylint: disable=consider-using-f-string
     val_c_string = ctypes.c_char_p(s.encode("ascii"))
     flintlib.fmpz_set_str(fmpz_pointer, val_c_string, 16)
     return fmpz_pointer
 
 
 def _fmpz_t_to_int(ptr: "ctypes._PointerLike") -> int:
     """Returns python integer from an fmpz_t."""
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/cleanup.py` & `tmlt_core-0.9.0/tmlt/core/utils/cleanup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 from typing import List
 
 from pyspark.sql import SparkSession
 
 from tmlt.core.utils.configuration import Config
 
 
-def _cleanup_temp():
+def _cleanup_temp() -> None:
     """Cleanup the temporary table."""
     spark = SparkSession.builder.getOrCreate()
     spark.sql(f"DROP DATABASE IF EXISTS `{Config.temp_db_name()}` CASCADE")
 
 
-def cleanup():
+def cleanup() -> None:
     """Cleanup Core's temporary table.
 
     If you call `spark.stop()`, you should call this function first.
     """
     _cleanup_temp()
 
 
-def remove_all_temp_tables():
+def remove_all_temp_tables() -> None:
     """Remove all temporary tables that Core has created.
 
     This will remove all temporary tables in the current Spark
     data warehouse.
     """
     spark = SparkSession.builder.getOrCreate()
     pattern = re.compile(r"tumult_temp_\d{8}_\d{6}_(\d|a-f)*")
     dbs_to_remove: List[str] = []
     for db in spark.catalog.listDatabases():
         if pattern.match(db.name):
             dbs_to_remove.append(db.name)
 
-    for db in dbs_to_remove:
-        spark.sql(f"DROP DATABASE `{db}` CASCADE")
+    for db_name in dbs_to_remove:
+        spark.sql(f"DROP DATABASE `{db_name}` CASCADE")
 
 
 atexit.register(_cleanup_temp)
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/configuration.py` & `tmlt_core-0.9.0/tmlt/core/utils/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,19 @@
 def _simple_java_version(long_version: str) -> Optional[int]:
     """Turn a long Java version (like 1.8.0_292) into an int (like 8)."""
     pattern = r"(\d+)\.(\d+).*"
     m = re.search(pattern, long_version)
     if m is None:
         # give up
         warnings.warn(
-            f"Unable to determine Java version from version string `{long_version}`."
-            " Tumult Core will assume you are running Java 11 or higher",
+            (
+                "Unable to determine Java version from version string"
+                f" `{long_version}`. Tumult Core will assume you are running Java 11 or"
+                " higher"
+            ),
             RuntimeWarning,
         )
         return None
     # Java versions 8 and earlier are 1.8, 1.7, etc
     if m.group(1) == "1":
         return int(m.group(2))
     return int(m.group(1))
@@ -64,24 +67,28 @@
         subprocess_env["PATH"] = new_path
     try:
         version = subprocess.check_output(
             ["java", "-version"], stderr=subprocess.STDOUT, env=subprocess_env
         )
     except FileNotFoundError:
         warnings.warn(
-            "Unable to locate Java executable to determine version, Tumult Core will "
-            "assume Java 11 or higher. This may indicate that Java is missing from "
-            "your environment.",
+            (
+                "Unable to locate Java executable to determine version, Tumult Core"
+                " will assume Java 11 or higher. This may indicate that Java is missing"
+                " from your environment."
+            ),
             RuntimeWarning,
         )
         return None
     except subprocess.CalledProcessError:
         warnings.warn(
-            "Error detecting Java version from executable, Tumult Core will "
-            "assume Java 11 or higher",
+            (
+                "Error detecting Java version from executable, Tumult Core will "
+                "assume Java 11 or higher"
+            ),
             RuntimeWarning,
         )
         return None
     # version is now a bytes() object, which ought to contain a substring
     # that looks like "1.2.345" (including the quotation marks)
     m = re.search(r'"(\d+)\.(\d+).*"', str(version))
     if m is None:
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/distributions.py` & `tmlt_core-0.9.0/tmlt/core/utils/distributions.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     See :cite:`Canonne0S20` for more information. The formula above is based on
     Definition 1.
 
     The implementation also referenced the paper's implementation, which can be found at
     https://github.com/IBM/discrete-gaussian-differential-privacy.
     """
     return np.exp(
-        -(k ** 2) / (2 * sigma_squared)
+        -(k**2) / (2 * sigma_squared)
     ) / _discrete_gaussian_normalizing_constant(sigma_squared)
 
 
 @overload
 def discrete_gaussian_cmf(k: int, sigma_squared: float) -> float:
     ...
 
@@ -271,23 +271,23 @@
     adjusted_p = p if p <= 0.5 else 1.0 - p
 
     unnormalized_cmf = adjusted_p * _discrete_gaussian_normalizing_constant(
         sigma_squared
     )
 
     def unnormalized_pmf(k):
-        return np.exp(-(k ** 2) / (2 * sigma_squared))
+        return np.exp(-(k**2) / (2 * sigma_squared))
 
     # _discrete_gaussian_normalizing_constant explains calculating the bound this way
-    lower_bound = min(-10000, -int(sigma_squared * 50))
+    lower_bound: float = min(-10000, -int(sigma_squared * 50))
 
     # if k < lower bound, cmf(k) returns pmf(k), so we can binary search for k.
     if unnormalized_pmf(lower_bound) > unnormalized_cmf:
-        hi = lower_bound
-        lo = lower_bound * 2
+        hi: float = lower_bound
+        lo: float = lower_bound * 2
         while unnormalized_pmf(lo) > unnormalized_cmf:
             hi = lo
             lo *= 2
         while hi != lo:
             mid = hi / 2 + lo / 2
             if unnormalized_pmf(mid) == unnormalized_cmf:
                 return mid if p <= 0.5 else -mid
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/exact_number.py` & `tmlt_core-0.9.0/tmlt/core/utils/exact_number.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,33 +160,33 @@
         return
     if isinstance(expr, (sp.Mul, sp.Add)):
         left_expr, right_expr = expr.as_two_terms()
         try:
             _verify_expr_is_an_exact_number(left_expr)
             _verify_expr_is_an_exact_number(right_expr)
         except ValueError as e:
-            raise ValueError(f"{expr} is invalid: {e}")
+            raise ValueError(f"{expr} is invalid: {e}") from e
         return
     if isinstance(expr, (sp.Pow, sp.exp)):
         try:
             _verify_expr_is_an_exact_number(expr.base)
         except ValueError as e:
-            raise ValueError(f"Base of {expr} is invalid: {e}")
+            raise ValueError(f"Base of {expr} is invalid: {e}") from e
         try:
             _verify_expr_is_an_exact_number(expr.exp)
         except ValueError as e:
-            raise ValueError(f"Exponent of {expr} is invalid: {e}")
+            raise ValueError(f"Exponent of {expr} is invalid: {e}") from e
         return
     if isinstance(expr, sp.log):
         if len(expr.args) != 1:
             raise ValueError(f"Logarithm {expr} has more than one term")
         try:
             _verify_expr_is_an_exact_number(expr.args[0])
         except ValueError as e:
-            raise ValueError(f"Invalid Logarithm {expr}: {e}")
+            raise ValueError(f"Invalid Logarithm {expr}: {e}") from e
         return
     if isinstance(expr, sp.Float):
         raise ValueError(f"{expr} is represented using floating point precision")
     raise ValueError(f"Invalid SymPy expression: {expr}")
 
 
 @typechecked
@@ -358,20 +358,20 @@
         """Returns difference of other and self."""
         other = ExactNumber(other)
         return ExactNumber(other.expr - self.expr)
 
     def __pow__(self, other: "ExactNumberInput") -> "ExactNumber":
         """Returns power obtained by raising self to other."""
         other = ExactNumber(other)
-        return ExactNumber(self.expr ** other.expr)
+        return ExactNumber(self.expr**other.expr)
 
     def __rpow__(self, other: "ExactNumberInput") -> "ExactNumber":
         """Returns power obtained by raising other to self."""
         other = ExactNumber(other)
-        return ExactNumber(other.expr ** self.expr)
+        return ExactNumber(other.expr**self.expr)
 
     def __eq__(self, other: Any) -> bool:
         """Returns True if other and self represent the same value."""
         try:
             other = ExactNumber(other)
         except ValueError:
             return False
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/grouped_dataframe.py` & `tmlt_core-0.9.0/tmlt/core/utils/grouped_dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, Callable, Dict, List
 
 import pandas as pd
 from pyspark.sql import Column, DataFrame, Row, SparkSession
 from pyspark.sql import functions as sf
 from pyspark.sql.types import StructType
 
+from tmlt.core.utils.join import join
 from tmlt.core.utils.misc import get_nonconflicting_string
 
 
 class GroupedDataFrame:
     """Grouped DataFrame implementation supporting explicit group keys.
 
     A GroupedDataFrame object encapsulates the spark DataFrame to be grouped by as well
@@ -80,40 +81,14 @@
         ]
         if invalid_columns:
             raise ValueError(f"Invalid columns: {invalid_columns}")
         return GroupedDataFrame(
             dataframe=self._dataframe.select(*columns), group_keys=self.group_keys
         )
 
-    def _null_safe_join(self, df: sf.DataFrame) -> DataFrame:
-        """Join self.group_keys with another Dataframe, in a null-safe way."""
-        # By default the join operator is NOT null-safe
-        # so instead, we have to make this ugly join condition:
-        cond = [
-            self.group_keys[col].eqNullSafe(df[col]) for col in self.groupby_columns
-        ]
-        # and use that for the 'on' parameter:
-        out = self.group_keys.join(df, on=cond, how="left")
-        # Now the dataframe will have 2 copies of each column that you grouped by -
-        # one for self.group_keys, and one for the other dataframe.
-        # (For example, if you joined on columns A and B,
-        # the resulting dataframe would have two column As and two column Bs.)
-        # The column from self.group_keys will have every relevant group_key
-        # (for example, column "A" would have "a1", "a2", and "a3").
-        # The other dataframe (df) might not have every value
-        # (for example, column "A" might only have "a2").
-        # So you want to drop the columns from the other dataframe,
-        # and keep the columns from self.group_keys.
-        for col in self.groupby_columns:
-            out = out.drop(df[col])
-        # Now we finally have the dataframe we want: one that contains every
-        # value from self.group_keys, without duplicate columns, joined
-        # appropriately on null values.
-        return out
-
     def agg(self, func: Column, fill_value: Any) -> DataFrame:
         """Applies given spark function (column expression) to each group.
 
         The output DataFrame is guaranteed to have exactly one row for each group
         key. For group keys corresponding to empty groups, the output column will
         contain the supplied `fill_value`. The output DataFrame is also sorted by
         the groupby columns.
@@ -132,22 +107,26 @@
         assert len(agg_output_columns) == 1
         output_column = agg_output_columns.pop()
         empty_indicator = get_nonconflicting_string(nonempty_groups_output.columns)
 
         nonempty_groups_output = (
             self._dataframe.groupBy(self.groupby_columns)
             .agg(func)
-            .withColumn(empty_indicator, sf.lit(False))
-        )
-        all_groups_output = self._null_safe_join(nonempty_groups_output).fillna(
-            {empty_indicator: True}
+            .withColumn(empty_indicator, sf.lit(0))
         )
+        all_groups_output = join(
+            left=self.group_keys,
+            right=nonempty_groups_output,
+            on=self.groupby_columns,
+            how="left",
+            nulls_are_equal=True,
+        ).fillna({empty_indicator: 1})
         return all_groups_output.withColumn(
             output_column,
-            sf.when(sf.col(empty_indicator), sf.lit(fill_value)).otherwise(
+            sf.when(sf.col(empty_indicator) == 1, sf.lit(fill_value)).otherwise(
                 sf.col(output_column)
             ),
         ).drop(empty_indicator)
 
     def apply_in_pandas(
         self,
         aggregation_function: Callable[[pd.DataFrame], pd.DataFrame],
@@ -173,18 +152,24 @@
             return spark.createDataFrame(
                 aggregation_function(self._dataframe.toPandas()),
                 schema=aggregation_output_schema,
             )
 
         empty_indicator = get_nonconflicting_string(self._dataframe.columns)
         sdf = self._dataframe.withColumn(
-            empty_indicator, sf.lit(False)  # pylint: disable=no-member
+            empty_indicator, sf.lit(0)  # pylint: disable=no-member
         )
 
-        sdf = self._null_safe_join(sdf).fillna({empty_indicator: True})
+        sdf = join(
+            left=self.group_keys,
+            right=sdf,
+            on=self.groupby_columns,
+            how="left",
+            nulls_are_equal=True,
+        ).fillna({empty_indicator: 1})
 
         grouped_df = sdf.groupby(*self.groupby_columns)
         agg_input_columns = list(
             set(sdf.columns) - set(self.groupby_columns) - {empty_indicator}
         )
         _wrapper = _create_aggregation_wrapper(
             aggregation_function=aggregation_function,
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/misc.py` & `tmlt_core-0.9.0/tmlt/core/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """Constructor.
 
         Args:
             rng: NumPy random generator.
         """
         self._rng = rng
         self._MAX_INT = int(np.iinfo(np.int64).max)
-        assert self._MAX_INT == 2 ** 63 - 1
+        assert self._MAX_INT == 2**63 - 1
 
     def randrange(self, high: int) -> int:
         """Returns a random integer between 0 (inclusive) and `high` (exclusive).
 
         Args:
             high: upper bound for random integer range.
         """
@@ -41,15 +41,15 @@
         while bits >= 63:
             bits -= 63
             random_integer <<= 63
             random_integer += int(
                 self._rng.integers(low=0, high=self._MAX_INT, endpoint=True)
             )
         random_integer <<= bits
-        random_integer += int(self._rng.integers(low=0, high=2 ** bits, endpoint=False))
+        random_integer += int(self._rng.integers(low=0, high=2**bits, endpoint=False))
         # random_integer may be >= high, but we can try again.
         # Note that this will work at least half of the time.
         if random_integer >= high:
             return self.randrange(high)
         return random_integer
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/parameters.py` & `tmlt_core-0.9.0/tmlt/core/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/testing.py` & `tmlt_core-0.9.0/tmlt/core/utils/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,26 @@
 # TODO(#1218): Move dummy aggregate class back to the test.
 
 import logging
 import shutil
 import sys
 import unittest
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Iterable, List, Sequence, Tuple, Union, overload
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    overload,
+)
 from unittest.mock import Mock, create_autospec
 
 import numpy as np
 import pandas as pd
 from nose.tools import nottest
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import DoubleType, StringType, StructField, StructType
@@ -352,30 +363,30 @@
         cls._spark.stop()
 
     @classmethod
     def assert_frame_equal_with_sort(
         cls,
         first_df: pd.DataFrame,
         second_df: pd.DataFrame,
-        sort_columns: Sequence[str] = None,
+        sort_columns: Optional[Sequence[str]] = None,
         **kwargs: Any,
     ):
         """Asserts that the two data frames are equal.
 
         Wrapper around pandas test function. Both dataframes are sorted
         since the ordering in Spark is not guaranteed.
 
         Args:
             first_df: First dataframe to compare.
             second_df: Second dataframe to compare.
             sort_columns: Names of column to sort on. By default sorts by all columns.
             **kwargs: Keyword arguments that will be passed to assert_frame_equal().
         """
         if sorted(first_df.columns) != sorted(second_df.columns):
-            raise ValueError(
+            raise AssertionError(
                 "Dataframes must have matching columns. "
                 f"first_df: {sorted(first_df.columns)}. "
                 f"second_df: {sorted(second_df.columns)}."
             )
         if first_df.empty and second_df.empty:
             return
         if sort_columns is None:
@@ -767,39 +778,39 @@
         else s2
     )
     if agg == "count":
         scale = second_if_gauss(1 / budget, 1 / (2 * budget))
         return {"count": scale}
     if agg == "sum":
         scale = second_if_gauss(
-            dataset.upper / budget, dataset.upper ** 2 / (2 * budget)
+            dataset.upper / budget, dataset.upper**2 / (2 * budget)
         )
         return {"sum": scale}
     if agg == "average":
         sod_sensitivity = (dataset.upper - dataset.lower) / 2
         budget_per_subagg = budget / 2
         sod_scale = second_if_gauss(
             sod_sensitivity / budget_per_subagg,
-            sod_sensitivity ** 2 / (2 * budget_per_subagg),
+            sod_sensitivity**2 / (2 * budget_per_subagg),
         )
         count_scale = second_if_gauss(
             1 / budget_per_subagg, 1 / (2 * budget_per_subagg)
         )
         return {"sum": sod_scale, "count": count_scale}
     if agg in ("standard deviation", "variance"):
         sod_sensitivity = (dataset.upper - dataset.lower) / 2
-        sos_sensitivity = (dataset.upper ** 2 - dataset.lower ** 2) / 2
+        sos_sensitivity = (dataset.upper**2 - dataset.lower**2) / 2
         budget_per_subagg = budget / 3
         sod_scale = second_if_gauss(
             sod_sensitivity / budget_per_subagg,
-            sod_sensitivity ** 2 / (2 * budget_per_subagg),
+            sod_sensitivity**2 / (2 * budget_per_subagg),
         )
         sos_scale = second_if_gauss(
             sos_sensitivity / budget_per_subagg,
-            sos_sensitivity ** 2 / (2 * budget_per_subagg),
+            sos_sensitivity**2 / (2 * budget_per_subagg),
         )
         count_scale = second_if_gauss(
             1 / budget_per_subagg, 1 / (2 * budget_per_subagg)
         )
         return {"sum": sod_scale, "count": count_scale, "sum_of_squares": sos_scale}
     raise ValueError(agg)
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/truncation.py` & `tmlt_core-0.9.0/tmlt/core/utils/truncation.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,26 +61,34 @@
 
     Args:
         df: DataFrame to truncate.
         grouping_columns: Columns defining the groups.
         threshold: Maximum number of rows to include for each group.
     """
     rank_column = get_nonconflicting_string(df.columns)
-    hash_column = get_nonconflicting_string(df.columns + [rank_column])
+    row_index_column = get_nonconflicting_string(df.columns + [rank_column])
+    hash_column = get_nonconflicting_string(
+        df.columns + [row_index_column, rank_column]
+    )
+    distinct_row_partitions = Window.partitionBy(*df.columns).orderBy(*df.columns)
     shuffled_partitions = Window.partitionBy(*grouping_columns).orderBy(
         hash_column, *df.columns
     )
     return (
-        df.withColumn(hash_column, sf.hash(*df.columns))  # pylint: disable=no-member
+        df.withColumn(row_index_column, sf.row_number().over(distinct_row_partitions))
+        .withColumn(
+            hash_column,
+            sf.hash(*df.columns, row_index_column),  # pylint: disable=no-member
+        )
         .withColumn(
             rank_column,
             sf.row_number().over(shuffled_partitions),  # pylint: disable=no-member
         )
         .filter(f"{rank_column}<={threshold}")
-        .drop(rank_column, hash_column)
+        .drop(rank_column, hash_column, row_index_column)
     )
 
 
 def drop_large_groups(
     df: DataFrame, grouping_columns: List[str], threshold: int
 ) -> DataFrame:
     """Drop all rows for groups that have more than `threshold` rows.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/type_utils.py` & `tmlt_core-0.9.0/tmlt/core/utils/type_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def assert_never(x: NoReturn) -> NoReturn:
     """Assertion for statically checking exhaustive pattern matches.
 
     From https://github.com/python/mypy/issues/5818.
     """
-    assert False, "Unhandled type: {}".format(type(x).__name__)
+    assert False, f"Unhandled type: {type(x).__name__}"
 
 
 def get_element_type(l: Sequence[Any], allow_none: bool = True) -> type:
     """Return the Python type of the non-``None`` elements of a list.
 
     If the given list is empty or contains elements with multiple types, raises
     ValueError.
```

### Comparing `tmlt_core-0.8.3/tmlt/core/utils/validation.py` & `tmlt_core-0.9.0/tmlt/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.8.3/PKG-INFO` & `tmlt_core-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-core
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tumult's differential privacy primitives
 Home-page: https://gitlab.com/tumult-labs/core
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

