# Comparing `tmp/astronomer_cosmos-0.5.2.tar.gz` & `tmp/astronomer_cosmos-0.6.0.dev0.tar.gz`

## Comparing `astronomer_cosmos-0.5.2.tar` & `astronomer_cosmos-0.6.0.dev0.tar`

### file list

```diff
@@ -1,27 +1,37 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/core/airflow.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/__init__.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0    17213 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/operators.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/utils/file_syncing.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/LICENSE
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/README.rst
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 astronomer_cosmos-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/README.rst
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/PKG-INFO
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,9 +52,9 @@
     """
     A task represents a single node in the DAG.
 
     :param operator_class: The name of the operator class to use for this task
     :param arguments: The arguments to pass to the operator
     """
 
-    operator_class: str = "airflow.operators.dummy.DummyOperator"
+    operator_class: str = "airflow.operators.empty.EmptyOperator"
     arguments: Dict[str, Any] = field(default_factory=dict)
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,32 +19,39 @@
     for additional configs to be passed.
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
+    :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
+        or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
+    :param execution_mode: The execution mode in which the dbt project should be run.
+        Options are "local", "docker", and "kubernetes".
+        Defaults to "local"
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
+        operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dbt",
         dbt_models_dir: str = "models",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
+        execution_mode: Literal["local", "docker", "kubernetes"] = "local",
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
             "conn_id": conn_id,
@@ -52,16 +59,18 @@
 
         # get the group of the dbt project
         group = render_project(
             dbt_project_name=dbt_project_name,
             dbt_root_path=dbt_root_path,
             dbt_models_dir=dbt_models_dir,
             task_args=dbt_args,
+            operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             select=select,
             exclude=exclude,
+            execution_mode=execution_mode,
         )
 
         # call the airflow DAG constructor
         super().__init__(group, *args, **kwargs)
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,85 @@
 """
 This module contains a function to render a dbt project into Cosmos entities.
 """
+import itertools
 import logging
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from typing import Any, Dict, List
 
 from airflow.exceptions import AirflowException
 
 from cosmos.core.graph.entities import CosmosEntity, Group, Task
 from cosmos.providers.dbt.core.utils.data_aware_scheduling import get_dbt_dataset
-from cosmos.providers.dbt.parser.project import DbtProject
+from cosmos.providers.dbt.parser.project import DbtModelType, DbtProject
 
 logger = logging.getLogger(__name__)
 
 
+def calculate_operator_class(
+    execution_mode: str,
+    dbt_class: str,
+) -> str:
+    return f"cosmos.providers.dbt.core.operators.{execution_mode}.{dbt_class}{execution_mode.capitalize()}Operator"
+
+
 def render_project(
     dbt_project_name: str,
     dbt_root_path: str = "/usr/local/airflow/dbt",
     dbt_models_dir: str = "models",
+    dbt_snapshots_dir: str = "snapshots",
     task_args: Dict[str, Any] = {},
+    operator_args: Dict[str, Any] = {},
     test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
     emit_datasets: bool = True,
     conn_id: str = "default_conn_id",
     select: Dict[str, List[str]] = {},
     exclude: Dict[str, List[str]] = {},
+    execution_mode: Literal["local", "docker", "kubernetes"] = "local",
 ) -> Group:
     """
     Turn a dbt project into a Group
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dbt
     :param task_args: Arguments to pass to the underlying dbt operators
+    :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
+        or DockerOperator parameters
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param conn_id: The Airflow connection ID to use in Airflow Datasets
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2]}})
+    :param execution_mode: The execution mode in which the dbt project should be run.
+        Options are "local", "docker", and "kubernetes".
+        Defaults to "local"
     """
     # first, get the dbt project
     project = DbtProject(
         dbt_root_path=dbt_root_path,
         dbt_models_dir=dbt_models_dir,
+        dbt_snapshots_dir=dbt_snapshots_dir,
         project_name=dbt_project_name,
     )
 
-    base_group = Group(id=dbt_project_name)  # this is the group that will be returned
+    # this is the group that will be returned
+    base_group = Group(id=dbt_project_name)
     entities: Dict[
         str, CosmosEntity
     ] = {}  # this is a dict of all the entities we create
 
     # add project_dir arg to task_args
-    task_args["project_dir"] = project.project_dir
+    if execution_mode == "local":
+        task_args["project_dir"] = project.project_dir
 
     # ensures the same tag isn't in select & exclude
     if "tags" in select and "tags" in exclude:
         if set(select["tags"]).intersection(exclude["tags"]):
             raise AirflowException(
                 f"Can't specify the same tag in `select` and `include`: "
                 f"{set(select['tags']).intersection(exclude['tags'])}"
@@ -70,15 +89,17 @@
         if set(select["paths"]).intersection(exclude["paths"]):
             raise AirflowException(
                 f"Can't specify the same path in `select` and `include`: "
                 f"{set(select['paths']).intersection(exclude['paths'])}"
             )
 
     # iterate over each model once to create the initial tasks
-    for model_name, model in project.models.items():
+    for model_name, model in itertools.chain(
+        project.models.items(), project.snapshots.items(), project.seeds.items()
+    ):
         # filters down to a path within the project_dir
         if "paths" in select:
             root_directories = [
                 project.project_dir / path.strip("/")
                 for path in select.get("paths", [])
             ]
             if not set(root_directories).intersection(model.path.parents):
@@ -96,78 +117,115 @@
             if not set(select["configs"]).intersection(model.config.config_selectors):
                 continue
 
         if "configs" in exclude:
             if set(exclude["configs"]).intersection(model.config.config_selectors):
                 continue
 
-        run_args: Dict[str, Any] = {**task_args, "models": model_name}
-        test_args: Dict[str, Any] = {**task_args, "models": model_name}
+        run_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
+        test_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
 
         if emit_datasets:
             outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
 
             if test_behavior == "after_each":
                 test_args["outlets"] = outlets
             else:
                 run_args["outlets"] = outlets
 
-        # make the run task
-        run_task = Task(
-            id=f"{model_name}_run",
-            operator_class="cosmos.providers.dbt.core.operators.DbtRunOperator",
-            arguments=run_args,
-        )
+        if model.type == DbtModelType.DBT_MODEL:
+            # make the run task for model
+            run_task = Task(
+                id=f"{model_name}_run",
+                operator_class=calculate_operator_class(
+                    execution_mode=execution_mode,
+                    dbt_class="DbtRun",
+                ),
+                arguments=run_args,
+            )
+        elif model.type == DbtModelType.DBT_SNAPSHOT:
+            # make the run task for snapshot
+            run_task = Task(
+                id=f"{model_name}_snapshot",
+                operator_class=calculate_operator_class(
+                    execution_mode=execution_mode,
+                    dbt_class="DbtSnapshot",
+                ),
+                arguments=run_args,
+            )
+        elif model.type == DbtModelType.DBT_SEED:
+            # make the run task for snapshot
+            run_task = Task(
+                id=f"{model_name}_seed",
+                operator_class=calculate_operator_class(
+                    execution_mode=execution_mode,
+                    dbt_class="DbtSeed",
+                ),
+                arguments=run_args,
+            )
+        else:
+            logger.error("Unknown DBT type.")
 
         # if test_behavior isn't "after_each", we can just add the task to the
         # base group and do nothing else for now
         if test_behavior != "after_each":
             entities[model_name] = run_task
             base_group.add_entity(entity=run_task)
             continue
 
-        # otherwise, we need to make a test task and turn them into a group
+        # otherwise, we need to make a test task after run tasks and turn them into a group
         entities[run_task.id] = run_task
 
-        test_task = Task(
-            id=f"{model_name}_test",
-            operator_class="cosmos.providers.dbt.core.operators.DbtTestOperator",
-            upstream_entity_ids=[run_task.id],
-            arguments=test_args,
-        )
-        entities[test_task.id] = test_task
-
-        # make the group
-        model_group = Group(
-            id=model_name,
-            entities=[run_task, test_task],
-        )
-        entities[model_group.id] = model_group
+        if model.type == DbtModelType.DBT_MODEL:
+            test_task = Task(
+                id=f"{model_name}_test",
+                operator_class=calculate_operator_class(
+                    execution_mode=execution_mode,
+                    dbt_class="DbtTest",
+                ),
+                upstream_entity_ids=[run_task.id],
+                arguments=test_args,
+            )
+            entities[test_task.id] = test_task
+            # make the group
+            model_group = Group(
+                id=f"{model_name}",
+                entities=[run_task, test_task],
+            )
+            entities[model_group.id] = model_group
+            base_group.add_entity(entity=model_group)
 
-        # just add to base group for now
-        base_group.add_entity(entity=model_group)
+        # all other non-run tasks don't need to be grouped with test tasks
+        else:
+            entities[model_name] = run_task
+            base_group.add_entity(entity=run_task)
 
     # add dependencies now that we have all the entities
-    for model_name, model in project.models.items():
+    for model_name, model in itertools.chain(
+        project.models.items(), project.snapshots.items(), project.seeds.items()
+    ):
         upstream_deps = model.config.upstream_models
         for upstream_model_name in upstream_deps:
             try:
                 dep_task = entities[upstream_model_name]
                 entities[model_name].add_upstream(dep_task)
             except KeyError:
                 logger.error(
                     f"Dependency {upstream_model_name} not found for model {model}"
                 )
 
     if test_behavior == "after_all":
         # make a test task
         test_task = Task(
             id=f"{dbt_project_name}_test",
-            operator_class="cosmos.providers.dbt.core.operators.DbtTestOperator",
-            arguments=task_args,
+            operator_class=calculate_operator_class(
+                execution_mode=execution_mode,
+                dbt_class="DbtTest",
+            ),
+            arguments={**task_args, **operator_args},
         )
         entities[test_task.id] = test_task
 
         # add it to the base group
         base_group.add_entity(test_task)
 
         # add it as an upstream to all the models that don't have downstream tasks
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,51 +17,63 @@
     """
     Render a dbt project as an Airflow Task Group. Overrides the Airflow Task Group model to allow
     for additional configs to be passed.
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
+    :param dbt_snapshots_dir: The path to the dbt snapshots directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
+    :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
+        or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
+    :param execution_mode: The execution mode in which the dbt project should be run.
+        Options are "local", "docker", and "kubernetes".
+        Defaults to "local"
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
+        operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dbt",
         dbt_models_dir: str = "models",
+        dbt_snapshots_dir: str = "snapshots",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
+        execution_mode: Literal["local", "docker", "kubernetes"] = "local",
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
             "conn_id": conn_id,
         }
 
         # get the group of the dbt project
         group = render_project(
             dbt_project_name=dbt_project_name,
             dbt_root_path=dbt_root_path,
             dbt_models_dir=dbt_models_dir,
+            dbt_snapshots_dir=dbt_snapshots_dir,
             task_args=dbt_args,
+            operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             select=select,
             exclude=exclude,
+            execution_mode=execution_mode,
         )
 
         # call the airflow constructor
         super().__init__(group, *args, **kwargs)
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable, Dict, Optional, Tuple
 
+from cosmos.providers.dbt.community.profiles.exasol import (
+    create_profile_vars_exasol,
+    exasol_profile,
+)
+from cosmos.providers.dbt.community.profiles.trino import (
+    create_profile_vars_trino,
+    trino_profile,
+)
 from cosmos.providers.dbt.core.profiles.bigquery import (
     bigquery_profile,
     create_profile_vars_google_cloud_platform,
 )
 from cosmos.providers.dbt.core.profiles.databricks import (
     create_profile_vars_databricks,
     databricks_profile,
@@ -50,8 +58,14 @@
             "bigquery_profile",
             bigquery_profile,
             create_profile_vars_google_cloud_platform,
         ),
         "databricks": AdapterConfig(
             "databricks_profile", databricks_profile, create_profile_vars_databricks
         ),
+        "exasol": AdapterConfig(
+            "exasol_profile", exasol_profile, create_profile_vars_exasol
+        ),
+        "trino": AdapterConfig(
+            "trino_profile", trino_profile, create_profile_vars_trino
+        ),
     }
```

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 import pkg_resources
 import yaml
+from airflow.exceptions import AirflowNotFoundException
 from airflow.hooks.base import BaseHook
 
 from cosmos.providers.dbt.core.profiles import get_available_adapters
 
 logger = logging.getLogger(__name__)
 
 
@@ -61,7 +62,15 @@
         return adapters[connection_type].create_profile_function(
             conn, db_override, schema_override
         )
 
     logging.getLogger().setLevel(logging.ERROR)
     logging.error(f"This connection type is currently not supported {connection_type}.")
     sys.exit(1)
+
+
+def conn_exists(conn_id: str) -> bool:
+    try:
+        BaseHook().get_connection(conn_id)
+        return True
+    except AirflowNotFoundException:
+        return False
```

### Comparing `astronomer_cosmos-0.5.2/.gitignore` & `astronomer_cosmos-0.6.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/LICENSE` & `astronomer_cosmos-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/README.rst` & `astronomer_cosmos-0.6.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.5.2/pyproject.toml` & `astronomer_cosmos-0.6.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,34 +32,40 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "apache-airflow>=2.4",
+    "apache-airflow-providers-docker>=3.5.0",
+    "apache-airflow-providers-cncf-kubernetes>=5.1.1",
     "filelock",
     "Jinja2>=3.0.0",
     "typing-extensions; python_version < '3.8'",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
     "dbt-bigquery",
     "dbt-databricks",
+    "dbt-exasol",
     "dbt-postgres",
     "dbt-redshift",
     "dbt-snowflake",
     "astronomer-cosmos[dbt-openlineage]"
 ]
 dbt-bigquery = [
     "dbt-bigquery",
 ]
 dbt-databricks = [
     "dbt-databricks",
 ]
+dbt-exasol = [
+    "dbt-exasol",
+]
 dbt-postgres = [
     "dbt-postgres",
 ]
 dbt-redshift = [
     "dbt-redshift",
 ]
 dbt-snowflake = [
```

### Comparing `astronomer_cosmos-0.5.2/PKG-INFO` & `astronomer_cosmos-0.6.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.5.2
+Version: 0.6.0.dev0
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -18,31 +18,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1
+Requires-Dist: apache-airflow-providers-docker>=3.5.0
 Requires-Dist: apache-airflow>=2.4
 Requires-Dist: filelock
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
 Requires-Dist: dbt-databricks; extra == 'dbt-all'
+Requires-Dist: dbt-exasol; extra == 'dbt-all'
 Requires-Dist: dbt-postgres; extra == 'dbt-all'
 Requires-Dist: dbt-redshift; extra == 'dbt-all'
 Requires-Dist: dbt-snowflake; extra == 'dbt-all'
 Provides-Extra: dbt-bigquery
 Requires-Dist: dbt-bigquery; extra == 'dbt-bigquery'
 Provides-Extra: dbt-databricks
 Requires-Dist: dbt-databricks; extra == 'dbt-databricks'
+Provides-Extra: dbt-exasol
+Requires-Dist: dbt-exasol; extra == 'dbt-exasol'
 Provides-Extra: dbt-openlineage
 Requires-Dist: dbt-core; extra == 'dbt-openlineage'
 Requires-Dist: openlineage-dbt>=0.21.1; extra == 'dbt-openlineage'
 Provides-Extra: dbt-postgres
 Requires-Dist: dbt-postgres; extra == 'dbt-postgres'
 Provides-Extra: dbt-redshift
 Requires-Dist: dbt-redshift; extra == 'dbt-redshift'
```

