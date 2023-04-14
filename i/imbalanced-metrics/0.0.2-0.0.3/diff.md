# Comparing `tmp/imbalanced_metrics-0.0.2.tar.gz` & `tmp/imbalanced_metrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbalanced_metrics-0.0.2.tar", last modified: Fri Apr 14 02:51:28 2023, max compression
+gzip compressed data, was "imbalanced_metrics-0.0.3.tar", last modified: Fri Apr 14 03:04:28 2023, max compression
```

## Comparing `imbalanced_metrics-0.0.2.tar` & `imbalanced_metrics-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 02:51:28.502886 imbalanced_metrics-0.0.2/
--rw-rw-rw-   0        0        0    35149 2023-04-11 01:48:50.000000 imbalanced_metrics-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6285 2023-04-14 02:51:28.501895 imbalanced_metrics-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5302 2023-04-14 02:40:02.000000 imbalanced_metrics-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 02:51:28.492570 imbalanced_metrics-0.0.2/imbalanced_metrics/
--rw-rw-rw-   0        0        0      102 2023-04-11 18:51:46.000000 imbalanced_metrics-0.0.2/imbalanced_metrics/__init__.py
--rw-rw-rw-   0        0        0     7752 2023-04-14 02:26:45.000000 imbalanced_metrics-0.0.2/imbalanced_metrics/classification_metrics.py
--rw-rw-rw-   0        0        0     9031 2023-04-07 14:43:50.000000 imbalanced_metrics-0.0.2/imbalanced_metrics/regression_metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-14 02:51:28.500903 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/
--rw-rw-rw-   0        0        0     6285 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 02:51:28.502886 imbalanced_metrics-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1345 2023-04-14 02:50:57.000000 imbalanced_metrics-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:04:28.205659 imbalanced_metrics-0.0.3/
+-rw-rw-rw-   0        0        0    35149 2023-04-11 01:48:50.000000 imbalanced_metrics-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6279 2023-04-14 03:04:28.204660 imbalanced_metrics-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5299 2023-04-14 02:53:51.000000 imbalanced_metrics-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 03:04:28.193133 imbalanced_metrics-0.0.3/imbalanced_metrics/
+-rw-rw-rw-   0        0        0      102 2023-04-11 18:51:46.000000 imbalanced_metrics-0.0.3/imbalanced_metrics/__init__.py
+-rw-rw-rw-   0        0        0     7752 2023-04-14 02:26:45.000000 imbalanced_metrics-0.0.3/imbalanced_metrics/classification_metrics.py
+-rw-rw-rw-   0        0        0     9031 2023-04-07 14:43:50.000000 imbalanced_metrics-0.0.3/imbalanced_metrics/regression_metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:04:28.203652 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/
+-rw-rw-rw-   0        0        0     6279 2023-04-14 03:04:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-14 03:04:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:04:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 02:51:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-04-14 03:04:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-14 03:04:28.000000 imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:04:28.205659 imbalanced_metrics-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1344 2023-04-14 03:02:46.000000 imbalanced_metrics-0.0.3/setup.py
```

### Comparing `imbalanced_metrics-0.0.2/LICENSE` & `imbalanced_metrics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imbalanced_metrics-0.0.2/PKG-INFO` & `imbalanced_metrics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: imbalanced_metrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Perfromance metrics for imbalanced classification and imbalanced regression tasks
-Home-page: https://github.com/paobranco/ImabalanceMetrics
+Home-page: https://github.com/paobranco/ImbalanceMetrics
 Author: Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco
 Author-email: stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca
 Keywords: imbalanced learning,classification,regression,metrics
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -88,15 +88,15 @@
 
 ## Contributions
 
 ImablanceMetrics is open for improvements and maintenance. Your help is valued to make the package better for everyone.
 
 ## License
 
-Â© Licensed under the General Public License v3.0 (GPLv3).
+Licensed under the General Public License v3.0 (GPLv3).
 
 ## Reference
 
 - Ribeiro, R.P.: Utility-based regression. Ph.D. thesis, Dep. Computer Science, Faculty of Sciences - University of Porto (2011)
 - Branco, P., Ribeiro, R.P., Torgo, L.: UBL: an R package for utility-based learning (2016), https://arxiv.org/abs/1604.08079
 - Branco, P., Torgo, L., Ribeiro, R.: A survey of predictive modelling under imbalanced distributions (2015)
 - Branco, P., Torgo, L., Ribeiro, R.P.: A survey of predictive modeling on imbalanced domains. ACM Computing Surveys (CSUR) 49(2), 1â€“50 (2016)
```

### Comparing `imbalanced_metrics-0.0.2/README.md` & `imbalanced_metrics-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 ## Contributions
 
 ImablanceMetrics is open for improvements and maintenance. Your help is valued to make the package better for everyone.
 
 ## License
 
-© Licensed under the General Public License v3.0 (GPLv3).
+Licensed under the General Public License v3.0 (GPLv3).
 
 ## Reference
 
 - Ribeiro, R.P.: Utility-based regression. Ph.D. thesis, Dep. Computer Science, Faculty of Sciences - University of Porto (2011)
 - Branco, P., Ribeiro, R.P., Torgo, L.: UBL: an R package for utility-based learning (2016), https://arxiv.org/abs/1604.08079
 - Branco, P., Torgo, L., Ribeiro, R.: A survey of predictive modelling under imbalanced distributions (2015)
 - Branco, P., Torgo, L., Ribeiro, R.P.: A survey of predictive modeling on imbalanced domains. ACM Computing Surveys (CSUR) 49(2), 1–50 (2016)
```

### Comparing `imbalanced_metrics-0.0.2/imbalanced_metrics/classification_metrics.py` & `imbalanced_metrics-0.0.3/imbalanced_metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `imbalanced_metrics-0.0.2/imbalanced_metrics/regression_metrics.py` & `imbalanced_metrics-0.0.3/imbalanced_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `imbalanced_metrics-0.0.2/imbalanced_metrics.egg-info/PKG-INFO` & `imbalanced_metrics-0.0.3/imbalanced_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: imbalanced-metrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Perfromance metrics for imbalanced classification and imbalanced regression tasks
-Home-page: https://github.com/paobranco/ImabalanceMetrics
+Home-page: https://github.com/paobranco/ImbalanceMetrics
 Author: Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco
 Author-email: stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca
 Keywords: imbalanced learning,classification,regression,metrics
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -88,15 +88,15 @@
 
 ## Contributions
 
 ImablanceMetrics is open for improvements and maintenance. Your help is valued to make the package better for everyone.
 
 ## License
 
-Â© Licensed under the General Public License v3.0 (GPLv3).
+Licensed under the General Public License v3.0 (GPLv3).
 
 ## Reference
 
 - Ribeiro, R.P.: Utility-based regression. Ph.D. thesis, Dep. Computer Science, Faculty of Sciences - University of Porto (2011)
 - Branco, P., Ribeiro, R.P., Torgo, L.: UBL: an R package for utility-based learning (2016), https://arxiv.org/abs/1604.08079
 - Branco, P., Torgo, L., Ribeiro, R.: A survey of predictive modelling under imbalanced distributions (2015)
 - Branco, P., Torgo, L., Ribeiro, R.P.: A survey of predictive modeling on imbalanced domains. ACM Computing Surveys (CSUR) 49(2), 1â€“50 (2016)
```

### Comparing `imbalanced_metrics-0.0.2/setup.py` & `imbalanced_metrics-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
       name='imbalanced_metrics',
-      version='0.0.2',
+      version='0.0.3',
       description='Perfromance metrics for imbalanced classification and imbalanced regression tasks',
       long_description = open('README.md').read(),
       long_description_content_type = "text/markdown",
-      url='https://github.com/paobranco/ImabalanceMetrics',
+      url='https://github.com/paobranco/ImbalanceMetrics',
       author='Sadid Rafsun Tulon, Jean-Gabriel Gaudreault, Paula Branco',
       author_email = 'stulo080@uottawa.ca, j.gaudreault@uottawa.ca, pbranco@uottawa.ca',
       classifiers = [
         'Programming Language :: Python :: 3',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
```

