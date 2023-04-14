# Comparing `tmp/resc_vcs_scanner-1.1.0.tar.gz` & `tmp/resc_vcs_scanner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-1.1.0.tar", last modified: Thu Mar  9 12:54:11 2023, max compression
+gzip compressed data, was "resc_vcs_scanner-1.2.0.tar", last modified: Fri Apr 14 15:09:49 2023, max compression
```

## Comparing `resc_vcs_scanner-1.1.0.tar` & `resc_vcs_scanner-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.186427 resc_vcs_scanner-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.190427 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 12:54:11.000000 resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.190427 resc_vcs_scanner-1.1.0/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/output_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/stdout_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:11.194428 resc_vcs_scanner-1.1.0/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-09 12:54:06.000000 resc_vcs_scanner-1.1.0/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.953434 resc_vcs_scanner-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/output_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/secret_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/stdout_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-1.1.0/PKG-INFO` & `resc_vcs_scanner-1.2.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.1.0/setup.cfg` & `resc_vcs_scanner-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 1.1.0
+version = 1.2.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scanner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/common.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/model.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/output_module.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/output_module.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,18 @@
                                envvar="RESC_EXIT_CODE_WARN",
                                help="Exit code given if CLI encounters findings tagged with Warn, default 2. "
                                     "Can also be set via the RESC_EXIT_CODE_WARN environment variable")
     parser_common.add_argument("-b", "--exit-code-block", required=False, action=EnvDefault, default=1, type=int,
                                envvar="RESC_EXIT_CODE_BLOCK",
                                help="Exit code given if CLI encounters findings tagged with Block, default 1. "
                                     "Can also be set via the RESC_EXIT_CODE_BLOCK environment variable")
+    parser_common.add_argument("--filter-tag", required=False, action=EnvDefault, type=str,
+                               envvar="RESC_FILTER_TAG",
+                               help="Filter for findings based on specified tag. "
+                                    "Can also be set via the RESC_FILTER_TAG environment variable")
     parser_common.add_argument("-v", "--verbose", required=False, action="store_true",
                                help="Enable more verbose logging")
 
     repository_common = ArgumentParser(add_help=False)
     repository_common.add_argument("--repo-name", type=str, required=False, action=EnvDefault, envvar="RESC_REPO_NAME",
                                    help="The name of the repository. "
                                         "Can also be set via the RESC_REPO_NAME environment variable")
@@ -194,15 +198,16 @@
         repository_id="local",
         project_key="local",
         vcs_instance_name="vcs_instance_name",
         branches=[]
     )
 
     output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
-                                 exit_code_warn=args.exit_code_warn, exit_code_block=args.exit_code_block)
+                                 exit_code_warn=args.exit_code_warn, exit_code_block=args.exit_code_block,
+                                 filter_tag=args.filter_tag)
     with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
         rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
@@ -246,15 +251,16 @@
 
     if args.rws_url:
         output_plugin = RESTAPIWriter(rws_url=args.rws_url)
         rule_pack_version = output_plugin.download_rule_pack()
 
     else:
         output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
-                                     exit_code_warn=args.exit_code_warn, exit_code_block=args.exit_code_block)
+                                     exit_code_warn=args.exit_code_warn, exit_code_block=args.exit_code_block,
+                                     filter_tag=args.filter_tag)
         with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
             rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
```

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/rws_api_writer.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/rws_api_writer.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/secret_scanners/stdout_writer.py` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/stdout_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 from prettytable import PrettyTable
 from resc_backend.resc_web_service.schema.branch import Branch
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.scan import ScanRead
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_instance import VCSInstanceRead
+from termcolor import colored
 
 # First Party
 from vcs_scanner.helpers.finding_action import FindingAction
 from vcs_scanner.model import VCSInstanceRuntime
 from vcs_scanner.output_module import OutputModule
 
 logger = logging.getLogger(__name__)
 
 
 class STDOUTWriter(OutputModule):
 
-    def __init__(self, toml_rule_file_path: str, exit_code_warn: int, exit_code_block: int):
+    def __init__(self, toml_rule_file_path: str, exit_code_warn: int, exit_code_block: int, filter_tag: str = None):
         self.toml_rule_file_path: str = toml_rule_file_path
         self.exit_code_warn: int = exit_code_warn
         self.exit_code_block: int = exit_code_block
+        self.filter_tag: str = filter_tag
         self.exit_code_success = 0
 
     def write_vcs_instance(self, vcs_instance_runtime: VCSInstanceRuntime) -> Optional[VCSInstanceRead]:
         vcs_instance = VCSInstanceRead(id_=1,
                                        name=vcs_instance_runtime.name,
                                        provider_type=vcs_instance_runtime.provider_type,
                                        hostname=vcs_instance_runtime.hostname,
@@ -82,14 +84,30 @@
         rule_action = FindingAction.INFO
         if FindingAction.WARN in rule_tags.get(finding.rule_name, []):
             rule_action = FindingAction.WARN
         if FindingAction.BLOCK in rule_tags.get(finding.rule_name, []):
             rule_action = FindingAction.BLOCK
         return rule_action
 
+    def _finding_tag_filter(self, finding: FindingCreate, rule_tags: dict, filter_tag: str) -> bool:
+        """
+            Determine the action to take for the finding, based on the rule tags
+        :param finding:
+            FindingCreate instance of the finding
+        :param rule_tags:
+            Dictionary continuing all the rules and there respective tags
+        :Param: filter_tag.
+            filter_tag will check for the tag
+        :return bool:
+            The output will be boolean, based on the tag filter given
+        """
+        if filter_tag and filter_tag not in rule_tags.get(finding.rule_name, []):
+            return False
+        return True
+
     def write_findings(self, scan_id: int, branch_id: int, scan_findings: List[FindingCreate]):
         """
             Write the findings to the STDOUT in a nice table and set the exit code based on the FindingActions found
         :param scan_id:
             id of the scan in question
         :param branch_id:
             id of the branch in question
@@ -98,31 +116,61 @@
         """
         # Initialize table
         output_table = PrettyTable()
         output_table.field_names = ['Level', 'Rule', 'Line', 'Position', 'File path']
         output_table.align = 'l'
         output_table.align['Line'] = 'r'
 
+        block_count = 0
+        warn_count = 0
+        info_count = 0
+
         exit_code = self.exit_code_success
 
         rule_tags = self._get_rule_tags()
         for finding in scan_findings:
-            finding_action = self._determine_finding_action(finding, rule_tags)
-
-            if exit_code != self.exit_code_block:
-                if exit_code == self.exit_code_success and finding_action == FindingAction.WARN:
-                    exit_code = self.exit_code_warn
-                elif finding_action == FindingAction.BLOCK:
-                    exit_code = self.exit_code_block
-
-            output_table.add_row([finding_action.value, finding.rule_name, finding.line_number,
-                                  f"{finding.column_start}-{finding.column_end}", finding.file_path])
-
-        logger.info(f"\n{output_table.get_string(sortby='Rule')}")
-        logger.info(f"Found {len(scan_findings)} findings {self.toml_rule_file_path}")
+            should_process_finding = self._finding_tag_filter(finding, rule_tags, self.filter_tag)
+            if should_process_finding:
+                finding_action = self._determine_finding_action(finding, rule_tags)
+                if finding_action == FindingAction.BLOCK:
+                    finding_action_value = colored(finding_action.value, "red", attrs=["bold"])
+                    block_count += 1
+                elif finding_action == FindingAction.WARN:
+                    finding_action_value = colored(finding_action.value, "light_red", attrs=["bold"])
+                    warn_count += 1
+                elif finding_action == FindingAction.INFO:
+                    finding_action_value = colored(finding_action.value, "light_yellow", attrs=["bold"])
+                    info_count += 1
+                else:
+                    finding_action_value = finding_action.value
+                    info_count += 1
+
+                if exit_code != self.exit_code_block:
+                    if exit_code == self.exit_code_success and finding_action == FindingAction.WARN:
+                        exit_code = self.exit_code_warn
+                    elif finding_action == FindingAction.BLOCK:
+                        exit_code = self.exit_code_block
+
+                output_table.add_row([finding_action_value, finding.rule_name, finding.line_number,
+                                     f"{finding.column_start}-{finding.column_end}", finding.file_path])
+
+        logger.info(f"\n{output_table.get_string(sortby='Level')}")
+
+        logger.info(f"Findings detected : Total - {block_count+warn_count+info_count}, Block - {block_count}, "
+                    f"Warn - {warn_count}, Info - {info_count}")
+
+        if exit_code == self.exit_code_success:
+            logger.info(f"Findings threshold check results: {colored('PASS', 'light_green', attrs=['bold'])}")
+        elif exit_code == self.exit_code_block:
+            logger.info(f"Findings threshold check results: {colored('FAIL', 'red', attrs=['bold'])}")
+            logger.info(
+                colored(f"Scan failed due to policy violations: [Block:{block_count}]", "red", attrs=["bold"]))
+        elif exit_code == self.exit_code_warn:
+            logger.info(f"Findings threshold check results: {colored('PASS', 'light_green', attrs=['bold'])}")
+            logger.info(colored(f"Warning for policy violations: [Warn:{warn_count}]", "light_red", attrs=["bold"]))
 
         sys.exit(exit_code)
 
     def write_scan(self, scan_type_to_run: ScanType, last_scanned_commit: str, scan_timestamp: datetime,
                    branch: Branch, rule_pack: str) -> Optional[ScanRead]:
         logger.info(f"Running {scan_type_to_run} scan on branch {branch.branch_name}")
         return ScanRead(last_scanned_commit="NONE",
```

### Comparing `resc_vcs_scanner-1.1.0/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-1.2.0/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

