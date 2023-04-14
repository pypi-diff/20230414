# Comparing `tmp/motion_python-0.1.33.tar.gz` & `tmp/motion_python-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.33.tar", max compression
+gzip compressed data, was "motion_python-0.1.34.tar", max compression
```

## Comparing `motion_python-0.1.33.tar` & `motion_python-0.1.34.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3232 2023-04-13 22:15:59.213348 motion_python-0.1.33/README.md
--rw-r--r--   0        0        0      671 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/__init__.py
--rw-r--r--   0        0        0     6684 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/api/models.py
--rw-r--r--   0        0        0     3776 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/cli.py
--rw-r--r--   0        0        0    10092 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/client.py
--rw-r--r--   0        0        0    22271 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/cursor.py
--rw-r--r--   0        0        0     9604 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1377 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/schema.py
--rw-r--r--   0        0        0    14740 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-13 22:15:59.217348 motion_python-0.1.33/motion/task.py
--rw-r--r--   0        0        0     6058 2023-04-13 22:15:59.221348 motion_python-0.1.33/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-13 22:15:59.221348 motion_python-0.1.33/motion/utils.py
--rw-r--r--   0        0        0     1578 2023-04-13 22:16:22.481694 motion_python-0.1.33/pyproject.toml
--rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 motion_python-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0     3232 2023-04-14 05:05:49.085532 motion_python-0.1.34/README.md
+-rw-r--r--   0        0        0      671 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/__init__.py
+-rw-r--r--   0        0        0     6684 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/models.py
+-rw-r--r--   0        0        0     3776 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/cli.py
+-rw-r--r--   0        0        0    10092 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/client.py
+-rw-r--r--   0        0        0    22271 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/cursor.py
+-rw-r--r--   0        0        0    10037 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1377 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/schema.py
+-rw-r--r--   0        0        0    15114 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/task.py
+-rw-r--r--   0        0        0     6058 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/utils.py
+-rw-r--r--   0        0        0     1578 2023-04-14 05:06:10.133161 motion_python-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 motion_python-0.1.34/PKG-INFO
```

### Comparing `motion_python-0.1.33/README.md` & `motion_python-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/__init__.py` & `motion_python-0.1.34/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/api/api.py` & `motion_python-0.1.34/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/api/models.py` & `motion_python-0.1.34/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/cli.py` & `motion_python-0.1.34/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/client.py` & `motion_python-0.1.34/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/cursor.py` & `motion_python-0.1.34/motion/cursor.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/entry.py` & `motion_python-0.1.34/motion/entry.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,21 +102,23 @@
             .read()
             .replace("{0}", name)
             .replace("{1}", author)
         )
 
 
 def init(
-    mconfig: dict, disable_cron_triggers: bool = False, session_id: str = ""
+    mconfig: dict,
+    disable_triggers: typing.List[str] = [],
+    session_id: str = "",
 ) -> Store:
     """Initializes a motion application by creating a data store and adding relations and triggers.
 
     Args:
         mconfig (dict): The motion configuration.
-        disable_cron_triggers (bool, optional): Whether to disable cron triggers. Used during testing. Defaults to False.
+        disable_triggers (typing.List[str], optional): A list of triggers to disable. Defaults to [].
         prod (bool, optional): Whether to run in production mode. Defaults to False.
 
     Returns:
         Store: The motion store.
     """
     # TODO(shreyashankar): use version to check for updates when
     # needing to reinit
@@ -130,20 +132,28 @@
     checkpoint = mconfig["checkpoint"] if "checkpoint" in mconfig else "0 * * * *"
 
     if session_id == "":
         session_id = str(uuid.uuid4())
 
     MOTION_HOME = os.environ.get("MOTION_HOME", os.path.expanduser("~/.cache/motion"))
 
+    # Check that disabled triggers exist
+    all_trigger_names = [t.__name__ for t in mconfig["triggers"]]
+    for trigger_name in disable_triggers:
+        if trigger_name not in all_trigger_names:
+            raise ValueError(
+                f"Trigger {trigger_name} specified in disable_triggers list does not exist."
+            )
+
     store = Store(
         name,
         session_id=session_id,
         datastore_prefix=os.path.join(MOTION_HOME, "datastores"),
         checkpoint=checkpoint,
-        disable_cron_triggers=disable_cron_triggers,
+        disable_triggers=disable_triggers,
     )
 
     # Create relations
     for relation in mconfig["relations"]:
         store.addrelation_pa(relation.__name__, relation)
 
     # Create triggers
@@ -205,37 +215,39 @@
     logger.addHandler(handler)
     logger.setLevel(level)
 
 
 def test(
     mconfig: dict,
     wait_for_triggers: typing.List[str] = [],
-    disable_cron_triggers: bool = False,
+    disable_triggers: typing.List[str] = [],
     motion_logging_level: str = "WARNING",
     session_id: str = "",
 ) -> ClientConnection:
     """Creates a test connection to a Motion application, defined by a mconfig. This will run the application and then shut it down when the connection goes out of scope. Uses the MOTION_API_TOKEN environment variable to authenticate.
 
     Args:
         mconfig (dict): Config for the Motion application, found in the mconfig.py file.
         wait_for_triggers (typing.List[str], optional): List of cron-scheduled trigger names to wait for a first completion of. Typically used to wait for a first scrape of data.
-        disable_cron_triggers (bool, optional): Whether cron triggers should be disabled for this session (can speed up testing some non-cron triggers). Defaults to False. Cannot be True if wait_for_triggers is not empty.
+        disable_triggers (typing.List[str], optional): List of cron-scheduled trigger names to disable. Typically used to disable scrapes of data.
         motion_logging_level (str, optional): Logging level for motion. Can be one of "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL". Defaults to "WARNING". Use "INFO" if you want to see all trigger execution logs.
         session_id (str, optional): Session ID to use for this connection. Defaults to a random UUID if empty.
 
     Returns:
         connection (motion.ClientConnection): A cannection to the Motion application.
     """
-    if wait_for_triggers and disable_cron_triggers:
-        raise ValueError("Cannot wait for triggers if cron triggers are disabled.")
+    if len(set(wait_for_triggers).intersection(set(disable_triggers))) > 0:
+        raise ValueError(
+            f"Cannot wait for triggers that are disabled. Please remove the following triggers from either the wait_for_triggers or disable_triggers lists: {set(wait_for_triggers).intersection(set(disable_triggers))}"
+        )
 
     configureLogging(motion_logging_level)
     store = init(
         mconfig,
-        disable_cron_triggers=disable_cron_triggers,
+        disable_triggers=disable_triggers,
         session_id=session_id,
     )
     app = create_fastapi_app(store, testing=True)
 
     connection = ClientConnection(
         mconfig["application"]["name"],
         server=app,
```

### Comparing `motion_python-0.1.33/motion/examples/cooking/dashboard.py` & `motion_python-0.1.34/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/examples/cooking/test.py` & `motion_python-0.1.34/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.34/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.34/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/routing.py` & `motion_python-0.1.34/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/schema.py` & `motion_python-0.1.34/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/store.py` & `motion_python-0.1.34/motion/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 class Store:
     def __init__(
         self,
         name: str,
         session_id: str,
         datastore_prefix: str = "datastores",
         checkpoint: str = "0 * * * *",
-        disable_cron_triggers: bool = False,
+        disable_triggers: typing.List[str] = [],
     ) -> None:
         self.name = name
         self.session_id: str = session_id
 
         self.datastore_prefix = datastore_prefix
         self.checkpoint_interval = checkpoint
-        self.disable_cron_triggers = disable_cron_triggers
+        self.disable_triggers = disable_triggers
 
         # Set listening to false
         self._listening = False
 
         # self.con = duckdb.connect(":memory:")
         if not os.path.exists(os.path.join(datastore_prefix, self.name)):
             os.makedirs(os.path.join(datastore_prefix, self.name))
@@ -48,15 +48,15 @@
         if self.log_table is None:
             self.addLogTable()
 
         # Set up triggers
         self.triggers: typing.Dict[str, list[TriggerFn]] = {}
         self.cron_triggers: typing.Dict[str, list[TriggerFn]] = {}
         self.cron_threads: typing.Dict[str, CronThread] = {}
-        self.trigger_names: typing.Dict[str, list[str]] = {}
+        self.trigger_names_to_keys: typing.Dict[str, list[str]] = {}
         self.trigger_fns: typing.Dict[str, Trigger] = {}
 
     def __del__(self) -> None:
         self.stop(wait=False)
 
     @property
     def listening(self) -> bool:
@@ -240,15 +240,21 @@
             name (str): Trigger name.
             trigger (Trigger): Trigger class to execute when trigger is fired. Must implement the Trigger interface.
             params (typing.Dict[str, typing.Any], optional): Parameters to pass
 
         Raises:
             ValueError: If there is already a trigger with the given name.
         """
-        if name in self.trigger_names:
+        if name in self.disable_triggers:
+            logger.warning(
+                f"Trigger {name} is disabled for this session. Doing nothing."
+            )
+            return
+
+        if name in self.trigger_names_to_keys:
             logger.warning(f"Trigger {name} already exists. Doing nothing.")
             return
 
         # Check that the class implements the Trigger interface
         if not issubclass(trigger, Trigger):
             raise ValueError(f"Trigger class must implement the Trigger interface.")
 
@@ -272,15 +278,15 @@
                     raise ValueError(
                         f"Trigger {name} has more than one cron key. Only one cron key is allowed per trigger."
                     )
 
                 cron_key_exists = True
 
         # Add the trigger to the store
-        self.trigger_names[name] = keys
+        self.trigger_names_to_keys[name] = keys
 
         version = self.log_table[self.log_table["trigger_name"] == name][
             "trigger_version"
         ].max()
 
         if pd.isnull(version):
             version = 0
@@ -304,30 +310,30 @@
 
     def deleteTrigger(self, name: str) -> None:
         """Delete a trigger from the store.
 
         Args:
             name (str): The name of the trigger.
         """
-        if name not in self.trigger_names:
+        if name not in self.trigger_names_to_keys:
             raise ValueError(f"Trigger {name} does not exist.")
 
         # Remove the trigger from the store
-        keys = self.trigger_names[name]
+        keys = self.trigger_names_to_keys[name]
         fn = self.trigger_fns[name]
         for key in keys:
             if croniter.is_valid(key):
                 self.cron_triggers[key].remove(TriggerFn(name, fn))
                 self.cron_threads[name].stop()
                 self.cron_threads[name].join()
 
             else:
                 self.triggers[key].remove(TriggerFn(name, fn))
 
-        del self.trigger_names[name]
+        del self.trigger_names_to_keys[name]
         del self.trigger_fns[name]
 
     def getTriggersForKey(self, relation: str, key: str) -> list[str]:
         """Get the list of triggers for a given key.
 
         Args:
             relation (str): The relation to get the triggers for.
@@ -346,51 +352,59 @@
             typing.Dict[str, typing.List[str]]: The list of triggers for all keys.
         """
         return {
             k: self.getTriggersForKey(k.split(".")[0], k.split(".")[1])
             for k in self.triggers.keys()
         }
 
+    @property
+    def trigger_names(self) -> typing.List[str]:
+        """Get the list of trigger names.
+
+        Returns:
+             typing.List[str]: The list of trigger names.
+        """
+        return list(self.trigger_names_to_keys.keys())
+
     def start(self) -> None:
         """Start the store."""
         # Start cron triggers
         self._listening = True
         self.cron_threads = {}
 
-        if not self.disable_cron_triggers:
-            for full_key, triggers in self.cron_triggers.items():
-                _, cron_expression = full_key.split(".")
-                for trigger_fn in triggers:
-                    e = threading.Event()
-                    t = CronThread(
-                        cron_expression,
-                        self.cursor(wait_for_results=True),
-                        trigger_fn,
-                        self.checkpoint_pa,
-                        e,
-                        self.session_id,
-                    )
-                    self.cron_threads[trigger_fn.name] = t
-                    t.start()
+        for full_key, triggers in self.cron_triggers.items():
+            _, cron_expression = full_key.split(".")
+            for trigger_fn in triggers:
+                e = threading.Event()
+                t = CronThread(
+                    cron_expression,
+                    self.cursor(wait_for_results=True),
+                    trigger_fn,
+                    self.checkpoint_pa,
+                    e,
+                    self.session_id,
+                )
+                self.cron_threads[trigger_fn.name] = t
+                t.start()
 
         # Start a thread to checkpoint the store every 5 minutes
         self.checkpoint_thread = CheckpointThread(
             self.name, self.checkpoint_pa, self.checkpoint_interval
         )
         self.checkpoint_thread.start()
 
     def waitForTrigger(self, trigger_name: str) -> None:
         """Wait for a cron-scheduled trigger to fire.
 
         Args:
             trigger_name (str): The name of the trigger to wait for.
         """
-        if self.disable_cron_triggers:
+        if trigger_name in self.disable_triggers:
             raise ValueError(
-                f"Cannot wait for trigger {trigger_name} because cron triggers are disabled."
+                f"Cannot wait for trigger {trigger_name} because it is disabled."
             )
 
         if trigger_name not in self.cron_threads.keys():
             raise FileNotFoundError(
                 f"Trigger {trigger_name} does not exist as a cron-scheduled thread. Valid cron-scheduled triggers are {list(self.cron_threads.keys())}."
             )
```

### Comparing `motion_python-0.1.33/motion/task.py` & `motion_python-0.1.34/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/trigger.py` & `motion_python-0.1.34/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/motion/utils.py` & `motion_python-0.1.34/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.33/pyproject.toml` & `motion_python-0.1.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.33"
+version = "0.1.34"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.33/PKG-INFO` & `motion_python-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.33
+Version: 0.1.34
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

