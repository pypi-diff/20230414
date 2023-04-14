# Comparing `tmp/lusid-workflow-sdk-preview-0.1.208.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.208.tar", last modified: Fri Apr 14 15:36:41 2023, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.209.tar", last modified: Fri Apr 14 16:04:20 2023, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.208.tar` & `lusid-workflow-sdk-preview-0.1.209.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7721 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     3276 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44932 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    32083 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    17241 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11241 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9372 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7455 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)    11826 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    10500 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_response.py
--rw-r--r--   0 root         (0) root         (0)     8669 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/version.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     4795 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1793 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7679 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44932 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    32083 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    17241 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11826 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    10500 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/version.py
+-rw-r--r--   0 root         (0) root         (0)     8987 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     4395 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/README.md` & `lusid-workflow-sdk-preview-0.1.209/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.208
-- Package version: 0.1.208
+- API version: 0.1.209
+- Package version: 0.1.209
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -109,15 +109,14 @@
 
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
- - [LuminesceView](docs/LuminesceView.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfTaskDefinition](docs/ResourceListOfTaskDefinition.md)
  - [Task](docs/Task.md)
  - [TaskDefinition](docs/TaskDefinition.md)
  - [TaskDefinitionVersion](docs/TaskDefinitionVersion.md)
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.208"
+__version__ = "0.1.209"
 
 # import apis into sdk package
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
@@ -33,15 +33,14 @@
 # import models into sdk package
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
-from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
 from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/task_definitions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -158,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -327,15 +327,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -504,15 +504,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -655,15 +655,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -839,15 +839,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/tasks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -171,15 +171,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -321,15 +321,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -479,15 +479,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -653,15 +653,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UpdateTaskResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/workers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -335,15 +335,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.208'
+        header_params['X-LUSID-SDK-Version'] = '0.1.209'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.208/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.209/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.208\n"\
-               "SDK Package Version: 0.1.208".\
+               "Version of the API: 0.1.209\n"\
+               "SDK Package Version: 0.1.209".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
-from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
 from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class CreateWorkerRequest(object):
+class Worker(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -38,173 +38,213 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
-        'worker_configuration': 'OneOfLuminesceView'
+        'worker_configuration': 'WorkerConfiguration',
+        'version': 'Version',
+        'links': 'list[Link]'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
-        'worker_configuration': 'workerConfiguration'
+        'worker_configuration': 'workerConfiguration',
+        'version': 'version',
+        'links': 'links'
     }
 
     required_map = {
         'id': 'required',
         'display_name': 'required',
         'description': 'optional',
-        'worker_configuration': 'required'
+        'worker_configuration': 'required',
+        'version': 'optional',
+        'links': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, worker_configuration=None, local_vars_configuration=None):  # noqa: E501
-        """CreateWorkerRequest - a model defined in OpenAPI"
+    def __init__(self, id=None, display_name=None, description=None, worker_configuration=None, version=None, links=None, local_vars_configuration=None):  # noqa: E501
+        """Worker - a model defined in OpenAPI"
         
         :param id:  (required)
         :type id: lusid_workflow.ResourceId
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param worker_configuration:  Information about how the worker should be executed (required)
-        :type worker_configuration: lusid_workflow.OneOfLuminesceView
+        :param worker_configuration:  (required)
+        :type worker_configuration: lusid_workflow.WorkerConfiguration
+        :param version: 
+        :type version: lusid_workflow.Version
+        :param links: 
+        :type links: list[lusid_workflow.Link]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._display_name = None
         self._description = None
         self._worker_configuration = None
+        self._version = None
+        self._links = None
         self.discriminator = None
 
         self.id = id
         self.display_name = display_name
         self.description = description
         self.worker_configuration = worker_configuration
+        if version is not None:
+            self.version = version
+        self.links = links
 
     @property
     def id(self):
-        """Gets the id of this CreateWorkerRequest.  # noqa: E501
+        """Gets the id of this Worker.  # noqa: E501
 
 
-        :return: The id of this CreateWorkerRequest.  # noqa: E501
+        :return: The id of this Worker.  # noqa: E501
         :rtype: lusid_workflow.ResourceId
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this CreateWorkerRequest.
+        """Sets the id of this Worker.
 
 
-        :param id: The id of this CreateWorkerRequest.  # noqa: E501
+        :param id: The id of this Worker.  # noqa: E501
         :type id: lusid_workflow.ResourceId
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def display_name(self):
-        """Gets the display_name of this CreateWorkerRequest.  # noqa: E501
+        """Gets the display_name of this Worker.  # noqa: E501
 
         Human readable name  # noqa: E501
 
-        :return: The display_name of this CreateWorkerRequest.  # noqa: E501
+        :return: The display_name of this Worker.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this CreateWorkerRequest.
+        """Sets the display_name of this Worker.
 
         Human readable name  # noqa: E501
 
-        :param display_name: The display_name of this CreateWorkerRequest.  # noqa: E501
+        :param display_name: The display_name of this Worker.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) > 512):
-            raise ValueError("Invalid value for `display_name`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) < 1):
             raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this CreateWorkerRequest.  # noqa: E501
+        """Gets the description of this Worker.  # noqa: E501
 
         Human readable description  # noqa: E501
 
-        :return: The description of this CreateWorkerRequest.  # noqa: E501
+        :return: The description of this Worker.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateWorkerRequest.
+        """Sets the description of this Worker.
 
         Human readable description  # noqa: E501
 
-        :param description: The description of this CreateWorkerRequest.  # noqa: E501
+        :param description: The description of this Worker.  # noqa: E501
         :type description: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 1024):
-            raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 0):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
-            raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
     @property
     def worker_configuration(self):
-        """Gets the worker_configuration of this CreateWorkerRequest.  # noqa: E501
+        """Gets the worker_configuration of this Worker.  # noqa: E501
 
-        Information about how the worker should be executed  # noqa: E501
 
-        :return: The worker_configuration of this CreateWorkerRequest.  # noqa: E501
-        :rtype: lusid_workflow.OneOfLuminesceView
+        :return: The worker_configuration of this Worker.  # noqa: E501
+        :rtype: lusid_workflow.WorkerConfiguration
         """
         return self._worker_configuration
 
     @worker_configuration.setter
     def worker_configuration(self, worker_configuration):
-        """Sets the worker_configuration of this CreateWorkerRequest.
+        """Sets the worker_configuration of this Worker.
 
-        Information about how the worker should be executed  # noqa: E501
 
-        :param worker_configuration: The worker_configuration of this CreateWorkerRequest.  # noqa: E501
-        :type worker_configuration: lusid_workflow.OneOfLuminesceView
+        :param worker_configuration: The worker_configuration of this Worker.  # noqa: E501
+        :type worker_configuration: lusid_workflow.WorkerConfiguration
         """
         if self.local_vars_configuration.client_side_validation and worker_configuration is None:  # noqa: E501
             raise ValueError("Invalid value for `worker_configuration`, must not be `None`")  # noqa: E501
 
         self._worker_configuration = worker_configuration
 
+    @property
+    def version(self):
+        """Gets the version of this Worker.  # noqa: E501
+
+
+        :return: The version of this Worker.  # noqa: E501
+        :rtype: lusid_workflow.Version
+        """
+        return self._version
+
+    @version.setter
+    def version(self, version):
+        """Sets the version of this Worker.
+
+
+        :param version: The version of this Worker.  # noqa: E501
+        :type version: lusid_workflow.Version
+        """
+
+        self._version = version
+
+    @property
+    def links(self):
+        """Gets the links of this Worker.  # noqa: E501
+
+
+        :return: The links of this Worker.  # noqa: E501
+        :rtype: list[lusid_workflow.Link]
+        """
+        return self._links
+
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Worker.
+
+
+        :param links: The links of this Worker.  # noqa: E501
+        :type links: list[lusid_workflow.Link]
+        """
+
+        self._links = links
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -239,18 +279,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateWorkerRequest):
+        if not isinstance(other, Worker):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateWorkerRequest):
+        if not isinstance(other, Worker):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_instance_field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class LuminesceView(object):
+class TaskInstanceField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,74 +35,97 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'view_name': 'str'
+        'name': 'str',
+        'value': 'str'
     }
 
     attribute_map = {
-        'view_name': 'viewName'
+        'name': 'name',
+        'value': 'value'
     }
 
     required_map = {
-        'view_name': 'required'
+        'name': 'required',
+        'value': 'required'
     }
 
-    def __init__(self, view_name=None, local_vars_configuration=None):  # noqa: E501
-        """LuminesceView - a model defined in OpenAPI"
+    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
+        """TaskInstanceField - a model defined in OpenAPI"
         
-        :param view_name:  Name of the view in Luminesce (required)
-        :type view_name: str
+        :param name:  The name of this Field (required)
+        :type name: str
+        :param value:  The value of this Field (required)
+        :type value: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._view_name = None
+        self._name = None
+        self._value = None
         self.discriminator = None
 
-        self.view_name = view_name
+        self.name = name
+        self.value = value
 
     @property
-    def view_name(self):
-        """Gets the view_name of this LuminesceView.  # noqa: E501
+    def name(self):
+        """Gets the name of this TaskInstanceField.  # noqa: E501
 
-        Name of the view in Luminesce  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :return: The view_name of this LuminesceView.  # noqa: E501
+        :return: The name of this TaskInstanceField.  # noqa: E501
         :rtype: str
         """
-        return self._view_name
+        return self._name
 
-    @view_name.setter
-    def view_name(self, view_name):
-        """Sets the view_name of this LuminesceView.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this TaskInstanceField.
 
-        Name of the view in Luminesce  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :param view_name: The view_name of this LuminesceView.  # noqa: E501
-        :type view_name: str
+        :param name: The name of this TaskInstanceField.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and view_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `view_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                view_name is not None and len(view_name) > 512):
-            raise ValueError("Invalid value for `view_name`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                view_name is not None and len(view_name) < 1):
-            raise ValueError("Invalid value for `view_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                view_name is not None and not re.search(r'^[\s\S]*$', view_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `view_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._view_name = view_name
+        self._name = name
+
+    @property
+    def value(self):
+        """Gets the value of this TaskInstanceField.  # noqa: E501
+
+        The value of this Field  # noqa: E501
+
+        :return: The value of this TaskInstanceField.  # noqa: E501
+        :rtype: str
+        """
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        """Sets the value of this TaskInstanceField.
+
+        The value of this Field  # noqa: E501
+
+        :param value: The value of this TaskInstanceField.  # noqa: E501
+        :type value: str
+        """
+        if self.local_vars_configuration.client_side_validation and value is None:  # noqa: E501
+            raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
+
+        self._value = value
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -138,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LuminesceView):
+        if not isinstance(other, TaskInstanceField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LuminesceView):
+        if not isinstance(other, TaskInstanceField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_list_of_task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_state_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_transition_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/trigger_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_response.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/version.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -46,31 +46,27 @@
         'type': 'type'
     }
 
     required_map = {
         'type': 'required'
     }
 
-    discriminator_value_class_map = {
-        'LuminesceView': 'LuminesceView'
-    }
-
     def __init__(self, type=None, local_vars_configuration=None):  # noqa: E501
         """WorkerConfiguration - a model defined in OpenAPI"
         
         :param type:  The type of worker (required)
         :type type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
-        self.discriminator = 'type'
+        self.discriminator = None
 
         self.type = type
 
     @property
     def type(self):
         """Gets the type of this WorkerConfiguration.  # noqa: E501
 
@@ -94,20 +90,14 @@
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 type is not None and len(type) < 1):
             raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._type = type
 
-    def get_real_child_model(self, data):
-        """Returns the real base class specified by the discriminator"""
-        discriminator_key = self.attribute_map[self.discriminator]
-        discriminator_value = data[discriminator_key]
-        return self.discriminator_value_class_map.get(discriminator_value)
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.208
+    The version of the OpenAPI document: 0.1.209
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 lusid_workflow/models/__init__.py
 lusid_workflow/models/create_task_definition_request.py
 lusid_workflow/models/create_task_request.py
 lusid_workflow/models/create_worker_request.py
 lusid_workflow/models/deleted_entity_response.py
 lusid_workflow/models/initial_state.py
 lusid_workflow/models/link.py
-lusid_workflow/models/luminesce_view.py
 lusid_workflow/models/lusid_problem_details.py
 lusid_workflow/models/lusid_validation_problem_details.py
 lusid_workflow/models/resource_id.py
 lusid_workflow/models/resource_list_of_task_definition.py
 lusid_workflow/models/task.py
 lusid_workflow/models/task_definition.py
 lusid_workflow/models/task_definition_version.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.208/setup.py` & `lusid-workflow-sdk-preview-0.1.209/setup.py`

 * *Files identical despite different names*

