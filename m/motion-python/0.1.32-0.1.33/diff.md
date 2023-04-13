# Comparing `tmp/motion_python-0.1.32.tar.gz` & `tmp/motion_python-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.32.tar", max compression
+gzip compressed data, was "motion_python-0.1.33.tar", max compression
```

## Comparing `motion_python-0.1.32.tar` & `motion_python-0.1.33.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3232 2023-04-12 05:57:39.812966 motion_python-0.1.32/README.md
--rw-r--r--   0        0        0      641 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/__init__.py
--rw-r--r--   0        0        0     6684 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/models.py
--rw-r--r--   0        0        0     2618 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/cli.py
--rw-r--r--   0        0        0    10092 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/client.py
--rw-r--r--   0        0        0    21621 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/cursor.py
--rw-r--r--   0        0        0     8664 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1348 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/schema.py
--rw-r--r--   0        0        0    14909 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/task.py
--rw-r--r--   0        0        0     5977 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/utils.py
--rw-r--r--   0        0        0     1544 2023-04-12 05:58:06.745106 motion_python-0.1.32/pyproject.toml
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 motion_python-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0     3232 2023-04-13 22:15:59.213348 motion_python-0.1.33/README.md
+-rw-r--r--   0        0        0      671 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/__init__.py
+-rw-r--r--   0        0        0     6684 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/models.py
+-rw-r--r--   0        0        0     3776 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/cli.py
+-rw-r--r--   0        0        0    10092 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/client.py
+-rw-r--r--   0        0        0    22271 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/cursor.py
+-rw-r--r--   0        0        0     9604 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1377 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/schema.py
+-rw-r--r--   0        0        0    14740 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/task.py
+-rw-r--r--   0        0        0     6058 2023-04-13 22:15:59.221348 motion_python-0.1.33/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-13 22:15:59.221348 motion_python-0.1.33/motion/utils.py
+-rw-r--r--   0        0        0     1578 2023-04-13 22:16:22.481694 motion_python-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 motion_python-0.1.33/PKG-INFO
```

### Comparing `motion_python-0.1.32/README.md` & `motion_python-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/__init__.py` & `motion_python-0.1.33/motion/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     init,
     serve,
     connect,
     test,
     create_token,
     create_app,
     create_example_app,
+    get_logs,
 )
 from motion.routing import Route
 from motion.utils import update_params
 from motion.client import ClientConnection
 from motion.cursor import Cursor
 from motion.utils import TriggerElement
 
@@ -26,8 +27,9 @@
     "update_params",
     "ClientConnection",
     "create_token",
     "create_app",
     "create_example_app",
     "Cursor",
     "TriggerElement",
+    "get_logs",
 ]
```

### Comparing `motion_python-0.1.32/motion/api/api.py` & `motion_python-0.1.33/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/api/models.py` & `motion_python-0.1.33/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/cli.py` & `motion_python-0.1.33/motion/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import shutil
 
 import click
+from rich.console import Console
+from rich.table import Table
 
 import motion
 
 
 @click.group()
 def motioncli() -> None:
     pass
@@ -94,7 +96,41 @@
 
 
 @motioncli.command("token", help="Generate a new API token")
 def token() -> None:
     """Generate a new API token."""
     token = motion.create_token()
     click.echo(token)
+
+
+@motioncli.command("logs", help="Show logs for a Motion application")
+@click.argument("name", required=True)
+@click.option(
+    "session_id",
+    "--session-id",
+    help="Session ID to show logs for.",
+    default="",
+)
+@click.option("limit", "--limit", help="Limit number of logs to show.", default=100)
+def logs(name: str, session_id: str, limit: int) -> None:
+    """Show logs for a Motion application."""
+    # Read logs
+    log_table = motion.get_logs(name, session_id=session_id)
+    log_table = log_table.tail(limit)
+
+    # create a Rich table and add columns
+    console = Console()
+    table = Table(show_header=True, header_style="bold magenta")
+    for column_name in log_table.columns:
+        if "trigger_" in column_name:
+            table.add_column(column_name.replace("trigger_", ""))
+        else:
+            table.add_column(column_name)
+
+    # add rows to the Rich table
+    for _, row in log_table.iterrows():
+        table.add_row(
+            *[str(row[column_name]) for column_name in log_table.columns],
+        )
+
+    # print the Rich table
+    console.print(table)
```

### Comparing `motion_python-0.1.32/motion/client.py` & `motion_python-0.1.33/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/cursor.py` & `motion_python-0.1.33/motion/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,28 @@
                 new_row_dict.update(
                     {
                         "identifier": identifier,  # type: ignore
                         "create_at": pd.Timestamp.now(),  # type: ignore
                         "session_id": self.session_id,  # type: ignore
                     }
                 )
+
                 new_row_dict.update(key_values)
                 new_row_df = pd.DataFrame([new_row_dict])
-                new_row = pa.Table.from_pandas(new_row_df, schema=table.schema)
+
+                try:
+                    new_row = pa.Table.from_pandas(new_row_df, schema=table.schema)
+                except pa.ArrowInvalid as e:
+                    raise TypeError(
+                        f"Invalid key-value pair for relation {relation}. Make sure the values are of the correct type. Full error: {e}"
+                    )
+                except pa.ArrowTypeError as e:
+                    raise TypeError(
+                        f"Invalid key-value pair for relation {relation}. Make sure the values are of the correct type. Full error: {e}"
+                    )
 
                 # Check schemas match
                 if collections.Counter(new_row.schema.names) != collections.Counter(
                     new_row_df.columns.values
                 ):
                     raise AttributeError(
                         f"One of the keys you are trying to set is not a valid key in the relation {relation}. Please double check your keys."
@@ -214,42 +225,41 @@
         return identifier
 
     def logTriggerExecution(
         self,
         trigger_name: str,
         trigger_version: int,
         trigger_action: str,
+        trigger_action_type: str,
         trigger_context: TriggerElement,
     ) -> None:
         """Logs the execution of a trigger.
 
         Args:
             trigger_name (str): The name of the trigger.
             trigger_version (int): The version of the trigger.
-            trigger_action (str): The action of the trigger.
+            trigger_action (str): The action of the trigger (method name).
+            trigger_action_type (str): The type of action (infer or fit).
             trigger_context (TriggerElement): The element that triggered the trigger.
         """
 
         # Append to the log table
         new_row = {
             "executed_time": pd.Timestamp.now(),
             "session_id": self.session_id,
             "trigger_name": trigger_name,
             "trigger_version": trigger_version,
             "trigger_action": trigger_action,
+            "trigger_action_type": trigger_action_type,
             "relation": trigger_context.relation,
             "identifier": trigger_context.identifier,
             "trigger_key": trigger_context.key,
         }
-        new_row = pa.Table.from_pandas(
-            pd.DataFrame(new_row, index=[0]), schema=self.log_table.schema
-        )
-
         with self.write_lock:
-            self.log_table = pa.concat_tables([self.log_table, new_row])
+            self.log_table.loc[len(self.log_table)] = pd.Series(new_row)
 
     def executeTrigger(
         self,
         *,
         trigger: TriggerFn,
         trigger_context: TriggerElement,
         triggers_to_run_on_duplicate: typing.Dict[TriggerFn, TriggerElement] = {},
@@ -308,15 +318,19 @@
             )
 
         # Execute the transform lifecycle: infer -> fit
         infer_context = None
         if route.infer is not None:
             infer_context = route.infer(new_connection, trigger_context)
             self.logTriggerExecution(
-                trigger_name, trigger_fn.version, "infer", trigger_context
+                trigger_name,
+                trigger_fn.version,
+                route.infer.__name__,
+                "INFER",
+                trigger_context,
             )
 
         # Fit is asynchronous
         if route.fit is not None:
             fit_thread = trigger_fn.fitWrapper(
                 new_connection, trigger_name, trigger_context, infer_context
             )
```

### Comparing `motion_python-0.1.32/motion/entry.py` & `motion_python-0.1.33/motion/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import shutil
 import typing
 import uuid
 
 import colorlog
+import pandas as pd
 import uvicorn
 
 from motion.api import create_fastapi_app
 from motion.client import ClientConnection
 from motion.store import Store
 from motion.utils import PRODUCTION_SESSION_ID
 
@@ -18,14 +19,42 @@
 
     Returns:
         str: The token.
     """
     return str(os.urandom(20).hex())
 
 
+def get_logs(name: str, session_id: str = "") -> pd.DataFrame:
+    """
+    Gets the log table for a given application. Can optionally filter by session ID.
+
+    Args:
+        name (str): The name of the application.
+        session_id (str, optional): The session ID to filter by. Defaults to "".
+
+    Returns:
+        pd.DataFrame: The log table.
+    """
+
+    MOTION_HOME = os.environ.get("MOTION_HOME", os.path.expanduser("~/.cache/motion"))
+    dirname = os.path.join(MOTION_HOME, "datastores", name)
+    if not os.path.exists(dirname):
+        raise KeyError(f"Application {name} does not exist.")
+
+    log_file = os.path.join(dirname, "logs.parquet")
+    if not os.path.exists(log_file):
+        raise ValueError(f"Application {name} does not have any logs.")
+
+    log_table = pd.read_parquet(log_file)
+    if session_id:
+        log_table = log_table[log_table["session_id"] == session_id]
+
+    return log_table
+
+
 def create_example_app(name: str, author: str) -> None:
     """Creates a motion app from examples."""
     name = name.strip().lower()
 
     if name == "cooking":
         # Copy the example project
         shutil.copytree(
```

### Comparing `motion_python-0.1.32/motion/examples/cooking/dashboard.py` & `motion_python-0.1.33/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/examples/cooking/test.py` & `motion_python-0.1.33/motion/examples/cooking/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,9 +36,11 @@
         as_df=True,
     ).rename(columns={"identifier": "recipe_id"})
     result = recipe_ids_and_scores.merge(recipe_ids_and_titles, on="recipe_id")
 
     print(f"Ingredient list: {ingredients}")
     print(f"Response: {result}")
 
+    connection.checkpoint()
+
 
 test_scrape()
```

### Comparing `motion_python-0.1.32/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.33/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.33/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/routing.py` & `motion_python-0.1.33/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/schema.py` & `motion_python-0.1.33/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/store.py` & `motion_python-0.1.33/motion/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import threading
 import typing
 
+import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
-import pyarrow.parquet as pq
 from croniter import croniter
 
 from motion import Schema, Trigger
 from motion.cursor import Cursor
 from motion.task import CheckpointThread, CronThread
 from motion.utils import TriggerFn, logger
 
@@ -42,15 +42,15 @@
         # Try loading from checkpoint
         (
             self.relations,
             self.table_columns,
             self.log_table,
         ) = self.loadFromCheckpoint_pa()
         if self.log_table is None:
-            self.addLogTable_pa()
+            self.addLogTable()
 
         # Set up triggers
         self.triggers: typing.Dict[str, list[TriggerFn]] = {}
         self.cron_triggers: typing.Dict[str, list[TriggerFn]] = {}
         self.cron_threads: typing.Dict[str, CronThread] = {}
         self.trigger_names: typing.Dict[str, list[str]] = {}
         self.trigger_fns: typing.Dict[str, Trigger] = {}
@@ -99,26 +99,29 @@
                     pa.schema([("session_id", pa.string())]), flavor="hive"
                 ),
                 existing_data_behavior="delete_matching",
                 schema=self.relations[relation].schema,
             )
 
         # Save logs
-        pq.write_table(self.log_table, os.path.join(base_path, "logs.parquet"))
+        self.log_table.to_parquet(os.path.join(base_path, "logs.parquet"))
 
         # TODO: checkpoint trigger objects
 
     def loadFromCheckpoint_pa(self) -> tuple[dict, dict, pa.Table]:
         """Load store object from checkpoint."""
+        # Check if log table exists
+        base_path = os.path.join(self.datastore_prefix, self.name)
+        if not os.path.exists(os.path.join(base_path, "logs.parquet")):
+            return {}, {}, None
+
         try:
             relations = {}
             table_columns = {}
 
-            base_path = os.path.join(self.datastore_prefix, self.name)
-
             # Iterate through all folders in base_path
             for relation in os.listdir(base_path):
                 if relation == "logs.parquet":
                     continue
 
                 dataset = ds.dataset(
                     os.path.join(base_path, relation),
@@ -143,47 +146,44 @@
                 table_columns[relation].remove("derived_id")
 
                 logger.info(
                     f"Loaded relation {relation} from checkpoint with {table.num_rows} existing rows in session."
                 )
 
             # Load logs
-            log_table = pq.read_table(os.path.join(base_path, "logs.parquet"))
+            # log_table = pq.read_table(os.path.join(base_path, "logs.parquet"))
+            log_table = pd.read_parquet(os.path.join(base_path, "logs.parquet"))
 
             return relations, table_columns, log_table
 
         except Exception as e:
             logger.warning(
                 f"Could not load database {self.name} from checkpoint. Error: {e}"
             )
             return {}, {}, None
 
         # TODO: load trigger objects
 
-    def addLogTable_pa(self) -> None:
+    def addLogTable(self) -> None:
         """Creates a table to store trigger logs."""
 
-        schema = pa.schema(
-            [
-                pa.field(
-                    "executed_time",
-                    pa.timestamp("us"),
-                    nullable=False,
-                ),
-                pa.field("session_id", pa.string(), nullable=False),
-                pa.field("trigger_name", pa.string(), nullable=False),
-                pa.field("trigger_version", pa.int64(), nullable=False),
-                pa.field("trigger_action", pa.string(), nullable=False),
-                pa.field("relation", pa.string(), nullable=False),
-                pa.field("identifier", pa.string(), nullable=False),
-                pa.field("trigger_key", pa.string(), nullable=False),
-            ]
+        schema = {
+            "executed_time": "datetime64[ns]",
+            "session_id": "string",
+            "trigger_name": "string",
+            "trigger_version": "int64",
+            "trigger_action": "string",
+            "trigger_action_type": "string",
+            "relation": "string",
+            "identifier": "string",
+            "trigger_key": "string",
+        }
+        self.log_table = pd.DataFrame(
+            {col: pd.Series(dtype=dtype) for col, dtype in schema.items()}
         )
-        # Create table with schema
-        self.log_table = schema.empty_table()
 
     def addrelation_pa(self, name: str, schema: Schema) -> None:
         """_Add a relation to the store.
 
         Args:
             name (str): The name of the relation.
             schema (motion.Schema): The schema of the relation.
@@ -274,22 +274,20 @@
                     )
 
                 cron_key_exists = True
 
         # Add the trigger to the store
         self.trigger_names[name] = keys
 
-        version = pc.max(
-            pc.filter(
-                self.log_table["trigger_version"],
-                pc.equal(self.log_table["trigger_name"], name),
-            )
-        ).as_py()
+        version = self.log_table[self.log_table["trigger_name"] == name][
+            "trigger_version"
+        ].max()
 
-        version = version if version is not None else 0
+        if pd.isnull(version):
+            version = 0
 
         trigger_exec = trigger(
             self.cursor(bypass_listening=True), name, version, params
         )
         self.trigger_fns[name] = trigger_exec
 
         for full_key in keys:
```

### Comparing `motion_python-0.1.32/motion/task.py` & `motion_python-0.1.33/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/motion/trigger.py` & `motion_python-0.1.33/motion/trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,16 @@
                 cursor,
                 trigger_name,
                 trigger_context,
                 infer_context,
                 fit_event,
             ) = self._fit_queue.get()
 
-            new_state = self.route_map[
-                f"{trigger_context.relation}.{trigger_context.key}"
-            ].fit(cursor, trigger_context, infer_context)
+            route = self.route_map[f"{trigger_context.relation}.{trigger_context.key}"]
+            new_state = route.fit(cursor, trigger_context, infer_context)
 
             if not isinstance(new_state, dict):
                 fit_event.set()
                 raise TypeError(
                     f"fit() of trigger {self.name} should return a dict of state updates."
                 )
 
@@ -169,15 +168,19 @@
             self.update(new_state)
 
             logger.info(
                 f"Finished running trigger {trigger_name} for identifier {trigger_context.identifier} and key {trigger_context.key}."
             )
 
             cursor.logTriggerExecution(
-                trigger_name, old_version, "fit", trigger_context
+                trigger_name,
+                old_version,
+                route.fit.__name__,
+                "FIT",
+                trigger_context,
             )
 
             fit_event.set()
 
     def fitWrapper(
         self,
         cursor: Cursor,
```

### Comparing `motion_python-0.1.32/motion/utils.py` & `motion_python-0.1.33/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.32/pyproject.toml` & `motion_python-0.1.33/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.32"
+version = "0.1.33"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -18,14 +18,16 @@
 numpy = "^1.24.2"
 requests = "^2.28.2"
 uvicorn = "^0.21.1"
 httpx = "^0.23.3"
 python-multipart = "^0.0.6"
 pydantic = "^1.10.7"
 urllib3 = "^1.26.15"
+flask = "^2.2.3"
+rich = "^13.3.4"
 
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
```

### Comparing `motion_python-0.1.32/PKG-INFO` & `motion_python-0.1.33/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.32
+Version: 0.1.33
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Motion
 
 [![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
```

