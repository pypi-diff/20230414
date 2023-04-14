# Comparing `tmp/evergreen.py-3.5.5.tar.gz` & `tmp/evergreen.py-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evergreen.py-3.5.5.tar", max compression
+gzip compressed data, was "evergreen.py-3.5.6.tar", max compression
```

## Comparing `evergreen.py-3.5.5.tar` & `evergreen.py-3.5.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11336 2023-03-31 18:23:11.701660 evergreen.py-3.5.5/LICENSE
--rw-r--r--   0        0        0     5302 2023-03-31 18:23:11.701660 evergreen.py-3.5.5/README.md
--rw-r--r--   0        0        0     1375 2023-03-31 18:23:11.701660 evergreen.py-3.5.5/pyproject.toml
--rw-r--r--   0        0        0      717 2023-03-31 18:23:11.701660 evergreen.py-3.5.5/src/evergreen/__init__.py
--rw-r--r--   0        0        0     1453 2023-03-31 18:23:11.701660 evergreen.py-3.5.5/src/evergreen/alias.py
--rw-r--r--   0        0        0    49131 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/api.py
--rw-r--r--   0        0        0     2264 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/api_requests.py
--rw-r--r--   0        0        0     3039 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/base.py
--rw-r--r--   0        0        0     4558 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/build.py
--rw-r--r--   0        0        0        0 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/cli/__init__.py
--rw-r--r--   0        0        0    15411 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/cli/main.py
--rw-r--r--   0        0        0     1538 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/commitqueue.py
--rw-r--r--   0        0        0     1745 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/config.py
--rw-r--r--   0        0        0     7450 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/distro.py
--rw-r--r--   0        0        0        0 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/errors/__init__.py
--rw-r--r--   0        0        0     1444 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/errors/exceptions.py
--rw-r--r--   0        0        0     3381 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/host.py
--rw-r--r--   0        0        0     1788 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/manifest.py
--rw-r--r--   0        0        0        0 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/metrics/__init__.py
--rw-r--r--   0        0        0    15510 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/metrics/buildmetrics.py
--rw-r--r--   0        0        0     9141 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/metrics/versionmetrics.py
--rw-r--r--   0        0        0     6469 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/patch.py
--rw-r--r--   0        0        0    10706 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/performance_results.py
--rw-r--r--   0        0        0     1737 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/project.py
--rw-r--r--   0        0        0        0 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/py.typed
--rw-r--r--   0        0        0     1250 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/resource_type_permissions.py
--rw-r--r--   0        0        0     1633 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/stats.py
--rw-r--r--   0        0        0    14468 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/task.py
--rw-r--r--   0        0        0     2668 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/task_annotations.py
--rw-r--r--   0        0        0     1271 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/task_reliability.py
--rw-r--r--   0        0        0     1741 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/tst.py
--rw-r--r--   0        0        0      585 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/users_for_role.py
--rw-r--r--   0        0        0     3424 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/util.py
--rw-r--r--   0        0        0     8010 2023-03-31 18:23:11.705660 evergreen.py-3.5.5/src/evergreen/version.py
--rw-r--r--   0        0        0     6482 2023-03-31 18:23:51.092176 evergreen.py-3.5.5/setup.py
--rw-r--r--   0        0        0     6209 2023-03-31 18:23:51.092661 evergreen.py-3.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/LICENSE
+-rw-r--r--   0        0        0     5548 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/README.md
+-rw-r--r--   0        0        0     1375 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/pyproject.toml
+-rw-r--r--   0        0        0      717 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/alias.py
+-rw-r--r--   0        0        0    51068 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/api.py
+-rw-r--r--   0        0        0     2264 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/api_requests.py
+-rw-r--r--   0        0        0     3039 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/base.py
+-rw-r--r--   0        0        0     4558 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/build.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/cli/__init__.py
+-rw-r--r--   0        0        0    16690 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/cli/main.py
+-rw-r--r--   0        0        0     1538 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/commitqueue.py
+-rw-r--r--   0        0        0     1745 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/config.py
+-rw-r--r--   0        0        0     7450 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/distro.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/errors/__init__.py
+-rw-r--r--   0        0        0     1444 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/errors/exceptions.py
+-rw-r--r--   0        0        0     3381 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/host.py
+-rw-r--r--   0        0        0     1788 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/__init__.py
+-rw-r--r--   0        0        0    15510 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/buildmetrics.py
+-rw-r--r--   0        0        0     9141 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/versionmetrics.py
+-rw-r--r--   0        0        0     6576 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/patch.py
+-rw-r--r--   0        0        0    10706 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/performance_results.py
+-rw-r--r--   0        0        0     1737 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/project.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/py.typed
+-rw-r--r--   0        0        0     1250 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/resource_type_permissions.py
+-rw-r--r--   0        0        0     1633 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/stats.py
+-rw-r--r--   0        0        0    14468 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task.py
+-rw-r--r--   0        0        0     2668 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task_annotations.py
+-rw-r--r--   0        0        0     1271 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task_reliability.py
+-rw-r--r--   0        0        0     1741 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/tst.py
+-rw-r--r--   0        0        0      585 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/users_for_role.py
+-rw-r--r--   0        0        0     3424 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/util.py
+-rw-r--r--   0        0        0     8010 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/version.py
+-rw-r--r--   0        0        0     6737 2023-04-14 16:45:49.049163 evergreen.py-3.5.6/setup.py
+-rw-r--r--   0        0        0     6455 2023-04-14 16:45:49.049752 evergreen.py-3.5.6/PKG-INFO
```

### Comparing `evergreen.py-3.5.5/LICENSE` & `evergreen.py-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/README.md` & `evergreen.py-3.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,22 @@
         "version_id": null,
         "build_id": null
     },
     "user_host": false
 }
 ```
 
+The `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host's DOCKERFILE:
+
+```bash
+RUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen
+RUN chmod +x evergreen
+ENV PATH="/project:$PATH"
+```
+
 ## Documentation
 
 You can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).
 
 ## Contributor's Guide
 
 ### Setting up a local development environment
```

### Comparing `evergreen.py-3.5.5/pyproject.toml` & `evergreen.py-3.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evergreen.py"
-version = "3.5.5"
+version = "3.5.6"
 description = "Python client for the Evergreen API"
 authors = [
     "Dev Prod DAG <dev-prod-dag@mongodb.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/evergreen-ci/evergreen.py"
```

### Comparing `evergreen.py-3.5.5/src/evergreen/__init__.py` & `evergreen.py-3.5.6/src/evergreen/__init__.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/alias.py` & `evergreen.py-3.5.6/src/evergreen/alias.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/api.py` & `evergreen.py-3.5.6/src/evergreen/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- encoding: utf-8 -*-
 """API for interacting with evergreen."""
 from __future__ import absolute_import
 
 import json
+import re
+import subprocess
 from contextlib import contextmanager
 from datetime import datetime
 from functools import lru_cache
 from json.decoder import JSONDecodeError
 from time import time
 from typing import Any, Callable, Dict, Generator, Iterable, Iterator, List, Optional, Union, cast
 
@@ -26,15 +28,15 @@
     get_auth_from_config,
     read_evergreen_config,
     read_evergreen_from_file,
 )
 from evergreen.distro import Distro
 from evergreen.host import Host
 from evergreen.manifest import Manifest
-from evergreen.patch import Patch
+from evergreen.patch import Patch, PatchCreationDetails
 from evergreen.performance_results import PerformanceData
 from evergreen.project import Project
 from evergreen.resource_type_permissions import (
     PermissionableResourceType,
     RemovablePermission,
     ResourceTypePermissions,
 )
@@ -58,14 +60,16 @@
 
 CACHE_SIZE = 5000
 DEFAULT_LIMIT = 100
 MAX_RETRIES = 3
 START_WAIT_TIME_SEC = 2
 MAX_WAIT_TIME_SEC = 5
 
+EVERGREEN_URL_REGEX = "(https?)://evergreen..*?(?=\\\\n)"
+
 
 class EvergreenApi(object):
     """Base methods for building API objects."""
 
     def __init__(
         self,
         api_server: str = DEFAULT_API_SERVER,
@@ -811,14 +815,60 @@
         :param patch_id: Id of patch to query for.
         :param params: Parameters to pass to endpoint.
         :return: Patch queried for.
         """
         url = self._create_url(f"/patches/{patch_id}")
         return Patch(self._call_api(url, params).json(), self)  # type: ignore[arg-type]
 
+    def get_patch_diff(self, patch_id: str) -> str:
+        """
+        Get the diff for a given patch.
+
+        :param patch_id: The id of the patch to request the diff for.
+        :return: The diff of the patch represented as a JSON string.
+        """
+        url = self._create_url(f"/patches/{patch_id}/raw")
+        return json.dumps(self._call_api(url, method="GET").json())
+
+    def patch_from_diff(
+        self,
+        diff_file_path: str,
+        params: str,
+        base: str,
+        task: str,
+        project: str,
+        description: str,
+        variant: str,
+        author: Optional[str] = None,
+    ) -> PatchCreationDetails:
+        """
+        Start a patch build based on a diff.
+
+        :param diff_file_path: The path to the diff.
+        :param params: The params to pass to the build.
+        :param base: The build's base commit.
+        :param task: The task(s) to run.
+        :param project: The project to start the build for.
+        :param description: A description of the build.
+        :param variant: The variant(s) to build against.
+        :raises Exception: If a build URL is not produced we raise an exception with the output included.
+        :return: _description_
+        """
+        command = f"evergreen patch-file --diff-file {diff_file_path} --description '{description}' --param {params} --base {base} --tasks {task} --variants {variant} --project {project} -y -f"
+        if author is not None:
+            command = f"{command} --author {author}"
+
+        process = subprocess.run(command, shell=True, capture_output=True)
+
+        match = re.search(EVERGREEN_URL_REGEX, str(process.stderr))
+        if match is None:
+            raise Exception(f"Unable to parse URL from command output: {str(process.stderr)}")
+
+        return PatchCreationDetails(url=match.group(0))
+
     def task_by_id(self, task_id: str, fetch_all_executions: Optional[bool] = None) -> Task:
         """
         Get a task by task_id.
 
         :param task_id: Id of task to query for.
         :param fetch_all_executions: Should all executions of the task be fetched.
         :return: Task queried for.
```

### Comparing `evergreen.py-3.5.5/src/evergreen/api_requests.py` & `evergreen.py-3.5.6/src/evergreen/api_requests.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/base.py` & `evergreen.py-3.5.6/src/evergreen/base.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/build.py` & `evergreen.py-3.5.6/src/evergreen/build.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/cli/main.py` & `evergreen.py-3.5.6/src/evergreen/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -514,14 +514,43 @@
     api = ctx.obj["api"]
     user_permissions = api.all_user_permissions_for_resource(
         resource_id, PermissionableResourceType(resource_type)
     )
     click.echo(user_permissions)
 
 
+@cli.command()
+@click.pass_context
+@click.option("--patch-id", required=True, help="Patch id to request diff for.")
+def patch_diff(ctx, patch_id):
+    """Get patch diff for a given patch."""
+    api = ctx.obj["api"]
+    diff = api.get_patch_diff(patch_id)
+    click.echo(diff)
+
+
+@cli.command()
+@click.pass_context
+@click.option("--diff-file", required=True, help="The path to the diff file.")
+@click.option("--description", required=True, help="The description of the build.")
+@click.option("--param", required=True, help="The params to pass to the build.")
+@click.option("--base", required=True, help="The base commit of the build.")
+@click.option("--project", required=True, help="The project of the build.")
+@click.option("--tasks", required=True, help="The tasks to execute.")
+@click.option("--variants", required=True, help="The variants to build against.")
+@click.option("--author", required=False, default=None, help="Indicate the author of the patch.")
+def patch_from_diff(ctx, diff_file, description, param, base, project, tasks, variants, author):
+    """Start a patch build based on the diff."""
+    api = ctx.obj["api"]
+    response = api.patch_from_diff(
+        diff_file, param, base, tasks, project, description, variants, author
+    )
+    click.echo(response)
+
+
 def main():
     """Create command line application."""
     return cli(obj={})
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evergreen.py-3.5.5/src/evergreen/commitqueue.py` & `evergreen.py-3.5.6/src/evergreen/commitqueue.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/config.py` & `evergreen.py-3.5.6/src/evergreen/config.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/distro.py` & `evergreen.py-3.5.6/src/evergreen/distro.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/errors/exceptions.py` & `evergreen.py-3.5.6/src/evergreen/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/host.py` & `evergreen.py-3.5.6/src/evergreen/host.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/manifest.py` & `evergreen.py-3.5.6/src/evergreen/manifest.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/metrics/buildmetrics.py` & `evergreen.py-3.5.6/src/evergreen/metrics/buildmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/metrics/versionmetrics.py` & `evergreen.py-3.5.6/src/evergreen/metrics/versionmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/patch.py` & `evergreen.py-3.5.6/src/evergreen/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Representation of an evergreen patch."""
 from __future__ import absolute_import
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
+from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple, Optional, Set
 
 from evergreen.base import _BaseEvergreenObject, evg_attrib, evg_datetime_attrib
 
 if TYPE_CHECKING:
     from evergreen.api import EvergreenApi
     from evergreen.version import Version
 
@@ -97,14 +97,20 @@
 
     @property
     def file_diffs(self) -> List[FileDiff]:
         """Retrieve a list of the file diffs for this patch."""
         return [FileDiff(diff, self._api) for diff in self.json["module_code_changes"]]
 
 
+class PatchCreationDetails(NamedTuple):
+    """Details of a patch creation."""
+
+    url: str
+
+
 class Patch(_BaseEvergreenObject):
     """Representation of an Evergreen patch."""
 
     patch_id = evg_attrib("patch_id")
     description = evg_attrib("description")
     project_id = evg_attrib("project_id")
     branch = evg_attrib("branch")
```

### Comparing `evergreen.py-3.5.5/src/evergreen/performance_results.py` & `evergreen.py-3.5.6/src/evergreen/performance_results.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/project.py` & `evergreen.py-3.5.6/src/evergreen/project.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/resource_type_permissions.py` & `evergreen.py-3.5.6/src/evergreen/resource_type_permissions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/stats.py` & `evergreen.py-3.5.6/src/evergreen/stats.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/task.py` & `evergreen.py-3.5.6/src/evergreen/task.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/task_annotations.py` & `evergreen.py-3.5.6/src/evergreen/task_annotations.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/task_reliability.py` & `evergreen.py-3.5.6/src/evergreen/task_reliability.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/tst.py` & `evergreen.py-3.5.6/src/evergreen/tst.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/users_for_role.py` & `evergreen.py-3.5.6/src/evergreen/users_for_role.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/util.py` & `evergreen.py-3.5.6/src/evergreen/util.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/src/evergreen/version.py` & `evergreen.py-3.5.6/src/evergreen/version.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.5/setup.py` & `evergreen.py-3.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'tenacity>=5']
 
 entry_points = \
 {'console_scripts': ['evg-api = evergreen.cli.main:main']}
 
 setup_kwargs = {
     'name': 'evergreen.py',
-    'version': '3.5.5',
+    'version': '3.5.6',
     'description': 'Python client for the Evergreen API',
-    'long_description': '# Evergreen.py\n\nA client library for the Evergreen API written in python. Currently supports the V2 version of\nthe API. For more details, see https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evergreen.py) [![PyPI](https://img.shields.io/pypi/v/evergreen.py.svg)](https://pypi.org/project/evergreen.py/) [![Coverage Status](https://coveralls.io/repos/github/evergreen-ci/evergreen.py/badge.svg?branch=master)](https://coveralls.io/github/evergreen-ci/evergreen.py?branch=master)\n\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Dependencies](#dependencies)\n4. [Installation](#installation)\n5. [Usage](#usage)\n6. [Documentation](#documentation)\n7. [Contributor\'s Guide](#contributors-guide)\n    - [Setting up a local development environment](#setting-up-a-local-development-environment)\n    - [Linting/formatting](#lintingformatting)\n    - [Running tests](#running-tests)\n    - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThis is a Python client library for interacting with Evergreen and Evergreen objects. It currently only\nsupports the V2 version of Evergreen\'s api. It can be used either by Python code in a separate application\nor on the command line to get data about Evergreen objects quickly and easily.\n\n## Getting Help\n\n### What\'s the right channel to ask my question?\nIf you have a question about evergreen.py, please mention @dag-on-call in\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evergreen.py?\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following:\n* **Motivation for Request**\n  * provide us the motivation for this change.\n* **Context**\n  * provide some background contexts for this issue.\n* **Description**\n  * provide some descriptions on how this issue happened.\n\n## Dependencies\n\n* Python 3.7 or later\n\n## Installation\n\n```bash\n$ pip install evergreen.py\n```\n\n## Usage\n\nThis client can be used either in code or directly via the command line.\n\nIn code:\n```python\n>> from evergreen.api import EvgAuth, EvergreenApi\n>> api = EvergreenApi.get_api(EvgAuth(\'david.bradford\', \'***\'))\n>> project = api.project_by_id(\'mongodb-mongo-master\')\n>> project.display_name\n\'MongoDB (master)\'\n```\n\nCli:\n```bash\n$ evg-api --json list-hosts\n{\n    "host_id": "host num 0",\n    "host_url": "host.num.com",\n    "distro": {\n        "distro_id": "ubuntu1804-build",\n        "provider": "static",\n        "image_id": ""\n    },\n    "provisioned": true,\n    "started_by": "mci",\n    "host_type": "",\n    "user": "mci-exec",\n    "status": "running",\n    "running_task": {\n        "task_id": null,\n        "name": null,\n        "dispatch_time": null,\n        "version_id": null,\n        "build_id": null\n    },\n    "user_host": false\n}\n```\n\n## Documentation\n\nYou can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).\n\n## Contributor\'s Guide\n\n### Setting up a local development environment\n\n#### Requirements\n* Poetry 1.1 or later\n\nYou will need Evergreen credentials on your local machine to use this library or the attached CLI. You\ncan set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).\n\n### Linting/formatting\n\nThis project uses [black](https://github.com/psf/black) for formatting.\n\n```bash\npoetry run black src tests\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\nThere are a few tests that are slow running. These tests are not run by default, but can be included\nby setting the env variable RUN_SLOW_TESTS to any value.\n\n```\n$ RUN_SLOW_TEST=1 poetry run pytest\n```\n\nTo get code coverage information:\n\n```\n$ poetry run pytest --cov=src --cov-report=html\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\n$ poetry run pre-commit install\n```\n\n### Versioning\n\nBefore deploying a new version, please update the `CHANGELOG.md` file with a description of what\nis being changed.\n\nDeploys to [PyPi](https://pypi.org/project/evergreen.py/) are done automatically on merges to master.\nIn order to avoid overwriting a previous deploy, the version should be updated on all changes. The\n[semver](https://semver.org/) versioning scheme should be used for determining the version number.\n\nThe version is found in the `pyproject.toml` file.\n\n### Code Review\n\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to production is automatically triggered on merges to master.\n',
+    'long_description': '# Evergreen.py\n\nA client library for the Evergreen API written in python. Currently supports the V2 version of\nthe API. For more details, see https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evergreen.py) [![PyPI](https://img.shields.io/pypi/v/evergreen.py.svg)](https://pypi.org/project/evergreen.py/) [![Coverage Status](https://coveralls.io/repos/github/evergreen-ci/evergreen.py/badge.svg?branch=master)](https://coveralls.io/github/evergreen-ci/evergreen.py?branch=master)\n\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Dependencies](#dependencies)\n4. [Installation](#installation)\n5. [Usage](#usage)\n6. [Documentation](#documentation)\n7. [Contributor\'s Guide](#contributors-guide)\n    - [Setting up a local development environment](#setting-up-a-local-development-environment)\n    - [Linting/formatting](#lintingformatting)\n    - [Running tests](#running-tests)\n    - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThis is a Python client library for interacting with Evergreen and Evergreen objects. It currently only\nsupports the V2 version of Evergreen\'s api. It can be used either by Python code in a separate application\nor on the command line to get data about Evergreen objects quickly and easily.\n\n## Getting Help\n\n### What\'s the right channel to ask my question?\nIf you have a question about evergreen.py, please mention @dag-on-call in\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evergreen.py?\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following:\n* **Motivation for Request**\n  * provide us the motivation for this change.\n* **Context**\n  * provide some background contexts for this issue.\n* **Description**\n  * provide some descriptions on how this issue happened.\n\n## Dependencies\n\n* Python 3.7 or later\n\n## Installation\n\n```bash\n$ pip install evergreen.py\n```\n\n## Usage\n\nThis client can be used either in code or directly via the command line.\n\nIn code:\n```python\n>> from evergreen.api import EvgAuth, EvergreenApi\n>> api = EvergreenApi.get_api(EvgAuth(\'david.bradford\', \'***\'))\n>> project = api.project_by_id(\'mongodb-mongo-master\')\n>> project.display_name\n\'MongoDB (master)\'\n```\n\nCli:\n```bash\n$ evg-api --json list-hosts\n{\n    "host_id": "host num 0",\n    "host_url": "host.num.com",\n    "distro": {\n        "distro_id": "ubuntu1804-build",\n        "provider": "static",\n        "image_id": ""\n    },\n    "provisioned": true,\n    "started_by": "mci",\n    "host_type": "",\n    "user": "mci-exec",\n    "status": "running",\n    "running_task": {\n        "task_id": null,\n        "name": null,\n        "dispatch_time": null,\n        "version_id": null,\n        "build_id": null\n    },\n    "user_host": false\n}\n```\n\nThe `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host\'s DOCKERFILE:\n\n```bash\nRUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen\nRUN chmod +x evergreen\nENV PATH="/project:$PATH"\n```\n\n## Documentation\n\nYou can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).\n\n## Contributor\'s Guide\n\n### Setting up a local development environment\n\n#### Requirements\n* Poetry 1.1 or later\n\nYou will need Evergreen credentials on your local machine to use this library or the attached CLI. You\ncan set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).\n\n### Linting/formatting\n\nThis project uses [black](https://github.com/psf/black) for formatting.\n\n```bash\npoetry run black src tests\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\nThere are a few tests that are slow running. These tests are not run by default, but can be included\nby setting the env variable RUN_SLOW_TESTS to any value.\n\n```\n$ RUN_SLOW_TEST=1 poetry run pytest\n```\n\nTo get code coverage information:\n\n```\n$ poetry run pytest --cov=src --cov-report=html\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\n$ poetry run pre-commit install\n```\n\n### Versioning\n\nBefore deploying a new version, please update the `CHANGELOG.md` file with a description of what\nis being changed.\n\nDeploys to [PyPi](https://pypi.org/project/evergreen.py/) are done automatically on merges to master.\nIn order to avoid overwriting a previous deploy, the version should be updated on all changes. The\n[semver](https://semver.org/) versioning scheme should be used for determining the version number.\n\nThe version is found in the `pyproject.toml` file.\n\n### Code Review\n\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to production is automatically triggered on merges to master.\n',
     'author': 'Dev Prod DAG',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/evergreen-ci/evergreen.py',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `evergreen.py-3.5.5/PKG-INFO` & `evergreen.py-3.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evergreen.py
-Version: 3.5.5
+Version: 3.5.6
 Summary: Python client for the Evergreen API
 Home-page: https://github.com/evergreen-ci/evergreen.py
 License: Apache-2.0
 Author: Dev Prod DAG
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -123,14 +123,22 @@
         "version_id": null,
         "build_id": null
     },
     "user_host": false
 }
 ```
 
+The `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host's DOCKERFILE:
+
+```bash
+RUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen
+RUN chmod +x evergreen
+ENV PATH="/project:$PATH"
+```
+
 ## Documentation
 
 You can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).
 
 ## Contributor's Guide
 
 ### Setting up a local development environment
```

