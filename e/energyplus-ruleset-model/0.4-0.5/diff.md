# Comparing `tmp/energyplus_ruleset_model-0.4.tar.gz` & `tmp/energyplus_ruleset_model-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_ruleset_model-0.4.tar", last modified: Fri Mar  3 20:56:32 2023, max compression
+gzip compressed data, was "energyplus_ruleset_model-0.5.tar", last modified: Fri Apr 14 16:23:31 2023, max compression
```

## Comparing `energyplus_ruleset_model-0.4.tar` & `energyplus_ruleset_model-0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:56:32.265081 energyplus_ruleset_model-0.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-03-03 20:56:32.265081 energyplus_ruleset_model-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:56:32.261081 energyplus_ruleset_model-0.4/energyplus_rmd/
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/input_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/output_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/status_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)    50958 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/translator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/energyplus_rmd/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:56:32.265081 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-03 20:56:32.000000 energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-03-03 20:56:32.265081 energyplus_ruleset_model-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-03-03 20:56:21.000000 energyplus_ruleset_model-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:23:31.680852 energyplus_ruleset_model-0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6310 2023-04-14 16:23:31.680852 energyplus_ruleset_model-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:23:31.680852 energyplus_ruleset_model-0.5/energyplus_rmd/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/input_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/output_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/status_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50958 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/translator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/energyplus_rmd/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:23:31.680852 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6310 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-14 16:23:31.000000 energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-04-14 16:23:31.680852 energyplus_ruleset_model-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-14 16:23:20.000000 energyplus_ruleset_model-0.5/setup.py
```

### Comparing `energyplus_ruleset_model-0.4/LICENSE` & `energyplus_ruleset_model-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/PKG-INFO` & `energyplus_ruleset_model-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: energyplus_ruleset_model
-Version: 0.4
+Version: 0.5
 Summary: A Python tool for generating RMDs.
 Home-page: https://github.com/JasonGlazer/createRulesetModelDescription
 Author: Jason Glazer
-Author-email: 
+License: ModifiedBSD
 Keywords: energyplus
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # createRulesetModelDescription
```

### Comparing `energyplus_ruleset_model-0.4/README.md` & `energyplus_ruleset_model-0.5/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/energyplus_rmd/input_file.py` & `energyplus_ruleset_model-0.5/energyplus_rmd/input_file.py`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/energyplus_rmd/status_reporter.py` & `energyplus_ruleset_model-0.5/energyplus_rmd/status_reporter.py`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/energyplus_rmd/translator.py` & `energyplus_ruleset_model-0.5/energyplus_rmd/translator.py`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/energyplus_rmd/validator.py` & `energyplus_ruleset_model-0.5/energyplus_rmd/validator.py`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/PKG-INFO` & `energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: energyplus-ruleset-model
-Version: 0.4
+Version: 0.5
 Summary: A Python tool for generating RMDs.
 Home-page: https://github.com/JasonGlazer/createRulesetModelDescription
 Author: Jason Glazer
-Author-email: 
+License: ModifiedBSD
 Keywords: energyplus
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # createRulesetModelDescription
```

### Comparing `energyplus_ruleset_model-0.4/energyplus_ruleset_model.egg-info/SOURCES.txt` & `energyplus_ruleset_model-0.5/energyplus_ruleset_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_ruleset_model-0.4/setup.py` & `energyplus_ruleset_model-0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 readme_contents = readme_file.read_text()
 
 setup(
     name='energyplus_ruleset_model',
     version=VERSION,
     packages=['energyplus_rmd'],
     url='https://github.com/JasonGlazer/createRulesetModelDescription',
-    license='',
+    license='ModifiedBSD',
     author='Jason Glazer',
-    author_email='',
     description='A Python tool for generating RMDs.',
     package_data={
         "eplus_rmd": [
             "example/*",
             "*.json",
             "*.yaml",
             "*.txt",
```

