# Comparing `tmp/cloud2sql-0.8.0.tar.gz` & `tmp/cloud2sql-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2sql-0.8.0.tar", last modified: Thu Mar  9 14:25:19 2023, max compression
+gzip compressed data, was "cloud2sql-0.8.1.tar", last modified: Fri Apr 14 17:00:15 2023, max compression
```

## Comparing `cloud2sql-0.8.0.tar` & `cloud2sql-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:19.840356 cloud2sql-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-09 14:25:19.840356 cloud2sql-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:19.840356 cloud2sql-0.8.0/cloud2sql/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:19.840356 cloud2sql-0.8.0/cloud2sql/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/cloud2sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:19.840356 cloud2sql-0.8.0/cloud2sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-09 14:25:19.000000 cloud2sql-0.8.0/cloud2sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements-mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements-parquet.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements-postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements-snowflake.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-09 14:25:19.844356 cloud2sql-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-09 14:21:57.000000 cloud2sql-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.828192 cloud2sql-0.8.1/cloud2sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/cloud2sql/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/cloud2sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-parquet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-snowflake.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/setup.py
```

### Comparing `cloud2sql-0.8.0/LICENSE` & `cloud2sql-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/PKG-INFO` & `cloud2sql-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.0
+Version: 0.8.1
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `cloud2sql-0.8.0/README.md` & `cloud2sql-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/__main__.py` & `cloud2sql-0.8.1/cloud2sql/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,71 @@
 from logging import getLogger
 from typing import Optional
+
+import yaml
 from resotolib.args import Namespace, ArgumentParser
 from resotolib.logger import setup_logger
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 
+from cloud2sql import __version__
 from cloud2sql.analytics import PosthogEventSender, NoEventSender, AnalyticsEventSender
-from cloud2sql.collect_plugins import collect_from_plugins, configure
+from cloud2sql.collect_plugins import collect_from_plugins, configure, default_config
 from cloud2sql.util import db_string_from_config, check_parquet_driver
 
 # Will fail in case snowflake is not installed - which is fine.
 try:
     from cloud2sql.snowflake import SnowflakeUpdater  # noqa:F401
 except ImportError:
     pass
 
 log = getLogger("cloud2sql")
 
 
 def parse_args() -> Namespace:
     parser = ArgumentParser(
         description="Collect data from cloud providers and store it in a database",
-        epilog="Synchronizes cloud data to a database",
+        epilog="Synchronizes cloud data to a database. Visit https://cloud2sql.com for more information.",
         env_args_prefix="CLOUD2SQL_",
     )
     parser.add_argument("--debug", action="store_true", help="Enable debug logging")
-    parser.add_argument("--config", help="Path to config file", required=True)
+    parser.add_argument("--config", help="Path to config file")
     parser.add_argument(
         "--show",
         choices=["progress", "log", "none"],
         default="progress",
         help="Output to show during the process. Default: progress",
     )
     parser.add_argument(
         "--analytics-opt-out",
         default=False,
         action="store_true",
-        help="Do not send anonimized analytics data",
+        help="Do not send anonymized analytics data",
+    )
+    parser.add_argument(
+        "--version",
+        default=False,
+        action="store_true",
+        help="Print version and exit",
+    )
+    parser.add_argument(
+        "--create-config",
+        action="store_true",
+        help="Print empty configuration and exit. Use this to create your own config file.",
     )
     args = parser.parse_args()
+    if args.version:
+        print(f"Cloud2SQL Version {__version__}")
+        exit(0)
+    elif args.create_config:
+        cfg = {"sources": default_config(), "destinations": {"sqlite": {"database": "cloud2sql.db"}}}
+        print(yaml.safe_dump(cfg, sort_keys=False))
+        exit(0)
+    elif not args.config:
+        parser.error("The following arguments are required: --config")
     args.log_level = "CRITICAL" if args.show != "log" else "DEBUG" if args.debug else "INFO"
     return args  # type: ignore
 
 
 def collect(engine: Optional[Engine], args: Namespace, sender: AnalyticsEventSender) -> None:
     try:
         collect_from_plugins(engine, args, sender)
@@ -55,15 +78,15 @@
     args = parse_args()
     sender: Optional[AnalyticsEventSender] = None
     try:
         setup_logger("resoto.cloud2sql", level=args.log_level, force=True)
         sender = NoEventSender() if args.analytics_opt_out else PosthogEventSender()
         config = configure(args.config)
         engine = None
-        if config["destinations"].keys() & set(["file", "s3", "gcs"]):
+        if config["destinations"].keys() & {"file", "s3", "gcs"}:
             check_parquet_driver()
         else:
             engine = create_engine(db_string_from_config(config))
         collect(engine, args, sender)
     except Exception as e:
         if args.debug:  # raise exception and show complete tracelog
             raise e
```

### Comparing `cloud2sql-0.8.0/cloud2sql/analytics.py` & `cloud2sql-0.8.1/cloud2sql/analytics.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/arrow/config.py` & `cloud2sql-0.8.1/cloud2sql/arrow/config.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/arrow/model.py` & `cloud2sql-0.8.1/cloud2sql/arrow/model.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/arrow/type_converter.py` & `cloud2sql-0.8.1/cloud2sql/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/arrow/writer.py` & `cloud2sql-0.8.1/cloud2sql/arrow/writer.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/collect_plugins.py` & `cloud2sql-0.8.1/cloud2sql/collect_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from resotoclient import Kind, Model
 from resotolib.args import Namespace
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import BaseResource, EdgeType
 from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.model_export import node_to_dict
-from resotolib.json import from_json
+from resotolib.json import from_json, to_json
 from resotolib.proc import emergency_shutdown
 from resotolib.types import Json
 from rich import print as rich_print
 from rich.live import Live
 from sqlalchemy.engine import Engine
 import re
 
@@ -41,14 +41,25 @@
 except ImportError:
     pass
 
 
 log = getLogger("resoto.cloud2sql")
 
 
+def default_config() -> Json:
+    config: Config = Config  # type: ignore
+    for entry_point in pkg_resources.iter_entry_points("resoto.plugins"):
+        plugin_class = entry_point.load()
+        if issubclass(plugin_class, BaseCollectorPlugin):
+            plugin_class.add_config(config)
+
+    Config.init_default_config()
+    return to_json(Config.running_config.data)
+
+
 def collectors(raw_config: Json, feedback: CoreFeedback) -> Dict[str, BaseCollectorPlugin]:
     result = {}
     config: Config = Config  # type: ignore
     for entry_point in pkg_resources.iter_entry_points("resoto.plugins"):
         plugin_class = entry_point.load()
         if issubclass(plugin_class, BaseCollectorPlugin) and plugin_class.cloud in raw_config:
             log.info(f"Found collector {plugin_class.cloud} ({plugin_class.__name__})")
@@ -61,29 +72,29 @@
     Config.init_default_config()
     Config.running_config.data = {**Config.running_config.data, **Config.read_config(raw_config)}
     return result
 
 
 def configure(path_to_config: Optional[str]) -> Json:
     # at least one key should be present
-    def require(keys: List[str], obj: Json, msg: str):
+    def require(keys: List[str], obj: Json, msg: str) -> None:
         if not (set(keys) & obj.keys()):
             raise ValueError(msg)
 
     config = {}
     if path_to_config:
         with open(path_to_config) as f:
-            config = yaml.safe_load(f)  # type: ignore
+            config = yaml.safe_load(f)
 
     if "sources" not in config:
         raise ValueError("No sources configured")
     if "destinations" not in config:
         raise ValueError("No destinations configured")
 
-    def validate_arrow_config(config: Json):
+    def validate_arrow_config(config: Json) -> None:
         require(["format"], config, "No format configured for arrow destination")
         if not config["format"] in ["parquet", "csv"]:
             raise ValueError("Format must be either parquet or csv")
         require(["path", "uri"], config, "No path configured for arrow destination")
 
     destinations = set((config.get("destinations", {}) or {}).keys())
 
@@ -145,15 +156,15 @@
 
 def collect(
     collector: BaseCollectorPlugin, engine: Optional[Engine], feedback: CoreFeedback, args: Namespace, config: Json
 ) -> Tuple[str, int, int]:
     if engine:
         return collect_sql(collector, engine, feedback, args)
     else:
-        if not set(["file", "s3", "gcs"]) & config["destinations"].keys():
+        if not {"file", "s3", "gcs"} & config["destinations"].keys():
             raise ValueError("No file destination configured")
         return collect_to_file(collector, feedback, config["destinations"]["arrow"])
 
 
 def prepare_node(node: BaseResource, collector: BaseCollectorPlugin) -> Json:
     node._graph = collector.graph
     exported = node_to_dict(node)
@@ -187,15 +198,15 @@
         if key.edge_type == EdgeType.default:
             edges_by_kind.add((from_node.kind, to_node.kind))
     # create the ddl metadata from the kinds
     model.create_schema(list(edges_by_kind))
     # ingest the data
     writer = ArrowWriter(model, output_config)
     node: BaseResource
-    for node in sorted(collector.graph.nodes, key=lambda n: n.kind):
+    for node in sorted(collector.graph.nodes, key=lambda n: n.kind):  # type: ignore
         exported = prepare_node(node, collector)
         writer.insert_node(exported)
         ne_current += 1
         if ne_current % progress_update == 0:
             feedback.progress_done("sync_db", ne_current, node_edge_count, context=[collector.cloud])
     for from_node, to_node, key in collector.graph.edges:
         if key.edge_type == EdgeType.default:
```

### Comparing `cloud2sql-0.8.0/cloud2sql/schema_utils.py` & `cloud2sql-0.8.1/cloud2sql/schema_utils.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/show_progress.py` & `cloud2sql-0.8.1/cloud2sql/show_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,8 +62,8 @@
         remaining -= 1
 
         for child in dn.get("children", []):
             for nid, _ in child.items():
                 walk_node(nid, child, sub)
         return sub
 
-    return walk_node(progress.sub_tree.root, progress.sub_tree.to_dict(with_data=True))
+    return walk_node(progress.sub_tree.root, progress.sub_tree.to_dict(with_data=True))  # type: ignore
```

### Comparing `cloud2sql-0.8.0/cloud2sql/snowflake.py` & `cloud2sql-0.8.1/cloud2sql/snowflake.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql/sql.py` & `cloud2sql-0.8.1/cloud2sql/sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,96 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Any, Type, Tuple, Dict, Iterator
+from datetime import datetime, date
+from typing import List, Any, Type, Tuple, Dict, Iterator, Optional
 
 from resotoclient.models import Kind, Model
 from resotolib.args import Namespace
 from resotolib.types import Json
-from sqlalchemy import Boolean, Column, Float, Integer, JSON, MetaData, String, Table, DDL
-from sqlalchemy.engine import Engine, Connection
+from resotolib.utils import UTC_Date_Format
+from sqlalchemy import (
+    Boolean,
+    Column,
+    Float,
+    Integer,
+    JSON,
+    MetaData,
+    String,
+    Table,
+    DDL,
+    DateTime,
+    Date,
+    TypeDecorator,
+)
+from sqlalchemy.engine import Engine, Connection, Dialect
 from sqlalchemy.sql.ddl import DropTable, DropConstraint
 from sqlalchemy.sql.dml import ValuesBase
 
-from cloud2sql.util import value_in_path
 from cloud2sql.schema_utils import (
     base_kinds,
     temp_prefix,
     carz_access,
     get_table_name,
     get_link_table_name,
     kind_properties,
 )
+from cloud2sql.util import value_in_path
 
 log = logging.getLogger("resoto.cloud2sql")
 
 
+class DateTimeString(TypeDecorator):  # type: ignore
+    """
+    This type decorator translates between string (python) and datetime (sqlalchemy) types.
+    """
+
+    impl = DateTime
+    cache_ok = True
+
+    def process_bind_param(self, value: Optional[str], dialect: Dialect) -> Optional[datetime]:
+        return datetime.strptime(value, UTC_Date_Format) if value else None
+
+    def process_result_value(self, value: Optional[datetime], dialect: Dialect) -> Optional[str]:
+        return value.strftime(UTC_Date_Format) if value else None
+
+
+class DateString(TypeDecorator):  # type: ignore
+    """
+    This type decorator translates between string (python) and date (sqlalchemy) types.
+    """
+
+    impl = Date
+    cache_ok = True
+
+    def process_bind_param(self, value: Optional[str], dialect: Dialect) -> Optional[date]:
+        return date.fromisoformat(value) if value else None
+
+    def process_result_value(self, value: Optional[datetime], dialect: Dialect) -> Optional[str]:
+        return value.strftime("%Y-%m-%d") if value else None
+
+
 def sql_kind_to_column_type(kind_name: str, model: Model) -> Any:  # Type[TypeEngine[Any]]
     kind = model.kinds.get(kind_name)
     if "[]" in kind_name:
         return JSON
     elif kind_name.startswith("dict"):
         return JSON
     elif kind_name == "any":
         return JSON
     elif kind_name in ("int32", "int64"):
         return Integer
-    elif kind_name in "float":
+    elif kind_name == "float":
         return Float
-    elif kind_name in "double":
+    elif kind_name == "double":
         return Float  # use Double with sqlalchemy 2
-    elif kind_name in ("string", "date", "datetime", "duration"):
+    elif kind_name == "datetime":
+        return DateTimeString
+    elif kind_name == "date":
+        return DateString
+    elif kind_name in ("string", "duration"):
         return String
     elif kind_name == "boolean":
         return Boolean
     elif kind and kind.properties:  # complex kind
         return JSON
     elif kind and kind.runtime_kind is not None:  # refined simple type like enum
         return sql_kind_to_column_type(kind.runtime_kind, model)
```

### Comparing `cloud2sql-0.8.0/cloud2sql/util.py` & `cloud2sql-0.8.1/cloud2sql/util.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql.egg-info/PKG-INFO` & `cloud2sql-0.8.1/cloud2sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.0
+Version: 0.8.1
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `cloud2sql-0.8.0/cloud2sql.egg-info/SOURCES.txt` & `cloud2sql-0.8.1/cloud2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.0/cloud2sql.egg-info/requires.txt` & `cloud2sql-0.8.1/cloud2sql.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 SQLAlchemy==1.4.45
 PyYAML>=6.0
 rich>=12.6.0
 resotoclient>=1.2.1
 posthog>=2.2.0
 requests>=2.28.2
-resotolib<3.3,>=3.2.5
-resoto-plugin-aws<3.3,>=3.2.5
-resoto-plugin-digitalocean<3.3,>=3.2.5
-resoto-plugin-gcp<3.3,>=3.2.5
-resoto-plugin-k8s<3.3,>=3.2.5
+resotolib<3.4,>=3.3.2
+resoto-plugin-aws<3.4,>=3.3
+resoto-plugin-digitalocean<3.4,>=3.3
+resoto-plugin-gcp<3.4,>=3.3
+resoto-plugin-k8s<3.4,>=3.3
 
 [all]
 pymysql>=1.0.2
 psycopg2-binary>=2.9.5
-snowflake-sqlalchemy==1.4.6
+snowflake-sqlalchemy==1.4.7
 pyarrow==11.0.0
-google-cloud-storage==2.7.0
+google-cloud-storage==2.8.0
 boto3>=1.26.61
 
 [mariadb]
 pymysql>=1.0.2
 
 [mysql]
 pymysql>=1.0.2
 
 [parquet]
 pyarrow==11.0.0
-google-cloud-storage==2.7.0
+google-cloud-storage==2.8.0
 boto3>=1.26.61
 
 [postgresql]
 psycopg2-binary>=2.9.5
 
 [snowflake]
-snowflake-sqlalchemy==1.4.6
+snowflake-sqlalchemy==1.4.7
```

### Comparing `cloud2sql-0.8.0/setup.py` & `cloud2sql-0.8.1/setup.py`

 * *Files identical despite different names*

