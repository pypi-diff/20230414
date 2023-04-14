# Comparing `tmp/resc_vcs_scraper-1.1.0.tar.gz` & `tmp/resc_vcs_scraper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scraper-1.1.0.tar", last modified: Thu Mar  9 12:54:00 2023, max compression
+gzip compressed data, was "resc_vcs_scraper-1.2.0.tar", last modified: Fri Apr 14 15:09:35 2023, max compression
```

## Comparing `resc_vcs_scraper-1.1.0.tar` & `resc_vcs_scraper-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.431169 resc_vcs_scraper-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.431169 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 12:54:00.000000 resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/src/vcs_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/src/vcs_scraper/project_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/project_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/project_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/src/vcs_scraper/repository_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/repository_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/repository_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/src/vcs_scraper/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/static/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:00.435169 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-09 12:53:55.000000 resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_instances_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/src/vcs_scraper/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_instances_parser.py
```

### Comparing `resc_vcs_scraper-1.1.0/PKG-INFO` & `resc_vcs_scraper-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scraper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.1.0/setup.cfg` & `resc_vcs_scraper-1.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scraper
 description = Repository Scanner - Version Control System - Scraper
-version = 1.1.0
+version = 1.2.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/PKG-INFO` & `resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scraper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.1.0/src/resc_vcs_scraper.egg-info/SOURCES.txt` & `resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/common.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/configuration.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/dict_remapper.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/environment_wrapper.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/model.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/project_collector/common.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,9 +81,12 @@
 
 
 def collect_all_projects():
 
     vcs_instances_map = load_vcs_instances_into_map(env_variables[VCS_INSTANCES_FILE_PATH])
 
     for vcs_instance in vcs_instances_map:
-
-        collect_projects_from_vcs_instance(vcs_instances_map[vcs_instance])
+        try:
+            collect_projects_from_vcs_instance(vcs_instances_map[vcs_instance])
+        except ConnectionError as connection_error:
+            logger.error(f"Failed to get projects for VCSInstance {vcs_instances_map[vcs_instance].name} "
+                         f"due to {connection_error}")
```

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/repository_collector/common.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/static/logging.ini` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/static/logging.ini`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, List
 
 # Third Party
 from azure.devops.connection import Connection
 from azure.devops.exceptions import AzureDevOpsServiceError
 from azure.devops.released.core.core_client import CoreClient
 from msrest.authentication import BasicAuthentication
+from msrest.exceptions import ClientRequestError
 
 # First Party
 from vcs_scraper.model import Branch, Repository
 from vcs_scraper.vcs_connectors.azure_devops_data_mapper import map_azure_devops_branch, map_azure_devops_repository
 from vcs_scraper.vcs_connectors.vcs_connector import VCSConnector
 from vcs_scraper.vcs_instances_parser import VCSInstance
 
@@ -56,25 +57,29 @@
     @property
     def git_api_client(self):
         if not self._git_api_client:
             self._git_api_client = self.api_client.clients.get_git_client()
         return self._git_api_client
 
     def get_all_projects(self):
-        all_projects = []
-        call_results: CoreClient.GetProjectsResponseValue = self.core_api_client.get_projects()
-        projects = call_results.value
-        all_projects.extend([project.name for project in projects])
-        while call_results.continuation_token:
-            call_results: CoreClient.GetProjectsResponseValue = self.core_api_client.get_projects(
-                continuation_token=call_results.continuation_token)
+        try:
+            self._core_api_client = self.api_client.clients.get_core_client()
+            all_projects = []
+            call_results: CoreClient.GetProjectsResponseValue = self.core_api_client.get_projects()
             projects = call_results.value
             all_projects.extend([project.name for project in projects])
-
-        return all_projects
+            while call_results.continuation_token:
+                call_results: CoreClient.GetProjectsResponseValue = self.core_api_client.get_projects(
+                    continuation_token=call_results.continuation_token)
+                projects = call_results.value
+                all_projects.extend([project.name for project in projects])
+
+            return all_projects
+        except ClientRequestError as ex:
+            raise ConnectionError(ex) from ex
 
     def project_exists(self, project_key: str) -> bool:
         return bool(self.core_api_client.get_project(project_key))
 
     def get_repos(self, project_key):
         return list(repo.as_dict() for repo in self.git_api_client.get_repositories(project_key))
```

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,19 @@
                 url=self.url,
                 session=session,
                 proxies={"no_proxy": self.proxy}
             )
         return self._api_client
 
     def get_all_projects(self):
-        return [project["key"] for project in self.api_client.project_list()]
+        try:
+            return [project["key"] for project in self.api_client.project_list()]
+        except (requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout, requests.exceptions.ProxyError,
+                requests.exceptions.ReadTimeout, requests.exceptions.SSLError, requests.exceptions.HTTPError) as ex:
+            raise ConnectionError(ex) from ex
 
     def project_exists(self, project_key: str) -> bool:
         return bool(self.api_client.project(project_key))
 
     def get_repos(self, project_key):
         return list(self.api_client.repo_all_list(project_key))
```

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/github_public_connector.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/github_public_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Library
 import os
 from typing import List
 
 # Third Party
+import requests
 from github import Github
 from github.Branch import Branch as GithubBranch
 from github.Repository import Repository as GithubRepository
 
 # First Party
 from vcs_scraper.model import Branch, Repository, VCSInstance
 from vcs_scraper.vcs_connectors.vcs_connector import VCSConnector
@@ -26,15 +27,19 @@
     @property
     def api_client(self):
         if not self._api_client:
             self._api_client = Github(login_or_token=self.access_token)
         return self._api_client
 
     def get_all_projects(self) -> List[str]:
-        return [user.login for user in self.api_client.get_users()]
+        try:
+            return [user.login for user in self.api_client.get_users()]
+        except (requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout, requests.exceptions.ProxyError,
+                requests.exceptions.ReadTimeout, requests.exceptions.SSLError, requests.exceptions.HTTPError) as ex:
+            raise ConnectionError(ex) from ex
 
     def get_repos(self, project_key) -> List[dict]:
         repository_list = []
         repos = list(self.api_client.get_user(project_key).get_repos())
         for repo in repos:
             repo_details = self.get_repository_details(project_key=project_key, repository_name=repo.name)
             repo_dict = {
```

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/vcs_connector.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.1.0/src/vcs_scraper/vcs_instances_parser.py` & `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_instances_parser.py`

 * *Files identical despite different names*

