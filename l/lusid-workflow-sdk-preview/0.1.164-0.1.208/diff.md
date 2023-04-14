# Comparing `tmp/lusid-workflow-sdk-preview-0.1.164.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.164.tar", last modified: Thu Mar  9 17:32:50 2023, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.208.tar", last modified: Fri Apr 14 15:36:41 2023, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.164.tar` & `lusid-workflow-sdk-preview-0.1.208.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8125 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     3223 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      225 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67113 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    21185 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api/task_instances_api.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     2180 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11832 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/create_task_instance_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/field_instance.py
--rw-r--r--   0 root         (0) root         (0)     4909 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/field_schema.py
--rw-r--r--   0 root         (0) root         (0)     4885 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/history_entry.py
--rw-r--r--   0 root         (0) root         (0)     5038 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)    10137 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    11342 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output_schema.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output_type.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7455 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7399 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/resource_list_of_task_instance.py
--rw-r--r--   0 root         (0) root         (0)     4564 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/state.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/status.py
--rw-r--r--   0 root         (0) root         (0)    13037 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/task_definition_id.py
--rw-r--r--   0 root         (0) root         (0)    17566 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/task_instance.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/transit_task_instance_request.py
--rw-r--r--   0 root         (0) root         (0)     7186 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/transition.py
--rw-r--r--   0 root         (0) root         (0)     4662 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/trigger.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/trigger_invocation_response.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)     6439 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1767 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 17:32:50.000000 lusid-workflow-sdk-preview-0.1.164/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-09 17:32:25.000000 lusid-workflow-sdk-preview-0.1.164/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7721 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44932 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    32083 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    17241 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9372 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11826 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    10500 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/version.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 15:36:41.000000 lusid-workflow-sdk-preview-0.1.208/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-14 15:36:18.000000 lusid-workflow-sdk-preview-0.1.208/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/README.md` & `lusid-workflow-sdk-preview-0.1.208/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.164
-- Package version: 0.1.164
+- API version: 0.1.208
+- Package version: 0.1.208
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -71,15 +71,15 @@
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with lusid_workflow.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = lusid_workflow.TaskDefinitionsApi(api_client)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","fields":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"states":[{"type":"Input","name":"Submitted"},{"type":"Internal","name":"InProgress"},{"type":"Internal","name":"SendingSurvey"},{"type":"Output","name":"Done"},{"type":"Output","name":"SurveyNotSent"},{"type":"Output","name":"NotDone"}],"transitions":[{"from":"Submitted","to":"InProgress","trigger":"start","guard":"fields.assignee exists AND fields.assignee NOT eq ''"},{"from":"InProgress","to":"SendingSurvey","trigger":"resolve","guard":"fields.resolutionDetail exists AND fields.resolutionDetail NOT eq ''","output":"sendSurvey"},{"from":"SendingSurvey","to":"Done","trigger":"success"},{"from":"SendingSurvey","to":"SurveyNotSent","trigger":"failure"},{"from":"SendingSurvey","to":"NotDone","trigger":"timeout"},{"from":"InProgress","to":"NotDone","trigger":"cancel","guard":"fields.cancellationDetail exists AND fields.cancellationDetail NOT eq ''"}],"triggers":[{"name":"start","schema":{"type":"External","timeInState":0}},{"name":"cancel","schema":{"type":"External","timeInState":0}},{"name":"resolve","schema":{"type":"External","timeInState":0}},{"name":"timeout","schema":{"type":"Timeout","timeInState":30}},{"name":"success","schema":{"type":"WebHook","timeInState":0,"responseCodes":{"in":[200]}}},{"name":"failure","schema":{"type":"WebHook","timeInState":0,"responseCodes":{"notIn":[200]}}}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"outputs":[{"name":"a web hook","schema":{"requestDetails":{"method":"Get","url":"www.zzz.com","parameters":[{"kind":"Query","key":"client_id","value":"ZZZ"}],"expectedHttpResponseCodes":["200"]},"type":"WebHook"}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields.assignee exists AND fields.assignee NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields.resolutionDetail exists AND fields.resolutionDetail NOT eq ''"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields.cancellationDetail exists AND fields.cancellationDetail NOT eq ''"}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
 
     try:
         # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.
         api_response = api_instance.create_task_definition(create_task_definition_request)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
@@ -89,53 +89,54 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.
-*TaskDefinitionsApi* | [**create_task_instance**](docs/TaskDefinitionsApi.md#create_task_instance) | **POST** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] CreateTaskInstance: Create a new Task Instance.
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition.
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition.
-*TaskDefinitionsApi* | [**get_task_instances_for_definition**](docs/TaskDefinitionsApi.md#get_task_instances_for_definition) | **GET** /api/taskdefinitions/{scope}/{code}/instances | [EXPERIMENTAL] GetTaskInstancesForDefinition: Get all Task Instances based on a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions/{scope} | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition.
-*TaskInstancesApi* | [**get_task_instance**](docs/TaskInstancesApi.md#get_task_instance) | **GET** /api/taskinstances/{id} | [EXPERIMENTAL] GetTaskInstance: Get a Task Instance.
-*TaskInstancesApi* | [**invoke_trigger**](docs/TaskInstancesApi.md#invoke_trigger) | **POST** /api/taskinstances/{id} | [EXPERIMENTAL] InvokeTrigger: Invoke a Task Instance Trigger.
+*TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task.
+*TasksApi* | [**delete_task**](docs/TasksApi.md#delete_task) | **DELETE** /api/tasks/{id} | [EXPERIMENTAL] DeleteTask: Delete a Task.
+*TasksApi* | [**get_task**](docs/TasksApi.md#get_task) | **GET** /api/tasks/{id} | [EXPERIMENTAL] GetTask: Get a Task.
+*TasksApi* | [**update_task**](docs/TasksApi.md#update_task) | **POST** /api/tasks/{id} | [EXPERIMENTAL] UpdateTask: Update a Task.
+*WorkersApi* | [**create_worker**](docs/WorkersApi.md#create_worker) | **POST** /api/workers | [EXPERIMENTAL] CreateWorker: Endpoint For Creating a Worker
+*WorkersApi* | [**get_worker**](docs/WorkersApi.md#get_worker) | **GET** /api/workers/{scope}/{code} | [EXPERIMENTAL] GetWorker: Endpoint for Retrieving a Worker
 
 
 ## Documentation For Models
 
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
- - [CreateTaskInstanceRequest](docs/CreateTaskInstanceRequest.md)
+ - [CreateTaskRequest](docs/CreateTaskRequest.md)
+ - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
- - [FieldInstance](docs/FieldInstance.md)
- - [FieldSchema](docs/FieldSchema.md)
- - [HistoryEntry](docs/HistoryEntry.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
+ - [LuminesceView](docs/LuminesceView.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
- - [Output](docs/Output.md)
- - [OutputSchema](docs/OutputSchema.md)
- - [OutputType](docs/OutputType.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfTaskDefinition](docs/ResourceListOfTaskDefinition.md)
- - [ResourceListOfTaskInstance](docs/ResourceListOfTaskInstance.md)
- - [State](docs/State.md)
- - [Status](docs/Status.md)
+ - [Task](docs/Task.md)
  - [TaskDefinition](docs/TaskDefinition.md)
- - [TaskDefinitionId](docs/TaskDefinitionId.md)
- - [TaskInstance](docs/TaskInstance.md)
- - [TransitTaskInstanceRequest](docs/TransitTaskInstanceRequest.md)
- - [Transition](docs/Transition.md)
- - [Trigger](docs/Trigger.md)
- - [TriggerInvocationResponse](docs/TriggerInvocationResponse.md)
+ - [TaskDefinitionVersion](docs/TaskDefinitionVersion.md)
+ - [TaskFieldDefinition](docs/TaskFieldDefinition.md)
+ - [TaskInstanceField](docs/TaskInstanceField.md)
+ - [TaskStateDefinition](docs/TaskStateDefinition.md)
+ - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
+ - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
  - [TriggerSchema](docs/TriggerSchema.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
+ - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
+ - [UpdateTaskResponse](docs/UpdateTaskResponse.md)
+ - [Version](docs/Version.md)
+ - [Worker](docs/Worker.md)
+ - [WorkerConfiguration](docs/WorkerConfiguration.md)
 
 
 ## Documentation For Authorization
 
 
 ## oauth2
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,64 +3,64 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.164"
+__version__ = "0.1.208"
 
 # import apis into sdk package
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
-from lusid_workflow.api.task_instances_api import TaskInstancesApi
+from lusid_workflow.api.tasks_api import TasksApi
+from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.configuration import Configuration
 from lusid_workflow.exceptions import OpenApiException
 from lusid_workflow.exceptions import ApiTypeError
 from lusid_workflow.exceptions import ApiValueError
 from lusid_workflow.exceptions import ApiKeyError
 from lusid_workflow.exceptions import ApiException
 # import models into sdk package
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
-from lusid_workflow.models.create_task_instance_request import CreateTaskInstanceRequest
+from lusid_workflow.models.create_task_request import CreateTaskRequest
+from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
-from lusid_workflow.models.field_instance import FieldInstance
-from lusid_workflow.models.field_schema import FieldSchema
-from lusid_workflow.models.history_entry import HistoryEntry
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
+from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from lusid_workflow.models.output import Output
-from lusid_workflow.models.output_schema import OutputSchema
-from lusid_workflow.models.output_type import OutputType
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
-from lusid_workflow.models.resource_list_of_task_instance import ResourceListOfTaskInstance
-from lusid_workflow.models.state import State
-from lusid_workflow.models.status import Status
+from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
-from lusid_workflow.models.task_definition_id import TaskDefinitionId
-from lusid_workflow.models.task_instance import TaskInstance
-from lusid_workflow.models.transit_task_instance_request import TransitTaskInstanceRequest
-from lusid_workflow.models.transition import Transition
-from lusid_workflow.models.trigger import Trigger
-from lusid_workflow.models.trigger_invocation_response import TriggerInvocationResponse
+from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
+from lusid_workflow.models.task_field_definition import TaskFieldDefinition
+from lusid_workflow.models.task_instance_field import TaskInstanceField
+from lusid_workflow.models.task_state_definition import TaskStateDefinition
+from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
+from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
+from lusid_workflow.models.update_task_request import UpdateTaskRequest
+from lusid_workflow.models.update_task_response import UpdateTaskResponse
+from lusid_workflow.models.version import Version
+from lusid_workflow.models.worker import Worker
+from lusid_workflow.models.worker_configuration import WorkerConfiguration
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
 from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
 from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
 from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api/task_definitions_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -20,22 +20,19 @@
 
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
-from lusid_workflow.models.create_task_instance_request import CreateTaskInstanceRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
-from lusid_workflow.models.resource_list_of_task_instance import ResourceListOfTaskInstance
 from lusid_workflow.models.task_definition import TaskDefinition
-from lusid_workflow.models.task_instance import TaskInstance
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 
 
 class TaskDefinitionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -161,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
+        header_params['X-LUSID-SDK-Version'] = '0.1.208'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -188,212 +185,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def create_task_instance(self, scope, code, create_task_instance_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTaskInstance: Create a new Task Instance.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_task_instance(scope, code, create_task_instance_request, async_req=True)
-        >>> result = thread.get()
-
-        :param scope: The scope of task definition to create task instance from (required)
-        :type scope: str
-        :param code: The code of task definition to create a task instance from (required)
-        :type code: str
-        :param create_task_instance_request: Request to create task instance (required)
-        :type create_task_instance_request: CreateTaskInstanceRequest
-        :param task_instance_scope: The scope of the task instance should be in; set to 'default' if not provided.
-        :type task_instance_scope: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: TaskInstance
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.create_task_instance_with_http_info(scope, code, create_task_instance_request, **kwargs)  # noqa: E501
-
-    def create_task_instance_with_http_info(self, scope, code, create_task_instance_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTaskInstance: Create a new Task Instance.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_task_instance_with_http_info(scope, code, create_task_instance_request, async_req=True)
-        >>> result = thread.get()
-
-        :param scope: The scope of task definition to create task instance from (required)
-        :type scope: str
-        :param code: The code of task definition to create a task instance from (required)
-        :type code: str
-        :param create_task_instance_request: Request to create task instance (required)
-        :type create_task_instance_request: CreateTaskInstanceRequest
-        :param task_instance_scope: The scope of the task instance should be in; set to 'default' if not provided.
-        :type task_instance_scope: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: (TaskInstance, int, HTTPHeaderDict)
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'scope',
-            'code',
-            'create_task_instance_request',
-            'task_instance_scope'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method create_task_instance" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'scope' is set
-        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
-                                                        local_var_params['scope'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `scope` when calling `create_task_instance`")  # noqa: E501
-        # verify the required parameter 'code' is set
-        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
-                                                        local_var_params['code'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `code` when calling `create_task_instance`")  # noqa: E501
-        # verify the required parameter 'create_task_instance_request' is set
-        if self.api_client.client_side_validation and ('create_task_instance_request' not in local_var_params or  # noqa: E501
-                                                        local_var_params['create_task_instance_request'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `create_task_instance_request` when calling `create_task_instance`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['scope']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `create_task_instance`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['scope']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `create_task_instance`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `create_task_instance`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['code']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `create_task_instance`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['code']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `create_task_instance`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `create_task_instance`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('task_instance_scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['task_instance_scope']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `task_instance_scope` when calling `create_task_instance`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('task_instance_scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['task_instance_scope']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `task_instance_scope` when calling `create_task_instance`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'task_instance_scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['task_instance_scope']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `task_instance_scope` when calling `create_task_instance`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
-        collection_formats = {}
-
-        path_params = {}
-        if 'scope' in local_var_params:
-            path_params['scope'] = local_var_params['scope']  # noqa: E501
-        if 'code' in local_var_params:
-            path_params['code'] = local_var_params['code']  # noqa: E501
-
-        query_params = []
-        if 'task_instance_scope' in local_var_params and local_var_params['task_instance_scope'] is not None:  # noqa: E501
-            query_params.append(('taskInstanceScope', local_var_params['task_instance_scope']))  # noqa: E501
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'create_task_instance_request' in local_var_params:
-            body_params = local_var_params['create_task_instance_request']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
-
-        # Authentication setting
-        auth_settings = ['oauth2']  # noqa: E501
-
-        response_types_map = {
-            201: "TaskInstance",
-            400: "LusidValidationProblemDetails",
-        }
-
-        return self.api_client.call_api(
-            '/api/taskdefinitions/{scope}/{code}', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def delete_task_definition(self, scope, code, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_task_definition(scope, code, async_req=True)
@@ -528,15 +327,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
+        header_params['X-LUSID-SDK-Version'] = '0.1.208'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -705,15 +504,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
+        header_params['X-LUSID-SDK-Version'] = '0.1.208'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -733,191 +532,14 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def get_task_instances_for_definition(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTaskInstancesForDefinition: Get all Task Instances based on a Task Definition  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_task_instances_for_definition(scope, code, async_req=True)
-        >>> result = thread.get()
-
-        :param scope: The scope of the source Task Definition and the Task Instances so be searched under. (required)
-        :type scope: str
-        :param code: The code that identifies the source Task Definition (required)
-        :type code: str
-        :param as_at: AsAt time to retrieve stated Task Instances. Default to latest AsAt if not provided.
-        :type as_at: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: ResourceListOfTaskInstance
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_task_instances_for_definition_with_http_info(scope, code, **kwargs)  # noqa: E501
-
-    def get_task_instances_for_definition_with_http_info(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTaskInstancesForDefinition: Get all Task Instances based on a Task Definition  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_task_instances_for_definition_with_http_info(scope, code, async_req=True)
-        >>> result = thread.get()
-
-        :param scope: The scope of the source Task Definition and the Task Instances so be searched under. (required)
-        :type scope: str
-        :param code: The code that identifies the source Task Definition (required)
-        :type code: str
-        :param as_at: AsAt time to retrieve stated Task Instances. Default to latest AsAt if not provided.
-        :type as_at: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: (ResourceListOfTaskInstance, int, HTTPHeaderDict)
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'scope',
-            'code',
-            'as_at'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_task_instances_for_definition" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'scope' is set
-        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
-                                                        local_var_params['scope'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `scope` when calling `get_task_instances_for_definition`")  # noqa: E501
-        # verify the required parameter 'code' is set
-        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
-                                                        local_var_params['code'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `code` when calling `get_task_instances_for_definition`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['scope']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `get_task_instances_for_definition`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['scope']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `get_task_instances_for_definition`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `get_task_instances_for_definition`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['code']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `get_task_instances_for_definition`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['code']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `get_task_instances_for_definition`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `code` when calling `get_task_instances_for_definition`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
-        collection_formats = {}
-
-        path_params = {}
-        if 'scope' in local_var_params:
-            path_params['scope'] = local_var_params['scope']  # noqa: E501
-        if 'code' in local_var_params:
-            path_params['code'] = local_var_params['code']  # noqa: E501
-
-        query_params = []
-        if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
-            query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
-
-        header_params = dict(local_var_params.get('_headers', {}))
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
-
-        # Authentication setting
-        auth_settings = ['oauth2']  # noqa: E501
-
-        response_types_map = {
-            200: "ResourceListOfTaskInstance",
-            400: "LusidValidationProblemDetails",
-            404: "str",
-        }
-
-        return self.api_client.call_api(
-            '/api/taskdefinitions/{scope}/{code}/instances', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_types_map=response_types_map,
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def list_task_definitions(self, scope, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] ListTaskDefinitions: List Task Definitions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_task_definitions(scope, async_req=True)
@@ -997,14 +619,18 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method list_task_definitions" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'scope' is set
+        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
+                                                        local_var_params['scope'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `list_task_definitions`")  # noqa: E501
 
         if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
                                                         len(local_var_params['scope']) > 64):  # noqa: E501
             raise ApiValueError("Invalid value for parameter `scope` when calling `list_task_definitions`, length must be less than or equal to `64`")  # noqa: E501
         if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
                                                         len(local_var_params['scope']) < 1):  # noqa: E501
             raise ApiValueError("Invalid value for parameter `scope` when calling `list_task_definitions`, length must be greater than or equal to `1`")  # noqa: E501
@@ -1029,15 +655,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
+        header_params['X-LUSID-SDK-Version'] = '0.1.208'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -1213,15 +839,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.164'
+        header_params['X-LUSID-SDK-Version'] = '0.1.208'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
-        self.user_agent = 'OpenAPI-Generator/0.1.164/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.208/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
-               "Version of the API: 0.1.164\n"\
-               "SDK Package Version: 0.1.164".\
+               "Version of the API: 0.1.208\n"\
+               "SDK Package Version: 0.1.208".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,43 +2,42 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
-from lusid_workflow.models.create_task_instance_request import CreateTaskInstanceRequest
+from lusid_workflow.models.create_task_request import CreateTaskRequest
+from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
-from lusid_workflow.models.field_instance import FieldInstance
-from lusid_workflow.models.field_schema import FieldSchema
-from lusid_workflow.models.history_entry import HistoryEntry
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
+from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from lusid_workflow.models.output import Output
-from lusid_workflow.models.output_schema import OutputSchema
-from lusid_workflow.models.output_type import OutputType
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
-from lusid_workflow.models.resource_list_of_task_instance import ResourceListOfTaskInstance
-from lusid_workflow.models.state import State
-from lusid_workflow.models.status import Status
+from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
-from lusid_workflow.models.task_definition_id import TaskDefinitionId
-from lusid_workflow.models.task_instance import TaskInstance
-from lusid_workflow.models.transit_task_instance_request import TransitTaskInstanceRequest
-from lusid_workflow.models.transition import Transition
-from lusid_workflow.models.trigger import Trigger
-from lusid_workflow.models.trigger_invocation_response import TriggerInvocationResponse
+from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
+from lusid_workflow.models.task_field_definition import TaskFieldDefinition
+from lusid_workflow.models.task_instance_field import TaskInstanceField
+from lusid_workflow.models.task_state_definition import TaskStateDefinition
+from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
+from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
+from lusid_workflow.models.update_task_request import UpdateTaskRequest
+from lusid_workflow.models.update_task_response import UpdateTaskResponse
+from lusid_workflow.models.version import Version
+from lusid_workflow.models.worker import Worker
+from lusid_workflow.models.worker_configuration import WorkerConfiguration
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/create_task_definition_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,95 +38,88 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
-        'fields': 'list[FieldSchema]',
-        'states': 'list[State]',
-        'transitions': 'list[Transition]',
-        'triggers': 'list[Trigger]',
+        'states': 'list[TaskStateDefinition]',
+        'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
-        'outputs': 'list[Output]'
+        'triggers': 'list[TransitionTriggerDefinition]',
+        'transitions': 'list[TaskTransitionDefinition]'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
-        'fields': 'fields',
         'states': 'states',
-        'transitions': 'transitions',
-        'triggers': 'triggers',
+        'field_schema': 'fieldSchema',
         'initial_state': 'initialState',
-        'outputs': 'outputs'
+        'triggers': 'triggers',
+        'transitions': 'transitions'
     }
 
     required_map = {
         'id': 'optional',
         'display_name': 'optional',
         'description': 'optional',
-        'fields': 'optional',
         'states': 'optional',
-        'transitions': 'optional',
-        'triggers': 'optional',
+        'field_schema': 'optional',
         'initial_state': 'optional',
-        'outputs': 'optional'
+        'triggers': 'optional',
+        'transitions': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, fields=None, states=None, transitions=None, triggers=None, initial_state=None, outputs=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, local_vars_configuration=None):  # noqa: E501
         """CreateTaskDefinitionRequest - a model defined in OpenAPI"
         
         :param id: 
         :type id: lusid_workflow.ResourceId
         :param display_name:  Human readable name
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param fields:  Defines the fields associated with this Task
-        :type fields: list[lusid_workflow.FieldSchema]
         :param states:  The states this Task Definition operates over
-        :type states: list[lusid_workflow.State]
-        :param transitions:  Transitions
-        :type transitions: list[lusid_workflow.Transition]
-        :param triggers:  Triggers
-        :type triggers: list[lusid_workflow.Trigger]
+        :type states: list[lusid_workflow.TaskStateDefinition]
+        :param field_schema:  Defines the fields associated with this Task
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         :param initial_state: 
         :type initial_state: lusid_workflow.InitialState
-        :param outputs:  The Outputs of this Task
-        :type outputs: list[lusid_workflow.Output]
+        :param triggers:  Triggers
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
+        :param transitions:  Transitions
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._display_name = None
         self._description = None
-        self._fields = None
         self._states = None
-        self._transitions = None
-        self._triggers = None
+        self._field_schema = None
         self._initial_state = None
-        self._outputs = None
+        self._triggers = None
+        self._transitions = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.display_name = display_name
         self.description = description
-        self.fields = fields
         self.states = states
-        self.transitions = transitions
-        self.triggers = triggers
+        self.field_schema = field_schema
         if initial_state is not None:
             self.initial_state = initial_state
-        self.outputs = outputs
+        self.triggers = triggers
+        self.transitions = transitions
 
     @property
     def id(self):
         """Gets the id of this CreateTaskDefinitionRequest.  # noqa: E501
 
 
         :return: The id of this CreateTaskDefinitionRequest.  # noqa: E501
@@ -188,104 +181,58 @@
         :param description: The description of this CreateTaskDefinitionRequest.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
-    def fields(self):
-        """Gets the fields of this CreateTaskDefinitionRequest.  # noqa: E501
-
-        Defines the fields associated with this Task  # noqa: E501
-
-        :return: The fields of this CreateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.FieldSchema]
-        """
-        return self._fields
-
-    @fields.setter
-    def fields(self, fields):
-        """Sets the fields of this CreateTaskDefinitionRequest.
-
-        Defines the fields associated with this Task  # noqa: E501
-
-        :param fields: The fields of this CreateTaskDefinitionRequest.  # noqa: E501
-        :type fields: list[lusid_workflow.FieldSchema]
-        """
-
-        self._fields = fields
-
-    @property
     def states(self):
         """Gets the states of this CreateTaskDefinitionRequest.  # noqa: E501
 
         The states this Task Definition operates over  # noqa: E501
 
         :return: The states of this CreateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.State]
+        :rtype: list[lusid_workflow.TaskStateDefinition]
         """
         return self._states
 
     @states.setter
     def states(self, states):
         """Sets the states of this CreateTaskDefinitionRequest.
 
         The states this Task Definition operates over  # noqa: E501
 
         :param states: The states of this CreateTaskDefinitionRequest.  # noqa: E501
-        :type states: list[lusid_workflow.State]
+        :type states: list[lusid_workflow.TaskStateDefinition]
         """
 
         self._states = states
 
     @property
-    def transitions(self):
-        """Gets the transitions of this CreateTaskDefinitionRequest.  # noqa: E501
-
-        Transitions  # noqa: E501
-
-        :return: The transitions of this CreateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.Transition]
-        """
-        return self._transitions
-
-    @transitions.setter
-    def transitions(self, transitions):
-        """Sets the transitions of this CreateTaskDefinitionRequest.
-
-        Transitions  # noqa: E501
-
-        :param transitions: The transitions of this CreateTaskDefinitionRequest.  # noqa: E501
-        :type transitions: list[lusid_workflow.Transition]
-        """
-
-        self._transitions = transitions
-
-    @property
-    def triggers(self):
-        """Gets the triggers of this CreateTaskDefinitionRequest.  # noqa: E501
+    def field_schema(self):
+        """Gets the field_schema of this CreateTaskDefinitionRequest.  # noqa: E501
 
-        Triggers  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :return: The triggers of this CreateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.Trigger]
+        :return: The field_schema of this CreateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskFieldDefinition]
         """
-        return self._triggers
+        return self._field_schema
 
-    @triggers.setter
-    def triggers(self, triggers):
-        """Sets the triggers of this CreateTaskDefinitionRequest.
+    @field_schema.setter
+    def field_schema(self, field_schema):
+        """Sets the field_schema of this CreateTaskDefinitionRequest.
 
-        Triggers  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :param triggers: The triggers of this CreateTaskDefinitionRequest.  # noqa: E501
-        :type triggers: list[lusid_workflow.Trigger]
+        :param field_schema: The field_schema of this CreateTaskDefinitionRequest.  # noqa: E501
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         """
 
-        self._triggers = triggers
+        self._field_schema = field_schema
 
     @property
     def initial_state(self):
         """Gets the initial_state of this CreateTaskDefinitionRequest.  # noqa: E501
 
 
         :return: The initial_state of this CreateTaskDefinitionRequest.  # noqa: E501
@@ -301,35 +248,58 @@
         :param initial_state: The initial_state of this CreateTaskDefinitionRequest.  # noqa: E501
         :type initial_state: lusid_workflow.InitialState
         """
 
         self._initial_state = initial_state
 
     @property
-    def outputs(self):
-        """Gets the outputs of this CreateTaskDefinitionRequest.  # noqa: E501
+    def triggers(self):
+        """Gets the triggers of this CreateTaskDefinitionRequest.  # noqa: E501
 
-        The Outputs of this Task  # noqa: E501
+        Triggers  # noqa: E501
 
-        :return: The outputs of this CreateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.Output]
+        :return: The triggers of this CreateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.TransitionTriggerDefinition]
         """
-        return self._outputs
+        return self._triggers
 
-    @outputs.setter
-    def outputs(self, outputs):
-        """Sets the outputs of this CreateTaskDefinitionRequest.
+    @triggers.setter
+    def triggers(self, triggers):
+        """Sets the triggers of this CreateTaskDefinitionRequest.
 
-        The Outputs of this Task  # noqa: E501
+        Triggers  # noqa: E501
 
-        :param outputs: The outputs of this CreateTaskDefinitionRequest.  # noqa: E501
-        :type outputs: list[lusid_workflow.Output]
+        :param triggers: The triggers of this CreateTaskDefinitionRequest.  # noqa: E501
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         """
 
-        self._outputs = outputs
+        self._triggers = triggers
+
+    @property
+    def transitions(self):
+        """Gets the transitions of this CreateTaskDefinitionRequest.  # noqa: E501
+
+        Transitions  # noqa: E501
+
+        :return: The transitions of this CreateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskTransitionDefinition]
+        """
+        return self._transitions
+
+    @transitions.setter
+    def transitions(self, transitions):
+        """Sets the transitions of this CreateTaskDefinitionRequest.
+
+        Transitions  # noqa: E501
+
+        :param transitions: The transitions of this CreateTaskDefinitionRequest.  # noqa: E501
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        """
+
+        self._transitions = transitions
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/create_task_instance_request.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/link.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class CreateTaskInstanceRequest(object):
+class Link(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,72 +35,151 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'correlation_id': 'str'
+        'relation': 'str',
+        'href': 'str',
+        'description': 'str',
+        'method': 'str'
     }
 
     attribute_map = {
-        'correlation_id': 'correlationId'
+        'relation': 'relation',
+        'href': 'href',
+        'description': 'description',
+        'method': 'method'
     }
 
     required_map = {
-        'correlation_id': 'optional'
+        'relation': 'required',
+        'href': 'required',
+        'description': 'optional',
+        'method': 'required'
     }
 
-    def __init__(self, correlation_id=None, local_vars_configuration=None):  # noqa: E501
-        """CreateTaskInstanceRequest - a model defined in OpenAPI"
+    def __init__(self, relation=None, href=None, description=None, method=None, local_vars_configuration=None):  # noqa: E501
+        """Link - a model defined in OpenAPI"
         
-        :param correlation_id:  An identifier to allow correlation across the application tier
-        :type correlation_id: str
+        :param relation:  (required)
+        :type relation: str
+        :param href:  (required)
+        :type href: str
+        :param description: 
+        :type description: str
+        :param method:  (required)
+        :type method: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._correlation_id = None
+        self._relation = None
+        self._href = None
+        self._description = None
+        self._method = None
         self.discriminator = None
 
-        self.correlation_id = correlation_id
+        self.relation = relation
+        self.href = href
+        self.description = description
+        self.method = method
 
     @property
-    def correlation_id(self):
-        """Gets the correlation_id of this CreateTaskInstanceRequest.  # noqa: E501
+    def relation(self):
+        """Gets the relation of this Link.  # noqa: E501
 
-        An identifier to allow correlation across the application tier  # noqa: E501
 
-        :return: The correlation_id of this CreateTaskInstanceRequest.  # noqa: E501
+        :return: The relation of this Link.  # noqa: E501
         :rtype: str
         """
-        return self._correlation_id
+        return self._relation
 
-    @correlation_id.setter
-    def correlation_id(self, correlation_id):
-        """Sets the correlation_id of this CreateTaskInstanceRequest.
-
-        An identifier to allow correlation across the application tier  # noqa: E501
-
-        :param correlation_id: The correlation_id of this CreateTaskInstanceRequest.  # noqa: E501
-        :type correlation_id: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                correlation_id is not None and len(correlation_id) > 64):
-            raise ValueError("Invalid value for `correlation_id`, length must be less than or equal to `64`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                correlation_id is not None and len(correlation_id) < 36):
-            raise ValueError("Invalid value for `correlation_id`, length must be greater than or equal to `36`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                correlation_id is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', correlation_id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `correlation_id`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+    @relation.setter
+    def relation(self, relation):
+        """Sets the relation of this Link.
 
-        self._correlation_id = correlation_id
+
+        :param relation: The relation of this Link.  # noqa: E501
+        :type relation: str
+        """
+        if self.local_vars_configuration.client_side_validation and relation is None:  # noqa: E501
+            raise ValueError("Invalid value for `relation`, must not be `None`")  # noqa: E501
+
+        self._relation = relation
+
+    @property
+    def href(self):
+        """Gets the href of this Link.  # noqa: E501
+
+
+        :return: The href of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._href
+
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Link.
+
+
+        :param href: The href of this Link.  # noqa: E501
+        :type href: str
+        """
+        if self.local_vars_configuration.client_side_validation and href is None:  # noqa: E501
+            raise ValueError("Invalid value for `href`, must not be `None`")  # noqa: E501
+
+        self._href = href
+
+    @property
+    def description(self):
+        """Gets the description of this Link.  # noqa: E501
+
+
+        :return: The description of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Link.
+
+
+        :param description: The description of this Link.  # noqa: E501
+        :type description: str
+        """
+
+        self._description = description
+
+    @property
+    def method(self):
+        """Gets the method of this Link.  # noqa: E501
+
+
+        :return: The method of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._method
+
+    @method.setter
+    def method(self, method):
+        """Sets the method of this Link.
+
+
+        :param method: The method of this Link.  # noqa: E501
+        :type method: str
+        """
+        if self.local_vars_configuration.client_side_validation and method is None:  # noqa: E501
+            raise ValueError("Invalid value for `method`, must not be `None`")  # noqa: E501
+
+        self._method = method
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -136,18 +215,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateTaskInstanceRequest):
+        if not isinstance(other, Link):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateTaskInstanceRequest):
+        if not isinstance(other, Link):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/deleted_entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/field_instance.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_instance_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class FieldInstance(object):
+class TaskInstanceField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -50,17 +50,17 @@
 
     required_map = {
         'name': 'required',
         'value': 'required'
     }
 
     def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
-        """FieldInstance - a model defined in OpenAPI"
+        """TaskInstanceField - a model defined in OpenAPI"
         
-        :param name:  The flattened path of a field, eg: investments.bonds.usd.tbill (required)
+        :param name:  The name of this Field (required)
         :type name: str
         :param value:  The value of this Field (required)
         :type value: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
@@ -71,55 +71,55 @@
         self.discriminator = None
 
         self.name = name
         self.value = value
 
     @property
     def name(self):
-        """Gets the name of this FieldInstance.  # noqa: E501
+        """Gets the name of this TaskInstanceField.  # noqa: E501
 
-        The flattened path of a field, eg: investments.bonds.usd.tbill  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :return: The name of this FieldInstance.  # noqa: E501
+        :return: The name of this TaskInstanceField.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this FieldInstance.
+        """Sets the name of this TaskInstanceField.
 
-        The flattened path of a field, eg: investments.bonds.usd.tbill  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :param name: The name of this FieldInstance.  # noqa: E501
+        :param name: The name of this TaskInstanceField.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def value(self):
-        """Gets the value of this FieldInstance.  # noqa: E501
+        """Gets the value of this TaskInstanceField.  # noqa: E501
 
         The value of this Field  # noqa: E501
 
-        :return: The value of this FieldInstance.  # noqa: E501
+        :return: The value of this TaskInstanceField.  # noqa: E501
         :rtype: str
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this FieldInstance.
+        """Sets the value of this TaskInstanceField.
 
         The value of this Field  # noqa: E501
 
-        :param value: The value of this FieldInstance.  # noqa: E501
+        :param value: The value of this TaskInstanceField.  # noqa: E501
         :type value: str
         """
         if self.local_vars_configuration.client_side_validation and value is None:  # noqa: E501
             raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
 
         self._value = value
 
@@ -161,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FieldInstance):
+        if not isinstance(other, TaskInstanceField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FieldInstance):
+        if not isinstance(other, TaskInstanceField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/field_schema.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_field_definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class FieldSchema(object):
+class TaskFieldDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -50,19 +50,19 @@
 
     required_map = {
         'name': 'optional',
         'type': 'optional'
     }
 
     def __init__(self, name=None, type=None, local_vars_configuration=None):  # noqa: E501
-        """FieldSchema - a model defined in OpenAPI"
+        """TaskFieldDefinition - a model defined in OpenAPI"
         
-        :param name:  The flattened path of a field, eg: investments.bonds.usd.tbill
+        :param name:  The name of this Field
         :type name: str
-        :param type:  The JSON type of the data: https://datatracker.ietf.org/doc/html/rfc8259
+        :param type:  The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")
         :type type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
@@ -71,53 +71,53 @@
         self.discriminator = None
 
         self.name = name
         self.type = type
 
     @property
     def name(self):
-        """Gets the name of this FieldSchema.  # noqa: E501
+        """Gets the name of this TaskFieldDefinition.  # noqa: E501
 
-        The flattened path of a field, eg: investments.bonds.usd.tbill  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :return: The name of this FieldSchema.  # noqa: E501
+        :return: The name of this TaskFieldDefinition.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this FieldSchema.
+        """Sets the name of this TaskFieldDefinition.
 
-        The flattened path of a field, eg: investments.bonds.usd.tbill  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :param name: The name of this FieldSchema.  # noqa: E501
+        :param name: The name of this TaskFieldDefinition.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
     @property
     def type(self):
-        """Gets the type of this FieldSchema.  # noqa: E501
+        """Gets the type of this TaskFieldDefinition.  # noqa: E501
 
-        The JSON type of the data: https://datatracker.ietf.org/doc/html/rfc8259  # noqa: E501
+        The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")  # noqa: E501
 
-        :return: The type of this FieldSchema.  # noqa: E501
+        :return: The type of this TaskFieldDefinition.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this FieldSchema.
+        """Sets the type of this TaskFieldDefinition.
 
-        The JSON type of the data: https://datatracker.ietf.org/doc/html/rfc8259  # noqa: E501
+        The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")  # noqa: E501
 
-        :param type: The type of this FieldSchema.  # noqa: E501
+        :param type: The type of this TaskFieldDefinition.  # noqa: E501
         :type type: str
         """
 
         self._type = type
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -157,18 +157,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FieldSchema):
+        if not isinstance(other, TaskFieldDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FieldSchema):
+        if not isinstance(other, TaskFieldDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/history_entry.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class HistoryEntry(object):
+class TransitionTriggerDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,94 +35,92 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'time_stamp': 'datetime',
-        'entry': 'str'
+        'name': 'str',
+        'trigger': 'TriggerSchema'
     }
 
     attribute_map = {
-        'time_stamp': 'timeStamp',
-        'entry': 'entry'
+        'name': 'name',
+        'trigger': 'trigger'
     }
 
     required_map = {
-        'time_stamp': 'optional',
-        'entry': 'optional'
+        'name': 'optional',
+        'trigger': 'optional'
     }
 
-    def __init__(self, time_stamp=None, entry=None, local_vars_configuration=None):  # noqa: E501
-        """HistoryEntry - a model defined in OpenAPI"
+    def __init__(self, name=None, trigger=None, local_vars_configuration=None):  # noqa: E501
+        """TransitionTriggerDefinition - a model defined in OpenAPI"
         
-        :param time_stamp:  The timestamp for the entry
-        :type time_stamp: datetime
-        :param entry:  The information itself
-        :type entry: str
+        :param name:  The key/Name of this Trigger
+        :type name: str
+        :param trigger: 
+        :type trigger: lusid_workflow.TriggerSchema
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._time_stamp = None
-        self._entry = None
+        self._name = None
+        self._trigger = None
         self.discriminator = None
 
-        if time_stamp is not None:
-            self.time_stamp = time_stamp
-        self.entry = entry
+        self.name = name
+        if trigger is not None:
+            self.trigger = trigger
 
     @property
-    def time_stamp(self):
-        """Gets the time_stamp of this HistoryEntry.  # noqa: E501
+    def name(self):
+        """Gets the name of this TransitionTriggerDefinition.  # noqa: E501
 
-        The timestamp for the entry  # noqa: E501
+        The key/Name of this Trigger  # noqa: E501
 
-        :return: The time_stamp of this HistoryEntry.  # noqa: E501
-        :rtype: datetime
+        :return: The name of this TransitionTriggerDefinition.  # noqa: E501
+        :rtype: str
         """
-        return self._time_stamp
+        return self._name
 
-    @time_stamp.setter
-    def time_stamp(self, time_stamp):
-        """Sets the time_stamp of this HistoryEntry.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this TransitionTriggerDefinition.
 
-        The timestamp for the entry  # noqa: E501
+        The key/Name of this Trigger  # noqa: E501
 
-        :param time_stamp: The time_stamp of this HistoryEntry.  # noqa: E501
-        :type time_stamp: datetime
+        :param name: The name of this TransitionTriggerDefinition.  # noqa: E501
+        :type name: str
         """
 
-        self._time_stamp = time_stamp
+        self._name = name
 
     @property
-    def entry(self):
-        """Gets the entry of this HistoryEntry.  # noqa: E501
+    def trigger(self):
+        """Gets the trigger of this TransitionTriggerDefinition.  # noqa: E501
 
-        The information itself  # noqa: E501
 
-        :return: The entry of this HistoryEntry.  # noqa: E501
-        :rtype: str
+        :return: The trigger of this TransitionTriggerDefinition.  # noqa: E501
+        :rtype: lusid_workflow.TriggerSchema
         """
-        return self._entry
+        return self._trigger
 
-    @entry.setter
-    def entry(self, entry):
-        """Sets the entry of this HistoryEntry.
+    @trigger.setter
+    def trigger(self, trigger):
+        """Sets the trigger of this TransitionTriggerDefinition.
 
-        The information itself  # noqa: E501
 
-        :param entry: The entry of this HistoryEntry.  # noqa: E501
-        :type entry: str
+        :param trigger: The trigger of this TransitionTriggerDefinition.  # noqa: E501
+        :type trigger: lusid_workflow.TriggerSchema
         """
 
-        self._entry = entry
+        self._trigger = trigger
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -158,18 +156,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HistoryEntry):
+        if not isinstance(other, TransitionTriggerDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, HistoryEntry):
+        if not isinstance(other, TransitionTriggerDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/initial_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -52,17 +52,17 @@
         'name': 'optional',
         'required_fields': 'optional'
     }
 
     def __init__(self, name=None, required_fields=None, local_vars_configuration=None):  # noqa: E501
         """InitialState - a model defined in OpenAPI"
         
-        :param name:  The initial State of the Task Instance
+        :param name:  The Initial State of the Task
         :type name: str
-        :param required_fields:  Required input Fields for the initial State
+        :param required_fields:  Required input Fields for the Initial State
         :type required_fields: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
@@ -73,49 +73,49 @@
         self.name = name
         self.required_fields = required_fields
 
     @property
     def name(self):
         """Gets the name of this InitialState.  # noqa: E501
 
-        The initial State of the Task Instance  # noqa: E501
+        The Initial State of the Task  # noqa: E501
 
         :return: The name of this InitialState.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this InitialState.
 
-        The initial State of the Task Instance  # noqa: E501
+        The Initial State of the Task  # noqa: E501
 
         :param name: The name of this InitialState.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
     @property
     def required_fields(self):
         """Gets the required_fields of this InitialState.  # noqa: E501
 
-        Required input Fields for the initial State  # noqa: E501
+        Required input Fields for the Initial State  # noqa: E501
 
         :return: The required_fields of this InitialState.  # noqa: E501
         :rtype: list[str]
         """
         return self._required_fields
 
     @required_fields.setter
     def required_fields(self, required_fields):
         """Sets the required_fields of this InitialState.
 
-        Required input Fields for the initial State  # noqa: E501
+        Required input Fields for the Initial State  # noqa: E501
 
         :param required_fields: The required_fields of this InitialState.  # noqa: E501
         :type required_fields: list[str]
         """
 
         self._required_fields = required_fields
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class Link(object):
+class UpdateTaskResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,151 +35,124 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'relation': 'str',
-        'href': 'str',
-        'description': 'str',
-        'method': 'str'
+        'was_successful': 'bool',
+        'as_at': 'datetime',
+        'message': 'str'
     }
 
     attribute_map = {
-        'relation': 'relation',
-        'href': 'href',
-        'description': 'description',
-        'method': 'method'
+        'was_successful': 'wasSuccessful',
+        'as_at': 'asAt',
+        'message': 'message'
     }
 
     required_map = {
-        'relation': 'required',
-        'href': 'required',
-        'description': 'optional',
-        'method': 'required'
+        'was_successful': 'optional',
+        'as_at': 'optional',
+        'message': 'optional'
     }
 
-    def __init__(self, relation=None, href=None, description=None, method=None, local_vars_configuration=None):  # noqa: E501
-        """Link - a model defined in OpenAPI"
+    def __init__(self, was_successful=None, as_at=None, message=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateTaskResponse - a model defined in OpenAPI"
         
-        :param relation:  (required)
-        :type relation: str
-        :param href:  (required)
-        :type href: str
-        :param description: 
-        :type description: str
-        :param method:  (required)
-        :type method: str
+        :param was_successful:  A flag indicating success
+        :type was_successful: bool
+        :param as_at:  If successful, the AsAt time
+        :type as_at: datetime
+        :param message:  Any messaging
+        :type message: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._relation = None
-        self._href = None
-        self._description = None
-        self._method = None
+        self._was_successful = None
+        self._as_at = None
+        self._message = None
         self.discriminator = None
 
-        self.relation = relation
-        self.href = href
-        self.description = description
-        self.method = method
+        if was_successful is not None:
+            self.was_successful = was_successful
+        self.as_at = as_at
+        self.message = message
 
     @property
-    def relation(self):
-        """Gets the relation of this Link.  # noqa: E501
+    def was_successful(self):
+        """Gets the was_successful of this UpdateTaskResponse.  # noqa: E501
 
+        A flag indicating success  # noqa: E501
 
-        :return: The relation of this Link.  # noqa: E501
-        :rtype: str
+        :return: The was_successful of this UpdateTaskResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._relation
+        return self._was_successful
 
-    @relation.setter
-    def relation(self, relation):
-        """Sets the relation of this Link.
+    @was_successful.setter
+    def was_successful(self, was_successful):
+        """Sets the was_successful of this UpdateTaskResponse.
 
+        A flag indicating success  # noqa: E501
 
-        :param relation: The relation of this Link.  # noqa: E501
-        :type relation: str
+        :param was_successful: The was_successful of this UpdateTaskResponse.  # noqa: E501
+        :type was_successful: bool
         """
-        if self.local_vars_configuration.client_side_validation and relation is None:  # noqa: E501
-            raise ValueError("Invalid value for `relation`, must not be `None`")  # noqa: E501
 
-        self._relation = relation
+        self._was_successful = was_successful
 
     @property
-    def href(self):
-        """Gets the href of this Link.  # noqa: E501
-
+    def as_at(self):
+        """Gets the as_at of this UpdateTaskResponse.  # noqa: E501
 
-        :return: The href of this Link.  # noqa: E501
-        :rtype: str
-        """
-        return self._href
+        If successful, the AsAt time  # noqa: E501
 
-    @href.setter
-    def href(self, href):
-        """Sets the href of this Link.
-
-
-        :param href: The href of this Link.  # noqa: E501
-        :type href: str
-        """
-        if self.local_vars_configuration.client_side_validation and href is None:  # noqa: E501
-            raise ValueError("Invalid value for `href`, must not be `None`")  # noqa: E501
-
-        self._href = href
-
-    @property
-    def description(self):
-        """Gets the description of this Link.  # noqa: E501
-
-
-        :return: The description of this Link.  # noqa: E501
-        :rtype: str
+        :return: The as_at of this UpdateTaskResponse.  # noqa: E501
+        :rtype: datetime
         """
-        return self._description
+        return self._as_at
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this Link.
+    @as_at.setter
+    def as_at(self, as_at):
+        """Sets the as_at of this UpdateTaskResponse.
 
+        If successful, the AsAt time  # noqa: E501
 
-        :param description: The description of this Link.  # noqa: E501
-        :type description: str
+        :param as_at: The as_at of this UpdateTaskResponse.  # noqa: E501
+        :type as_at: datetime
         """
 
-        self._description = description
+        self._as_at = as_at
 
     @property
-    def method(self):
-        """Gets the method of this Link.  # noqa: E501
+    def message(self):
+        """Gets the message of this UpdateTaskResponse.  # noqa: E501
 
+        Any messaging  # noqa: E501
 
-        :return: The method of this Link.  # noqa: E501
+        :return: The message of this UpdateTaskResponse.  # noqa: E501
         :rtype: str
         """
-        return self._method
+        return self._message
 
-    @method.setter
-    def method(self, method):
-        """Sets the method of this Link.
+    @message.setter
+    def message(self, message):
+        """Sets the message of this UpdateTaskResponse.
 
+        Any messaging  # noqa: E501
 
-        :param method: The method of this Link.  # noqa: E501
-        :type method: str
+        :param message: The message of this UpdateTaskResponse.  # noqa: E501
+        :type message: str
         """
-        if self.local_vars_configuration.client_side_validation and method is None:  # noqa: E501
-            raise ValueError("Invalid value for `method`, must not be `None`")  # noqa: E501
 
-        self._method = method
+        self._message = message
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -215,18 +188,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Link):
+        if not isinstance(other, UpdateTaskResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Link):
+        if not isinstance(other, UpdateTaskResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_problem_details.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -42,43 +42,40 @@
         'name': 'str',
         'error_details': 'list[dict(str, str)]',
         'code': 'int',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
-        'instance': 'str',
-        'extensions': 'dict(str, object)'
+        'instance': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'error_details': 'errorDetails',
         'code': 'code',
         'type': 'type',
         'title': 'title',
         'status': 'status',
         'detail': 'detail',
-        'instance': 'instance',
-        'extensions': 'extensions'
+        'instance': 'instance'
     }
 
     required_map = {
         'name': 'required',
         'error_details': 'optional',
         'code': 'required',
         'type': 'optional',
         'title': 'optional',
         'status': 'optional',
         'detail': 'optional',
-        'instance': 'optional',
-        'extensions': 'optional'
+        'instance': 'optional'
     }
 
-    def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, extensions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
         :type error_details: list[dict(str, str)]
         :param code:  (required)
@@ -89,42 +86,38 @@
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
         :type detail: str
         :param instance: 
         :type instance: str
-        :param extensions: 
-        :type extensions: dict(str, object)
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._error_details = None
         self._code = None
         self._type = None
         self._title = None
         self._status = None
         self._detail = None
         self._instance = None
-        self._extensions = None
         self.discriminator = None
 
         self.name = name
         self.error_details = error_details
         self.code = code
         self.type = type
         self.title = title
         self.status = status
         self.detail = detail
         self.instance = instance
-        self.extensions = extensions
 
     @property
     def name(self):
         """Gets the name of this LusidProblemDetails.  # noqa: E501
 
 
         :return: The name of this LusidProblemDetails.  # noqa: E501
@@ -138,14 +131,17 @@
 
 
         :param name: The name of this LusidProblemDetails.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._name = name
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidProblemDetails.  # noqa: E501
 
@@ -290,35 +286,14 @@
 
         :param instance: The instance of this LusidProblemDetails.  # noqa: E501
         :type instance: str
         """
 
         self._instance = instance
 
-    @property
-    def extensions(self):
-        """Gets the extensions of this LusidProblemDetails.  # noqa: E501
-
-
-        :return: The extensions of this LusidProblemDetails.  # noqa: E501
-        :rtype: dict(str, object)
-        """
-        return self._extensions
-
-    @extensions.setter
-    def extensions(self, extensions):
-        """Sets the extensions of this LusidProblemDetails.
-
-
-        :param extensions: The extensions of this LusidProblemDetails.  # noqa: E501
-        :type extensions: dict(str, object)
-        """
-
-        self._extensions = extensions
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -43,45 +43,42 @@
         'error_details': 'list[dict(str, str)]',
         'code': 'int',
         'errors': 'dict(str, list[str])',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
-        'instance': 'str',
-        'extensions': 'dict(str, object)'
+        'instance': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'error_details': 'errorDetails',
         'code': 'code',
         'errors': 'errors',
         'type': 'type',
         'title': 'title',
         'status': 'status',
         'detail': 'detail',
-        'instance': 'instance',
-        'extensions': 'extensions'
+        'instance': 'instance'
     }
 
     required_map = {
         'name': 'required',
         'error_details': 'optional',
         'code': 'required',
         'errors': 'optional',
         'type': 'optional',
         'title': 'optional',
         'status': 'optional',
         'detail': 'optional',
-        'instance': 'optional',
-        'extensions': 'optional'
+        'instance': 'optional'
     }
 
-    def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, extensions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidValidationProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
         :type error_details: list[dict(str, str)]
         :param code:  (required)
@@ -94,16 +91,14 @@
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
         :type detail: str
         :param instance: 
         :type instance: str
-        :param extensions: 
-        :type extensions: dict(str, object)
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
@@ -111,27 +106,25 @@
         self._code = None
         self._errors = None
         self._type = None
         self._title = None
         self._status = None
         self._detail = None
         self._instance = None
-        self._extensions = None
         self.discriminator = None
 
         self.name = name
         self.error_details = error_details
         self.code = code
         self.errors = errors
         self.type = type
         self.title = title
         self.status = status
         self.detail = detail
         self.instance = instance
-        self.extensions = extensions
 
     @property
     def name(self):
         """Gets the name of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The name of this LusidValidationProblemDetails.  # noqa: E501
@@ -145,14 +138,17 @@
 
 
         :param name: The name of this LusidValidationProblemDetails.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._name = name
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidValidationProblemDetails.  # noqa: E501
 
@@ -318,35 +314,14 @@
 
         :param instance: The instance of this LusidValidationProblemDetails.  # noqa: E501
         :type instance: str
         """
 
         self._instance = instance
 
-    @property
-    def extensions(self):
-        """Gets the extensions of this LusidValidationProblemDetails.  # noqa: E501
-
-
-        :return: The extensions of this LusidValidationProblemDetails.  # noqa: E501
-        :rtype: dict(str, object)
-        """
-        return self._extensions
-
-    @extensions.setter
-    def extensions(self, extensions):
-        """Sets the extensions of this LusidValidationProblemDetails.
-
-
-        :param extensions: The extensions of this LusidValidationProblemDetails.  # noqa: E501
-        :type extensions: dict(str, object)
-        """
-
-        self._extensions = extensions
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/luminesce_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class Output(object):
+class LuminesceView(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,95 +35,74 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'name': 'str',
-        'schema': 'OutputSchema'
+        'view_name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'schema': 'schema'
+        'view_name': 'viewName'
     }
 
     required_map = {
-        'name': 'required',
-        'schema': 'required'
+        'view_name': 'required'
     }
 
-    def __init__(self, name=None, schema=None, local_vars_configuration=None):  # noqa: E501
-        """Output - a model defined in OpenAPI"
+    def __init__(self, view_name=None, local_vars_configuration=None):  # noqa: E501
+        """LuminesceView - a model defined in OpenAPI"
         
-        :param name:  The Name of this Output (required)
-        :type name: str
-        :param schema:  (required)
-        :type schema: lusid_workflow.OutputSchema
+        :param view_name:  Name of the view in Luminesce (required)
+        :type view_name: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._schema = None
+        self._view_name = None
         self.discriminator = None
 
-        self.name = name
-        self.schema = schema
+        self.view_name = view_name
 
     @property
-    def name(self):
-        """Gets the name of this Output.  # noqa: E501
+    def view_name(self):
+        """Gets the view_name of this LuminesceView.  # noqa: E501
 
-        The Name of this Output  # noqa: E501
+        Name of the view in Luminesce  # noqa: E501
 
-        :return: The name of this Output.  # noqa: E501
+        :return: The view_name of this LuminesceView.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._view_name
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this Output.
+    @view_name.setter
+    def view_name(self, view_name):
+        """Sets the view_name of this LuminesceView.
 
-        The Name of this Output  # noqa: E501
+        Name of the view in Luminesce  # noqa: E501
 
-        :param name: The name of this Output.  # noqa: E501
-        :type name: str
+        :param view_name: The view_name of this LuminesceView.  # noqa: E501
+        :type view_name: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and view_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `view_name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                view_name is not None and len(view_name) > 512):
+            raise ValueError("Invalid value for `view_name`, length must be less than or equal to `512`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                view_name is not None and len(view_name) < 1):
+            raise ValueError("Invalid value for `view_name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                view_name is not None and not re.search(r'^[\s\S]*$', view_name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `view_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._name = name
-
-    @property
-    def schema(self):
-        """Gets the schema of this Output.  # noqa: E501
-
-
-        :return: The schema of this Output.  # noqa: E501
-        :rtype: lusid_workflow.OutputSchema
-        """
-        return self._schema
-
-    @schema.setter
-    def schema(self, schema):
-        """Sets the schema of this Output.
-
-
-        :param schema: The schema of this Output.  # noqa: E501
-        :type schema: lusid_workflow.OutputSchema
-        """
-        if self.local_vars_configuration.client_side_validation and schema is None:  # noqa: E501
-            raise ValueError("Invalid value for `schema`, must not be `None`")  # noqa: E501
-
-        self._schema = schema
+        self._view_name = view_name
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -159,18 +138,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Output):
+        if not isinstance(other, LuminesceView):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Output):
+        if not isinstance(other, LuminesceView):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output_schema.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/trigger_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class OutputSchema(object):
+class TriggerSchema(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,59 +35,60 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'OutputType'
+        'type': 'str'
     }
 
     attribute_map = {
         'type': 'type'
     }
 
     required_map = {
         'type': 'optional'
     }
 
     def __init__(self, type=None, local_vars_configuration=None):  # noqa: E501
-        """OutputSchema - a model defined in OpenAPI"
+        """TriggerSchema - a model defined in OpenAPI"
         
-        :param type: 
-        :type type: lusid_workflow.OutputType
+        :param type:  The type of Trigger
+        :type type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self.discriminator = None
 
-        if type is not None:
-            self.type = type
+        self.type = type
 
     @property
     def type(self):
-        """Gets the type of this OutputSchema.  # noqa: E501
+        """Gets the type of this TriggerSchema.  # noqa: E501
 
+        The type of Trigger  # noqa: E501
 
-        :return: The type of this OutputSchema.  # noqa: E501
-        :rtype: lusid_workflow.OutputType
+        :return: The type of this TriggerSchema.  # noqa: E501
+        :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this OutputSchema.
+        """Sets the type of this TriggerSchema.
 
+        The type of Trigger  # noqa: E501
 
-        :param type: The type of this OutputSchema.  # noqa: E501
-        :type type: lusid_workflow.OutputType
+        :param type: The type of this TriggerSchema.  # noqa: E501
+        :type type: str
         """
 
         self._type = type
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
@@ -126,18 +127,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OutputSchema):
+        if not isinstance(other, TriggerSchema):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OutputSchema):
+        if not isinstance(other, TriggerSchema):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/output_type.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_state_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,57 +18,81 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class OutputType(object):
+class TaskStateDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
-    allowed enum values
-    """
-    UNDEFINED = "Undefined"
-    WEBHOOK = "WebHook"
-
-    allowable_values = [UNDEFINED, WEBHOOK]  # noqa: E501
-
-    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'name': 'str'
     }
 
     attribute_map = {
+        'name': 'name'
     }
 
     required_map = {
+        'name': 'optional'
     }
 
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """OutputType - a model defined in OpenAPI"
+    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
+        """TaskStateDefinition - a model defined in OpenAPI"
         
+        :param name:  The Name of this State
+        :type name: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
+
+        self._name = None
         self.discriminator = None
 
+        self.name = name
+
+    @property
+    def name(self):
+        """Gets the name of this TaskStateDefinition.  # noqa: E501
+
+        The Name of this State  # noqa: E501
+
+        :return: The name of this TaskStateDefinition.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this TaskStateDefinition.
+
+        The Name of this State  # noqa: E501
+
+        :param name: The name of this TaskStateDefinition.  # noqa: E501
+        :type name: str
+        """
+
+        self._name = name
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -103,18 +127,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OutputType):
+        if not isinstance(other, TaskStateDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OutputType):
+        if not isinstance(other, TaskStateDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/resource_list_of_task_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/state.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/worker_configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class State(object):
+class WorkerConfiguration(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,93 +35,78 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
-        'name': 'str'
+        'type': 'str'
     }
 
     attribute_map = {
-        'type': 'type',
-        'name': 'name'
+        'type': 'type'
     }
 
     required_map = {
-        'type': 'optional',
-        'name': 'optional'
+        'type': 'required'
     }
 
-    def __init__(self, type=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """State - a model defined in OpenAPI"
+    discriminator_value_class_map = {
+        'LuminesceView': 'LuminesceView'
+    }
+
+    def __init__(self, type=None, local_vars_configuration=None):  # noqa: E501
+        """WorkerConfiguration - a model defined in OpenAPI"
         
-        :param type:  Input/Internal/Output
+        :param type:  The type of worker (required)
         :type type: str
-        :param name:  The Name of this State
-        :type name: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
-        self._name = None
-        self.discriminator = None
+        self.discriminator = 'type'
 
         self.type = type
-        self.name = name
 
     @property
     def type(self):
-        """Gets the type of this State.  # noqa: E501
+        """Gets the type of this WorkerConfiguration.  # noqa: E501
 
-        Input/Internal/Output  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :return: The type of this State.  # noqa: E501
+        :return: The type of this WorkerConfiguration.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this State.
+        """Sets the type of this WorkerConfiguration.
 
-        Input/Internal/Output  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :param type: The type of this State.  # noqa: E501
+        :param type: The type of this WorkerConfiguration.  # noqa: E501
         :type type: str
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._type = type
 
-    @property
-    def name(self):
-        """Gets the name of this State.  # noqa: E501
-
-        The Name of this State  # noqa: E501
-
-        :return: The name of this State.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this State.
-
-        The Name of this State  # noqa: E501
-
-        :param name: The name of this State.  # noqa: E501
-        :type name: str
-        """
-
-        self._name = name
+    def get_real_child_model(self, data):
+        """Returns the real base class specified by the discriminator"""
+        discriminator_key = self.attribute_map[self.discriminator]
+        discriminator_value = data[discriminator_key]
+        return self.discriminator_value_class_map.get(discriminator_value)
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -157,18 +142,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, State):
+        if not isinstance(other, WorkerConfiguration):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, State):
+        if not isinstance(other, WorkerConfiguration):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/status.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition_version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,61 +18,82 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class Status(object):
+class TaskDefinitionVersion(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
-    allowed enum values
-    """
-    UNDEFINED = "Undefined"
-    NOTSTARTED = "NotStarted"
-    INPROGRESS = "InProgress"
-    FAILED = "Failed"
-    COMPLETE = "Complete"
-    BLOCKED = "Blocked"
-
-    allowable_values = [UNDEFINED, NOTSTARTED, INPROGRESS, FAILED, COMPLETE, BLOCKED]  # noqa: E501
-
-    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'as_at_modified': 'datetime'
     }
 
     attribute_map = {
+        'as_at_modified': 'asAtModified'
     }
 
     required_map = {
+        'as_at_modified': 'optional'
     }
 
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """Status - a model defined in OpenAPI"
+    def __init__(self, as_at_modified=None, local_vars_configuration=None):  # noqa: E501
+        """TaskDefinitionVersion - a model defined in OpenAPI"
         
+        :param as_at_modified:  The asAt datetime of the Task Definition used by this Task
+        :type as_at_modified: datetime
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
+
+        self._as_at_modified = None
         self.discriminator = None
 
+        if as_at_modified is not None:
+            self.as_at_modified = as_at_modified
+
+    @property
+    def as_at_modified(self):
+        """Gets the as_at_modified of this TaskDefinitionVersion.  # noqa: E501
+
+        The asAt datetime of the Task Definition used by this Task  # noqa: E501
+
+        :return: The as_at_modified of this TaskDefinitionVersion.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._as_at_modified
+
+    @as_at_modified.setter
+    def as_at_modified(self, as_at_modified):
+        """Sets the as_at_modified of this TaskDefinitionVersion.
+
+        The asAt datetime of the Task Definition used by this Task  # noqa: E501
+
+        :param as_at_modified: The as_at_modified of this TaskDefinitionVersion.  # noqa: E501
+        :type as_at_modified: datetime
+        """
+
+        self._as_at_modified = as_at_modified
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -107,18 +128,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Status):
+        if not isinstance(other, TaskDefinitionVersion):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Status):
+        if not isinstance(other, TaskDefinitionVersion):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,126 +35,141 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'task_definition_id': 'TaskDefinitionId',
+        'id': 'ResourceId',
+        'version': 'Version',
         'display_name': 'str',
         'description': 'str',
-        'states': 'list[State]',
-        'fields_schema': 'list[FieldSchema]',
+        'states': 'list[TaskStateDefinition]',
+        'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
-        'triggers': 'list[Trigger]',
-        'outputs': 'list[Output]',
-        'transitions': 'list[Transition]',
-        'instances': 'list[str]'
+        'triggers': 'list[TransitionTriggerDefinition]',
+        'transitions': 'list[TaskTransitionDefinition]'
     }
 
     attribute_map = {
-        'task_definition_id': 'taskDefinitionId',
+        'id': 'id',
+        'version': 'version',
         'display_name': 'displayName',
         'description': 'description',
         'states': 'states',
-        'fields_schema': 'fieldsSchema',
+        'field_schema': 'fieldSchema',
         'initial_state': 'initialState',
         'triggers': 'triggers',
-        'outputs': 'outputs',
-        'transitions': 'transitions',
-        'instances': 'instances'
+        'transitions': 'transitions'
     }
 
     required_map = {
-        'task_definition_id': 'optional',
+        'id': 'optional',
+        'version': 'optional',
         'display_name': 'optional',
         'description': 'optional',
         'states': 'optional',
-        'fields_schema': 'optional',
+        'field_schema': 'optional',
         'initial_state': 'optional',
         'triggers': 'optional',
-        'outputs': 'optional',
-        'transitions': 'optional',
-        'instances': 'optional'
+        'transitions': 'optional'
     }
 
-    def __init__(self, task_definition_id=None, display_name=None, description=None, states=None, fields_schema=None, initial_state=None, triggers=None, outputs=None, transitions=None, instances=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, version=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, local_vars_configuration=None):  # noqa: E501
         """TaskDefinition - a model defined in OpenAPI"
         
-        :param task_definition_id: 
-        :type task_definition_id: lusid_workflow.TaskDefinitionId
+        :param id: 
+        :type id: lusid_workflow.ResourceId
+        :param version: 
+        :type version: lusid_workflow.Version
         :param display_name:  Human readable name
         :type display_name: str
         :param description:  Human readable description
         :type description: str
         :param states:  The states this Task Definition operates over
-        :type states: list[lusid_workflow.State]
-        :param fields_schema:  The Fields that this Task Definition operates on
-        :type fields_schema: list[lusid_workflow.FieldSchema]
+        :type states: list[lusid_workflow.TaskStateDefinition]
+        :param field_schema:  The Fields that this Task Definition operates on
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         :param initial_state: 
         :type initial_state: lusid_workflow.InitialState
         :param triggers:  The Triggers for State transition
-        :type triggers: list[lusid_workflow.Trigger]
-        :param outputs:  The Outputs of this Task
-        :type outputs: list[lusid_workflow.Output]
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         :param transitions:  The Transitions between States
-        :type transitions: list[lusid_workflow.Transition]
-        :param instances:  Each Definition will have a number of instances associated with it
-        :type instances: list[str]
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._task_definition_id = None
+        self._id = None
+        self._version = None
         self._display_name = None
         self._description = None
         self._states = None
-        self._fields_schema = None
+        self._field_schema = None
         self._initial_state = None
         self._triggers = None
-        self._outputs = None
         self._transitions = None
-        self._instances = None
         self.discriminator = None
 
-        if task_definition_id is not None:
-            self.task_definition_id = task_definition_id
+        if id is not None:
+            self.id = id
+        if version is not None:
+            self.version = version
         self.display_name = display_name
         self.description = description
         self.states = states
-        self.fields_schema = fields_schema
+        self.field_schema = field_schema
         if initial_state is not None:
             self.initial_state = initial_state
         self.triggers = triggers
-        self.outputs = outputs
         self.transitions = transitions
-        self.instances = instances
 
     @property
-    def task_definition_id(self):
-        """Gets the task_definition_id of this TaskDefinition.  # noqa: E501
+    def id(self):
+        """Gets the id of this TaskDefinition.  # noqa: E501
 
 
-        :return: The task_definition_id of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.TaskDefinitionId
+        :return: The id of this TaskDefinition.  # noqa: E501
+        :rtype: lusid_workflow.ResourceId
         """
-        return self._task_definition_id
+        return self._id
 
-    @task_definition_id.setter
-    def task_definition_id(self, task_definition_id):
-        """Sets the task_definition_id of this TaskDefinition.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this TaskDefinition.
 
 
-        :param task_definition_id: The task_definition_id of this TaskDefinition.  # noqa: E501
-        :type task_definition_id: lusid_workflow.TaskDefinitionId
+        :param id: The id of this TaskDefinition.  # noqa: E501
+        :type id: lusid_workflow.ResourceId
         """
 
-        self._task_definition_id = task_definition_id
+        self._id = id
+
+    @property
+    def version(self):
+        """Gets the version of this TaskDefinition.  # noqa: E501
+
+
+        :return: The version of this TaskDefinition.  # noqa: E501
+        :rtype: lusid_workflow.Version
+        """
+        return self._version
+
+    @version.setter
+    def version(self, version):
+        """Sets the version of this TaskDefinition.
+
+
+        :param version: The version of this TaskDefinition.  # noqa: E501
+        :type version: lusid_workflow.Version
+        """
+
+        self._version = version
 
     @property
     def display_name(self):
         """Gets the display_name of this TaskDefinition.  # noqa: E501
 
         Human readable name  # noqa: E501
 
@@ -201,52 +216,52 @@
     @property
     def states(self):
         """Gets the states of this TaskDefinition.  # noqa: E501
 
         The states this Task Definition operates over  # noqa: E501
 
         :return: The states of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.State]
+        :rtype: list[lusid_workflow.TaskStateDefinition]
         """
         return self._states
 
     @states.setter
     def states(self, states):
         """Sets the states of this TaskDefinition.
 
         The states this Task Definition operates over  # noqa: E501
 
         :param states: The states of this TaskDefinition.  # noqa: E501
-        :type states: list[lusid_workflow.State]
+        :type states: list[lusid_workflow.TaskStateDefinition]
         """
 
         self._states = states
 
     @property
-    def fields_schema(self):
-        """Gets the fields_schema of this TaskDefinition.  # noqa: E501
+    def field_schema(self):
+        """Gets the field_schema of this TaskDefinition.  # noqa: E501
 
         The Fields that this Task Definition operates on  # noqa: E501
 
-        :return: The fields_schema of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.FieldSchema]
+        :return: The field_schema of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskFieldDefinition]
         """
-        return self._fields_schema
+        return self._field_schema
 
-    @fields_schema.setter
-    def fields_schema(self, fields_schema):
-        """Sets the fields_schema of this TaskDefinition.
+    @field_schema.setter
+    def field_schema(self, field_schema):
+        """Sets the field_schema of this TaskDefinition.
 
         The Fields that this Task Definition operates on  # noqa: E501
 
-        :param fields_schema: The fields_schema of this TaskDefinition.  # noqa: E501
-        :type fields_schema: list[lusid_workflow.FieldSchema]
+        :param field_schema: The field_schema of this TaskDefinition.  # noqa: E501
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         """
 
-        self._fields_schema = fields_schema
+        self._field_schema = field_schema
 
     @property
     def initial_state(self):
         """Gets the initial_state of this TaskDefinition.  # noqa: E501
 
 
         :return: The initial_state of this TaskDefinition.  # noqa: E501
@@ -268,99 +283,53 @@
     @property
     def triggers(self):
         """Gets the triggers of this TaskDefinition.  # noqa: E501
 
         The Triggers for State transition  # noqa: E501
 
         :return: The triggers of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.Trigger]
+        :rtype: list[lusid_workflow.TransitionTriggerDefinition]
         """
         return self._triggers
 
     @triggers.setter
     def triggers(self, triggers):
         """Sets the triggers of this TaskDefinition.
 
         The Triggers for State transition  # noqa: E501
 
         :param triggers: The triggers of this TaskDefinition.  # noqa: E501
-        :type triggers: list[lusid_workflow.Trigger]
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         """
 
         self._triggers = triggers
 
     @property
-    def outputs(self):
-        """Gets the outputs of this TaskDefinition.  # noqa: E501
-
-        The Outputs of this Task  # noqa: E501
-
-        :return: The outputs of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.Output]
-        """
-        return self._outputs
-
-    @outputs.setter
-    def outputs(self, outputs):
-        """Sets the outputs of this TaskDefinition.
-
-        The Outputs of this Task  # noqa: E501
-
-        :param outputs: The outputs of this TaskDefinition.  # noqa: E501
-        :type outputs: list[lusid_workflow.Output]
-        """
-
-        self._outputs = outputs
-
-    @property
     def transitions(self):
         """Gets the transitions of this TaskDefinition.  # noqa: E501
 
         The Transitions between States  # noqa: E501
 
         :return: The transitions of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.Transition]
+        :rtype: list[lusid_workflow.TaskTransitionDefinition]
         """
         return self._transitions
 
     @transitions.setter
     def transitions(self, transitions):
         """Sets the transitions of this TaskDefinition.
 
         The Transitions between States  # noqa: E501
 
         :param transitions: The transitions of this TaskDefinition.  # noqa: E501
-        :type transitions: list[lusid_workflow.Transition]
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
         """
 
         self._transitions = transitions
 
-    @property
-    def instances(self):
-        """Gets the instances of this TaskDefinition.  # noqa: E501
-
-        Each Definition will have a number of instances associated with it  # noqa: E501
-
-        :return: The instances of this TaskDefinition.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._instances
-
-    @instances.setter
-    def instances(self, instances):
-        """Sets the instances of this TaskDefinition.
-
-        Each Definition will have a number of instances associated with it  # noqa: E501
-
-        :param instances: The instances of this TaskDefinition.  # noqa: E501
-        :type instances: list[str]
-        """
-
-        self._instances = instances
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/transit_task_instance_request.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/update_task_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class TransitTaskInstanceRequest(object):
+class UpdateTaskRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,60 +35,60 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'fields': 'list[FieldInstance]'
+        'fields': 'list[TaskInstanceField]'
     }
 
     attribute_map = {
         'fields': 'fields'
     }
 
     required_map = {
         'fields': 'optional'
     }
 
     def __init__(self, fields=None, local_vars_configuration=None):  # noqa: E501
-        """TransitTaskInstanceRequest - a model defined in OpenAPI"
+        """UpdateTaskRequest - a model defined in OpenAPI"
         
-        :param fields:  Defines the fields associated with the Trigger
-        :type fields: list[lusid_workflow.FieldInstance]
+        :param fields:  Defines the fields associated with the update
+        :type fields: list[lusid_workflow.TaskInstanceField]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._fields = None
         self.discriminator = None
 
         self.fields = fields
 
     @property
     def fields(self):
-        """Gets the fields of this TransitTaskInstanceRequest.  # noqa: E501
+        """Gets the fields of this UpdateTaskRequest.  # noqa: E501
 
-        Defines the fields associated with the Trigger  # noqa: E501
+        Defines the fields associated with the update  # noqa: E501
 
-        :return: The fields of this TransitTaskInstanceRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.FieldInstance]
+        :return: The fields of this UpdateTaskRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskInstanceField]
         """
         return self._fields
 
     @fields.setter
     def fields(self, fields):
-        """Sets the fields of this TransitTaskInstanceRequest.
+        """Sets the fields of this UpdateTaskRequest.
 
-        Defines the fields associated with the Trigger  # noqa: E501
+        Defines the fields associated with the update  # noqa: E501
 
-        :param fields: The fields of this TransitTaskInstanceRequest.  # noqa: E501
-        :type fields: list[lusid_workflow.FieldInstance]
+        :param fields: The fields of this UpdateTaskRequest.  # noqa: E501
+        :type fields: list[lusid_workflow.TaskInstanceField]
         """
 
         self._fields = fields
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
@@ -127,18 +127,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TransitTaskInstanceRequest):
+        if not isinstance(other, UpdateTaskRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TransitTaskInstanceRequest):
+        if not isinstance(other, UpdateTaskRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/models/transition.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/models/task_transition_definition.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
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
 
 
-class Transition(object):
+class TaskTransitionDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,184 +35,154 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        '_from': 'str',
-        'to': 'str',
+        'from_state': 'str',
+        'to_state': 'str',
         'trigger': 'str',
-        'guard': 'str',
-        'output': 'str'
+        'guard': 'str'
     }
 
     attribute_map = {
-        '_from': 'from',
-        'to': 'to',
+        'from_state': 'fromState',
+        'to_state': 'toState',
         'trigger': 'trigger',
-        'guard': 'guard',
-        'output': 'output'
+        'guard': 'guard'
     }
 
     required_map = {
-        '_from': 'optional',
-        'to': 'optional',
+        'from_state': 'optional',
+        'to_state': 'optional',
         'trigger': 'optional',
-        'guard': 'optional',
-        'output': 'optional'
+        'guard': 'optional'
     }
 
-    def __init__(self, _from=None, to=None, trigger=None, guard=None, output=None, local_vars_configuration=None):  # noqa: E501
-        """Transition - a model defined in OpenAPI"
+    def __init__(self, from_state=None, to_state=None, trigger=None, guard=None, local_vars_configuration=None):  # noqa: E501
+        """TaskTransitionDefinition - a model defined in OpenAPI"
         
-        :param _from:  The State this Transition if coming From
-        :type _from: str
-        :param to:  The State this Transition is going To
-        :type to: str
+        :param from_state:  The State this Transition if coming From
+        :type from_state: str
+        :param to_state:  The State this Transition is going To
+        :type to_state: str
         :param trigger:  The Trigger for this Transition
         :type trigger: str
         :param guard:  The Guard for this Transition, if any
         :type guard: str
-        :param output:  The Output action to invoke on successful Transition
-        :type output: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self.__from = None
-        self._to = None
+        self._from_state = None
+        self._to_state = None
         self._trigger = None
         self._guard = None
-        self._output = None
         self.discriminator = None
 
-        self._from = _from
-        self.to = to
+        self.from_state = from_state
+        self.to_state = to_state
         self.trigger = trigger
         self.guard = guard
-        self.output = output
 
     @property
-    def _from(self):
-        """Gets the _from of this Transition.  # noqa: E501
+    def from_state(self):
+        """Gets the from_state of this TaskTransitionDefinition.  # noqa: E501
 
         The State this Transition if coming From  # noqa: E501
 
-        :return: The _from of this Transition.  # noqa: E501
+        :return: The from_state of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
-        return self.__from
+        return self._from_state
 
-    @_from.setter
-    def _from(self, _from):
-        """Sets the _from of this Transition.
+    @from_state.setter
+    def from_state(self, from_state):
+        """Sets the from_state of this TaskTransitionDefinition.
 
         The State this Transition if coming From  # noqa: E501
 
-        :param _from: The _from of this Transition.  # noqa: E501
-        :type _from: str
+        :param from_state: The from_state of this TaskTransitionDefinition.  # noqa: E501
+        :type from_state: str
         """
 
-        self.__from = _from
+        self._from_state = from_state
 
     @property
-    def to(self):
-        """Gets the to of this Transition.  # noqa: E501
+    def to_state(self):
+        """Gets the to_state of this TaskTransitionDefinition.  # noqa: E501
 
         The State this Transition is going To  # noqa: E501
 
-        :return: The to of this Transition.  # noqa: E501
+        :return: The to_state of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
-        return self._to
+        return self._to_state
 
-    @to.setter
-    def to(self, to):
-        """Sets the to of this Transition.
+    @to_state.setter
+    def to_state(self, to_state):
+        """Sets the to_state of this TaskTransitionDefinition.
 
         The State this Transition is going To  # noqa: E501
 
-        :param to: The to of this Transition.  # noqa: E501
-        :type to: str
+        :param to_state: The to_state of this TaskTransitionDefinition.  # noqa: E501
+        :type to_state: str
         """
 
-        self._to = to
+        self._to_state = to_state
 
     @property
     def trigger(self):
-        """Gets the trigger of this Transition.  # noqa: E501
+        """Gets the trigger of this TaskTransitionDefinition.  # noqa: E501
 
         The Trigger for this Transition  # noqa: E501
 
-        :return: The trigger of this Transition.  # noqa: E501
+        :return: The trigger of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
         return self._trigger
 
     @trigger.setter
     def trigger(self, trigger):
-        """Sets the trigger of this Transition.
+        """Sets the trigger of this TaskTransitionDefinition.
 
         The Trigger for this Transition  # noqa: E501
 
-        :param trigger: The trigger of this Transition.  # noqa: E501
+        :param trigger: The trigger of this TaskTransitionDefinition.  # noqa: E501
         :type trigger: str
         """
 
         self._trigger = trigger
 
     @property
     def guard(self):
-        """Gets the guard of this Transition.  # noqa: E501
+        """Gets the guard of this TaskTransitionDefinition.  # noqa: E501
 
         The Guard for this Transition, if any  # noqa: E501
 
-        :return: The guard of this Transition.  # noqa: E501
+        :return: The guard of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
         return self._guard
 
     @guard.setter
     def guard(self, guard):
-        """Sets the guard of this Transition.
+        """Sets the guard of this TaskTransitionDefinition.
 
         The Guard for this Transition, if any  # noqa: E501
 
-        :param guard: The guard of this Transition.  # noqa: E501
+        :param guard: The guard of this TaskTransitionDefinition.  # noqa: E501
         :type guard: str
         """
 
         self._guard = guard
 
-    @property
-    def output(self):
-        """Gets the output of this Transition.  # noqa: E501
-
-        The Output action to invoke on successful Transition  # noqa: E501
-
-        :return: The output of this Transition.  # noqa: E501
-        :rtype: str
-        """
-        return self._output
-
-    @output.setter
-    def output(self, output):
-        """Sets the output of this Transition.
-
-        The Output action to invoke on successful Transition  # noqa: E501
-
-        :param output: The output of this Transition.  # noqa: E501
-        :type output: str
-        """
-
-        self._output = output
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -247,18 +217,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Transition):
+        if not isinstance(other, TaskTransitionDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Transition):
+        if not isinstance(other, TaskTransitionDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.164
+    The version of the OpenAPI document: 0.1.208
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.208/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 lusid_workflow/__version__.py
 lusid_workflow/api_client.py
 lusid_workflow/configuration.py
 lusid_workflow/exceptions.py
 lusid_workflow/rest.py
 lusid_workflow/api/__init__.py
 lusid_workflow/api/task_definitions_api.py
-lusid_workflow/api/task_instances_api.py
+lusid_workflow/api/tasks_api.py
+lusid_workflow/api/workers_api.py
 lusid_workflow/models/__init__.py
 lusid_workflow/models/create_task_definition_request.py
-lusid_workflow/models/create_task_instance_request.py
+lusid_workflow/models/create_task_request.py
+lusid_workflow/models/create_worker_request.py
 lusid_workflow/models/deleted_entity_response.py
-lusid_workflow/models/field_instance.py
-lusid_workflow/models/field_schema.py
-lusid_workflow/models/history_entry.py
 lusid_workflow/models/initial_state.py
 lusid_workflow/models/link.py
+lusid_workflow/models/luminesce_view.py
 lusid_workflow/models/lusid_problem_details.py
 lusid_workflow/models/lusid_validation_problem_details.py
-lusid_workflow/models/output.py
-lusid_workflow/models/output_schema.py
-lusid_workflow/models/output_type.py
 lusid_workflow/models/resource_id.py
 lusid_workflow/models/resource_list_of_task_definition.py
-lusid_workflow/models/resource_list_of_task_instance.py
-lusid_workflow/models/state.py
-lusid_workflow/models/status.py
+lusid_workflow/models/task.py
 lusid_workflow/models/task_definition.py
-lusid_workflow/models/task_definition_id.py
-lusid_workflow/models/task_instance.py
-lusid_workflow/models/transit_task_instance_request.py
-lusid_workflow/models/transition.py
-lusid_workflow/models/trigger.py
-lusid_workflow/models/trigger_invocation_response.py
+lusid_workflow/models/task_definition_version.py
+lusid_workflow/models/task_field_definition.py
+lusid_workflow/models/task_instance_field.py
+lusid_workflow/models/task_state_definition.py
+lusid_workflow/models/task_transition_definition.py
+lusid_workflow/models/transition_trigger_definition.py
 lusid_workflow/models/trigger_schema.py
 lusid_workflow/models/update_task_definition_request.py
+lusid_workflow/models/update_task_request.py
+lusid_workflow/models/update_task_response.py
+lusid_workflow/models/version.py
+lusid_workflow/models/worker.py
+lusid_workflow/models/worker_configuration.py
 lusid_workflow_sdk_preview.egg-info/PKG-INFO
 lusid_workflow_sdk_preview.egg-info/SOURCES.txt
 lusid_workflow_sdk_preview.egg-info/dependency_links.txt
 lusid_workflow_sdk_preview.egg-info/requires.txt
 lusid_workflow_sdk_preview.egg-info/top_level.txt
```

### Comparing `lusid-workflow-sdk-preview-0.1.164/setup.py` & `lusid-workflow-sdk-preview-0.1.208/setup.py`

 * *Files identical despite different names*

