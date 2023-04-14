# Comparing `tmp/yellowdog-python-examples-5.0.1.tar.gz` & `tmp/yellowdog-python-examples-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.1.tar", last modified: Mon Apr  3 12:07:30 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-5.0.2.tar", last modified: Fri Apr 14 14:21:00 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.1.tar` & `yellowdog-python-examples-5.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-03 12:07:30.194294 yellowdog-python-examples-5.0.1/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.1/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-03 12:07:30.194376 yellowdog-python-examples-5.0.1/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.1/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   103259 2023-04-03 12:06:33.000000 yellowdog-python-examples-5.0.1/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.1/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.1/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-03 12:07:30.194692 yellowdog-python-examples-5.0.1/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-03 12:07:30.193288 yellowdog-python-examples-5.0.1/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-03 12:06:33.000000 yellowdog-python-examples-5.0.1/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.1/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.1/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.1/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.1/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.1/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.1/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12167 2023-04-03 12:06:33.000000 yellowdog-python-examples-5.0.1/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     8947 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.1/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.1/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.1/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.1/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.1/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    39155 2023-04-03 12:06:33.000000 yellowdog-python-examples-5.0.1/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     5963 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.1/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.1/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.1/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.1/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.1/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.1/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    10629 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.1/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.1/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.1/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-03 12:07:30.194195 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-03 12:07:30.000000 yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.040494 yellowdog-python-examples-5.0.2/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.2/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-14 14:21:00.040572 yellowdog-python-examples-5.0.2/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.2/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109044 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.2/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.2/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-14 14:21:00.040868 yellowdog-python-examples-5.0.2/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.033852 yellowdog-python-examples-5.0.2/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.2/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.2/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.2/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.2/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.2/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.2/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.2/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.2/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.2/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    39150 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.2/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.2/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.2/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.2/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.2/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    10735 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.2/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.2/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.040384 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.1/LICENSE` & `yellowdog-python-examples-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/PKG-INFO` & `yellowdog-python-examples-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.1
+Version: 5.0.2
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.1/PYPI_README.md` & `yellowdog-python-examples-5.0.2/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/README.md` & `yellowdog-python-examples-5.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 * [Naming Rules](#naming-rules)
 * [Common Properties](#common-properties)
    * [Specifying Common Properties using the Command Line or Environment Variables](#specifying-common-properties-using-the-command-line-or-environment-variables)
    * [Variable Substitutions in Common Properties](#variable-substitutions-in-common-properties)
 * [Variable Substitutions](#variable-substitutions)
    * [Default Variables](#default-variables)
    * [User-Defined Variables](#user-defined-variables)
+   * [Nested Variables](#nested-variables)
 * [Work Requirement Properties](#work-requirement-properties)
    * [Work Requirement JSON File Structure](#work-requirement-json-file-structure)
    * [Property Inheritance](#property-inheritance)
    * [Work Requirement Property Dictionary](#work-requirement-property-dictionary)
    * [Automatic Properties](#automatic-properties)
       * [Work Requirement, Task Group and Task Naming](#work-requirement-task-group-and-task-naming)
       * [Task Types](#task-types)
@@ -41,14 +42,19 @@
          * [Files in the inputs List](#files-in-the-inputs-list)
          * [Files in the uploadFiles List](#files-in-the-uploadfiles-list)
       * [File Dependencies Using verifyAtStart and verifyWait](#file-dependencies-using-verifyatstart-and-verifywait)
       * [Files Downloaded Using inputsOptional](#files-downloaded-using-inputsoptional)
       * [Files Downloaded to a Node for use in Task Execution](#files-downloaded-to-a-node-for-use-in-task-execution)
       * [Files Uploaded from a Node to the Object Store after Task Execution](#files-uploaded-from-a-node-to-the-object-store-after-task-execution)
       * [Files Downloaded from the Object Store to Local Storage](#files-downloaded-from-the-object-store-to-local-storage)
+   * [Task Execution Context](#task-execution-context)
+      * [Task Execution Steps](#task-execution-steps)
+      * [The User and Group used for Tasks](#the-user-and-group-used-for-tasks)
+      * [Home Directory for yd-agent](#home-directory-for-yd-agent)
+      * [Task Execution Directory](#task-execution-directory)
    * [Specifying Work Requirements using CSV Data](#specifying-work-requirements-using-csv-data)
       * [Work Requirement CSV Data Example](#work-requirement-csv-data-example)
       * [CSV Variable Substitutions](#csv-variable-substitutions)
       * [Property Inheritance](#property-inheritance-1)
       * [Multiple Task Groups using Multiple CSV Files](#multiple-task-groups-using-multiple-csv-files)
       * [Using CSV Data with Simple, TOML-Only Work Requirement Specifications](#using-csv-data-with-simple-toml-only-work-requirement-specifications)
       * [Inspecting the Results of CSV Variable Substitution](#inspecting-the-results-of-csv-variable-substitution)
@@ -74,15 +80,15 @@
    * [yd-delete](#yd-delete)
    * [yd-upload](#yd-upload)
    * [yd-shutdown](#yd-shutdown)
    * [yd-instantiate](#yd-instantiate)
       * [Test-Running a Dynamic Template](#test-running-a-dynamic-template)
    * [yd-terminate](#yd-terminate)
 
-<!-- Added by: pwt, at: Mon Mar 13 14:01:55 GMT 2023 -->
+<!-- Added by: pwt, at: Fri Apr 14 15:14:49 BST 2023 -->
 
 <!--te-->
 
 # Overview
 
 This repository contains a set of example Python scripts for interacting with the YellowDog Platform. The scripts use the **[YellowDog Python SDK](https://docs.yellowdog.co/api/python/index.html)**, the code for which can be found [on GitHub](https://github.com/yellowdog/yellowdog-sdk-python-public).
 
@@ -331,14 +337,34 @@
 run_id = "1234"
 ```
 
 Directives set on the command line take precedence over directives set in environment variables, and both of them take precedence over directives set in a TOML file.
 
 This method can be used to override the default directives, e.g., setting `-v username="other-user"` will override the default `{{username}}` directive.
 
+## Nested Variables
+
+In the case of **TOML properties only**, variable substitutions can be nested.
+
+For example, if one wanted to select a different `templateId` for a Worker Pool depending on the value of a `region` variable, one could use the following:
+
+```toml
+[common.variables]
+    template_london = "ydid:crt:65EF4F:a4d757cf-b67a-4eb6-bd39-8a6ffd46c8f4"
+    template_phoenix = "ydid:crt:65EF4F:e4239dec-78c2-421c-a7f3-71e61b72946f"
+    template_frankfurt = "ydid:crt:65EF4F:329602cf-5945-4aad-a288-ea424d64d55e"
+
+[common.workerPool]
+    templateId = "{{template_{{region}}}}"
+```
+
+Then, if one used `yd-provision -v region=phoenix`, the `templateId` property would first resolve to `"{{template_pheonix}}"`, and then to `"ydid:crt:65EF4F:e4239dec-78c2-421c-a7f3-71e61b72946f"`.
+
+Nesting can be up to three levels deep including the top level.
+
 # Work Requirement Properties
 
 The `workRequirement` section of the configuration file is optional. It's used only by the `yd-submit` command, and controls the Work Requirement that is submitted to the Platform.
 
 The details of a Work Requirement to be submitted can be captured entirely within the TOML configuration file for simple examples. More complex examples capture the Work Requirement in a combination of the TOML file plus a JSON document, or in a JSON document only.
 
 ## Work Requirement JSON File Structure
@@ -973,15 +999,15 @@
 
 
 2. If the `flattenInputPaths` property is set to `true` for the Task, the downloaded objects are all placed directly in root of the Task's working directory.
 
 For example:
 
 ```shell
-If the required object is: development:testrun_221108-120404-7d2/dev/file_1.txt
+If the required object is: development::testrun_221108-120404-7d2/dev/file_1.txt
 
 then, if flattenInputPaths is false, the file will be found at:
  -> <working_directory>/testrun_221108-120404-7d2/dev/file_1.txt
  
 else, if flattenInputPaths is true, the file will be found at:
  -> <working_directory>/file_1.txt 
  
@@ -995,15 +1021,15 @@
 environment = {WR_DIRECTORY = "{{wr_name}}"}
 ```
 
 The Work Requirement name would then be available to the Task in the environment variable `$WR_DIRECTORY`.
 
 ### Files Uploaded from a Node to the Object Store after Task Execution
 
-After Task completion, the Agent will upload specified output files to the Object Store. The files to be uploaded are those listed in the `outputs` property for the Task.
+After Task completion, the Agent will upload specified output files to the Object Store. The files to be uploaded are those listed in the `outputs` and `outputsRequired` properties for the Task.
 
 In addition, the console output of the Task is captured in a file called `taskoutput.txt` in the root of the Task's working directory. Whether the `taskoutput.txt` file is uploaded to the Object Store is determined by the `captureTaskOutput` property for the Task, and this is set to 'true' by default.
 
 If Task outputs are created in subdirectories below the Task's working directory, include the directories for files in the `outputs` property. E.g., if a Task creates files `results/openfoam.tar.gz` and `results/openfoam.log`, then specify these for upload in the `outputs` property as follows:
 
 `"outputs": ["results/openfoam.tar.gz", "results/openfoam.log"]`
 
@@ -1040,14 +1066,77 @@
             └── taskoutput.txt
 ```
 
 Note that everything within the `namespace::work-requirement` directory in the Object Store is downloaded, including any files that were specified in `inputs` and uploaded as part of the Work Requirement submission. Multiple Task Groups, and multiple Tasks will all appear in the directory structure.
 
 If the `development` directory already exists, `yd-download` will try `development.01`, etc., to avoid overwriting previous downloads.
 
+## Task Execution Context
+
+This section discusses the context within which a Task operates when it's executed by a Worker on a node. It applies specifically to the YellowDog Agent running on a Linux node, and configured using the default username, directories, etc. Configurations can vary.
+
+### Task Execution Steps
+
+When a Task is allocated to a Worker on a node by the YellowDog Scheduler, the following steps are followed:
+
+1. The Agent running on the node downloads the Task's properties: its `taskType`,  `arguments`, `environment`, `taskdata`, and (from the Object Store) any files in the `inputs` list and any available files in the `inputsOptional` list.
+2. These files are placed in an ephemeral directory created for this Task's execution, and into which any output files are also placed by default.
+2. The Agent runs the command specified for the `taskType` in the Agent's `application.yaml` configuration file. This done as a simple `exec` of a subprocess.
+3. When the Task concludes, the Agent uses the exit code of the subprocess to report success (zero) or failure (non-zero).
+4. The Agent then gathers any files in the `outputs` and `outputsRequired` lists and uploads them to the Object Store. If a file in the `outputsRequired` list is not found, the Task will be reported as failed. The Agent will also optionally upload the console output (including both `stdout` and `stderr`) of the Task, contained in the `taskoutput.txt` file.
+5. The ephemeral Task directory is then deleted.
+
+Note that if a Task is aborted during execution, the Task's subprocess is sent a `SIGINT`, allowing the Task an opportunity to terminate any child processes or other resources (e.g., containers) that may have been started as part of Task execution.
+
+Once the steps above have been completed, the Worker is ready to accept its next Task from the YellowDog scheduler.
+
+Note that if the Agent on a node has multiple Workers, then Tasks are executed in parallel on the node and can start and stop independently.
+
+### The User and Group used for Tasks
+
+By default, the Agent runs as user and group `yd-agent`, and hence Tasks also execute under this user.
+
+`yd-agent` does not have `sudo` privileges as standard, but this can be added if required at instance boot time via the `userData` property of a provisioning request. E.g. (for Ubuntu):
+
+```shell
+usermod -aG wheel yd-agent
+echo -e "yd-agent\tALL=(ALL)\tNOPASSWD: ALL" > /etc/sudoers.d/020-yd-agent
+```
+
+### Home Directory for `yd-agent`
+
+By default, the home directory of the `yd-agent` user is `/opt/yellowdog/agent`. This directory typically contains the `application.yaml` file used to configure the Agent, as well as any scripts that are used to execute the Task Types that the node supports.
+
+If one wants to SSH to an instance as user `yd-agent`, perhaps for debugging purposes, SSH keys can be inserted via instance `userData`, e.g.:
+
+```shell
+YDA_HOME=/opt/yellowdog/agent
+mkdir -p $YDA_HOME/.ssh
+chmod og-rwx $YDA_HOME/.ssh
+cat >> $YDA_HOME/.ssh/authorized_keys << EOF
+<<Insert_Public_key_Here>>
+EOF
+chmod og-rw $YDA_HOME/.ssh/authorized_keys
+chown -R yd-agent:yd-agent $YDA_HOME/.ssh
+```
+
+### Task Execution Directory
+
+Ephemeral Task directories are created under `/var/opt/yellowdog/agent/data/workers`. This directory contains one or more numbered subdirectories where each numbered directory corresponds to a Worker on the node.
+
+When a Task is allocated to a node, an ephemeral directory is created under the applicable Worker directory, with a name corresponding the YellowDog ID for the Task. For example, this is an ephemeral directory being used by Worker number `1`:
+
+`/var/opt/yellowdog/agent/data/workers/1/ydid_task_559EBE_74949336-ac2b-4811-a7d5-f3ecd9739908_1_1`
+
+This is the directory into which downloaded objects are placed, and in which output files are created by default. The console output `taskoutput.txt` file will also be created in this directory.
+
+See the [Files Downloaded to a Node](#files-downloaded-to-a-node-for-use-in-task-execution) section above for more details on how files in this directory are handled.
+
+At the conclusion of the Task, after any files requested for upload have been uploaded to the Object Store (see the [Files Uploaded from a Node](#files-uploaded-from-a-node-to-the-object-store-after-task-execution) section for more information), the `ydid_task_559EBE_74949336-ac2b-4811-a7d5-f3ecd9739908_1_1` will be removed.
+
 ## Specifying Work Requirements using CSV Data
 
 CSV data files can be used to drive the generation of lists of Tasks, as follows:
 
 - A **prototype** Task specification is created within a JSON Work Requirement specification or in the `workRequirement` section of the TOML configuration file
 - The prototype task includes one or more variable substitutions
 - A CSV file is created, with the **headers** (first row) matching the names of the variable substitutions in the Task prototype
@@ -1481,23 +1570,27 @@
 
 The scripts provide full support for variable substitutions in Jsonnet files, using the same rules as for the JSON specifications. Remember that for **Worker Pool** specifications, variable substitutions must be prefixed by `__`, e.g. `"__{{username}}}"`.
 
 Variable substitution is performed before Jsonnet expansion into JSON, and again after the expansion.
 
 ## Checking Jsonnet Processing
 
-To inspect the basic conversion of Jsonnet into JSON, without any additional processing by the Python Examples scripts, the `yd-jsonnet2json` command can be used. This takes a single command line argument which is the name of the jsonnet file to be processed:
+There are three possibilities for verifying that a Jsonnet specification is doing what is intended:
+
+1. To inspect the basic conversion of Jsonnet into JSON, without any additional processing by the Python Examples scripts, the `yd-jsonnet2json` command can be used. This takes a single command line argument which is the name of the jsonnet file to be processed:
 
 ```shell
 yd-jsonnet2json my_file.jsonnet
 ```
 
-The `jsonnet-dry-run` (`-J`) option of the `yd-submit`, `yd-provision` and `yd-instantiate` commands will generate JSON output representing the Jsonnet to JSON processing only, including applicable variable substitutions, but before full property expansion into the JSON that will be submitted to the Platform.
 
-The `dry-run` (`-D`) option will generate JSON output representing the full processing of the Jsonnet file into what will be submitted to the API. This allows inspection to check that the output matches expectations, prior to submitting to the Platform.
+2. The `jsonnet-dry-run` (`-J`) option of the `yd-submit`, `yd-provision` and `yd-instantiate` commands will generate JSON output representing the Jsonnet to JSON processing only, including applicable variable substitutions, but before full property expansion into the JSON that will be submitted to the Platform.
+
+
+3. The `dry-run` (`-D`) option will generate JSON output representing the full processing of the Jsonnet file into what will be submitted to the API. This allows inspection to check that the output matches expectations, prior to submitting to the Platform.
 
 ## Jsonnet Example
 
 Here's an example of a Jsonnet file that generates a Work Requirement with four Tasks:
 
 ```jsonnet
 # Function for synthesising Tasks
```

### Comparing `yellowdog-python-examples-5.0.1/pyproject.toml` & `yellowdog-python-examples-5.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/setup.cfg` & `yellowdog-python-examples-5.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/abort.py` & `yellowdog-python-examples-5.0.2/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/admin.py` & `yellowdog-python-examples-5.0.2/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/args.py` & `yellowdog-python-examples-5.0.2/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/cancel.py` & `yellowdog-python-examples-5.0.2/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/check_imports.py` & `yellowdog-python-examples-5.0.2/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/compact_json.py` & `yellowdog-python-examples-5.0.2/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/config.py` & `yellowdog-python-examples-5.0.2/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/config_keys.py` & `yellowdog-python-examples-5.0.2/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/csv_data.py` & `yellowdog-python-examples-5.0.2/yd_commands/csv_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         (config_wr.flatten_input_paths, FLATTEN_PATHS),
         (config_wr.input_files, INPUT_FILES),
         (config_wr.optional_inputs, INPUTS_OPTIONAL),
         (config_wr.output_files, OUTPUT_FILES),
         (config_wr.output_files_required, OUTPUT_FILES_REQUIRED),
         (config_wr.task_data, TASK_DATA),
         (config_wr.task_data_file, TASK_DATA_FILE),
-        (config_wr.task_group_name, TASK_GROUP_NAME),
+        (config_wr.task_group_name, TASK_GROUP_NAME),  # Note: oddity
         (config_wr.task_name, TASK_NAME),
         (config_wr.task_type, TASK_TYPE),
         (config_wr.upload_files, UPLOAD_FILES),
         (config_wr.verify_at_start, VERIFY_AT_START),
         (config_wr.verify_wait, VERIFY_WAIT),
     ]:
         if config_value is not None and substitions_present(
```

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/delete.py` & `yellowdog-python-examples-5.0.2/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/download.py` & `yellowdog-python-examples-5.0.2/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/instantiate.py` & `yellowdog-python-examples-5.0.2/yd_commands/instantiate.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,24 @@
                 instanceTags=CONFIG_WP.instance_tags,
                 imagesId=CONFIG_WP.images_id,
                 userData=get_user_data_property(CONFIG_WP),
             )
 
             if ARGS_PARSER.report:
                 print_log("Generating provisioning report only")
-                test_result: ComputeRequirementTemplateTestResult = (
-                    CLIENT.compute_client.test_compute_requirement_template(
-                        compute_requirement_template_usage
+                try:
+                    test_result: ComputeRequirementTemplateTestResult = (
+                        CLIENT.compute_client.test_compute_requirement_template(
+                            compute_requirement_template_usage
+                        )
                     )
-                )
-                print_compute_template_test_result(test_result)
+                    print_compute_template_test_result(test_result)
+                except requests.HTTPError as http_error:
+                    if "No sources" in http_error.response.text:
+                        print_log("No Compute Sources match the Template's constraints")
                 return
 
             if not ARGS_PARSER.dry_run:
                 compute_requirement = (
                     CLIENT.compute_client.provision_compute_requirement_template(
                         compute_requirement_template_usage
                     )
```

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/interactive.py` & `yellowdog-python-examples-5.0.2/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-5.0.2/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/list.py` & `yellowdog-python-examples-5.0.2/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/object_utilities.py` & `yellowdog-python-examples-5.0.2/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/printing.py` & `yellowdog-python-examples-5.0.2/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/provision.py` & `yellowdog-python-examples-5.0.2/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/provision_utils.py` & `yellowdog-python-examples-5.0.2/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/reformat_json.py` & `yellowdog-python-examples-5.0.2/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/shutdown.py` & `yellowdog-python-examples-5.0.2/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/submit.py` & `yellowdog-python-examples-5.0.2/yd_commands/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     if wr_data.get(TASK_TYPE, None) is not None:
         if wr_data.get(TASK_TYPES, None) is None:
             wr_data[TASK_TYPES] = [wr_data[TASK_TYPE]]
 
     # Overwrite the WR name?
     global ID, CONFIG_WR
     ID = format_yd_name(
-        wr_data.get(L_WR_NAME, ID if CONFIG_WR.wr_name is None else CONFIG_WR.wr_name)
+        wr_data.get(NAME, ID if CONFIG_WR.wr_name is None else CONFIG_WR.wr_name)
     )
     # Lazy substitution of the Work Requirement name, now it's defined
     add_substitutions(subs={L_WR_NAME: ID})
     process_variable_substitutions(wr_data)
     CONFIG_WR = update_config_work_requirement(CONFIG_WR)
 
     # Handle any files that need to be uploaded
```

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/submit_utils.py` & `yellowdog-python-examples-5.0.2/yd_commands/submit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,8 +177,11 @@
 def format_yd_name(yd_name: str) -> str:
     """
     Format a string to be consistent with YellowDog naming requirements.
     """
     # Make obvious substitutions
     yd_name = yd_name.replace("/", "-").replace(" ", "_").lower()
     # Enforce acceptable regex and name length
-    return re.sub("[^a-z0-9_-]", "", yd_name)[:60]
+    yd_name = re.sub("[^a-z0-9_-]", "", yd_name)
+    if not yd_name[0].isalpha():
+        yd_name = f"z_{yd_name}"
+    return yd_name[:60]
```

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/terminate.py` & `yellowdog-python-examples-5.0.2/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/type_check.py` & `yellowdog-python-examples-5.0.2/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/upload.py` & `yellowdog-python-examples-5.0.2/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/upload_utils.py` & `yellowdog-python-examples-5.0.2/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/validate_properties.py` & `yellowdog-python-examples-5.0.2/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/variables.py` & `yellowdog-python-examples-5.0.2/yd_commands/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     L_TASK_COUNT = "task_count"
     L_TASK_GROUP_COUNT = "task_group_count"
 
 # Type annotations for variable type substitutions
 NUMBER_SUB = "num:"
 BOOL_SUB = "bool:"
 
+# Nested variables depth supported in TOML files
+NESTED_DEPTH = 3
+
 # Add user-defined variable substitutions
 # Can supersede the existing substitutions above
 ENV_VAR_PREFIX = "YD_VAR_"
 
 # Directives from environment variables
 for key, value in os.environ.items():
     if key.startswith(ENV_VAR_PREFIX):
@@ -247,15 +250,17 @@
                 var_name: str(var_value)
                 for var_name, var_value in config[COMMON_SECTION][VARIABLES].items()
             }
         )
     except KeyError:
         pass
 
-    process_variable_substitutions(config, prefix=prefix)
+    for _ in range(NESTED_DEPTH):
+        process_variable_substitutions(config, prefix=prefix)
+
     return config
 
 
 class VariableSubstitutedJsonnetFile:
     """
     The jsonnet 'evaluate_file' function will only operate on files,
     not strings, so this context manager class will create a
```

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/version.py` & `yellowdog-python-examples-5.0.2/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yd_commands/wrapper.py` & `yellowdog-python-examples-5.0.2/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.1
+Version: 5.0.2
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.1/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

