# Comparing `tmp/surveyequivalence-0.1.2.tar.gz` & `tmp/surveyequivalence-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tweni\PycharmProjects\surveyequivalence\dist\.tmp-gjqrmw2o\surveyequivalence-0.1.2.tar", last modified: Fri Apr 14 18:20:53 2023, max compression
+gzip compressed data, was "surveyequivalence-0.1.3.tar", last modified: Fri Apr 14 20:20:25 2023, max compression
```

## Comparing `surveyequivalence-0.1.2.tar` & `surveyequivalence-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.500638 surveyequivalence-0.1.2/
--rw-rw-rw-   0        0        0     1971 2021-05-25 14:16:08.000000 surveyequivalence-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1122 2020-05-18 15:29:55.000000 surveyequivalence-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      106 2021-07-14 13:45:42.000000 surveyequivalence-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4251 2023-04-14 18:20:53.501633 surveyequivalence-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3654 2021-09-09 19:37:27.000000 surveyequivalence-0.1.2/README.md
--rw-rw-rw-   0        0        0      110 2021-07-14 13:45:41.000000 surveyequivalence-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1060 2023-04-14 18:20:53.502627 surveyequivalence-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.404707 surveyequivalence-0.1.2/surveyequivalence/
--rw-rw-rw-   0        0        0      922 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/__init__.py
--rw-rw-rw-   0        0        0    16966 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/combiners.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.436091 surveyequivalence-0.1.2/surveyequivalence/data/
--rw-rw-rw-   0        0        0   143987 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/credweb.csv
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.446115 surveyequivalence-0.1.2/surveyequivalence/data/running_example/
--rw-rw-rw-   0        0        0    76969 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/running_example/predictions.csv
--rw-rw-rw-   0        0        0    44933 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/running_example/ref_rater_labels.csv
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.451105 surveyequivalence-0.1.2/surveyequivalence/data/running_example_50_items/
--rw-rw-rw-   0        0        0     3869 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/running_example_50_items/predictions.csv
--rw-rw-rw-   0        0        0     2233 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/running_example_50_items/ref_rater_labels.csv
--rw-rw-rw-   0        0        0 13168506 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/vote_gtk2.csv
--rw-rw-rw-   0        0        0   750661 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/surveyequivalence/data/wiki_attack_labels_and_predictor.csv
--rw-rw-rw-   0        0        0     2319 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/data_noise_generator.py
--rw-rw-rw-   0        0        0    66164 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/equivalence.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.473868 surveyequivalence-0.1.2/surveyequivalence/examples/
--rw-rw-rw-   0        0        0        0 2021-03-01 16:06:38.000000 surveyequivalence-0.1.2/surveyequivalence/examples/__init__.py
--rw-rw-rw-   0        0        0     8322 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/examples/credbank.py
--rw-rw-rw-   0        0        0     9827 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/examples/guessthekarma.py
--rw-rw-rw-   0        0        0    10107 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/examples/paper_running_example.py
--rw-rw-rw-   0        0        0    10064 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/examples/personal_attacks.py
--rw-rw-rw-   0        0        0    49301 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/scoring_functions.py
--rw-rw-rw-   0        0        0    38545 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/synthetic_datasets.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.481093 surveyequivalence-0.1.2/surveyequivalence/templates/
--rw-rw-rw-   0        0        0      219 2020-12-01 00:29:17.000000 surveyequivalence-0.1.2/surveyequivalence/templates/classifier_template.txt
--rw-rw-rw-   0        0        0      642 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/templates/performance_ratio_template.txt
--rw-rw-rw-   0        0        0      747 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/surveyequivalence/templates/pgf_template.txt
--rw-rw-rw-   0        0        0      210 2021-05-10 16:30:33.000000 surveyequivalence-0.1.2/surveyequivalence/templates/plot_template.txt
--rw-rw-rw-   0        0        0      343 2021-03-03 17:51:25.000000 surveyequivalence-0.1.2/surveyequivalence/templates/surveyequiv_template.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.492138 surveyequivalence-0.1.2/surveyequivalence.egg-info/
--rw-rw-rw-   0        0        0     4251 2023-04-14 18:20:53.000000 surveyequivalence-0.1.2/surveyequivalence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2563 2023-04-14 18:20:53.000000 surveyequivalence-0.1.2/surveyequivalence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 18:20:53.000000 surveyequivalence-0.1.2/surveyequivalence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-04-14 18:20:53.000000 surveyequivalence-0.1.2/surveyequivalence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-14 18:20:53.000000 surveyequivalence-0.1.2/surveyequivalence.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 18:20:53.500638 surveyequivalence-0.1.2/tests/
--rw-rw-rw-   0        0        0     1109 2021-07-14 13:44:25.000000 surveyequivalence-0.1.2/tests/continuous_prediction_tests.py
--rw-rw-rw-   0        0        0    19892 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/tests/discrete_distribution_tests.py
--rw-rw-rw-   0        0        0     9167 2023-04-14 14:21:55.000000 surveyequivalence-0.1.2/tests/scoring_function_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.142294 surveyequivalence-0.1.3/
+-rw-rw-rw-   0        0        0     1971 2021-05-25 14:16:08.000000 surveyequivalence-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0      245 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1122 2020-05-18 15:29:55.000000 surveyequivalence-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      106 2021-07-14 13:45:42.000000 surveyequivalence-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4461 2023-04-14 20:20:25.144246 surveyequivalence-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3864 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/README.md
+-rw-rw-rw-   0        0        0      110 2021-07-14 13:45:41.000000 surveyequivalence-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1060 2023-04-14 20:20:25.148243 surveyequivalence-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.057196 surveyequivalence-0.1.3/surveyequivalence/
+-rw-rw-rw-   0        0        0      922 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/__init__.py
+-rw-rw-rw-   0        0        0    16966 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/combiners.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.083865 surveyequivalence-0.1.3/surveyequivalence/data/
+-rw-rw-rw-   0        0        0   143987 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/credweb.csv
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.089358 surveyequivalence-0.1.3/surveyequivalence/data/running_example/
+-rw-rw-rw-   0        0        0    76969 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/running_example/predictions.csv
+-rw-rw-rw-   0        0        0    44933 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/running_example/ref_rater_labels.csv
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.093379 surveyequivalence-0.1.3/surveyequivalence/data/running_example_50_items/
+-rw-rw-rw-   0        0        0     3869 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/running_example_50_items/predictions.csv
+-rw-rw-rw-   0        0        0     2233 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/running_example_50_items/ref_rater_labels.csv
+-rw-rw-rw-   0        0        0 13168506 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/vote_gtk2.csv
+-rw-rw-rw-   0        0        0   750661 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/surveyequivalence/data/wiki_attack_labels_and_predictor.csv
+-rw-rw-rw-   0        0        0     2319 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/data_noise_generator.py
+-rw-rw-rw-   0        0        0    66164 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/equivalence.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.102080 surveyequivalence-0.1.3/surveyequivalence/examples/
+-rw-rw-rw-   0        0        0        0 2021-03-01 16:06:38.000000 surveyequivalence-0.1.3/surveyequivalence/examples/__init__.py
+-rw-rw-rw-   0        0        0     8322 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/examples/credbank.py
+-rw-rw-rw-   0        0        0     9827 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/examples/guessthekarma.py
+-rw-rw-rw-   0        0        0    10107 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/examples/paper_running_example.py
+-rw-rw-rw-   0        0        0    10064 2023-04-14 20:11:27.000000 surveyequivalence-0.1.3/surveyequivalence/examples/personal_attacks.py
+-rw-rw-rw-   0        0        0    49301 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/scoring_functions.py
+-rw-rw-rw-   0        0        0    38545 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/synthetic_datasets.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.109978 surveyequivalence-0.1.3/surveyequivalence/templates/
+-rw-rw-rw-   0        0        0      219 2020-12-01 00:29:17.000000 surveyequivalence-0.1.3/surveyequivalence/templates/classifier_template.txt
+-rw-rw-rw-   0        0        0      642 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/templates/performance_ratio_template.txt
+-rw-rw-rw-   0        0        0      747 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/surveyequivalence/templates/pgf_template.txt
+-rw-rw-rw-   0        0        0      210 2021-05-10 16:30:33.000000 surveyequivalence-0.1.3/surveyequivalence/templates/plot_template.txt
+-rw-rw-rw-   0        0        0      343 2021-03-03 17:51:25.000000 surveyequivalence-0.1.3/surveyequivalence/templates/surveyequiv_template.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.125439 surveyequivalence-0.1.3/surveyequivalence.egg-info/
+-rw-rw-rw-   0        0        0     4461 2023-04-14 20:20:24.000000 surveyequivalence-0.1.3/surveyequivalence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2581 2023-04-14 20:20:25.000000 surveyequivalence-0.1.3/surveyequivalence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:20:24.000000 surveyequivalence-0.1.3/surveyequivalence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-04-14 20:20:24.000000 surveyequivalence-0.1.3/surveyequivalence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-14 20:20:24.000000 surveyequivalence-0.1.3/surveyequivalence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:20:25.140261 surveyequivalence-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1109 2021-07-14 13:44:25.000000 surveyequivalence-0.1.3/tests/continuous_prediction_tests.py
+-rw-rw-rw-   0        0        0    19892 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/tests/discrete_distribution_tests.py
+-rw-rw-rw-   0        0        0     9167 2023-04-14 20:11:26.000000 surveyequivalence-0.1.3/tests/scoring_function_tests.py
```

### Comparing `surveyequivalence-0.1.2/.gitignore` & `surveyequivalence-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/LICENSE` & `surveyequivalence-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/PKG-INFO` & `surveyequivalence-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: surveyequivalence
-Version: 0.1.2
+Version: 0.1.3
 Summary: Code for calculating survey equivalence
 Home-page: https://github.com/presnick/surveyequivalence
 Author: Paul Resnick, Tim Weninger, Yuqing Kong, and Grant Schoenebeck
 Author-email: presnick@umich.edu
 Project-URL: Bug Tracker, https://github.com/presnick/surveyequivalence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SurveyEquivalence
 Author: Paul Resnick, Yuqing Kong, Grant Schoenebeck, Tim Weninger
 
 **arxiv paper available**: https://arxiv.org/abs/2106.01254
@@ -21,14 +21,15 @@
 **Documentation available**: https://surveyequivalence.readthedocs.io 
 
 ## Overview
 Given a dataset W of ratings for 
 
 Installation
 ------------
+Requires Python version 3.8 or higher. We have tested this with VirtualEnvironment and Conda using Python 3.8 and 3.10 
 
 .. code-block:: console
 
     pip install surveyequivalence
 
 At root level, you should find config.py and directories surveyequivalence, docs, data, etc.
 
@@ -37,22 +38,26 @@
 
 The running example dataset has 1000 items. It takes a while to run it with 500 bootstrap item samples.
 If you're just trying to verify that your installation is good, you may want to run it on a smaller set of items
 with fewer bootstrap item samples.
 
 .. code-block:: console
 
-    (survey_equiv) surveyequivalence[master !?]$ python
-    Python 3.7.4 (default, Aug 13 2019, 20:35:49)
-    [GCC 7.3.0] :: Anaconda, Inc. on linux
+
+    % python 
+    Python 3.8.16 (default, Mar  1 2023, 21:18:45) 
+    [Clang 14.0.6 ] :: Anaconda, Inc. on darwin
     Type "help", "copyright", "credits" or "license" for more information.
     >>> from surveyequivalence.examples.paper_running_example import main
-    >>> main(path='data/running_example_50_items', num_bootstrap_item_samples=10)
+    >>> import pkg_resources
+    >>> DATA_PATH = pkg_resources.resource_filename('surveyequivalence', 'data')
+    >>> main(path=f"{DATA_PATH}/running_example_50_items", num_bootstrap_item_samples=10)
     starting classifiers: computing scores
 
+
 As described in the tutorial, the running example for the paper computes three survey power curves, for three different
 combiner/scorer pairings.
 
 If you have multiple processors, the AnalysisPipeline will try to take advantage of them to speed up execution.
 That may cause the progress indicator output to show some things out of order, like what is shown here.
 That's nothing to worry about.
```

### Comparing `surveyequivalence-0.1.2/README.md` & `surveyequivalence-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 **Documentation available**: https://surveyequivalence.readthedocs.io 
 
 ## Overview
 Given a dataset W of ratings for 
 
 Installation
 ------------
+Requires Python version 3.8 or higher. We have tested this with VirtualEnvironment and Conda using Python 3.8 and 3.10 
 
 .. code-block:: console
 
     pip install surveyequivalence
 
 At root level, you should find config.py and directories surveyequivalence, docs, data, etc.
 
@@ -22,22 +23,26 @@
 
 The running example dataset has 1000 items. It takes a while to run it with 500 bootstrap item samples.
 If you're just trying to verify that your installation is good, you may want to run it on a smaller set of items
 with fewer bootstrap item samples.
 
 .. code-block:: console
 
-    (survey_equiv) surveyequivalence[master !?]$ python
-    Python 3.7.4 (default, Aug 13 2019, 20:35:49)
-    [GCC 7.3.0] :: Anaconda, Inc. on linux
+
+    % python 
+    Python 3.8.16 (default, Mar  1 2023, 21:18:45) 
+    [Clang 14.0.6 ] :: Anaconda, Inc. on darwin
     Type "help", "copyright", "credits" or "license" for more information.
     >>> from surveyequivalence.examples.paper_running_example import main
-    >>> main(path='data/running_example_50_items', num_bootstrap_item_samples=10)
+    >>> import pkg_resources
+    >>> DATA_PATH = pkg_resources.resource_filename('surveyequivalence', 'data')
+    >>> main(path=f"{DATA_PATH}/running_example_50_items", num_bootstrap_item_samples=10)
     starting classifiers: computing scores
 
+
 As described in the tutorial, the running example for the paper computes three survey power curves, for three different
 combiner/scorer pairings.
 
 If you have multiple processors, the AnalysisPipeline will try to take advantage of them to speed up execution.
 That may cause the progress indicator output to show some things out of order, like what is shown here.
 That's nothing to worry about.
```

### Comparing `surveyequivalence-0.1.2/setup.cfg` & `surveyequivalence-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7572 7665 7965 7175 6976 616c   = surveyequival
 00000020: 656e 6365 0d0a 7665 7273 696f 6e20 3d20  ence..version = 
-00000030: 302e 312e 320d 0a61 7574 686f 7220 3d20  0.1.2..author = 
+00000030: 302e 312e 330d 0a61 7574 686f 7220 3d20  0.1.3..author = 
 00000040: 5061 756c 2052 6573 6e69 636b 2c20 5469  Paul Resnick, Ti
 00000050: 6d20 5765 6e69 6e67 6572 2c20 5975 7169  m Weninger, Yuqi
 00000060: 6e67 204b 6f6e 672c 2061 6e64 2047 7261  ng Kong, and Gra
 00000070: 6e74 2053 6368 6f65 6e65 6265 636b 0d0a  nt Schoenebeck..
 00000080: 6175 7468 6f72 5f65 6d61 696c 203d 2070  author_email = p
 00000090: 7265 736e 6963 6b40 756d 6963 682e 6564  resnick@umich.ed
 000000a0: 750d 0a64 6573 6372 6970 7469 6f6e 203d  u..description =
@@ -34,15 +34,15 @@
 00000210: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
 00000220: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 00000230: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 00000240: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
 00000250: 5f64 6972 203d 200d 0a09 3d20 2e0d 0a70  _dir = ...= ...p
 00000260: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
 00000270: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000280: 203d 203e 3d33 2e36 0d0a 696e 636c 7564   = >=3.6..includ
+00000280: 203d 203e 3d33 2e38 0d0a 696e 636c 7564   = >=3.8..includ
 00000290: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
 000002a0: 2066 616c 7365 0d0a 696e 7374 616c 6c5f   false..install_
 000002b0: 7265 7175 6972 6573 203d 200d 0a09 7365  requires = ...se
 000002c0: 7475 7074 6f6f 6c73 7e3d 3637 2e36 2e31  tuptools~=67.6.1
 000002d0: 0d0a 096e 756d 7079 7e3d 312e 3234 2e30  ...numpy~=1.24.0
 000002e0: 0d0a 0970 616e 6461 737e 3d32 2e30 2e30  ...pandas~=2.0.0
 000002f0: 0d0a 096d 6174 706c 6f74 6c69 627e 3d33  ...matplotlib~=3
```

### Comparing `surveyequivalence-0.1.2/surveyequivalence/__init__.py` & `surveyequivalence-0.1.3/surveyequivalence/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/combiners.py` & `surveyequivalence-0.1.3/surveyequivalence/combiners.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/credweb.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/credweb.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/running_example/predictions.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/running_example/predictions.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/running_example/ref_rater_labels.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/running_example/ref_rater_labels.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/running_example_50_items/predictions.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/running_example_50_items/predictions.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/running_example_50_items/ref_rater_labels.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/running_example_50_items/ref_rater_labels.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/vote_gtk2.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/vote_gtk2.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data/wiki_attack_labels_and_predictor.csv` & `surveyequivalence-0.1.3/surveyequivalence/data/wiki_attack_labels_and_predictor.csv`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/data_noise_generator.py` & `surveyequivalence-0.1.3/surveyequivalence/data_noise_generator.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/equivalence.py` & `surveyequivalence-0.1.3/surveyequivalence/equivalence.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/examples/credbank.py` & `surveyequivalence-0.1.3/surveyequivalence/examples/credbank.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/examples/guessthekarma.py` & `surveyequivalence-0.1.3/surveyequivalence/examples/guessthekarma.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/examples/paper_running_example.py` & `surveyequivalence-0.1.3/surveyequivalence/examples/paper_running_example.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/examples/personal_attacks.py` & `surveyequivalence-0.1.3/surveyequivalence/examples/personal_attacks.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/scoring_functions.py` & `surveyequivalence-0.1.3/surveyequivalence/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/synthetic_datasets.py` & `surveyequivalence-0.1.3/surveyequivalence/synthetic_datasets.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/templates/performance_ratio_template.txt` & `surveyequivalence-0.1.3/surveyequivalence/templates/performance_ratio_template.txt`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence/templates/pgf_template.txt` & `surveyequivalence-0.1.3/surveyequivalence/templates/pgf_template.txt`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/surveyequivalence.egg-info/PKG-INFO` & `surveyequivalence-0.1.3/surveyequivalence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: surveyequivalence
-Version: 0.1.2
+Version: 0.1.3
 Summary: Code for calculating survey equivalence
 Home-page: https://github.com/presnick/surveyequivalence
 Author: Paul Resnick, Tim Weninger, Yuqing Kong, and Grant Schoenebeck
 Author-email: presnick@umich.edu
 Project-URL: Bug Tracker, https://github.com/presnick/surveyequivalence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SurveyEquivalence
 Author: Paul Resnick, Yuqing Kong, Grant Schoenebeck, Tim Weninger
 
 **arxiv paper available**: https://arxiv.org/abs/2106.01254
@@ -21,14 +21,15 @@
 **Documentation available**: https://surveyequivalence.readthedocs.io 
 
 ## Overview
 Given a dataset W of ratings for 
 
 Installation
 ------------
+Requires Python version 3.8 or higher. We have tested this with VirtualEnvironment and Conda using Python 3.8 and 3.10 
 
 .. code-block:: console
 
     pip install surveyequivalence
 
 At root level, you should find config.py and directories surveyequivalence, docs, data, etc.
 
@@ -37,22 +38,26 @@
 
 The running example dataset has 1000 items. It takes a while to run it with 500 bootstrap item samples.
 If you're just trying to verify that your installation is good, you may want to run it on a smaller set of items
 with fewer bootstrap item samples.
 
 .. code-block:: console
 
-    (survey_equiv) surveyequivalence[master !?]$ python
-    Python 3.7.4 (default, Aug 13 2019, 20:35:49)
-    [GCC 7.3.0] :: Anaconda, Inc. on linux
+
+    % python 
+    Python 3.8.16 (default, Mar  1 2023, 21:18:45) 
+    [Clang 14.0.6 ] :: Anaconda, Inc. on darwin
     Type "help", "copyright", "credits" or "license" for more information.
     >>> from surveyequivalence.examples.paper_running_example import main
-    >>> main(path='data/running_example_50_items', num_bootstrap_item_samples=10)
+    >>> import pkg_resources
+    >>> DATA_PATH = pkg_resources.resource_filename('surveyequivalence', 'data')
+    >>> main(path=f"{DATA_PATH}/running_example_50_items", num_bootstrap_item_samples=10)
     starting classifiers: computing scores
 
+
 As described in the tutorial, the running example for the paper computes three survey power curves, for three different
 combiner/scorer pairings.
 
 If you have multiple processors, the AnalysisPipeline will try to take advantage of them to speed up execution.
 That may cause the progress indicator output to show some things out of order, like what is shown here.
 That's nothing to worry about.
```

### Comparing `surveyequivalence-0.1.2/surveyequivalence.egg-info/SOURCES.txt` & `surveyequivalence-0.1.3/surveyequivalence.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 ./surveyequivalence/__init__.py
 ./surveyequivalence/combiners.py
```

### Comparing `surveyequivalence-0.1.2/tests/continuous_prediction_tests.py` & `surveyequivalence-0.1.3/tests/continuous_prediction_tests.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/tests/discrete_distribution_tests.py` & `surveyequivalence-0.1.3/tests/discrete_distribution_tests.py`

 * *Files identical despite different names*

### Comparing `surveyequivalence-0.1.2/tests/scoring_function_tests.py` & `surveyequivalence-0.1.3/tests/scoring_function_tests.py`

 * *Files identical despite different names*

