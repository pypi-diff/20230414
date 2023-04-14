# Comparing `tmp/pulp-glue-0.18.0.tar.gz` & `tmp/pulp-glue-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.18.0.tar", last modified: Thu Mar  9 13:27:50 2023, max compression
+gzip compressed data, was "pulp-glue-0.19.0.tar", last modified: Fri Apr 14 15:26:02 2023, max compression
```

## Comparing `pulp-glue-0.18.0.tar` & `pulp-glue-0.19.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.856563 pulp-glue-0.18.0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.860563 pulp-glue-0.18.0/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.860563 pulp-glue-0.18.0/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34297 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/common/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/container/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/file/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/python/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.864563 pulp-glue-0.18.0/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:27:50.860563 pulp-glue-0.18.0/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-09 13:27:50.000000 pulp-glue-0.18.0/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-09 13:27:50.000000 pulp-glue-0.18.0/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:27:50.000000 pulp-glue-0.18.0/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-09 13:27:50.000000 pulp-glue-0.18.0/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-09 13:27:50.000000 pulp-glue-0.18.0/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 13:27:50.868564 pulp-glue-0.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-09 13:27:41.000000 pulp-glue-0.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/setup.py
```

### Comparing `pulp-glue-0.18.0/PKG-INFO` & `pulp-glue-0.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.18.0
+Version: 0.19.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.18.0/pulp_glue/ansible/context.py` & `pulp-glue-0.19.0/pulp_glue/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/common/context.py` & `pulp-glue-0.19.0/pulp_glue/common/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,34 @@
                         if (
                             parameter["name"] in ["fields", "exclude_fields"]
                             and parameter["in"] == "query"
                             and "schema" in parameter
                             and parameter["schema"]["type"] == "string"
                         ):
                             parameter["schema"] = {"type": "array", "items": {"type": "string"}}
+        if self.has_plugin(PluginRequirement("core", max="99.99.0")):
+            # https://github.com/pulp/pulpcore/issues/3634
+            for operation_id, (method, path) in self.api.operations.items():
+                if (
+                    operation_id == "repository_versions_list"
+                    or (
+                        operation_id.startswith("repositories_")
+                        and operation_id.endswith("_versions_list")
+                    )
+                    or (operation_id.startswith("publications_") and operation_id.endswith("_list"))
+                ):
+                    operation = api_spec["paths"][path][method]
+                    for parameter in operation["parameters"]:
+                        if (
+                            parameter["name"] == "content__in"
+                            and parameter["in"] == "query"
+                            and "schema" in parameter
+                            and parameter["schema"]["type"] == "string"
+                        ):
+                            parameter["schema"] = {"type": "array", "items": {"type": "string"}}
         if self.has_plugin(PluginRequirement("file", min="1.10.0", max="1.11.0")):
             operation = api_spec["paths"]["{file_file_alternate_content_source_href}refresh/"][
                 "post"
             ]
             operation.pop("requestBody")
         if self.has_plugin(
             PluginRequirement("python", max="99.99.0.dev")
@@ -256,36 +276,42 @@
                 err=True,
             )
             if not non_blocking:
                 result = self.wait_for_task_group(result)
         return result
 
     @classmethod
-    def _check_task_finished(cls, task: EntityDefinition) -> bool:
+    def _check_task_finished(cls, task: EntityDefinition, expect_cancel: bool = False) -> bool:
         task_href = task["pulp_href"]
 
         if task["state"] == "completed":
+            if expect_cancel:
+                raise PulpException(
+                    _("The task {task_href} meant to be canceled, completed instead.")
+                )
             return True
         elif task["state"] == "failed":
             raise PulpException(
                 _("Task {task_href} failed: '{description}'").format(
                     task_href=task_href,
                     description=task["error"].get("description") or task["error"].get("reason"),
                 )
             )
         elif task["state"] == "canceled":
+            if expect_cancel:
+                return True
             raise PulpException(_("Task {task_href} canceled").format(task_href=task_href))
         elif task["state"] in ["waiting", "running", "canceling"]:
             return False
         else:
             raise NotImplementedError(_("Unknown task state: {state}").format(state=task["state"]))
 
-    def _poll_task(self, task: EntityDefinition) -> EntityDefinition:
+    def _poll_task(self, task: EntityDefinition, expect_cancel: bool = False) -> EntityDefinition:
         while True:
-            if self._check_task_finished(task):
+            if self._check_task_finished(task, expect_cancel=expect_cancel):
                 self.echo("Done.", err=True)
                 return task
             else:
                 if self.timeout:
                     assert isinstance(self.start_time, datetime.datetime)
                     if (datetime.datetime.now() - self.start_time).seconds > self.timeout:
                         raise PulpNoWait(
@@ -293,27 +319,27 @@
                                 task_href=task["pulp_href"]
                             )
                         )
                 time.sleep(1)
                 self.echo(".", nl=False, err=True)
                 task = self.api.call("tasks_read", parameters={"task_href": task["pulp_href"]})
 
-    def wait_for_task(self, task: EntityDefinition) -> Any:
+    def wait_for_task(self, task: EntityDefinition, expect_cancel: bool = False) -> Any:
         """
         Wait for a task to finish and return the finished task object.
 
         Raise `PulpNoWait` on timeout, background, ctrl-c, if task failed or was canceled.
         """
         self.start_time = datetime.datetime.now()
 
         if self.background_tasks:
             raise PulpNoWait(_("Not waiting for task because --background was specified."))
         task_href = task["pulp_href"]
         try:
-            return self._poll_task(task)
+            return self._poll_task(task, expect_cancel=expect_cancel)
         except KeyboardInterrupt:
             raise PulpNoWait(_("Task {task_href} sent to background.").format(task_href=task_href))
 
     def wait_for_task_group(self, task_group: EntityDefinition) -> Any:
         """
         Wait for a task group to finish and return the finished task object.
 
@@ -492,14 +518,18 @@
                 )
             )
 
         # Setting this property will always (lazily) retrigger retrieving the entity.
         self._entity_lookup = {"pulp_href": value}
         self._entity = None
 
+    @property
+    def tangible(self) -> bool:
+        return bool(self._entity) or bool(self._entity_lookup)
+
     def __init__(
         self,
         pulp_ctx: PulpContext,
         pulp_href: Optional[str] = None,
         entity: Optional[EntityDefinition] = None,
     ) -> None:
         assert pulp_href is None or entity is None
@@ -746,16 +776,16 @@
         "sock_read_timeout",
         "rate_limit",
     }
 
 
 class PulpPublicationContext(PulpEntityContext):
     ENTITY = _("publication")
-    ENTITIES = _("pulications")
-    ID_PREFIX = "pulications"
+    ENTITIES = _("publications")
+    ID_PREFIX = "publications"
     HREF_PATTERN = r"publications/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
 
     def list(self, limit: int, offset: int, parameters: Dict[str, Any]) -> List[Any]:
         if parameters.get("repository") is not None:
             self.pulp_ctx.needs_plugin(
                 PluginRequirement("core", min="3.20.0", feature=_("repository filter"))
             )
@@ -766,48 +796,40 @@
     ENTITY = _("distribution")
     ENTITIES = _("distributions")
     ID_PREFIX = "distributions"
     HREF_PATTERN = r"distributions/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
 
 
 class PulpRepositoryVersionContext(PulpEntityContext):
-    """
-    Base class for repository version specific contexts.
-    This class provides the basic CRUD commands and
-    ties its instances to the global PulpContext for api access.
-    """
-
     ENTITY = _("repository version")
     ENTITIES = _("repository versions")
+    ID_PREFIX = "repository_versions"
     repository_ctx: "PulpRepositoryContext"
 
     def __init__(self, pulp_ctx: PulpContext, repository_ctx: "PulpRepositoryContext") -> None:
         super().__init__(pulp_ctx)
         self.repository_ctx = repository_ctx
 
     @property
     def scope(self) -> Dict[str, Any]:
-        return {self.repository_ctx.HREF: self.repository_ctx.pulp_href}
+        if self.ID_PREFIX == "repository_versions":
+            return {}
+        else:
+            return {self.repository_ctx.HREF: self.repository_ctx.pulp_href}
 
     def repair(self, href: Optional[str] = None) -> Any:
         return self.call("repair", parameters={self.HREF: href or self.pulp_href}, body={})
 
 
 class PulpRepositoryContext(PulpEntityContext):
-    """
-    Base class for repository specific contexts.
-    This class provides the basic CRUD commands as well as synchronizing and
-    ties its instances to the global PulpContext for api access.
-    """
-
     ENTITY = _("repository")
     ENTITIES = _("repositories")
     HREF_PATTERN = r"repositories/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
     ID_PREFIX = "repositories"
-    VERSION_CONTEXT: ClassVar[Type[PulpRepositoryVersionContext]]
+    VERSION_CONTEXT: ClassVar[Type[PulpRepositoryVersionContext]] = PulpRepositoryVersionContext
     NULLABLES = {"description", "retain_repo_versions"}
 
     def get_version_context(self) -> PulpRepositoryVersionContext:
         return self.VERSION_CONTEXT(self.pulp_ctx, self)
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
@@ -837,18 +859,14 @@
             body["remove_content_units"] = remove_content
         if base_version is not None:
             body["base_version"] = base_version
         return self.call("modify", parameters={self.HREF: href or self.pulp_href}, body=body)
 
 
 class PulpContentContext(PulpEntityContext):
-    """
-    Base class for content specific contexts
-    """
-
     ENTITY = _("content")
     ENTITIES = _("content")
     ID_PREFIX = "content"
 
     def upload(
         self,
         file: IO[bytes],
```

### Comparing `pulp-glue-0.18.0/pulp_glue/common/i18n.py` & `pulp-glue-0.19.0/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/common/openapi.py` & `pulp-glue-0.19.0/pulp_glue/common/openapi.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/container/context.py` & `pulp-glue-0.19.0/pulp_glue/container/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/core/context.py` & `pulp-glue-0.19.0/pulp_glue/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,17 +249,18 @@
 
 
 class PulpContentGuardContext(PulpEntityContext):
     ENTITY = "content guard"
     ENTITIES = "content guards"
     ID_PREFIX = "contentguards"
     HREF_PATTERN = r"contentguards/(?P<plugin>[\w\-_]+)/(?P<resource_type>[\w\-_]+)/"
+    NULLABLES = {"description"}
 
 
-class PulpContentRedirectContentGuardContext(PulpEntityContext):
+class PulpContentRedirectContentGuardContext(PulpContentGuardContext):
     ENTITY = "content redirect content guard"
     ENTITIES = "content redirect content guards"
     HREF = "content_redirect_content_guard_href"
     ID_PREFIX = "contentguards_core_content_redirect"
     NEEDS_PLUGINS = [PluginRequirement("core", min="3.18.0")]
 
 
@@ -268,18 +269,20 @@
     ENTITIES = _("Pulp importers")
     HREF = "pulp_importer_href"
     ID_PREFIX = "importers_core_pulp"
 
 
 class PulpOrphanContext(PulpEntityContext):
     def cleanup(self, body: Optional[Dict[str, Any]] = None) -> Any:
-        if body:
+        if body is not None:
             body = self.preprocess_entity(body)
             if "orphan_protection_time" in body:
                 self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.15.0"))
+        else:
+            body = {}
         if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.14.0")):
             result = self.pulp_ctx.call("orphans_cleanup_cleanup", body=body)
         else:
             if body:
                 self.pulp_ctx.needs_plugin(PluginRequirement("core", min="3.14.0"))
             result = self.pulp_ctx.call("orphans_delete")
         return result
@@ -339,14 +342,15 @@
 
 
 class PulpSigningServiceContext(PulpEntityContext):
     ENTITY = _("signing service")
     ENTITIES = _("signing services")
     HREF = "signing_service_href"
     ID_PREFIX = "signing_services"
+    HREF_PATTERN = r"signing-services/"
 
 
 class PulpTaskContext(PulpEntityContext):
     ENTITY = _("task")
     ENTITIES = _("tasks")
     HREF = "task_href"
     ID_PREFIX = "tasks"
@@ -386,20 +390,26 @@
                         feature=_("specify multiple reserved resources"),
                     ),
                 )
             parameters["reserved_resources_record"] = reserved_resources_record
 
         return super().list(limit=limit, offset=offset, parameters=parameters)
 
-    def cancel(self, task_href: Optional[str] = None) -> Any:
-        return self.call(
+    def cancel(self, task_href: Optional[str] = None, background: bool = False) -> Any:
+        task_href = task_href or self.pulp_href
+        task = self.call(
             "cancel",
-            parameters={self.HREF: task_href or self.pulp_href},
+            parameters={self.HREF: task_href},
             body={"state": "canceled"},
         )
+        if not background:
+            self.pulp_ctx.echo(_("Waiting to cancel task {href}").format(href=task_href), err=True)
+            task = self.pulp_ctx.wait_for_task(task, expect_cancel=True)
+            self.pulp_ctx.echo(_("Done."), err=True)
+        return task
 
     @property
     def scope(self) -> Dict[str, Any]:
         if self.resource_context:
             if self.pulp_ctx.has_plugin(PluginRequirement("core", min="3.22.0")):
                 return {"reserved_resources": self.resource_context.pulp_href}
             else:
```

### Comparing `pulp-glue-0.18.0/pulp_glue/file/context.py` & `pulp-glue-0.19.0/pulp_glue/file/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/python/context.py` & `pulp-glue-0.19.0/pulp_glue/python/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue/rpm/context.py` & `pulp-glue-0.19.0/pulp_glue/rpm/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.18.0/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.19.0/pulp_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.18.0
+Version: 0.19.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.18.0/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.19.0/pulp_glue.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 pulp_glue.egg-info/SOURCES.txt
 pulp_glue.egg-info/dependency_links.txt
 pulp_glue.egg-info/requires.txt
 pulp_glue.egg-info/top_level.txt
 pulp_glue/ansible/__init__.py
 pulp_glue/ansible/context.py
 pulp_glue/ansible/py.typed
+pulp_glue/certguard/__init__.py
+pulp_glue/certguard/context.py
+pulp_glue/certguard/py.typed
 pulp_glue/common/__init__.py
 pulp_glue/common/context.py
 pulp_glue/common/i18n.py
 pulp_glue/common/openapi.py
 pulp_glue/common/py.typed
 pulp_glue/container/__init__.py
 pulp_glue/container/context.py
```

### Comparing `pulp-glue-0.18.0/setup.py` & `pulp-glue-0.19.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     name="pulp-glue",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://github.com/pulp/pulp-cli",
-    version="0.18.0",
+    version="0.19.0",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
         "packaging",
         "setuptools",
         "requests~=2.24",
```

