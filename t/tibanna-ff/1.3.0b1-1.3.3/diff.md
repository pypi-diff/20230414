# Comparing `tmp/tibanna_ff-1.3.0b1.tar.gz` & `tmp/tibanna_ff-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibanna_ff-1.3.0b1.tar", max compression
+gzip compressed data, was "tibanna_ff-1.3.3.tar", max compression
```

## Comparing `tibanna_ff-1.3.0b1.tar` & `tibanna_ff-1.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1083 2021-09-09 16:55:28.100725 tibanna_ff-1.3.0b1/LICENSE.txt
--rw-r--r--   0        0        0      290 2021-09-09 16:55:28.100977 tibanna_ff-1.3.0b1/README.md
--rw-r--r--   0        0        0     2169 2022-12-13 18:44:05.792839 tibanna_ff-1.3.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.176651 tibanna_ff-1.3.0b1/tibanna_4dn/__init__.py
--rw-r--r--   0        0        0     9943 2021-09-09 16:55:28.176936 tibanna_ff-1.3.0b1/tibanna_4dn/__main__.py
--rw-r--r--   0        0        0     2352 2022-05-12 18:43:14.943285 tibanna_ff-1.3.0b1/tibanna_4dn/core.py
--rw-r--r--   0        0        0      317 2021-09-09 16:55:28.177367 tibanna_ff-1.3.0b1/tibanna_4dn/iam_utils.py
--rw-r--r--   0        0        0      131 2021-09-23 17:36:29.921830 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/__init__.py
--rw-r--r--   0        0        0      447 2021-09-09 16:55:28.177955 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/check_task.py
--rw-r--r--   0        0        0      105 2022-12-09 17:52:33.748799 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/requirements.txt
--rw-r--r--   0        0        0      435 2021-09-09 16:55:28.178373 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/run_task.py
--rw-r--r--   0        0        0     1065 2022-05-12 18:43:14.950624 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/start_run.py
--rw-r--r--   0        0        0      230 2021-11-02 15:52:14.099351 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/update_cost.py
--rw-r--r--   0        0        0     1251 2022-05-12 18:43:14.956966 tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     6067 2021-10-06 17:12:17.709226 tibanna_ff-1.3.0b1/tibanna_4dn/pony_utils.py
--rw-r--r--   0        0        0      934 2022-02-02 21:42:36.484027 tibanna_ff-1.3.0b1/tibanna_4dn/start_run.py
--rw-r--r--   0        0        0      318 2021-09-09 16:55:28.180862 tibanna_ff-1.3.0b1/tibanna_4dn/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-11-02 15:52:14.100504 tibanna_ff-1.3.0b1/tibanna_4dn/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1450 2021-09-09 16:55:28.181306 tibanna_ff-1.3.0b1/tibanna_4dn/update_ffmeta.py
--rw-r--r--   0        0        0      863 2022-09-07 17:39:50.069810 tibanna_ff-1.3.0b1/tibanna_4dn/vars.py
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.181843 tibanna_ff-1.3.0b1/tibanna_cgap/__init__.py
--rw-r--r--   0        0        0     9962 2022-02-02 21:42:36.485354 tibanna_ff-1.3.0b1/tibanna_cgap/__main__.py
--rw-r--r--   0        0        0      255 2021-09-09 16:55:28.182378 tibanna_ff-1.3.0b1/tibanna_cgap/check_task.py
--rw-r--r--   0        0        0     2769 2022-02-02 21:42:36.486858 tibanna_ff-1.3.0b1/tibanna_cgap/core.py
--rw-r--r--   0        0        0      300 2021-09-09 16:55:28.182774 tibanna_ff-1.3.0b1/tibanna_cgap/cw_utils.py
--rw-r--r--   0        0        0      318 2021-09-09 16:55:28.182976 tibanna_ff-1.3.0b1/tibanna_cgap/iam_utils.py
--rw-r--r--   0        0        0      132 2021-09-16 20:24:20.855907 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/__init__.py
--rw-r--r--   0        0        0      467 2021-09-09 16:55:28.183470 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/check_task.py
--rw-r--r--   0        0        0      105 2022-12-09 17:52:24.544723 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/requirements.txt
--rw-r--r--   0        0        0      436 2021-09-09 16:55:28.183912 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/run_task.py
--rw-r--r--   0        0        0     1068 2022-05-12 18:43:14.968145 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/start_run.py
--rw-r--r--   0        0        0      231 2021-11-02 15:52:14.104064 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/update_cost.py
--rw-r--r--   0        0        0     1285 2022-05-12 18:43:14.977223 tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     1281 2022-02-02 21:42:36.490690 tibanna_ff-1.3.0b1/tibanna_cgap/start_run.py
--rw-r--r--   0        0        0      319 2021-09-09 16:55:28.185766 tibanna_ff-1.3.0b1/tibanna_cgap/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-11-01 14:42:13.461080 tibanna_ff-1.3.0b1/tibanna_cgap/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1098 2021-09-09 16:55:28.186145 tibanna_ff-1.3.0b1/tibanna_cgap/update_ffmeta.py
--rw-r--r--   0        0        0     1106 2022-09-07 17:39:50.071236 tibanna_ff-1.3.0b1/tibanna_cgap/vars.py
--rw-r--r--   0        0        0     6094 2021-10-06 17:12:17.709135 tibanna_ff-1.3.0b1/tibanna_cgap/zebra_utils.py
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.186877 tibanna_ff-1.3.0b1/tibanna_ffcommon/__init__.py
--rw-r--r--   0        0        0      504 2022-05-12 18:43:14.981898 tibanna_ff-1.3.0b1/tibanna_ffcommon/_version.py
--rw-r--r--   0        0        0      677 2021-09-09 16:55:28.187272 tibanna_ff-1.3.0b1/tibanna_ffcommon/config.py
--rw-r--r--   0        0        0     4090 2022-12-06 22:12:33.447840 tibanna_ff-1.3.0b1/tibanna_ffcommon/core.py
--rw-r--r--   0        0        0     3796 2021-09-09 16:55:28.187763 tibanna_ff-1.3.0b1/tibanna_ffcommon/exceptions.py
--rw-r--r--   0        0        0     2302 2021-09-09 16:55:28.188001 tibanna_ff-1.3.0b1/tibanna_ffcommon/extra_files.py
--rw-r--r--   0        0        0     2171 2021-09-09 16:55:28.188228 tibanna_ff-1.3.0b1/tibanna_ffcommon/file_format.py
--rw-r--r--   0        0        0     2019 2022-02-02 21:42:36.495197 tibanna_ff-1.3.0b1/tibanna_ffcommon/iam_utils.py
--rw-r--r--   0        0        0    16971 2021-10-06 17:12:17.709262 tibanna_ff-1.3.0b1/tibanna_ffcommon/input_files.py
--rw-r--r--   0        0        0    71677 2022-10-19 22:24:26.016980 tibanna_ff-1.3.0b1/tibanna_ffcommon/portal_utils.py
--rw-r--r--   0        0        0    22781 2022-07-15 16:52:13.865320 tibanna_ff-1.3.0b1/tibanna_ffcommon/qc.py
--rw-r--r--   0        0        0     3162 2021-09-09 16:55:28.190327 tibanna_ff-1.3.0b1/tibanna_ffcommon/stepfunction.py
--rw-r--r--   0        0        0     3252 2022-12-13 18:36:29.816428 tibanna_ff-1.3.0b1/tibanna_ffcommon/vars.py
--rw-r--r--   0        0        0     6489 2022-09-07 16:28:57.074344 tibanna_ff-1.3.0b1/tibanna_ffcommon/wfr.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 tibanna_ff-1.3.0b1/setup.py
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 tibanna_ff-1.3.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-02-12 17:25:26.338682 tibanna_ff-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      290 2020-02-12 17:25:26.339062 tibanna_ff-1.3.3/README.md
+-rw-r--r--   0        0        0     2166 2023-04-14 15:18:20.779999 tibanna_ff-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-12 17:25:26.388455 tibanna_ff-1.3.3/tibanna_4dn/__init__.py
+-rw-r--r--   0        0        0     9943 2021-08-18 20:28:06.333123 tibanna_ff-1.3.3/tibanna_4dn/__main__.py
+-rw-r--r--   0        0        0     2352 2022-07-28 15:27:13.955013 tibanna_ff-1.3.3/tibanna_4dn/core.py
+-rw-r--r--   0        0        0      317 2021-07-19 16:31:16.918389 tibanna_ff-1.3.3/tibanna_4dn/iam_utils.py
+-rw-r--r--   0        0        0      131 2021-09-22 18:05:42.578265 tibanna_ff-1.3.3/tibanna_4dn/lambdas/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-12 17:25:26.389426 tibanna_ff-1.3.3/tibanna_4dn/lambdas/check_task.py
+-rw-r--r--   0        0        0      106 2023-04-14 15:18:20.781080 tibanna_ff-1.3.3/tibanna_4dn/lambdas/requirements.txt
+-rw-r--r--   0        0        0      435 2020-02-12 17:25:26.389831 tibanna_ff-1.3.3/tibanna_4dn/lambdas/run_task.py
+-rw-r--r--   0        0        0     1065 2022-07-28 15:27:13.969283 tibanna_ff-1.3.3/tibanna_4dn/lambdas/start_run.py
+-rw-r--r--   0        0        0      230 2021-11-18 14:02:19.666429 tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1251 2022-07-28 15:27:13.974943 tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     6067 2021-11-01 16:47:18.092418 tibanna_ff-1.3.3/tibanna_4dn/pony_utils.py
+-rw-r--r--   0        0        0      934 2022-05-12 18:36:39.965873 tibanna_ff-1.3.3/tibanna_4dn/start_run.py
+-rw-r--r--   0        0        0      318 2021-08-18 20:28:06.335284 tibanna_ff-1.3.3/tibanna_4dn/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-11-18 14:02:19.668068 tibanna_ff-1.3.3/tibanna_4dn/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1450 2021-07-19 16:31:16.926459 tibanna_ff-1.3.3/tibanna_4dn/update_ffmeta.py
+-rw-r--r--   0        0        0      863 2022-09-21 14:52:08.834451 tibanna_ff-1.3.3/tibanna_4dn/vars.py
+-rw-r--r--   0        0        0        0 2020-02-12 17:25:26.392374 tibanna_ff-1.3.3/tibanna_cgap/__init__.py
+-rw-r--r--   0        0        0     9962 2022-05-12 18:36:39.978678 tibanna_ff-1.3.3/tibanna_cgap/__main__.py
+-rw-r--r--   0        0        0      255 2020-02-12 17:25:26.392929 tibanna_ff-1.3.3/tibanna_cgap/check_task.py
+-rw-r--r--   0        0        0     2769 2022-05-12 18:36:39.983996 tibanna_ff-1.3.3/tibanna_cgap/core.py
+-rw-r--r--   0        0        0      300 2021-07-19 16:31:16.931753 tibanna_ff-1.3.3/tibanna_cgap/cw_utils.py
+-rw-r--r--   0        0        0      318 2021-07-19 16:31:16.932909 tibanna_ff-1.3.3/tibanna_cgap/iam_utils.py
+-rw-r--r--   0        0        0      132 2021-09-22 18:05:42.579587 tibanna_ff-1.3.3/tibanna_cgap/lambdas/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-12 17:25:26.393889 tibanna_ff-1.3.3/tibanna_cgap/lambdas/check_task.py
+-rw-r--r--   0        0        0      106 2023-04-14 15:18:20.781386 tibanna_ff-1.3.3/tibanna_cgap/lambdas/requirements.txt
+-rw-r--r--   0        0        0      436 2020-02-12 17:25:26.394271 tibanna_ff-1.3.3/tibanna_cgap/lambdas/run_task.py
+-rw-r--r--   0        0        0     1068 2022-07-28 15:27:13.984898 tibanna_ff-1.3.3/tibanna_cgap/lambdas/start_run.py
+-rw-r--r--   0        0        0      231 2021-11-18 14:02:19.688789 tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1285 2022-07-28 15:27:13.990793 tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     1281 2022-05-12 18:36:39.995036 tibanna_ff-1.3.3/tibanna_cgap/start_run.py
+-rw-r--r--   0        0        0      319 2021-08-18 20:28:06.339708 tibanna_ff-1.3.3/tibanna_cgap/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-09-22 18:05:42.586269 tibanna_ff-1.3.3/tibanna_cgap/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1098 2020-02-12 17:25:26.396103 tibanna_ff-1.3.3/tibanna_cgap/update_ffmeta.py
+-rw-r--r--   0        0        0     1106 2022-09-21 14:52:08.841665 tibanna_ff-1.3.3/tibanna_cgap/vars.py
+-rw-r--r--   0        0        0     6094 2021-11-01 16:47:18.100132 tibanna_ff-1.3.3/tibanna_cgap/zebra_utils.py
+-rw-r--r--   0        0        0        0 2020-02-12 17:25:26.396782 tibanna_ff-1.3.3/tibanna_ffcommon/__init__.py
+-rw-r--r--   0        0        0      504 2022-07-28 15:27:14.000802 tibanna_ff-1.3.3/tibanna_ffcommon/_version.py
+-rw-r--r--   0        0        0      677 2021-07-19 16:31:16.941336 tibanna_ff-1.3.3/tibanna_ffcommon/config.py
+-rw-r--r--   0        0        0     4090 2023-04-14 13:36:23.433794 tibanna_ff-1.3.3/tibanna_ffcommon/core.py
+-rw-r--r--   0        0        0     3796 2021-07-19 16:31:16.949528 tibanna_ff-1.3.3/tibanna_ffcommon/exceptions.py
+-rw-r--r--   0        0        0     2302 2021-07-19 16:31:16.949786 tibanna_ff-1.3.3/tibanna_ffcommon/extra_files.py
+-rw-r--r--   0        0        0     2171 2021-07-19 16:31:16.950054 tibanna_ff-1.3.3/tibanna_ffcommon/file_format.py
+-rw-r--r--   0        0        0     2019 2022-05-12 18:36:40.014086 tibanna_ff-1.3.3/tibanna_ffcommon/iam_utils.py
+-rw-r--r--   0        0        0    16981 2023-04-14 13:36:23.434318 tibanna_ff-1.3.3/tibanna_ffcommon/input_files.py
+-rw-r--r--   0        0        0    71687 2023-04-14 13:36:23.435112 tibanna_ff-1.3.3/tibanna_ffcommon/portal_utils.py
+-rw-r--r--   0        0        0    22791 2023-04-14 13:36:23.435831 tibanna_ff-1.3.3/tibanna_ffcommon/qc.py
+-rw-r--r--   0        0        0     3162 2021-08-18 20:28:06.348560 tibanna_ff-1.3.3/tibanna_ffcommon/stepfunction.py
+-rw-r--r--   0        0        0     3252 2023-04-14 13:36:23.436171 tibanna_ff-1.3.3/tibanna_ffcommon/vars.py
+-rw-r--r--   0        0        0     6499 2023-04-14 13:36:23.436523 tibanna_ff-1.3.3/tibanna_ffcommon/wfr.py
+-rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 tibanna_ff-1.3.3/setup.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 tibanna_ff-1.3.3/PKG-INFO
```

### Comparing `tibanna_ff-1.3.0b1/LICENSE.txt` & `tibanna_ff-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/pyproject.toml` & `tibanna_ff-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibanna_ff"
-version = "1.3.0b1"
+version = "1.3.3"
 description = "Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tibanna"]
 homepage = "http://github.com/4dn-dcic/tibanna_ff"
 repository = "http://github.com/4dn-dcic/tibanna_ff.git"
@@ -25,16 +25,16 @@
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
-tibanna = "3.0.1b0"
-dcicutils = "^6.0.0"
+tibanna = "^3.3.1"
+dcicutils = "^7.0.0"
 boto3 = "^1.9.0"
 botocore = "^1.12.1"
 requests = "2.27.1" # Pin version as 2.28.* currently leads to warnings then running cwltool
 tomlkit = "^0.11.0"
 
 [tool.poetry.dev-dependencies]
 invoke = "0.18.1"
```

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/__main__.py` & `tibanna_ff-1.3.3/tibanna_4dn/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/core.py` & `tibanna_ff-1.3.3/tibanna_4dn/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/start_run.py` & `tibanna_ff-1.3.3/tibanna_4dn/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/lambdas/update_ffmeta.py` & `tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/pony_utils.py` & `tibanna_ff-1.3.3/tibanna_4dn/pony_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/start_run.py` & `tibanna_ff-1.3.3/tibanna_4dn/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/stepfunction_cost_updater.py` & `tibanna_ff-1.3.3/tibanna_4dn/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/update_ffmeta.py` & `tibanna_ff-1.3.3/tibanna_4dn/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_4dn/vars.py` & `tibanna_ff-1.3.3/tibanna_4dn/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/__main__.py` & `tibanna_ff-1.3.3/tibanna_cgap/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/core.py` & `tibanna_ff-1.3.3/tibanna_cgap/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/start_run.py` & `tibanna_ff-1.3.3/tibanna_cgap/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/lambdas/update_ffmeta.py` & `tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/start_run.py` & `tibanna_ff-1.3.3/tibanna_cgap/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/stepfunction_cost_updater.py` & `tibanna_ff-1.3.3/tibanna_cgap/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/update_ffmeta.py` & `tibanna_ff-1.3.3/tibanna_cgap/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/vars.py` & `tibanna_ff-1.3.3/tibanna_cgap/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_cgap/zebra_utils.py` & `tibanna_ff-1.3.3/tibanna_cgap/zebra_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/config.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/config.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/core.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/exceptions.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/exceptions.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/extra_files.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/extra_files.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/file_format.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/file_format.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/iam_utils.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/iam_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/input_files.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/input_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     # do not modify them or access them directly, but use self.get_metadata
     # or self.fe_map or instead
     _metadata = dict()
     _fe_map = None
 
     def __init__(self, uuid=None, workflow_argument_name=None, object_key=None,
                  bucket_name=None, rename='', unzip='', mount=False,
-                 format_if_extra='', ff_key=None, ff_env=None):
+                 format_if_extra='', ff_key=None, ff_env=None, **kwargs):
         # uuid and workflow_argument_name are required
         if not uuid or not workflow_argument_name:
             raise MalFormattedFFInputException("malformed input, check input_files in your input json")
         self.uuid = uuid  # either a single value or a list
         self.workflow_argument_name = workflow_argument_name
         # here objct key means <accession>.<extension>
         self._object_key = object_key  # either a single value or a list
```

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/portal_utils.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/portal_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
     if isinstance(val, (list, tuple)):
         return val
     return [val]
 
 
 class TibannaSettings(SerializableObject):
 
-    def __init__(self, env=None, ff_keys=None, sbg_keys=None, settings=None):
+    def __init__(self, env=None, ff_keys=None, sbg_keys=None, settings=None, **kwargs):
         if not env:
             self.env = None
             self.s3 = None
             self.ff_keys = None
             self.settings = None
         else:
             logger.debug("Getting tibanna settings for env %s" % env)
```

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/qc.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class QCArgument(SerializableObject):
     """This is a class that represents a QC-type workflow argument which is a part of
     a workflow metadata
     """
     def __init__(self, argument_type, workflow_argument_name, argument_to_be_attached_to, qc_type=None,
                  qc_zipped=False, qc_html=False, qc_json=False, qc_table=False,
                  qc_zipped_html=None, qc_zipped_tables=None, qc_acl='public-read',
-                 qc_unzip_from_ec2=False):
+                 qc_unzip_from_ec2=False, **kwargs):
         if argument_type != 'Output QC file':
             raise Exception("QC Argument must be an Output QC file: %s" % argument_type)
         self.workflow_argument_name = workflow_argument_name
         self.argument_to_be_attached_to = argument_to_be_attached_to
         self.qc_type = qc_type  # qc metadata item type (e.g. quality_metric_fastqc)
         self.qc_zipped = qc_zipped
         self.qc_html = qc_html  # boolean, true if qc is unzipped html
```

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/stepfunction.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/stepfunction.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/vars.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.0b1/tibanna_ffcommon/wfr.py` & `tibanna_ff-1.3.3/tibanna_ffcommon/wfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 class InputFileForWFRMeta(object):
     """This class defines the structure of an input_file as part of
     the workflow_run metadata. It is a single element of an input file list
     defined in the InputFilesForWFRMeta class.
     """
     def __init__(self, workflow_argument_name=None, value=None, ordinal=None,
-                       format_if_extra=None, dimension=None):
+                       format_if_extra=None, dimension=None, **kwargs):
         """dimension is '0' for a singleton argument,
         '0', '1', '2' ... for a 1d-list argument,
         '0-0', '0-1', ... , '1-0', '1-1', ... for a 2d-list argument, and so on.
         ordinal is 1 for a singleton,
         1, 2, 3, 4, ... for an any-dimensional list argument.
         value (uuid for the input file) is never a list
         """
```

### Comparing `tibanna_ff-1.3.0b1/setup.py` & `tibanna_ff-1.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.9.0,<2.0.0',
  'botocore>=1.12.1,<2.0.0',
- 'dcicutils>=6.0.0,<7.0.0',
+ 'dcicutils>=7.0.0,<8.0.0',
  'requests==2.27.1',
- 'tibanna==3.0.1b0',
+ 'tibanna>=3.3.1,<4.0.0',
  'tomlkit>=0.11.0,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['tibanna_4dn = tibanna_4dn.__main__:main',
                      'tibanna_cgap = tibanna_cgap.__main__:main']}
 
 setup_kwargs = {
     'name': 'tibanna-ff',
-    'version': '1.3.0b1',
+    'version': '1.3.3',
     'description': 'Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.',
     'long_description': '# Tibanna_ff\n\nThis is an extension of Tibanna that integrates with 4DN/CGAP data portals.\n\n[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/) ![Build Status](https://travis-ci.com/4dn-dcic/tibanna_ff.svg?branch=master)\n\n\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://github.com/4dn-dcic/tibanna_ff',
```

### Comparing `tibanna_ff-1.3.0b1/PKG-INFO` & `tibanna_ff-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibanna-ff
-Version: 1.3.0b1
+Version: 1.3.3
 Summary: Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.
 Home-page: http://github.com/4dn-dcic/tibanna_ff
 License: MIT
 Keywords: tibanna
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.9
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: boto3 (>=1.9.0,<2.0.0)
 Requires-Dist: botocore (>=1.12.1,<2.0.0)
-Requires-Dist: dcicutils (>=6.0.0,<7.0.0)
+Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: requests (==2.27.1)
-Requires-Dist: tibanna (==3.0.1b0)
+Requires-Dist: tibanna (>=3.3.1,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.0,<0.12.0)
 Project-URL: Repository, http://github.com/4dn-dcic/tibanna_ff.git
 Description-Content-Type: text/markdown
 
 # Tibanna_ff
 
 This is an extension of Tibanna that integrates with 4DN/CGAP data portals.
```

