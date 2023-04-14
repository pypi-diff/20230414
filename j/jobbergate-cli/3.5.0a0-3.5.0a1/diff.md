# Comparing `tmp/jobbergate-cli-3.5.0a0.tar.gz` & `tmp/jobbergate-cli-3.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-cli-3.5.0a0.tar", max compression
+gzip compressed data, was "jobbergate-cli-3.5.0a1.tar", max compression
```

## Comparing `jobbergate-cli-3.5.0a0.tar` & `jobbergate-cli-3.5.0a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1082 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/LICENSE
--rw-r--r--   0        0        0     1065 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/README.rst
--rw-r--r--   0        0        0      801 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/__init__.py
--rw-r--r--   0        0        0     1112 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/application_base.py
--rw-r--r--   0        0        0    11156 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/auth.py
--rw-r--r--   0        0        0     3614 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/compat.py
--rw-r--r--   0        0        0     4355 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/config.py
--rw-r--r--   0        0        0     1139 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/constants.py
--rw-r--r--   0        0        0     3112 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/exceptions.py
--rw-r--r--   0        0        0     1134 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/jobberappslib.py
--rw-r--r--   0        0        0     1095 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/logging.py
--rw-r--r--   0        0        0     6510 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/main.py
--rw-r--r--   0        0        0     7002 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/render.py
--rw-r--r--   0        0        0     7348 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/requests.py
--rw-r--r--   0        0        0     6006 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/schemas.py
--rw-r--r--   0        0        0       66 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/__init__.py
--rw-r--r--   0        0        0       66 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/__init__.py
--rw-r--r--   0        0        0    10132 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/app.py
--rw-r--r--   0        0        0     1725 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/application_base.py
--rw-r--r--   0        0        0     1558 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/application_helpers.py
--rw-r--r--   0        0        0    13800 2023-03-28 06:43:17.749190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/questions.py
--rw-r--r--   0        0        0    10292 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/tools.py
--rw-r--r--   0        0        0       61 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/clusters/__init__.py
--rw-r--r--   0        0        0      728 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/clusters/app.py
--rw-r--r--   0        0        0     3284 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/clusters/tools.py
--rw-r--r--   0        0        0       64 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_scripts/__init__.py
--rw-r--r--   0        0        0    10067 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_scripts/app.py
--rw-r--r--   0        0        0     5519 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_scripts/tools.py
--rw-r--r--   0        0        0       68 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6502 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_submissions/app.py
--rw-r--r--   0        0        0     4167 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_submissions/tools.py
--rw-r--r--   0        0        0     1370 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/text_tools.py
--rw-r--r--   0        0        0     3524 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/jobbergate_cli/time_loop.py
--rw-r--r--   0        0        0     2531 2023-03-28 06:43:17.753190 jobbergate-cli-3.5.0a0/pyproject.toml
--rw-r--r--   0        0        0     2542 2023-03-28 06:43:33.206533 jobbergate-cli-3.5.0a0/setup.py
--rw-r--r--   0        0        0     2824 2023-03-28 06:43:33.206999 jobbergate-cli-3.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/LICENSE
+-rw-r--r--   0        0        0     1065 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/README.rst
+-rw-r--r--   0        0        0      801 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/jobbergate_cli/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/jobbergate_cli/application_base.py
+-rw-r--r--   0        0        0    11271 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/jobbergate_cli/auth.py
+-rw-r--r--   0        0        0     3614 2023-04-14 17:46:38.597634 jobbergate-cli-3.5.0a1/jobbergate_cli/compat.py
+-rw-r--r--   0        0        0     4355 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/config.py
+-rw-r--r--   0        0        0     1139 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/constants.py
+-rw-r--r--   0        0        0     3112 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/exceptions.py
+-rw-r--r--   0        0        0     1134 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/jobberappslib.py
+-rw-r--r--   0        0        0     1095 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/logging.py
+-rw-r--r--   0        0        0     6510 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/main.py
+-rw-r--r--   0        0        0     7002 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/render.py
+-rw-r--r--   0        0        0     7348 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/requests.py
+-rw-r--r--   0        0        0     6006 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/schemas.py
+-rw-r--r--   0        0        0       66 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/__init__.py
+-rw-r--r--   0        0        0       66 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/__init__.py
+-rw-r--r--   0        0        0    10132 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/app.py
+-rw-r--r--   0        0        0     1725 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/application_base.py
+-rw-r--r--   0        0        0     1558 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/application_helpers.py
+-rw-r--r--   0        0        0    13800 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/questions.py
+-rw-r--r--   0        0        0    10292 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/tools.py
+-rw-r--r--   0        0        0       61 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/clusters/__init__.py
+-rw-r--r--   0        0        0      728 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/clusters/app.py
+-rw-r--r--   0        0        0     3284 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/clusters/tools.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    10067 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_scripts/app.py
+-rw-r--r--   0        0        0     5519 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_scripts/tools.py
+-rw-r--r--   0        0        0       68 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6502 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_submissions/app.py
+-rw-r--r--   0        0        0     4167 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_submissions/tools.py
+-rw-r--r--   0        0        0     1370 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/text_tools.py
+-rw-r--r--   0        0        0     3524 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/jobbergate_cli/time_loop.py
+-rw-r--r--   0        0        0     2531 2023-04-14 17:46:38.601635 jobbergate-cli-3.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2542 2023-04-14 17:46:55.537515 jobbergate-cli-3.5.0a1/setup.py
+-rw-r--r--   0        0        0     2824 2023-04-14 17:46:55.538018 jobbergate-cli-3.5.0a1/PKG-INFO
```

### Comparing `jobbergate-cli-3.5.0a0/LICENSE` & `jobbergate-cli-3.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/README.rst` & `jobbergate-cli-3.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/__init__.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/application_base.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/auth.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,20 @@
 
     # Make static type checkers happy
     assert settings.JOBBERGATE_ACCESS_TOKEN_PATH is not None
     assert settings.JOBBERGATE_REFRESH_TOKEN_PATH is not None
 
     logger.debug(f"Caching access token at {settings.JOBBERGATE_ACCESS_TOKEN_PATH}")
     settings.JOBBERGATE_ACCESS_TOKEN_PATH.write_text(token_set.access_token)
+    settings.JOBBERGATE_ACCESS_TOKEN_PATH.chmod(0o600)
 
     if token_set.refresh_token is not None:
         logger.debug(f"Caching refresh token at {settings.JOBBERGATE_REFRESH_TOKEN_PATH}")
         settings.JOBBERGATE_REFRESH_TOKEN_PATH.write_text(token_set.refresh_token)
+        settings.JOBBERGATE_REFRESH_TOKEN_PATH.chmod(0o600)
 
 
 def clear_token_cache():
     """
     Clears the token cache.
     """
     logger.debug("Clearing cached tokens")
```

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/compat.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/compat.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/config.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/constants.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/exceptions.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/jobberappslib.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/jobberappslib.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/logging.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/main.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/render.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/render.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/requests.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/requests.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/schemas.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/app.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/application_base.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/application_helpers.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/application_helpers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/questions.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/questions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/applications/tools.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/applications/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/clusters/app.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/clusters/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/clusters/tools.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/clusters/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_scripts/app.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_scripts/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_scripts/tools.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_submissions/app.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_submissions/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/subapps/job_submissions/tools.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/subapps/job_submissions/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/text_tools.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/jobbergate_cli/time_loop.py` & `jobbergate-cli-3.5.0a1/jobbergate_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a0/pyproject.toml` & `jobbergate-cli-3.5.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-cli"
-version = "3.5.0-alpha.0"
+version = "3.5.0-alpha.1"
 description = "Jobbergate CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 packages = [ { include = "jobbergate_cli" } ]
 classifiers = [
```

### Comparing `jobbergate-cli-3.5.0a0/setup.py` & `jobbergate-cli-3.5.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'yarl>=1.7.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['jobbergate = jobbergate_cli.main:app']}
 
 setup_kwargs = {
     'name': 'jobbergate-cli',
-    'version': '3.5.0a0',
+    'version': '3.5.0a1',
     'description': 'Jobbergate CLI Client',
     'long_description': '================\n Jobbergate CLI\n================\n\nThe Jobbergate CLI provides a command-line interface to view and manage the Jobbergate\nresources. It can be used to create Job Scripts from template and then submit them to\nthe Slurm cluster to which Jobbergate is connected.\n\nJobbergate CLI is a Python project implemented with the\n`Typer <https://typer.tiangolo.com/>`_ CLI builder library. Its dependencies and\nenvironment are managed by `Poetry <https://python-poetry.org/>`_.\n\nThe CLI has a rich help system that can be accessed by passing the ``--help`` flag to\nthe main command:\n\n.. code-block:: console\n\n   jobbergate job-scripts --help\n\n\nThere is also help and parameter guides for each of the subcommands that can be accessed\nby passing them the ``--help`` flag:\n\n.. code-block:: console\n\n   jobbergate job-scripts list --help\n\nSee also:\n\n* `jobbergate-api <https://github.com/omnivector-solutions/jobbergate/jobbergate-api>`_\n\nLicense\n-------\n* `MIT <LICENSE>`_\n\n\nCopyright\n---------\n* Copyright (c) 2020 OmniVector Solutions <info@omnivector.solutions>\n',
     'author': 'Omnivector Solutions',
     'author_email': 'info@omnivector.solutions',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/omnivector-solutions/jobbergate',
```

### Comparing `jobbergate-cli-3.5.0a0/PKG-INFO` & `jobbergate-cli-3.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-cli
-Version: 3.5.0a0
+Version: 3.5.0a1
 Summary: Jobbergate CLI Client
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

