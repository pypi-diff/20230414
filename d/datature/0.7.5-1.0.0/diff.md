# Comparing `tmp/datature-0.7.5.tar.gz` & `tmp/datature-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-7pilbe7p/datature-0.7.5.tar", last modified: Wed Mar 22 08:05:53 2023, max compression
+gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-kbibbuc8/datature-1.0.0.tar", last modified: Fri Apr 14 09:08:20 2023, max compression
```

## Comparing `datature-0.7.5.tar` & `datature-1.0.0.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-03-22 08:05:39.000000 datature-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-22 08:05:39.000000 datature-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-22 08:05:53.000000 datature-0.7.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-22 08:05:39.000000 datature-0.7.5/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/datature/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-03-22 08:05:39.000000 datature-0.7.5/datature/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-03-22 08:05:39.000000 datature-0.7.5/datature/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-03-22 08:05:39.000000 datature-0.7.5/datature/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-03-22 08:05:39.000000 datature-0.7.5/datature/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-22 08:05:39.000000 datature-0.7.5/datature/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/datature/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-22 08:05:39.000000 datature-0.7.5/datature/http/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-22 08:05:39.000000 datature-0.7.5/datature/http/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-22 08:05:39.000000 datature-0.7.5/datature/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-22 08:05:39.000000 datature-0.7.5/datature/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-22 08:05:39.000000 datature-0.7.5/datature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-22 08:05:39.000000 datature-0.7.5/datature/processor/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-22 08:05:39.000000 datature-0.7.5/datature/processor/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-22 08:05:39.000000 datature-0.7.5/datature/processor/nii_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature/rest/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-22 08:05:39.000000 datature-0.7.5/datature/rest/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-22 08:05:53.000000 datature-0.7.5/datature.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-22 08:05:39.000000 datature-0.7.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 08:05:53.000000 datature-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-22 08:05:39.000000 datature-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/test/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-22 08:05:39.000000 datature-0.7.5/test/fixture/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/test/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/test/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-22 08:05:39.000000 datature-0.7.5/test/http/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 08:05:39.000000 datature-0.7.5/test/http/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:53.000000 datature-0.7.5/test/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-22 08:05:39.000000 datature-0.7.5/test/rest/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-22 08:05:39.000000 datature-0.7.5/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-22 08:05:39.000000 datature-0.7.5/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-14 09:08:09.000000 datature-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 09:08:09.000000 datature-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 09:08:20.000000 datature-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 09:08:09.000000 datature-1.0.0/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 09:08:09.000000 datature-1.0.0/datature/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-14 09:08:09.000000 datature-1.0.0/datature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-14 09:08:09.000000 datature-1.0.0/datature/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/nii_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/rest/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 09:08:09.000000 datature-1.0.0/datature/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-14 09:08:09.000000 datature-1.0.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:08:20.000000 datature-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 09:08:09.000000 datature-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 09:08:09.000000 datature-1.0.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 09:08:09.000000 datature-1.0.0/test/test_logger.py
```

### Comparing `datature-0.7.5/LICENSE` & `datature-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/PKG-INFO` & `datature-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 0.7.5
+Version: 1.0.0
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 
 ## Usage
 
 The library needs to be configured with your project's secret key which is available in your Project Dashboard `Advanced/API Management`
 
 ```python
 import datature
-datature.project_secret = "6874c3c9b..."
+datature.secret_key = "6874c3c9b..."
 
 # retrieve project
 project = datature.Project.retrieve()
 
 # print project information
 print(project)
```

### Comparing `datature-0.7.5/datature/__init__.py` & `datature-1.0.0/datature/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,33 +4,33 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   __init__.py
 @Author  :   Raighne.Weng
-@Version :   0.6.1
+@Version :   1.0.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   init module, include global configuration
 '''
 
 # Global Configuration
 API_BASE_URL = "https://api.datature.io/v1"
-SDK_VERSION = "0.7.5"
+SDK_VERSION = "1.0.0"
 
 # Constant environment
-OPERATION_LOOPING_TIMES = 8
+OPERATION_LOOPING_TIMES = 20
 ASSET_UPLOAD_BATCH_SIZE = 5000
 SHOW_PROGRESS = False
 OPERATION_LOOPING_DELAY_SECONDS = 5
 HTTP_TIMEOUT_SECONDS = 120
 
 # Set to either 'debug' or 'info'
 LOG_LEVEL = None
 
 # pylint: disable=C0103
-project_secret = None
+secret_key = None
 
 # API resources
 # pylint: disable=C0413
 from datature.rest import *
```

### Comparing `datature-0.7.5/datature/cli/commands.py` & `datature-1.0.0/datature/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI supported commands
 '''
 
 import sys
-from typing import Optional
 from argparse import ArgumentParser, _SubParsersAction
+from typing import Optional
+
 import datature
 
 
 # pylint: disable = R0903,R0914
 class Commands:
     """All Datature CLI commands."""
```

### Comparing `datature-0.7.5/datature/cli/config.py` & `datature-1.0.0/datature/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI config class
 '''
 
 import io
 import sys
+import base64
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
-import base64
+
 import yaml
-from datature.messages import NO_PROJECT_MESSAGE, INVALID_PROJECT_MESSAGE
+from datature.messages import INVALID_PROJECT_MESSAGE, NO_PROJECT_MESSAGE
 
 
 class Config():
     """Handles YAML configuration files"""
 
     def __init__(self):
         """Init config file"""
```

### Comparing `datature-0.7.5/datature/cli/functions.py` & `datature-1.0.0/datature/cli/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,38 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   functions.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   0.7.6
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI functions
 '''
 
-from typing import Optional
-from pathlib import Path
-from os.path import exists, isfile, basename, join
 import os
 import re
-import glob
-import time
 import sys
+import time
+from os.path import basename, exists, isfile, join
+from pathlib import Path
+from typing import Optional
+
 import inquirer
+import requests
 from halo import Halo
 from alive_progress import alive_bar
-import requests
+
 import datature
-from datature import error
-from datature import messages
+from datature.utils import utils
+from datature import error, messages
 from datature.cli.config import Config
-from datature.rest.types import (AnnotationFormat)
+from datature.rest.types import AnnotationFormat
 
 # pylint: disable=E1102
 
 ASSET_UPLOAD_BATCH_SIZE = datature.ASSET_UPLOAD_BATCH_SIZE
 datature.SHOW_PROGRESS = True
 
 if 'DATATURE_API_BASE_URL' in os.environ:
@@ -52,15 +53,15 @@
 
     project_secret = project_secret.strip()
     if project_secret == "":
         print(messages.AUTHENTICATION_REMINDER_MESSAGE)
         sys.exit(1)
 
     try:
-        datature.project_secret = project_secret
+        datature.secret_key = project_secret
         project = datature.Project.retrieve()
 
         project_name = project.get("name")
         project_id = project.get("id")
 
         default_project = inquirer.confirm(
             f"Make [{project_name}] the default project?", default=True)
@@ -106,15 +107,15 @@
 
     output = [[
         "NAME", "TOTAL_ASSETS", "ANNOTATED_ASSETS", "ANNOTATIONS", "TAGS"
     ]]
     for project_name in project_names:
         project = config.get_project_by_name(project_name)
         try:
-            datature.project_secret = project.get("project_secret")
+            datature.secret_key = project.get("project_secret")
             project = datature.Project.retrieve()
             asset_total = project.get("statistic").get("asset_total")
             asset_annotated = project.get("statistic").get("asset_annotated")
             annotation_total = project.get("statistic").get("annotation_total")
             tags = project.get("tags")
             output.append([
                 project_name, asset_total, asset_annotated, annotation_total,
@@ -164,35 +165,14 @@
             progress_bar(percentage)
             time.sleep(datature.OPERATION_LOOPING_DELAY_SECONDS)
         progress_bar(1.)
     print(messages.SERVER_COMPLETED_MESSAGE)
     datature.SHOW_PROGRESS = True
 
 
-def find_all_assets(path: Path) -> [str]:
-    """
-    List all assets under folder, include sub folder.
-
-    :param path: The folder to upload assets.
-    :return: assets path list.
-    """
-    default_file_exts = [
-        '*.jpg', '*.JPG', '*.png', '*.PNG', '*.jpeg', '*.JPEG', '*.mp4',
-        '*.MP4', "*.dcm", "*.DCM", '*.nii', '*.NII'
-    ]
-    file_paths = []
-
-    # find all assets under folder and sub folders
-    for file_ext in default_file_exts:
-        file_paths.extend(
-            glob.glob(os.path.join(path, '**', file_ext), recursive=True))
-
-    return file_paths
-
-
 def upload_assets(path: Optional[Path] = None, groups: Optional[str] = None):
     """
     Upload assets from path.
 
     :param path: The folder to upload assets.
     :return: None
     """
@@ -207,15 +187,15 @@
         path = answer.get("path_result")
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
 
     # find all images under folder and sub folders
-    file_paths = find_all_assets(path)
+    file_paths = utils.find_all_assets(path)
 
     if len(file_paths) == 0:
         print(messages.NO_ASSETS_FOUND_MESSAGE)
         sys.exit(1)
 
     nii_orientation = None
     if '.nii' in ",".join(str(file_path).lower() for file_path in file_paths):
@@ -328,32 +308,14 @@
         for data in resp.iter_content(chunk_size=1024):
             size = file.write(data)
             current_size += size
             progress_bar(float(current_size / total))
         progress_bar(1.0)
 
 
-def get_available_artifact_format(model_name: str):
-    """
-    Get available artifact format from model name.
-
-    :param model_name: The name of the model.
-    :return: [str]
-    """
-    switcher = {
-        "yolov4": ["tensorflow", "onnx"],
-        "mask": ["tensorflow", "onnx"],
-        "yolox": ["onnx"],
-        "deeplabv3": ["onnx"],
-        "unet": ["onnx"],
-    }
-    model_type = model_name.split("-")[0]
-    return switcher.get(model_type, ["tensorflow", "tflite", "onnx"])
-
-
 # pylint: disable=R0912,R0914
 def download_artifact(artifact_id: Optional[str] = None,
                       model_format: Optional[str] = None,
                       path: Optional[str] = None):
     """
     Download artifact model.
 
@@ -398,22 +360,20 @@
                 choices=artifact_lists,
             ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         artifact_key = answer.get("artifact")
         artifact = artifacts_key_map.get(artifact_key)
 
-    model_type = get_available_artifact_format(artifact.get("model_name"))
-
     if not model_format:
         questions = [
             inquirer.List(
                 "model_format",
                 message=messages.ARTIFACT_MODEL_FORMAT_DOWNLOAD_MESSAGE,
-                choices=model_type,
+                choices=artifact.get("exportable_formats", []),
             ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         model_format = answer.get("model_format")
 
     if model_format in artifact.get("exports"):
         # already exported, can download directly
@@ -505,15 +465,15 @@
     operation = datature.Annotation.export(annotation_format,
                                            export_options={
                                                "normalized": normalized,
                                                "shuffle": shuffle,
                                                "split_ratio": split_ratio,
                                                "seed": 1337
                                            },
-                                           early_return=False)
+                                           background=False)
 
     annotation = datature.Annotation.retrieve_exported_file(
         operation.get("id"))
     wait_spinner.stop()
     download_file_from_link(annotation.get("download").get("url"), path)
```

### Comparing `datature-0.7.5/datature/cli/main.py` & `datature-1.0.0/datature/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 @Version :   0.7.1
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI main entrance
 '''
 
 import sys
+
 import datature
 from datature import messages
-from datature.cli.commands import Commands
 from datature.cli import functions
+from datature.cli.commands import Commands
 from datature.cli.config import Config
-from datature.error import ForbiddenError, ErrorWithCode
+from datature.error import ErrorWithCode, ForbiddenError
 
 
 # pylint: disable=R0912,R0915
 def main() -> None:
     """
     Executes the main function of cli.
 
@@ -49,15 +50,15 @@
             config = Config()
             project = config.get_default_project()
             if not project:
                 print(messages.NO_PROJECT_MESSAGE)
                 sys.exit(1)
 
             # Set project secret
-            datature.project_secret = project.get("project_secret")
+            datature.secret_key = project.get("project_secret")
 
             if args.command == "asset":
                 if args.action == "upload":
                     functions.upload_assets(args.path, args.groups)
                 elif args.action == "group":
                     functions.assets_group(args.group)
                 else:
```

### Comparing `datature-0.7.5/datature/error.py` & `datature-1.0.0/datature/error.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/http/requester.py` & `datature-1.0.0/datature/http/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   A wrapper to make HTTP requests
 '''
 
 import json
 from urllib.parse import urlencode
+
 import humps
-from requests import request, Response
-from datature import error, logger
+from requests import Response, request
+
 import datature
+from datature import error, logger
 
 
 # pylint: disable=R0913,R0903
 class Requester():
     """An HTTP requester."""
 
     def request(self,
@@ -39,19 +41,19 @@
         :param url: The request url
         :param query: The query object
         :param request_body: The request body
         :param request_headers: If have custom request headers
         :param request_files: If have file to upload
         """
 
-        # CHeck Project-Secret
-        if datature.project_secret is None:
+        # CHeck Secret
+        if datature.secret_key is None:
             raise error.UnauthorizedError(
-                "No project secret key provided. (Set your project secret key"
-                " using datature.project_secret = <project_secret>)")
+                "No project secret key provided. (Set your secret key"
+                " using datature.secret_key = <secret_key>)")
 
         absolute_url = f"{datature.API_BASE_URL}{url}"
 
         # Assemble queries and request body.
         post_data = None
         post_files = None
 
@@ -98,15 +100,15 @@
     def _make_headers(self, method, request_headers):
         """Make request headers
 
         :param method: The request method
         :param request_headers: The custom request headers
         """
         headers = {
-            "Project-Secret": datature.project_secret,
+            "Secret-Key": datature.secret_key,
         }
 
         if method in ["POST", "PUT"]:
             headers["Content-Type"] = "application/json"
 
         if request_headers is not None:
             for key, value in request_headers.items():
```

### Comparing `datature-0.7.5/datature/http/resource.py` & `datature-1.0.0/datature/http/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 @Version :   0.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Base class for REST API resources
 '''
 
 from halo import Halo
+
+import datature
 from datature.http.requester import Requester
 from datature.messages import REQUEST_SERVER_MESSAGE
-import datature
 
 
 # pylint: disable=R0913,R0903
 class RESTResource():
     """Datature REST resource."""
 
     @classmethod
```

### Comparing `datature-0.7.5/datature/logger.py` & `datature-1.0.0/datature/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   logger module
 '''
 
 import sys
 import logging
+
 import datature
 
 logger = logging.getLogger("datature")
 
 
 def _console_log_level():
     """Get log level"""
```

### Comparing `datature-0.7.5/datature/messages.py` & `datature-1.0.0/datature/messages.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/processor/__init__.py` & `datature-1.0.0/datature/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/processor/base_processor.py` & `datature-1.0.0/datature/processor/base_processor.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/processor/dicom_processor.py` & `datature-1.0.0/datature/processor/dicom_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 @Author  :   Raighne.Weng
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Dicom Processor
 '''
 
-from os.path import exists, join
-from os import makedirs
-from pathlib import Path
 import tempfile
+from pathlib import Path
+from os import makedirs, path
+
 import cv2
-from pydicom import dcmread, config
+from pydicom import config, dcmread
+
 from datature import error
 from datature.processor.base_processor import BaseProcessor
 
 # Enforcing Valid DICOM
 config.settings.reading_validation_mode = config.RAISE
 
 
@@ -49,17 +50,17 @@
         :return: str: The generate video path.
         """
         out_path = tempfile.mkdtemp()
         file_path = request_data.get("file")
 
         file_name = Path(file_path).stem
 
-        video_output = join(out_path, file_name)
+        video_output = path.join(out_path, file_name)
 
-        if not exists(video_output):
+        if not path.exists(video_output):
             makedirs(video_output)
 
         dicom_data = dcmread(file_path)
 
         four_cc = cv2.VideoWriter_fourcc(*'avc1')
 
         number_of_frames = int(dicom_data.get('NumberOfFrames', 1))
```

### Comparing `datature-0.7.5/datature/processor/nii_processor.py` & `datature-1.0.0/datature/processor/nii_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Nii Processor
 '''
 
 import tempfile
-from os.path import exists, join
-from os import makedirs
+from os import makedirs, path
 from pathlib import Path
+
 import cv2
 import numpy as np
 import nibabel as nib
 from datature import error
 from datature.processor.base_processor import BaseProcessor
 
 
@@ -56,17 +56,17 @@
         out_path = tempfile.mkdtemp()
 
         file_path = request_data.get("file")
         direction = request_data.get("options").get("direction")
 
         file_name = Path(file_path).stem
 
-        video_output = join(out_path, file_name)
+        video_output = path.join(out_path, file_name)
 
-        if not exists(video_output):
+        if not path.exists(video_output):
             makedirs(video_output)
 
         scan = nib.load(file_path)
 
         # Read data and get scan's shape
         scan_array = scan.get_fdata()
         scan_array_shape = scan_array.shape
```

### Comparing `datature-0.7.5/datature/rest/__init__.py` & `datature-1.0.0/datature/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/rest/annotation.py` & `datature-1.0.0/datature/rest/annotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 @Version :   0.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API
 '''
 
 from os.path import exists
+
 from datature.error import Error
 from datature.http.resource import RESTResource
 from datature.rest.operation import Operation
-from datature.rest.types import (AnnotationFormat, AnnotationMetadata,
-                                 AnnotationExportOptions)
+from datature.rest.types import (AnnotationExportOptions, AnnotationFormat,
+                                 AnnotationMetadata)
 
 
 class Annotation(RESTResource):
     """Datature Annotation API Resource."""
 
     @classmethod
     def list(cls, asset_id: str) -> dict:
@@ -69,20 +70,20 @@
         """
         return cls.request("DELETE", f"/annotation/{annotation_id}")
 
     @classmethod
     def export(cls,
                annotation_format: AnnotationFormat,
                export_options: AnnotationExportOptions,
-               early_return=True) -> dict:
+               background=False) -> dict:
         """Export all annotations
 
         :param annotation_format: the format of annotation
         :param export_options: the options of export
-        :param early_return: if need wait server process
+        :param background: complete upload process in the background
         :return: response json data
         """
         response = cls.request("POST",
                                "/annotation/export",
                                query={"format": annotation_format},
                                request_body={
                                    "options": {
@@ -93,15 +94,15 @@
                                        "normalized":
                                        export_options.get("normalized"),
                                        "shuffle":
                                        export_options.get("shuffle")
                                    }
                                })
 
-        if early_return:
+        if background:
             return response
 
         op_link = response["op_link"]
         return Operation.loop_retrieve(op_link)
 
     @classmethod
     def retrieve_exported_file(cls, op_id: str) -> dict:
@@ -112,21 +113,21 @@
         """
         return cls.request("GET", f"/annotation/export/{op_id}")
 
     @classmethod
     def upload(cls,
                annotation_format: AnnotationFormat,
                file_path: str,
-               early_return=True) -> dict:
+               background=False) -> dict:
         """Import annotations
 
 
         :param annotation_format: the format of annotation
         :param file_path: the path of imported file
-        :param early_return: if need wait server process
+        :param background: complete upload process in the background
         :return: response json data
         """
         file_exists = exists(file_path)
 
         if not file_exists:
             raise Error("Could not find the Asset file")
 
@@ -136,12 +137,12 @@
             response = cls.request(
                 "POST",
                 "/annotation/import",
                 query={"format": annotation_format},
                 request_files=files,
             )
 
-            if early_return:
+            if background:
                 return response
 
             op_link = response["op_link"]
             return Operation.loop_retrieve(op_link)
```

### Comparing `datature-0.7.5/datature/rest/artifact.py` & `datature-1.0.0/datature/rest/artifact.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/rest/asset/asset.py` & `datature-1.0.0/datature/rest/asset/asset.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,23 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   asset.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   0.7.6
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API
 '''
 
 from datature.http.resource import RESTResource
 from datature.rest.asset.upload_session import UploadSession
-from datature.rest.types import Pagination, AssetMetadata
+from datature.rest.types import AssetMetadata, Pagination
 
 
 class Asset(RESTResource):
     """Datature Annotation API Resource."""
 
     @classmethod
     def list(cls, pagination: Pagination = None) -> dict:
@@ -28,42 +28,49 @@
 
         :param pagination: the pagination of return list
         :return: response json data
         """
         return cls.request("GET", "/asset/list", query=pagination)
 
     @classmethod
-    def retrieve(cls, asset_id: str) -> dict:
+    def retrieve(cls, asset_id_or_name: str) -> dict:
         """Get an asset
 
-        :param asset_id: the id of asset
+        :param asset_id_or_name: the id or name of the asset
         :return: response json data
         """
-        return cls.request("GET", f"/asset/{asset_id}")
+        return cls.request("GET", f"/asset/{asset_id_or_name}")
 
     @classmethod
-    def modify(cls, asset_id: str, asset_meta: AssetMetadata) -> dict:
+    def modify(cls, asset_id_or_name: str, asset_meta: AssetMetadata) -> dict:
         """Update an asset
 
-        :param asset_id: the id of asset
+        :param asset_id_or_name: the id or name of the asset
         :param asset_meta: the metadata of asset
         :return: response json data
         """
+        request_body = {}
+        if asset_meta.get("status") is not None:
+            request_body["status"] = asset_meta.get("status")
+
+        if asset_meta.get("custom_metadata") is not None:
+            request_body["customMetadata"] = asset_meta.get("custom_metadata")
+
         return cls.request("PUT",
-                           f"/asset/{asset_id}",
-                           request_body=asset_meta)
+                           f"/asset/{asset_id_or_name}",
+                           request_body=request_body)
 
     @classmethod
-    def delete(cls, asset_id: str) -> dict:
+    def delete(cls, asset_id_or_name: str) -> dict:
         """Delete a asset
 
-        :param asset_id: the id of asset
+        :param asset_id_or_name: the id or name of the asset
         :return: response json data
         """
-        return cls.request("DELETE", f"/asset/{asset_id}")
+        return cls.request("DELETE", f"/asset/{asset_id_or_name}")
 
     @classmethod
     def upload_session(cls) -> dict:
         """Bulk update assets
 
         :return: UploadSession class
         """
```

### Comparing `datature-0.7.5/datature/rest/asset/upload_session.py` & `datature-1.0.0/datature/rest/asset/upload_session.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,54 +4,62 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload_session.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   0.7.6
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session
 '''
 
-import os
+import json
 import struct
-from os.path import exists
+from os import path
 from pathlib import Path
-from requests import request
+
+import cv2
 import google_crc32c
+from requests import request
 from filetype import filetype
-import cv2
 from alive_progress import alive_bar
+
 import datature
+from datature.utils import utils
 from datature import error, logger
 from datature.http.resource import RESTResource
-from datature.rest.operation import Operation
 from datature.processor import get_processor
+from datature.rest.operation import Operation
 
 
-# pylint: disable=E1102,R0914
+# pylint: disable=E1102,R0914,R0912
 class UploadSession(RESTResource):
     """Datature Asset Upload Session Class."""
 
     def __init__(self):
         self.assets = []
         self.file_name_map = {}
+        self.custom_metadata_map = {}
+        project = datature.Project.retrieve()
 
-    def add(self, file_path: str, **kwargs):
+        self.metadata_limit = utils.get_asset_metadata_limit_by_tier(
+            project.get("tier", "free"))
+
+    def add(self, file_path: str, custom_metadata: dict = None, **kwargs):
         """Add asset to upload."""
         if len(self.assets) >= datature.ASSET_UPLOAD_BATCH_SIZE:
             raise error.Error("One upload session allow max 5000 assets.")
 
-        if not exists(file_path):
+        if not path.exists(file_path):
             raise error.Error("Cannot find the Asset file")
 
         # Prepare filename size and mime type
-        filename = os.path.basename(file_path)
+        filename = path.basename(file_path)
 
         # Convert DICOM and NII file to video asset
         if file_path.lower().endswith(('.dcm', '.nii')):
             processor = get_processor(file_path)
 
             process_data = {"file": file_path, "options": kwargs}
             processor.valid(process_data)
@@ -68,28 +76,28 @@
             # calculate file crc32
             file_hash = google_crc32c.Checksum()
             file_hash.update(contents)
 
             # To fix the wrong crc32 caused by mac M1 clip
             crc32 = struct.unpack(">l", file_hash.digest())[0]
 
-            size = os.path.getsize(file_path)
+            size = path.getsize(file_path)
 
             mime_kind = filetype.guess(file_path)
 
             file.close()
 
             if self.file_name_map.get(filename) is not None:
                 raise error.Error(
                     f"Cannot add multiple files with the same name, {filename}"
                 )
 
             if (filename and size and crc32 and mime_kind):
                 if mime_kind.mime in ["image/jpeg", "image/png"]:
-                    metadata = {
+                    asset_metadata = {
                         "filename": filename,
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime
                     }
                 elif mime_kind.mime == "video/mp4":
                     cap = cv2.VideoCapture(file_path)
@@ -98,54 +106,68 @@
                     codec = chr(four_c_c
                                 & 0xff) + chr((four_c_c >> 8) & 0xff) + chr(
                                     (four_c_c >> 16)
                                     & 0xff) + chr((four_c_c >> 24) & 0xff)
                     if not codec.startswith('avc1'):
                         raise error.Error("UnSupported asset file")
 
-                    metadata = {
+                    asset_metadata = {
                         "filename": filename,
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime,
                         "frames": frames,
                         "encoder": {
                             "profile": "h264Saver",
                             "everyNthFrame": 1
                         },
                     }
                 else:
                     raise error.Error("UnSupported asset file")
 
-                self.assets.append(metadata)
+                self.assets.append(asset_metadata)
                 self.file_name_map[filename] = {"path": file_path}
 
-                logger.log_info("Add asset:", metadata=metadata)
+                if custom_metadata is not None:
+                    if len(json.dumps(custom_metadata)) > self.metadata_limit:
+                        raise error.Error(
+                            f"Your tier only allow upload {self.metadata_limit} bytes metadata."
+                        )
+
+                    self.custom_metadata_map[filename] = custom_metadata
+
+                logger.log_info("Add asset:", metadata=asset_metadata)
             else:
                 raise error.Error("UnSupported asset file")
 
-    def start(self, groups: [str] = None, early_return=True) -> dict:
+    def start(self, groups: [str] = None, background: bool = False) -> dict:
         """Request server to get signed ur and upload file to gcp."""
 
         # Set default groups
         if groups is None:
             groups = ["main"]
 
         # check asset length
         if not self.assets:
             raise error.Error("Assets to upload is empty")
 
+        if self.custom_metadata_map and background:
+            logger.log_info(
+                "Warning: have custom metadata, force set background to False."
+            )
+            datature.SHOW_PROGRESS = False
+            background = False
+
         # call API to get signed url
         response = self.request("POST",
                                 "/asset/uploadSession",
                                 request_body={
                                     "groups": groups,
                                     "assets": self.assets
                                 })
-
         op_link = response["op_link"]
 
         if datature.SHOW_PROGRESS:
             with alive_bar(
                     len(response["assets"]),
                     title='Uploading',
                     title_length=12,
@@ -180,11 +202,21 @@
                 request("PUT",
                         asset_upload["upload"]["url"],
                         headers=asset_upload["upload"]["headers"],
                         data=contents,
                         timeout=10)
                 logger.log_info("Done Uploading" + file_path)
 
-        if early_return:
+        if background:
             return {"op_link": op_link}
 
-        return Operation.loop_retrieve(op_link)
+        # Wait server finish generate thumbnail
+        Operation.loop_retrieve(op_link)
+
+        # Update custom_metadata
+        for filename in self.custom_metadata_map:
+            datature.Asset.modify(filename, {
+                "custom_metadata":
+                self.custom_metadata_map.get(filename, {})
+            })
+
+        return {"op_link": op_link}
```

### Comparing `datature-0.7.5/datature/rest/deploy.py` & `datature-1.0.0/datature/rest/deploy.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/rest/operation.py` & `datature-1.0.0/datature/rest/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 @Version :   0.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation API
 '''
 
 import time
-from datature.http.resource import RESTResource
-from datature import error, logger
+
 import datature
+from datature import error, logger
+from datature.http.resource import RESTResource
 
 
 class Operation(RESTResource):
     """Datature Operation API Resource."""
 
     @classmethod
     def retrieve(cls, op_link: str) -> dict:
```

### Comparing `datature-0.7.5/datature/rest/project.py` & `datature-1.0.0/datature/rest/project.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/datature/rest/run.py` & `datature-1.0.0/datature/rest/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @File    :   run.py
 @Author  :   Raighne.Weng
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Run API
 '''
+
 from datature.http.resource import RESTResource
 from datature.rest.types import RunSetupMetadata
 
 
 class Run(RESTResource):
     """Datature Run API Resource."""
```

### Comparing `datature-0.7.5/datature/rest/tag.py` & `datature-1.0.0/datature/rest/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @File    :   tag.py
 @Author  :   Raighne.Weng
 @Version :   0.2.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Tag API
 '''
+
 from datature.http.resource import RESTResource
 
 
 class Tag(RESTResource):
     """Datature Tag API Resource."""
 
     @classmethod
```

### Comparing `datature-0.7.5/datature/rest/types.py` & `datature-1.0.0/datature/rest/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 @Author  :   Raighne.Weng
 @Version :   0.7.2
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Types for Datature API resources.
 '''
 
-from dataclasses import dataclass
 from enum import Enum
+from dataclasses import dataclass
 
 
 @dataclass
 class ProjectMetadata:
     """Project metadata."""
 
     name: str
@@ -54,14 +54,15 @@
 
 
 @dataclass
 class AssetMetadata:
     """Asset Metadata."""
 
     status: str
+    custom_metadata: object
 
 
 class AnnotationFormat(Enum):
     """Annotation CSV Format."""
 
     CSV_FOURCORNER = "csv_fourcorner"
     CSV_WIDTHHEIGHT = "csv_widthheight"
```

### Comparing `datature-0.7.5/datature/rest/workflow.py` & `datature-1.0.0/datature/rest/workflow.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 @Author  :   Raighne.Weng
 @Version :   0.3.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Workflow API
 '''
 
-from datature.http.resource import RESTResource
 from datature.rest.types import FlowMetadata
+from datature.http.resource import RESTResource
 
 
 class Workflow(RESTResource):
     """Datature Workflow API Resource."""
 
     @classmethod
     def list(cls) -> dict:
```

### Comparing `datature-0.7.5/datature.egg-info/PKG-INFO` & `datature-1.0.0/datature.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 0.7.5
+Version: 1.0.0
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 
 ## Usage
 
 The library needs to be configured with your project's secret key which is available in your Project Dashboard `Advanced/API Management`
 
 ```python
 import datature
-datature.project_secret = "6874c3c9b..."
+datature.secret_key = "6874c3c9b..."
 
 # retrieve project
 project = datature.Project.retrieve()
 
 # print project information
 print(project)
```

### Comparing `datature-0.7.5/datature.egg-info/SOURCES.txt` & `datature-1.0.0/datature.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 datature/rest/run.py
 datature/rest/tag.py
 datature/rest/types.py
 datature/rest/workflow.py
 datature/rest/asset/__int__.py
 datature/rest/asset/asset.py
 datature/rest/asset/upload_session.py
+datature/utils/__init__.py
+datature/utils/utils.py
 test/__init__.py
 test/test_error.py
 test/test_logger.py
 test/fixture/__init__.py
 test/fixture/mock.py
 test/fixture/data/__init__.py
 test/fixture/data/error_fixture.py
```

### Comparing `datature-0.7.5/readme.md` & `datature-1.0.0/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 The library needs to be configured with your project's secret key which is available in your Project Dashboard `Advanced/API Management`
 
 ```python
 import datature
-datature.project_secret = "6874c3c9b..."
+datature.secret_key = "6874c3c9b..."
 
 # retrieve project
 project = datature.Project.retrieve()
 
 # print project information
 print(project)
```

### Comparing `datature-0.7.5/setup.py` & `datature-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/fixture/data/error_fixture.py` & `datature-1.0.0/test/fixture/data/error_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/fixture/data/operation_fixture.py` & `datature-1.0.0/test/fixture/data/operation_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/fixture/data/upload_session_fixture.py` & `datature-1.0.0/test/fixture/data/upload_session_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/fixture/mock.py` & `datature-1.0.0/test/fixture/mock.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/http/test_requester.py` & `datature-1.0.0/test/http/test_requester.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 from datature.error import (ForbiddenError, NotFoundError,
                             TooManyRequestsError, InternalServerError,
                             UnauthorizedError)
 import datature
 
 
 class TestRequester(unittest.TestCase):
-    """Datature HTTP Resource Teset Cases."""
+    """Datature HTTP Resource Test Cases."""
 
     def test_request_with_no_project_key(self):
         """Test resource request."""
 
-        datature.project_secret = None
+        datature.secret_key = None
         try:
             # pylint: disable=W0212
             Requester().request("GET", "test_end_poimt")
         # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, UnauthorizedError)
 
     @patch("datature.http.requester.request")
     def test_request_with_query(self, patch_request):
         """Test resource request."""
 
-        datature.project_secret = "project_secret"
+        datature.secret_key = "project_secret"
 
         patch_request.return_value = MockResponse(
             operation_fixture.pending_operation_response, 200)
 
         # pylint: disable=W0212
         response = Requester().request("GET",
                                        "test_end_poimt",
@@ -55,58 +55,58 @@
                                        request_body={"key": "value"})
         assert response == operation_fixture.pending_operation_response
 
     @patch("datature.http.requester.request")
     def test_request_with_request_files(self, patch_request):
         """Test resource request with request files."""
 
-        datature.project_secret = "project_secret"
+        datature.secret_key = "project_secret"
 
         patch_request.return_value = MockResponse(
             operation_fixture.pending_operation_response, 200)
 
         # pylint: disable=W0212
         response = Requester().request("POST",
                                        "test_end_poimt",
                                        request_files="FileObject")
         assert response == operation_fixture.pending_operation_response
 
     def test_make_headers_with_get_method(self):
         """Test make headers."""
 
-        datature.project_secret = "project_secret"
+        datature.secret_key = "project_secret"
         # pylint: disable=W0212
         headers = Requester()._make_headers("GET", {})
 
-        assert headers == {"Project-Secret": "project_secret"}
+        assert headers == {"Secret-Key": "project_secret"}
 
     def test_make_headers_with_post_method(self):
         """Test make headers with post method."""
 
-        datature.project_secret = "project_secret"
+        datature.secret_key = "project_secret"
         # pylint: disable=W0212
         headers = Requester()._make_headers("POST", {})
 
         assert headers == {
-            "Project-Secret": "project_secret",
+            "Secret-Key": "project_secret",
             "Content-Type": "application/json"
         }
 
     def test_make_headers_with_supplied_headers(self):
         """Test make headers with supplied headers."""
 
-        datature.project_secret = "project_secret"
+        datature.secret_key = "project_secret"
         # pylint: disable=W0212
         headers = Requester()._make_headers("GET", {
             "Connection": "keep-alive",
             "Accept": "*/*"
         })
 
         assert headers == {
-            "Project-Secret": "project_secret",
+            "Secret-Key": "project_secret",
             "Connection": "keep-alive",
             "Accept": "*/*"
         }
 
     def test_interpret_response_with_403(self):
         """Test interpret response with 403 code."""
```

### Comparing `datature-0.7.5/test/http/test_resource.py` & `datature-1.0.0/test/http/test_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import unittest
 from unittest.mock import patch
 from datature.http.resource import RESTResource
 
 
 class TestResource(unittest.TestCase):
-    """Datature HTTP Resource Teset Cases."""
+    """Datature HTTP Resource Test Cases."""
 
     @patch("datature.http.resource.Requester")
     def test_request(self, patch_requester):
         """Test resource request."""
 
         RESTResource.request("GET", "/test_end_point")
```

### Comparing `datature-0.7.5/test/rest/test_annotation.py` & `datature-1.0.0/test/rest/test_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from test.fixture.mock import MockResponse
 from test.fixture.data import operation_fixture
 from datature.rest.annotation import Annotation
 from datature.error import Error
 
 
 class TestAnnotation(unittest.TestCase):
-    """Datature Annotation API Resource Teset Cases."""
+    """Datature Annotation API Resource Test Cases."""
 
     def test_list(self):
         """Test retrieve a list of annotations."""
         Annotation.request = MagicMock()
 
         Annotation.list("asset_id")
 
@@ -80,47 +80,47 @@
         Annotation.request = MagicMock()
 
         Annotation.delete("annotation_id")
 
         Annotation.request.assert_called_once_with(
             "DELETE", "/annotation/annotation_id")
 
-    def test_export(self):
+    def test_export_with_background(self):
         """Test export annotations."""
         Annotation.request = MagicMock()
 
         Annotation.export("csv_fourcorner",
                           export_options={
                               "split_ratio": 0.4,
                               "seed": 1337,
-                          })
+                          },
+                          background=True)
         Annotation.request.assert_called_once_with(
             "POST",
             "/annotation/export",
             query={"format": "csv_fourcorner"},
             request_body={
                 "options": {
                     "splitRatio": 0.4,
                     "seed": 1337,
                     "normalized": None,
                     "shuffle": None
                 }
             })
 
     @patch("datature.rest.annotation.Operation")
-    def test_export_with_no_early_return(self, operation):
+    def test_export(self, operation):
         """Test export annotations."""
         Annotation.request = MagicMock()
 
         Annotation.export("csv_fourcorner",
                           export_options={
                               "split_ratio": 0.4,
                               "seed": 1337,
-                          },
-                          early_return=False)
+                          })
         Annotation.request.side_effect = MockResponse(
             operation_fixture.pending_operation_response, 200)
 
         operation.loop_retrieve.assert_called()
 
     def test_retrieve_exported_file(self):
         """Test get export annotations."""
@@ -152,21 +152,21 @@
         patch_exist.return_value = True
         patch_open = MagicMock()
         patch_open.side_effect = True
 
         Annotation.request.side_effect = [
             operation_fixture.pending_operation_response
         ]
-        Annotation.upload("csv_fourcorner", "pathPath", early_return=False)
+        Annotation.upload("csv_fourcorner", "pathPath")
 
         operation.loop_retrieve.assert_called()
 
     @patch("datature.rest.annotation.exists")
     @patch("datature.rest.annotation.open")
-    def test_upload_with_file_early_return(
+    def test_upload_with_file_background(
         self,
         patch_open,
         patch_exist,
     ):
         """Test import annotation with file exist."""
 
         Annotation.request = MagicMock()
@@ -175,9 +175,9 @@
         patch_open = MagicMock()
         patch_open.side_effect = True
 
         Annotation.request.side_effect = [
             operation_fixture.pending_operation_response
         ]
         assert Annotation.upload(
-            "csv_fourcorner",
-            "pathPath") == operation_fixture.pending_operation_response
+            "csv_fourcorner", "pathPath",
+            background=True) == operation_fixture.pending_operation_response
```

### Comparing `datature-0.7.5/test/rest/test_artifact.py` & `datature-1.0.0/test/rest/test_artifact.py`

 * *Files identical despite different names*

### Comparing `datature-0.7.5/test/rest/test_asset.py` & `datature-1.0.0/test/rest/test_asset.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 @Version :   0.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API Test Cases
 '''
 
 import unittest
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, patch
 from datature.rest.asset.asset import Asset
 from datature.rest.asset.upload_session import UploadSession
 
 
+# pylint: disable=W0613
 class TestAsset(unittest.TestCase):
-    """Datature Asset API Resource Teset Cases."""
+    """Datature Asset API Resource Test Cases."""
 
     def test_list(self):
         """Test retrieve a list of assets."""
         Asset.request = MagicMock()
 
         Asset.list()
 
@@ -57,23 +58,33 @@
         Asset.request = MagicMock()
 
         Asset.modify("asset_id", {"status": "status"})
 
         Asset.request.assert_called_once_with(
             "PUT", "/asset/asset_id", request_body={"status": "status"})
 
+    def test_modify_custom_metadata(self):
+        """Test update an asset custom metadata."""
+        Asset.request = MagicMock()
+
+        Asset.modify("asset_id", {"custom_metadata": "s"})
+
+        Asset.request.assert_called_once_with(
+            "PUT", "/asset/asset_id", request_body={"customMetadata": "s"})
+
     def test_delete(self):
         """Test delete an asset."""
         Asset.request = MagicMock()
 
         Asset.delete("asset_id")
 
         Asset.request.assert_called_once_with("DELETE", "/asset/asset_id")
 
-    def test_upload_session(self):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_upload_session(self, patch_datature):
         """Test create Asset."""
         upload_session = Asset.upload_session()
         assert isinstance(upload_session, UploadSession)
 
     def test_group(self):
         """Test retrieve assets statistic."""
         Asset.request = MagicMock()
```

### Comparing `datature-0.7.5/test/rest/test_asset_upload_session.py` & `datature-1.0.0/test/rest/test_asset_upload_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,167 +13,172 @@
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock, patch
 from test.fixture.data import upload_session_fixture
-from datature.rest.asset.upload_session import UploadSession
+
 from datature.error import Error
+from datature.rest.asset.upload_session import UploadSession
 
 
+# pylint: disable=W0613,R0913,C0103,W0703
 class TestAssetUploadSession(unittest.TestCase):
-    """Datature Asset Upload Session API Resource Teset Cases."""
+    """Datature Asset Upload Session API Resource Test Cases."""
 
-    def test_add_with_file_not_exist(self):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_add_with_file_not_exist(self, patch_datature):
         """Test add asset to upload with ."""
+        patch_datature.ASSET_UPLOAD_BATCH_SIZE = 100
+
         upload_session = UploadSession()
         try:
             upload_session.add("assetPath")
-        # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.rest.asset.upload_session.filetype")
-    @patch("datature.rest.asset.upload_session.os")
     @patch("datature.rest.asset.upload_session.struct")
     @patch("datature.rest.asset.upload_session.google_crc32c")
-    @patch("datature.rest.asset.upload_session.exists")
+    @patch("datature.rest.asset.upload_session.path")
     @patch("datature.rest.asset.upload_session.open")
-    # pylint: disable=W0613,R0913,C0103
-    def test_add_with_duplicated_file(self, patch_open, patch_exist,
-                                      google_crc32c, struct, os, filetype):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_add_with_duplicated_file(self, patch_datature, patch_open,
+                                      patch_path, google_crc32c, struct,
+                                      filetype):
         """Test add asset to upload with duplicated file."""
+        patch_datature.ASSET_UPLOAD_BATCH_SIZE = 100
+
         upload_session = UploadSession()
         upload_session.file_name_map = {"assetName": {"path": "file_path"}}
 
         struct.unpack.return_value = [-384617082]
-        os.path.basename.return_value = "assetName"
-        os.path.getsize.return_value = 5613
+        patch_path.basename.return_value = "assetName"
+        patch_path.getsize.return_value = 5613
 
         mock_guess = MagicMock()
         mock_guess.mime = "image/jpeg"
         filetype.guess.return_value = mock_guess
 
         try:
             upload_session.add("assetPath")
-        # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.rest.asset.upload_session.filetype")
-    @patch("datature.rest.asset.upload_session.os")
+    @patch("datature.rest.asset.upload_session.path")
     @patch("datature.rest.asset.upload_session.struct")
     @patch("datature.rest.asset.upload_session.google_crc32c")
-    @patch("datature.rest.asset.upload_session.exists")
     @patch("datature.rest.asset.upload_session.open")
-    # pylint: disable=W0613,R0913,C0103
-    def test_add_with_file_not_supported(self, patch_open, patch_exist,
-                                         google_crc32c, struct, os, filetype):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_add_with_file_not_supported(self, patch_datature, patch_open,
+                                         google_crc32c, struct, path,
+                                         filetype):
         """Test add asset to upload with file not supported."""
+        patch_datature.ASSET_UPLOAD_BATCH_SIZE = 100
+
         upload_session = UploadSession()
 
         struct.unpack.return_value = [-384617082]
-        os.path.basename.return_value = "assetName"
-        os.path.getsize.return_value = 5613
+        path.basename.return_value = "assetName"
+        path.getsize.return_value = 5613
 
         mock_guess = MagicMock()
         mock_guess.mime = ""
         filetype.guess.return_value = mock_guess
 
         try:
             upload_session.add("assetPath")
-        # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.rest.asset.upload_session.filetype")
-    @patch("datature.rest.asset.upload_session.os")
+    @patch("datature.rest.asset.upload_session.path")
     @patch("datature.rest.asset.upload_session.struct")
     @patch("datature.rest.asset.upload_session.google_crc32c")
-    @patch("datature.rest.asset.upload_session.exists")
     @patch("datature.rest.asset.upload_session.open")
-    # pylint: disable=W0613,R0913,C0103
-    def test_add_with_file(self, patch_open, patch_exist, google_crc32c,
-                           struct, os, filetype):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_add_with_file(self, patch_datature, patch_open, google_crc32c,
+                           struct, path, filetype):
         """Test add asset to upload with file."""
         upload_session = UploadSession()
 
+        patch_datature.ASSET_UPLOAD_BATCH_SIZE = 100
         struct.unpack.return_value = [-384617082]
-        os.path.basename.return_value = "assetName"
-        os.path.getsize.return_value = 5613
+        path.basename.return_value = "assetName"
+        path.getsize.return_value = 5613
 
         mock_guess = MagicMock()
         mock_guess.mime = "image/jpeg"
         filetype.guess.return_value = mock_guess
 
         upload_session.add("assetPath")
 
-    def test_start_with_empty_assets(self):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_start_with_empty_assets(self, patch_datature):
         """Test start upload with empty assets ."""
         upload_session = UploadSession()
 
         try:
             upload_session.start(["main"])
-        # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.rest.asset.upload_session.request")
     @patch("datature.rest.asset.upload_session.open")
-    # pylint: disable=W0613
-    def test_start_with_early_return(self, patch_open, patch_request):
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_start(self, patch_datature, patch_open, patch_request):
         """Test start upload with empty assets ."""
+        patch_datature.ASSET_UPLOAD_BATCH_SIZE = 100
+
         upload_session = UploadSession()
         upload_session.assets = [{
             "filename": "test.jpeg",
             "mime": "image/jpeg",
             "size": 5613,
             "crc32c": -384617082
         }]
         upload_session.file_name_map = {"test.jpeg": {"path": "file_path"}}
         upload_session.request = MagicMock()
 
-        upload_session.request.side_effect = [
-            upload_session_fixture.upload_assets_response
-        ]
+        upload_session.request.return_value = upload_session_fixture.upload_assets_response
 
         upload_session.assets = [{
             "filename": "test.jpeg",
             "mime": "image/jpeg",
             "size": 5613,
             "crc32c": -384617082
         }]
 
-        upload_session.start(["main"])
+        upload_session.start(["main"], background=True)
 
     @patch("datature.rest.asset.upload_session.Operation")
     @patch("datature.rest.asset.upload_session.request")
     @patch("datature.rest.asset.upload_session.open")
-    # pylint: disable=W0613
-    def test_start_with_no_early_return(self, patch_open, patch_request,
-                                        operation):
-        """Test start upload with empty assets ."""
+    @patch("datature.rest.asset.upload_session.datature")
+    def test_start_with_background(self, patch_datature, patch_open,
+                                   patch_request, operation):
+        """Test start upload with wait server process."""
+        patch_datature.SHOW_PROGRESS = False
         upload_session = UploadSession()
         upload_session.assets = [{
             "filename": "test.jpeg",
             "mime": "image/jpeg",
             "size": 5613,
             "crc32c": -384617082
         }]
         upload_session.file_name_map = {"test.jpeg": {"path": "file_path"}}
         upload_session.request = MagicMock()
 
-        upload_session.request.side_effect = [
-            upload_session_fixture.upload_assets_response
-        ]
+        upload_session.request.return_value = upload_session_fixture.upload_assets_response
 
         upload_session.assets = [{
             "filename": "test.jpeg",
             "mime": "image/jpeg",
             "size": 5613,
             "crc32c": -384617082
         }]
 
-        upload_session.start(["main"], early_return=False)
+        upload_session.start(["main"])
 
         operation.loop_retrieve.assert_called()
```

### Comparing `datature-0.7.5/test/rest/test_deploy.py` & `datature-1.0.0/test/rest/test_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import unittest
 from unittest.mock import MagicMock
 from datature.rest.deploy import Deploy
 
 
 class TestDeploy(unittest.TestCase):
-    """Datature Deploy API Resource Teset Cases."""
+    """Datature Deploy API Resource Test Cases."""
 
     def test_list(self):
         """Test list all deployments."""
         Deploy.request = MagicMock()
 
         Deploy.list()
```

### Comparing `datature-0.7.5/test/rest/test_operation.py` & `datature-1.0.0/test/rest/test_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from test.fixture.data import operation_fixture
 from datature.rest.operation import Operation
 from datature.error import Error
 import datature
 
 
 class TestOperation(unittest.TestCase):
-    """Datature Operation API Resource Teset Cases."""
+    """Datature Operation API Resource Test Cases."""
 
     def test_retrieve(self):
         """Test retrieve an operation."""
         Operation.request = MagicMock()
 
         Operation.retrieve("op_link")
```

### Comparing `datature-0.7.5/test/rest/test_project.py` & `datature-1.0.0/test/rest/test_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import unittest
 from unittest.mock import MagicMock
 from datature.rest.project import Project
 
 
 class TestProject(unittest.TestCase):
-    """Datature Project API Resource Teset Cases."""
+    """Datature Project API Resource Test Cases."""
 
     def test_retrieve(self):
         """Test retrieve a project."""
         Project.request = MagicMock()
 
         Project.retrieve()
```

### Comparing `datature-0.7.5/test/rest/test_run.py` & `datature-1.0.0/test/rest/test_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                         "evaluationInterval": 1,
                         "metric": "Loss/total_loss"
                     },
                     "limit": {
                         "metric": "LIM_MINUTE",
                         "value": 260
                     },
+                    "debug": None
                 },
                 "features": {
                     "preview": True
                 }
             })
 
     def test_log(self):
```

### Comparing `datature-0.7.5/test/rest/test_tag.py` & `datature-1.0.0/test/rest/test_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import unittest
 from unittest.mock import MagicMock
 from datature.rest.tag import Tag
 
 
 class TestTag(unittest.TestCase):
-    """Datature Tag API Resource Teset Cases."""
+    """Datature Tag API Resource Test Cases."""
 
     def test_list(self):
         """Test list tags."""
         Tag.request = MagicMock()
 
         Tag.list()
```

### Comparing `datature-0.7.5/test/rest/test_workflow.py` & `datature-1.0.0/test/rest/test_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import unittest
 from unittest.mock import MagicMock
 from datature.rest.workflow import Workflow
 
 
 class TestWorkflow(unittest.TestCase):
-    """Datature Workflow API Resource Teset Cases."""
+    """Datature Workflow API Resource Test Cases."""
 
     def test_list(self):
         """Test list all workflows."""
         Workflow.request = MagicMock()
 
         Workflow.list()
```

### Comparing `datature-0.7.5/test/test_error.py` & `datature-1.0.0/test/test_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 '''
 
 import unittest
 from datature.error import BadRequestError
 
 
 class TestError(unittest.TestCase):
-    """Datature Logger Teset Cases."""
+    """Datature Logger Test Cases."""
 
     def test_bad_request_error(self):
         """Test BadRequestError class."""
 
         bad_request_error = BadRequestError("Test BadRequestError")
 
         error_string = repr(bad_request_error)
```

### Comparing `datature-0.7.5/test/test_logger.py` & `datature-1.0.0/test/test_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import unittest
 from unittest.mock import patch
 from datature.logger import log_debug, log_info
 import datature
 
 
 class TestLogger(unittest.TestCase):
-    """Datature Logger Teset Cases."""
+    """Datature Logger Test Cases."""
 
     @patch("datature.logger.logger")
     def test_log_debug(self, patch_logging):
         """Test log debug function."""
 
         datature.LOG_LEVEL = "debug"
         log_debug("log_debug test.")
```

